# Comparing `tmp/pydeequ-1.1.0.tar.gz` & `tmp/pydeequ-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeequ-1.1.0.tar", max compression
+gzip compressed data, was "pydeequ-1.1.0rc0.tar", max compression
```

## Comparing `pydeequ-1.1.0.tar` & `pydeequ-1.1.0rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-08 15:55:16.576797 pydeequ-1.1.0/LICENSE
--rw-r--r--   0        0        0     7928 2023-07-06 22:05:22.357018 pydeequ-1.1.0/README.md
--rw-r--r--   0        0        0     1595 2023-07-06 23:38:30.307835 pydeequ-1.1.0/pydeequ/__init__.py
--rw-r--r--   0        0        0    27271 2023-06-08 15:55:16.581835 pydeequ-1.1.0/pydeequ/analyzers.py
--rw-r--r--   0        0        0    10670 2023-06-08 15:55:16.581996 pydeequ-1.1.0/pydeequ/anomaly_detection.py
--rw-r--r--   0        0        0    41886 2023-06-19 16:30:42.591643 pydeequ-1.1.0/pydeequ/checks.py
--rw-r--r--   0        0        0     1434 2023-06-19 16:30:42.592148 pydeequ-1.1.0/pydeequ/configs.py
--rw-r--r--   0        0        0     2061 2023-06-08 15:55:16.582423 pydeequ-1.1.0/pydeequ/metrics.py
--rw-r--r--   0        0        0     2475 2023-06-08 15:55:16.582525 pydeequ-1.1.0/pydeequ/pandas_utils.py
--rw-r--r--   0        0        0    17640 2023-06-08 15:55:16.582681 pydeequ-1.1.0/pydeequ/profiles.py
--rw-r--r--   0        0        0     6704 2023-06-08 15:55:16.582819 pydeequ-1.1.0/pydeequ/repository.py
--rw-r--r--   0        0        0     3774 2023-06-08 15:55:16.582925 pydeequ-1.1.0/pydeequ/scala_utils.py
--rw-r--r--   0        0        0     8740 2023-06-08 15:55:16.583035 pydeequ-1.1.0/pydeequ/suggestions.py
--rw-r--r--   0        0        0    10216 2023-06-08 15:55:16.583154 pydeequ-1.1.0/pydeequ/verification.py
--rw-r--r--   0        0        0     2706 2023-07-06 23:38:30.308579 pydeequ-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9069 1970-01-01 00:00:00.000000 pydeequ-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 15:55:16.576797 pydeequ-1.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     7718 2023-06-08 15:55:16.576915 pydeequ-1.1.0rc0/README.md
+-rw-r--r--   0        0        0     1598 2023-06-19 16:36:21.702250 pydeequ-1.1.0rc0/pydeequ/__init__.py
+-rw-r--r--   0        0        0    27271 2023-06-08 15:55:16.581835 pydeequ-1.1.0rc0/pydeequ/analyzers.py
+-rw-r--r--   0        0        0    10670 2023-06-08 15:55:16.581996 pydeequ-1.1.0rc0/pydeequ/anomaly_detection.py
+-rw-r--r--   0        0        0    41886 2023-06-19 16:30:42.591643 pydeequ-1.1.0rc0/pydeequ/checks.py
+-rw-r--r--   0        0        0     1434 2023-06-19 16:30:42.592148 pydeequ-1.1.0rc0/pydeequ/configs.py
+-rw-r--r--   0        0        0     2061 2023-06-08 15:55:16.582423 pydeequ-1.1.0rc0/pydeequ/metrics.py
+-rw-r--r--   0        0        0     2475 2023-06-08 15:55:16.582525 pydeequ-1.1.0rc0/pydeequ/pandas_utils.py
+-rw-r--r--   0        0        0    17640 2023-06-08 15:55:16.582681 pydeequ-1.1.0rc0/pydeequ/profiles.py
+-rw-r--r--   0        0        0     6704 2023-06-08 15:55:16.582819 pydeequ-1.1.0rc0/pydeequ/repository.py
+-rw-r--r--   0        0        0     3774 2023-06-08 15:55:16.582925 pydeequ-1.1.0rc0/pydeequ/scala_utils.py
+-rw-r--r--   0        0        0     8740 2023-06-08 15:55:16.583035 pydeequ-1.1.0rc0/pydeequ/suggestions.py
+-rw-r--r--   0        0        0    10216 2023-06-08 15:55:16.583154 pydeequ-1.1.0rc0/pydeequ/verification.py
+-rw-r--r--   0        0        0     2709 2023-06-19 17:06:59.998275 pydeequ-1.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     8862 1970-01-01 00:00:00.000000 pydeequ-1.1.0rc0/PKG-INFO
```

### Comparing `pydeequ-1.1.0/LICENSE` & `pydeequ-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/README.md` & `pydeequ-1.1.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     - Perform data validation on a dataset with respect to various constraints set by you.   
 - Metrics Repository
     - Allows for persistence and tracking of Deequ runs over time.
 
 ![](imgs/pydeequ_architecture.jpg)
 
 ## 🎉 Announcements 🎉
