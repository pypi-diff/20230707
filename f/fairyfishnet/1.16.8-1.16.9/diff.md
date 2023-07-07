# Comparing `tmp/fairyfishnet-1.16.8.tar.gz` & `tmp/fairyfishnet-1.16.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairyfishnet-1.16.8.tar", last modified: Thu Apr  7 07:36:27 2022, max compression
+gzip compressed data, was "fairyfishnet-1.16.9.tar", last modified: Tue Apr 12 08:15:28 2022, max compression
```

## Comparing `fairyfishnet-1.16.8.tar` & `fairyfishnet-1.16.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tamas     (1001) tamas     (1001)        0 2022-04-07 07:36:27.061330 fairyfishnet-1.16.8/
--rw-rw-r--   0 tamas     (1001) tamas     (1001)    35147 2019-09-30 21:21:18.000000 fairyfishnet-1.16.8/LICENSE.txt
--rw-rw-r--   0 tamas     (1001) tamas     (1001)       39 2019-09-30 21:21:18.000000 fairyfishnet-1.16.8/MANIFEST.in
--rw-rw-r--   0 tamas     (1001) tamas     (1001)     2836 2022-04-07 07:36:27.061330 fairyfishnet-1.16.8/PKG-INFO
--rw-rw-r--   0 tamas     (1001) tamas     (1001)     1733 2021-09-12 10:05:39.000000 fairyfishnet-1.16.8/README.rst
-drwxrwxr-x   0 tamas     (1001) tamas     (1001)        0 2022-04-07 07:36:27.061330 fairyfishnet-1.16.8/fairyfishnet.egg-info/
--rw-rw-r--   0 tamas     (1001) tamas     (1001)     2836 2022-04-07 07:36:26.000000 fairyfishnet-1.16.8/fairyfishnet.egg-info/PKG-INFO
--rw-rw-r--   0 tamas     (1001) tamas     (1001)      248 2022-04-07 07:36:26.000000 fairyfishnet-1.16.8/fairyfishnet.egg-info/SOURCES.txt
--rw-rw-r--   0 tamas     (1001) tamas     (1001)        1 2022-04-07 07:36:26.000000 fairyfishnet-1.16.8/fairyfishnet.egg-info/dependency_links.txt
--rw-rw-r--   0 tamas     (1001) tamas     (1001)       31 2022-04-07 07:36:26.000000 fairyfishnet-1.16.8/fairyfishnet.egg-info/requires.txt
--rw-rw-r--   0 tamas     (1001) tamas     (1001)       13 2022-04-07 07:36:26.000000 fairyfishnet-1.16.8/fairyfishnet.egg-info/top_level.txt
--rwxrwxr-x   0 tamas     (1001) tamas     (1001)    72570 2022-04-07 07:35:35.000000 fairyfishnet-1.16.8/fairyfishnet.py
--rw-rw-r--   0 tamas     (1001) tamas     (1001)      150 2022-04-07 07:36:27.061330 fairyfishnet-1.16.8/setup.cfg
--rwxrwxr-x   0 tamas     (1001) tamas     (1001)     2380 2022-02-14 10:43:02.000000 fairyfishnet-1.16.8/setup.py
+drwxrwxr-x   0 tamas     (1001) tamas     (1001)        0 2022-04-12 08:15:28.526961 fairyfishnet-1.16.9/
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)    35147 2019-09-30 21:21:18.000000 fairyfishnet-1.16.9/LICENSE.txt
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)       39 2019-09-30 21:21:18.000000 fairyfishnet-1.16.9/MANIFEST.in
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)     2836 2022-04-12 08:15:28.526961 fairyfishnet-1.16.9/PKG-INFO
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)     1733 2021-09-12 10:05:39.000000 fairyfishnet-1.16.9/README.rst
+drwxrwxr-x   0 tamas     (1001) tamas     (1001)        0 2022-04-12 08:15:28.526961 fairyfishnet-1.16.9/fairyfishnet.egg-info/
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)     2836 2022-04-12 08:15:27.000000 fairyfishnet-1.16.9/fairyfishnet.egg-info/PKG-INFO
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)      248 2022-04-12 08:15:28.000000 fairyfishnet-1.16.9/fairyfishnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)        1 2022-04-12 08:15:27.000000 fairyfishnet-1.16.9/fairyfishnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)       31 2022-04-12 08:15:27.000000 fairyfishnet-1.16.9/fairyfishnet.egg-info/requires.txt
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)       13 2022-04-12 08:15:27.000000 fairyfishnet-1.16.9/fairyfishnet.egg-info/top_level.txt
+-rwxrwxr-x   0 tamas     (1001) tamas     (1001)    72606 2022-04-12 08:12:06.000000 fairyfishnet-1.16.9/fairyfishnet.py
+-rw-rw-r--   0 tamas     (1001) tamas     (1001)      150 2022-04-12 08:15:28.526961 fairyfishnet-1.16.9/setup.cfg
+-rwxrwxr-x   0 tamas     (1001) tamas     (1001)     2380 2022-02-14 10:43:02.000000 fairyfishnet-1.16.9/setup.py
```

### Comparing `fairyfishnet-1.16.8/LICENSE.txt` & `fairyfishnet-1.16.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fairyfishnet-1.16.8/PKG-INFO` & `fairyfishnet-1.16.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairyfishnet
-Version: 1.16.8
+Version: 1.16.9
 Summary: Distributed Fairy-Stockfish analysis for pychess-variants
 Home-page: https://github.com/gbtami/fairyfishnet
 Author: Bajusz Tamás
 Author-email: gbtami@gmail.com
 License: UNKNOWN
 Keywords: lichess.org chess stockfish uci
 Platform: UNKNOWN
