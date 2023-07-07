# Comparing `tmp/pyghelpers-1.0.3.tar.gz` & `tmp/pyghelpers-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghelpers-1.0.3.tar", last modified: Sun Nov  7 20:28:10 2021, max compression
+gzip compressed data, was "pyghelpers-1.0.41.tar", last modified: Fri Jul  7 17:23:44 2023, max compression
```

## Comparing `pyghelpers-1.0.3.tar` & `pyghelpers-1.0.41.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.745041 pyghelpers-1.0.3/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      160 2018-12-25 05:37:38.000000 pyghelpers-1.0.3/MANIFEST.in
--rw-r--r--   0 irvkalb    (501) staff       (20)      544 2021-11-07 20:28:10.744786 pyghelpers-1.0.3/PKG-INFO
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      723 2021-10-14 15:58:57.000000 pyghelpers-1.0.3/README
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.685526 pyghelpers-1.0.3/pyghelpers/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-13 19:35:54.000000 pyghelpers-1.0.3/pyghelpers/__init__.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     5138 2021-11-06 23:06:05.000000 pyghelpers-1.0.3/pyghelpers/conf.py
--rw-r--r--   0 irvkalb    (501) staff       (20)    39887 2021-11-05 23:21:16.000000 pyghelpers-1.0.3/pyghelpers/pyghelpers.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.687554 pyghelpers-1.0.3/pyghelpers.egg-info/
--rw-r--r--   0 irvkalb    (501) staff       (20)      544 2021-11-07 20:28:10.000000 pyghelpers-1.0.3/pyghelpers.egg-info/PKG-INFO
--rw-r--r--   0 irvkalb    (501) staff       (20)     4759 2021-11-07 20:28:10.000000 pyghelpers-1.0.3/pyghelpers.egg-info/SOURCES.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)        1 2021-11-07 20:28:10.000000 pyghelpers-1.0.3/pyghelpers.egg-info/dependency_links.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       28 2021-11-07 20:28:10.000000 pyghelpers-1.0.3/pyghelpers.egg-info/requires.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       27 2021-11-07 20:28:10.000000 pyghelpers-1.0.3/pyghelpers.egg-info/top_level.txt
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.687814 pyghelpers-1.0.3/pyghelpers_test/
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.688571 pyghelpers-1.0.3/pyghelpers_test/DialogTester/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     7995 2020-11-14 22:08:05.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/Main_DialogTester.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.701865 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    21412 2018-06-19 19:45:14.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22141 2018-06-19 19:43:10.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22283 2018-06-19 19:38:50.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22264 2018-06-19 19:46:32.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19027 2018-06-19 19:58:28.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18893 2018-06-19 19:59:34.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18985 2018-06-19 20:00:54.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18986 2018-06-19 20:02:18.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/controlsBackground.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3645 2018-05-15 17:35:14.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/dialog.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    26577 2018-05-15 23:37:20.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/highScoresBackground.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1497 2018-06-16 21:51:20.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1695 2018-06-16 21:51:52.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1606 2018-06-16 21:48:48.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1621 2018-06-16 21:53:06.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19119 2018-06-19 20:15:20.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19825 2018-06-19 20:16:32.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19916 2018-06-19 20:17:42.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19936 2018-06-19 20:18:50.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17066 2018-06-19 20:12:52.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17631 2018-06-19 20:11:38.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17722 2018-06-19 20:09:16.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17663 2018-06-19 20:06:54.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1797 2018-06-16 21:50:56.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1959 2018-06-16 21:52:16.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1834 2018-06-16 21:48:36.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1896 2018-06-16 21:52:48.000000 pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesOver.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.708762 pyghelpers-1.0.3/pyghelpers_test/Dodger/
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2812 2021-09-06 20:00:39.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/Baddies.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)      445 2021-08-09 04:29:01.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/Constants.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     3599 2021-07-29 04:18:53.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/Goodies.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2468 2021-09-05 19:48:00.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/HighScoresData.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     1090 2021-09-06 19:17:49.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/Main_Dodger.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)      860 2021-09-05 19:23:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/Player.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-06-24 22:19:51.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneExample.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     8159 2021-09-05 19:39:41.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneHighScores.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     9837 2021-09-05 19:14:11.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/ScenePlay.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-07-28 03:38:15.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneSplash.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.741540 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    24713 2021-09-05 17:52:14.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    23298 2021-09-05 17:46:48.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    26868 2021-09-05 17:44:38.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    22706 2021-09-05 17:49:02.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     4571 2021-08-03 16:14:09.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3796 2021-08-03 16:06:41.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6270 2021-08-03 15:50:18.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     2696 2021-08-03 16:01:52.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     2416 2018-12-19 17:45:20.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/baddie.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13447 2018-12-16 06:45:56.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13214 2018-12-16 06:46:48.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    14317 2018-12-16 06:45:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12926 2018-12-16 06:46:24.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/controlsBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6005 2018-09-03 02:09:30.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/dialog.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3602 2018-12-19 18:59:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/dodger.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     1199 2017-01-11 03:50:38.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gameOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3078 2018-12-19 17:45:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/goodie.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    17632 2018-12-19 00:36:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    16540 2018-12-19 00:36:58.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    18691 2018-12-19 00:35:54.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    15948 2018-12-19 00:36:36.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    65967 2018-09-02 05:38:44.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     9456 2018-12-16 05:42:22.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8681 2018-12-16 05:44:14.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    10087 2018-12-16 05:41:04.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8375 2018-12-16 05:42:46.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13980 2018-12-16 06:31:54.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13080 2018-12-16 06:32:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    15081 2018-12-16 06:31:38.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12490 2018-12-16 06:32:20.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13388 2018-12-16 06:49:26.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13000 2018-12-16 06:50:12.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    14237 2018-12-16 06:48:44.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12689 2018-12-16 06:49:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)      913 2011-03-26 00:48:20.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/player.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5853 2018-12-16 03:12:28.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5770 2018-12-16 03:13:36.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6225 2018-12-16 03:12:08.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5671 2018-12-16 03:12:46.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7511 2018-12-16 05:02:42.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7054 2018-12-16 05:04:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7909 2018-12-16 05:02:06.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6675 2018-12-16 05:03:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   133232 2018-09-02 05:47:28.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/splashBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6102 2018-12-16 03:05:44.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5847 2018-12-16 03:06:54.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8004 2018-12-16 05:20:00.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7937 2018-12-16 05:19:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     9086 2018-12-16 05:20:16.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8495 2018-12-16 05:19:32.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7214 2018-12-16 03:05:00.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6517 2018-12-16 03:06:38.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startOver.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-11-07 20:28:10.743368 pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7162 2011-03-26 00:48:20.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/background.mid
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   123716 2017-01-06 04:16:32.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/ding.wav
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   258876 2011-03-26 00:48:20.000000 pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/gameover.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.3/pyghelpers_test/__init__.py
--rw-r--r--   0 irvkalb    (501) staff       (20)       38 2021-11-07 20:28:10.745119 pyghelpers-1.0.3/setup.cfg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      797 2021-10-14 15:52:01.000000 pyghelpers-1.0.3/setup.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.584655 pyghelpers-1.0.41/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pyghelpers-1.0.41/LICENSE
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      160 2018-12-25 05:37:38.000000 pyghelpers-1.0.41/MANIFEST.in
+-rw-r--r--   0 irvkalb    (501) staff       (20)      519 2023-07-07 17:23:44.584066 pyghelpers-1.0.41/PKG-INFO
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1796 2023-06-27 22:58:33.000000 pyghelpers-1.0.41/README
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.526203 pyghelpers-1.0.41/pyghelpers/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-13 19:35:54.000000 pyghelpers-1.0.41/pyghelpers/__init__.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     5192 2023-07-07 17:20:46.000000 pyghelpers-1.0.41/pyghelpers/conf.py
+-rw-r--r--   0 irvkalb    (501) staff       (20)    51238 2023-07-05 17:17:20.000000 pyghelpers-1.0.41/pyghelpers/pyghelpers.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.527941 pyghelpers-1.0.41/pyghelpers.egg-info/
+-rw-r--r--   0 irvkalb    (501) staff       (20)      519 2023-07-07 17:23:44.000000 pyghelpers-1.0.41/pyghelpers.egg-info/PKG-INFO
+-rw-r--r--   0 irvkalb    (501) staff       (20)     4767 2023-07-07 17:23:44.000000 pyghelpers-1.0.41/pyghelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-07 17:23:44.000000 pyghelpers-1.0.41/pyghelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       31 2023-07-07 17:23:44.000000 pyghelpers-1.0.41/pyghelpers.egg-info/requires.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-07 17:23:44.000000 pyghelpers-1.0.41/pyghelpers.egg-info/top_level.txt
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.528366 pyghelpers-1.0.41/pyghelpers_test/
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.528879 pyghelpers-1.0.41/pyghelpers_test/DialogTester/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     7714 2023-07-05 17:35:47.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/Main_DialogTester.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.544918 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    21412 2018-06-19 19:45:14.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22141 2018-06-19 19:43:10.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22283 2018-06-19 19:38:50.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22264 2018-06-19 19:46:32.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19027 2018-06-19 19:58:28.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18893 2018-06-19 19:59:34.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18985 2018-06-19 20:00:54.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18986 2018-06-19 20:02:18.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/controlsBackground.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3645 2018-05-15 17:35:14.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/dialog.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    26577 2018-05-15 23:37:20.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/highScoresBackground.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1497 2018-06-16 21:51:20.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1695 2018-06-16 21:51:52.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1606 2018-06-16 21:48:48.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1621 2018-06-16 21:53:06.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19119 2018-06-19 20:15:20.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19825 2018-06-19 20:16:32.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19916 2018-06-19 20:17:42.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19936 2018-06-19 20:18:50.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17066 2018-06-19 20:12:52.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17631 2018-06-19 20:11:38.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17722 2018-06-19 20:09:16.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17663 2018-06-19 20:06:54.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1797 2018-06-16 21:50:56.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1959 2018-06-16 21:52:16.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1834 2018-06-16 21:48:36.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1896 2018-06-16 21:52:48.000000 pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesOver.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.550633 pyghelpers-1.0.41/pyghelpers_test/Dodger/
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2812 2021-09-06 20:00:39.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/Baddies.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)      445 2021-08-09 04:29:01.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/Constants.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     3599 2021-07-29 04:18:53.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/Goodies.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2468 2021-09-05 19:48:00.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/HighScoresData.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     1169 2023-07-05 17:21:38.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/Main_Dodger.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)      847 2021-11-23 19:31:34.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/Player.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-06-24 22:19:51.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneExample.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     8159 2021-09-05 19:39:41.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneHighScores.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     9837 2021-09-05 19:14:11.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/ScenePlay.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-07-28 03:38:15.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneSplash.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.579344 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    24713 2021-09-05 17:52:14.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    23298 2021-09-05 17:46:48.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    26868 2021-09-05 17:44:38.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    22706 2021-09-05 17:49:02.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     4571 2021-08-03 16:14:09.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3796 2021-08-03 16:06:41.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6270 2021-08-03 15:50:18.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     2696 2021-08-03 16:01:52.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     2416 2018-12-19 17:45:20.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/baddie.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13447 2018-12-16 06:45:56.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13214 2018-12-16 06:46:48.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    14317 2018-12-16 06:45:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12926 2018-12-16 06:46:24.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/controlsBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6005 2018-09-03 02:09:30.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/dialog.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3602 2018-12-19 18:59:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/dodger.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     1199 2017-01-11 03:50:38.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gameOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3078 2018-12-19 17:45:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/goodie.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    17632 2018-12-19 00:36:16.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    16540 2018-12-19 00:36:58.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    18691 2018-12-19 00:35:54.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    15948 2018-12-19 00:36:36.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    65967 2018-09-02 05:38:44.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     9456 2018-12-16 05:42:22.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8681 2018-12-16 05:44:14.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    10087 2018-12-16 05:41:04.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8375 2018-12-16 05:42:46.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13980 2018-12-16 06:31:54.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13080 2018-12-16 06:32:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    15081 2018-12-16 06:31:38.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12490 2018-12-16 06:32:20.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13388 2018-12-16 06:49:26.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13000 2018-12-16 06:50:12.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    14237 2018-12-16 06:48:44.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12689 2018-12-16 06:49:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)      913 2011-03-26 00:48:20.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/player.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5853 2018-12-16 03:12:28.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5770 2018-12-16 03:13:36.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6225 2018-12-16 03:12:08.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5671 2018-12-16 03:12:46.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7511 2018-12-16 05:02:42.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7054 2018-12-16 05:04:16.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7909 2018-12-16 05:02:06.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6675 2018-12-16 05:03:16.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   133232 2018-09-02 05:47:28.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/splashBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6102 2018-12-16 03:05:44.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5847 2018-12-16 03:06:54.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8004 2018-12-16 05:20:00.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7937 2018-12-16 05:19:16.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     9086 2018-12-16 05:20:16.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8495 2018-12-16 05:19:32.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7214 2018-12-16 03:05:00.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6517 2018-12-16 03:06:38.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startOver.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 17:23:44.581847 pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7162 2011-03-26 00:48:20.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/background.mid
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   123716 2017-01-06 04:16:32.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/ding.wav
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   258876 2011-03-26 00:48:20.000000 pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/gameover.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.41/pyghelpers_test/__init__.py
+-rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-07 17:23:44.584781 pyghelpers-1.0.41/setup.cfg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      782 2023-07-07 17:20:40.000000 pyghelpers-1.0.41/setup.py
```

### Comparing `pyghelpers-1.0.3/pyghelpers/conf.py` & `pyghelpers-1.0.41/pyghelpers/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 
 import os
 import sys
 
