# Comparing `tmp/apprise-1.4.0.tar.gz` & `tmp/apprise-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apprise-1.4.0.tar", last modified: Mon May 15 20:33:07 2023, max compression
+gzip compressed data, was "apprise-1.4.5.tar", last modified: Fri Jul  7 00:30:17 2023, max compression
```

## Comparing `apprise-1.4.0.tar` & `apprise-1.4.5.tar`

### file list

```diff
@@ -1,318 +1,322 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.301585 apprise-1.4.0/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      712 2023-05-13 16:20:00.000000 apprise-1.4.0/KEYWORDS
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1530 2023-05-12 22:30:02.000000 apprise-1.4.0/LICENSE
--rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2022-12-18 21:46:05.000000 apprise-1.4.0/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40904 2023-05-15 20:33:07.302585 apprise-1.4.0/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38862 2023-05-13 16:20:00.000000 apprise-1.4.0/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.208585 apprise-1.4.0/apprise/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    31245 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/Apprise.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/Apprise.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11489 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseAsset.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/AppriseAsset.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12778 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseAttachment.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/AppriseAttachment.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17116 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseConfig.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/AppriseConfig.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7216 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseLocale.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25284 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/URLBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/URLBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3573 2023-05-15 20:31:40.000000 apprise-1.4.0/apprise/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.210585 apprise-1.4.0/apprise/assets/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/NotifyXML-1.0.xsd
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/NotifyXML-1.1.xsd
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.201585 apprise-1.4.0/apprise/assets/themes/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.225585 apprise-1.4.0/apprise/assets/themes/default/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16135 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    41931 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2437 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7600 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-72x72.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16671 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    43331 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2485 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7875 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-72x72.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-logo.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    17446 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    48729 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2471 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7858 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-72x72.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16784 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    43708 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2472 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7913 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-72x72.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.226585 apprise-1.4.0/apprise/attachment/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13764 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/attachment/AttachBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4970 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12200 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4534 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19701 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/common.pyi
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.228585 apprise-1.4.0/apprise/config/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    45093 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/config/ConfigBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6343 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9662 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3034 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigMemory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4116 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6402 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/conversion.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/decorators/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9106 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/CustomNotifyPlugin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1692 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5316 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/notify.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/i18n/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)        0 2019-10-13 18:35:45.000000 apprise-1.4.0/apprise/i18n/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.202585 apprise-1.4.0/apprise/i18n/en/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/i18n/en/LC_MESSAGES/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      455 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise/i18n/en/LC_MESSAGES/apprise.mo
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7126 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/logger.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.245585 apprise-1.4.0/apprise/plugins/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16863 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyAppriseAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15891 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20079 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/plugins/NotifyBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12639 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBoxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16118 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBulkSMS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11434 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyClickSend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15218 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyD7Networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14662 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyDBus.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13829 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyDapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12076 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyDingTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20677 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyDiscord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38214 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyEmail.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24244 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyEmby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11703 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyEnigma2.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.245585 apprise-1.4.0/apprise/plugins/NotifyFCM/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21874 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4797 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/color.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1923 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11327 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/oauth.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8368 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/priority.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7177 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFaast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12914 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyFlock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18025 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyForm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14366 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyGitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9342 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12827 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGoogleChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10786 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14228 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGrowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3846 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGuilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10944 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyHomeAssistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13632 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyIFTTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15331 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyJSON.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13816 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyJoin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12825 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyKavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8419 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyKumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    37724 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyLametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10852 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyLine.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19632 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMQTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11785 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMSG91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23181 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMSTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8642 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMacOSX.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25396 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35187 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    43733 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMatrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12926 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12453 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMessageBird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9804 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMisskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12157 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9902 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNextcloudTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13186 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyNotica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12240 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyNotifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28308 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNtfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25262 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOffice365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18328 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOneSignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20720 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOpsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18075 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPagerDuty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14054 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPagerTree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10570 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyParsePlatform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10762 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPopcornNotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyProwl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15443 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushBullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26876 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushSafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12475 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9157 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21380 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25758 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyReddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24829 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyRocketChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11992 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyRyver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    33490 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySES.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24221 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySMSEagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19847 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySMTP2Go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24264 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySNS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16420 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySendGrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5985 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyServerChan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16844 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySignalAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11101 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifySimplePush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17018 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    41877 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySlack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    27924 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySparkPost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13624 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySpontit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16254 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyStreamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15465 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifySyslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7458 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyTechulusPush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    32361 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTelegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16181 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28986 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    30048 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12768 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyVoipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13636 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyVonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9369 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyWebexTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8846 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyWindows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12301 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyXBMC.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17127 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyXML.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13930 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyZulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20913 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/py.typed
--rw-r--r--   0 l2g       (1000) l2g       (1000)    57545 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/utils.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.209585 apprise-1.4.0/apprise.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40904 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9213 2023-05-15 20:33:07.000000 apprise-1.4.0/apprise.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       46 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/top_level.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2022-12-19 22:58:15.000000 apprise-1.4.0/dev-requirements.txt
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.246585 apprise-1.4.0/packaging/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.246585 apprise-1.4.0/packaging/man/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8306 2023-02-17 23:21:59.000000 apprise-1.4.0/packaging/man/apprise.1
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7785 2023-05-13 02:23:07.000000 apprise-1.4.0/packaging/man/apprise.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.248585 apprise-1.4.0/packaging/redhat/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1554 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-click67-support.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      524 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-no-macosx-testing.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      837 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12476 2023-05-15 20:32:18.000000 apprise-1.4.0/packaging/redhat/python-apprise.spec
--rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2022-12-19 22:58:15.000000 apprise-1.4.0/requirements.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      842 2023-05-15 20:33:07.302585 apprise-1.4.0/setup.cfg
--rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4542 2023-05-15 20:31:30.000000 apprise-1.4.0/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.294585 apprise-1.4.0/test/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2159 2023-05-12 22:30:02.000000 apprise-1.4.0/test/conftest.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.295585 apprise-1.4.0/test/helpers/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1823 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2692 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/module.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20392 2023-05-13 02:23:07.000000 apprise-1.4.0/test/helpers/rest.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    65226 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12791 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_attachments.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    41102 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_config.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    98018 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_utils.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3850 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3629 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8696 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16131 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38417 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    32106 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4317 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10987 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2563 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_memory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5204 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_conversion.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15782 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_decorator_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7800 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_escapes.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6828 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_locale.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14566 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13351 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_notify_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9886 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_apprise_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5479 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_bark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6375 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_boxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7485 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_bulksms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3563 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_clicksend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15886 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_form.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9598 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_json.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11978 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_xml.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7691 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_d7networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8239 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_dapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4185 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_dingtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17508 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_discord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    54366 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_email.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14726 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_emby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6293 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_enigma2.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3183 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_faast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    31528 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_fcm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6513 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_flock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9429 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17909 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_glib.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12515 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6526 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_google_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6620 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12895 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_growl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6775 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_guilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5438 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_homeassistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6966 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ifttt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7653 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_join.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4431 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_kavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4268 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_kumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_lametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3560 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_line.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7906 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_macosx.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14877 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_mailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25170 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_mastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28712 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_matrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5145 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_mattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4780 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_messagebird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4018 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_misskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14403 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_mqtt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5279 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_msg91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24031 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_msteams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5641 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_nextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5367 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_nextcloudtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5284 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_notica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4581 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_notifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19775 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ntfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12600 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_office365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8154 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_onesignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7644 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_opsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5148 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pagerduty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5076 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pagertree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3955 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_parse_platform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3824 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_popcorn_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6837 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_prowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13285 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushbullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7441 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3986 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15365 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9248 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushsafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14541 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_reddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11403 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_rocket_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5272 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ryver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5702 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sendgrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2915 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_serverchan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14848 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ses.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13560 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_signal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5900 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_simplepush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6451 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23392 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_slack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25763 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_smseagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8969 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_smtp2go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14499 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sns.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14377 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_sparkpost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4848 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_spontit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5241 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_streamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9643 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_syslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3266 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_techululs_push.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    34883 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_telegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8458 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16971 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35809 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7789 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_voipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8123 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_vonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4175 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_webex_teams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10991 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_windows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6700 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_xbmc_kodi.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4960 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_zulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13376 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_rest_plugins.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.299585 apprise-1.4.0/test/var/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2022-12-18 21:46:05.000000 apprise-1.4.0/test/var/01_test_example.html
--rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2022-12-19 22:58:15.000000 apprise-1.4.0/test/var/apprise-archive.zip
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    76646 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.gif
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    73667 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.jpeg
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2022-12-18 21:46:05.000000 apprise-1.4.0/test/var/apprise-test.mp4
--rw-rw-r--   0 l2g       (1000) l2g       (1000)   248280 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.301585 apprise-1.4.0/test/var/fcm/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2022-12-18 17:34:53.000000 apprise-1.4.0/test/var/fcm/service_account-bad-type.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2022-12-18 17:34:53.000000 apprise-1.4.0/test/var/fcm/service_account.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2022-12-18 17:34:53.000000 apprise-1.4.0/win-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.537908 apprise-1.4.5/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      731 2023-07-06 23:28:30.000000 apprise-1.4.5/KEYWORDS
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1530 2023-07-01 16:51:30.000000 apprise-1.4.5/LICENSE
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2023-06-03 19:32:05.000000 apprise-1.4.5/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41337 2023-07-07 00:30:17.537908 apprise-1.4.5/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    39296 2023-07-06 23:28:30.000000 apprise-1.4.5/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.512908 apprise-1.4.5/apprise/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    31245 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/Apprise.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/Apprise.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11489 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/AppriseAsset.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/AppriseAsset.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12778 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/AppriseAttachment.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/AppriseAttachment.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17116 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/AppriseConfig.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/AppriseConfig.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7216 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/AppriseLocale.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25284 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/URLBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/URLBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3573 2023-07-07 00:11:05.000000 apprise-1.4.5/apprise/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.513908 apprise-1.4.5/apprise/assets/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/NotifyXML-1.0.xsd
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/NotifyXML-1.1.xsd
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.509908 apprise-1.4.5/apprise/assets/themes/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.515908 apprise-1.4.5/apprise/assets/themes/default/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-failure-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16135 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-failure-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41931 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-failure-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2437 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-failure-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7600 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-failure-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-info-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16671 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-info-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43331 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-info-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2485 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-info-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7875 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-info-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-logo.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-success-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17446 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-success-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    48729 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-success-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2471 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-success-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7858 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-success-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-warning-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16784 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-warning-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43708 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-warning-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2472 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-warning-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7913 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/assets/themes/default/apprise-warning-72x72.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.516908 apprise-1.4.5/apprise/attachment/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13764 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/attachment/AttachBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/attachment/AttachBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4970 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/attachment/AttachFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12200 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/attachment/AttachHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4534 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/attachment/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19701 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/common.pyi
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.516908 apprise-1.4.5/apprise/config/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    45093 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/config/ConfigBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/config/ConfigBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6343 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/config/ConfigFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9662 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/config/ConfigHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3034 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/config/ConfigMemory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4116 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/config/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6402 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/conversion.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.517908 apprise-1.4.5/apprise/decorators/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9106 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/decorators/CustomNotifyPlugin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1692 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/decorators/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5316 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/decorators/notify.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.517908 apprise-1.4.5/apprise/i18n/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/i18n/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.509908 apprise-1.4.5/apprise/i18n/en/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.517908 apprise-1.4.5/apprise/i18n/en/LC_MESSAGES/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      457 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise/i18n/en/LC_MESSAGES/apprise.mo
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7126 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/logger.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.525908 apprise-1.4.5/apprise/plugins/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16863 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyAppriseAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15903 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyBark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20079 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/plugins/NotifyBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13157 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyBoxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16208 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyBulkSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15755 2023-07-06 23:28:30.000000 apprise-1.4.5/apprise/plugins/NotifyBurstSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11434 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyClickSend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15248 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyD7Networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14662 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyDBus.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13829 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyDapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12214 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyDingTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20677 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyDiscord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38404 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyEmail.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24244 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyEmby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11703 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyEnigma2.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.525908 apprise-1.4.5/apprise/plugins/NotifyFCM/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21874 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyFCM/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4797 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyFCM/color.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1923 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyFCM/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11402 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyFCM/oauth.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8368 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyFCM/priority.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7177 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyFaast.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12953 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyFlock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18025 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyForm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14674 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyGitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9342 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyGnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12827 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyGoogleChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10756 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyGotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14228 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyGrowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3846 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyGuilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10944 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyHomeAssistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13632 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyIFTTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15331 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyJSON.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13786 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyJoin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12825 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyKavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8419 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyKumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    37739 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyLametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10881 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyLine.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19632 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyMQTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11815 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyMSG91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23181 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyMSTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8642 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyMacOSX.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25529 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyMailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35326 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyMastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43811 2023-07-07 00:29:19.000000 apprise-1.4.5/apprise/plugins/NotifyMatrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12927 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyMattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12453 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyMessageBird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9804 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyMisskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12242 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyNextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10038 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyNextcloudTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13195 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyNotica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12240 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyNotifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27943 2023-07-06 23:28:30.000000 apprise-1.4.5/apprise/plugins/NotifyNtfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25395 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyOffice365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18358 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyOneSignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20720 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyOpsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18079 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyPagerDuty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14054 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyPagerTree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10570 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyParsePlatform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10792 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyPopcornNotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyProwl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15443 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyPushBullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26876 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyPushSafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12475 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyPushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9157 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyPushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21344 2023-07-06 23:28:30.000000 apprise-1.4.5/apprise/plugins/NotifyPushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25954 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyReddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24829 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyRocketChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12028 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyRyver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    33589 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySES.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24281 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySMSEagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19847 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifySMTP2Go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24334 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySNS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16420 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifySendGrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5984 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyServerChan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16844 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifySignalAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11081 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySimplePush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17018 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifySinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41790 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySlack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27998 2023-07-06 23:47:35.000000 apprise-1.4.5/apprise/plugins/NotifySparkPost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13594 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySpontit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16254 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyStreamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15435 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifySyslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7458 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyTechulusPush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    34561 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyTelegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16181 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyTwilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    29046 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyTwist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    30243 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyTwitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12757 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyVoipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13636 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyVonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9369 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyWebexTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20129 2023-07-06 23:28:30.000000 apprise-1.4.5/apprise/plugins/NotifyWhatsApp.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8846 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyWindows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12301 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyXBMC.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17127 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/plugins/NotifyXML.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13960 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/NotifyZulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21834 2023-07-01 21:03:44.000000 apprise-1.4.5/apprise/plugins/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.4.5/apprise/py.typed
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    57545 2023-07-01 16:51:30.000000 apprise-1.4.5/apprise/utils.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.513908 apprise-1.4.5/apprise.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41337 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9339 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       45 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-07-07 00:30:17.000000 apprise-1.4.5/apprise.egg-info/top_level.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2023-06-03 19:32:05.000000 apprise-1.4.5/dev-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.526908 apprise-1.4.5/packaging/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2023-06-03 19:32:05.000000 apprise-1.4.5/packaging/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.526908 apprise-1.4.5/packaging/man/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8409 2023-07-01 16:51:30.000000 apprise-1.4.5/packaging/man/apprise.1
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7785 2023-07-01 16:51:30.000000 apprise-1.4.5/packaging/man/apprise.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.526908 apprise-1.4.5/packaging/redhat/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1554 2023-06-03 19:32:05.000000 apprise-1.4.5/packaging/redhat/apprise-click67-support.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      524 2023-06-03 19:32:05.000000 apprise-1.4.5/packaging/redhat/apprise-no-macosx-testing.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      837 2023-06-03 19:32:05.000000 apprise-1.4.5/packaging/redhat/apprise-pytest-session_mocker-removal.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12672 2023-07-07 00:21:20.000000 apprise-1.4.5/packaging/redhat/python-apprise.spec
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2023-06-03 19:32:05.000000 apprise-1.4.5/requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      842 2023-07-07 00:30:17.538908 apprise-1.4.5/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4542 2023-07-07 00:10:51.000000 apprise-1.4.5/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.536908 apprise-1.4.5/test/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2159 2023-07-01 16:51:30.000000 apprise-1.4.5/test/conftest.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.536908 apprise-1.4.5/test/helpers/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1823 2023-07-01 16:51:30.000000 apprise-1.4.5/test/helpers/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-07-01 16:51:30.000000 apprise-1.4.5/test/helpers/asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2692 2023-07-01 16:51:30.000000 apprise-1.4.5/test/helpers/module.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20392 2023-07-01 17:00:26.000000 apprise-1.4.5/test/helpers/rest.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    65243 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12791 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_apprise_attachments.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41102 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_apprise_config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    98018 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_apprise_utils.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3850 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3629 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_attach_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8696 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_attach_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16131 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_attach_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38417 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    32106 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_config_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4317 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_config_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10987 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_config_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2563 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_config_memory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5204 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_conversion.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15782 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_decorator_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7800 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_escapes.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6828 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_locale.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14566 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13351 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_notify_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9886 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_apprise_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5479 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_bark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6633 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_plugin_boxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7485 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_bulksms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6471 2023-07-06 23:28:30.000000 apprise-1.4.5/test/test_plugin_burstsms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3563 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_clicksend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15886 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_custom_form.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9598 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_custom_json.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11978 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_custom_xml.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7691 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_d7networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8239 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_dapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4185 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_dingtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17508 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_discord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    54366 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_email.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14726 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_emby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6293 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_enigma2.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3183 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_faast.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    31528 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_fcm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6513 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_flock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9519 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_plugin_gitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17909 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_glib.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12515 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_gnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6526 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_google_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6620 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_gotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12895 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_growl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6775 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_guilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5438 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_homeassistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6966 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_ifttt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7653 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_join.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4431 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_kavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4268 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_kumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_lametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3560 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_line.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7906 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_macosx.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14877 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_mailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25260 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_plugin_mastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    28712 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_matrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5145 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_mattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4780 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_messagebird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4018 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_misskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14403 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_mqtt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5279 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_msg91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24031 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_msteams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5641 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_nextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5367 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_nextcloudtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5284 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_notica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4581 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_notifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19775 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_ntfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12600 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_office365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8154 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_onesignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7644 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_opsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5148 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pagerduty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5076 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pagertree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3955 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_parse_platform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3824 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_popcorn_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6837 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_prowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13285 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pushbullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7441 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3986 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15369 2023-07-06 23:28:30.000000 apprise-1.4.5/test/test_plugin_pushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9248 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_pushsafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14758 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_plugin_reddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11403 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_rocket_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5272 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_ryver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5702 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_sendgrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2915 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_serverchan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14848 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_ses.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13560 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_signal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5900 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_simplepush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6451 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_sinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23392 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_slack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25763 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_smseagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8969 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_smtp2go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14499 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_sns.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14377 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_sparkpost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4848 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_spontit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5241 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_streamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9643 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_syslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3266 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_techululs_push.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35338 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_telegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8458 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_twilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16971 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_twist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35932 2023-07-01 21:03:44.000000 apprise-1.4.5/test/test_plugin_twitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7789 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_voipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8123 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_vonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4175 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_webex_teams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9334 2023-07-06 23:28:30.000000 apprise-1.4.5/test/test_plugin_whatsapp.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10991 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_windows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6700 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_xbmc_kodi.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4960 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_plugin_zulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13376 2023-07-01 16:51:30.000000 apprise-1.4.5/test/test_rest_plugins.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.537908 apprise-1.4.5/test/var/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/01_test_example.html
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/apprise-archive.zip
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    76646 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/apprise-test.gif
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    73667 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/apprise-test.jpeg
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/apprise-test.mp4
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   248280 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/apprise-test.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-07-07 00:30:17.537908 apprise-1.4.5/test/var/fcm/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/fcm/service_account-bad-type.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2023-06-03 19:32:05.000000 apprise-1.4.5/test/var/fcm/service_account.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-06-03 19:32:05.000000 apprise-1.4.5/win-requirements.txt
```

### Comparing `apprise-1.4.0/KEYWORDS` & `apprise-1.4.5/KEYWORDS`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Alerts
 API
 AWS
 Boxcar
 BulkSMS
+Burst SMS
 Chat
 CLI
 ClickSend
 DAPNET
 Dbus
 Dingtalk
 Discord
@@ -81,10 +82,11 @@
 Techulus
 Telegram
 Twilio
 Twist
 Twitter
 Vonage
 Webex
+WhatsApp
 Windows
 Voipms
 XBMC
```