-- **NEW!!!** As of 06/19, 1.1.0rc0 of Python Deequ is published https://github.com/awslabs/python-deequ/releases/tag/v1.1.0rc0. We will bake for around 2 weeks. Any feedbacks are welcome through github issues.
 - With PyDeequ v0.1.8+, we now officially support Spark3 ! Just make sure you have an environment variable `SPARK_VERSION` to specify your Spark version! 
 - We've release a blogpost on integrating PyDeequ onto AWS leveraging services such as AWS Glue, Athena, and SageMaker! Check it out: [Monitor data quality in your data lake using PyDeequ and AWS Glue](https://aws.amazon.com/blogs/big-data/monitor-data-quality-in-your-data-lake-using-pydeequ-and-aws-glue/).
 - Check out the [PyDeequ Release Announcement Blogpost](https://aws.amazon.com/blogs/big-data/testing-data-quality-at-scale-with-pydeequ/) with a tutorial walkthrough the Amazon Reviews dataset!
 - Join the PyDeequ community on [PyDeequ Slack](https://join.slack.com/t/pydeequ/shared_invite/zt-te6bntpu-yaqPy7bhiN8Lu0NxpZs47Q) to chat with the devs!
 
 ## Quickstart
```

### Comparing `pydeequ-1.1.0/pydeequ/__init__.py` & `pydeequ-1.1.0rc0/pydeequ/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 """Placeholder docstrings"""
-__version__ = "1.1.0"
+__version__ = "1.1.0rc0"
 
 from pyspark.sql import SparkSession
 
 from pydeequ.analyzers import AnalysisRunner
 from pydeequ.checks import Check, CheckLevel
 from pydeequ.configs import DEEQU_MAVEN_COORD
 from pydeequ.profiles import ColumnProfilerRunner
```

### Comparing `pydeequ-1.1.0/pydeequ/analyzers.py` & `pydeequ-1.1.0rc0/pydeequ/analyzers.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/anomaly_detection.py` & `pydeequ-1.1.0rc0/pydeequ/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/checks.py` & `pydeequ-1.1.0rc0/pydeequ/checks.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/configs.py` & `pydeequ-1.1.0rc0/pydeequ/configs.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/metrics.py` & `pydeequ-1.1.0rc0/pydeequ/metrics.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/pandas_utils.py` & `pydeequ-1.1.0rc0/pydeequ/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/profiles.py` & `pydeequ-1.1.0rc0/pydeequ/profiles.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/repository.py` & `pydeequ-1.1.0rc0/pydeequ/repository.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/scala_utils.py` & `pydeequ-1.1.0rc0/pydeequ/scala_utils.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/suggestions.py` & `pydeequ-1.1.0rc0/pydeequ/suggestions.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pydeequ/verification.py` & `pydeequ-1.1.0rc0/pydeequ/verification.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.1.0/pyproject.toml` & `pydeequ-1.1.0rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeequ"
-version = "1.1.0"
+version = "1.1.0rc0"
 description = "PyDeequ - Unit Tests for Data"
 authors = ["Calvin Wang <calviwan@amazon.com>"]
 maintainers = ["Calvin Wang <calviwan@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://pydeequ.readthedocs.io"
 repository = "https://github.com/awslabs/python-deequ"
```

### Comparing `pydeequ-1.1.0/PKG-INFO` & `pydeequ-1.1.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeequ
-Version: 1.1.0
+Version: 1.1.0rc0
 Summary: PyDeequ - Unit Tests for Data
 Home-page: https://pydeequ.readthedocs.io
 License: Apache-2.0
 Keywords: deequ,pydeequ,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers
 Author: Calvin Wang
 Author-email: calviwan@amazon.com
 Maintainer: Calvin Wang
@@ -42,15 +42,14 @@
     - Perform data validation on a dataset with respect to various constraints set by you.   
 - Metrics Repository
     - Allows for persistence and tracking of Deequ runs over time.
 
 ![](imgs/pydeequ_architecture.jpg)
 
 ## 🎉 Announcements 🎉
-- **NEW!!!** As of 06/19, 1.1.0rc0 of Python Deequ is published https://github.com/awslabs/python-deequ/releases/tag/v1.1.0rc0. We will bake for around 2 weeks. Any feedbacks are welcome through github issues.
 - With PyDeequ v0.1.8+, we now officially support Spark3 ! Just make sure you have an environment variable `SPARK_VERSION` to specify your Spark version! 
 - We've release a blogpost on integrating PyDeequ onto AWS leveraging services such as AWS Glue, Athena, and SageMaker! Check it out: [Monitor data quality in your data lake using PyDeequ and AWS Glue](https://aws.amazon.com/blogs/big-data/monitor-data-quality-in-your-data-lake-using-pydeequ-and-aws-glue/).
 - Check out the [PyDeequ Release Announcement Blogpost](https://aws.amazon.com/blogs/big-data/testing-data-quality-at-scale-with-pydeequ/) with a tutorial walkthrough the Amazon Reviews dataset!
 - Join the PyDeequ community on [PyDeequ Slack](https://join.slack.com/t/pydeequ/shared_invite/zt-te6bntpu-yaqPy7bhiN8Lu0NxpZs47Q) to chat with the devs!
 
 ## Quickstart
```