-print('Inserting this into the os search path', os.path.join(os.path.dirname(__file__)), 'pyghelpers')
+print('Inserting this into the os search path', os.path.dirname(os.path.dirname(__file__)))
+print()
 
-sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'pyghelpers'))
+sys.path.insert(0, os.path.dirname(os.path.dirname(__file__)))
 
 #print()
 #for path in sys.path:
 #    print(path)
 #print()
 
 
@@ -31,22 +32,23 @@
 project = 'pyghelpers'
 copyright = '2019, Irv Kalb'
 author = 'Irv Kalb'
 
 # The short X.Y version
 version = '1.0'
 # The full version, including alpha/beta/rc tags
-release = '1.0.3'
+release = '1.0.41'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
-# needs_sphinx = '1.0'
+needs_sphinx = '7.0.1'
+toc_object_entries = False  # Added 6/23 to only show class names
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc'
 ]
@@ -66,15 +68,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -82,21 +84,21 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'classic' # sphinx_rtd_theme'
+html_theme = 'classic' 
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
-#html_theme_options = {}
+html_theme_options = {'stickysidebar': True}
 
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = [ ]  # was:   ['_static']   IK 8/19
```

### Comparing `pyghelpers-1.0.3/pyghelpers/pyghelpers.py` & `pyghelpers-1.0.41/pyghelpers/pyghelpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 - textYesNoDialog - a text-based dialog box allowing for one or two answers (yes/no, or just OK)
 - customYesNoDialog - a dialog box with custom graphics (yes/no, or just OK)
 - textAnswerDialog - a text-based dialog box allowing the user to enter a string
 - customAnswerDialog - a dialog box with custom graphics that allows the user to enter a string
 
 