### Comparing `apprise-1.4.0/LICENSE` & `apprise-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/PKG-INFO` & `apprise-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.4.0
+Version: 1.4.5
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
-Keywords: Alerts API AWS Boxcar BulkSMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex Windows Voipms XBMC
-Platform: UNKNOWN
+Keywords: Alerts API AWS Boxcar BulkSMS Burst SMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex WhatsApp Windows Voipms XBMC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -150,22 +149,24 @@
 | [Spontit](https://github.com/caronc/apprise/wiki/Notify_spontit) | spontit://  | (TCP) 443   | spontit://UserID@APIKey/<br />spontit://UserID@APIKey/Channel<br />spontit://UserID@APIKey/Channel1/Channel2/ChannelN
 | [Syslog](https://github.com/caronc/apprise/wiki/Notify_syslog) | syslog://  | (UDP) 514 (_if hostname specified_) | syslog://<br />syslog://Facility<br />syslog://hostname<br />syslog://hostname/Facility
 | [Telegram](https://github.com/caronc/apprise/wiki/Notify_telegram) | tgram://  | (TCP) 443   | tgram://bottoken/ChatID<br />tgram://bottoken/ChatID1/ChatID2/ChatIDN
 | [Twitter](https://github.com/caronc/apprise/wiki/Notify_twitter) | twitter://  | (TCP) 443   | twitter://CKey/CSecret/AKey/ASecret<br/>twitter://user@CKey/CSecret/AKey/ASecret<br/>twitter://CKey/CSecret/AKey/ASecret/User1/User2/User2<br/>twitter://CKey/CSecret/AKey/ASecret?mode=tweet
 | [Twist](https://github.com/caronc/apprise/wiki/Notify_twist) | twist://  | (TCP) 443   | twist://pasword:login<br/>twist://password:login/#channel<br/>twist://password:login/#team:channel<br/>twist://password:login/#team:channel1/channel2/#team3:channel
 | [XBMC](https://github.com/caronc/apprise/wiki/Notify_xbmc) | xbmc:// or xbmcs://    | (TCP) 8080 or 443   | xbmc://hostname<br />xbmc://user@hostname<br />xbmc://user:password@hostname:port
 | [Webex Teams (Cisco)](https://github.com/caronc/apprise/wiki/Notify_wxteams) | wxteams://  | (TCP) 443   | wxteams://Token
+| [WhatsApp](https://github.com/caronc/apprise/wiki/Notify_whatsapp) | whatsapp://  | (TCP) 443   | whatsapp://AccessToken@FromPhoneID/ToPhoneNo<br/> whatsapp://Template:AccessToken@FromPhoneID/ToPhoneNo
 | [Zulip Chat](https://github.com/caronc/apprise/wiki/Notify_zulip) | zulip://  | (TCP) 443   | zulip://botname@Organization/Token<br />zulip://botname@Organization/Token/Stream<br />zulip://botname@Organization/Token/Email
 
 ## SMS Notifications
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [AWS SNS](https://github.com/caronc/apprise/wiki/Notify_sns)  | sns://   | (TCP) 443   | sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo<br/>sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo1/+PhoneNo2/+PhoneNoN<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic1/Topic2/TopicN
 | [BulkSMS](https://github.com/caronc/apprise/wiki/Notify_bulksms) | bulksms://  | (TCP) 443   | bulksms://user:password@ToPhoneNo<br/>bulksms://User:Password@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
+| [Burst SMS](https://github.com/caronc/apprise/wiki/Notify_burst_sms) | burstsms://  | (TCP) 443   | burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo<br/>burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [ClickSend](https://github.com/caronc/apprise/wiki/Notify_clicksend) | clicksend://  | (TCP) 443   | clicksend://user:pass@PhoneNo<br/>clicksend://user:pass@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DAPNET](https://github.com/caronc/apprise/wiki/Notify_dapnet) | dapnet://  | (TCP) 80   | dapnet://user:pass@callsign<br/>dapnet://user:pass@callsign1/callsign2/callsignN
 | [D7 Networks](https://github.com/caronc/apprise/wiki/Notify_d7networks) | d7sms://  | (TCP) 443   | d7sms://token@PhoneNo<br/>d7sms://token@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DingTalk](https://github.com/caronc/apprise/wiki/Notify_dingtalk)  | dingtalk://   | (TCP) 443   | dingtalk://token/<br />dingtalk://token/ToPhoneNo<br />dingtalk://token/ToPhoneNo1/ToPhoneNo2/ToPhoneNo1/
 | [Kavenegar](https://github.com/caronc/apprise/wiki/Notify_kavenegar) | kavenegar://  | (TCP) 443   | kavenegar://ApiKey/ToPhoneNo<br/>kavenegar://FromPhoneNo@ApiKey/ToPhoneNo<br/>kavenegar://ApiKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [MessageBird](https://github.com/caronc/apprise/wiki/Notify_messagebird) | msgbird://  | (TCP) 443   | msgbird://ApiKey/FromPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [MSG91](https://github.com/caronc/apprise/wiki/Notify_msg91) | msg91://  | (TCP) 443   | msg91://AuthKey/ToPhoneNo<br/>msg91://SenderID@AuthKey/ToPhoneNo<br/>msg91://AuthKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
@@ -559,9 +560,7 @@
 * ⚡ [Create Your Own Custom Notifications](https://github.com/caronc/apprise/wiki/decorator_notify)
 * 🌎 [Apprise API/Web Interface](https://github.com/caronc/apprise-api)
 * 🎉 [Showcase](https://github.com/caronc/apprise/wiki/showcase)
 
 Want to help make Apprise better?
 * 💡 [Contribute to the Apprise Code Base](https://github.com/caronc/apprise/wiki/Development_Contribution)
 * ❤️ [Sponsorship and Donations](https://github.com/caronc/apprise/wiki/Sponsors)
-
-
```

### Comparing `apprise-1.4.0/README.md` & `apprise-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,22 +118,24 @@
 | [Spontit](https://github.com/caronc/apprise/wiki/Notify_spontit) | spontit://  | (TCP) 443   | spontit://UserID@APIKey/<br />spontit://UserID@APIKey/Channel<br />spontit://UserID@APIKey/Channel1/Channel2/ChannelN
 | [Syslog](https://github.com/caronc/apprise/wiki/Notify_syslog) | syslog://  | (UDP) 514 (_if hostname specified_) | syslog://<br />syslog://Facility<br />syslog://hostname<br />syslog://hostname/Facility
 | [Telegram](https://github.com/caronc/apprise/wiki/Notify_telegram) | tgram://  | (TCP) 443   | tgram://bottoken/ChatID<br />tgram://bottoken/ChatID1/ChatID2/ChatIDN
 | [Twitter](https://github.com/caronc/apprise/wiki/Notify_twitter) | twitter://  | (TCP) 443   | twitter://CKey/CSecret/AKey/ASecret<br/>twitter://user@CKey/CSecret/AKey/ASecret<br/>twitter://CKey/CSecret/AKey/ASecret/User1/User2/User2<br/>twitter://CKey/CSecret/AKey/ASecret?mode=tweet
 | [Twist](https://github.com/caronc/apprise/wiki/Notify_twist) | twist://  | (TCP) 443   | twist://pasword:login<br/>twist://password:login/#channel<br/>twist://password:login/#team:channel<br/>twist://password:login/#team:channel1/channel2/#team3:channel
 | [XBMC](https://github.com/caronc/apprise/wiki/Notify_xbmc) | xbmc:// or xbmcs://    | (TCP) 8080 or 443   | xbmc://hostname<br />xbmc://user@hostname<br />xbmc://user:password@hostname:port
 | [Webex Teams (Cisco)](https://github.com/caronc/apprise/wiki/Notify_wxteams) | wxteams://  | (TCP) 443   | wxteams://Token
+| [WhatsApp](https://github.com/caronc/apprise/wiki/Notify_whatsapp) | whatsapp://  | (TCP) 443   | whatsapp://AccessToken@FromPhoneID/ToPhoneNo<br/> whatsapp://Template:AccessToken@FromPhoneID/ToPhoneNo
 | [Zulip Chat](https://github.com/caronc/apprise/wiki/Notify_zulip) | zulip://  | (TCP) 443   | zulip://botname@Organization/Token<br />zulip://botname@Organization/Token/Stream<br />zulip://botname@Organization/Token/Email
 
 ## SMS Notifications
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [AWS SNS](https://github.com/caronc/apprise/wiki/Notify_sns)  | sns://   | (TCP) 443   | sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo<br/>sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo1/+PhoneNo2/+PhoneNoN<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic1/Topic2/TopicN
 | [BulkSMS](https://github.com/caronc/apprise/wiki/Notify_bulksms) | bulksms://  | (TCP) 443   | bulksms://user:password@ToPhoneNo<br/>bulksms://User:Password@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
+| [Burst SMS](https://github.com/caronc/apprise/wiki/Notify_burst_sms) | burstsms://  | (TCP) 443   | burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo<br/>burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [ClickSend](https://github.com/caronc/apprise/wiki/Notify_clicksend) | clicksend://  | (TCP) 443   | clicksend://user:pass@PhoneNo<br/>clicksend://user:pass@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DAPNET](https://github.com/caronc/apprise/wiki/Notify_dapnet) | dapnet://  | (TCP) 80   | dapnet://user:pass@callsign<br/>dapnet://user:pass@callsign1/callsign2/callsignN
 | [D7 Networks](https://github.com/caronc/apprise/wiki/Notify_d7networks) | d7sms://  | (TCP) 443   | d7sms://token@PhoneNo<br/>d7sms://token@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DingTalk](https://github.com/caronc/apprise/wiki/Notify_dingtalk)  | dingtalk://   | (TCP) 443   | dingtalk://token/<br />dingtalk://token/ToPhoneNo<br />dingtalk://token/ToPhoneNo1/ToPhoneNo2/ToPhoneNo1/
 | [Kavenegar](https://github.com/caronc/apprise/wiki/Notify_kavenegar) | kavenegar://  | (TCP) 443   | kavenegar://ApiKey/ToPhoneNo<br/>kavenegar://FromPhoneNo@ApiKey/ToPhoneNo<br/>kavenegar://ApiKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [MessageBird](https://github.com/caronc/apprise/wiki/Notify_messagebird) | msgbird://  | (TCP) 443   | msgbird://ApiKey/FromPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [MSG91](https://github.com/caronc/apprise/wiki/Notify_msg91) | msg91://  | (TCP) 443   | msg91://AuthKey/ToPhoneNo<br/>msg91://SenderID@AuthKey/ToPhoneNo<br/>msg91://AuthKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
```

### Comparing `apprise-1.4.0/apprise/Apprise.py` & `apprise-1.4.5/apprise/Apprise.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/Apprise.pyi` & `apprise-1.4.5/apprise/Apprise.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseAsset.py` & `apprise-1.4.5/apprise/AppriseAsset.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseAsset.pyi` & `apprise-1.4.5/apprise/AppriseAsset.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseAttachment.py` & `apprise-1.4.5/apprise/AppriseAttachment.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseAttachment.pyi` & `apprise-1.4.5/apprise/AppriseAttachment.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseConfig.py` & `apprise-1.4.5/apprise/AppriseConfig.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseConfig.pyi` & `apprise-1.4.5/apprise/AppriseConfig.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/AppriseLocale.py` & `apprise-1.4.5/apprise/AppriseLocale.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/URLBase.py` & `apprise-1.4.5/apprise/URLBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/URLBase.pyi` & `apprise-1.4.5/apprise/URLBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/__init__.py` & `apprise-1.4.5/apprise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 __title__ = 'Apprise'
-__version__ = '1.4.0'
+__version__ = '1.4.5'
 __author__ = 'Chris Caron'
 __license__ = 'BSD'
 __copywrite__ = 'Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .common import NotifyType
```

### Comparing `apprise-1.4.0/apprise/assets/NotifyXML-1.0.xsd` & `apprise-1.4.5/apprise/assets/NotifyXML-1.0.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/NotifyXML-1.1.xsd` & `apprise-1.4.5/apprise/assets/NotifyXML-1.1.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.ico` & `apprise-1.4.5/apprise/assets/themes/default/apprise-failure-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-failure-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-256x256.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-failure-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-32x32.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-failure-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-72x72.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-failure-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.ico` & `apprise-1.4.5/apprise/assets/themes/default/apprise-info-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-info-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-info-256x256.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-info-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-info-32x32.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-info-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-info-72x72.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-info-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-logo.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-logo.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.ico` & `apprise-1.4.5/apprise/assets/themes/default/apprise-success-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-success-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-success-256x256.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-success-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-success-32x32.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-success-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-success-72x72.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-success-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.ico` & `apprise-1.4.5/apprise/assets/themes/default/apprise-warning-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-warning-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-256x256.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-warning-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-32x32.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-warning-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-72x72.png` & `apprise-1.4.5/apprise/assets/themes/default/apprise-warning-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/attachment/AttachBase.py` & `apprise-1.4.5/apprise/attachment/AttachBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/attachment/AttachBase.pyi` & `apprise-1.4.5/apprise/attachment/AttachBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/attachment/AttachFile.py` & `apprise-1.4.5/apprise/attachment/AttachFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/attachment/AttachHTTP.py` & `apprise-1.4.5/apprise/attachment/AttachHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/attachment/__init__.py` & `apprise-1.4.5/apprise/attachment/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/cli.py` & `apprise-1.4.5/apprise/cli.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/common.py` & `apprise-1.4.5/apprise/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/config/ConfigBase.py` & `apprise-1.4.5/apprise/config/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/config/ConfigFile.py` & `apprise-1.4.5/apprise/config/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/config/ConfigHTTP.py` & `apprise-1.4.5/apprise/config/ConfigHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/config/ConfigMemory.py` & `apprise-1.4.5/apprise/config/ConfigMemory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/config/__init__.py` & `apprise-1.4.5/apprise/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/conversion.py` & `apprise-1.4.5/apprise/conversion.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/decorators/CustomNotifyPlugin.py` & `apprise-1.4.5/apprise/decorators/CustomNotifyPlugin.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/decorators/__init__.py` & `apprise-1.4.5/apprise/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/decorators/notify.py` & `apprise-1.4.5/apprise/decorators/notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/logger.py` & `apprise-1.4.5/apprise/logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyAppriseAPI.py` & `apprise-1.4.5/apprise/plugins/NotifyAppriseAPI.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyBark.py` & `apprise-1.4.5/apprise/plugins/NotifyBark.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,18 @@
 
     # Allows the user to specify the NotifyImageSize object; this is supported
     # through the webhook
     image_size = NotifyImageSize.XY_128
 
     # Define object templates
     templates = (
+        '{schema}://{host}/{targets}',
         '{schema}://{host}:{port}/{targets}',
         '{schema}://{user}:{password}@{host}/{targets}',
         '{schema}://{user}:{password}@{host}:{port}/{targets}',
-        '{schema}://{user}:{password}@{host}/{targets}',
     )
 
     # Define our template arguments
     template_tokens = dict(NotifyBase.template_tokens, **{
         'host': {
             'name': _('Hostname'),
             'type': 'string',
@@ -159,14 +159,15 @@
             'name': _('Target Device'),
             'type': 'string',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyBase.py` & `apprise-1.4.5/apprise/plugins/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyBoxcar.py` & `apprise-1.4.5/apprise/plugins/NotifyBoxcar.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,14 +147,20 @@
             'type': 'bool',
             'default': True,
             'map_to': 'include_image',
         },
         'to': {
             'alias_of': 'targets',
         },
+        'access': {
+            'alias_of': 'access_key',
+        },
+        'secret': {
+            'alias_of': 'secret_key',
+        },
     })
 
     def __init__(self, access, secret, targets=None, include_image=True,
                  **kwargs):
         """
         Initialize Boxcar Object
         """
@@ -377,12 +383,22 @@
         results['targets'] = entries
 
         # The 'to' makes it easier to use yaml configuration
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'] += \
                 NotifyBoxcar.parse_list(results['qsd'].get('to'))
 
+        # Access
+        if 'access' in results['qsd'] and results['qsd']['access']:
+            results['access'] = NotifyBoxcar.unquote(
+                results['qsd']['access'].strip())
+
+        # Secret
+        if 'secret' in results['qsd'] and results['qsd']['secret']:
+            results['secret'] = NotifyBoxcar.unquote(
+                results['qsd']['secret'].strip())
+
         # Include images with our message
         results['include_image'] = \
             parse_bool(results['qsd'].get('image', True))
 
         return results
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyBulkSMS.py` & `apprise-1.4.5/apprise/plugins/NotifyBulkSMS.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,19 +117,21 @@
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'user': {
             'name': _('User Name'),
             'type': 'string',
+            'required': True,
         },
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
+            'required': True,
         },
         'target_phone': {
             'name': _('Target Phone No'),
             'type': 'string',
             'prefix': '+',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
@@ -140,14 +142,15 @@
             'prefix': '+',
             'regex': (r'^[A-Z0-9 _-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyClickSend.py` & `apprise-1.4.5/apprise/plugins/NotifyClickSend.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyD7Networks.py` & `apprise-1.4.5/apprise/plugins/NotifyD7Networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             'prefix': '+',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'unicode': {
             # Unicode characters (default is 'auto')
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyDBus.py` & `apprise-1.4.5/apprise/plugins/NotifyDBus.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyDapnet.py` & `apprise-1.4.5/apprise/plugins/NotifyDapnet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyDingTalk.py` & `apprise-1.4.5/apprise/plugins/NotifyDingTalk.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,21 +99,26 @@
             'name': _('Token'),
             'type': 'string',
             'private': True,
             'required': True,
             'regex': (r'^[a-z0-9]+$', 'i'),
         },
         'secret': {
-            'name': _('Token'),
+            'name': _('Secret'),
             'type': 'string',
             'private': True,
             'regex': (r'^[a-z0-9]+$', 'i'),
         },
-        'targets': {
+        'target_phone_no': {
             'name': _('Target Phone No'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
+        'targets': {
+            'name': _('Targets'),
             'type': 'list:string',
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyDiscord.py` & `apprise-1.4.5/apprise/plugins/NotifyDiscord.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyEmail.py` & `apprise-1.4.5/apprise/plugins/NotifyEmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from email.mime.multipart import MIMEMultipart
 from email.utils import formataddr, make_msgid
 from email.header import Header
 from email import charset
 
 from socket import error as SocketError
 from datetime import datetime
+from datetime import timezone
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyFormat, NotifyType
 from ..conversion import convert_between
 from ..utils import is_email, parse_emails
 from ..AppriseLocale import gettext_lazy as _
@@ -380,16 +381,21 @@
         },
         'port': {
             'name': _('Port'),
             'type': 'int',
             'min': 1,
             'max': 65535,
         },
+        'target_email': {
+            'name': _('Target Email'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
         'targets': {
-            'name': _('Target Emails'),
+            'name': _('Targets'),
             'type': 'list:string',
         },
     })
 
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'name': _('To Email'),
@@ -801,15 +807,16 @@
                 base[k] = Header(v, self._get_charset(v))
 
             base['Subject'] = Header(title, self._get_charset(title))
             base['From'] = formataddr(self.from_addr, charset='utf-8')
             base['To'] = formataddr((to_name, to_addr), charset='utf-8')
             base['Message-ID'] = make_msgid(domain=self.smtp_host)
             base['Date'] = \
-                datetime.utcnow().strftime("%a, %d %b %Y %H:%M:%S +0000")
+                datetime.now(timezone.utc)\
+                .strftime("%a, %d %b %Y %H:%M:%S +0000")
             base['X-Application'] = self.app_id
 
             if cc:
                 base['Cc'] = ','.join(cc)
 
             if reply_to:
                 base['Reply-To'] = ','.join(reply_to)
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyEmby.py` & `apprise-1.4.5/apprise/plugins/NotifyEmby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyEnigma2.py` & `apprise-1.4.5/apprise/plugins/NotifyEnigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFCM/__init__.py` & `apprise-1.4.5/apprise/plugins/NotifyFCM/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
             'name': _('OAuth2 KeyFile'),
             'type': 'string',
             'private': True,
         },
         'project': {
             'name': _('Project ID'),
             'type': 'string',
-            'required': True,
         },
         'target_device': {
             'name': _('Target Device'),
             'type': 'string',
             'map_to': 'targets',
         },
         'target_topic': {
@@ -169,14 +168,15 @@
             'type': 'string',
             'prefix': '#',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
         },
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFCM/color.py` & `apprise-1.4.5/apprise/plugins/NotifyFCM/color.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFCM/common.py` & `apprise-1.4.5/apprise/plugins/NotifyFCM/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFCM/oauth.py` & `apprise-1.4.5/apprise/plugins/NotifyFCM/oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from cryptography.hazmat import backends
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives import asymmetric
 from cryptography.exceptions import UnsupportedAlgorithm
 from datetime import datetime
 from datetime import timedelta
+from datetime import timezone
 from json.decoder import JSONDecodeError
 from urllib.parse import urlencode as _urlencode
 
 from ...logger import logger
 
 
 class GoogleOAuth:
@@ -102,26 +103,26 @@
 
         # Our generated key information we cache once loaded
         self.private_key = None
 
         # Our keys we build using the provided content
         self.__refresh_token = None
         self.__access_token = None
-        self.__access_token_expiry = datetime.utcnow()
+        self.__access_token_expiry = datetime.now(timezone.utc)
 
     def load(self, path):
         """
         Generate our SSL details
         """
 
         # Reset our objects
         self.content = None
         self.private_key = None
         self.__access_token = None
-        self.__access_token_expiry = datetime.utcnow()
+        self.__access_token_expiry = datetime.now(timezone.utc)
 
         try:
             with open(path, mode="r", encoding=self.encoding) as fp:
                 self.content = json.loads(fp.read())
 
         except (OSError, IOError):
             logger.debug('FCM keyfile {} could not be accessed'.format(path))
@@ -195,25 +196,25 @@
         if not self.private_key or not self.content:
             # invalid content (or not loaded)
             logger.error(
                 'No FCM JSON keyfile content loaded to generate a access '
                 'token with.')
             return None
 
-        if self.__access_token_expiry > datetime.utcnow():
+        if self.__access_token_expiry > datetime.now(timezone.utc):
             # Return our no-expired key
             return self.__access_token
 
         # If we reach here we need to prepare our payload
         token_uri = self.content.get('token_uri', self.default_token_uri)
         service_email = self.content.get('client_email')
         key_identifier = self.content.get('private_key_id')
 
         # Generate our Assertion
-        now = datetime.utcnow()
+        now = datetime.now(timezone.utc)
         expiry = now + self.access_token_lifetime_sec
 
         payload = {
             # The number of seconds since the UNIX epoch.
             "iat": calendar.timegm(now.utctimetuple()),
             "exp": calendar.timegm(expiry.utctimetuple()),
             # The issuer must be the service account email.
@@ -297,15 +298,15 @@
         self.__access_token = response['access_token']
         self.__refresh_token = response.get(
             'refresh_token', self.__refresh_token)
 
         if 'expires_in' in response:
             delta = timedelta(seconds=int(response['expires_in']))
             self.__access_token_expiry = \
-                delta + datetime.utcnow() - self.clock_skew
+                delta + datetime.now(timezone.utc) - self.clock_skew
 
         else:
             # Allow some grace before we expire
             self.__access_token_expiry = expiry - self.clock_skew
 
         logger.debug(
             'Access Token successfully acquired: %s', self.__access_token)
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFCM/priority.py` & `apprise-1.4.5/apprise/plugins/NotifyFCM/priority.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFaast.py` & `apprise-1.4.5/apprise/plugins/NotifyFaast.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyFlock.py` & `apprise-1.4.5/apprise/plugins/NotifyFlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,31 +93,32 @@
 
     # Allows the user to specify the NotifyImageSize object
     image_size = NotifyImageSize.XY_72
 
     # Define object templates
     templates = (
         '{schema}://{token}',
-        '{schema}://{user}@{token}',
-        '{schema}://{user}@{token}/{targets}',
+        '{schema}://{botname}@{token}',
+        '{schema}://{botname}@{token}/{targets}',
         '{schema}://{token}/{targets}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'token': {
             'name': _('Access Key'),
             'type': 'string',
             'regex': (r'^[a-z0-9-]+$', 'i'),
             'private': True,
             'required': True,
         },
-        'user': {
+        'botname': {
             'name': _('Bot Name'),
             'type': 'string',
+            'map_to': 'user',
         },
         'to_user': {
             'name': _('To User ID'),
             'type': 'string',
             'prefix': '@',
             'regex': (r'^[A-Z0-9_]+$', 'i'),
             'map_to': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyForm.py` & `apprise-1.4.5/apprise/plugins/NotifyForm.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGitter.py` & `apprise-1.4.5/apprise/plugins/NotifyGitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 # Official API reference: https://developer.gitter.im/docs/user-resource
 
 import re
 import requests
 from json import loads
 from json import dumps
 from datetime import datetime
+from datetime import timezone
 
 from .NotifyBase import NotifyBase
 from ..common import NotifyImageSize
 from ..common import NotifyFormat
 from ..common import NotifyType
 from ..utils import parse_list
 from ..utils import parse_bool
@@ -95,15 +96,15 @@
     # X-RateLimit-Reset: The epoc time (in seconds) we can expect our
     #                    rate-limit to be reset.
     # X-RateLimit-Remaining: an integer identifying how many requests we're
     #                        still allow to make.
     request_rate_per_sec = 0
 
     # For Tracking Purposes
-    ratelimit_reset = datetime.utcnow()
+    ratelimit_reset = datetime.now(timezone.utc).replace(tzinfo=None)
 
     # Default to 1
     ratelimit_remaining = 1
 
     # Default Notification Format
     notify_format = NotifyFormat.MARKDOWN
 
@@ -117,17 +118,23 @@
         'token': {
             'name': _('Token'),
             'type': 'string',
             'private': True,
             'required': True,
             'regex': (r'^[a-z0-9]{40}$', 'i'),
         },
+        'target_room': {
+            'name': _('Target Room'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
         'targets': {
-            'name': _('Rooms'),
+            'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'image': {
             'name': _('Include Image'),
@@ -294,15 +301,15 @@
         if self.ratelimit_remaining <= 0:
             # Determine how long we should wait for or if we should wait at
             # all. This isn't fool-proof because we can't be sure the client
             # time (calling this script) is completely synced up with the
             # Gitter server.  One would hope we're on NTP and our clocks are
             # the same allowing this to role smoothly:
 
-            now = datetime.utcnow()
+            now = datetime.now(timezone.utc).replace(tzinfo=None)
             if now < self.ratelimit_reset:
                 # We need to throttle for the difference in seconds
                 # We add 0.5 seconds to the end just to allow a grace
                 # period.
                 wait = (self.ratelimit_reset - now).total_seconds() + 0.5
 
         # Always call throttle before any remote server i/o is made
@@ -346,16 +353,17 @@
                 # TypeError = r.content is None
                 # AttributeError = r is None
                 content = {}
 
             try:
                 self.ratelimit_remaining = \
                     int(r.headers.get('X-RateLimit-Remaining'))
-                self.ratelimit_reset = datetime.utcfromtimestamp(
-                    int(r.headers.get('X-RateLimit-Reset')))
+                self.ratelimit_reset = datetime.fromtimestamp(
+                    int(r.headers.get('X-RateLimit-Reset')), timezone.utc
+                ).replace(tzinfo=None)
 
             except (TypeError, ValueError):
                 # This is returned if we could not retrieve this information
                 # gracefully accept this state and move on
                 pass
 
         except requests.RequestException as e:
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGnome.py` & `apprise-1.4.5/apprise/plugins/NotifyGnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGoogleChat.py` & `apprise-1.4.5/apprise/plugins/NotifyGoogleChat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGotify.py` & `apprise-1.4.5/apprise/plugins/NotifyGotify.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,14 @@
             'required': True,
         },
         'path': {
             'name': _('Path'),
             'type': 'string',
             'map_to': 'fullpath',
             'default': '/',
-            'required': True,
         },
         'port': {
             'name': _('Port'),
             'type': 'int',
             'min': 1,
             'max': 65535,
         },
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGrowl.py` & `apprise-1.4.5/apprise/plugins/NotifyGrowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyGuilded.py` & `apprise-1.4.5/apprise/plugins/NotifyGuilded.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyHomeAssistant.py` & `apprise-1.4.5/apprise/plugins/NotifyHomeAssistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyIFTTT.py` & `apprise-1.4.5/apprise/plugins/NotifyIFTTT.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyJSON.py` & `apprise-1.4.5/apprise/plugins/NotifyJSON.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyJoin.py` & `apprise-1.4.5/apprise/plugins/NotifyJoin.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,14 @@
                 'all', 'android', 'chrome', 'windows10', 'phone', 'tablet',
                 'pc'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
-            'required': True,
         },
     })
 
     template_args = dict(NotifyBase.template_args, **{
         'image': {
             'name': _('Include Image'),
             'type': 'bool',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyKavenegar.py` & `apprise-1.4.5/apprise/plugins/NotifyKavenegar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyKumulos.py` & `apprise-1.4.5/apprise/plugins/NotifyKumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyLametric.py` & `apprise-1.4.5/apprise/plugins/NotifyLametric.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,15 @@
     templates = (
         # Cloud (App) Mode
         '{schema}://{app_token}@{app_id}',
         '{schema}://{app_token}@{app_id}/{app_ver}',
 
         # Device Mode
         '{schema}://{apikey}@{host}',
+        '{schema}://{user}:{apikey}@{host}',
         '{schema}://{apikey}@{host}:{port}',
         '{schema}://{user}:{apikey}@{host}:{port}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         # Used for Local Device mode
@@ -400,15 +401,14 @@
             'name': _('App Access Token'),
             'type': 'string',
             'regex': (r'^[A-Z0-9]{80,}==$', 'i'),
         },
         'host': {
             'name': _('Hostname'),
             'type': 'string',
-            'required': True,
         },
         'port': {
             'name': _('Port'),
             'type': 'int',
             'min': 1,
             'max': 65535,
             'default': 8080,
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyLine.py` & `apprise-1.4.5/apprise/plugins/NotifyLine.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             'name': _('Target User'),
             'type': 'string',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMQTT.py` & `apprise-1.4.5/apprise/plugins/NotifyMQTT.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMSG91.py` & `apprise-1.4.5/apprise/plugins/NotifyMSG91.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
             'prefix': '+',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
         'sender': {
             'name': _('Sender ID'),
             'type': 'string',
         },
     })
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMSTeams.py` & `apprise-1.4.5/apprise/plugins/NotifyMSTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMacOSX.py` & `apprise-1.4.5/apprise/plugins/NotifyMacOSX.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMailgun.py` & `apprise-1.4.5/apprise/plugins/NotifyMailgun.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,21 @@
         },
         'apikey': {
             'name': _('API Key'),
             'type': 'string',
             'private': True,
             'required': True,
         },
+        'target_email': {
+            'name': _('Target Email'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
         'targets': {
-            'name': _('Target Emails'),
+            'name': _('Targets'),
             'type': 'list:string',
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'name': {
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMastodon.py` & `apprise-1.4.5/apprise/plugins/NotifyMastodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 import re
 import requests
 from copy import deepcopy
 from json import dumps, loads
 from datetime import datetime
+from datetime import timezone
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyImageSize
 from ..common import NotifyFormat
 from ..common import NotifyType
 from ..utils import parse_list
@@ -146,15 +147,15 @@
     # X-Rate-Limit-Reset: The epoc time (in seconds) we can expect our
     #                    rate-limit to be reset.
     # X-Rate-Limit-Remaining: an integer identifying how many requests we're
     #                        still allow to make.
     request_rate_per_sec = 0
 
     # For Tracking Purposes
-    ratelimit_reset = datetime.utcnow()
+    ratelimit_reset = datetime.now(timezone.utc).replace(tzinfo=None)
 
     # Default to 1000; users can send up to 1000 DM's and 2400 toot a day
     # This value only get's adjusted if the server sets it that way
     ratelimit_remaining = 1
 
     # Define object templates
     templates = (
@@ -830,15 +831,15 @@
         if self.ratelimit_remaining == 0:
             # Determine how long we should wait for or if we should wait at
             # all. This isn't fool-proof because we can't be sure the client
             # time (calling this script) is completely synced up with the
             # Mastodon server.  One would hope we're on NTP and our clocks are
             # the same allowing this to role smoothly:
 
-            now = datetime.utcnow()
+            now = datetime.now(timezone.utc).replace(tzinfo=None)
             if now < self.ratelimit_reset:
                 # We need to throttle for the difference in seconds
                 # We add 0.5 seconds to the end just to allow a grace
                 # period.
                 wait = (self.ratelimit_reset - now).total_seconds() + 0.5
 
         # Always call throttle before any remote server i/o is made;
@@ -888,16 +889,17 @@
                 # Mark our failure
                 return (False, content)
 
             try:
                 # Capture rate limiting if possible
                 self.ratelimit_remaining = \
                     int(r.headers.get('X-RateLimit-Remaining'))
-                self.ratelimit_reset = datetime.utcfromtimestamp(
-                    int(r.headers.get('X-RateLimit-Limit')))
+                self.ratelimit_reset = datetime.fromtimestamp(
+                    int(r.headers.get('X-RateLimit-Limit')), timezone.utc
+                ).replace(tzinfo=None)
 
             except (TypeError, ValueError):
                 # This is returned if we could not retrieve this information
                 # gracefully accept this state and move on
                 pass
 
         except requests.RequestException as e:
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMatrix.py` & `apprise-1.4.5/apprise/plugins/NotifyMatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'host': {
             'name': _('Hostname'),
             'type': 'string',
-            'required': True,
         },
         'port': {
             'name': _('Port'),
             'type': 'int',
             'min': 1,
             'max': 65535,
         },
@@ -190,14 +189,15 @@
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
         },
         'token': {
             'name': _('Access Token'),
+            'private': True,
             'map_to': 'password',
         },
         'target_user': {
             'name': _('Target User'),
             'type': 'string',
             'prefix': '@',
             'map_to': 'targets',
@@ -987,19 +987,19 @@
 
         if self.access_token is not None:
             headers["Authorization"] = 'Bearer %s' % self.access_token
 
         default_port = 443 if self.secure else 80
 
         url = \
-            '{schema}://{hostname}:{port}{matrix_api}{path}'.format(
+            '{schema}://{hostname}{port}{matrix_api}{path}'.format(
                 schema='https' if self.secure else 'http',
                 hostname=self.host,
                 port='' if self.port is None
-                or self.port == default_port else self.port,
+                or self.port == default_port else f':{self.port}',
                 matrix_api=MATRIX_V2_API_PATH,
                 path=path)
 
         # Our response object
         response = {}
 
         # fetch function
@@ -1027,14 +1027,15 @@
                     data=dumps(payload),
                     params=params,
                     headers=headers,
                     verify=self.verify_certificate,
                     timeout=self.request_timeout,
                 )
 
+                self.logger.debug('Matrix Response: %s' % str(r.content))
                 response = loads(r.content)
 
                 if r.status_code == 429:
                     wait = self.default_wait_ms / 1000
                     try:
                         wait = response['retry_after_ms'] / 1000
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMattermost.py` & `apprise-1.4.5/apprise/plugins/NotifyMattermost.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,19 +87,19 @@
 
     # Mattermost does not have a title
     title_maxlen = 0
 
     # Define object templates
     templates = (
         '{schema}://{host}/{token}',
-        '{schema}://{host}/{token}:{port}',
+        '{schema}://{host}:{port}/{token}',
+        '{schema}://{host}/{fullpath}/{token}',
+        '{schema}://{host}:{port}/{fullpath}/{token}',
         '{schema}://{botname}@{host}/{token}',
         '{schema}://{botname}@{host}:{port}/{token}',
-        '{schema}://{host}/{fullpath}/{token}',
-        '{schema}://{host}/{fullpath}{token}:{port}',
         '{schema}://{botname}@{host}/{fullpath}/{token}',
         '{schema}://{botname}@{host}:{port}/{fullpath}/{token}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'host': {
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMessageBird.py` & `apprise-1.4.5/apprise/plugins/NotifyMessageBird.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyMisskey.py` & `apprise-1.4.5/apprise/plugins/NotifyMisskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyNextcloud.py` & `apprise-1.4.5/apprise/plugins/NotifyNextcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     title_maxlen = 255
 
     # Defines the maximum allowable characters per message.
     body_maxlen = 4000
 
     # Define object templates
     templates = (
+        '{schema}://{host}/{targets}',
+        '{schema}://{host}:{port}/{targets}',
         '{schema}://{user}:{password}@{host}/{targets}',
         '{schema}://{user}:{password}@{host}:{port}/{targets}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'host': {
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyNextcloudTalk.py` & `apprise-1.4.5/apprise/plugins/NotifyNextcloudTalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,19 @@
         },
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
             'required': True,
         },
+        'target_room_id': {
+            'name': _('Room ID'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
             'required': True,
         },
     })
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyNotica.py` & `apprise-1.4.5/apprise/plugins/NotifyNotica.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,20 @@
         '{schema}://{host}:{port}/{token}',
         '{schema}://{user}@{host}/{token}',
         '{schema}://{user}@{host}:{port}/{token}',
         '{schema}://{user}:{password}@{host}/{token}',
         '{schema}://{user}:{password}@{host}:{port}/{token}',
 
         # Self-hosted notica servers (with custom path)
-        '{schema}://{host}{path}{token}',
-        '{schema}://{host}:{port}{path}{token}',
-        '{schema}://{user}@{host}{path}{token}',
-        '{schema}://{user}@{host}:{port}{path}{token}',
-        '{schema}://{user}:{password}@{host}{path}{token}',
-        '{schema}://{user}:{password}@{host}:{port}{path}{token}',
+        '{schema}://{host}{path}/{token}',
+        '{schema}://{host}:{port}/{path}/{token}',
+        '{schema}://{user}@{host}/{path}/{token}',
+        '{schema}://{user}@{host}:{port}{path}/{token}',
+        '{schema}://{user}:{password}@{host}{path}/{token}',
+        '{schema}://{user}:{password}@{host}:{port}/{path}/{token}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'token': {
             'name': _('Token'),
             'type': 'string',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyNotifico.py` & `apprise-1.4.5/apprise/plugins/NotifyNotifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyNtfy.py` & `apprise-1.4.5/apprise/plugins/NotifyNtfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,18 +449,14 @@
         """
 
         # Prepare our headers
         headers = {
             'User-Agent': self.app_id,
         }
 
-        # Some default values for our request object to which we'll update
-        # depending on what our payload is
-        files = None
-
         # See https://ntfy.sh/docs/publish/#publish-as-json
         data = {}
 
         # Posting Parameters
         params = {}
 
         auth = None
@@ -490,19 +486,31 @@
 
         if not attach:
             headers['Content-Type'] = 'application/json'
 
             data['topic'] = topic
             virt_payload = data
 
+            if self.attach:
+                virt_payload['attach'] = self.attach
+
+                if self.filename:
+                    virt_payload['filename'] = self.filename
+
         else:
             # Point our payload to our parameters
             virt_payload = params
             notify_url += '/{topic}'.format(topic=topic)
 
+            # Prepare our Header
+            virt_payload['filename'] = attach.name
+
+            with open(attach.path, 'rb') as fp:
+                data = fp.read()
+
         if image_url:
             headers['X-Icon'] = image_url
 
         if title:
             virt_payload['title'] = title
 
         if body:
@@ -519,45 +527,38 @@
 
         if self.email is not None:
             headers['X-Email'] = self.email
 
         if self.__tags:
             headers['X-Tags'] = ",".join(self.__tags)
 
-        if isinstance(attach, AttachBase):
-            # Prepare our Header
-            params['filename'] = attach.name
-
-            # prepare our files object
-            files = {'file': (attach.name, open(attach.path, 'rb'))}
-
-        elif self.attach is not None:
-            data['attach'] = self.attach
-            if self.filename is not None:
-                data['filename'] = self.filename
-
         self.logger.debug('ntfy POST URL: %s (cert_verify=%r)' % (
             notify_url, self.verify_certificate,
         ))
         self.logger.debug('ntfy Payload: %s' % str(virt_payload))
         self.logger.debug('ntfy Headers: %s' % str(headers))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         # Default response type
         response = None
 
+        if data:
+            data = data if attach else dumps(data)
+
+        else:  # not data:
+            data = None
+
         try:
             r = requests.post(
                 notify_url,
                 params=params if params else None,
-                data=dumps(data) if data else None,
+                data=data,
                 headers=headers,
-                files=files,
                 auth=auth,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
 
             if r.status_code != requests.codes.ok:
                 # We had a problem
@@ -604,29 +605,23 @@
 
         except requests.RequestException as e:
             self.logger.warning(
                 'A Connection error occurred sending ntfy:%s ' % (
                     notify_url) + 'notification.'
             )
             self.logger.debug('Socket Exception: %s' % str(e))
-            return False, response
 
         except (OSError, IOError) as e:
             self.logger.warning(
                 'An I/O error occurred while handling {}.'.format(
                     attach.name if isinstance(attach, AttachBase)
                     else virt_payload))
             self.logger.debug('I/O Exception: %s' % str(e))
-            return False, response
 
-        finally:
-            # Close our file (if it's open) stored in the second element
-            # of our files tuple (index 1)
-            if files:
-                files['file'][1].close()
+        return False, response
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
         default_port = 443 if self.secure else 80
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyOffice365.py` & `apprise-1.4.5/apprise/plugins/NotifyOffice365.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,21 @@
         },
         'secret': {
             'name': _('Client Secret'),
             'type': 'string',
             'private': True,
             'required': True,
         },
+        'target_email': {
+            'name': _('Target Email'),
+            'type': 'string',
+            'map_to': 'targets',
+        },
         'targets': {
-            'name': _('Target Emails'),
+            'name': _('Targets'),
             'type': 'list:string',
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyOneSignal.py` & `apprise-1.4.5/apprise/plugins/NotifyOneSignal.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
             'type': 'string',
             'prefix': '#',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
         },
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyOpsgenie.py` & `apprise-1.4.5/apprise/plugins/NotifyOpsgenie.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPagerDuty.py` & `apprise-1.4.5/apprise/plugins/NotifyPagerDuty.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             'name': _('API Key'),
             'type': 'string',
             'private': True,
             'required': True
         },
         # Optional but triggers V2 API
         'integrationkey': {
-            'name': _('Routing Key'),
+            'name': _('Integration Key'),
             'type': 'string',
             'private': True,
             'required': True
         },
         'source': {
             # Optional Source Identifier (preferably a FQDN)
             'name': _('Source'),
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPagerTree.py` & `apprise-1.4.5/apprise/plugins/NotifyPagerTree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyParsePlatform.py` & `apprise-1.4.5/apprise/plugins/NotifyParsePlatform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPopcornNotify.py` & `apprise-1.4.5/apprise/plugins/NotifyPopcornNotify.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
             'name': _('Target Email'),
             'type': 'string',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         }
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyProwl.py` & `apprise-1.4.5/apprise/plugins/NotifyProwl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPushBullet.py` & `apprise-1.4.5/apprise/plugins/NotifyPushBullet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPushSafer.py` & `apprise-1.4.5/apprise/plugins/NotifyPushSafer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPushed.py` & `apprise-1.4.5/apprise/plugins/NotifyPushed.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPushjet.py` & `apprise-1.4.5/apprise/plugins/NotifyPushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyPushover.py` & `apprise-1.4.5/apprise/plugins/NotifyPushover.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,17 +284,16 @@
         self.supplemental_url = supplemental_url
         self.supplemental_url_title = supplemental_url_title
 
         # Setup our sound
         self.sound = NotifyPushover.default_pushover_sound \
             if not isinstance(sound, str) else sound.lower()
         if self.sound and self.sound not in PUSHOVER_SOUNDS:
-            msg = 'The sound specified ({}) is invalid.'.format(sound)
-            self.logger.warning(msg)
-            raise TypeError(msg)
+            msg = 'Using custom sound specified ({}). '.format(sound)
+            self.logger.debug(msg)
 
         # The Priority of the message
         self.priority = int(
             NotifyPushover.template_args['priority']['default']
             if priority is None else
             next((
                 v for k, v in PUSHOVER_PRIORITY_MAP.items()
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyReddit.py` & `apprise-1.4.5/apprise/plugins/NotifyReddit.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 #   - https://www.reddit.com/dev/api/
 #   - https://www.reddit.com/dev/api/#POST_api_submit
 #   - https://github.com/reddit-archive/reddit/wiki/API
 import requests
 from json import loads
 from datetime import timedelta
 from datetime import datetime
+from datetime import timezone
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyFormat
 from ..common import NotifyType
 from ..utils import parse_list
 from ..utils import parse_bool
@@ -130,15 +131,15 @@
     # X-RateLimit-Reset: The epoc time (in seconds) we can expect our
     #                    rate-limit to be reset.
     # X-RateLimit-Remaining: an integer identifying how many requests we're
     #                        still allow to make.
     request_rate_per_sec = 0
 
     # For Tracking Purposes
-    ratelimit_reset = datetime.utcnow()
+    ratelimit_reset = datetime.now(timezone.utc).replace(tzinfo=None)
 
     # Default to 1.0
     ratelimit_remaining = 1.0
 
     # Taken right from google.auth.helpers:
     clock_skew = timedelta(seconds=10)
 
@@ -181,14 +182,15 @@
             'name': _('Target Subreddit'),
             'type': 'string',
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
@@ -271,15 +273,15 @@
         # Flair details
         self.flair_id = flair_id
         self.flair_text = flair_text
 
         # Our keys we build using the provided content
         self.__refresh_token = None
         self.__access_token = None
-        self.__access_token_expiry = datetime.utcnow()
+        self.__access_token_expiry = datetime.now(timezone.utc)
 
         self.kind = kind.strip().lower() \
             if isinstance(kind, str) \
             else self.template_args['kind']['default']
 
         if self.kind not in REDDIT_MESSAGE_KINDS:
             msg = 'An invalid Reddit message kind ({}) was specified'.format(
@@ -413,18 +415,18 @@
         # Acquire our token
         self.__access_token = response.get('access_token')
 
         # Handle other optional arguments we can use
         if 'expires_in' in response:
             delta = timedelta(seconds=int(response['expires_in']))
             self.__access_token_expiry = \
-                delta + datetime.utcnow() - self.clock_skew
+                delta + datetime.now(timezone.utc) - self.clock_skew
         else:
             self.__access_token_expiry = self.access_token_lifetime_sec + \
-                datetime.utcnow() - self.clock_skew
+                datetime.now(timezone.utc) - self.clock_skew
 
         # The Refresh Token
         self.__refresh_token = response.get(
             'refresh_token', self.__refresh_token)
 
         if self.__access_token:
             self.logger.info('Authenticated to Reddit as {}'.format(self.user))
@@ -543,15 +545,15 @@
         if self.ratelimit_remaining <= 0.0:
             # Determine how long we should wait for or if we should wait at
             # all. This isn't fool-proof because we can't be sure the client
             # time (calling this script) is completely synced up with the
             # Gitter server.  One would hope we're on NTP and our clocks are
             # the same allowing this to role smoothly:
 
-            now = datetime.utcnow()
+            now = datetime.now(timezone.utc).replace(tzinfo=None)
             if now < self.ratelimit_reset:
                 # We need to throttle for the difference in seconds
                 wait = abs(
                     (self.ratelimit_reset - now + self.clock_skew)
                     .total_seconds())
 
         # Always call throttle before any remote server i/o is made;
@@ -667,16 +669,17 @@
                 return (False, content)
 
             try:
                 # Store our rate limiting (if provided)
                 self.ratelimit_remaining = \
                     float(r.headers.get(
                         'X-RateLimit-Remaining'))
-                self.ratelimit_reset = datetime.utcfromtimestamp(
-                    int(r.headers.get('X-RateLimit-Reset')))
+                self.ratelimit_reset = datetime.fromtimestamp(
+                    int(r.headers.get('X-RateLimit-Reset')), timezone.utc
+                ).replace(tzinfo=None)
 
             except (TypeError, ValueError):
                 # This is returned if we could not retrieve this information
                 # gracefully accept this state and move on
                 pass
 
         except requests.RequestException as e:
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyRocketChat.py` & `apprise-1.4.5/apprise/plugins/NotifyRocketChat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyRyver.py` & `apprise-1.4.5/apprise/plugins/NotifyRyver.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     # The maximum allowable characters allowed in the body per message
     body_maxlen = 1000
 
     # Define object templates
     templates = (
         '{schema}://{organization}/{token}',
-        '{schema}://{user}@{organization}/{token}',
+        '{schema}://{botname}@{organization}/{token}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'organization': {
             'name': _('Organization'),
             'type': 'string',
@@ -105,17 +105,18 @@
         'token': {
             'name': _('Token'),
             'type': 'string',
             'required': True,
             'private': True,
             'regex': (r'^[A-Z0-9]{15}$', 'i'),
         },
-        'user': {
+        'botname': {
             'name': _('Bot Name'),
             'type': 'string',
+            'map_to': 'user',
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'mode': {
             'name': _('Webhook Mode'),
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySES.py` & `apprise-1.4.5/apprise/plugins/NotifySES.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 import re
 import hmac
 import base64
 import requests
 from hashlib import sha256
 from datetime import datetime
+from datetime import timezone
 from collections import OrderedDict
 from xml.etree import ElementTree
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 from email.utils import formataddr
 from email.header import Header
@@ -169,14 +170,15 @@
             'private': True,
             'required': True,
         },
         'region': {
             'name': _('Region'),
             'type': 'string',
             'regex': (r'^[a-z]{2}-[a-z-]+?-[0-9]+$', 'i'),
+            'required': True,
             'map_to': 'region_name',
         },
         'targets': {
             'name': _('Target Emails'),
             'type': 'list:string',
         },
     })
@@ -432,15 +434,16 @@
                 (from_name if from_name else False, self.from_addr),
                 charset='utf-8')
             base['To'] = formataddr((to_name, to_addr), charset='utf-8')
             if reply_to[1] != self.from_addr:
                 base['Reply-To'] = formataddr(reply_to, charset='utf-8')
             base['Cc'] = ','.join(cc)
             base['Date'] = \
-                datetime.utcnow().strftime("%a, %d %b %Y %H:%M:%S +0000")
+                datetime.now(
+                    timezone.utc).strftime("%a, %d %b %Y %H:%M:%S +0000")
             base['X-Application'] = self.app_id
 
             if attach:
                 # First attach our body to our content as the first element
                 base.attach(content)
 
                 # Now store our attachments
@@ -581,15 +584,15 @@
             # Populated below
             'Content-Length': 0,
             'Authorization': None,
             'X-Amz-Date': None,
         }
 
         # Get a reference time (used for header construction)
-        reference = datetime.utcnow()
+        reference = datetime.now(timezone.utc)
 
         # Provide Content-Length
         headers['Content-Length'] = str(len(payload))
 
         # Amazon Date Format
         amzdate = reference.strftime('%Y%m%dT%H%M%SZ')
         headers['X-Amz-Date'] = amzdate
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySMSEagle.py` & `apprise-1.4.5/apprise/plugins/NotifySMSEagle.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
             'type': 'int',
             'min': 1,
             'max': 65535,
         },
         'token': {
             'name': _('Access Token'),
             'type': 'string',
+            'required': True,
         },
         'target_phone': {
             'name': _('Target Phone No'),
             'type': 'string',
             'prefix': '+',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
@@ -166,14 +167,15 @@
             'prefix': '@',
             'regex': (r'^[a-z0-9_-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         }
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySMTP2Go.py` & `apprise-1.4.5/apprise/plugins/NotifySMTP2Go.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifySNS.py` & `apprise-1.4.5/apprise/plugins/NotifySNS.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 import re
 import hmac
 import requests
 from hashlib import sha256
 from datetime import datetime
+from datetime import timezone
 from collections import OrderedDict
 from xml.etree import ElementTree
 from itertools import chain
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyType
@@ -98,15 +99,15 @@
 
     # A title can not be used for SMS Messages.  Setting this to zero will
     # cause any title (if defined) to get placed into the message body.
     title_maxlen = 0
 
     # Define object templates
     templates = (
-        '{schema}://{access_key_id}/{secret_access_key}{region}/{targets}',
+        '{schema}://{access_key_id}/{secret_access_key}/{region}/{targets}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'access_key_id': {
             'name': _('Access Key ID'),
             'type': 'string',
@@ -120,14 +121,15 @@
             'required': True,
         },
         'region': {
             'name': _('Region'),
             'type': 'string',
             'required': True,
             'regex': (r'^[a-z]{2}-[a-z-]+?-[0-9]+$', 'i'),
+            'required': True,
             'map_to': 'region_name',
         },
         'target_phone_no': {
             'name': _('Target Phone No'),
             'type': 'string',
             'map_to': 'targets',
             'regex': (r'^[0-9\s)(+-]+$', 'i')
@@ -392,15 +394,15 @@
             # Populated below
             'Content-Length': 0,
             'Authorization': None,
             'X-Amz-Date': None,
         }
 
         # Get a reference time (used for header construction)
-        reference = datetime.utcnow()
+        reference = datetime.now(timezone.utc)
 
         # Provide Content-Length
         headers['Content-Length'] = str(len(payload))
 
         # Amazon Date Format
         amzdate = reference.strftime('%Y%m%dT%H%M%SZ')
         headers['X-Amz-Date'] = amzdate
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySendGrid.py` & `apprise-1.4.5/apprise/plugins/NotifySendGrid.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyServerChan.py` & `apprise-1.4.5/apprise/plugins/NotifyServerChan.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     setup_url = 'https://github.com/caronc/apprise/wiki/Notify_serverchan'
 
     # ServerChan API
     notify_url = 'https://sctapi.ftqq.com/{token}.send'
 
     # Define object templates
     templates = (
-        '{schema}://{token}/',
+        '{schema}://{token}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'token': {
             'name': _('Token'),
             'type': 'string',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySignalAPI.py` & `apprise-1.4.5/apprise/plugins/NotifySignalAPI.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifySimplePush.py` & `apprise-1.4.5/apprise/plugins/NotifySimplePush.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,20 @@
             'type': 'string',
             'private': True,
             'required': True,
         },
 
         # Used for encrypted logins
         'password': {
-            'name': _('Encrypted Password'),
+            'name': _('Password'),
             'type': 'string',
             'private': True,
         },
         'salt': {
-            'name': _('Encrypted Salt'),
+            'name': _('Salt'),
             'type': 'string',
             'private': True,
             'map_to': 'user',
         },
     })
 
     # Define our template arguments
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySinch.py` & `apprise-1.4.5/apprise/plugins/NotifySinch.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifySlack.py` & `apprise-1.4.5/apprise/plugins/NotifySlack.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,18 +161,18 @@
     # Bot's do not have default channels to notify; so #general
     # becomes the default channel in BOT mode
     default_notification_channel = '#general'
 
     # Define object templates
     templates = (
         # Webhook
-        '{schema}://{token_a}/{token_b}{token_c}',
+        '{schema}://{token_a}/{token_b}/{token_c}',
         '{schema}://{botname}@{token_a}/{token_b}{token_c}',
-        '{schema}://{token_a}/{token_b}{token_c}/{targets}',
-        '{schema}://{botname}@{token_a}/{token_b}{token_c}/{targets}',
+        '{schema}://{token_a}/{token_b}/{token_c}/{targets}',
+        '{schema}://{botname}@{token_a}/{token_b}/{token_c}/{targets}',
 
         # Bot
         '{schema}://{access_token}/',
         '{schema}://{access_token}/{targets}',
     )
 
     # Define our template tokens
@@ -194,33 +194,30 @@
         },
         # Token required as part of the Webhook request
         #  /AAAAAAAAA/........./........................
         'token_a': {
             'name': _('Token A'),
             'type': 'string',
             'private': True,
-            'required': True,
             'regex': (r'^[A-Z0-9]+$', 'i'),
         },
         # Token required as part of the Webhook request
         #  /........./BBBBBBBBB/........................
         'token_b': {
             'name': _('Token B'),
             'type': 'string',
             'private': True,
-            'required': True,
             'regex': (r'^[A-Z0-9]+$', 'i'),
         },
         # Token required as part of the Webhook request
         #  /........./........./CCCCCCCCCCCCCCCCCCCCCCCC
         'token_c': {
             'name': _('Token C'),
             'type': 'string',
             'private': True,
-            'required': True,
             'regex': (r'^[A-Za-z0-9]+$', 'i'),
         },
         'target_encoded_id': {
             'name': _('Target Encoded ID'),
             'type': 'string',
             'prefix': '+',
             'map_to': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySparkPost.py` & `apprise-1.4.5/apprise/plugins/NotifySparkPost.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         'tokens': {
             'name': _('Template Tokens'),
             'prefix': ':',
         },
     }
 
     def __init__(self, apikey, targets, cc=None, bcc=None, from_name=None,
-                 region_name=None, headers=None, tokens=None, batch=False,
+                 region_name=None, headers=None, tokens=None, batch=None,
                  **kwargs):
         """
         Initialize SparkPost Object
         """
         super().__init__(**kwargs)
 
         # API Key (associated with project)
@@ -292,15 +292,16 @@
 
         self.tokens = {}
         if tokens:
             # Store our template tokens
             self.tokens.update(tokens)
 
         # Prepare Batch Mode Flag
-        self.batch = batch
+        self.batch = self.template_args['batch']['default'] \
+            if batch is None else batch
 
         if targets:
             # Validate recipients (to:) and drop bad ones:
             for recipient in parse_emails(targets):
                 result = is_email(recipient)
                 if result:
                     self.targets.append(
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifySpontit.py` & `apprise-1.4.5/apprise/plugins/NotifySpontit.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
             'prefix': '#',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
-            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyStreamlabs.py` & `apprise-1.4.5/apprise/plugins/NotifyStreamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifySyslog.py` & `apprise-1.4.5/apprise/plugins/NotifySyslog.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,14 @@
             'type': 'choice:string',
             'values': [k for k in SYSLOG_FACILITY_MAP.keys()],
             'default': SyslogFacility.USER,
         },
         'host': {
             'name': _('Hostname'),
             'type': 'string',
-            'required': True,
         },
         'port': {
             'name': _('Port'),
             'type': 'int',
             'min': 1,
             'max': 65535,
             'default': 514,
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyTechulusPush.py` & `apprise-1.4.5/apprise/plugins/NotifyTechulusPush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyTelegram.py` & `apprise-1.4.5/apprise/plugins/NotifyTelegram.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,31 @@
 # If the Chat ID is negative, then it's targeting a group
 IS_CHAT_ID_RE = re.compile(
     r'^(@*(?P<idno>-?[0-9]{1,32})|(?P<name>[a-z_-][a-z0-9_-]+))$',
     re.IGNORECASE,
 )
 
 
+class TelegramContentPlacement:
+    """
+    The Telegram Content Placement
+    """
+    # Before Attachments
+    BEFORE = "before"
+    # After Attachments
+    AFTER = "after"
+
+
+# Identify Placement Categories
+TELEGRAM_CONTENT_PLACEMENT = (
+    TelegramContentPlacement.BEFORE,
+    TelegramContentPlacement.AFTER,
+)
+
+
 class NotifyTelegram(NotifyBase):
     """
     A wrapper for Telegram Notifications
     """
     # The default descriptive name associated with the Notification
     service_name = 'Telegram'
 
@@ -315,19 +332,25 @@
         'topic': {
             'name': _('Topic Thread ID'),
             'type': 'int',
         },
         'to': {
             'alias_of': 'targets',
         },
+        'content': {
+            'name': _('Content Placement'),
+            'type': 'choice:string',
+            'values': TELEGRAM_CONTENT_PLACEMENT,
+            'default': TelegramContentPlacement.BEFORE,
+        },
     })
 
     def __init__(self, bot_token, targets, detect_owner=True,
                  include_image=False, silent=None, preview=None, topic=None,
-                 **kwargs):
+                 content=None, **kwargs):
         """
         Initialize Telegram Object
         """
         super().__init__(**kwargs)
 
         self.bot_token = validate_regex(
             bot_token, *self.template_tokens['bot_token']['regex'],
@@ -345,14 +368,23 @@
         self.silent = self.template_args['silent']['default'] \
             if silent is None else bool(silent)
 
         # Define whether or not we should display a web page preview
         self.preview = self.template_args['preview']['default'] \
             if preview is None else bool(preview)
 
+        # Setup our content placement
+        self.content = self.template_args['content']['default'] \
+            if not isinstance(content, str) else content.lower()
+        if self.content and self.content not in TELEGRAM_CONTENT_PLACEMENT:
+            msg = 'The content placement specified ({}) is invalid.'\
+                .format(content)
+            self.logger.warning(msg)
+            raise TypeError(msg)
+
         if topic:
             try:
                 self.topic = int(topic)
 
             except (TypeError, ValueError):
                 # Not a valid integer; ignore entry
                 err = 'The Telegram Topic ID specified ({}) is invalid.'\
@@ -435,19 +467,22 @@
         )
 
         # Always call throttle before any remote server i/o is made;
         # Telegram throttles to occur before sending the image so that
         # content can arrive together.
         self.throttle()
 
+        payload = {'chat_id': chat_id}
+        if self.topic:
+            payload['message_thread_id'] = self.topic
+
         try:
             with open(path, 'rb') as f:
                 # Configure file payload (for upload)
                 files = {key: (file_name, f)}
-                payload = {'chat_id': chat_id}
 
                 self.logger.debug(
                     'Telegram attachment POST URL: %s (cert_verify=%r)' % (
                         url, self.verify_certificate))
 
                 r = requests.post(
                     url,
@@ -709,14 +744,23 @@
                 if not self.send_media(payload['chat_id'], notify_type):
                     # We failed to send the image associated with our
                     notify_type
                     self.logger.warning(
                         'Failed to send Telegram type image to {}.',
                         payload['chat_id'])
 
+            if attach and self.content == TelegramContentPlacement.AFTER:
+                # Send our attachments now (if specified and if it exists)
+                if not self._send_attachments(
+                        chat_id=payload['chat_id'], notify_type=notify_type,
+                        attach=attach):
+
+                    has_error = True
+                    continue
+
             # Always call throttle before any remote server i/o is made;
             # Telegram throttles to occur before sending the image so that
             # content can arrive together.
             self.throttle()
 
             self.logger.debug('Telegram POST URL: %s (cert_verify=%r)' % (
                 url, self.verify_certificate,
@@ -771,41 +815,58 @@
 
                 # Flag our error
                 has_error = True
                 continue
 
             self.logger.info('Sent Telegram notification.')
 
-            if attach:
-                # Send our attachments now (if specified and if it exists)
-                for attachment in attach:
-                    if not self.send_media(
-                            payload['chat_id'], notify_type,
-                            attach=attachment):
-
-                        # We failed; don't continue
-                        has_error = True
-                        break
+            if attach and self.content == TelegramContentPlacement.BEFORE:
+                # Send our attachments now (if specified and if it exists) as
+                # it was identified to send the content before the attachments
+                # which is now done.
+                if not self._send_attachments(
+                        chat_id=payload['chat_id'],
+                        notify_type=notify_type,
+                        attach=attach):
 
-                    self.logger.info(
-                        'Sent Telegram attachment: {}.'.format(attachment))
+                    has_error = True
+                    continue
+
+        return not has_error
+
+    def _send_attachments(self, chat_id, notify_type, attach):
+        """
+        Sends our attachments
+        """
+        has_error = False
+        # Send our attachments now (if specified and if it exists)
+        for attachment in attach:
+            if not self.send_media(chat_id, notify_type, attach=attachment):
+
+                # We failed; don't continue
+                has_error = True
+                break
+
+            self.logger.info(
+                'Sent Telegram attachment: {}.'.format(attachment))
 
         return not has_error
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
         # Define any URL parameters
         params = {
             'image': self.include_image,
             'detect': 'yes' if self.detect_owner else 'no',
             'silent': 'yes' if self.silent else 'no',
             'preview': 'yes' if self.preview else 'no',
+            'content': self.content,
         }
 
         if self.topic:
             params['topic'] = self.topic
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
@@ -881,14 +942,18 @@
         bot_token_b = entries.pop(0)
 
         bot_token = '%s:%s' % (bot_token_a, bot_token_b)
 
         # Store our chat ids (as these are the remaining entries)
         results['targets'] = entries
 
+        # content to be displayed 'before' or 'after' attachments
+        if 'content' in results['qsd'] and len(results['qsd']['content']):
+            results['content'] = results['qsd']['content']
+
         # Support the 'to' variable so that we can support rooms this way too
         # The 'to' makes it easier to use yaml configuration
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'] += \
                 NotifyTelegram.parse_list(results['qsd']['to'])
 
         # Store our bot token
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyTwilio.py` & `apprise-1.4.5/apprise/plugins/NotifyTwilio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyTwist.py` & `apprise-1.4.5/apprise/plugins/NotifyTwist.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,18 +102,20 @@
 
     # Define our template arguments
     template_tokens = dict(NotifyBase.template_tokens, **{
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
+            'required': True,
         },
         'email': {
             'name': _('Email'),
             'type': 'string',
+            'required': True,
         },
         'target_channel': {
             'name': _('Target Channel'),
             'type': 'string',
             'prefix': '#',
             'map_to': 'targets',
         },
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyTwitter.py` & `apprise-1.4.5/apprise/plugins/NotifyTwitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 # See https://developer.twitter.com/en/docs/direct-messages/\
 #           sending-and-receiving/api-reference/new-event.html
 import re
 import requests
 from copy import deepcopy
 from datetime import datetime
+from datetime import timezone
 from requests_oauthlib import OAuth1
 from json import dumps
 from json import loads
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyType
 from ..utils import parse_list
@@ -120,21 +121,22 @@
     # X-Rate-Limit-Reset: The epoc time (in seconds) we can expect our
     #                    rate-limit to be reset.
     # X-Rate-Limit-Remaining: an integer identifying how many requests we're
     #                        still allow to make.
     request_rate_per_sec = 0
 
     # For Tracking Purposes
-    ratelimit_reset = datetime.utcnow()
+    ratelimit_reset = datetime.now(timezone.utc).replace(tzinfo=None)
 
     # Default to 1000; users can send up to 1000 DM's and 2400 tweets a day
     # This value only get's adjusted if the server sets it that way
     ratelimit_remaining = 1
 
     templates = (
+        '{schema}://{ckey}/{csecret}/{akey}/{asecret}',
         '{schema}://{ckey}/{csecret}/{akey}/{asecret}/{targets}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'ckey': {
             'name': _('Consumer Key'),
@@ -674,15 +676,15 @@
         if self.ratelimit_remaining == 0:
             # Determine how long we should wait for or if we should wait at
             # all. This isn't fool-proof because we can't be sure the client
             # time (calling this script) is completely synced up with the
             # Twitter server.  One would hope we're on NTP and our clocks are
             # the same allowing this to role smoothly:
 
-            now = datetime.utcnow()
+            now = datetime.now(timezone.utc).replace(tzinfo=None)
             if now < self.ratelimit_reset:
                 # We need to throttle for the difference in seconds
                 # We add 0.5 seconds to the end just to allow a grace
                 # period.
                 wait = (self.ratelimit_reset - now).total_seconds() + 0.5
 
         # Default content response object
@@ -732,16 +734,17 @@
                 # Mark our failure
                 return (False, content)
 
             try:
                 # Capture rate limiting if possible
                 self.ratelimit_remaining = \
                     int(r.headers.get('x-rate-limit-remaining'))
-                self.ratelimit_reset = datetime.utcfromtimestamp(
-                    int(r.headers.get('x-rate-limit-reset')))
+                self.ratelimit_reset = datetime.fromtimestamp(
+                    int(r.headers.get('x-rate-limit-reset')), timezone.utc
+                ).replace(tzinfo=None)
 
             except (TypeError, ValueError):
                 # This is returned if we could not retrieve this information
                 # gracefully accept this state and move on
                 pass
 
         except requests.RequestException as e:
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyVoipms.py` & `apprise-1.4.5/apprise/plugins/NotifyVoipms.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 
     # A title can not be used for SMS Messages.  Setting this to zero will
     # cause any title (if defined) to get placed into the message body.
     title_maxlen = 0
 
     # Define object templates
     templates = (
-        '{schema}://{password}:{email}',
         '{schema}://{password}:{email}/{from_phone}/{targets}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'email': {
             'name': _('User Email'),
@@ -107,14 +106,15 @@
             'prefix': '+',
             'regex': (r'^[0-9\s)(+-]+$', 'i'),
             'map_to': 'targets',
         },
         'targets': {
             'name': _('Targets'),
             'type': 'list:string',
+            'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
```

### Comparing `apprise-1.4.0/apprise/plugins/NotifyVonage.py` & `apprise-1.4.5/apprise/plugins/NotifyVonage.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyWebexTeams.py` & `apprise-1.4.5/apprise/plugins/NotifyWebexTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyWindows.py` & `apprise-1.4.5/apprise/plugins/NotifyWindows.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyXBMC.py` & `apprise-1.4.5/apprise/plugins/NotifyXBMC.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyXML.py` & `apprise-1.4.5/apprise/plugins/NotifyXML.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise/plugins/NotifyZulip.py` & `apprise-1.4.5/apprise/plugins/NotifyZulip.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
         'botname': {
             'name': _('Bot Name'),
             'type': 'string',
             'regex': (r'^[A-Z0-9_-]{1,32}$', 'i'),
+            'required': True,
         },
         'organization': {
             'name': _('Organization'),
             'type': 'string',
             'required': True,
             'regex': (r'^[A-Z0-9_-]{1,32})$', 'i')
         },
```

### Comparing `apprise-1.4.0/apprise/plugins/__init__.py` & `apprise-1.4.5/apprise/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,17 @@
     """
     This is called by the details() function and santizes the output by
     populating expected and consistent arguments if they weren't otherwise
     specified.
 
     """
 
+    # Used for tracking groups
+    group_map = {}
+
     # Iterate over our tokens
     for key in tokens.keys():
 
         for element in tokens[key].keys():
             # Perform translations (if detected to do so)
             if isinstance(tokens[key][element], LazyTranslation):
                 tokens[key][element] = str(tokens[key][element])
@@ -177,22 +180,35 @@
             # Do not touch this field
             continue
 
         if 'map_to' not in tokens[key]:
             # Default type to key
             tokens[key]['map_to'] = key
 
+        # Track our map_to objects
+        if tokens[key]['map_to'] not in group_map:
+            group_map[tokens[key]['map_to']] = set()
+        group_map[tokens[key]['map_to']].add(key)
+
         if 'type' not in tokens[key]:
             # Default type to string
             tokens[key]['type'] = 'string'
 
-        elif tokens[key]['type'].startswith('list') \
-                and 'delim' not in tokens[key]:
-            # Default list delimiter (if not otherwise specified)
-            tokens[key]['delim'] = default_delimiter
+        elif tokens[key]['type'].startswith('list'):
+            if 'delim' not in tokens[key]:
+                # Default list delimiter (if not otherwise specified)
+                tokens[key]['delim'] = default_delimiter
+
+            if key in group_map[tokens[key]['map_to']]:  # pragma: no branch
+                # Remove ourselves from the list
+                group_map[tokens[key]['map_to']].remove(key)
+
+            # Pointing to the set directly so we can dynamically update
+            # ourselves
+            tokens[key]['group'] = group_map[tokens[key]['map_to']]
 
         elif tokens[key]['type'].startswith('choice') \
                 and 'default' not in tokens[key] \
                 and 'values' in tokens[key] \
                 and len(tokens[key]['values']) == 1:
 
             # If there is only one choice; then make it the default
@@ -262,14 +278,21 @@
     #            # this list as a (True, False) such as ('Yes, 'No') or
     #            # ('Enabled', 'Disabled'), etc
     #            'values': [ 'http', 'https' ],
     #
     #            # Identifies if the entry specified is required or not
     #            'required': True,
     #
+    #            # Identifies all tokens detected to be associated with the
+    #            # list:string
+    #            # This is ony present in list:string objects and is only set
+    #            # if this element acts as an alias for several other
+    #            # kwargs/fields.
+    #            'group': [],
+    #
     #            # Identify a default value
     #            'default': 'http',
     #
     #            # Optional Verification Entries min and max are for floats
     #            # and/or integers
     #            'min': 4,
     #            'max': 5,
```

### Comparing `apprise-1.4.0/apprise/utils.py` & `apprise-1.4.5/apprise/utils.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/apprise.egg-info/PKG-INFO` & `apprise-1.4.5/apprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.4.0
+Version: 1.4.5
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
-Keywords: Alerts API AWS Boxcar BulkSMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex Windows Voipms XBMC
-Platform: UNKNOWN
+Keywords: Alerts API AWS Boxcar BulkSMS Burst SMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex WhatsApp Windows Voipms XBMC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -150,22 +149,24 @@
 | [Spontit](https://github.com/caronc/apprise/wiki/Notify_spontit) | spontit://  | (TCP) 443   | spontit://UserID@APIKey/<br />spontit://UserID@APIKey/Channel<br />spontit://UserID@APIKey/Channel1/Channel2/ChannelN
 | [Syslog](https://github.com/caronc/apprise/wiki/Notify_syslog) | syslog://  | (UDP) 514 (_if hostname specified_) | syslog://<br />syslog://Facility<br />syslog://hostname<br />syslog://hostname/Facility
 | [Telegram](https://github.com/caronc/apprise/wiki/Notify_telegram) | tgram://  | (TCP) 443   | tgram://bottoken/ChatID<br />tgram://bottoken/ChatID1/ChatID2/ChatIDN
 | [Twitter](https://github.com/caronc/apprise/wiki/Notify_twitter) | twitter://  | (TCP) 443   | twitter://CKey/CSecret/AKey/ASecret<br/>twitter://user@CKey/CSecret/AKey/ASecret<br/>twitter://CKey/CSecret/AKey/ASecret/User1/User2/User2<br/>twitter://CKey/CSecret/AKey/ASecret?mode=tweet
 | [Twist](https://github.com/caronc/apprise/wiki/Notify_twist) | twist://  | (TCP) 443   | twist://pasword:login<br/>twist://password:login/#channel<br/>twist://password:login/#team:channel<br/>twist://password:login/#team:channel1/channel2/#team3:channel
 | [XBMC](https://github.com/caronc/apprise/wiki/Notify_xbmc) | xbmc:// or xbmcs://    | (TCP) 8080 or 443   | xbmc://hostname<br />xbmc://user@hostname<br />xbmc://user:password@hostname:port
 | [Webex Teams (Cisco)](https://github.com/caronc/apprise/wiki/Notify_wxteams) | wxteams://  | (TCP) 443   | wxteams://Token
+| [WhatsApp](https://github.com/caronc/apprise/wiki/Notify_whatsapp) | whatsapp://  | (TCP) 443   | whatsapp://AccessToken@FromPhoneID/ToPhoneNo<br/> whatsapp://Template:AccessToken@FromPhoneID/ToPhoneNo
 | [Zulip Chat](https://github.com/caronc/apprise/wiki/Notify_zulip) | zulip://  | (TCP) 443   | zulip://botname@Organization/Token<br />zulip://botname@Organization/Token/Stream<br />zulip://botname@Organization/Token/Email
 
 ## SMS Notifications
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [AWS SNS](https://github.com/caronc/apprise/wiki/Notify_sns)  | sns://   | (TCP) 443   | sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo<br/>sns://AccessKeyID/AccessSecretKey/RegionName/+PhoneNo1/+PhoneNo2/+PhoneNoN<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic<br/>sns://AccessKeyID/AccessSecretKey/RegionName/Topic1/Topic2/TopicN
 | [BulkSMS](https://github.com/caronc/apprise/wiki/Notify_bulksms) | bulksms://  | (TCP) 443   | bulksms://user:password@ToPhoneNo<br/>bulksms://User:Password@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
+| [Burst SMS](https://github.com/caronc/apprise/wiki/Notify_burst_sms) | burstsms://  | (TCP) 443   | burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo<br/>burstsms://ApiKey:ApiSecret@FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [ClickSend](https://github.com/caronc/apprise/wiki/Notify_clicksend) | clicksend://  | (TCP) 443   | clicksend://user:pass@PhoneNo<br/>clicksend://user:pass@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DAPNET](https://github.com/caronc/apprise/wiki/Notify_dapnet) | dapnet://  | (TCP) 80   | dapnet://user:pass@callsign<br/>dapnet://user:pass@callsign1/callsign2/callsignN
 | [D7 Networks](https://github.com/caronc/apprise/wiki/Notify_d7networks) | d7sms://  | (TCP) 443   | d7sms://token@PhoneNo<br/>d7sms://token@ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [DingTalk](https://github.com/caronc/apprise/wiki/Notify_dingtalk)  | dingtalk://   | (TCP) 443   | dingtalk://token/<br />dingtalk://token/ToPhoneNo<br />dingtalk://token/ToPhoneNo1/ToPhoneNo2/ToPhoneNo1/
 | [Kavenegar](https://github.com/caronc/apprise/wiki/Notify_kavenegar) | kavenegar://  | (TCP) 443   | kavenegar://ApiKey/ToPhoneNo<br/>kavenegar://FromPhoneNo@ApiKey/ToPhoneNo<br/>kavenegar://ApiKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN
 | [MessageBird](https://github.com/caronc/apprise/wiki/Notify_messagebird) | msgbird://  | (TCP) 443   | msgbird://ApiKey/FromPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo<br/>msgbird://ApiKey/FromPhoneNo/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
 | [MSG91](https://github.com/caronc/apprise/wiki/Notify_msg91) | msg91://  | (TCP) 443   | msg91://AuthKey/ToPhoneNo<br/>msg91://SenderID@AuthKey/ToPhoneNo<br/>msg91://AuthKey/ToPhoneNo1/ToPhoneNo2/ToPhoneNoN/
@@ -559,9 +560,7 @@
 * ⚡ [Create Your Own Custom Notifications](https://github.com/caronc/apprise/wiki/decorator_notify)
 * 🌎 [Apprise API/Web Interface](https://github.com/caronc/apprise-api)
 * 🎉 [Showcase](https://github.com/caronc/apprise/wiki/showcase)
 
 Want to help make Apprise better?
 * 💡 [Contribute to the Apprise Code Base](https://github.com/caronc/apprise/wiki/Development_Contribution)
 * ❤️ [Sponsorship and Donations](https://github.com/caronc/apprise/wiki/Sponsors)
-
-
```

### Comparing `apprise-1.4.0/apprise.egg-info/SOURCES.txt` & `apprise-1.4.5/apprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 apprise/i18n/en/LC_MESSAGES/apprise.mo
 apprise/plugins/NotifyAppriseAPI.py
 apprise/plugins/NotifyBark.py
 apprise/plugins/NotifyBase.py
 apprise/plugins/NotifyBase.pyi
 apprise/plugins/NotifyBoxcar.py
 apprise/plugins/NotifyBulkSMS.py
+apprise/plugins/NotifyBurstSMS.py
 apprise/plugins/NotifyClickSend.py
 apprise/plugins/NotifyD7Networks.py
 apprise/plugins/NotifyDBus.py
 apprise/plugins/NotifyDapnet.py
 apprise/plugins/NotifyDingTalk.py
 apprise/plugins/NotifyDiscord.py
 apprise/plugins/NotifyEmail.py
@@ -152,14 +153,15 @@
 apprise/plugins/NotifyTelegram.py
 apprise/plugins/NotifyTwilio.py
 apprise/plugins/NotifyTwist.py
 apprise/plugins/NotifyTwitter.py
 apprise/plugins/NotifyVoipms.py
 apprise/plugins/NotifyVonage.py
 apprise/plugins/NotifyWebexTeams.py
+apprise/plugins/NotifyWhatsApp.py
 apprise/plugins/NotifyWindows.py
 apprise/plugins/NotifyXBMC.py
 apprise/plugins/NotifyXML.py
 apprise/plugins/NotifyZulip.py
 apprise/plugins/__init__.py
 apprise/plugins/NotifyFCM/__init__.py
 apprise/plugins/NotifyFCM/color.py
@@ -193,14 +195,15 @@
 test/test_locale.py
 test/test_logger.py
 test/test_notify_base.py
 test/test_plugin_apprise_api.py
 test/test_plugin_bark.py
 test/test_plugin_boxcar.py
 test/test_plugin_bulksms.py
+test/test_plugin_burstsms.py
 test/test_plugin_clicksend.py
 test/test_plugin_custom_form.py
 test/test_plugin_custom_json.py
 test/test_plugin_custom_xml.py
 test/test_plugin_d7networks.py
 test/test_plugin_dapnet.py
 test/test_plugin_dingtalk.py
@@ -274,14 +277,15 @@
 test/test_plugin_telegram.py
 test/test_plugin_twilio.py
 test/test_plugin_twist.py
 test/test_plugin_twitter.py
 test/test_plugin_voipms.py
 test/test_plugin_vonage.py
 test/test_plugin_webex_teams.py
+test/test_plugin_whatsapp.py
 test/test_plugin_windows.py
 test/test_plugin_xbmc_kodi.py
 test/test_plugin_zulip.py
 test/test_rest_plugins.py
 test/helpers/__init__.py
 test/helpers/asyncio.py
 test/helpers/module.py
```

### Comparing `apprise-1.4.0/packaging/README.md` & `apprise-1.4.5/packaging/README.md`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/packaging/man/apprise.1` & `apprise-1.4.5/packaging/man/apprise.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "APPRISE" "1" "July 2022" ""
+.TH "APPRISE" "1" "May 2023" ""
 .SH "NAME"
 \fBapprise\fR \- Push Notifications that work with just about every platform!
 .SH "SYNOPSIS"
 \fBapprise\fR [\fIoptions\fR\|\.\|\.\|\.] \fIservice\-url\fR\|\.\|\.\|\.
 .br
 .SH "DESCRIPTION"
 \fBApprise\fR allows you to send a notification to \fIalmost all\fR of the most popular notification services available to us today such as: Discord, Telegram, Pushbullet, Slack, Twitter, etc\.
@@ -116,14 +116,15 @@
 Apprise can additionally allow you to define your own custom \fBschema://\fR entries that you can trigger on and call services you\'ve defined\.
 .P
 By default \fBapprise\fR looks in the following local locations for custom plugin files and loads them:
 .IP "" 4
 .nf
 ~/\.apprise/plugins
 ~/\.config/apprise/plugins
+/var/lib/apprise/plugins
 .fi
 .IP "" 0
 .P
 Simply create your own python file with the following bare minimum content in it: from apprise\.decorators import notify
 .IP "" 4
 .nf
 # This example assumes you want your function to trigger on foobar://
@@ -149,14 +150,19 @@
 ~/\.config/apprise
 ~/\.config/apprise\.yml
 
 ~/\.apprise/apprise
 ~/\.apprise/apprise\.yaml
 ~/\.config/apprise/apprise
 ~/\.config/apprise/apprise\.yaml
+
+/etc/apprise
+/etc/apprise\.yml
+/etc/apprise/apprise
+/etc/apprise/apprise\.yml
 .fi
 .IP "" 0
 .P
 If a default configuration file is referenced in any way by the \fBapprise\fR tool, you no longer need to provide it a Service URL\. Usage of the \fBapprise\fR tool simplifies to:
 .IP "" 4
 .nf
 $ apprise \-vv \-t "my title" \-b "my notification body"
@@ -169,8 +175,8 @@
 $ apprise \-vv \-t "Will Be Late" \-b "Go ahead and make dinner without me" \e
           \-\-tag=family
 .fi
 .IP "" 0
 .SH "BUGS"
 If you find any bugs, please make them known at: \fIhttps://github\.com/caronc/apprise/issues\fR
 .SH "COPYRIGHT"
-Apprise is Copyright (C) 2021 Chris Caron \fIlead2gold@gmail\.com\fR
+Apprise is Copyright (C) 2023 Chris Caron \fIlead2gold@gmail\.com\fR
```

### Comparing `apprise-1.4.0/packaging/man/apprise.md` & `apprise-1.4.5/packaging/man/apprise.md`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/packaging/redhat/apprise-click67-support.patch` & `apprise-1.4.5/packaging/redhat/apprise-click67-support.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/packaging/redhat/apprise-no-macosx-testing.patch` & `apprise-1.4.5/packaging/redhat/apprise-no-macosx-testing.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch` & `apprise-1.4.5/packaging/redhat/apprise-pytest-session_mocker-removal.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/packaging/redhat/python-apprise.spec` & `apprise-1.4.5/packaging/redhat/python-apprise.spec`

 * *Files 0% similar despite different names*

```diff
@@ -39,28 +39,28 @@
 %global pypi_name apprise
 
 %global common_description %{expand: \
 Apprise is a Python package for simplifying access to all of the different
 notification services that are out there. Apprise opens the door and makes
 it easy to access:
 
-Apprise API, AWS SES, AWS SNS, Bark, BulkSMS, Boxcar, ClickSend, DAPNET,
-DingTalk, Discord, E-Mail, Emby, Faast, FCM, Flock, Gitter, Google Chat,
+Apprise API, AWS SES, AWS SNS, Bark, Boxcar, Burst SMS, BulkSMS, ClickSend,
+DAPNET, DingTalk, Discord, E-Mail, Emby, Faast, FCM, Flock, Gitter, Google Chat,
 Gotify, Growl, Guilded, Home Assistant, IFTTT, Join, Kavenegar, KODI, Kumulos,
 LaMetric, Line, MacOSX, Mailgun, Mastodon, Mattermost, Matrix, MessageBird,
 Microsoft Windows, Microsoft Teams, Misskey, MQTT, MSG91, MyAndroid, Nexmo,
 Nextcloud, NextcloudTalk, Notica, Notifico, ntfy, Office365, OneSignal,
 Opsgenie, PagerDuty, PagerTree, ParsePlatform, PopcornNotify, Prowl, Pushalot,
 PushBullet, Pushjet, Pushover, PushSafer, Reddit, Rocket.Chat, SendGrid,
 ServerChan, Signal, SimplePush, Sinch, Slack, SMSEagle, SMTP2Go, Spontit,
 SparkPost, Super Toasty, Streamlabs, Stride, Syslog, Techulus Push, Telegram,
-Twilio, Twitter, Twist, XBMC, Voipms, Vonage, Webex Teams}
+Twilio, Twitter, Twist, XBMC, Voipms, Vonage, WhatsApp, Webex Teams}
 
 Name:           python-%{pypi_name}
-Version:        1.4.0
+Version:        1.4.5
 Release:        1%{?dist}
 Summary:        A simple wrapper to many popular notification services used today
 License:        BSD
 URL:            https://github.com/caronc/%{pypi_name}
 Source0:        %{url}/archive/v%{version}/%{pypi_name}-%{version}.tar.gz
 
 # RHEL/Rocky 8 ship with Click v6.7 which does not support the .stdout
@@ -182,14 +182,20 @@
 
 %files -n %{pypi_name}
 %{_bindir}/%{pypi_name}
 %{_mandir}/man1/%{pypi_name}.1*
 %{python3_sitelib}/%{pypi_name}/cli.*
 
 %changelog
+* Thu Jul  6 2023 Chris Caron <lead2gold@gmail.com> - 1.4.5
+- Updated to v1.4.5
+
+* Wed Jun 14 2023 Python Maint <python-maint@redhat.com> - 1.4.0-2
+- Rebuilt for Python 3.12
+
 * Mon May 15 2023 Chris Caron <lead2gold@gmail.com> - 1.4.0
 - Updated to v1.4.0
 
 * Wed Feb 22 2023 Chris Caron <lead2gold@gmail.com> - 1.3.0
 - Updated to v1.3.0
 
 * Fri Jan 20 2023 Fedora Release Engineering <releng@fedoraproject.org> - 1.2.1-2
```

### Comparing `apprise-1.4.0/setup.cfg` & `apprise-1.4.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bdist_wheel]
-universal = 1
+universal = 0
 
 [metadata]
 license_file = LICENSE
 
 [flake8]
 exclude = .eggs,.tox
 ignore = E741,E722,W503,W504,W605
```

### Comparing `apprise-1.4.0/setup.py` & `apprise-1.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['apprise = apprise.cli:main']
 
 setup(
     name='apprise',
-    version='1.4.0',
+    version='1.4.5',
     description='Push Notifications that work with just about every platform!',
     license='BSD',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     cmdclass=cmdclass,
     url='https://github.com/caronc/apprise',
     keywords=' '.join(re.split(r'\s+', open('KEYWORDS').read())),
```

### Comparing `apprise-1.4.0/test/conftest.py` & `apprise-1.4.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/helpers/__init__.py` & `apprise-1.4.5/test/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/helpers/asyncio.py` & `apprise-1.4.5/test/helpers/asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/helpers/module.py` & `apprise-1.4.5/test/helpers/module.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/helpers/rest.py` & `apprise-1.4.5/test/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_api.py` & `apprise-1.4.5/test/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1482,14 +1482,15 @@
         'verify', 'cto', 'rto',
     ])
 
     # Valid Schema Entries:
     valid_schema_keys = (
         'name', 'private', 'required', 'type', 'values', 'min', 'max',
         'regex', 'default', 'list', 'delim', 'prefix', 'map_to', 'alias_of',
+        'group',
     )
     for entry in details['schemas']:
 
         # Track the map_to entries (if specified); We need to make sure that
         # these properly map back
         map_to_entries = set()
```

### Comparing `apprise-1.4.0/test/test_apprise_attachments.py` & `apprise-1.4.5/test/test_apprise_attachments.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_apprise_config.py` & `apprise-1.4.5/test/test_apprise_config.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_apprise_utils.py` & `apprise-1.4.5/test/test_apprise_utils.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_asyncio.py` & `apprise-1.4.5/test/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_attach_base.py` & `apprise-1.4.5/test/test_attach_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_attach_file.py` & `apprise-1.4.5/test/test_attach_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_attach_http.py` & `apprise-1.4.5/test/test_attach_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_cli.py` & `apprise-1.4.5/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_config_base.py` & `apprise-1.4.5/test/test_config_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_config_file.py` & `apprise-1.4.5/test/test_config_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_config_http.py` & `apprise-1.4.5/test/test_config_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_config_memory.py` & `apprise-1.4.5/test/test_config_memory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_conversion.py` & `apprise-1.4.5/test/test_conversion.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_decorator_notify.py` & `apprise-1.4.5/test/test_decorator_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_escapes.py` & `apprise-1.4.5/test/test_escapes.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_locale.py` & `apprise-1.4.5/test/test_locale.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_logger.py` & `apprise-1.4.5/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_notify_base.py` & `apprise-1.4.5/test/test_notify_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_apprise_api.py` & `apprise-1.4.5/test/test_plugin_apprise_api.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_bark.py` & `apprise-1.4.5/test/test_plugin_bark.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_boxcar.py` & `apprise-1.4.5/test/test_plugin_boxcar.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,20 @@
     # our access, secret and device are all 64 characters
     # which is what we're doing here
     ('boxcar://%s/%s/@tag1/tag2///%s/?to=tag3' % (
         'a' * 64, 'b' * 64, 'd' * 64), {
         'instance': NotifyBoxcar,
         'requests_response_code': requests.codes.created,
     }),
+    ('boxcar://?access=%s&secret=%s&to=tag5' % ('d' * 64, 'b' * 64), {
+        # Test access and secret kwargs
+        'privacy_url': 'boxcar://d...d/****/',
+        'instance': NotifyBoxcar,
+        'requests_response_code': requests.codes.created,
+    }),
     # An invalid tag
     ('boxcar://%s/%s/@%s' % ('a' * 64, 'b' * 64, 't' * 64), {
         'instance': NotifyBoxcar,
         'requests_response_code': requests.codes.created,
     }),
     ('boxcar://%s/%s/' % ('a' * 64, 'b' * 64), {
         'instance': NotifyBoxcar,
```

### Comparing `apprise-1.4.0/test/test_plugin_bulksms.py` & `apprise-1.4.5/test/test_plugin_bulksms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_clicksend.py` & `apprise-1.4.5/test/test_plugin_clicksend.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_custom_form.py` & `apprise-1.4.5/test/test_plugin_custom_form.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_custom_json.py` & `apprise-1.4.5/test/test_plugin_custom_json.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_custom_xml.py` & `apprise-1.4.5/test/test_plugin_custom_xml.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_d7networks.py` & `apprise-1.4.5/test/test_plugin_d7networks.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_dapnet.py` & `apprise-1.4.5/test/test_plugin_dapnet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_dingtalk.py` & `apprise-1.4.5/test/test_plugin_dingtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_discord.py` & `apprise-1.4.5/test/test_plugin_discord.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_email.py` & `apprise-1.4.5/test/test_plugin_email.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_emby.py` & `apprise-1.4.5/test/test_plugin_emby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_enigma2.py` & `apprise-1.4.5/test/test_plugin_enigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_faast.py` & `apprise-1.4.5/test/test_plugin_faast.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_fcm.py` & `apprise-1.4.5/test/test_plugin_fcm.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_flock.py` & `apprise-1.4.5/test/test_plugin_flock.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_gitter.py` & `apprise-1.4.5/test/test_plugin_gitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import requests
 
 from apprise.plugins.NotifyGitter import NotifyGitter
 from helpers import AppriseURLTester
 
 from json import dumps
 from datetime import datetime
+from datetime import timezone
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
@@ -152,21 +153,22 @@
             'userCount': 1,
             'id': '5c981cecd73408ce4fbbad31',
             'name': 'apprise/community',
         },
     ]
 
     # Epoch time:
-    epoch = datetime.utcfromtimestamp(0)
+    epoch = datetime.fromtimestamp(0, timezone.utc)
 
     request = mock.Mock()
     request.content = dumps(response_obj)
     request.status_code = requests.codes.ok
     request.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
 
     # Prepare Mock
     mock_get.return_value = request
     mock_post.return_value = request
 
@@ -207,29 +209,29 @@
 
     # Handle cases where our epoch time is wrong
     del request.headers['X-RateLimit-Reset']
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['X-RateLimit-Reset'] = \
-        (datetime.utcnow() - epoch).total_seconds() + 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() + 1
     request.headers['X-RateLimit-Remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['X-RateLimit-Reset'] = \
-        (datetime.utcnow() - epoch).total_seconds() - 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() - 1
     request.headers['X-RateLimit-Remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our limits to always work
     request.headers['X-RateLimit-Reset'] = \
-        (datetime.utcnow() - epoch).total_seconds()
+        (datetime.now(timezone.utc) - epoch).total_seconds()
     request.headers['X-RateLimit-Remaining'] = 1
     obj.ratelimit_remaining = 1
 
     # Cause content response to be None
     request.content = None
     assert obj.send(body="test") is True
```

### Comparing `apprise-1.4.0/test/test_plugin_glib.py` & `apprise-1.4.5/test/test_plugin_glib.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_gnome.py` & `apprise-1.4.5/test/test_plugin_gnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_google_chat.py` & `apprise-1.4.5/test/test_plugin_google_chat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_gotify.py` & `apprise-1.4.5/test/test_plugin_gotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_growl.py` & `apprise-1.4.5/test/test_plugin_growl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_guilded.py` & `apprise-1.4.5/test/test_plugin_guilded.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_homeassistant.py` & `apprise-1.4.5/test/test_plugin_homeassistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_ifttt.py` & `apprise-1.4.5/test/test_plugin_ifttt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_join.py` & `apprise-1.4.5/test/test_plugin_join.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_kavenegar.py` & `apprise-1.4.5/test/test_plugin_kavenegar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_kumulos.py` & `apprise-1.4.5/test/test_plugin_kumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_lametric.py` & `apprise-1.4.5/test/test_plugin_lametric.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_line.py` & `apprise-1.4.5/test/test_plugin_line.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_macosx.py` & `apprise-1.4.5/test/test_plugin_macosx.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_mailgun.py` & `apprise-1.4.5/test/test_plugin_mailgun.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_mastodon.py` & `apprise-1.4.5/test/test_plugin_mastodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 import os
 from unittest import mock
 
 import requests
 from json import dumps, loads
 from datetime import datetime
+from datetime import timezone
 from apprise import Apprise
 from apprise import NotifyType
 from apprise import AppriseAttachment
 from apprise.plugins.NotifyMastodon import NotifyMastodon
 from helpers import AppriseURLTester
 
 # Disable logging for a cleaner testing output
@@ -171,21 +172,22 @@
 
     response_obj = {
         'username': 'caronc',
         'id': 1234,
     }
 
     # Epoch time:
-    epoch = datetime.utcfromtimestamp(0)
+    epoch = datetime.fromtimestamp(0, timezone.utc)
 
     request = mock.Mock()
     request.content = dumps(response_obj)
     request.status_code = requests.codes.ok
     request.headers = {
-        'X-RateLimit-Limit': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Limit': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
 
     # Prepare Mock
     mock_get.return_value = request
     mock_post.return_value = request
 
@@ -227,29 +229,29 @@
 
     # Handle cases where our epoch time is wrong
     del request.headers['X-RateLimit-Limit']
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['X-RateLimit-Limit'] = \
-        (datetime.utcnow() - epoch).total_seconds() + 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() + 1
     request.headers['X-RateLimit-Remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['X-RateLimit-Limit'] = \
-        (datetime.utcnow() - epoch).total_seconds() - 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() - 1
     request.headers['X-RateLimit-Remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our limits to always work
     request.headers['X-RateLimit-Limit'] = \
-        (datetime.utcnow() - epoch).total_seconds()
+        (datetime.now(timezone.utc) - epoch).total_seconds()
     request.headers['X-RateLimit-Remaining'] = 1
     obj.ratelimit_remaining = 1
 
     # Alter pending targets
     obj.targets.append('usera')
     request.content = dumps(response_obj)
     response_obj = {
```

### Comparing `apprise-1.4.0/test/test_plugin_matrix.py` & `apprise-1.4.5/test/test_plugin_matrix.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_mattermost.py` & `apprise-1.4.5/test/test_plugin_mattermost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_messagebird.py` & `apprise-1.4.5/test/test_plugin_messagebird.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_misskey.py` & `apprise-1.4.5/test/test_plugin_misskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_mqtt.py` & `apprise-1.4.5/test/test_plugin_mqtt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_msg91.py` & `apprise-1.4.5/test/test_plugin_msg91.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_msteams.py` & `apprise-1.4.5/test/test_plugin_msteams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_nextcloud.py` & `apprise-1.4.5/test/test_plugin_nextcloud.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_nextcloudtalk.py` & `apprise-1.4.5/test/test_plugin_nextcloudtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_notica.py` & `apprise-1.4.5/test/test_plugin_notica.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_notifico.py` & `apprise-1.4.5/test/test_plugin_notifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_ntfy.py` & `apprise-1.4.5/test/test_plugin_ntfy.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_office365.py` & `apprise-1.4.5/test/test_plugin_office365.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_onesignal.py` & `apprise-1.4.5/test/test_plugin_onesignal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_opsgenie.py` & `apprise-1.4.5/test/test_plugin_opsgenie.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pagerduty.py` & `apprise-1.4.5/test/test_plugin_pagerduty.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pagertree.py` & `apprise-1.4.5/test/test_plugin_pagertree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_parse_platform.py` & `apprise-1.4.5/test/test_plugin_parse_platform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_popcorn_notify.py` & `apprise-1.4.5/test/test_plugin_popcorn_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_prowl.py` & `apprise-1.4.5/test/test_plugin_prowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pushbullet.py` & `apprise-1.4.5/test/test_plugin_pushbullet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pushed.py` & `apprise-1.4.5/test/test_plugin_pushed.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pushjet.py` & `apprise-1.4.5/test/test_plugin_pushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_pushover.py` & `apprise-1.4.5/test/test_plugin_pushover.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     ('pover://:@/', {
         'instance': TypeError,
     }),
     # APIkey; no user
     ('pover://%s' % ('a' * 30), {
         'instance': TypeError,
     }),
-    # API Key + invalid sound setting
-    ('pover://%s@%s?sound=invalid' % ('u' * 30, 'a' * 30), {
-        'instance': TypeError,
+    # API Key + custom sound setting
+    ('pover://%s@%s?sound=mysound' % ('u' * 30, 'a' * 30), {
+        'instance': NotifyPushover,
     }),
     # API Key + valid alternate sound picked
     ('pover://%s@%s?sound=spacealarm' % ('u' * 30, 'a' * 30), {
         'instance': NotifyPushover,
     }),
     # API Key + valid url_title with url
     ('pover://%s@%s?url=my-url&url_title=title' % ('u' * 30, 'a' * 30), {
```

### Comparing `apprise-1.4.0/test/test_plugin_pushsafer.py` & `apprise-1.4.5/test/test_plugin_pushsafer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_reddit.py` & `apprise-1.4.5/test/test_plugin_reddit.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from apprise.plugins.NotifyReddit import NotifyReddit
 from helpers import AppriseURLTester
 from unittest import mock
 
 from json import dumps
 from datetime import datetime
 from datetime import timedelta
+from datetime import timezone
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
@@ -246,15 +247,15 @@
         'app_secret': 'b' * 20,
         'user': 'user',
         'password': 'pasword',
         'targets': 'apprise',
     }
 
     # Epoch time:
-    epoch = datetime.utcfromtimestamp(0)
+    epoch = datetime.fromtimestamp(0, timezone.utc)
 
     good_response = mock.Mock()
     good_response.content = dumps({
         "access_token": 'abc123',
         "token_type": "bearer",
         "expires_in": 100000,
         "scope": '*',
@@ -263,15 +264,16 @@
         "json": {
             # No errors during post
             "errors": [],
         },
     })
     good_response.status_code = requests.codes.ok
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
 
     # Prepare Mock
     mock_post.return_value = good_response
 
     # Variation Initializations
@@ -292,67 +294,73 @@
     assert obj.ratelimit_remaining == 1
 
     # Return the status
     mock_post.return_value = good_response
 
     # Force a case where there are no more remaining posts allowed
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 0,
     }
     # behind the scenes, it should cause us to update our rate limit
     assert obj.send(body="test") is True
     assert obj.ratelimit_remaining == 0
 
     # This should cause us to block
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 10,
     }
     assert obj.send(body="test") is True
     assert obj.ratelimit_remaining == 10
 
     # Handle cases where we simply couldn't get this field
     del good_response.headers['X-RateLimit-Remaining']
     assert obj.send(body="test") is True
     # It remains set to the last value
     assert obj.ratelimit_remaining == 10
 
     # Reset our variable back to 1
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
     # Handle cases where our epoch time is wrong
     del good_response.headers['X-RateLimit-Reset']
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds() + 1,
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds() + 1,
         'X-RateLimit-Remaining': 0,
     }
 
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds() - 1,
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds() - 1,
         'X-RateLimit-Remaining': 0,
     }
     assert obj.send(body="test") is True
 
     # Return our limits to always work
     obj.ratelimit_remaining = 1
 
     # Invalid JSON
     response = mock.Mock()
     response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
     response.content = '{'
     response.status_code = requests.codes.ok
     mock_post.return_value = response
     obj = NotifyReddit(**kwargs)
     assert obj.send(body="test") is False
@@ -389,15 +397,16 @@
         "json": {
             # No errors during post
             "errors": [],
         },
     })
     good_response.status_code = requests.codes.ok
     good_response.headers = {
-        'X-RateLimit-Reset': (datetime.utcnow() - epoch).total_seconds(),
+        'X-RateLimit-Reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'X-RateLimit-Remaining': 1,
     }
 
     # Reset our mock object
     mock_post.reset_mock()
 
     # Test sucessful re-authentication after failed post
```

### Comparing `apprise-1.4.0/test/test_plugin_rocket_chat.py` & `apprise-1.4.5/test/test_plugin_rocket_chat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_ryver.py` & `apprise-1.4.5/test/test_plugin_ryver.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_sendgrid.py` & `apprise-1.4.5/test/test_plugin_sendgrid.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_serverchan.py` & `apprise-1.4.5/test/test_plugin_serverchan.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_ses.py` & `apprise-1.4.5/test/test_plugin_ses.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_signal.py` & `apprise-1.4.5/test/test_plugin_signal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_simplepush.py` & `apprise-1.4.5/test/test_plugin_simplepush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_sinch.py` & `apprise-1.4.5/test/test_plugin_sinch.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_slack.py` & `apprise-1.4.5/test/test_plugin_slack.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_smseagle.py` & `apprise-1.4.5/test/test_plugin_smseagle.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_smtp2go.py` & `apprise-1.4.5/test/test_plugin_smtp2go.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_sns.py` & `apprise-1.4.5/test/test_plugin_sns.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_sparkpost.py` & `apprise-1.4.5/test/test_plugin_sparkpost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_spontit.py` & `apprise-1.4.5/test/test_plugin_spontit.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_streamlabs.py` & `apprise-1.4.5/test/test_plugin_streamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_syslog.py` & `apprise-1.4.5/test/test_plugin_syslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_techululs_push.py` & `apprise-1.4.5/test/test_plugin_techululs_push.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_telegram.py` & `apprise-1.4.5/test/test_plugin_telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
     ('tgram://bottest@123456789:abcdefg_hijklmnop/id1/?topic=12345', {
         'instance': NotifyTelegram,
     }),
     # Threads must be numeric
     ('tgram://bottest@123456789:abcdefg_hijklmnop/id1/?topic=invalid', {
         'instance': TypeError,
     }),
+    # content must be 'before' or 'after'
+    ('tgram://bottest@123456789:abcdefg_hijklmnop/id1/?content=invalid', {
+        'instance': TypeError,
+    }),
     # Testing image
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?image=Yes', {
         'instance': NotifyTelegram,
     }),
     # Testing invalid format (fall's back to html)
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=invalid', {
         'instance': NotifyTelegram,
@@ -409,26 +413,34 @@
     assert mock_post.call_count == 1
     payload = loads(mock_post.call_args_list[0][1]['data'])
 
     # Test our payload
     assert payload['text'] == \
         '<b>special characters</b>\r\n\'"This can\'t\t\r\nfail us"\'\r\n'
 
-    # Test sending attachments
-    attach = AppriseAttachment(os.path.join(TEST_VAR_DIR, 'apprise-test.gif'))
-    assert obj.notify(
-        body='body', title='title', notify_type=NotifyType.INFO,
-        attach=attach) is True
-
-    # An invalid attachment will cause a failure
-    path = os.path.join(TEST_VAR_DIR, '/invalid/path/to/an/invalid/file.jpg')
-    attach = AppriseAttachment(path)
-    assert obj.notify(
-        body='body', title='title', notify_type=NotifyType.INFO,
-        attach=path) is False
+    for content in ('before', 'after'):
+        # Test our content settings
+        obj = NotifyTelegram(
+            bot_token=bot_token, targets='12345', content=content)
+        # Reset our mock
+        mock_post.reset_mock()
+        # Test sending attachments
+        attach = AppriseAttachment(
+            os.path.join(TEST_VAR_DIR, 'apprise-test.gif'))
+        assert obj.notify(
+            body='body', title='title', notify_type=NotifyType.INFO,
+            attach=attach) is True
+
+        # An invalid attachment will cause a failure
+        path = os.path.join(
+            TEST_VAR_DIR, '/invalid/path/to/an/invalid/file.jpg')
+        attach = AppriseAttachment(path)
+        assert obj.notify(
+            body='body', title='title', notify_type=NotifyType.INFO,
+            attach=path) is False
 
     obj = NotifyTelegram(bot_token=bot_token, targets=None)
     # No user detected; this happens after our firsst notification
     assert len(obj.targets) == 0
 
     assert obj.notify(title='hello', body='world') is True
     assert len(obj.targets) == 1
```

### Comparing `apprise-1.4.0/test/test_plugin_twilio.py` & `apprise-1.4.5/test/test_plugin_twilio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_twist.py` & `apprise-1.4.5/test/test_plugin_twist.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_twitter.py` & `apprise-1.4.5/test/test_plugin_twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import json
 import logging
 import os
 from datetime import datetime
+from datetime import timezone
 from unittest.mock import Mock, patch
 
 import pytest
 import requests
 
 from apprise import Apprise
 from apprise import NotifyType
@@ -337,21 +338,22 @@
 
     response_obj = [{
         'screen_name': TWITTER_SCREEN_NAME,
         'id': 9876,
     }]
 
     # Epoch time:
-    epoch = datetime.utcfromtimestamp(0)
+    epoch = datetime.fromtimestamp(0, timezone.utc)
 
     request = Mock()
     request.content = json.dumps(response_obj)
     request.status_code = requests.codes.ok
     request.headers = {
-        'x-rate-limit-reset': (datetime.utcnow() - epoch).total_seconds(),
+        'x-rate-limit-reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'x-rate-limit-remaining': 1,
     }
 
     # Prepare Mock
     mock_get.return_value = request
     mock_post.return_value = request
 
@@ -398,29 +400,29 @@
 
     # Handle cases where our epoch time is wrong
     del request.headers['x-rate-limit-reset']
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['x-rate-limit-reset'] = \
-        (datetime.utcnow() - epoch).total_seconds() + 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() + 1
     request.headers['x-rate-limit-remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our object, but place it in the future forcing us to block
     request.headers['x-rate-limit-reset'] = \
-        (datetime.utcnow() - epoch).total_seconds() - 1
+        (datetime.now(timezone.utc) - epoch).total_seconds() - 1
     request.headers['x-rate-limit-remaining'] = 0
     obj.ratelimit_remaining = 0
     assert obj.send(body="test") is True
 
     # Return our limits to always work
     request.headers['x-rate-limit-reset'] = \
-        (datetime.utcnow() - epoch).total_seconds()
+        (datetime.now(timezone.utc) - epoch).total_seconds()
     request.headers['x-rate-limit-remaining'] = 1
     obj.ratelimit_remaining = 1
 
     # Alter pending targets
     obj.targets.append('usera')
     request.content = json.dumps(response_obj)
     response_obj = [{
@@ -591,18 +593,19 @@
     NotifyTwitter() DM Attachment Checks - Basic
     """
 
     mock_get = mocker.patch("requests.get")
     mock_post = mocker.patch("requests.post")
 
     # Epoch time:
-    epoch = datetime.utcfromtimestamp(0)
+    epoch = datetime.fromtimestamp(0, timezone.utc)
     mock_get.return_value = good_message_response
     mock_post.return_value.headers = {
-        'x-rate-limit-reset': (datetime.utcnow() - epoch).total_seconds(),
+        'x-rate-limit-reset': (
+            datetime.now(timezone.utc) - epoch).total_seconds(),
         'x-rate-limit-remaining': 1,
     }
 
     # The first response is for uploading the attachment,
     # the second one for posting the actual message.
     mock_post.side_effect = [good_media_response, good_message_response]
```

### Comparing `apprise-1.4.0/test/test_plugin_voipms.py` & `apprise-1.4.5/test/test_plugin_voipms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_vonage.py` & `apprise-1.4.5/test/test_plugin_vonage.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_webex_teams.py` & `apprise-1.4.5/test/test_plugin_webex_teams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_windows.py` & `apprise-1.4.5/test/test_plugin_windows.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_xbmc_kodi.py` & `apprise-1.4.5/test/test_plugin_xbmc_kodi.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_plugin_zulip.py` & `apprise-1.4.5/test/test_plugin_zulip.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/test_rest_plugins.py` & `apprise-1.4.5/test/test_rest_plugins.py`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/01_test_example.html` & `apprise-1.4.5/test/var/01_test_example.html`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/apprise-test.gif` & `apprise-1.4.5/test/var/apprise-test.gif`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/apprise-test.jpeg` & `apprise-1.4.5/test/var/apprise-test.jpeg`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/apprise-test.mp4` & `apprise-1.4.5/test/var/apprise-test.mp4`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/apprise-test.png` & `apprise-1.4.5/test/var/apprise-test.png`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/fcm/service_account-bad-type.json` & `apprise-1.4.5/test/var/fcm/service_account-bad-type.json`

 * *Files identical despite different names*

### Comparing `apprise-1.4.0/test/var/fcm/service_account.json` & `apprise-1.4.5/test/var/fcm/service_account.json`

 * *Files identical despite different names*

