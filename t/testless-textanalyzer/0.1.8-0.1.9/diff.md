# Comparing `tmp/testless_textanalyzer-0.1.8.tar.gz` & `tmp/testless_textanalyzer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.8.tar", last modified: Wed Jul  5 00:00:35 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.9.tar", last modified: Fri Jul  7 17:34:07 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.8.tar` & `testless_textanalyzer-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-05 00:00:28.000000 testless_textanalyzer-0.1.8/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-05 00:00:35.000000 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      589 2023-07-05 00:00:35.000000 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-05 00:00:35.000000 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-05 00:00:35.000000 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-05 00:00:35.000000 testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.8/textanalyzer/__init__.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:35.815637 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:22.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/__init__.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     6030 2023-07-04 23:53:51.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/crf.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     7379 2023-07-04 23:49:28.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/crf_utils.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       93 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/exceptions.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/feature.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      857 2023-07-04 23:53:44.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/read_data.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2679 2023-07-04 23:48:29.000000 testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/text_analyzer.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-07 17:34:07.114349 testless_textanalyzer-0.1.9/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-07 17:34:07.114349 testless_textanalyzer-0.1.9/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-07 17:34:07.114349 testless_textanalyzer-0.1.9/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-07 17:32:20.000000 testless_textanalyzer-0.1.9/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-07 17:34:07.106350 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-07 17:34:06.000000 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      589 2023-07-07 17:34:06.000000 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-07 17:34:06.000000 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-07 17:34:06.000000 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-07 17:34:06.000000 testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-07 17:34:07.106350 testless_textanalyzer-0.1.9/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.9/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-07 17:34:07.110349 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-07-05 00:00:22.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/__init__.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     6007 2023-07-07 17:31:52.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/crf.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     7379 2023-07-04 23:49:28.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/crf_utils.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       93 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/exceptions.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/feature.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      857 2023-07-04 23:53:44.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/read_data.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2679 2023-07-04 23:48:29.000000 testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/text_analyzer.py
```

### Comparing `testless_textanalyzer-0.1.8/setup.py` & `testless_textanalyzer-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.8',
+  version='0.1.9',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
   long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
```

### Comparing `testless_textanalyzer-0.1.8/testless_textanalyzer.egg-info/SOURCES.txt` & `testless_textanalyzer-0.1.9/testless_textanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/crf.py` & `testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/crf.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             "params": list(self.params),
         }
         with open('Text_Analyzer/model/'+model_filename + '.pkl', 'wb') as f:
             pickle.dump(model, f)
         print(f'* Trained CRF Model has been saved at "{os.getcwd()}Text_Analyzer/model/{model_filename}"')
 
     def load(self, model_filename):
-        with open('Text_Analyzer/model/'+model_filename + '.pkl', 'rb') as f:
+        with open(model_filename + '.pkl', 'rb') as f:
             model = pickle.load(f)
 
         self.feature_set = FeatureSet()
         self.feature_set.load(model['feature_dic'], model['num_features'], model['labels'])
         self.label_dic, self.label_array = self.feature_set.get_labels()
         self.num_labels = len(self.label_array)
         self.params = np.asarray(model['params'])
```

### Comparing `testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/crf_utils.py` & `testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/crf_utils.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/feature.py` & `testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/feature.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/read_data.py` & `testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/read_data.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.8/textanalyzer/testless_textanalyzer/text_analyzer.py` & `testless_textanalyzer-0.1.9/textanalyzer/testless_textanalyzer/text_analyzer.py`

 * *Files identical despite different names*

