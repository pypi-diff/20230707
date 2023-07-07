# Comparing `tmp/sliceguard-0.0.4.tar.gz` & `tmp/sliceguard-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.4.tar", last modified: Fri Jul  7 08:13:34 2023, max compression
+gzip compressed data, was "sliceguard-0.0.5.tar", last modified: Fri Jul  7 08:35:45 2023, max compression
```

## Comparing `sliceguard-0.0.4.tar` & `sliceguard-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2844 2023-07-07 08:13:34.066984 sliceguard-0.0.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2188 2023-07-07 08:09:57.000000 sliceguard-0.0.4/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-07 08:11:41.000000 sliceguard-0.0.4/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 08:13:34.066984 sliceguard-0.0.4/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.4/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9222 2023-07-07 08:09:57.000000 sliceguard-0.0.4/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2844 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4644 2023-07-07 08:09:57.000000 sliceguard-0.0.4/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2907 2023-07-07 08:35:45.453053 sliceguard-0.0.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2251 2023-07-07 08:31:58.000000 sliceguard-0.0.5/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-07 08:33:44.000000 sliceguard-0.0.5/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 08:35:45.453053 sliceguard-0.0.5/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.5/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9222 2023-07-07 08:09:57.000000 sliceguard-0.0.5/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-05 08:28:25.000000 sliceguard-0.0.5/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2907 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-07 08:35:45.000000 sliceguard-0.0.5/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:35:45.453053 sliceguard-0.0.5/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4644 2023-07-07 08:09:57.000000 sliceguard-0.0.5/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.4/LICENSE` & `sliceguard-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/PKG-INFO` & `sliceguard-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,16 @@
 
 Install the jiwer package for computing the word error rate metric using `pip install jiwer`
 
 Get started by loading your first dataset and let sliceguard do its work:
 
 ```python
 import pandas as pd
+import numpy as np
+from jiwer import wer
 from sliceguard import SliceGuard
 
 # Load the example data
 df = pd.read_json("example_data.json")
 
 # Define a metric function to evaluate your model
 def wer_metric(y_true, y_pred):
@@ -52,14 +54,15 @@
 sg = SliceGuard()
 issue_df = sg.find_issues(
     df,
     ["age", "gender", "accent"],
     "sentence",
     "prediction",
     wer_metric,
+    metric_mode="min"
 )
 sg.report()
 ```
 
 For a more comprehensive tutorial check the following blog post on Medium:
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
```

### Comparing `sliceguard-0.0.4/README.md` & `sliceguard-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 Install the jiwer package for computing the word error rate metric using `pip install jiwer`
 
 Get started by loading your first dataset and let sliceguard do its work:
 
 ```python
 import pandas as pd
+import numpy as np
+from jiwer import wer
 from sliceguard import SliceGuard
 
 # Load the example data
 df = pd.read_json("example_data.json")
 
 # Define a metric function to evaluate your model
 def wer_metric(y_true, y_pred):
@@ -38,14 +40,15 @@
 sg = SliceGuard()
 issue_df = sg.find_issues(
     df,
     ["age", "gender", "accent"],
     "sentence",
     "prediction",
     wer_metric,
+    metric_mode="min"
 )
 sg.report()
 ```
 
 For a more comprehensive tutorial check the following blog post on Medium:
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
```

### Comparing `sliceguard-0.0.4/pyproject.toml` & `sliceguard-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sliceguard-0.0.4/sliceguard/detection.py` & `sliceguard-0.0.5/sliceguard/detection.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/sliceguard/embedding_utils.py` & `sliceguard-0.0.5/sliceguard/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/sliceguard/explanation.py` & `sliceguard-0.0.5/sliceguard/explanation.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/sliceguard/sliceguard.py` & `sliceguard-0.0.5/sliceguard/sliceguard.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/sliceguard/utils.py` & `sliceguard-0.0.5/sliceguard/utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.4/sliceguard.egg-info/PKG-INFO` & `sliceguard-0.0.5/sliceguard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,16 @@
 
 Install the jiwer package for computing the word error rate metric using `pip install jiwer`
 
 Get started by loading your first dataset and let sliceguard do its work:
 
 ```python
 import pandas as pd
+import numpy as np
+from jiwer import wer
 from sliceguard import SliceGuard
 
 # Load the example data
 df = pd.read_json("example_data.json")
 
 # Define a metric function to evaluate your model
 def wer_metric(y_true, y_pred):
@@ -52,14 +54,15 @@
 sg = SliceGuard()
 issue_df = sg.find_issues(
     df,
     ["age", "gender", "accent"],
     "sentence",
     "prediction",
     wer_metric,
+    metric_mode="min"
 )
 sg.report()
 ```
 
 For a more comprehensive tutorial check the following blog post on Medium:
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
```

### Comparing `sliceguard-0.0.4/tests/test_sliceguard.py` & `sliceguard-0.0.5/tests/test_sliceguard.py`

 * *Files identical despite different names*