```

### Comparing `fairyfishnet-1.16.8/README.rst` & `fairyfishnet-1.16.9/README.rst`

 * *Files identical despite different names*

### Comparing `fairyfishnet-1.16.8/fairyfishnet.egg-info/PKG-INFO` & `fairyfishnet-1.16.9/fairyfishnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairyfishnet
-Version: 1.16.8
+Version: 1.16.9
 Summary: Distributed Fairy-Stockfish analysis for pychess-variants
 Home-page: https://github.com/gbtami/fairyfishnet
 Author: Bajusz Tamás
 Author-email: gbtami@gmail.com
 License: UNKNOWN
 Keywords: lichess.org chess stockfish uci
 Platform: UNKNOWN
```

### Comparing `fairyfishnet-1.16.8/fairyfishnet.py` & `fairyfishnet-1.16.9/fairyfishnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # Python 3
     DEAD_ENGINE_ERRORS = (EOFError, IOError, BrokenPipeError)
 except NameError:
     # Python 2
     DEAD_ENGINE_ERRORS = (EOFError, IOError)
 
 
-__version__ = "1.16.8"
+__version__ = "1.16.9"
 
 __author__ = "Bajusz Tamás"
 __email__ = "gbtami@gmail.com"
 __license__ = "GPLv3+"
 
 DEFAULT_ENDPOINT = "https://pychess-variants.herokuapp.com/fishnet/"
 STOCKFISH_RELEASES = "https://api.github.com/repos/gbtami/Fairy-Stockfish/releases/latest"
@@ -138,17 +138,18 @@
 LVL_DEPTHS = [1, 1, 1, 2, 3, 5, 8, 13, 22]
 
 NNUE_NET = {
     "asean": "88c4f9118f34",
     "atomic": "4ecb2067c716",
     "capablanca": "e605d6d3dd31",
     "chak": "0dfa519b8ee7",
-    "crazyhouse": "f0782c10a2d4",
+    "crazyhouse": "ca0dab479c68",
     "empire": "d14c0d04359e",
     "grand": "596776a80f03",
+    "hoppelpoppel": "ca81db235bbe",
     "janggi": "ffbf1d95cea2",
     "makpong": "75299b96ab1d",
     "makruk": "e14ecd7ae145",
     "minishogi": "32efe2ac350b",
     "nn": "46832cfbead3",
     "orda": "af8fab8f210b",
     "ordamirror": "b432a42e3738",
```

### Comparing `fairyfishnet-1.16.8/setup.py` & `fairyfishnet-1.16.9/setup.py`

 * *Files identical despite different names*

