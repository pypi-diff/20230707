# Comparing `tmp/avsub-0.0.3.tar.gz` & `tmp/avsub-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsub-0.0.3.tar", last modified: Tue Apr 18 02:01:22 2023, max compression
+gzip compressed data, was "avsub-0.0.4.tar", last modified: Fri Jul  7 20:12:19 2023, max compression
```

## Comparing `avsub-0.0.3.tar` & `avsub-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:01:22.476285 avsub-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-04-09 03:51:55.000000 avsub-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      797 2023-04-18 02:01:22.476285 avsub-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2023-04-18 01:35:53.000000 avsub-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:01:22.461379 avsub-0.0.3/avsub/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:52:44.000000 avsub-0.0.3/avsub/__init__.py
--rw-rw-rw-   0        0        0     3850 2023-04-18 01:06:44.000000 avsub-0.0.3/avsub/__main__.py
--rw-rw-rw-   0        0        0       81 2023-04-18 01:52:44.000000 avsub-0.0.3/avsub/__version__.py
--rw-rw-rw-   0        0        0      433 2023-04-13 17:23:33.000000 avsub-0.0.3/avsub/actions.py
--rw-rw-rw-   0        0        0     5722 2023-04-13 17:19:23.000000 avsub-0.0.3/avsub/cli.py
--rw-rw-rw-   0        0        0      609 2023-04-13 01:02:10.000000 avsub-0.0.3/avsub/consts.py
--rw-rw-rw-   0        0        0     3559 2023-04-13 17:48:03.000000 avsub-0.0.3/avsub/ffmpeg.py
--rw-rw-rw-   0        0        0      211 2023-04-11 12:57:13.000000 avsub-0.0.3/avsub/globs.py
--rw-rw-rw-   0        0        0     1680 2023-04-13 00:17:21.000000 avsub-0.0.3/avsub/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:01:22.466120 avsub-0.0.3/avsub.egg-info/
--rw-rw-rw-   0        0        0      797 2023-04-18 02:01:22.000000 avsub-0.0.3/avsub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-04-18 02:01:22.000000 avsub-0.0.3/avsub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:01:22.000000 avsub-0.0.3/avsub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-18 02:01:22.000000 avsub-0.0.3/avsub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 02:01:21.000000 avsub-0.0.3/avsub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-18 02:01:22.000000 avsub-0.0.3/avsub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1049 2023-04-18 01:51:41.000000 avsub-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 02:01:22.477294 avsub-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.464959 avsub-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 01:59:47.000000 avsub-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      797 2023-07-07 20:12:19.464959 avsub-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-18 01:59:47.000000 avsub-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.422742 avsub-0.0.4/avsub/
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/__init__.py
+-rw-rw-rw-   0        0        0     3850 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/__main__.py
+-rw-rw-rw-   0        0        0       81 2023-07-06 21:02:32.000000 avsub-0.0.4/avsub/__version__.py
+-rw-rw-rw-   0        0        0      433 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/actions.py
+-rw-rw-rw-   0        0        0     6106 2023-07-07 19:47:45.000000 avsub-0.0.4/avsub/cli.py
+-rw-rw-rw-   0        0        0      735 2023-07-07 19:34:42.000000 avsub-0.0.4/avsub/consts.py
+-rw-rw-rw-   0        0        0     4112 2023-07-07 20:07:19.000000 avsub-0.0.4/avsub/ffmpeg.py
+-rw-rw-rw-   0        0        0      211 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/globs.py
+-rw-rw-rw-   0        0        0     1680 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.464959 avsub-0.0.4/avsub.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 20:12:18.000000 avsub-0.0.4/avsub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1049 2023-04-18 01:59:47.000000 avsub-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 20:12:19.464959 avsub-0.0.4/setup.cfg
```

### Comparing `avsub-0.0.3/LICENSE` & `avsub-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avsub-0.0.3/PKG-INFO` & `avsub-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.3/avsub/__main__.py` & `avsub-0.0.4/avsub/__main__.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.3/avsub/cli.py` & `avsub-0.0.4/avsub/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 
 from avsub.__version__ import __version__
 from avsub.actions import ExitAction
 from avsub.consts import (
     CHOICES_CHANNEL,
+    CHOICES_SPEED,
     CHOICES_SUB_ALIGNMENT,
     CHOICES_SUB_BGR_CHART,
     X,
 )
 from avsub.utils import check_for_updates
 
 parser = argparse.ArgumentParser(
@@ -93,14 +94,21 @@
 )
 parser.add_argument(
     '--ffmpeg-list', '-f',
     help='provide %(metavar)s as ffmpeg argument list',
     metavar='ARGS',
     dest='ffmpeg_list',
 )
