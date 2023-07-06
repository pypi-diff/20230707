# Comparing `tmp/datatypes-0.9.5.tar.gz` & `tmp/datatypes-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatypes-0.9.5.tar", last modified: Wed Jul  5 00:00:59 2023, max compression
+gzip compressed data, was "datatypes-0.9.6.tar", last modified: Wed Jul  5 23:30:09 2023, max compression
```

## Comparing `datatypes-0.9.5.tar` & `datatypes-0.9.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.261099 datatypes-0.9.5/
--rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.5/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 00:00:59.260957 datatypes-0.9.5/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.5/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.259472 datatypes-0.9.5/datatypes/
--rw-r--r--   0 jaymon     (501) staff       (20)     2287 2023-07-04 23:59:31.000000 datatypes-0.9.5/datatypes/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.5/datatypes/collections.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.5/datatypes/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.5/datatypes/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.5/datatypes/copy.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.5/datatypes/csv.py
--rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.5/datatypes/datetime.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.260752 datatypes-0.9.5/datatypes/decorators/
--rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.5/datatypes/decorators/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.5/datatypes/decorators/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.5/datatypes/decorators/descriptor.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.5/datatypes/decorators/misc.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.5/datatypes/email.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.5/datatypes/enum.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.5/datatypes/environ.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.5/datatypes/event.py
--rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.5/datatypes/html.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.5/datatypes/http.py
--rw-r--r--   0 jaymon     (501) staff       (20)    12930 2023-07-04 00:02:42.000000 datatypes-0.9.5/datatypes/logging.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5758 2023-06-13 23:17:08.000000 datatypes-0.9.5/datatypes/number.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3739 2023-02-27 22:36:06.000000 datatypes-0.9.5/datatypes/parse.py
--rw-r--r--   0 jaymon     (501) staff       (20)   124655 2023-06-29 22:48:32.000000 datatypes-0.9.5/datatypes/path.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.5/datatypes/profile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    36242 2023-07-04 22:29:52.000000 datatypes-0.9.5/datatypes/reflection.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11373 2023-06-24 18:12:15.000000 datatypes-0.9.5/datatypes/server.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.5/datatypes/service.py
--rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.5/datatypes/string.py
--rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.5/datatypes/token.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.5/datatypes/url.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.5/datatypes/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.260189 datatypes-0.9.5/datatypes.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-05 00:00:59.261141 datatypes-0.9.5/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.5/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 23:30:09.341682 datatypes-0.9.6/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.6/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 23:30:09.341529 datatypes-0.9.6/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.6/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 23:30:09.339001 datatypes-0.9.6/datatypes/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2287 2023-07-05 23:28:51.000000 datatypes-0.9.6/datatypes/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.6/datatypes/collections.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.6/datatypes/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.6/datatypes/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.6/datatypes/copy.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.6/datatypes/csv.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.6/datatypes/datetime.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 23:30:09.341196 datatypes-0.9.6/datatypes/decorators/
+-rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.6/datatypes/decorators/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.6/datatypes/decorators/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.6/datatypes/decorators/descriptor.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.6/datatypes/decorators/misc.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.6/datatypes/email.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.6/datatypes/enum.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.6/datatypes/environ.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.6/datatypes/event.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.6/datatypes/html.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.6/datatypes/http.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12930 2023-07-04 00:02:42.000000 datatypes-0.9.6/datatypes/logging.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5758 2023-06-13 23:17:08.000000 datatypes-0.9.6/datatypes/number.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4915 2023-07-05 17:47:40.000000 datatypes-0.9.6/datatypes/parse.py
+-rw-r--r--   0 jaymon     (501) staff       (20)   124655 2023-06-29 22:48:32.000000 datatypes-0.9.6/datatypes/path.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.6/datatypes/profile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    36242 2023-07-04 22:29:52.000000 datatypes-0.9.6/datatypes/reflection.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11373 2023-06-24 18:12:15.000000 datatypes-0.9.6/datatypes/server.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.6/datatypes/service.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.6/datatypes/string.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.6/datatypes/token.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.6/datatypes/url.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.6/datatypes/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 23:30:09.339599 datatypes-0.9.6/datatypes.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 23:30:09.000000 datatypes-0.9.6/datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-07-05 23:30:09.000000 datatypes-0.9.6/datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-05 23:30:09.000000 datatypes-0.9.6/datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-07-05 23:30:09.000000 datatypes-0.9.6/datatypes.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-05 23:30:09.341726 datatypes-0.9.6/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.6/setup.py
```

### Comparing `datatypes-0.9.5/LICENSE.txt` & `datatypes-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/PKG-INFO` & `datatypes-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.5
+Version: 0.9.6
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.5/datatypes/__init__.py` & `datatypes-0.9.6/datatypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,14 @@
 from .server import (
     PathServer,
     CallbackServer,
     WSGIServer,
 )
 
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 
 # get rid of "No handler found" warnings (cribbed from requests)
 # DEPRECATED 7-15-2022, doesn't seem to be needed in python3
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `datatypes-0.9.5/datatypes/collections.py` & `datatypes-0.9.6/datatypes/collections.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/compat.py` & `datatypes-0.9.6/datatypes/compat.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/config.py` & `datatypes-0.9.6/datatypes/config.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/copy.py` & `datatypes-0.9.6/datatypes/copy.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/csv.py` & `datatypes-0.9.6/datatypes/csv.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/datetime.py` & `datatypes-0.9.6/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/decorators/base.py` & `datatypes-0.9.6/datatypes/decorators/base.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/decorators/descriptor.py` & `datatypes-0.9.6/datatypes/decorators/descriptor.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/decorators/misc.py` & `datatypes-0.9.6/datatypes/decorators/misc.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/email.py` & `datatypes-0.9.6/datatypes/email.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/enum.py` & `datatypes-0.9.6/datatypes/enum.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/environ.py` & `datatypes-0.9.6/datatypes/environ.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/event.py` & `datatypes-0.9.6/datatypes/event.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/html.py` & `datatypes-0.9.6/datatypes/html.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/http.py` & `datatypes-0.9.6/datatypes/http.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/logging.py` & `datatypes-0.9.6/datatypes/logging.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/number.py` & `datatypes-0.9.6/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/parse.py` & `datatypes-0.9.6/datatypes/parse.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,61 +7,95 @@
 from .string import String
 
 
 class ArgvParser(dict):
     """Parses what is contained in sys.argv or the extra list of argparse.parse_known_args()
 
     :Example:
-        d = ArgumentParser([
+        d = ArgvParser([
             "--foo=1",
             "--bar",
             "che"
         ])
         print(d["foo"]) # ["1"]
         print(d["bar"]) # ["che"]
     """
-    def __init__(self, argv):
+    def __init__(self, argv, **kwargs):
         """
         :param argv: list<str>, the argv list or the extra args returned from parse_known_args
             https://docs.python.org/3/library/sys.html#sys.argv
             https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.parse_known_args
+        :param **kwargs: passed through to .normalize_* methods
         :returns: dict, key is the arg name (* for non positional args) and value is
             a list of found arguments (so --foo 1 --foo 2 is supported). The value is
             always a list of strings
         """
         d = defaultdict(list)
         i = 0
         length = len(argv)
         while i < length:
             argv[i] = String(argv[i])
             if argv[i].startswith("-"):
                 s = argv[i].lstrip("-")
                 bits = s.split("=", 1)
                 if len(bits) > 1:
-                    key = bits[0]
-                    val = bits[1].strip("\"'")
+                    key = self.normalize_key(
+                        bits[0],
+                        **kwargs
+                    )
+                    val = self.normalize_value(
+                        bits[1].strip("\"'"),
+                        **kwargs
+                    )
+
                     d[key].append(val)
 
                 else:
+                    s = self.normalize_key(s, **kwargs)
+
                     if i + 1 < length:
                         argv[i + 1] = String(argv[i + 1])
                         if argv[i + 1].startswith("-"):
-                            d[s].append(True)
+                            val = self.normalize_value(True, **kwargs)
+                            d[s].append(val)
 
                         else:
-                            d[s].append(argv[i + 1])
+                            val = self.normalize_value(argv[i + 1], **kwargs)
+                            d[s].append(val)
                             i += 1
 
+                    else:
+                        # the last flag is a boolean flag
+                        val = self.normalize_value(True, **kwargs)
+                        d[s].append(val)
+
             else:
                 d["*"].append(argv[i])
 
             i += 1
 
         super().__init__(d)
 
+    def normalize_key(self, k, **kwargs):
+        """Normalize the key
+
+        :param **kwargs:
+            * hyphen_to_underscore: bool, convert hyphens to underscores (eg, 
+                foo-bar becomes foo_bar)
+        :returns: str, the normalized key
+        """
+        htu = kwargs.get("hyphen_to_underscore", False)
+        if htu:
+            k = k.replace("-", "_")
+        return k
+
+    def normalize_value(self, v, **kwargs):
+        """normalize the value"""
+        return v
+
     def unwrap(self, ignore_keys=None):
         """remove list wrapper of any value that has a count of 1
 
         by default, this returns lists for everything because it has no idea what
         might have multiple values so it treats everything as if it has multiple values
         so it can support things like `--foo=1 --foo=2` but that might not be wanted,
         so this method will return a dict with any value that has a length of one it
@@ -94,15 +128,15 @@
 
     all values will be lists, this is for uniformity, if you want to squash lists
     that only contain one value to just have the value then call .unwrap()
 
     References:
         * https://stackoverflow.com/questions/44945815/
     """
-    def __init__(self, argline):
+    def __init__(self, argline, **kwargs):
         """
         :param argline: str, the arguments string that should be parsed
         """
         # https://docs.python.org/3/library/shlex.html#shlex.split
         argv = shlex.split(argline)
-        super().__init__(argv)
+        super().__init__(argv, **kwargs)
```

### Comparing `datatypes-0.9.5/datatypes/path.py` & `datatypes-0.9.6/datatypes/path.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/profile.py` & `datatypes-0.9.6/datatypes/profile.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/reflection.py` & `datatypes-0.9.6/datatypes/reflection.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/server.py` & `datatypes-0.9.6/datatypes/server.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/service.py` & `datatypes-0.9.6/datatypes/service.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/string.py` & `datatypes-0.9.6/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/token.py` & `datatypes-0.9.6/datatypes/token.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/url.py` & `datatypes-0.9.6/datatypes/url.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes/utils.py` & `datatypes-0.9.6/datatypes/utils.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/datatypes.egg-info/PKG-INFO` & `datatypes-0.9.6/datatypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.5
+Version: 0.9.6
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.5/datatypes.egg-info/SOURCES.txt` & `datatypes-0.9.6/datatypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.5/setup.py` & `datatypes-0.9.6/setup.py`

 * *Files identical despite different names*

