# Comparing `tmp/ectool-1.1.2.tar.gz` & `tmp/ectool-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.2.tar", last modified: Fri Jul  7 12:46:39 2023, max compression
+gzip compressed data, was "ectool-1.1.3.tar", last modified: Fri Jul  7 13:09:54 2023, max compression
```

## Comparing `ectool-1.1.2.tar` & `ectool-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.693385 ectool-1.1.2/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2023 2023-07-07 12:46:39.694386 ectool-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-07-07 12:05:42.000000 ectool-1.1.2/README.md
--rw-rw-rw-   0        0        0      113 2023-07-07 12:46:39.694386 ectool-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     7947 2023-07-07 12:36:57.000000 ectool-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.672386 ectool-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.685387 ectool-1.1.2/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.2/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15985 2023-07-07 10:38:19.000000 ectool-1.1.2/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.2/src/ectool/ecag.py
--rw-rw-rw-   0        0        0     5048 2023-07-07 12:41:03.000000 ectool-1.1.2/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.2/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.2/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3896 2023-07-07 12:43:56.000000 ectool-1.1.2/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.692387 ectool-1.1.2/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.592749 ectool-1.1.3/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2023 2023-07-07 13:09:54.592749 ectool-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-07-07 12:05:42.000000 ectool-1.1.3/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-07 13:09:54.593750 ectool-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-07 13:08:09.000000 ectool-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.574748 ectool-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.585750 ectool-1.1.3/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.3/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15985 2023-07-07 10:38:19.000000 ectool-1.1.3/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.3/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     5142 2023-07-07 13:07:09.000000 ectool-1.1.3/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.3/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.3/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3896 2023-07-07 12:43:56.000000 ectool-1.1.3/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.591749 ectool-1.1.3/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.2/LICENSE` & `ectool-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/PKG-INFO` & `ectool-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ectool-1.1.2/README.md` & `ectool-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/setup.py` & `ectool-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.1.2",  # Required
+    version="1.1.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.1.2/src/ectool/ecaction.py` & `ectool-1.1.3/src/ectool/ecaction.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/src/ectool/ecag.py` & `ectool-1.1.3/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/src/ectool/eccli.py` & `ectool-1.1.3/src/ectool/eccli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 def ecburn_auto_select() :
     for item in serial.tools.list_ports.comports():
         if not item.pid or not item.location :
             continue
         if item.vid == 0x17D1 and item.pid == 0x0001 :
             return item.device
+            # return item.name
     return None
 
 def cli_burn() :
     if not ecargs.file :
         logger.error("require -f/--file !!!")
         sys.exit(3)
     import ectool.unpkg as unpkg
@@ -46,16 +47,17 @@
             logger.error("timeout for searching, exit")
             sys.exit(2)
             return
     logger.info("Select " + ecargs.port)
     COM = ecargs.port
 
     # burncom = serial.Serial(COM, baudrate=921600, exclusive=None, timeout=1, xonxoff=False, rtscts=False, dsrdtr=False)
-    burncom = serial.Serial(COM, baudrate=921600)
+    burncom = serial.Serial(COM, baudrate=921600, timeout=1)
     burncom.dtr = 1
+    burncom.timeout = 1
 
     logging.info("Go   Sync")
     if 0 != burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_DLBOOT, 2) :
         return -1
     logging.info("Done Sync")
     
     logging.info("Go   AgentBoot download")
@@ -95,14 +97,15 @@
     if not ecargs.file :
         logger.error("require -f/--file !!!")
         sys.exit(3)
     import ectool.unpkg as unpkg
     unpkg.binpkg_unpack(ecargs.file, ecargs.outdir)
 
 def main() :
+    # print("1.2.3.4.5")
     global ecargs
     global logger
     import argparse
     parser = argparse.ArgumentParser(description='A tool for EC modules, like EC618')
     parser.add_argument("action", choices=["burn", "unpack"], help="main action to perform")
     parser.add_argument("--file", "-f", help="file path")
     parser.add_argument("--burn_addr",  help="burn bin file to addr")
```

### Comparing `ectool-1.1.2/src/ectool/ecconst.py` & `ectool-1.1.3/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/src/ectool/ecstruct.py` & `ectool-1.1.3/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/src/ectool/unpkg.py` & `ectool-1.1.3/src/ectool/unpkg.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.2/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.3/src/ectool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
```

