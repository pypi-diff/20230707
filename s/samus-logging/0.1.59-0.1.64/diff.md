# Comparing `tmp/samus-logging-0.1.59.tar.gz` & `tmp/samus-logging-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samus-logging-0.1.59.tar", last modified: Fri Jul  7 20:45:48 2023, max compression
+gzip compressed data, was "samus-logging-0.1.64.tar", last modified: Fri Jul  7 20:53:11 2023, max compression
```

## Comparing `samus-logging-0.1.59.tar` & `samus-logging-0.1.64.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:45:48.970219 samus-logging-0.1.59/
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.59/LICENSE
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:45:48.970219 samus-logging-0.1.59/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.59/README.md
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:45:48.970219 samus-logging-0.1.59/samus_logging/
--rw-rw-r--   0 samu      (1000) samu      (1000)       54 2023-07-07 20:37:42.000000 samus-logging-0.1.59/samus_logging/__init__.py
--rw-rw-r--   0 samu      (1000) samu      (1000)      277 2023-06-28 16:49:59.000000 samus-logging-0.1.59/samus_logging/level_filter.py
--rw-rw-r--   0 samu      (1000) samu      (1000)     4573 2023-07-07 20:45:46.000000 samus-logging-0.1.59/samus_logging/samus_logging.py
-drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:45:48.970219 samus-logging-0.1.59/samus_logging.egg-info/
--rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:45:48.000000 samus-logging-0.1.59/samus_logging.egg-info/PKG-INFO
--rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-07 20:45:48.000000 samus-logging-0.1.59/samus_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:45:48.000000 samus-logging-0.1.59/samus_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:45:48.000000 samus-logging-0.1.59/samus_logging.egg-info/requires.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-07 20:45:48.000000 samus-logging-0.1.59/samus_logging.egg-info/top_level.txt
--rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:45:48.970219 samus-logging-0.1.59/setup.cfg
--rw-rw-r--   0 samu      (1000) samu      (1000)      975 2023-07-07 20:39:48.000000 samus-logging-0.1.59/setup.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:53:11.230304 samus-logging-0.1.64/
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:05.000000 samus-logging-0.1.64/LICENSE
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:53:11.230304 samus-logging-0.1.64/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)        0 2023-06-28 14:33:21.000000 samus-logging-0.1.64/README.md
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:53:11.230304 samus-logging-0.1.64/samus_logging/
+-rw-rw-r--   0 samu      (1000) samu      (1000)       54 2023-07-07 20:52:33.000000 samus-logging-0.1.64/samus_logging/__init__.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)      277 2023-06-28 16:49:59.000000 samus-logging-0.1.64/samus_logging/level_filter.py
+-rw-rw-r--   0 samu      (1000) samu      (1000)     4648 2023-07-07 20:52:41.000000 samus-logging-0.1.64/samus_logging/samus_logging.py
+drwxrwxr-x   0 samu      (1000) samu      (1000)        0 2023-07-07 20:53:11.230304 samus-logging-0.1.64/samus_logging.egg-info/
+-rw-rw-r--   0 samu      (1000) samu      (1000)      389 2023-07-07 20:53:11.000000 samus-logging-0.1.64/samus_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 samu      (1000) samu      (1000)      303 2023-07-07 20:53:11.000000 samus-logging-0.1.64/samus_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)        1 2023-07-07 20:53:11.000000 samus-logging-0.1.64/samus_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       20 2023-07-07 20:53:11.000000 samus-logging-0.1.64/samus_logging.egg-info/requires.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       14 2023-07-07 20:53:11.000000 samus-logging-0.1.64/samus_logging.egg-info/top_level.txt
+-rw-rw-r--   0 samu      (1000) samu      (1000)       38 2023-07-07 20:53:11.230304 samus-logging-0.1.64/setup.cfg
+-rw-rw-r--   0 samu      (1000) samu      (1000)      975 2023-07-07 20:39:48.000000 samus-logging-0.1.64/setup.py
```

### Comparing `samus-logging-0.1.59/samus_logging/samus_logging.py` & `samus-logging-0.1.64/samus_logging/samus_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     DEFAULT_NAME = 'LOG'
     DEFAULT_LEVEL = 'INFO'
     DEFAULT_LOG_FILE = ''
     DEFAULT_MESSAGE_FORMAT = '%(name)s | %(asctime)s | %(levelname)s | %(filename)s | %(funcName)s() | %(message)s'
     DEFAULT_DATETIME_FORMAT = '%Y.%m.%d %H:%M:%S'
     dev_mode = False
+    log = None
 
     @classmethod
     def __init__(
             cls,
             level=DEFAULT_LEVEL,
             message_format=DEFAULT_MESSAGE_FORMAT,
             datetime_format=DEFAULT_DATETIME_FORMAT,
@@ -29,19 +30,21 @@
         - dev_mode: If True, set Level to 'DEBUG' \n
         """
         cls.dev_mode = dev_mode
 
         if cls.dev_mode:
             level = 'DEBUG'
             logging.basicConfig(level=level.strip().upper(), format=message_format.strip())
+            cls.log = logging
             logging.debug(f'Set basic Config (Dev-mode: {cls.dev_mode}, Level: \'{level}\', '
                           f'Message-format: {message_format}, Datetime-format: {datetime_format}).')
         else:
             logging.basicConfig(level=level.strip().upper(), format=message_format.strip(),
                                 datefmt=datetime_format.strip())
+            cls.log = logging
             logging.debug(f'Set basic Config (Level: \'{level}\', Message-format: {message_format}, '
                           f'Datetime-format: {datetime_format}).')
 
     @classmethod
     def create_logger(
             cls, name=DEFAULT_NAME, level=DEFAULT_LEVEL,
             file='', remove_old_file=True,
```

### Comparing `samus-logging-0.1.59/setup.py` & `samus-logging-0.1.64/setup.py`

 * *Files identical despite different names*