-Many helpers allow the use of a callback (a function or method to be called when an action happens)
+While not required, manyhelpers allow the use of a callback (a function or method to be called when an action happens)
     Any widget that uses a callback should be set up like this: 
     def <callbackMethodName>(self, nickName):
     When the appropriate action happens, the callback method will be called and the nickName will be passed.
     If you don't need the nickname, you can just ignore that parameter
 
 """
 """
@@ -63,23 +63,42 @@
 or implied, of Irv Kalb.
 
 ******************************************************************************************
 
 
 History:
 
+6/23 Version 1.1
+    Big change to startup:
+       The main program should now create a dictionary of sceneKey: sceneObject pairs
+           and get pass this in when creating the SceneMgr.
+       This eliminates the earlier need for each scene to have a getSceneKey() method.
+       (The old approach is still supported for backward compatibility)
+    Added addScene to add a scene dynamically (pass in a sceneKey and sceneObject)
+    Added removeScene to remove an existing scene to free up memory (pass in a sceneKey)
+       (This can be called from the current scene, as long as the next line is a gotoScene)
+2/23
+    Added code in all timers to check for and handle multiple pauses and resumes.
+    In CountDownTimer made ended() method check the time
+       Client code doesn't need to call getTime()   Suggested by Lando Chan
+    In CountUpTimer and CountDown timer added forceFullHHMMSS for full HH:MM:SS presentation
+10/22
+   SceneMgr:  Added optional frame rate display for debugging
+4/22
+    Timer, CountUpTimer, CountDownTimer: Added pause() and resume()
+
 11/21  Version 1.0.3
     Cleaned up some documentation of parameters
     Removed all FileIO functions
     Added __all__ to define what gets imported when you import *
     Change the SceneMgr so you pass in list of Scenes objects instead of a dictionary.
        Each scene must implement getSceenKey to define the scene key.
        First scene in the list is the starting scene.
     Use ABC for abstract base class and abstract methods
-    Updated code using f strings in Timer's getTimeHHMMSS, and clean up of timers
+    Updated code using f strings in Timer's getTimeInHHMMSS, and clean up of timers
     Turn off key repeating when going to a new scene
     Changed SceneMgr _goToScene method to goToScene
 
 5/26/20  Version 1.0.2
     Added __version__  and function  getVersion()
 
 Version 1.0     01/13/20
@@ -101,32 +120,26 @@
 ]
 
 import pygame
 from pygame.locals import *
 import pygwidgets
 import sys
 import time
+import os
 from abc import ABC, abstractmethod
 
-__version__ = "1.0.3"
-
 
 def getVersion():
     """Returns the current version number of the pyghelpers package"""
-    return __version__
-
+    version = "1.1"
+    return version
 
-# Timer classes:
-#    Timer (simple)
-#    CountUpTimer
-#    CountDownTimer
 
 
 #  Timer
-
 class Timer():
     """
     This class is used to create a very simple Timer.
 
     Typical use:
 
     1)  Create a Timer object:
@@ -147,34 +160,42 @@
 
     Parameters:
         | timeInSeconds - the duration of the timer, in seconds (integer or float)
 
     Optional keyword parameters:
         | nickname - an internal name to associate with this timer (defaults to None)
         | callback - a function or object.method to be called back when the timer is finished
-        |            The nickname of the timer will be passed in when the callback is made (defaults to None)
-
+        |            The nickname of the timer will be passed in if a callback is made (defaults to None)
 
     """
+
     def __init__(self, timeInSeconds, nickname=None, callBack=None):
         self.timeInSeconds = timeInSeconds
         self.nickname = nickname
         self.callBack = callBack
         self.savedSecondsElapsed = 0.0
         self.running = False
+        self.paused = False
+        self.pauseCounter = 0  # counts how many calls to pause without a resume
 
     def start(self, newTimeInSeconds=None):
         """Start the timer running (starts at zero).
         Allows you to optionally specify a different amount of time.
-        
+
+        Optional keyword parameter:
+        | newTimeInSeconds - a new duration for the timer (integer or float, default None)
+
         """
         if newTimeInSeconds is not None:
             self.timeInSeconds = newTimeInSeconds
         self.running = True
         self.startTime = time.time()
+        self.paused = False
+        self.timePaused = None
+        self.pauseCounter = 0
 
     def update(self):
         """Call this in every frame to update the timer
 
         Returns:
            |   False - most of the time
            |   True - when the timer is finished
@@ -198,27 +219,48 @@
         """ Call this if you want to know how much has elapsed
 
         Returns:
            |   0 - if the Timer is not running
            |   seconds elapsed since start, as a float
 
         """
-        if self.running:
+        if self.running or self.paused:
             self.savedSecondsElapsed = time.time() - self.startTime
-            
+
         return self.savedSecondsElapsed
 
+    def pause(self):
+        """Pauses the timer"""
+        self.pauseCounter = self.pauseCounter + 1
+        self.timePaused = time.time()
+        self.paused = True
+
+    def resume(self):
+        """Resumes the timer after a pause"""
+        if self.pauseCounter == 0:
+            print('Warning - called resume timer but the timer is not paused ... ignored')
+        else:
+            self.pauseCounter = self.pauseCounter -1
+        if self.pauseCounter != 0:
+            return  # don't resume
+
+        # OK to resume
+        pauseTime = time.time() - self.timePaused
+        self.secondsStart = self.secondsStart + pauseTime
+        self.paused = False
+
     def stop(self):
         """Stops the timer"""
-        self.getTime()   # remembers final self.savedSecondsElapsed
+        self.getTime()  # remembers final self.savedSecondsElapsed
         self.running = False
+        self.paused = False
+        self.pauseCounter = 0
 
 
 # CountUpTimer class
-
 class CountUpTimer():
     """
     This class is used to create a Timer that counts up (starting at zero).
 
     Its intended use is where you want to continuously display the time in a window (using a DisplayText object).
 
     Typical use:
@@ -231,19 +273,19 @@
 
         myTimer.start()
 
         This method can also be called to restart the timer.
 
     3)  Whenever you want to get the current time (in seconds since start), you can call any of:
 
-        theTime = pyghelpers.getTime() # gets time as a float
+        theTime = myTimer.getTime() # gets time as a float
 
-        theTime = pyghelpers.getTimeInSeconds() # gets the time as an integer number of seconds
+        theTime = myTimer.getTimeInSeconds() # gets the time as an integer number of seconds
 
-        theTime = pyghelpers.getTimeInHHMMSS() # gets the time in HH:MM:SS string format
+        theTime = myTimer.getTimeInHHMMSS() # gets the time in HH:MM:SS string format
 
         One of the above should be called every time through your main loop.
 
     4)  If you want to stop the timer, call:
 
         myTimer.stop()
 
@@ -253,101 +295,127 @@
 
     """
 
     def __init__(self):
         self.running = False
         self.savedSecondsElapsed = 0.0
         self.secondsStart = 0  # safeguard
+        self.paused = False
+        self.timePaused = None
+        self.pauseCounter = 0  # counts how many calls to pause without a resume
 
     def start(self):
         """Start the timer running (starts at zero).  Can be called to restart the timer, for example to play a game multiple times"""
         self.secondsStart = time.time()  # get the current seconds and save the value
         self.running = True
+        self.paused = False
         self.savedSecondsElapsed = 0.0
+        self.pauseCounter = 0
 
     def getTime(self):
         """Returns the time elapsed as a float"""
-        if not self.running:
+        if not self.running or self.paused:
             return self.savedSecondsElapsed  # do nothing
         
         self.savedSecondsElapsed = time.time() - self.secondsStart
         return self.savedSecondsElapsed  # returns a float
 
     def getTimeInSeconds(self):
         """Returns the time elapsed as an integer number of seconds"""
         nSeconds = int(self.getTime())
         return nSeconds
 
     # Updated version using fStrings
-    def getTimeInHHMMSS(self, nMillisecondsDigits=0):
+    def getTimeInHHMMSS(self, nMillisecondsDigits=0, forceFullHHMMSS= False):
         """Returns the elapsed time as a HH:MM:SS.mmm formatted string
 
         Parameters:
 
         Optional keyword parameters:
             | nMillisecondsDigits - number of milliseconds digits to include (defaults to 0)
