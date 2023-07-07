# Comparing `tmp/genit-0.21.tar.gz` & `tmp/genit-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genit-0.21.tar", last modified: Wed Feb 15 17:53:48 2023, max compression
+gzip compressed data, was "genit-0.35.tar", last modified: Fri Jul  7 17:29:31 2023, max compression
```

## Comparing `genit-0.21.tar` & `genit-0.35.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:53:48.377748 genit-0.21/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-15 17:53:29.000000 genit-0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 17:53:29.000000 genit-0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-15 17:53:48.377748 genit-0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-15 17:53:29.000000 genit-0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:53:48.377748 genit-0.21/genit/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-15 17:53:29.000000 genit-0.21/genit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:53:48.377748 genit-0.21/genit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-15 17:53:48.000000 genit-0.21/genit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-15 17:53:48.000000 genit-0.21/genit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 17:53:48.000000 genit-0.21/genit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-15 17:53:48.000000 genit-0.21/genit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 17:53:48.377748 genit-0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-15 17:53:29.000000 genit-0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:29:31.980749 genit-0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-07 17:29:20.000000 genit-0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 17:29:20.000000 genit-0.35/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 17:29:31.980749 genit-0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-07 17:29:20.000000 genit-0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:29:31.980749 genit-0.35/genit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 17:29:20.000000 genit-0.35/genit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:29:31.980749 genit-0.35/genit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 17:29:31.000000 genit-0.35/genit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 17:29:31.000000 genit-0.35/genit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:29:31.000000 genit-0.35/genit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 17:29:31.000000 genit-0.35/genit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:29:31.980749 genit-0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-07 17:29:20.000000 genit-0.35/setup.py
```

### Comparing `genit-0.21/LICENSE` & `genit-0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `genit-0.21/genit/__init__.py` & `genit-0.35/genit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 
 import random
 
-def Gstr(length, add_characters = "") -> str:
+def str(length, add_characters = "") -> str:
 
     characters = "abcdefghijklmnopqrstuvwxyz" + add_characters
 
     random_str = ""
 
     for i in range(length):
         random_str = "{}{}".format(random_str, characters[random.randint(0, len(characters) - 1)])
 
     return random_str
 
-def Gint(length) -> int:
+def int(length) -> int:
 
     characters = "1234567890"
 
     random_int = ""
 
     for i in range(length):
         random_int = "{}{}".format(random_int, characters[random.randint(0, len(characters) - 1)])
 
     return int(random_int)
 
-def Gall(length, add_characters = "") -> str:
+def all(length, add_characters = "") -> str:
 
     characters = "abcdefghijklmnopqrstuvwxyz1234567890" + add_characters
 
     random_str = ""
 
     for i in range(length):
         random_str = "{}{}".format(random_str, characters[random.randint(0, len(characters) - 1)])
 
     return random_str
 
-def Gspecial(length, characters) -> str:
+def special(length, characters) -> str:
 
     characters = "" + characters
     random_str = ""
 
     for i in range(length):
         random_str = "{}{}".format(random_str, characters[random.randint(0, len(characters) - 1)])
```

### Comparing `genit-0.21/setup.py` & `genit-0.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='genit',
-    version='0.21',
+    version='0.35',
     description='Simple integer and string Generator',
     Long_description= open("README.md").read() + "\n\n" + open('CHANGELOG.txt').read(),
     url = "https://github.com/devmoamal/genit", 
     author='Moamal Hussin',
     author_email='dev.moamal@gmail.com',
     License= 'MIT',
     classifiers=classifiers,
```

