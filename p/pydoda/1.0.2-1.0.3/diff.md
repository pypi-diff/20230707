# Comparing `tmp/pydoda-1.0.2.tar.gz` & `tmp/pydoda-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoda-1.0.2.tar", last modified: Fri Jul  7 21:41:32 2023, max compression
+gzip compressed data, was "pydoda-1.0.3.tar", last modified: Fri Jul  7 21:49:58 2023, max compression
```

## Comparing `pydoda-1.0.2.tar` & `pydoda-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,74 @@
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.496249 pydoda-1.0.2/
--rw-rw-r--   0 saad      (1000) saad      (1000)     2572 2023-07-07 12:52:32.000000 pydoda-1.0.2/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:41:32.496249 pydoda-1.0.2/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)     4900 2023-07-07 21:39:16.000000 pydoda-1.0.2/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda/
--rw-rw-r--   0 saad      (1000) saad      (1000)      795 2023-06-26 22:43:54.000000 pydoda-1.0.2/pydoda/__init__.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4719 2023-06-26 12:14:41.000000 pydoda-1.0.2/pydoda/category.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4014 2023-06-26 23:18:19.000000 pydoda-1.0.2/pydoda/custom_category.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda/dataset/
--rw-rw-r--   0 saad      (1000) saad      (1000)     1235 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)     3877 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/README.md
--rw-rw-r--   0 saad      (1000) saad      (1000)    49090 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/imagenet_b_darija.csv
--rw-rw-r--   0 saad      (1000) saad      (1000)      460 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/progress.py
--rw-rw-r--   0 saad      (1000) saad      (1000)   589131 2023-06-26 11:43:35.000000 pydoda-1.0.2/pydoda/dataset/sentences.csv
--rw-rw-r--   0 saad      (1000) saad      (1000)     3786 2023-06-26 23:07:25.000000 pydoda-1.0.2/pydoda/loader.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     2772 2023-06-26 23:45:18.000000 pydoda-1.0.2/pydoda/py_doda.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     3497 2023-06-26 22:45:08.000000 pydoda-1.0.2/pydoda/sentence.py
--rw-rw-r--   0 saad      (1000) saad      (1000)      367 2023-07-07 21:32:50.000000 pydoda-1.0.2/pydoda/utils.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.492249 pydoda-1.0.2/pydoda.egg-info/
--rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)      513 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/SOURCES.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/dependency_links.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        7 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/requires.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       13 2023-07-07 21:41:32.000000 pydoda-1.0.2/pydoda.egg-info/top_level.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-07 21:41:32.496249 pydoda-1.0.2/setup.cfg
--rw-rw-r--   0 saad      (1000) saad      (1000)     1222 2023-07-07 21:41:22.000000 pydoda-1.0.2/setup.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:41:32.496249 pydoda-1.0.2/tests/
--rw-rw-r--   0 saad      (1000) saad      (1000)        0 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/__init__.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     4646 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/test_category.py
--rw-rw-r--   0 saad      (1000) saad      (1000)     2555 2023-06-27 12:10:35.000000 pydoda-1.0.2/tests/test_py_doda.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.738968 pydoda-1.0.3/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2572 2023-07-07 12:52:32.000000 pydoda-1.0.3/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:49:58.738968 pydoda-1.0.3/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4900 2023-07-07 21:39:16.000000 pydoda-1.0.3/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.730969 pydoda-1.0.3/pydoda/
+-rw-rw-r--   0 saad      (1000) saad      (1000)      795 2023-06-26 22:43:54.000000 pydoda-1.0.3/pydoda/__init__.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4719 2023-06-26 12:14:41.000000 pydoda-1.0.3/pydoda/category.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4014 2023-06-26 23:18:19.000000 pydoda-1.0.3/pydoda/custom_category.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.730969 pydoda-1.0.3/pydoda/dataset/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1235 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3877 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/README.md
+-rw-rw-r--   0 saad      (1000) saad      (1000)    49090 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/imagenet_b_darija.csv
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.734969 pydoda-1.0.3/pydoda/dataset/images/
+-rw-rw-r--   0 saad      (1000) saad      (1000)    25454 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/images/doda_logo.png
+-rw-rw-r--   0 saad      (1000) saad      (1000)   175684 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/images/video_img.png
+-rw-rw-r--   0 saad      (1000) saad      (1000)   282921 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/images/wordcloud.png
+-rw-rw-r--   0 saad      (1000) saad      (1000)      460 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/progress.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.738968 pydoda-1.0.3/pydoda/dataset/semantic categories/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3379 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/animals.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2776 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/art.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1280 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/clothes.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)      666 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/colors.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3284 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/economy.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3170 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/education.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2044 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/emotions.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2426 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/environment.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1117 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/family.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2109 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/femalenames.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4596 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/food.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1966 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/health.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2311 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/humanbody.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2323 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/malenames.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3365 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/numbers.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5328 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/places.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)      487 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/plants.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1396 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/professions.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2588 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/religion.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1326 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/sport.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2817 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/semantic categories/time.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)   589131 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/sentences.csv
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.738968 pydoda-1.0.3/pydoda/dataset/syntactic categories/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2113 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/(in)definite.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    22273 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/adjectives.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3233 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/adverbs.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    61083 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/conjug_past.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    80724 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/conjug_present.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    27072 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/imperatives.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    27927 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/masculine_feminine_plural.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    36874 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/nouns.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1276 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/prepositions.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1179 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/pronouns.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    14003 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/verb-to-noun.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)    37059 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/syntactic categories/verbs.csv
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.738968 pydoda-1.0.3/pydoda/dataset/x-tra/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1455 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/x-tra/idioms.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)      774 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/x-tra/proverbs.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     9027 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/x-tra/utils.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2458 2023-06-26 11:43:35.000000 pydoda-1.0.3/pydoda/dataset/x-tra/weird.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3786 2023-06-26 23:07:25.000000 pydoda-1.0.3/pydoda/loader.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2772 2023-06-26 23:45:18.000000 pydoda-1.0.3/pydoda/py_doda.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     3497 2023-06-26 22:45:08.000000 pydoda-1.0.3/pydoda/sentence.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)      367 2023-07-07 21:32:50.000000 pydoda-1.0.3/pydoda/utils.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.730969 pydoda-1.0.3/pydoda.egg-info/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     5809 2023-07-07 21:49:58.000000 pydoda-1.0.3/pydoda.egg-info/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2363 2023-07-07 21:49:58.000000 pydoda-1.0.3/pydoda.egg-info/SOURCES.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-07 21:49:58.000000 pydoda-1.0.3/pydoda.egg-info/dependency_links.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        7 2023-07-07 21:49:58.000000 pydoda-1.0.3/pydoda.egg-info/requires.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       13 2023-07-07 21:49:58.000000 pydoda-1.0.3/pydoda.egg-info/top_level.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-07 21:49:58.738968 pydoda-1.0.3/setup.cfg
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1412 2023-07-07 21:49:51.000000 pydoda-1.0.3/setup.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-07 21:49:58.738968 pydoda-1.0.3/tests/
+-rw-rw-r--   0 saad      (1000) saad      (1000)        0 2023-06-27 12:10:35.000000 pydoda-1.0.3/tests/__init__.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4646 2023-06-27 12:10:35.000000 pydoda-1.0.3/tests/test_category.py
+-rw-rw-r--   0 saad      (1000) saad      (1000)     2555 2023-06-27 12:10:35.000000 pydoda-1.0.3/tests/test_py_doda.py
```

### Comparing `pydoda-1.0.2/LICENSE` & `pydoda-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/PKG-INFO` & `pydoda-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoda
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper Python library for working with the DODa dataset
 Home-page: https://github.com/saad-out/pydoda
 Author: Saad Outchakoucht
 Author-email: outsaad03@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydoda-1.0.2/README.md` & `pydoda-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/__init__.py` & `pydoda-1.0.3/pydoda/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/category.py` & `pydoda-1.0.3/pydoda/category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/custom_category.py` & `pydoda-1.0.3/pydoda/custom_category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/dataset/LICENSE` & `pydoda-1.0.3/pydoda/dataset/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/dataset/README.md` & `pydoda-1.0.3/pydoda/dataset/README.md`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/dataset/imagenet_b_darija.csv` & `pydoda-1.0.3/pydoda/dataset/imagenet_b_darija.csv`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/dataset/sentences.csv` & `pydoda-1.0.3/pydoda/dataset/sentences.csv`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/loader.py` & `pydoda-1.0.3/pydoda/loader.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/py_doda.py` & `pydoda-1.0.3/pydoda/py_doda.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda/sentence.py` & `pydoda-1.0.3/pydoda/sentence.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/pydoda.egg-info/PKG-INFO` & `pydoda-1.0.3/pydoda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoda
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper Python library for working with the DODa dataset
 Home-page: https://github.com/saad-out/pydoda
 Author: Saad Outchakoucht
 Author-email: outsaad03@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydoda-1.0.2/setup.py` & `pydoda-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydoda",
-    version="1.0.2",
+    version="1.0.3",
     author="Saad Outchakoucht",
     author_email="outsaad03@gmail.com",
     description="A wrapper Python library for working with the DODa dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saad-out/pydoda",
     packages=setuptools.find_packages(),
@@ -26,10 +26,18 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     include_package_data=True,
-    package_data={"pydoda": ["dataset/**"]},
+    package_data={
+        "pydoda": [
+            "dataset/*",
+            "dataset/images/*",
+            "dataset/semantic categories/*",
+            "dataset/syntactic categories/*",
+            "dataset/x-tra/*",
+        ]
+    },
     python_requires=">=3.6",
 )
```

### Comparing `pydoda-1.0.2/tests/test_category.py` & `pydoda-1.0.3/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `pydoda-1.0.2/tests/test_py_doda.py` & `pydoda-1.0.3/tests/test_py_doda.py`

 * *Files identical despite different names*