-            |    If specified, returned string will look like:    HH:MM:SS.mmm
+            |    If specified, returned string will include nMillisecondsDigits of milliseconds digits
+            | forceFullHHMMSS forces the output to be in full HH:MM:SS format (defaults to False)
 
         """
         nSeconds = self.getTime()
         mins, secs = divmod(nSeconds, 60)
         hours, mins = divmod(int(mins), 60)
 
         if nMillisecondsDigits > 0:
             secondsWidth = nMillisecondsDigits + 3
         else:
             secondsWidth = 2
 
-        if hours > 0:
+        if forceFullHHMMSS:
+            output = f'{hours:02d}:{mins:02d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
+        elif hours > 0:
             output = f'{hours:d}:{mins:02d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
         elif mins > 0:
             output = f'{mins:d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
         else:
             output = f'{secs:.{nMillisecondsDigits}f}'
 
         return output
     
     def stop(self):
         """Stops the timer"""
         self.getTime()   # remembers final self.savedSecondsElapsed
         self.running = False
+        self.paused = False
+        self.pauseCounter = 0
 
-    # To do:  Would be nice to add both pause and continue methods
+    def pause(self):
+        """Pauses the timer"""
+        self.pauseCounter = self.pauseCounter + 1
+        self.timePaused = time.time()
+        self.paused = True
+
+    def resume(self):
+        """Resumes the timer after a pause"""
+        if self.pauseCounter == 0:
+            print('Warning - called resume timer but the timer is not paused ... ignored')
+        else:
+            self.pauseCounter = self.pauseCounter -1
+        if self.pauseCounter != 0:
+            return  # don't resume
+
+        # OK to resume
+        pauseTime = time.time() - self.timePaused
+        self.secondsStart = self.secondsStart + pauseTime
+        self.paused = False
 
 
 
 #
 # CountDownTimer class
 #
 class CountDownTimer():
     """
     This class is used to create a Timer that counts down from a given starting number of seconds.
-
     Its intended use is where you want to continuously display the time in a window (using a DisplayText object).
 
-
     Typical use:
 
     1)  Create a CountDownTimer object:
 
         myTimer = pyghelpers.CountDownTimer(60)   # start the timer at 60 seconds
 
     2)  When you want the timer to start running, make this call:
 
         myTimer.start()
 
         This method can also be used to restart the timer.
 
     3)  Whenever you want to get the remaining time (in seconds since start), you can call any of:
 
-        theTime = pyghelpers.getTime() # gets time as a float
+        theTime = myTimer.getTime() # gets time as a float
 
-        theTime = pyghelpers.getTimeInSeconds() # gets the time as an integer number of seconds
+        theTime = myTimer.getTimeInSeconds() # gets the time as an integer number of seconds
 
-        theTime = pyghelpers.getTimeInHHMMSS() # gets the time in HH:MM:SS string format
+        theTime = myTimer.getTimeInHHMMSS() # gets the time in HH:MM:SS string format
 
     4)  If you want to stop the timer, call:
 
         myTimer.stop()
 
 
     Parameters:
@@ -355,39 +423,42 @@
 
     Optional keyword parameters:
         | stopAtZero - should the timer stop when it reaches zero (defaults to True)
         | nickname - an internal name used to refer to this timer (defaults to None)
         | callback - a function or object.method to be called back when the timer is finished
         |            The nickname of the timer will be passed in when the callback is made (defaults to None)
 
-
     """
 
     def __init__(self, nStartingSeconds, stopAtZero=True, nickname=None, callBack=None):
         self.nStartingSeconds = nStartingSeconds
         self.stopAtZero = stopAtZero
         self.nickname = nickname
         self.callBack = callBack
 
         self.running = False
         self.secondsSavedRemaining = 0.0
         self.reachedZero = False
+        self.pauseCounter = 0  # counts how many calls to pause without a resume
 
     def start(self, newStartingSeconds=None):
         """Start the timer running starting at nStartingSeconds (or optional different setting)"""
         secondsNow = time.time()
         if newStartingSeconds is not None:
             self.nStartingSeconds = newStartingSeconds
         self.secondsEnd = secondsNow + self.nStartingSeconds
         self.reachedZero = False
         self.running = True
+        self.paused = False
+        self.timePaused = None
+        self.pauseCounter = 0
 
     def getTime(self):
         """Returns the remaining time as a float number of seconds"""
-        if not self.running:
+        if not self.running or self.paused:
             return self.secondsSavedRemaining
         
         self.secondsSavedRemaining = self.secondsEnd - time.time()
         if self.stopAtZero and (self.secondsSavedRemaining <= 0):
             self.secondsSavedRemaining = 0.0
             self.running = False
             self.reachedZero = True
@@ -396,151 +467,199 @@
 
     def getTimeInSeconds(self):
         """Returns the remaining time as an integer number of seconds"""
         nSeconds = int(self.getTime())
         return nSeconds
 
     # Updated version using fStrings
-    def getTimeInHHMMSS(self, nMillisecondsDigits=0):
+    def getTimeInHHMMSS(self, nMillisecondsDigits=0, forceFullHHMMSS=False):
         """Returns the remaining time as a HH:MM:SS.mmm formatted string
 
         Parameters:
 
         Optional keyword parameters:
             | nMillisecondsDigits - number of milliseconds digits to include (defaults to 0)
-            |    If specified, returned string will look like:    HH:MM:SS.mmm
+            |    If specified, returned string will include nMillisecondsDigits of milliseconds digits
+            | forceFullHHMMSS forces the output to be in full HH:MM:SS format (defaults to False)
 
         """
         nSeconds = self.getTime()
         mins, secs = divmod(nSeconds, 60)
         hours, mins = divmod(int(mins), 60)
 
         if nMillisecondsDigits > 0:
             secondsWidth = nMillisecondsDigits + 3
         else:
             secondsWidth = 2
 
-        if hours > 0:
+        if forceFullHHMMSS:
+            output = f'{hours:02d}:{mins:02d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
+        elif hours > 0:
             output = f'{hours:d}:{mins:02d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
         elif mins > 0:
             output = f'{mins:d}:{secs:0{secondsWidth}.{nMillisecondsDigits}f}'
         else:
             output = f'{secs:.{nMillisecondsDigits}f}'
 
+
         self.savedSecondsElapsed = output
         return output
 
 
     def stop(self):
         """Stops the timer """
         self.getTime()   # remembers final self.savedSecondsElapsed
         self.running = False
+        self.paused = False
+        self.pauseCounter = 0
         
 
     def ended(self):
         """Call to see if the timer has reached zero. Should be called every time through the loop"""
+        dontCare = self.getTime()   #  called to  set self.reachedZero
         if self.reachedZero:
             self.reachedZero = False  # reset
             if self.callBack is not None:
                 self.callBack(self.nickname)
             return True
         else:
             return False
 
-    # To do:  Would be nice to add both pause and continue methods
+    def pause(self):
+        """Pauses the timer"""
+        self.pauseCounter = self.pauseCounter + 1
+        self.timePaused = time.time()
+        self.paused = True
+
+    def resume(self):
+        """Resumes the timer after a pause"""
+        if self.pauseCounter == 0:
+            print('Warning - called resume timer but the timer is not paused ... ignored')
+        else:
+            self.pauseCounter = self.pauseCounter -1
+        if self.pauseCounter != 0:
+            return  # don't resume
+
+        # OK to resume
+        pauseTime = time.time() - self.timePaused
+        self.secondsStart = self.secondsStart + pauseTime
+        self.paused = False
 
 
 #
-#
 # Scene Manager
 #
-#
 class SceneMgr():
     """SceneMgr (Scene Manager)  allows you to build a program with multiple scenes.
 
     The SceneMgr manages any number of scenes built as subclasses of the "Scene" class.
