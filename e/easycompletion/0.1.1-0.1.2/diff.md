# Comparing `tmp/easycompletion-0.1.1.tar.gz` & `tmp/easycompletion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.1.tar", last modified: Fri Jul  7 11:59:10 2023, max compression
+gzip compressed data, was "easycompletion-0.1.2.tar", last modified: Fri Jul  7 12:02:12 2023, max compression
```

## Comparing `easycompletion-0.1.1.tar` & `easycompletion-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 11:59:10.477838 easycompletion-0.1.1/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.1/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 11:59:10.477655 easycompletion-0.1.1/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2929 2023-07-07 11:54:52.000000 easycompletion-0.1.1/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 11:59:10.476127 easycompletion-0.1.1/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      368 2023-07-07 11:59:06.000000 easycompletion-0.1.1/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      439 2023-07-07 11:44:12.000000 easycompletion-0.1.1/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    10224 2023-07-07 11:48:52.000000 easycompletion-0.1.1/easycompletion/language.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     1250 2023-07-07 11:55:29.000000 easycompletion-0.1.1/easycompletion/language_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 11:59:10.477377 easycompletion-0.1.1/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 11:59:10.000000 easycompletion-0.1.1/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      329 2023-07-07 11:59:10.000000 easycompletion-0.1.1/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 11:59:10.000000 easycompletion-0.1.1/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 11:59:10.000000 easycompletion-0.1.1/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-07 11:59:10.000000 easycompletion-0.1.1/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 11:59:10.477899 easycompletion-0.1.1/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-07 11:59:06.000000 easycompletion-0.1.1/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.418508 easycompletion-0.1.2/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.2/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 12:02:12.418309 easycompletion-0.1.2/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2929 2023-07-07 11:54:52.000000 easycompletion-0.1.2/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.412197 easycompletion-0.1.2/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      368 2023-07-07 12:02:08.000000 easycompletion-0.1.2/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      439 2023-07-07 11:44:12.000000 easycompletion-0.1.2/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    10224 2023-07-07 11:48:52.000000 easycompletion-0.1.2/easycompletion/language.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1250 2023-07-07 11:55:29.000000 easycompletion-0.1.2/easycompletion/language_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.418028 easycompletion-0.1.2/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      329 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 12:02:12.418564 easycompletion-0.1.2/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-07 12:02:08.000000 easycompletion-0.1.2/setup.py
```

### Comparing `easycompletion-0.1.1/LICENSE` & `easycompletion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.1/PKG-INFO` & `easycompletion-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.1/README.md` & `easycompletion-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.1/easycompletion/language.py` & `easycompletion-0.1.2/easycompletion/language.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.1/easycompletion/language_test.py` & `easycompletion-0.1.2/easycompletion/language_test.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.1/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.1.2/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.1/setup.py` & `easycompletion-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='easycompletion',
-    version='0.1.1',
+    version='0.1.2',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/easycompletion',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

