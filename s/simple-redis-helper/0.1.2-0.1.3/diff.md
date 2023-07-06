# Comparing `tmp/simple-redis-helper-0.1.2.tar.gz` & `tmp/simple-redis-helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-redis-helper-0.1.2.tar", last modified: Fri Oct  1 03:15:47 2021, max compression
+gzip compressed data, was "simple-redis-helper-0.1.3.tar", last modified: Thu Jul  6 23:17:43 2023, max compression
```

## Comparing `simple-redis-helper-0.1.2.tar` & `simple-redis-helper-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      291 2021-10-01 03:12:58.000000 simple-redis-helper-0.1.2/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      116 2021-09-14 00:46:54.000000 simple-redis-helper-0.1.2/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 simple-redis-helper-0.1.2/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1102 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4405 2021-10-01 03:14:38.000000 simple-redis-helper-0.1.2/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1304 2021-10-01 03:12:58.000000 simple-redis-helper-0.1.2/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/src/simple_redis_helper/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:45:09.000000 simple-redis-helper-0.1.2/src/simple_redis_helper/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2527 2021-09-22 03:03:34.000000 simple-redis-helper-0.1.2/src/simple_redis_helper/broadcast.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3732 2021-10-01 03:14:22.000000 simple-redis-helper-0.1.2/src/simple_redis_helper/listen.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1706 2021-09-14 01:11:43.000000 simple-redis-helper-0.1.2/src/simple_redis_helper/load.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2011 2021-09-14 01:11:43.000000 simple-redis-helper-0.1.2/src/simple_redis_helper/save.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-10-01 03:15:47.256741 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1102 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      513 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      213 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       20 2021-10-01 03:15:47.000000 simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      443 2023-07-06 23:16:13.000000 simple-redis-helper-0.1.3/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      116 2021-09-14 00:46:54.000000 simple-redis-helper-0.1.3/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 simple-redis-helper-0.1.3/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1302 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6466 2023-07-06 23:16:13.000000 simple-redis-helper-0.1.3/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1304 2023-07-06 23:17:14.000000 simple-redis-helper-0.1.3/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/simple_redis_helper/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:45:09.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2994 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/broadcast.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4185 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/listen.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2174 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/load.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2479 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/save.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1159 2023-07-06 23:12:45.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1302 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      546 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      213 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       20 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/top_level.txt
```

### Comparing `simple-redis-helper-0.1.2/PKG-INFO` & `simple-redis-helper-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: simple-redis-helper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Command-line utilities to for sending/receiving data to/from a Redis backend.
 Home-page: https://github.com/fracpete/redis_helper
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Little command-line library to send/receive data to/from a Redis backend.
         
         https://github.com/fracpete/redis_helper
         
         Changelog
         =========
         
+        0.1.3 (2023-07-07)
+        ------------------
+        
+        - added support for supplying a password for connecting to the Redis server (`--password` or `--password_env`)
+        
+        
         0.1.2 (2021-10-01)
         ------------------
         
         - `listen.py` now supports output in a directory
         
         
         0.1.1 (2021-09-22)
```

### Comparing `simple-redis-helper-0.1.2/setup.py` & `simple-redis-helper-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=[
       'simple_redis_helper',
     ],