+parser.add_argument(
+    '--frame', '-p',
+    type=float,
+    help='set %(metavar)s as frame rate',
+    metavar='VALUE',
+    dest='frame',
+)
 mutual.add_argument(
     '--only-audio', '-A',
     action='store_const',
     const=['-dn', '-sn', '-vn'],
     default=[],
     help='choose audio stream only',
     dest='only_a',
@@ -139,14 +147,22 @@
 parser.add_argument(
     '--remove-metadata',
     action='store_true',
     help='remove metadata',
     dest='metadata',
 )
 parser.add_argument(
+    '--speed',
+    nargs=2,
+    choices=CHOICES_SPEED,
+    help='speed up or slow down audio and video stream (choices: %(choices)s)',
+    metavar=('AUDIO', 'VIDEO'),
+    dest='speed',
+)
+parser.add_argument(
     '--trim',
     nargs=6,
     type=int,
     choices=range(0, 60),
     help='extract a part of a video',
     metavar=('H:', 'M:', 'S:', ':H', ':M', ':S'),
     dest='trim',
```

### Comparing `avsub-0.0.3/avsub/ffmpeg.py` & `avsub-0.0.4/avsub/ffmpeg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """FFmpeg module."""
 
 from __future__ import annotations
 
+import math
 import os
 import subprocess as sp  # nosec
+from fractions import Fraction
 from itertools import chain, count
 from typing import TYPE_CHECKING
 
 from avsub.consts import (
     CHOICES_CHANNEL,
+    CHOICES_SPEED,
     CHOICES_SUB_ALIGNMENT,
     CHOICES_SUB_BGR_CHART,
     LOGLEVEL,
     X,
 )
 from avsub.globs import completed, controller, corrupted, untouched
 
@@ -43,21 +46,33 @@
         cmd += ['-crf', str(opts.compress)]
 
         cmd += chain(*(['-codec:' + _[0].strip(X), 'copy'] for _ in opts.copy))
 
         if not opts.disable:
             cmd += ['-map', '0']
 
+        if opts.frame is not None:
+            cmd += ['-r', str(opts.frame)]
+
         cmd += opts.only_a + opts.only_s + opts.only_v
 
         cmd += [f'-{_[0]}n' for _ in opts.remove]
 
         cmd += ['-map_chapters', str(-int(opts.chapters))]
         cmd += ['-map_metadata', str(-int(opts.metadata))]
 
+        if opts.speed is not None:
+            speed_a, speed_v = opts.speed
+            by_a, by_v = float(Fraction(speed_a)), float(Fraction(speed_v))
+            k = CHOICES_SPEED[speed_a]
+            n = int(math.log(by_a, k))
+            extra = by_a / (k ** n)
+            cmd += ['-af', ','.join([f'atempo={k}'] * n + [f'atempo={extra}'])]
+            cmd += ['-vf', f'setpts=PTS/{by_v}']
+
         if opts.trim is not None:
             seek = (opts.trim[0] * 3600) + (opts.trim[1] * 60) + opts.trim[2]
             stop = (opts.trim[3] * 3600) + (opts.trim[4] * 60) + opts.trim[5]
             cmd += ['-ss', str(seek), '-to', str(stop)]
 
         cmd += ['-loglevel', LOGLEVEL[opts.loglevel]]
```

### Comparing `avsub-0.0.3/avsub/utils.py` & `avsub-0.0.4/avsub/utils.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.3/avsub.egg-info/PKG-INFO` & `avsub-0.0.4/avsub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.3/pyproject.toml` & `avsub-0.0.4/pyproject.toml`

 * *Files identical despite different names*

