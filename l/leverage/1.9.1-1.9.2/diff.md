# Comparing `tmp/leverage-1.9.1.tar.gz` & `tmp/leverage-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leverage-1.9.1.tar", last modified: Fri Jan 13 15:39:05 2023, max compression
+gzip compressed data, was "leverage-1.9.2.tar", last modified: Mon Jan 30 14:41:21 2023, max compression
```

## Comparing `leverage-1.9.1.tar` & `leverage-1.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:39:05.774086 leverage-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-13 15:38:01.000000 leverage-1.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-13 15:39:05.774086 leverage-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-13 15:38:01.000000 leverage-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:39:05.774086 leverage-1.9.1/leverage/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-13 15:39:04.000000 leverage-1.9.1/leverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/_internals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/leverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:39:05.774086 leverage-1.9.1/leverage/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/modules/tfautomv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-01-13 15:38:01.000000 leverage-1.9.1/leverage/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:39:05.774086 leverage-1.9.1/leverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-13 15:39:05.000000 leverage-1.9.1/leverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-13 15:38:01.000000 leverage-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-13 15:39:05.778086 leverage-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-13 15:38:01.000000 leverage-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-30 14:40:19.000000 leverage-1.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-30 14:41:21.986854 leverage-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-30 14:40:19.000000 leverage-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/leverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/tfautomv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-30 14:40:19.000000 leverage-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-30 14:41:21.986854 leverage-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-30 14:40:19.000000 leverage-1.9.2/setup.py
```

### Comparing `leverage-1.9.1/LICENSE.txt` & `leverage-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/PKG-INFO` & `leverage-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leverage
-Version: 1.9.1
+Version: 1.9.2
 Summary: Binbash Leverage Command-Line tool.
 Home-page: https://github.com/binbashar/leverage
 Author: BinBash Inc
 Author-email: leverage@binbash.com.ar
 License: MIT License
 Project-URL: Source Code, https://github.com/binbashar/leverage
 Keywords: BINBASH,LEVERAGE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: leverage Version: 1.9.1 Summary: Binbash Leverage
+Metadata-Version: 2.1 Name: leverage Version: 1.9.2 Summary: Binbash Leverage
 Command-Line tool. Home-page: https://github.com/binbashar/leverage Author:
 BinBash Inc Author-email: leverage@binbash.com.ar License: MIT License Project-
 URL: Source Code, https://github.com/binbashar/leverage Keywords:
 BINBASH,LEVERAGE Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `leverage-1.9.1/README.md` & `leverage-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/_internals.py` & `leverage-1.9.2/leverage/_internals.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/_parsing.py` & `leverage-1.9.2/leverage/_parsing.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/_utils.py` & `leverage-1.9.2/leverage/_utils.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/conf.py` & `leverage-1.9.2/leverage/conf.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/container.py` & `leverage-1.9.2/leverage/container.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/leverage.py` & `leverage-1.9.2/leverage/leverage.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/logger.py` & `leverage-1.9.2/leverage/logger.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/modules/aws.py` & `leverage-1.9.2/leverage/modules/aws.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/modules/credentials.py` & `leverage-1.9.2/leverage/modules/credentials.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/modules/project.py` & `leverage-1.9.2/leverage/modules/project.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/modules/run.py` & `leverage-1.9.2/leverage/modules/run.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/modules/terraform.py` & `leverage-1.9.2/leverage/modules/terraform.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,19 @@
 
     # validate each layer before calling the execute command
     for layer in layers:
         logger.debug(f"Checking for layer {layer}...")
         # change to current dir and set it in the container
         tf.cwd = layer
 
+        # check layers existence
+        if not layer.is_dir():
+            logger.error(f"Directory [red]{layer}[/red] does not exist or is not a directory\n")
+            raise Exit(1)
+
         # set the s3 key
         tf.set_backend_key(skip_validation)
 
         #validate layer
         validate_for_all_commands(layer, skip_validation=skip_validation)
 
         # change to original dir and set it in the container
@@ -256,20 +261,15 @@
     Validate existense of layer and, if set, all the Leverage related stuff
     of each of them
 
     Args:
         layer: a full layer directory
     """
 
-    # check layers existence
     logger.debug(f"Checking layer {layer}...")
-    if not layer.is_dir():
-        logger.error(f"Directory [red]{layer}[/red] does not exist or is not a directory\n")
-        raise Exit(1)
-
     if not skip_validation and not _validate_layout():
         logger.error("Layer configuration doesn't seem to be valid. Exiting.\n"
                     "If you are sure your configuration is actually correct "
                     "you may skip this validation using the --skip-validation flag.")
         raise Exit(1)
 
 # ###########################################################################
@@ -279,17 +279,14 @@
 def _init(tf, args):
     """ Initialize this layer. """
 
     args = [arg for index, arg in enumerate(args)
             if not arg.startswith("-backend-config") or not arg[index - 1] == "-backend-config"]
     args.append(f"-backend-config={tf.backend_tfvars}")
     args.append(f"-backend-config=\"region={tf.terraform_backend.get('region')}\"")
-    # if the backend key is set send it as a backend config
-    if not tf.backend_key is None:
-        args.append(f"-backend-config=\"key={tf.backend_key}\"")
 
     exit_code = tf.start_in_layer("init", *args)
 
     if exit_code:
         raise Exit(exit_code)
```

### Comparing `leverage-1.9.1/leverage/modules/tfautomv.py` & `leverage-1.9.2/leverage/modules/tfautomv.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/path.py` & `leverage-1.9.2/leverage/path.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage/tasks.py` & `leverage-1.9.2/leverage/tasks.py`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/leverage.egg-info/PKG-INFO` & `leverage-1.9.2/leverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leverage
-Version: 1.9.1
+Version: 1.9.2
 Summary: Binbash Leverage Command-Line tool.
 Home-page: https://github.com/binbashar/leverage
 Author: BinBash Inc
 Author-email: leverage@binbash.com.ar
 License: MIT License
 Project-URL: Source Code, https://github.com/binbashar/leverage
 Keywords: BINBASH,LEVERAGE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: leverage Version: 1.9.1 Summary: Binbash Leverage
+Metadata-Version: 2.1 Name: leverage Version: 1.9.2 Summary: Binbash Leverage
 Command-Line tool. Home-page: https://github.com/binbashar/leverage Author:
 BinBash Inc Author-email: leverage@binbash.com.ar License: MIT License Project-
 URL: Source Code, https://github.com/binbashar/leverage Keywords:
 BINBASH,LEVERAGE Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `leverage-1.9.1/leverage.egg-info/SOURCES.txt` & `leverage-1.9.2/leverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leverage-1.9.1/setup.cfg` & `leverage-1.9.2/setup.cfg`

 * *Files identical despite different names*