-    version="0.1.2",
+    version="0.1.3",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     install_requires=[
         "redis",
     ],
     entry_points={
         "console_scripts": [
```

### Comparing `simple-redis-helper-0.1.2/src/simple_redis_helper/broadcast.py` & `simple-redis-helper-0.1.3/src/simple_redis_helper/broadcast.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import redis
 import traceback
+from simple_redis_helper.utils import get_password
 
 
 def main(args=None):
     """
     The main method for parsing command-line arguments and running the application.
 
     :param args: the commandline arguments, uses sys.argv if not supplied
@@ -12,27 +13,30 @@
     """
     parser = argparse.ArgumentParser(
         prog="simple_redis_helper-broadcast",
         description="Loads a file and broadcasts its content to the specified Redis channel.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-H', '--host', metavar='HOST', required=False, default="localhost", help='The redis server to connect to')
     parser.add_argument('-p', '--port', metavar='PORT', required=False, default=6379, type=int, help='The port the redis server is listening on')
+    parser.add_argument('--password', metavar='PASSWORD', required=False, default=None, type=str, help='The password to use for the redis server (takes precedence over --password_env)')
+    parser.add_argument('--password_env', metavar='PASSWORD', required=False, default=None, type=str, help='The environment variable to obtain the password from to use for connecting')
     parser.add_argument('-d', '--database', metavar='DB', required=False, default=0, type=int, help='The redis database to use')
     parser.add_argument('-c', '--channel', metavar='CHANNEL', required=True, default=None, help='The channel to broadcast the content on')
     parser.add_argument('-f', '--file', metavar='FILE', default=None, help='The file to load into Redis (if not using a string)')
     parser.add_argument('-b', '--binary', action="store_true", help='Whether to treat the file as binary')
     parser.add_argument('-s', '--string', metavar='STR', default=None, help='The string to load into Redis (if not reading a file)')
     parsed = parser.parse_args(args=args)
 
     if (parsed.file is None) and (parsed.string is None):
         raise Exception("Either file or string need to be supplied")
     if (parsed.file is not None) and (parsed.string is not None):
         raise Exception("File and string cannot be supplied at the same time")
 
-    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database)
+    # connect
+    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database, password=get_password(parsed))
 
     if parsed.file is not None:
         if parsed.binary:
             with open(parsed.file, "rb") as f:
                 content = f.read()
         else:
             with open(parsed.file, "r") as f:
```

### Comparing `simple-redis-helper-0.1.2/src/simple_redis_helper/listen.py` & `simple-redis-helper-0.1.3/src/simple_redis_helper/listen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import os
 import redis
 import traceback
 from datetime import datetime
+from simple_redis_helper.utils import get_password
 
 DATETIME_FORMAT_URL = "https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes"
 
 
 def main(args=None):
     """
     The main method for parsing command-line arguments and running the application.
@@ -16,14 +17,16 @@
     """
     parser = argparse.ArgumentParser(
         prog="simple_redis_helper-listen",
         description="Listens to the specified channel for messages to come through and outputs them on stdout if no output directory provided.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-H', '--host', metavar='HOST', required=False, default="localhost", help='The redis server to connect to')
     parser.add_argument('-p', '--port', metavar='PORT', required=False, default=6379, type=int, help='The port the redis server is listening on')
+    parser.add_argument('--password', metavar='PASSWORD', required=False, default=None, type=str, help='The password to use for the redis server (takes precedence over --password_env)')
+    parser.add_argument('--password_env', metavar='PASSWORD', required=False, default=None, type=str, help='The environment variable to obtain the password from to use for connecting')
     parser.add_argument('-d', '--database', metavar='DB', required=False, default=0, type=int, help='The redis database to use')
     parser.add_argument('-c', '--channel', metavar='CHANNEL', required=True, default=None, help='The channel to broadcast the content on')
     parser.add_argument('-D', '--data_only', action='store_true', help='Whether to output only the message data')
     parser.add_argument('-s', '--convert_to_string', action='store_true', help='Whether to convert the message data to string (requires --data_only)')
     parser.add_argument('-o', '--output_dir', metavar='DIR', required=False, default=None, help='The directory to store the received messages/data in')
     parser.add_argument("-f", "--file_format", metavar="FORMAT", help="the format to use for the output files (when using '--output_dir'), see: %s" % DATETIME_FORMAT_URL, required=False, default="%Y%m%d_%H%M%S.%f.dat")
     parsed = parser.parse_args(args=args)
@@ -37,15 +40,15 @@
     # check output format
     try:
         datetime.now().strftime(parsed.file_format)
     except Exception as e:
         raise Exception("Invalid timestamp format: %s\nSee: %s" % (parsed.file_format, DATETIME_FORMAT_URL)) from e
 
     # connect
-    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database)
+    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database, password=get_password(parsed))
 
     # handler for listening/outputting
     def anon_handler(message):
         data = message
         if parsed.data_only:
             data = message['data']
             if parsed.convert_to_string:
```

### Comparing `simple-redis-helper-0.1.2/src/simple_redis_helper/save.py` & `simple-redis-helper-0.1.3/src/simple_redis_helper/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import argparse
 import redis
 import traceback
+from simple_redis_helper.utils import get_password
 
 
 def main(args=None):
     """
     The main method for parsing command-line arguments and running the application.
 
     :param args: the commandline arguments, uses sys.argv if not supplied
     :type args: list
     """
     parser = argparse.ArgumentParser(
-        prog="simple_redis_helper-save",
-        description="Saves the content from a Redis key in the specified file.",
+        prog="simple_redis_helper-load",
+        description="Loads a file into Redis under the specified key.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-H', '--host', metavar='HOST', required=False, default="localhost", help='The redis server to connect to')
     parser.add_argument('-p', '--port', metavar='PORT', required=False, default=6379, type=int, help='The port the redis server is listening on')
+    parser.add_argument('--password', metavar='PASSWORD', required=False, default=None, type=str, help='The password to use for the redis server (takes precedence over --password_env)')
+    parser.add_argument('--password_env', metavar='PASSWORD', required=False, default=None, type=str, help='The environment variable to obtain the password from to use for connecting')
     parser.add_argument('-d', '--database', metavar='DB', required=False, default=0, type=int, help='The redis database to use')
-    parser.add_argument('-k', '--key', metavar='KEY', required=True, default=None, help='The key to retrieve')
-    parser.add_argument('-f', '--file', metavar='FILE', required=False, default=None, help='The file to save the content in. Outputs the content to stdout if not provided.')
-    parser.add_argument('-s', '--convert_to_string', action='store_true', help='Whether to convert the retrieved bytes to string')
+    parser.add_argument('-k', '--key', metavar='KEY', required=True, default=None, help='The key to store the file content under')
+    parser.add_argument('-f', '--file', metavar='FILE', required=True, default=None, help='The file to load into Redis')
     parsed = parser.parse_args(args=args)
 
-    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database)
-    content = r.get(parsed.key)
-    if parsed.convert_to_string:
-        content = content.decode()
-    if parsed.file is None:
-        print(content)
-    else:
-        with open(parsed.file, "w") as f:
-            f.write(content)
+    # connect
+    r = redis.Redis(host=parsed.host, port=parsed.port, db=parsed.database, password=get_password(parsed))
+
+    with open(parsed.file, "r") as f:
+        content = f.read()
+        r.set(parsed.key, content)
 
 
 def sys_main():
     """
     Runs the main function using the system cli arguments, and
     returns a system error code.
     :return: 0 for success, 1 for failure.
```

### Comparing `simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/PKG-INFO` & `simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: simple-redis-helper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Command-line utilities to for sending/receiving data to/from a Redis backend.
 Home-page: https://github.com/fracpete/redis_helper
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Little command-line library to send/receive data to/from a Redis backend.
         
         https://github.com/fracpete/redis_helper
         
         Changelog
         =========
         
+        0.1.3 (2023-07-07)
+        ------------------
+        
+        - added support for supplying a password for connecting to the Redis server (`--password` or `--password_env`)
+        
+        
         0.1.2 (2021-10-01)
         ------------------
         
         - `listen.py` now supports output in a directory
         
         
         0.1.1 (2021-09-22)
```

### Comparing `simple-redis-helper-0.1.2/src/simple_redis_helper.egg-info/SOURCES.txt` & `simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 README.md
 setup.py
 src/simple_redis_helper/__init__.py
 src/simple_redis_helper/broadcast.py
 src/simple_redis_helper/listen.py
 src/simple_redis_helper/load.py
 src/simple_redis_helper/save.py
+src/simple_redis_helper/utils.py
 src/simple_redis_helper.egg-info/PKG-INFO
 src/simple_redis_helper.egg-info/SOURCES.txt
 src/simple_redis_helper.egg-info/dependency_links.txt
 src/simple_redis_helper.egg-info/entry_points.txt
 src/simple_redis_helper.egg-info/requires.txt
 src/simple_redis_helper.egg-info/top_level.txt
```

