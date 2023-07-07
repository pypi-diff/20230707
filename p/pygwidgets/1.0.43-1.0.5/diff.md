# Comparing `tmp/pygwidgets-1.0.43.tar.gz` & `tmp/pygwidgets-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwidgets-1.0.43.tar", last modified: Fri Jul  7 16:19:56 2023, max compression
+gzip compressed data, was "pygwidgets-1.0.5.tar", last modified: Thu Jul  6 17:51:39 2023, max compression
```

## Comparing `pygwidgets-1.0.43.tar` & `pygwidgets-1.0.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.886883 pygwidgets-1.0.43/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pygwidgets-1.0.43/LICENSE
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.0.43/MANIFEST.in
--rw-r--r--   0 irvkalb    (501) staff       (20)      523 2023-07-07 16:19:56.886634 pygwidgets-1.0.43/PKG-INFO
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1708 2023-07-01 03:54:42.000000 pygwidgets-1.0.43/README
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.866512 pygwidgets-1.0.43/pygwidgets/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.0.43/pygwidgets/__init__.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     5193 2023-07-07 16:09:22.000000 pygwidgets-1.0.43/pygwidgets/conf.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)   153310 2023-06-29 18:40:42.000000 pygwidgets-1.0.43/pygwidgets/pygwidgets.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.868133 pygwidgets-1.0.43/pygwidgets.egg-info/
--rw-r--r--   0 irvkalb    (501) staff       (20)      523 2023-07-07 16:19:56.000000 pygwidgets-1.0.43/pygwidgets.egg-info/PKG-INFO
--rw-r--r--   0 irvkalb    (501) staff       (20)     2582 2023-07-07 16:19:56.000000 pygwidgets-1.0.43/pygwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-07 16:19:56.000000 pygwidgets-1.0.43/pygwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       15 2023-07-07 16:19:56.000000 pygwidgets-1.0.43/pygwidgets.egg-info/requires.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-07 16:19:56.000000 pygwidgets-1.0.43/pygwidgets.egg-info/top_level.txt
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.868701 pygwidgets-1.0.43/pygwidgets_test/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    13561 2023-05-29 17:59:51.000000 pygwidgets-1.0.43/pygwidgets_test/Main_Test_pygwidgets.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.0.43/pygwidgets_test/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.881756 pygwidgets-1.0.43/pygwidgets_test/images/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.0.43/pygwidgets_test/images/background.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/dragMeDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/dragMeDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/dragMeOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/dragMeUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/extenDisabled.png
--rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.0.43/pygwidgets_test/images/frisbee.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.0.43/pygwidgets_test/images/imageDown.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/imageLeft.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.0.43/pygwidgets_test/images/imageRight.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.0.43/pygwidgets_test/images/imageStart.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.0.43/pygwidgets_test/images/imageUp.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.0.43/pygwidgets_test/images/pythonIcon.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioHighOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioLowOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/radioMedOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/restartButtonDisabled.png
--rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.0.43/pygwidgets_test/images/restartButtonDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/restartButtonOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/restartButtonUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/sliderExtent.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/sliderExtentDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/sliderThumb.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/sliderThumbDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/images/testImage.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-07 16:19:56.886268 pygwidgets-1.0.43/pygwidgets_test/sounds/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Anybutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Coin.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Item.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Jump.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Nextbutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/Warp.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/blip.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/boing.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/bonus.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.0.43/pygwidgets_test/sounds/dink.wav
--rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-07 16:19:56.886962 pygwidgets-1.0.43/setup.cfg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      749 2023-07-07 16:18:41.000000 pygwidgets-1.0.43/setup.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.041408 pygwidgets-1.0.5/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pygwidgets-1.0.5/LICENSE
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.0.5/MANIFEST.in
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-06 17:51:39.040990 pygwidgets-1.0.5/PKG-INFO
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1708 2023-07-01 03:54:42.000000 pygwidgets-1.0.5/README
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.010220 pygwidgets-1.0.5/pygwidgets/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.0.5/pygwidgets/__init__.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     5192 2023-07-06 17:47:29.000000 pygwidgets-1.0.5/pygwidgets/conf.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)   153310 2023-06-29 18:40:42.000000 pygwidgets-1.0.5/pygwidgets/pygwidgets.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.012156 pygwidgets-1.0.5/pygwidgets.egg-info/
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-06 17:51:38.000000 pygwidgets-1.0.5/pygwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 irvkalb    (501) staff       (20)     2582 2023-07-06 17:51:38.000000 pygwidgets-1.0.5/pygwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-06 17:51:38.000000 pygwidgets-1.0.5/pygwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       15 2023-07-06 17:51:38.000000 pygwidgets-1.0.5/pygwidgets.egg-info/requires.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-06 17:51:38.000000 pygwidgets-1.0.5/pygwidgets.egg-info/top_level.txt
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.012889 pygwidgets-1.0.5/pygwidgets_test/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    13561 2023-05-29 17:59:51.000000 pygwidgets-1.0.5/pygwidgets_test/Main_Test_pygwidgets.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.0.5/pygwidgets_test/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.032692 pygwidgets-1.0.5/pygwidgets_test/images/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.0.5/pygwidgets_test/images/background.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/dragMeDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/dragMeDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/dragMeOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/dragMeUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/extenDisabled.png
+-rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.0.5/pygwidgets_test/images/frisbee.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.0.5/pygwidgets_test/images/imageDown.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/imageLeft.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.0.5/pygwidgets_test/images/imageRight.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.0.5/pygwidgets_test/images/imageStart.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.0.5/pygwidgets_test/images/imageUp.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.0.5/pygwidgets_test/images/pythonIcon.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioHighOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioLowOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/radioMedOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/restartButtonDisabled.png
+-rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.0.5/pygwidgets_test/images/restartButtonDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/restartButtonOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/restartButtonUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/sliderExtent.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/sliderExtentDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/sliderThumb.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/sliderThumbDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/images/testImage.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-06 17:51:39.040334 pygwidgets-1.0.5/pygwidgets_test/sounds/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Anybutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Coin.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Item.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Jump.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Nextbutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/Warp.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/blip.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/boing.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/bonus.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.0.5/pygwidgets_test/sounds/dink.wav
+-rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-06 17:51:39.041526 pygwidgets-1.0.5/setup.cfg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      748 2023-07-06 17:50:41.000000 pygwidgets-1.0.5/setup.py
```

### Comparing `pygwidgets-1.0.43/LICENSE` & `pygwidgets-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/PKG-INFO` & `pygwidgets-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.0.43
+Version: 1.0.5
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
 Keywords: pygame widgets user interface buttons text dragger animation image
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygwidgets-1.0.43/README` & `pygwidgets-1.0.5/README`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets/conf.py` & `pygwidgets-1.0.5/pygwidgets/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 project = 'pygwidgets'
 copyright = '2021, Irv Kalb'
 author = 'Irv Kalb'
 
 # The short X.Y version
 version = '1.0'
 # The full version, including alpha/beta/rc tags
-release = '1.0.43'
+release = '1.0.5'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '7.0.1'
```