-    
     For more details, see the "Scene" class.
 
     Typical use:
 
     1) Instantiate as many Scenes as you want:
-        |
         |  oScene1 = StartingScene(window)
         |  oScene2 = MainScene(window)
-        |  oScene3 = SometherScene(window)
+        |  oScene3 = SomeOtherScene(window)
+
+    2) Build a dictionary of these scenes:
+        |  myScenesDict = {'sceneKey1': oScene1, 'sceneKey2': oScene2, 'sceneKey3': oScene3}
 
-    2) Build a list of these scenes:
+        The keys are any unique strings that you want to use.
 
-        myScenesList = [oScene1, oScene2, oScene3]
+            OLDER APPROACH:  Before pyghelpers 1.1, but still works for backwards compatibility
+            Build a list of the scenes:
+            | myScenesList = [oScene1, oScene2, oScene3]
 
     3) Instantiate *one* SceneMgr (a singleton):
+        |  oSceneMgr = SceneMgr(myScenesDict, 30) # First scene in the dict is the starting scene
 
-        oSceneMgr = SceneMgr(myScenesList, 30) # First scene in the list is the starting scene
+            OLDER APPROACH:  Before pyghelpers 1.1, but still works for backwards compatibility
+                oSceneMgr = SceneMgr(myScenesList, 30) # First scene in the list is the starting scene
 
-    4) Call the run method to start the SceneMgr running:
+        You can optionally pass a DisplayText object for showing the frame rate, e.g.
+        |  oDebugFrameRate = pygwidgets.DisplayText(window, (0, 0), '', fontSize=24)
+        |  oSceneMgr = SceneMgr(scenesDictOrList, FRAMES_PER_SECOND, oDebugFrameRate)
 
-        oSceneMgr.run()  # First scene in the list is the starting scene
+    4) Call the run method to start the SceneMgr running:
+        |  oSceneMgr.run()  # First scene in the list is the starting scene
 
 
     Parameters:
-        | scenesList - is a list that consists of:
-        |    [<sceneObject>, <sceneObject>, ...]
+        | scenesDictOrList - is a dictionary or list that consists of:
+        |    {<sceneKey>: <sceneObject>, <sceneKey>: <sceneObject>, ...}
+        |    OR older (before pyghelpers 1.1):  [<sceneObject>, <sceneObject>, ...]
         |      where each sceneObject is an object instantiated from a scene class
         |      (For details on Scenes, see the Scene class)
         | fps - is the frames per second at which the program should run
 
     Based on the concept of a "Scene Manager" by Blake O'Hare of Nerd Paradise (nerdparadise.com)
 
     """
-    def __init__(self, scenesList, fps):
+    def __init__(self, scenesDictOrList, fps, oFrameRateDisplay=None):
 
-        # Build a dictionary, each entry of which is a scene key : scene object
-        self.scenesDict = {}
-        for oScene in scenesList:
-            key = oScene.getSceneKey()  # Each scene must return a unique key to identify itself
-            self.scenesDict[key] = oScene
+        # Newer approach (pyghelpers 1.1), pass in a dictionary of {scene keys: scene objects}
+        # (No need to have each scene implement a getSceneKey method.)
+        if isinstance(scenesDictOrList, dict):
+            self.scenesDict = scenesDictOrList
+            keysList = list(self.scenesDict)  # get all the keys
+            startingKey = keysList[0]  # first key is the starting scene ley
+            self.oCurrentScene = self.scenesDict[startingKey]
+
+        else:  # Older style, we start with a list of scenes
+            # Build a dictionary, each entry of which is a scene key : scene object
+            # Then we call getSceneKey so each scene can identify itself
+            self.scenesDict = {}
+            for oScene in scenesDictOrList:
+                key = oScene.getSceneKey()  # Each scene must return a unique key to identify itself
+                self.scenesDict[key] = oScene
+            # The first element in the list is the used as the starting scene
+            self.oCurrentScene = scenesDictOrList[0]
 
-        # The first element in the list is the used as the starting scene
-        self.oCurrentScene = scenesList[0]
         self.framesPerSecond = fps
+        self.oFrameRateDisplay = oFrameRateDisplay
+        self.showFrameRate = oFrameRateDisplay is not None  # for fast checking in main loop
+        self.scenesToRemoveList = []
 
         # Give each scene a reference back to the SceneMgr.
         # This allows any scene to do a goToScene, request, send,
         # or sendAll, which gets forwarded to the scene manager.
         for key, oScene in self.scenesDict.items():
             oScene._setRefToSceneMgr(self)
 
     def run(self):
-        """ This method implements the main pygame loop.
+        """
+        This method implements the main pygame loop.
 
         It should typically be called as the last line of your main program.
 
         It is designed to call a standardized set of methods in the current scene.
-        
-        All scenes must implement the following methods (polymorphism):
-
-           |    handleInputs  # called in every frame
-           |    draw          # called in every frame
 
+        All scenes must implement the following methods (polymorphism):
+            |   handleInputs()  # called in every frame
+            |   draw()          # called in every frame
 
-        The following methods can be implemented in a scene.  If they are not
-        implemented, then the default version in the Scene base class will be used.
-        (Those methods do not do anything):
+        The following methods can be implemented in a scene:
+            |   enter()  # called once whenever the scene is entered
+            |   update()  # called in every frame
+            |   leave()  # called once whenever the scene is left
 
-           |    enter          # called once whenever the scene is entered
-           |    update       # called in every frame
-           |    leave          # called once whenever the scene is left
+        If any is not implemented, then the version in the Scene base class,
+        which only performs a pass statement, will be used.
 
-        
         """
         clock = pygame.time.Clock()
 
         # 6 - Loop forever
         while True:
+            # If there are any scenes to be removed (keys added by removeScene method)
+            if not(self.scenesToRemoveList is []):
+                for key in self.scenesToRemoveList:
+                    del self.scenesDict[key]
+                self.scenesToRemoveList = []  # reset
 
             keysDownList = pygame.key.get_pressed()
 
             # 7 - Check for and handle events
             eventsList = []
             for event in pygame.event.get():
                 if (event.type == pygame.QUIT) or \
@@ -549,20 +668,24 @@
                     # Tell current scene we're leaving
                     self.oCurrentScene.leave()  
                     pygame.quit()
                     sys.exit()
 
                 eventsList.append(event)
 
-            # Here, we let the current scene process all events,
-            # do any "per frame" actions in its update method,
-            # and draw everything that needs to be drawn.
+            # Here, we let the current scene process all events by calling its handleInputs() method
+            # do any "per frame" actions in its update() method,
+            # and call its draw() method so it can draw everything that needs to be drawn.
             self.oCurrentScene.handleInputs(eventsList, keysDownList)
             self.oCurrentScene.update()
             self.oCurrentScene.draw()
+            if self.showFrameRate:
+                fps = str(clock.get_fps())
+                self.oFrameRateDisplay.setText('FPS: ' + fps)
+                self.oFrameRateDisplay.draw()
 
             # 11 - Update the window
             pygame.display.update()
 
             # 12 - Slow things down a bit
             clock.tick(self.framesPerSecond)
             
