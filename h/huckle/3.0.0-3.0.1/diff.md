# Comparing `tmp/huckle-3.0.0.tar.gz` & `tmp/huckle-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-3.0.0.tar", last modified: Sun Apr  9 23:11:31 2023, max compression
+gzip compressed data, was "huckle-3.0.1.tar", last modified: Fri Jul  7 03:05:10 2023, max compression
```

## Comparing `huckle-3.0.0.tar` & `huckle-3.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079616 huckle-3.0.0/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.0.0/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.0.0/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-04-09 23:11:31.079683 huckle-3.0.0/PKG-INFO
--rwx------   0 jeff       (501) staff       (20)     7575 2023-04-09 22:47:09.000000 huckle-3.0.0/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.078526 huckle-3.0.0/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     4501 2023-04-09 22:30:29.000000 huckle-3.0.0/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079514 huckle-3.0.0/huckle/data/
--rwxr-x---   0 jeff       (501) staff       (20)     2352 2023-04-09 22:53:51.000000 huckle-3.0.0/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    10129 2022-10-29 17:56:09.000000 huckle-3.0.0/huckle/hclinav.py
--rwxr-x---   0 jeff       (501) staff       (20)     2842 2023-04-09 22:16:07.000000 huckle-3.0.0/huckle/huckle.py
--rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-3.0.0/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2023-04-09 19:06:38.000000 huckle-3.0.0/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-04-09 23:11:31.079401 huckle-3.0.0/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      381 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2023-04-09 23:11:31.000000 huckle-3.0.0/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2023-04-09 23:11:31.079889 huckle-3.0.0/setup.cfg
--rwxr-x---   0 jeff       (501) staff       (20)     3314 2023-04-09 22:54:19.000000 huckle-3.0.0/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320445 huckle-3.0.1/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.0.1/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.0.1/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-07-07 03:05:10.320558 huckle-3.0.1/PKG-INFO
+-rwx------   0 jeff       (501) staff       (20)     7575 2023-04-09 22:47:09.000000 huckle-3.0.1/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.319349 huckle-3.0.1/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)      308 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4505 2023-07-07 02:58:30.000000 huckle-3.0.1/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320226 huckle-3.0.1/huckle/data/
+-rwxr-x---   0 jeff       (501) staff       (20)     2352 2023-04-09 22:53:51.000000 huckle-3.0.1/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    10129 2023-07-07 02:34:29.000000 huckle-3.0.1/huckle/hclinav.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2842 2023-07-07 02:33:09.000000 huckle-3.0.1/huckle/huckle.py
+-rwxr-x---   0 jeff       (501) staff       (20)      858 2022-03-20 22:23:06.000000 huckle-3.0.1/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2023-07-07 02:55:08.000000 huckle-3.0.1/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-07 03:05:10.320123 huckle-3.0.1/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     8422 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      381 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2023-07-07 03:05:10.000000 huckle-3.0.1/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2023-07-07 03:05:10.320833 huckle-3.0.1/setup.cfg
+-rwxr-x---   0 jeff       (501) staff       (20)     3314 2023-07-07 02:52:48.000000 huckle-3.0.1/setup.py
```

### Comparing `huckle-3.0.0/LICENSE.txt` & `huckle-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/PKG-INFO` & `huckle-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.0.0/README.rst` & `huckle-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/huckle/config.py` & `huckle-3.0.1/huckle/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 # sets up an alias for a cli so that it can be called directly by name (instead of calling it via the explicit huckle call) 
 def alias_cli(cli):
     if not os.path.exists(dot_huckle_scripts + "/" + cli):
         g = open(dot_huckle_scripts + "/" + cli, "a+")
         os.chmod(dot_huckle_scripts + "/" + cli, 0o700)
         g.write("#!/bin/bash\n")
-        g.write("huckle cli run " + cli + " $@")
+        g.write("huckle cli run " + cli + " \"$@\"")
         g.close
 
 # initializes the configuration file of a given cli (initialized when a cli "created")
 def init_configuration(cli, url):
     config_file_path = dot_huckle_config + "/" + cli + "/config"
     parser = SafeConfigParser()
     parser.readfp(StringIO(u"[default]"))
```

### Comparing `huckle-3.0.0/huckle/data/huckle.1` & `huckle-3.0.1/huckle/data/huckle.1`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/huckle/hclinav.py` & `huckle-3.0.1/huckle/hclinav.py`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/huckle/huckle.py` & `huckle-3.0.1/huckle/huckle.py`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/huckle/hutils.py` & `huckle-3.0.1/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-3.0.0/huckle.egg-info/PKG-INFO` & `huckle-3.0.1/huckle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.0.0/setup.py` & `huckle-3.0.1/setup.py`

 * *Files identical despite different names*