### Comparing `pygwidgets-1.0.43/pygwidgets/pygwidgets.py` & `pygwidgets-1.0.5/pygwidgets/pygwidgets.py`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets.egg-info/PKG-INFO` & `pygwidgets-1.0.5/pygwidgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.0.43
+Version: 1.0.5
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
 Keywords: pygame widgets user interface buttons text dragger animation image
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygwidgets-1.0.43/pygwidgets.egg-info/SOURCES.txt` & `pygwidgets-1.0.5/pygwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/Main_Test_pygwidgets.py` & `pygwidgets-1.0.5/pygwidgets_test/Main_Test_pygwidgets.py`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/background.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/background.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOff.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOff.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOffDisabled.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOffDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOffDown.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOffDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOn.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOn.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOnDisabled.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOnDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/checkBoxOnDown.png` & `pygwidgets-1.0.5/pygwidgets_test/images/checkBoxOnDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/dragMeDisabled.png` & `pygwidgets-1.0.5/pygwidgets_test/images/dragMeDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/dragMeDown.png` & `pygwidgets-1.0.5/pygwidgets_test/images/dragMeDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/dragMeOver.png` & `pygwidgets-1.0.5/pygwidgets_test/images/dragMeOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/dragMeUp.png` & `pygwidgets-1.0.5/pygwidgets_test/images/dragMeUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/frisbee.png` & `pygwidgets-1.0.5/pygwidgets_test/images/frisbee.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/imageDown.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/imageDown.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/imageLeft.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/imageLeft.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/imageRight.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/imageRight.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/imageStart.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/imageStart.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/imageUp.jpg` & `pygwidgets-1.0.5/pygwidgets_test/images/imageUp.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/pythonIcon.png` & `pygwidgets-1.0.5/pygwidgets_test/images/pythonIcon.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/restartButtonDisabled.png` & `pygwidgets-1.0.5/pygwidgets_test/images/restartButtonDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/restartButtonDown.png` & `pygwidgets-1.0.5/pygwidgets_test/images/restartButtonDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/restartButtonOver.png` & `pygwidgets-1.0.5/pygwidgets_test/images/restartButtonOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/images/restartButtonUp.png` & `pygwidgets-1.0.5/pygwidgets_test/images/restartButtonUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Anybutton.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Anybutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Coin.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Coin.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Item.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Item.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Jump.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Jump.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Nextbutton.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Nextbutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/Warp.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/Warp.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/blip.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/blip.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/boing.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/boing.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/bonus.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/bonus.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/pygwidgets_test/sounds/dink.wav` & `pygwidgets-1.0.5/pygwidgets_test/sounds/dink.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.43/setup.py` & `pygwidgets-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pygwidgets',
-    version='1.0.43',
+    version='1.0.5',
     author='Irv Kalb',
     author_email='Irv@furrypants.com',
     description='User interface widgets for use with Pygame',
     long_description='User interface widgets for building programs using Pygame',
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
```