@@ -604,79 +727,143 @@
         The target scene must implement a method named "respond"
 
         """
         oTargetScene = self.scenesDict[targetSceneKey]
         info = oTargetScene.respond(requestID)
         return info
 
-
     def _send_receive(self, targetSceneKey, sendID, info):
         """Internal method, called by a Scene, tells the Scene Manager to send information to another scene
 
         (From the sending scene's point of view, it just needs to call its own send method)
         The target scene must implement a method named "receive"
 
         """
         oTargetScene = self.scenesDict[targetSceneKey]
         oTargetScene.receive(sendID, info)
 
-
     def _sendAll_receive(self, oSenderScene, sendID, info):
         """Internal method, called by a Scene tells the Scene Manager to send information to all scenes (other than itself)
 
         (From the sending scene's point of view, it just needs to call its own sendAll method)
         All scenes must implement a method named "receive"
 
         """
         for sceneKey in self.scenesDict:
             oTargetScene = self.scenesDict[sceneKey]
             if oTargetScene != oSenderScene:
                 oTargetScene.receive(sendID, info)
 
+    def _addScene(self, sceneKey, oNewScene):
+        """Called in a Scene, tells the SceneMgr to add a new scene dynamically
+        (From the Scene's point of view, it just needs to call its own addScene method)
+
+        The scene must first instantiate a new Scene object, then call this method
+
+        Parameters:
+            | sceneKey - an key that uniquely identifies this scene (typically a string)
+            | oNewScene - an object of an instance of the new scene
+
+        Raises:
+        |    KeyError - if a scene with the same key already exists (must be unique)
+
+        """
+        # Ask the new scene for its scene key, and add it to the scenes dictionary
+        newSceneKey = oNewScene.getSceneKey()
+        if newSceneKey in self.scenesDict:
+            raise KeyError('Trying to add a scene with key' + newSceneKey + 'but that scene key already exists')
+        self.scenesDict[newSceneKey] = oNewScene
+        # Send the new scene a reference to the SceneMgr
+        oNewScene._setRefToSceneMgr(self)
+
+    def _removeScene(self, sceneKeyToRemove):
+        """Called by a Scene, tells the SceneMgr to remove an existing scene (to free up memory)
+        (From the Scene's point of view, it just needs to call its own remove method)
+
+        Parameter:
+            | sceneKeyToRemove - the scene key of the scene to be eliminated
+
+        Raises:
+            | KeyError if the nextSceneKey is not valid
+
+        """
+        if not(sceneKeyToRemove in self.scenesDict):
+            raise KeyError('Attempting to remove scene with key ' + sceneKeyToRemove +
+                           ' but no scene with that key currently exists (either never defined or removed).')
+        # Add the key to a list of keys to be removed
+        # The scene(s) will be removed the next time around the main loop.from
+        # This allows a scene to make a call to removeScene to remove itself right before doing a goToScene
+        #    (and the call will return successfully)
+        self.scenesToRemoveList.append(sceneKeyToRemove)
+
 
 
 class Scene(ABC):
-    """The Scene class is an abstract class to be used as a base class for any scenes that you want to create.
+    """
+    The Scene class is an abstract class to be used as a base class for any scenes that you want to create.
 
-    At startup, you create an instance of each of your scenes, and pass a list of these scenes objects
-    when you instantiate the scene manager.
+    In the startup code for your  application, you create an instance of each of the
+    scenes that you want to be available.  Then you build a dictionary like this
 
-    In the __init__ method of your scene subclass, you will receive a window reference.
-    You should copy this into an instance variable like this:
+        |    {<sceneKey1>:<sceneObject1>, <sceneKey2>:<sceneObject2>, ...}
+
+    Then you pass this dictionary when you instantiate the Scene Manager.
+    See the SceneMgr documentation for details.
+
+    To create a scene, you must write a subclass that inherits from this class.
+    Your class must implement these methods
+
+        |   __init__(), handleInputs(), draw()
+
+    You will typically overwrite the update() method to do any processing in every frame.
+
+    Other methods can be overridden if you wish:
+
+        | enter(), leave()
+
+    You can add any additional methods that your class requires.
+    Additionally, there are other methods to allow you to get or set info, or navigate to other scenes:
+
+        | goToScene(), quit(), request(), respond() and more.
+
+    In the __init__() method of your scene subclass, you will receive a window reference.
+    You should copy this into an instance variable like this, and use it when drawing:
 
         |    def __init__(self, window):
         |        self.window = window
         |        # Add any initialization you want to do here.
 
-    You also need to write a getSceneKey() method that returns a string
-    or constant that uniquely identifies the scene.  It is recommended that you
-    build and import a Constants.py file that contains constants for each scene,
-    and use the key associated with the current scene here.
-
-        |    def getSceneKey(self):
-        |        return <string or CONSTANT that identifies this scene>
+    Before version 1.1 of pyghelpers you had to do the following, but
+    as of version 1.1, this method is no longer needed.  Instead, you now
+    set the scene keys at start up  (much more betterer!).
+
+                OLD: You also need to write a getSceneKey() method that returns a string
+                or constant that uniquely identifies the scene.  It is recommended that you
+                build and import a Constants.py file that contains constants for each scene,
+                and use the key associated with the current scene here.
+                |    def getSceneKey(self):
+                |        return <string or CONSTANT that identifies this scene>
 
     When your scene is active, the SceneManager calls a standard set of methods in the current scene.
     Therefore, all scenes must implement these methods (polymorphism):
 
-        |    handleInputs  # called in every frame
-        |    draw          # called in every frame
-
+        |    handleInputs()  # called in every frame
+        |    draw()          # called in every frame
 
     The following methods can optionally be implemented in a scene.  If they are not
-    implemented, then the default version in the Scene subclass will be used.
-    (The Scene class' default versions do not do anything, they just return):
+    implemented, then the null version in the Scene subclass will be used.
+    (The Scene class' default versions only execute a pass statement):
 
-        |    enter          # called once whenever the scene is entered
-        |    update         # called in every frame
-        |    leave          # called once whenever the scene is left
+        |    enter()          # called once whenever the scene is entered
+        |    update()       # called in every frame
+        |    leave()          # called once whenever the scene is left
 
-    When you want to go to a new scene:
+    When you want to go to a new scene, call:
 
-        |    Call self.goToScene() and pass in the sceneKey of the scene you want to go to,
+        |    self.goToScene() and pass in the sceneKey of the scene you want to go to,
         |    and optionally, pass any data you want the next scene to receive in its enter() method.
 
     If you want to quit the program from your scene, call:
 
         |    self.quit()
 
     """
@@ -684,33 +871,35 @@
         """Internal method, called when the scene is about to die."""
         self.oSceneMgr = None  # eliminate the reference to the SceneMgr
 
     def _setRefToSceneMgr(self, oSceneMgr):
         """Internal method to save  a reference to the SceneMgr object
 
         This exists so each class built from this base class can call methods in the Scene Manager
-        That reference is used by the goToScene, request, and send methods in each Scene
+        That reference is used by the goToScene(), request(), and send ()methods in each Scene
         Do not change or override this method.
 
         """
         self.oSceneMgr = oSceneMgr
 
     def enter(self, data):
         """This method is called whenever the user enters a scene.
 
         Should be overridden if you expect data when your scene is entered.
         Add any code you need to start or re-start the scene
 
-        Parameters:
+        Parameter:
             |    data - can be of any type agreed to by the old and new scenes
 
         """
         pass
 
-    @abstractmethod
+    # This is no longer needed (as of pyghelpers 1.1)
+    # Left in for backwards compatibility, but no longer needs to be an abstract method
+    #@abstractmethod
     def getSceneKey(self):
         """This method must return the scene key for this scene
         """
         raise NotImplementedError
 
     @abstractmethod
     def handleInputs(self, events, keyPressedList):
@@ -722,22 +911,26 @@
             |    events - a list of events your method should handle.
             |    keyPressedList - a list of keys that are pressed (a Boolean for each key).
 
         """
         raise NotImplementedError
 
     def update(self):
-        """This method is called in every frame of the scene do any processing you need to do here"""
+        """This method is called in every frame of the scene do any processing you need to do here
+
+        Your code will typically override this method.
+
+        """
         pass
 
     @abstractmethod
     def draw(self):
         """This method is called in every frame of the scene to draw anything that needs to be drawn
 
-        Your code must override this method.
+        Your code MUST override this method.
 
         """
         raise NotImplementedError
 
     def leave(self):
         """This method is called whenever the user leaves a scene
 
@@ -752,14 +945,16 @@
 
 
     def goToScene(self, nextSceneKey, data=None):
         """Call this method whenever you want to go to a new scene
 
         Parameters:
             |    nextSceneKey - the scene key (string) of the scene to go to
+
+        Optional keyword parameter:
             |    data - any data you want sent to the next scene (defaults to None)
             |          (The data can be a single value, a list, dictionary, object, etc.)
 
         """
         self.oSceneMgr._goToScene(nextSceneKey, data)
 
 
@@ -784,15 +979,14 @@
         You can pass any info the two scenes agree upon
 
         Parameters:
             |    targetSceneKey - the scene key (string) of the scene to ask for data
             |    sendID - the type of data you are sending the target scene (typically a string)
             |    info - the actual data to send (can be any type)
 
-
         """
         self.oSceneMgr._send_receive(targetSceneKey, sendID, info)
 
     def sendAll(self, sendID, info):
         """Call this method to send information to all other scenes
 
         The other scenes must implement a method named:  receive().
@@ -826,14 +1020,42 @@
         Parameters:
             |    receiveID - an identifier for what type of information is being received
             |    info - the information sent from another scene
 
         """
         raise NotImplementedError
 
+    def addScene(self, sceneKey, oScene):
+        """Call this method whenever you want to add a new scene dynamically.
+        For example, you could have a game with many levels (each implemented as a scene),
+        but only have the current level loaded.  As the player completes a level, you
+        could do a removeScene on the current level and do an addScene on the
+        next level, then do a goToScene on the new level.
+
+        Parameters:
+            |    sceneKey - a key to uniquely identify this scene (typically a string)
+            |    oScene - an instance of the new scene to be added
+            |         (typically, you would instantiate the new scene, and pass in that reference to this call)
+
+        """
+        self.oSceneMgr._addScene(sceneKey, oScene)
+
+    def removeScene(self, sceneKey):
+        """Call this method whenever you want to remove an existing scene
+        You can remove a scene to save memory - the scene object will be deleted.
+        The SceneMgr delays removing the scene until the next time thru the main loop.
+        Therefore, it is safe to call to removeScene from its own scene, if you immediately
+        go to another scene.
+
+        Parameters:
+            |    sceneKey - the scene key (string) of the scene to remove
+
+        """
+        self.oSceneMgr._removeScene(sceneKey)
+
 
 #
 #  Dialog functions
 #
 DIALOG_BACKGROUND_COLOR = (0, 200, 200)
 DIALOG_BLACK = (0, 0, 0)
 
@@ -860,15 +1082,14 @@
     Returns:
         |    True - meaning the Yes button was pressed
         |        or
         |    False - meaning the No button was pressed
         |
         |   (With an alert dialog, you can ignore the returned value, as it will always be True.)
 
-
     """
     dialogLeft = theRect[0]
     dialogTop = theRect[1]
     dialogWidth = theRect[2]
     dialogHeight = theRect[3]
     frameRect = pygame.Rect(dialogLeft + 1, dialogTop + 1, dialogWidth - 2, dialogHeight - 2)
     INSET = 30 # inset buttons from the edges of the dialog box
@@ -927,27 +1148,30 @@
         # 11 - Update the window
         pygame.display.update()
 
         # 12 - Slow things down a bit
         #clock.tick(FRAMES_PER_SECOND)  # no need for this
 
 
-def customYesNoDialog(theWindow, oDialogImage, oPromptText, oYesButton, oNoButton):
+def customYesNoDialog(theWindow, oDialogImage, oPromptText, oYesButton, oNoButton=None):
     """A function that puts up a custom two-button modal dialog (typically Yes/No or OK/Cancel)
 
     It can also be used to put up a single button alert dialog (with a typcial OK button)
 
     Parameters:
         |    theWindow - the window to draw in
         |    oDialogImage - an Image object (from pygwidgets) with the background of the dialog box
         |    oPromptText - a TextDisplay object (from pygwidgets) containing the prompt to display
         |    oYesButton - a CustomButton object (from pygwidgets) representing Yes or OK, etc.
-        |    oNoButton - a CustomButton object (from pygwidgets) representing No or Cancel, etc.
+
+    Optional keyword parameter:
+        |    oNoButton - a CustomButton object (from pygwidgets) representing No or Cancel, etc. (default None)
         |       Note:  If oNoButton is None, the No button will not be drawn
-        |              This way, you can present an "alert" box with only a single button, like 'OK' 
+        |              This way, you can present an "alert" box with only a single button, like 'OK'
+
     Returns:
         |    True - meaning the Yes button was pressed
         |        or
         |    False - meaning the No button was pressed
         |
         |   (With an alert dialog, you can ignore the returned value, as it will always be True.)
```

### Comparing `pyghelpers-1.0.3/pyghelpers.egg-info/SOURCES.txt` & `pyghelpers-1.0.41/pyghelpers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README
 setup.py
 pyghelpers/__init__.py
 pyghelpers/conf.py
 pyghelpers/pyghelpers.py
 pyghelpers.egg-info/PKG-INFO
```

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/Main_DialogTester.py` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/Main_DialogTester.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,63 +18,63 @@
 WINDOW_HEIGHT = 480
 FRAMES_PER_SECOND = 30
 
 
 
 def showCustomAlertDialog(theWindow, theText):
     oDialogBackground = pygwidgets.Image(theWindow, (60, 120), 'images/dialog.png')
-    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText, \
+    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText,
                                 width=WINDOW_WIDTH, justified='center', fontSize=36)
-    oOKButton = pygwidgets.CustomButton(theWindow, (355, 265), \
-                                        'images/okNormal.png',\
-                                        over='images/okOver.png',\
-                                        down='images/okDown.png',\
+    oOKButton = pygwidgets.CustomButton(theWindow, (355, 265),
+                                        'images/okNormal.png',
+                                        over='images/okOver.png',
+                                        down='images/okDown.png',
                                         disabled='images/okDisabled.png')
-    userAnswer = pyghelpers.customYesNoDialog(theWindow, oDialogBackground, \
+    userAnswer = pyghelpers.customYesNoDialog(theWindow, oDialogBackground,
                                     oPromptDisplayText, oOKButton, None)
     return userAnswer
 
 
 def showCustomYesNoDialog(theWindow, theText):
     oDialogBackground = pygwidgets.Image(theWindow, (60, 120), 'images/dialog.png')
-    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText, \
+    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText,
                                 width=WINDOW_WIDTH, justified='center', fontSize=36)
-    oNoButton = pygwidgets.CustomButton(theWindow, (95, 265), \
-                                        'images/noNormal.png',\
-                                        over='images/noOver.png',\
-                                        down='images/noDown.png',\
+    oNoButton = pygwidgets.CustomButton(theWindow, (95, 265),
+                                        'images/noNormal.png',
+                                        over='images/noOver.png',
+                                        down='images/noDown.png',
                                         disabled='images/noDisabled.png')
-    oYesButton = pygwidgets.CustomButton(theWindow, (355, 265), \
-                                        'images/yesNormal.png',\
-                                        over='images/yesOver.png',\
-                                        down='images/yesDown.png',\
+    oYesButton = pygwidgets.CustomButton(theWindow, (355, 265),
+                                        'images/yesNormal.png',
+                                        over='images/yesOver.png',
+                                        down='images/yesDown.png',
                                         disabled='images/yesDisabled.png')
-    userAnswer = pyghelpers.customYesNoDialog(theWindow, oDialogBackground, \
+    userAnswer = pyghelpers.customYesNoDialog(theWindow, oDialogBackground,
                                     oPromptDisplayText, oYesButton, oNoButton)
     return userAnswer
 
 def showCustomAnswerDialog(theWindow, theText):
     oDialogBackground = pygwidgets.Image(theWindow, (60, 120), 'images/dialog.png')
-    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText, \
+    oPromptDisplayText = pygwidgets.DisplayText(theWindow, (0, 170), theText,
                                 width=WINDOW_WIDTH, justified='center', fontSize=36)
     oUserInputText = pygwidgets.InputText(theWindow, (225, 220), '',
                                             fontSize=36, initialFocus=True)
-    oNoButton = pygwidgets.CustomButton(theWindow, (105, 265), \
-                                        'images/cancelNormal.png',\
-                                        over='images/cancelOver.png',\
-                                        down='images/cancelDown.png',\
+    oNoButton = pygwidgets.CustomButton(theWindow, (105, 265),
+                                        'images/cancelNormal.png',
+                                        over='images/cancelOver.png',
+                                        down='images/cancelDown.png',
                                         disabled='images/cancelDisabled.png')
-    oYesButton = pygwidgets.CustomButton(theWindow, (375, 265), \
-                                        'images/okNormal.png',\
-                                        over='images/okOver.png',\
-                                        down='images/okDown.png',\
+    oYesButton = pygwidgets.CustomButton(theWindow, (375, 265),
+                                        'images/okNormal.png',
+                                        over='images/okOver.png',
+                                        down='images/okDown.png',
                                         disabled='images/okDisabled.png')
-    choiceAsBoolean, userAnswer = pyghelpers.customAnswerDialog(theWindow, oDialogBackground, \
+    userAnswer = pyghelpers.customAnswerDialog(theWindow, oDialogBackground,
                                     oPromptDisplayText, oUserInputText, oYesButton, oNoButton)
-    return choiceAsBoolean, userAnswer
+    return userAnswer
 
 
 # 3 - Initialize the world
 pygame.init()
 window = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
 clock = pygame.time.Clock()  # set the speed (frames per second)
 
@@ -86,15 +86,15 @@
 textAlertButton = pygwidgets.TextButton(window, (75, 370), 'Text Alert')
 customAlertButton = pygwidgets.TextButton(window, (75, 420), 'Custom Alert')
 textYesNoButton = pygwidgets.TextButton(window, (280, 370), 'Text Yes/No')
 customYesNoButton = pygwidgets.TextButton(window, (280, 420), 'Custom Yes/No')
 textAnswerButton = pygwidgets.TextButton(window, (485, 370), 'Text Answer')
 customAnswerButton = pygwidgets.TextButton(window, (485, 420), 'Custom Answer')
 
-title = pygwidgets.DisplayText(window, (150, 50), 'Click all buttons to test dialogs', \
+title = pygwidgets.DisplayText(window, (150, 50), 'Click all buttons to test dialogs',
                                     fontSize=36, textColor=WHITE)
 
 
 # 6 - Loop forever
 while True:
 
     # 7 -  Check for and handle events
@@ -104,15 +104,15 @@
             # if it is quit the game
             pygame.quit()
             sys.exit()
 
         if textAlertButton.handleEvent(event):
             # Note, only an OK button, so need to check the value returned from this call (will be True)
             pyghelpers.textYesNoDialog(window, (75, 100, 500, 150),
-                                                  'This is an alert!', 'OK', '')
+                                                  'This is an alert!', 'OK', None)
             print('User clicked the OK button')
 
         if customAlertButton.handleEvent(event):
             # Note, only an OK button, so need to check the value returned from this call (will be True)
             showCustomAlertDialog(window, 'This is an alert!')
             print('User clicked the OK button')
 
@@ -140,22 +140,22 @@
             if returnedValue:
                 print('User clicked OK')
                 print('Users answer was:', userAnswer)
             else:
                 print('User clicked cancel')
 
         if customAnswerButton.handleEvent(event):
-            returnedValue, userAnswer = showCustomAnswerDialog(window, \
+            userAnswer = showCustomAnswerDialog(window,
                                                            'What is your favorite flavor of ice cream?')
-            print('Returned values were:', returnedValue, userAnswer )                                                                                        
-            if returnedValue:
-                print('User clicked OK')
-                print('Users answer was:', userAnswer)
-            else:
+            if userAnswer is None:
                 print('User clicked Cancel')
+            else:
+                print('Users answer was:', userAnswer)
+
+
 
 
     # 8 - Do any "per frame" actions
 
     # 9 - Clear the screen before drawing it again
     window.fill(BACKGROUND_COLOR)
```

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/addOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/addOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/cancelOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/cancelOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/controlsBackground.jpg` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/controlsBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/dialog.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/dialog.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/highScoresBackground.jpg` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/highScoresBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/noThanksOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/noThanksOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/okOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/okOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesDown.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/DialogTester/images/yesOver.png` & `pyghelpers-1.0.41/pyghelpers_test/DialogTester/images/yesOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/Baddies.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/Baddies.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/Goodies.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/Goodies.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/HighScoresData.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/HighScoresData.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/Main_Dodger.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/Main_Dodger.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # 3 - Initialize the world
 pygame.init()
 window = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
 
 # 4 - Load assets: image(s), sounds,  etc.
 
 # 5 - Initialize variables
-# Instantiate all scenes and store them in a list
-scenesList = [SceneSplash(window),
-                    SceneHighScores(window),
-                    ScenePlay(window)]
+# Instantiate all scenes and store them in a dict (new approach for pyghelpers 1.1)
+scenesList = {SCENE_SPLASH: SceneSplash(window),
+                    SCENE_HIGH_SCORES: SceneHighScores(window),
+                    SCENE_PLAY: ScenePlay(window)}
 
 # Create the scene manager, passing in the scenes list and the FPS
 oSceneMgr = pyghelpers.SceneMgr(scenesList, FRAMES_PER_SECOND)
 
 # Tell the Scene Manager to start running
 oSceneMgr.run()
```

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/Player.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/Player.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Player
-import pygame
+
 import pygwidgets
 from Constants import *
 
 class Player():
     def __init__(self, window):
         self.window = window
         self.image = pygwidgets.Image(window,
```

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneExample.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneExample.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneHighScores.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneHighScores.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/ScenePlay.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/ScenePlay.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/SceneSplash.py` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/SceneSplash.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/addOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/addOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/backOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/backOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/baddie.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/baddie.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/cancelOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/cancelOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/controlsBackground.jpg` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/controlsBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/dialog.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/dialog.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/dodger.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/dodger.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gameOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gameOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/goodie.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/goodie.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/gotoHighScoresOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/gotoHighScoresOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresBackground.jpg` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/highScoresOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/highScoresOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/noThanksOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/noThanksOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/okOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/okOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/player.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/player.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/quitOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/quitOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/resetOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/resetOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/splashBackground.jpg` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/splashBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewDisabled.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewDown.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNewOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNewOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startNormal.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/images/startOver.png` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/images/startOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/background.mid` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/background.mid`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/ding.wav` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/ding.wav`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/pyghelpers_test/Dodger/sounds/gameover.wav` & `pyghelpers-1.0.41/pyghelpers_test/Dodger/sounds/gameover.wav`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.3/setup.py` & `pyghelpers-1.0.41/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pyghelpers',
-    version='1.0.3',
+    version='1.0.41',
     author='Irv Kalb',
     author_email='Irv@furrypants.com',
     description='Classes and functions for use with Pygame',
     long_description='A collection of classes and functions for building programs using Pygame',
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
     url='https://github.com/IrvKalb/pyghelpers',
     install_requires=[
-        'pygame>=2.0',
+        'pygame-ce>=2.0',
         'pygwidgets>=1.0',        
         ],
-    keywords="Timer classes, Scene and SceneMgr classes, Dialogs, file IO functions",
+    keywords="Timer classes, Scene and SceneMgr classes, Dialogs",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent"
       ]
     )
```

