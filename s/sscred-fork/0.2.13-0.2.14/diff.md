# Comparing `tmp/sscred_fork-0.2.13.tar.gz` & `tmp/sscred_fork-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.13.tar", last modified: Wed Jul  5 10:13:19 2023, max compression
+gzip compressed data, was "dist/sscred_fork-0.2.14.tar", last modified: Fri Jul  7 14:30:32 2023, max compression
```

## Comparing `sscred_fork-0.2.13.tar` & `sscred_fork-0.2.14.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.13/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6655 2023-07-03 23:37:50.000000 sscred_fork-0.2.13/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-05 10:13:19.000000 sscred_fork-0.2.13/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.13/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.14/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.14/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-07 14:30:32.000000 sscred_fork-0.2.14/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.14/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.13/LICENSE` & `sscred_fork-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/PKG-INFO` & `sscred_fork-0.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.13
+Version: 0.2.14
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.13/README.md` & `sscred_fork-0.2.14/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/setup.cfg` & `sscred_fork-0.2.14/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.13
+version = 0.2.14
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.13/setup.py` & `sscred_fork-0.2.14/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/sscred/acl.py` & `sscred_fork-0.2.14/sscred/acl.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/sscred/blind_pedersen.py` & `sscred_fork-0.2.14/sscred/blind_pedersen.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/sscred/blind_signature.py` & `sscred_fork-0.2.14/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/sscred/commitment.py` & `sscred_fork-0.2.14/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.13/sscred/pack.py` & `sscred_fork-0.2.14/sscred/pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             kv['bc_param'] = obj.bc_param
         if hasattr(obj, 'pk'):
             kv['pk'] = obj.pk
         if hasattr(obj, 'z'):
             kv['z'] = obj.z
         if hasattr(obj, 'param'):
             kv['param'] = obj.param
+        if hasattr(obj, 'zeta'):
+            kv['zeta'] = obj.zeta
         data.update(kv)
 
         return packb(data)
 
     def dec(data):
         obj = cls.__new__(cls)
         for key, value in unpackb(data).items():
```

### Comparing `sscred_fork-0.2.13/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.14/sscred_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.13
+Version: 0.2.14
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.13/test/test_sscred.py` & `sscred_fork-0.2.14/test/test_sscred.py`

 * *Files identical despite different names*

