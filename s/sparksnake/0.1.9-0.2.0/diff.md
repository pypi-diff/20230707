# Comparing `tmp/sparksnake-0.1.9.tar.gz` & `tmp/sparksnake-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparksnake-0.1.9.tar", last modified: Mon Mar 27 02:19:15 2023, max compression
+gzip compressed data, was "sparksnake-0.2.0.tar", last modified: Fri Jul  7 15:19:18 2023, max compression
```

## Comparing `sparksnake-0.1.9.tar` & `sparksnake-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.406170 sparksnake-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-27 02:19:03.000000 sparksnake-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-27 02:19:15.402170 sparksnake-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-27 02:19:03.000000 sparksnake-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 02:19:15.406170 sparksnake-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-27 02:19:03.000000 sparksnake-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.398170 sparksnake-0.1.9/sparksnake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25976 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/sparksnake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/sparksnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/test_glue_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/test_manager_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 15:19:05.000000 sparksnake-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-07 15:19:18.933099 sparksnake-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-07 15:19:05.000000 sparksnake-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:19:18.933099 sparksnake-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 15:19:06.000000 sparksnake-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/tester/dataframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/sparksnake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/helpers/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_glue_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_manager_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_tester_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_utils_log.py
```

### Comparing `sparksnake-0.1.9/LICENSE` & `sparksnake-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksnake-0.1.9/PKG-INFO` & `sparksnake-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.1.9
+Version: 0.2.0
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
@@ -28,54 +28,50 @@
 
 <div align="center">  
   <br>
   
   [![PyPI](https://img.shields.io/pypi/v/sparksnake?color=purple)](https://pypi.org/project/sparksnake/)
   ![PyPI - Downloads](https://img.shields.io/pypi/dm/sparksnake?color=purple)
   ![PyPI - Status](https://img.shields.io/pypi/status/sparksnake?color=purple)
-  ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ThiagoPanini/sparksnake?color=purple)
-  ![GitHub Last Commit](https://img.shields.io/github/last-commit/ThiagoPanini/sparksnake?color=purple)
   <br>
 
   ![CI workflow](https://img.shields.io/github/actions/workflow/status/ThiagoPanini/sparksnake/ci-main.yml?label=ci)
   [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/en/latest/?badge=latest)
   [![codecov](https://codecov.io/gh/ThiagoPanini/sparksnake/branch/main/graph/badge.svg?token=zSdFO9jkD8)](https://codecov.io/gh/ThiagoPanini/sparksnake)
 
 </div>
 
 ## Table of content
 
 - [Table of content](#table-of-content)
 - [What is the sparksnake library?](#what-is-the-sparksnake-library)
 - [Features](#features)
-- [Contacts](#contacts)
+- [Contact me](#contact-me)
 - [References](#references)
 
 
 ## What is the sparksnake library?
 
-The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications along all the particularities found in AWS services, such as Glue and EMR, for example.
-
-Do you want to take your job Glue or your EMR cluster to the next level? Take a look at *sparksnake*!
+The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications anywhere!
 
 > **Note**
->  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, practical examples and more!
+>  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, hands on demos and more!
 
 
 ## Features
 
-- 🤖 Enhanced development experience of Spark Applications to be deployed as jobs in AWS services like Glue and EMR
-- 🌟 Possibility to use common Spark operations for improving ETL steps using custom classes and methods
-- ⚙️ No need to think too much into the hard and complex service setup (e.g. with *sparksnake* you can have all elements for a Glue Job on AWS with a single line of code)
-- 👁️‍🗨️ Application observability improvement with detailed log messages in CloudWatch
-- 🛠️ Exception handling already embedded in library methods
+- 🤖 Apply common Spark operations using few lines of code
+- 💻 Start developing your Spark applications anywhere using the "default" mode or in any AWS services that uses Spark
+- ⏳ Stop spending time setting up the boring stuff of your Spark applications
+- 💡 Apply the best practices on your application by structuring your code following the best practices
+- 👁️‍🗨️ Improve your aplication's observability by using detailed log messages on CloudWatch and exception handlers
 
 ___
 
-## Contacts
+## Contact me
 
 - [Thiago Panini - LinkedIn](https://www.linkedin.com/in/thiago-panini/)
 - [paninitechlab @ hashnode](https://panini.hashnode.dev/)
 
 ___
 
 ## References
```

### Comparing `sparksnake-0.1.9/README.md` & `sparksnake-0.2.0/sparksnake.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,77 @@
+Metadata-Version: 2.1
+Name: sparksnake
+Version: 0.2.0
+Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
+Home-page: https://github.com/ThiagoPanini/sparksnake
+Author: Thiago Panini
+Author-email: panini.development@gmail.com
+License: MIT
+Keywords: Cloud,AWS,Python,Spark,pyspark
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: Portuguese (Brazilian)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.0.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <br><img src="https://github.com/ThiagoPanini/snakespark/blob/main/docs/assets/imgs/header-readme.png?raw=true" alt="snakespark-logo">
 </div>
 
 <div align="center">  
   <br>
   
   [![PyPI](https://img.shields.io/pypi/v/sparksnake?color=purple)](https://pypi.org/project/sparksnake/)
   ![PyPI - Downloads](https://img.shields.io/pypi/dm/sparksnake?color=purple)
   ![PyPI - Status](https://img.shields.io/pypi/status/sparksnake?color=purple)
-  ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ThiagoPanini/sparksnake?color=purple)
-  ![GitHub Last Commit](https://img.shields.io/github/last-commit/ThiagoPanini/sparksnake?color=purple)
   <br>
 
   ![CI workflow](https://img.shields.io/github/actions/workflow/status/ThiagoPanini/sparksnake/ci-main.yml?label=ci)
   [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/en/latest/?badge=latest)
   [![codecov](https://codecov.io/gh/ThiagoPanini/sparksnake/branch/main/graph/badge.svg?token=zSdFO9jkD8)](https://codecov.io/gh/ThiagoPanini/sparksnake)
 
 </div>
 
 ## Table of content
 
 - [Table of content](#table-of-content)
 - [What is the sparksnake library?](#what-is-the-sparksnake-library)
 - [Features](#features)
-- [Contacts](#contacts)
+- [Contact me](#contact-me)
 - [References](#references)
 
 
 ## What is the sparksnake library?
 
-The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications along all the particularities found in AWS services, such as Glue and EMR, for example.
-
-Do you want to take your job Glue or your EMR cluster to the next level? Take a look at *sparksnake*!
+The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications anywhere!
 
 > **Note**
->  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, practical examples and more!
+>  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, hands on demos and more!
 
 
 ## Features
 
-- 🤖 Enhanced development experience of Spark Applications to be deployed as jobs in AWS services like Glue and EMR
-- 🌟 Possibility to use common Spark operations for improving ETL steps using custom classes and methods
-- ⚙️ No need to think too much into the hard and complex service setup (e.g. with *sparksnake* you can have all elements for a Glue Job on AWS with a single line of code)
-- 👁️‍🗨️ Application observability improvement with detailed log messages in CloudWatch
-- 🛠️ Exception handling already embedded in library methods
+- 🤖 Apply common Spark operations using few lines of code
+- 💻 Start developing your Spark applications anywhere using the "default" mode or in any AWS services that uses Spark
+- ⏳ Stop spending time setting up the boring stuff of your Spark applications
+- 💡 Apply the best practices on your application by structuring your code following the best practices
+- 👁️‍🗨️ Improve your aplication's observability by using detailed log messages on CloudWatch and exception handlers
 
 ___
 
-## Contacts
+## Contact me
 
 - [Thiago Panini - LinkedIn](https://www.linkedin.com/in/thiago-panini/)
 - [paninitechlab @ hashnode](https://panini.hashnode.dev/)
 
 ___
 
 ## References
@@ -77,8 +97,8 @@
 
 **Tests**
 
 - [Codecov - Setting Threshold](https://github.com/codecov/codecov-action/issues/554#issuecomment-1261250304)
 - [Codecov - About the Codecov YAML](https://docs.codecov.com/docs/codecov-yaml)
 - [Codecov - Status Checks](https://docs.codecov.com/docs/commit-status)
 - [Codecov - codecov.yml Reference](https://docs.codecov.com/docs/codecovyml-reference)
-- [Codecov - Ignore Paths](https://docs.codecov.com/docs/ignoring-paths)
+- [Codecov - Ignore Paths](https://docs.codecov.com/docs/ignoring-paths)
```

### Comparing `sparksnake-0.1.9/setup.py` & `sparksnake-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 # Reading README.md for project description
 with open("README.md", "r", encoding='utf-8') as f:
     __long_description__ = f.read()
 
 # Setting up package information
 setup(
     name='sparksnake',
-    version='0.1.9',
+    version='0.2.0',
     author='Thiago Panini',
     author_email='panini.development@gmail.com',
     packages=find_packages(),
     install_requires=[
-        "pyspark"
+        "pyspark",
+        "Faker"
     ],
     license='MIT',
     description="Improving the development of Spark applications deployed as "
                 "jobs on AWS services like Glue and EMR",
     long_description=__long_description__,
     long_description_content_type="text/markdown",
     url='https://github.com/ThiagoPanini/sparksnake',
```

### Comparing `sparksnake-0.1.9/sparksnake/glue.py` & `sparksnake-0.2.0/sparksnake/glue.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,23 +21,28 @@
 
 
 # Setting up a logger object
 logger = log_config(logger_name=__file__)
 
 
 class GlueJobManager():
-    """Management of elements and operations commonly used in Glue jobs.
+    """Enables users to use AWS Glue features in their Spark applications.
 
-    This class is responsible for managing and providing all necessary inputs
-    for launching and developing Glue jobs in AWS. All attributes and methods
-    declared in this class are *inherited* by `SparkETLManager`class in the
-    `manager` module.
-
-    To see a end to end usage example, check the docs for the `SparkETLManager`
-    class.
+    This class provides an enhanced experience on developing Glue jobs using
+    Apache Spark. The core idea behind it is related complex code encapsulation
+    that is mandatory to build and run Glue jobs. By that, it's possible to
+    say that this `GlueJobManager` class has attributes and methods that uses
+    the `awsglue` library to handle almost everything that would be handled
+    individually by users if they are not using sparksnake.
+
+    By the end, it's important to mention that all attributes and methods of
+    this class are inherited by `SparkETLManager` class in the `manager` module
+    when users initialize it with `mode="glue"`. So, when doing that, users
+    need to pass some additional arguments in order to make things work
+    properly in the Glue specific world.
 
     Args:
         argv_list (list):
             List with all user defined arguments for the job
 
         data_dict (dict):
             Dictionary with all source data references to be read from the
@@ -58,69 +63,109 @@
             A Glue context object used for creating a Spark session object
 
         spark (SparkSession):
             A Spark session object used as a central point for job operations
 
     Tip: About setting up the data_dict class attribute
         The data_dict dictionary passed as a required attribute for the
-        `GlueJobManager` class must be defined following some rules.
+        `GlueJobManager` class must be defined following some rules. Then main
+        purpose of such attribute is to provide a single variable to handle
+        all data sources to be read by the Glue job application.
+
+        With that in mind, it's important to say that the data_dict attribute
+        can be defined using everything that is available and acceptable in
+        the Glue DynamicFrameReader class. Users can take a look at the AWS
+        official docs about the DynamicFrameReader class to see more details
+        about reading DynamicFrame objects in Glue jobs.
+
+        On this class scope, the data_dict dictionary can also have additional
+        keys that can used to guide reading proccesses and apply some special
+        conditions. The additional keys that can be put on data_dict class
+        attribute are:
+
+        - "source_method": str -> Defines if users want to read data
+        from catalog ('from_catalog') or from other options ('from_options').
+        Under the hood, the 'source_method' dictionary key defines which method
+        will be used along the `glueContext.create_dynamic_frame` method.
+        The default value is 'from_catalog'.
+
+        - "create_temp_view": bool -> Sets the creation of a Spark temporary
+        table (view) after reading the data source as a DynamicFrame. If this
+        additional key is set as True, then the `DataFrame.createTempView()`
+        method is executed in order to create temporary tables using the
+        table name as the main reference for the temp view.
+
+        By the end, an example on how to define the data_dict class attribute
+        dictionary can be find right below:
+
+        ```python
+        # Defining elements of all data sources used on the job
+        ```python
+        {
+            "orders": {
+                "database": "ra8",
+                "table_name": "orders",
+                "transformation_ctx": "dyf_orders"
+            },
+            "customers": {
+                "database": "ra8",
+                "table_name": "customers",
+                "transformation_ctx": "dyf_customers",
+                "push_down_predicate": "anomesdia=20221201",
+                "create_temp_view": True,
+                "additional_options": {
+                    "compressionType": "lzo"
+                }
+            },
+            "payments": {
+                "source_method": "from_options",
+                "connection_type": "s3",
+                "connection_options": {
+                    "paths": [
+                        "s3://some-bucket-name/some-prefix/file.csv"
+                    ],
+                    "recurse": True
+                },
+                "format": "csv",
+                "format_options": {
+                    "withHeader": True,
+                    "separator": ",",
+                    "quoteChar": '"'
+                },
+                "transformation_ctx": "dyf_payments"
+            }
+        }
+        ```
 
-        Your main purpose is to provide a single point for controlling all
-        data sources used in the job. So, your composition is something really
-        important for ensuring that reading process can be executed in an
-        expected way.
-
-        With that in mind, it's crucial to say that the data_dict dictionary
-        can be defined with all parameters found in
-        `glueContext.create_dynamic_frame.from_catalog` Glue method. In other
-        words, all keys of data_dict dictionary can be assume any valid
-        parameter of the Glue method mentioned above. Of course the values
-        of those keys defined in data_dict depends on the job rules.
-
-        :star: It means that if the user wants to read a data source from the
-        catalog using the push down predicate Glue feature, it's only necessary
-        to define a key called "push_down_predicate" (the same way as found in
-        `glueContext.create_dynamic_frame.from_catalog` method) with the value
-        to be filtered. This is the same rule for all other parameters, such as
-        additional_options, catalog_id, transformation_ctx, and others. If the
-        user wants to read some data source with a special parameter, just take
-        a look at the mentioned Glue method above and input a key on the
-        data_dict to set up the data source reading process.
-
-        By the other hand, it's also important to mention that the user is not
-        forced to define the data_dict dictionary with all parameters found in
-        `glueContext.create_dynamic_frame.from_catalog` method. If the
-        data_dict attribute doesn't have a key for a specific parameter on the
-        Glue method mentioned abouve, so its default value will be considered.
-        For example, that if data_dict doesn't have a push_down_predicate key
-        for a data source, the value "None" will be considered as it's the
-        default value for this key on the
-        `glueContext.create_dynamic_frame.from_catalog` method.
+        As you can see, the DATA_DICT variable defined in the example above
+        uses mixed data sources, each one with special configurations
+        accepted by the DynamicFrameReader Glue methods. But don't worry,
+        you will find more examples along this documentation page.
     """
 
     def __init__(self, argv_list: list, data_dict: dict) -> None:
         self.argv_list = argv_list
         self.data_dict = data_dict
 
         # Getting job arguments
         self.args = getResolvedOptions(sys.argv, self.argv_list)
 
     def job_initial_log_message(self) -> None:
-        """Preparation of a detailed log message for job initialization.
+        """Preparing a detailed log message for job start up.
 
         This method is responsible for composing an initial log message to be
-        shown in CloudWatch after the user initializes a Glue Job. The message
-        aim to clarify some job details, such as all the data sources mapped
-        and its push down predicate values (if used). This can be a good
-        practice for making Glue jobs cleaner and more organized.
+        logged in CloudWatch after the user starts a Glue Job. The message aims
+        to clarify some job details, such as the data sources mapped and its
+        push down predicate values (if used). This can be a good practice in
+        order to develop more organized Glue jobs.
         """
 
         # Defining a initial string for composing the message
-        welcome_msg = f"Initializing the execution of {self.args['JOB_NAME']}"\
-                      " job. Data sources used in this ETL process:\n\n"
+        welcome_msg = f"Successfully started Glue job {self.args['JOB_NAME']}"\
+                      ". Data sources in this ETL process:\n\n"
         initial_msg = ""
 
         # Iterating over the data_dict dicionary for extracting some info
         for _, params in self.data_dict.items():
             # Getting table name and start building the message
             tbl_ref = f"{params['database']}.{params['table_name']}"
             table_msg = f"Table {tbl_ref} "
@@ -160,15 +205,15 @@
         """
         logger.info("Creating SparkContext, GlueContext and SparkSession")
         self.sc = SparkContext.getOrCreate()
         self.glueContext = GlueContext(self.sc)
         self.spark = self.glueContext.spark_session
 
     def init_job(self):
-        """Initializing a Glue job.
+        """Starting a Glue job.
 
         This method consolidates all the necessary steps required for a Glue
         job initialization process. In its definition, it calls the following
         methods:
 
         * `self.job_initial_log_message()`
         * `self.print_args()`
@@ -237,19 +282,25 @@
                     "additional_options": {
                         "compressionType": "lzo"
                     }
                 }
             }
             ```
 
-            As stated before, all
-            `glueContext.create_dynamic_frame.from_catalog()` can be used as
-            dictionary keys on `self.data_dict` definition. Moreover, some
-            additional keys can be defined by the user for some special
-            purposes, such as:
+            As stated before, all elements on Glue DynamicFrameReader class
+            methods can be used as dictionary keys on `self.data_dict`
+            definition. Moreover, some additional keys can be defined by the
+            user for some special purposes, such as:
+
+            - "source_method": str -> Defines if users want to read data
+            from catalog ('from_catalog') or from other options
+            ('from_options'). Under the hood, the 'source_method' dictionary
+            key defines which method will be used along the
+            `glueContext.create_dynamic_frame` method. The default value is
+            'from_catalog'.
 
             - "create_temp_view": bool -> Sets the creation of a Spark
                 temporary table (view) after reading the data source as a
                 DynamicFrame
 
             The return of the method `generate_dynamicframes_dict()` will be
             presented as the following format:
@@ -261,65 +312,123 @@
             }
             ```
 
             where the tags <DynamicFrame> means objects of DynamicFrame type
             read for each data source.
         """
 
-        logger.info("Iterating over data_dict dictionary for reading data "
-                    "sources as Glue DynamicFrame objects")
+        logger.info("Reading all data sources as Glue DynamicFrame objects")
         try:
             dynamic_frames = []
             for t in self.data_dict.keys():
-                # Getting some required args: database, table_name, ctx
-                database = self.data_dict[t]["database"]
-                table_name = self.data_dict[t]["table_name"]
-                transformation_ctx = self.data_dict[t]["transformation_ctx"]
-
-                # Getting non required args: push_down_predicate
-                push_down_predicate = self.data_dict[t]["push_down_predicate"]\
-                    if "push_down_predicate" in self.data_dict[t].keys()\
-                    else ""
-
-                # Getting non required args: additional_options
-                additional_options = self.data_dict[t]["additional_options"] \
-                    if "additional_options" in self.data_dict[t].keys()\
-                    else {}
-
-                # Getting non required args: catalog_id
-                catalog_id = self.data_dict[t]["catalog_id"] \
-                    if "catalog_id" in self.data_dict[t].keys()\
-                    else None
-
-                # Reading the DynamicFrame
-                dyf = self.glueContext.create_dynamic_frame.from_catalog(
-                    database=database,
-                    table_name=table_name,
-                    transformation_ctx=transformation_ctx,
-                    push_down_predicate=push_down_predicate,
-                    additional_options=additional_options,
-                    catalog_id=catalog_id
-                )
+                # Defining the source method to be called to read the dyf
+                source_method = self.data_dict[t]["source"].lower().strip() \
+                    if "source" in self.data_dict[t].keys()\
+                    else "from_catalog"
+
+                # Entering a condition where the data is read from catalog
+                if source_method == "from_catalog":
+                    # Getting some required args: database and table_name
+                    database = self.data_dict[t]["database"]
+                    table_name = self.data_dict[t]["table_name"]
+
+                    # Getting non required args: redshift_tmp_dir
+                    redshift_tmp_dir = self.data_dict[t]["redshift_tmp_dir"]\
+                        if "redshift_tmp_dir" in self.data_dict[t].keys()\
+                        else ""
+
+                    # Getting non required args: transformation_ctx
+                    transformation_ctx = \
+                        self.data_dict[t]["transformation_ctx"]\
+                        if "transformation_ctx" in self.data_dict[t].keys()\
+                        else ""
+
+                    # Getting non required args: push_down_predicate
+                    push_down_predicate = \
+                        self.data_dict[t]["push_down_predicate"]\
+                        if "push_down_predicate" in self.data_dict[t].keys()\
+                        else ""
+
+                    # Getting non required args: additional_options
+                    additional_options = \
+                        self.data_dict[t]["additional_options"] \
+                        if "additional_options" in self.data_dict[t].keys()\
+                        else {}
+
+                    # Getting non required args: catalog_id
+                    catalog_id = self.data_dict[t]["catalog_id"] \
+                        if "catalog_id" in self.data_dict[t].keys()\
+                        else None
+
+                    # Reads a DynamicFrame from catalog
+                    dyf = self.glueContext.create_dynamic_frame.from_catalog(
+                        database=database,
+                        table_name=table_name,
+                        redshift_tmp_dir=redshift_tmp_dir,
+                        transformation_ctx=transformation_ctx,
+                        push_down_predicate=push_down_predicate,
+                        additional_options=additional_options,
+                        catalog_id=catalog_id
+                    )
+
+                # Entering a condition where the data is read from other option
+                elif source_method == "from_options":
+                    # Getting some required args: connection_type
+                    connection_type = self.data_dict[t]["connection_type"]
+
+                    # Getting non required args: connection_options
+                    conn_options = self.data_dict[t]["connection_options"] \
+                        if "connection_options" in self.data_dict[t].keys()\
+                        else {}
+
+                    # Getting non required args: catalog_id
+                    format = self.data_dict[t]["format"] \
+                        if "format" in self.data_dict[t].keys()\
+                        else None
+
+                    # Getting non required args: format_options
+                    format_options = self.data_dict[t]["format_options"] \
+                        if "format_options" in self.data_dict[t].keys()\
+                        else {}
+
+                    # Reads a DynamicFrame from options
+                    dyf = self.glueContext.create_dynamic_frame.from_options(
+                        connection_type=connection_type,
+                        connection_options=conn_options,
+                        format=format,
+                        format_options=format_options,
+                        transformation_ctx=transformation_ctx
+                    )
+
+                else:
+                    # Raising an error if source_method is not expected
+                    raise TypeError("Invalid value for 'source_method' in "
+                                    f"DATA_DICT dictionary ({source_method}). "
+                                    "Acceptable values are 'from_catalog' or "
+                                    "'from_options'.")
 
                 # Appending the DynamicFrame obnject to DynamicFrames list
                 dynamic_frames.append(dyf)
 
         except Exception as e:
-            logger.error("Error on generating a list of DynamicFrames list. "
-                         f"Exception: {e}")
+            logger.error("Failed to read data sources mapped on DATA_DICT "
+                         f"dictionary as Glue DynamicFrames. Exception: {e}")
             raise e
 
-        logger.info("Mapping DynamicFrames objects to a dictionary key")
-        sleep(0.01)
-
         # Creating a DynamicFrames dictionary
-        dynamic_dict = {k: dyf for k, dyf
-                        in zip(self.data_dict.keys(), dynamic_frames)}
-        logger.info("Success on reading data. There are "
-                    f"{len(dynamic_dict.values())} DynamicFrames available.")
+        dynamic_dict = {
+            k: dyf for k, dyf in zip(self.data_dict.keys(), dynamic_frames)
+        }
+
+        # Preparing a final message with all data sources read
+        print_dict = {k: type(v) for k, v in dynamic_dict.items()}
+        logger.info("Sucessfully read all data sources. There are "
+                    f"{len(dynamic_dict.values())} DynamicFrames available "
+                    "in a Python dictionary presented as following: \n"
+                    f"{print_dict}")
 
         # Returning the dictionary
         sleep(0.01)
         return dynamic_dict
 
     def generate_dataframes_dict(self) -> dict:
         """Getting a dictionary of DataFrames objects read from the catalog.
@@ -404,20 +513,28 @@
         # Getting a DynamicFrame objects dictionary
         dyf_dict = self.generate_dynamicframes_dict()
 
         # Transforming DynamicFrames into DataFrames
         logger.info(f"Transforming {len(dyf_dict.keys())} "
                     "Glue DynamicFrames into Spark DataFrames")
         try:
+            # Transforming objects and mapping the result into a python dict
             df_dict = {k: dyf.toDF() for k, dyf in dyf_dict.items()}
-            logger.info("Success on generating all Spark DataFrames")
+
+            # Preparing a log message
+            print_dict = {k: type(v) for k, v in df_dict.items()}
+            logger.info("Sucessfully generated Spark DataFrames from Glue "
+                        "DynamicFrames previously read. There are "
+                        f"{len(df_dict.values())} Spark DataFrames available "
+                        "in a Python dictionary presented as following: "
+                        f"{print_dict}")
             sleep(0.01)
 
         except Exception as e:
-            logger.error("Error on transforming Glue DataFrames into Spark "
+            logger.error("Failed to transform Glue DynamicFrames into Spark "
                          f"DataFrames. Exception: {e}")
             raise e
 
         # Creating spark temporary tables if applicable
         for table_key, params in self.data_dict.items():
             try:
                 # Extracting useful variables from the dict
@@ -425,20 +542,20 @@
                 table_name = params["table_name"]
 
                 # Creating temp tables (if the flag for it was set as True)
                 if "create_temp_view" in params\
                         and bool(params["create_temp_view"]):
                     df.createOrReplaceTempView(table_name)
 
-                    logger.info(f"Spark temporary table (view) {table_name} "
-                                "was successfully created.")
+                    logger.info("Successfully created a Spark temporary table "
+                                f"(view) named {table_name}")
 
             except Exception as e:
-                logger.error("Error on creating Spark temporary table "
-                             f"{table_name}. Exception: {e}")
+                logger.error("Failed to create a Spark temporary table for "
+                             f"data source {table_name}. Exception: {e}")
                 raise e
 
         # Returning the DataFrames dict
         sleep(0.01)
         return df_dict
 
     def drop_partition(self, s3_partition_uri: str,
@@ -466,33 +583,33 @@
             retention_period (int): Hours to data retention
 
         Raises:
             Exception: Generic exception raises when a failed attempt of
             executing the `glueContext.purge_s3_path()` method.
         """
 
-        logger.info(f"Searching for the partition {s3_partition_uri} and "
+        logger.info(f"Searching for partition {s3_partition_uri} and "
                     "dropping it (if exists)")
         try:
             self.glueContext.purge_s3_path(
                 s3_path=s3_partition_uri,
                 options={"retentionPeriod": retention_period}
             )
         except Exception as e:
-            logger.error(f"Error on purging partition {s3_partition_uri}. "
+            logger.error(f"Failed to purge partition {s3_partition_uri}. "
                          f"Exception: {e}")
             raise e
 
     def write_and_catalog_data(
             self,
             df: DataFrame or DynamicFrame,
             s3_table_uri: str,
             output_database_name: str,
             output_table_name: str,
-            partition_name: str = None,
+            partition_name: str or list = None,
             connection_type: str = "s3",
             update_behavior: str = "UPDATE_IN_DATABASE",
             compression: str = "snappy",
             enable_update_catalog: bool = True,
             output_data_format: str = "parquet"
     ) -> None:
         """Writing data on S3 anda cataloging on Data Catalog.
@@ -507,15 +624,15 @@
         2. Make a sink with data catalog
         3. Write data in S3 and update the data catalog with the behavior
         chosen by the user
 
         Examples:
             ```python
             # Writing and cataloging data
-            spark_manager.write_data(
+            spark_manager.write_and_catalog_data(
                 df=df_orders,
                 s3_table_uri="s3://some-bucket/some-table",
                 output_database_name="db_corp_business_inteligence",
                 output_table_name="tbl_orders_prep",
                 partition_name="anomesdia"
             )
             ```
@@ -539,18 +656,19 @@
                 from `glueContext.getSink().setCatalogInfo()` method.
 
             output_table_name (str):
                 Reference for the table used on the catalog process. This
                 information is used on parameter "catalogTableName"
                 from `glueContext.getSink().setCatalogInfo()` method.
 
-            partition_name (str or None):
+            partition_name (str or list or None):
                 Partition coumn name chosen for the table. This information is
                 used on parameter "partitionKeys" from `glueContext.getSink()`
-                method.
+                method. In case of partitioning by multiple columns, users can
+                pass a list with partition names.
 
             connection_type (str):
                 Connection type used in storage. This information is used on
                 parameter "connection_type" from `glueContext.getSink()` method
 
             update_behavior (str):
                 Defines the update behavior for the target table. This
@@ -575,50 +693,60 @@
 
         # Converting DataFrame into DynamicFrame
         if type(df) == DataFrame:
             logger.info("Converting the Spark DataFrame as Glue DynamicFrame")
             try:
                 dyf = DynamicFrame.fromDF(df, self.glueContext, "dyf")
             except Exception as e:
-                logger.error("Error on converting the DataFrame object as "
-                             f"DynamicFrame. Exception: {e}")
+                logger.error("Failed to transform the Spark DataFrame object "
+                             f"in a Glue DynamicFrame object. Exception: {e}")
                 raise e
         else:
             dyf = df
 
+        # Handling partition information
+        if isinstance(partition_name, str):
+            partition_keys = [partition_name]
+        elif isinstance(partition_name, list):
+            partition_keys = partition_name
+        else:
+            raise ValueError("Invalid type for argument partition_name. "
+                             "Acceptable values are str or list")
+
         # Creating a sink with S3
         logger.info("Creating a sink with all configurations provided")
         try:
             # Criando relação de escrita de dados
             data_sink = self.glueContext.getSink(
                 path=s3_table_uri,
                 connection_type=connection_type,
                 updateBehavior=update_behavior,
-                partitionKeys=[partition_name],
+                partitionKeys=partition_keys,
                 compression=compression,
                 enableUpdateCatalog=enable_update_catalog,
                 transformation_ctx="data_sink",
             )
         except Exception as e:
-            logger.error("Error on creating a sink for the output table. "
+            logger.error("Failed to create a sink for the output table. "
                          f"Exception: {e}")
             raise e
 
         # Setting up data catalog info
         logger.info("Setting up information on the Data Catalog for the table")
         try:
             data_sink.setCatalogInfo(
                 catalogDatabase=output_database_name,
                 catalogTableName=output_table_name
             )
             data_sink.setFormat(output_data_format,
                                 useGlueParquetWriter=True)
             data_sink.writeFrame(dyf)
 
-            logger.info(f"Table {output_database_name}."
-                        f"{output_table_name} "
-                        "successfully update on Data Catalog. Its data are "
-                        f"stored in the following path: {s3_table_uri}")
+            logger.info(f"Successfully updated table {output_database_name}"
+                        f".{output_table_name} in Glue Data Catalog. The "
+                        "table data are stored in the following S3 path: "
+                        f"{s3_table_uri}")
         except Exception as e:
-            logger.error("Error on trying to write data for the given table "
-                         f". Exception: {e}")
+            logger.error("Failed to write and catalog data for table  "
+                         f"{output_database_name}.{output_table_name}. "
+                         f"Exception: {e}")
             raise e
```

### Comparing `sparksnake-0.1.9/sparksnake/manager.py` & `sparksnake-0.2.0/sparksnake/manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,46 +9,81 @@
 # Importing libraries
 from time import sleep
 
 from sparksnake.utils.log import log_config
 
 from pyspark.sql import SparkSession, DataFrame
 from pyspark.sql.functions import expr, lit
+from pyspark.sql.utils import AnalysisException
 
+# Trying to inherit features from GlueJobManager class
 try:
     from sparksnake.glue import GlueJobManager as ManagerClass
 except ImportError:
+    # Providing an empty class with a common alias name in case of ImportError
     class ManagerClass:
         pass
 
+
 # Setting up a logger object
 logger = log_config(logger_name=__file__)
 
 
 class SparkETLManager(ManagerClass):
-    """Puts together all Spark features used in ETL jobs in AWS.
+    """Puts together all Spark features provided by sparksnake library.
+
+    This class provides an easy and fast way for users to improve and enhance
+    the development of their Apache Spark applications. This class can be
+    considered a central point of contact for users who whant to use all
+    features (attributes and methods) provided by sparksnake whenever the
+    Spark application is running locally or in any supported AWS services
+    such as AWS Glue.
+
+    To configure this class and start using all its features, users just need
+    to set up an "operation mode" represented by the "mode" class attribute.
+    The operation mode can be chosen based on where the Spark application will
+    run. Currently there are two available options:
+
+    - `mode="default"` enables features do enhance the development of Spark
+        applications anywhere
+    - `mode="glue"` enables features to enhance the development of Spark
+        applications deployed as Glue jobs in AWS. In this case, a class
+        inheritance process is applied in order to enable users to use
+        `awsglue` modules in a Glue environment.
+
+    Example: "Setting up the operation mode within `SparkETLManager` class"
+        ```python
+        # Importing the class
+        from sparksnake.manager import SparkETLManager
 
-    This class provides an easy and fast way for users to improve and
-    enhance the development of their Spark applications. The class makes it
-    possible through a series of features (attributes and methods) specially
-    coded for making the development journey something really simple and fun.
-
-    According to the AWS service to be used by the user to run their Spark
-    application, this class can be configured through its "mode" attribute.
-    Technically, it means that the "mode" attribute literally handles all
-    class inheritance processes based on target AWS service to be used.
-
-    So, users can have available special attributes and methods for improving
-    their development process wherever they are creating a Spark application
-    for running on AWS Glue, Amazon EMR or even locally.
+        # Creating a spark manager object to develop Spark apps anywhere
+        spark_manager = SparkETLManager(
+            mode="default"
+        )
+
+        # Creating a spark manager object to develop Spark apps on AWS Glue
+        spark_manager = SparkETLManager(
+            mode="glue",
+            argv_list=[]  # A list of Glue job arguments
+            data_dict={}  # A dictionary with all data sources for the job
+        )
+        ```
+
+    A special note about the sparksnake's operation mode takes place on
+    different behaviors the deployment environment demands in order to work
+    properly. In other words, when choosing "glue" as the operation mode while
+    creating a `SparkETLManager` object, users need to check what additional
+    attributes must be passed to the class so the Glue custom features can
+    available to be applied in their Spark application.
 
     Example: A basic usage example of class `SparkETLManager` with mode="glue"
         ```python
-        # Importing class
+        # Importing packages
         from sparksnake.manager import SparkETLManager
+        from datetime import datetime
 
         # Defining job arguments
         ARGV_LIST = ["JOB_NAME", "S3_OUTPUT_PATH"]
 
         # Defining dictionary of data sources to be used on job
         DATA_DICT = {
             "orders": {
@@ -87,139 +122,155 @@
         spark_manager.drop_partition(
             s3_partition_uri="s3://some-bucket-name/some-table-name/partition/"
         )
 
         # Adding a partition column into the DataFrame
         df_orders_partitioned = spark_manager.add_partition_column(
             partition_name="anomesdia",
-            partition_value="20230101"
+            partition_value=int(datetime.now().strftime("%Y%m%d"))
         )
 
         # Applying a repartition method for storage optimization
         df_orders_repartitioned = spark_manager.repartition_dataframe(
             df=df_orders_partitioned,
             num_partitions=10
         )
 
         # Writing data on S3 and cataloging it on Data Catalog
-        spark_manager.write_data_to_catalog(df=df_orders_repartitioned)
+        spark_manager.write_and_catalog_data(df=df_orders_repartitioned)
 
         # Job commit
         spark_manager.job.commit()
         ```
 
     Args:
         mode (string):
             Operation mode for the class. It handles inheritance from other
             classes based on this library so the `SparkETLManager` class can
             expand its features for a Spark application development in
             specific scenarios.
-            Acceptable values are: "glue", "emr", "local".
+            Acceptable values are: "default", "glue".
 
-    Tip: The "mode" attribute may not be the only one
-        By its own construction, the class `SparkETLManager`inherits attributes
-        and methods from other classes in the library. It means that these
-        other classes may have its own attributes to be passed on class
-        construction.
-
-        For example, when users choose to set the Glue operation mode
-        (`mode="glue"`) on starting up the class `SparkETLManager`, a class
-        inheritance from `GlueJobManager` is set under the hood. Because of
-        that, attributes like `argv_list` and `data_dict` must be passed
-        together with `mode` as they are mandatory on `GlueJobManager` class
-        construction.
-
-        For a special tip, check the construction of the class to be inherited
-        based on mode operation to see which attributes are necessary to pass
-        at `SparkETLManager` class start up.
+    Tip: The "mode" attribute may not be the only one.
+        As stated before, the `SparkETLManager` class provides a "mode"
+        attribute that can be used to set special class configuration
+        according to where users pretend to develop their Spark applications.
+        Technically, it happens by class inheritance.
+
+        In other words, when users set `mode="glue"` in order to develop their
+        Spark applications as Glue jobs on AWS, all Glue features that is
+        needed to provide such environment is inherited by another class inside
+        the sparksnake library. This class is the `GlueJobManager` and its
+        source code is available on the `glue.py` library module.
+
+        By saying that the "mode" attribute may not be the only one, it is said
+        that those class inheritance processes may demands the input of some
+        other attributes. For example, to initialize an object from the
+        `GlueJobManager` class, users need to pass two more attributes named
+        `argv_list` and `data_dict`, each one with their special purposes. So,
+        in this situation, anyone who needs to use sparksnake in the Glue ops
+        mode may pass those two mode class attributes in the `SparkETLManager`
+        class.
+
+        To be awared of which additional attributes is needed to start the
+        `SparkETLManager` class in any available mode, you can always check the
+        source code of the class to be inherited. The table below provides
+        information about all operation modes and the inherited classes:
+
+        | Operation Mode | Inherited Class |
+        | :-- | :-- |
+        | default | None |
+        | glue | GlueJobManager |
     """
 
     def __init__(self, mode: str, **kwargs) -> None:
+        # Cleaning up the mode string attribute to apply validations
         self.mode = mode.strip().lower()
 
-        # Checking if the operation mode value was passed as expected
-        if self.mode not in ("local", "glue", "emr"):
-            raise ValueError(f"The attribute mode was set as {self.mode} "
-                             "but acceptable values are 'local', 'glue' and "
-                             'emr')
-
-        # Looking out for glue operation mode
+        # Glue operation mode: applying validations and obtaining Glue features
         if self.mode == "glue":
             # Checking if required args for GlueJobManager were passed
             if "argv_list" not in kwargs or "data_dict" not in kwargs:
                 raise TypeError("The operation mode was set as 'glue' but "
                                 "'argv_list' and/or 'data_dict' required "
-                                "arguments weren't set properly. Please pass "
-                                "those arguments at class initialization.")
+                                "attributes weren't set properly. Please "
+                                "provide both attributes during class "
+                                "start up in order to use sparksnake with "
+                                "glue operation mode.")
 
             # Collecting required args for mode="glue"
             argv_list = kwargs["argv_list"]
             data_dict = kwargs["data_dict"]
 
             # Applying class inheritance for this mode
             try:
                 ManagerClass.__init__(self, argv_list=argv_list,
                                       data_dict=data_dict)
             except TypeError:
                 raise TypeError("Error on inherting class GlueJobManager. "
                                 "Check if your environment has the awsglue "
                                 "libraries and try again. If you don't have "
                                 "awsglue libs available, you probably want to "
-                                "run sparksnake in a local operation mode. If "
-                                "this is the case, change the mode attribute "
-                                "to 'local'")
+                                "run sparksnake in a default operation mode. "
+                                "If this is the case, change the mode "
+                                "attribute to 'default'")
 
             # Logging initialization message
-            logger.info("The class was succesfully initialized with Glue "
-                        "operation mode and all Glue sparksnake features were "
-                        "inherited and are now available")
-
-        # Looking out for local mode
-        elif self.mode == "local":
-            # Checking if user wants to pass its own SparkSession object
-            if "spark" in kwargs and type(kwargs["spark"]) is SparkSession:
-                self.spark = kwargs["spark"]
-            else:
-                logger.info("Creating a SparkSession object to be used in a "
-                            "local environment")
-                self.spark = SparkSession.builder\
-                    .appName("sparksnake-app")\
-                    .getOrCreate()
+            logger.info("Sucessfully initialized sparksnake with Glue "
+                        "operation mode. You know have some special AWS Glue "
+                        "features to improve your Glue job.")
+
+        # Default operation mode:
+        elif self.mode == "default":
+            # Getting or creating a SparkSession object as a class attribute
+            logger.info("Creating a SparkSession object (or getting one if it "
+                        "already exists)")
+            self.spark = SparkSession.builder.getOrCreate()
 
             # Logging initialization message
-            logger.info("The class was succesfully initialized with 'local' "
-                        "operation mode")
+            logger.info("Successfully initialized sparksnake with default "
+                        "operation mode. You can know use the sparksnake "
+                        "features to improve your Spark application.")
+
+        # None of acceptable operation modes
+        else:
+            raise ValueError(f"Invalid value for operation mode (mode={mode})."
+                             "Acceptable values are 'default' and 'glue'.")
 
     @staticmethod
-    def date_transform(df: DataFrame,
-                       date_col: str,
-                       date_col_type: str = "date",
-                       date_format: str = "yyyy-MM-dd",
-                       convert_string_to_date: bool = True,
-                       **kwargs) -> DataFrame:
+    def date_transform(
+        df: DataFrame,
+        date_col: str,
+        date_col_type: str = "date",
+        date_format: str = "yyyy-MM-dd",
+        cast_string_to_date: bool = True,
+        **kwargs
+    ) -> DataFrame:
         """Extracting date attributes from a Spark DataFrame date column.
 
         This method makes it possible to extract multiple date attributes from
-        a column in a Spark DataFrame that represents a date or timestamp
-        information. To do that, the given date column in the DataFrame should
-        be of types DATE, TIMESTAMP. There is a special case where the target
-        date column is of STRING data type. In that situtation, the column
-        must be parseable as a date so the date attributes can be extracted
-        from it.
-
-        The method logic is made for a initial field casting validation
-        followed by the extraction of all date attributes according to the user
-        input on the method call. The big idea behing this features is the
-        ability to provide users a huge DataFrame enrichment with a single
-        method call to improve their analytics processes.
+        a Spark DataFrame column that represents a date or timestamp value.
+        The date attributes are extracted using all available Apache Spark date
+        functions such as year(), month(), dayofmonth() and many others that
+        can be found on the official pyspark documentation page.
+
+        So, the given date column (date_col argument) should has a DATE or
+        a TIMESTAMP data type. If this can be achieved, the date column should
+        then be a string that can be parseable to a date type object. This is
+        the condition to extract date attributes using pyspark date functions.
+
+        The main idea behind this method is to provide users an easy way to
+        enhance their data analysis by extracting multiple date attributes
+        from a date column. This can be a huge improvement on analytics
+        processes and DataFrames enrichment.
 
         Examples:
             ```python
             # Extracting date attributes from a date column in a Spark df
-            df_date_prep = spark_manager.extract_date_attributes(
+            df_date_prep = spark_manager.date_transform(
                 df=df_raw,
                 date_col="order_date",
                 date_col_type="timestamp",
                 year=True,
                 month=True,
                 dayofmonth=True
             )
@@ -239,17 +290,17 @@
 
             date_col_type (str):
                 Reference for data type of `date_col` argument. Acceptable
                 values are "date" or "timestamp".
 
             date_format (str):
                 Date format applied in a optional string to date casting.
-                It's applicable only if `convert_string_to_date=True`
+                It's applicable only if `cast_string_to_date=True`
 
-            convert_string_to_date (bool):
+            cast_string_to_date (bool):
                 Enables an automatic casting of the `date_col` column reference
                 into a given `date_format`.
 
         Keyword Args:
             year (bool): Extracts the year of target date column
             quarter (bool): Extracts the quarter of target date column
             month (bool): Extracts the month of target date column
@@ -265,103 +316,116 @@
         Returns:
             Spark DataFrame with new date columns extracted.
         """
 
         try:
             # Creating casting expressions based on data type of date_col arg
             date_col_type = date_col_type.strip().lower()
-            if convert_string_to_date:
+            if cast_string_to_date:
                 if date_col_type == "date":
-                    conversion_expr = f"to_date({date_col},\
+                    casting_expr = f"to_date({date_col},\
                         '{date_format}') AS {date_col}_{date_col_type}"
                 elif date_col_type == "timestamp":
-                    conversion_expr = f"to_timestamp({date_col},\
+                    casting_expr = f"to_timestamp({date_col},\
                         '{date_format}') AS {date_col}_{date_col_type}"
                 else:
-                    raise ValueError("The data type of date_col_type parameter"
-                                     " is invalid. Acceptable values are "
-                                     "'date'or 'timestamp'")
+                    raise ValueError("Invalid data type of date_col_type "
+                                     "argument. Acceptable values are 'date' "
+                                     "or 'timestamp'")
 
                 # Applying a select expression for casting data if applicable
                 df = df.selectExpr(
                     "*",
-                    conversion_expr
+                    casting_expr
                 ).drop(date_col)\
                     .withColumnRenamed(f"{date_col}_{date_col_type}", date_col)
 
-        except Exception as e:
-            logger.error(f"Error on casting the column {date_col} as "
-                         f"{date_col_type} using the expression "
-                         f"{conversion_expr}. Exception: {e}")
-            raise e
+        except ValueError as ve:
+            logger.error(ve)
+            raise ve
+
+        except AnalysisException as ae:
+            logger.error("Analysis error on trying to cast the column "
+                         f"{date_col} using the expression {casting_expr}. "
+                         "Maybe this column doesn't exist on the DataFrame. "
+                         f"Check the error traceback for more details: {ae}")
+            raise ae
 
         # Creating a list of all possible date attributes to be extracted
         possible_date_attribs = ["year", "quarter", "month", "dayofmonth",
                                  "dayofweek", "dayofyear", "weekofyear"]
 
-        try:
-            # Looping over all possible attributes and extracting date attribs
-            for attrib in possible_date_attribs:
-                # Add a new column only if attrib is in kwargs
-                if attrib in kwargs and bool(kwargs[attrib]):
-                    df = df.withColumn(
-                        f"{attrib}_{date_col}",
-                        expr(f"{attrib}({date_col})")
-                    )
-
-            return df
+        # Iterating over all possible attributes and extracting date attribs
+        for attrib in possible_date_attribs:
+            # Add a new column only if attrib is in kwargs
+            if attrib in kwargs and bool(kwargs[attrib]):
+                df = df.withColumn(
+                    f"{attrib}_{date_col}", expr(f"{attrib}({date_col})")
+                )
 
-        except Exception as e:
-            logger.error("Error on adding new date columns into the "
-                         f"DataFrame. Exception: {e}")
-            raise e
+        return df
 
     @staticmethod
-    def aggregate_data(df: DataFrame,
-                       spark_session: SparkSession,
-                       numeric_col: str,
-                       group_by: str or list,
-                       round_result: bool = False,
-                       n_round: int = 2,
-                       **kwargs) -> DataFrame:
-        """Extracts statistical attributes based on a group by opreation.
-
-        This method makes it possible to extract multiple statistical
-        aggregations based in a numerical column and a set of columns to be
-        grouped by. With this feature, users can configure complex aggregations
-        in a single method call in order to enhance their analysis.
+    def agg_data(
+        spark_session: SparkSession,
+        df: DataFrame,
+        agg_col: str,
+        group_by: str or list,
+        round_result: bool = False,
+        n_round: int = 2,
+        **kwargs
+    ) -> DataFrame:
+        """Extracting statistical attributes based on a group by operation.
+
+        This method makes it possible to run complex aggregations using a
+        single method call. To use this feature, users can follow the steps
+        below:
+
+        1. Provide a aggregation column (agg_col argument)
+        2. Provide a single column reference or a list of columns to be
+        grouped by (group_by argument)
+        3. Provide the aggregation functions on **kwargs
+
+        The aggregation functions mentioned on the third step are represented
+        by almost any avaiable pyspark function, such as `sum()`, `mean()`,
+        `max()`, `min()` and many others.
 
         Examples:
             ```python
             # Creating a new special and aggregated DataFrame
-            df_stats = spark_manager.extract_aggregate_statistics(
+            df_stats = spark_manager.agg_data(
+                spark_session=spark,
                 df=df_orders,
-                numeric_col="order_value",
+                agg_col="order_value",
                 group_by=["order_id", "order_year"],
                 sum=True,
                 mean=True,
                 max=True,
                 min=True
             )
 
-            # In the above example, the method will return a new DataFrame with
+            # In the example above, the method will return a new DataFrame with
             # the following columns:
             # order_id e order_year (group by)
             # sum_order_value (sum of order_value column)
             # mean_order_value (average of order_value column)
             # max_order_value (max value of order_value column)
             # min_order_value (min value of order_value column)
             ```
 
         Args:
+            spark_session (pyspark.sql.SparkSession):
+                A SparkSession object to be used to run SparkSQL query for
+                grouping data
+
             df (pyspark.sql.DataFrame):
                 A target Spark DataFrame for applying the transformation
 
-            numeric_col (str):
-                A numeric column name on the target DataFrame to be used as
+            agg_col (str):
+                A column reference on the target DataFrame to be used as
                 target of aggregation process
 
             group_by (str or list):
                 A column name or a list of columns used as group categories
                 on the aggregation process
 
             round_result (bool):
@@ -412,27 +476,26 @@
         if type(group_by) == list and len(group_by) > 1:
             group_by = ",".join(group_by)
 
         # Creating a Spark temporary table for grouping data using SparkSQL
         df.createOrReplaceTempView("tmp_extract_aggregate_statistics")
 
         possible_functions = ["sum", "mean", "max", "min", "count",
-                              "countDistinct", "variance", "stddev",
-                              "kurtosis", "skewness"]
+                              "variance", "stddev", "kurtosis", "skewness"]
         try:
-            # Looping over the attributes to build a single aggregation expr
+            # Iterating over the attributes to build a single aggregation expr
             agg_query = ""
             for f in possible_functions:
                 if f in kwargs and bool(kwargs[f]):
                     if round_result:
-                        agg_function = f"round({f}({numeric_col}), {n_round})"
+                        agg_function = f"round({f}({agg_col}), {n_round})"
                     else:
-                        agg_function = f"{f}({numeric_col})"
+                        agg_function = f"{f}({agg_col})"
 
-                    agg_query += f"{agg_function} AS {f}_{numeric_col},"
+                    agg_query += f"{agg_function} AS {f}_{agg_col},"
 
             # Dropping the last comma on the expression
             agg_query = agg_query[:-1]
 
             # Building the final query to be executed
             final_query = f"""
                 SELECT
@@ -441,36 +504,45 @@
                 FROM tmp_extract_aggregate_statistics
                 GROUP BY
                     {group_by}
             """
 
             return spark_session.sql(final_query)
 
-        except Exception as e:
-            logger.error("Error on extracting statistical attributes from "
-                         f"DataFrame. Exception: {e}")
-            raise e
+        except AnalysisException as ae:
+            logger.error("Error on trying to aggregate data from DataFrame "
+                         f"using the following query:\n {final_query}. "
+                         "Possible reasons are: missing to pass group_by "
+                         "parameter or the agg_col argument doesn't exists"
+                         f" on the DataFrame. Exception: {ae}")
+            raise ae
 
     @staticmethod
-    def add_partition_column(df: DataFrame,
-                             partition_name: str,
-                             partition_value) -> DataFrame:
+    def add_partition_column(
+        df: DataFrame,
+        partition_name: str,
+        partition_value
+    ) -> DataFrame:
         """Adding a "partition" column on a Spark DataFrame.
 
         This method is responsible for adding a new column on a target Spark
         DataFrame to be considered as a table partition. In essence, this
         method uses the native pyspark `.withColumn()` method for adding a
-        new column to the DataFrame using a name for the partition column
-        (partition_name) and its value (partition_value).
+        new column to the DataFrame using a name (partition_name) and a value
+        (partition_value).
+
+        The idea behind this method is to provide users a more clear way to
+        add a partition column in their Spark DataFrames and make it very
+        explicity to whoever is reading the code.
 
         Examples
             ```python
             # Defining partition information
             partition_name = "anomesdia"
-            partition_value = int(datetime.strftime('%Y%m%d'))
+            partition_value = int(datetime.now().strftime('%Y%m%d'))
 
             # Adding a partition column to the DataFrame
             df_partitioned = spark_manager.add_partition_column(
                 df=df_orders,
                 partition_name=partition_name,
                 partition_value=partition_value
             )
@@ -495,21 +567,23 @@
 
         logger.info("Adding a new partition column to the DataFrame "
                     f"({partition_name}={str(partition_value)})")
         try:
             df_partitioned = df.withColumn(partition_name,
                                            lit(partition_value))
             return df_partitioned
+
         except Exception as e:
             logger.error("Error on adding a partition colum to the DataFrame "
                          f"using the .withColumn() method. Exception: {e}")
+            raise e
 
     @staticmethod
     def repartition_dataframe(df: DataFrame, num_partitions: int) -> DataFrame:
-        """Repartitioning a Spark DataFrame for optimizing storage.
+        """Repartitioning a Spark DataFrame in order to optimize storage.
 
         This method applies the repartition process in a Spark DataFrame in
         order to optimize its storage on S3. The method has some important
         checks based on each pyspark method to use for repartitioning the
         DataFrame. Take a look at the below tip to learn more.
 
         Tip: Additional details on method behavior
@@ -532,15 +606,15 @@
                 df=df_orders,
                 num_partitions=10
             )
             ```
 
         Args:
             df (pyspark.sql.DataFrame): A target Spark Dataframe.
-            num_partitions (int): Desider number of partitions.
+            num_partitions (int): Desired number of partitions.
 
         Returns:
             A new Spark DataFrame gotten after the repartition process.
 
         Raises:
             Exception: A generic exception is raised on a failed attempt to\
             run the repartition method (`coalesce()` or `repartition()`) in\
@@ -552,23 +626,23 @@
 
         # Getting the current number of partitions of the given DataFrame
         logger.info("Getting the current number of partition of the DataFrame")
         try:
             current_partitions = df.rdd.getNumPartitions()
 
         except Exception as e:
-            logger.error("Error on collecting the current number of "
-                         "using df.rdd.getNumPartitions method. "
+            logger.error("Failed to collect the current number of partitions"
+                         "using the df.rdd.getNumPartitions method. "
                          f"Exception: {e}")
             raise e
 
         # If the desired partition number if equal to the current number, skip
         if num_partitions == current_partitions:
             logger.warning(f"The current number of partitions "
-                           f"({current_partitions}) is equal to the desired "
+                           f"({current_partitions}) is equal to the target "
                            f"number ({num_partitions}). There is no need to "
                            "run any Spark repartition method")
             sleep(0.01)
             return df
 
         # If the desired number if LESS THAN the current, use coalesce()
         elif num_partitions < current_partitions:
@@ -576,34 +650,237 @@
                         f"coalesce(), changing the number of DataFrame "
                         f"partitions from {current_partitions} to "
                         f"{num_partitions}")
             try:
                 df_repartitioned = df.coalesce(num_partitions)
 
             except Exception as e:
-                logger.warning("Error on repartitioning using coalesce(). "
+                logger.warning("Failed to repartition using coalesce(). "
                                "The repartition process won't be executed and "
                                "the target DataFrame will be returned without "
                                f"any changes. Exception: {e}")
                 return df
 
         # If the desired number is GREATER THAN the current, use repartition()
         elif num_partitions > current_partitions:
-            logger.warning(f"The desired partition number ({num_partitions}) "
+            logger.warning(f"The target partition number ({num_partitions}) "
                            f"is greater than the current one "
                            f"({current_partitions}) and, because of that, "
                            "the repartitioning operation will be executed "
                            "using the repartition() method which can be "
                            "expensive under the application perspective. As a "
                            "suggestion, check if this is really the expected "
                            "behavior for this operation.")
             try:
                 df_repartitioned = df.repartition(num_partitions)
 
             except Exception as e:
-                logger.warning("Error on repartitioning using repartition(). "
+                logger.warning("Failed to repartition using repartition(). "
                                "The repartition process won't be executed and "
                                "the target DataFrame will be returned without "
                                f"any changes. Exception: {e}")
                 return df
 
         return df_repartitioned
+
+    @staticmethod
+    def run_spark_sql_pipeline(
+        spark_session: SparkSession,
+        spark_sql_pipeline: list
+    ) -> DataFrame:
+        """Providing a way to run multiple SparkSQL queries in sequence.
+
+        This method allows users to define a sequence of SparkSQL queries to
+        built transformation DAGs in order to transform DataFrames in a Spark
+        application using only SQL. The core idea behind this method is that
+        users can define a sequence of SparkSQL statements using a predefined
+        list of dictionaries (`spark_sql_pipeline` argument) that will be
+        handled by the method as the main piece for sequentially running
+        the queries and providing the desired result as a Spark DataFrame.
+
+        As said before, everything around this method takes place
+        `spark_sql_pipeline` argument definition. In essence, this argument
+        can be defined as a list with multiple dictionaries, where each
+        inner dictionary in this list can have elements that describe the
+        execution of a SparkSQL query (including the query itself).
+
+        Examples:
+        ```python
+        # Defining a list with all SparkSQL steps to be executed
+        spark_sql_pipeline = [
+            {
+                "step": 1,
+                "query": '''
+                    SELECT
+                        order_id,
+                        order_status,
+                        order_purchase_ts
+
+                    FROM tbl_orders
+                '''
+                "create_temp_view": True,
+                "temp_view_name": "auto"
+            },
+            {
+                "step": 2,
+                "query": '''
+                    SELECT
+                        order_id,
+                        sum(payment_value) AS sum_payment_value
+
+                    FROM tbl_payments
+
+                    GROUP BY order_id
+                '''
+                "create_temp_view": True,
+                "temp_view_name": "auto"
+            },
+            {
+                "step": 3,
+                "query": '''
+                    SELECT
+                        step_1.order_id,
+                        step_1.order_status,
+                        step_1.order_purchase_ts,
+                        step_2.sum_payment_value
+
+                    FROM step_1
+
+                    LEFT JOIN step_2
+                        ON step_1.order_id = step_2.order_id
+                '''
+                "create_temp_view": True,
+                "temp_view_name": "auto"
+            }
+        ]
+
+        # Running the SparkSQL pipeline
+        df_prep = run_spark_sql_pipeline(
+            spark_session=spark_manager.spark,
+            spark_sql_pipeline=spark_sql_pipeline
+        )
+        ```
+
+        Tip: About the spark_sql_pipeline definition
+            As stated before, the `spark_sql_pipeline` method argument can be
+            defined as a Python list where each element is a Python dictionary
+            with all information needed to run SparkSQL statements in sequence.
+
+            First of all, it's important to say that the inner dictionaries
+            must be defined with some acceptable keys:
+
+            - `"step"` (required): defines an integer number to inform the
+                method in which order the query in the given dictionary should
+                be executed. The value passed on the "step" inner dictionary
+                key is used in a sorting proccess that defines the execution
+                order of the SparkSQL statements.
+
+            - `"query"` (required): well, this is the SparkSQL query itself
+                that will be executed by the method. This could be defines as a
+                Python string directly on the dictionary or even by reading
+                some external JSON or SQL file in the project directory.
+
+            - `"create_temp_view"` (optional, default=True): defines a boolean
+                flag that handles the creation of a new temporary view for
+                each executed step. By the default, it's set as True, meaning
+                that after each execution, a new temporary view will be
+                available for further SparkSQL statements.
+
+            - `"temp_view_name"` (optional, default="auto"): defines the name
+                of the temporary view created after executing the SparkSQL
+                query in a given step. It's applicable only if
+                "create_temp_view" is True for the step. By default, it's value
+                is set as "auto", meaning that the name of the intermediate
+                temporary view will be set as "step_N", where N is the integer
+                that defines the step. For example, in the first inner
+                dictionary of the `spark_sql_pipeline` list (for instance,
+                "step": 1), a query will be executed and, if there is no an
+                explicit "create_temp_view": False in the dictionary, then a
+                new temporary view with query result will be created and named
+                as "step_1". So, any further SparkSQL statements that selects
+                data from any "step_1" table will be pointing to the
+                intermediate results of the first step of the pipeline. By the
+                other hand, users can define a specific name for the step
+                temporary view by filling this key with any desired string.
+
+            If users don't explicit define the keys "create_temp_view" and
+            "temp_view_name", the method will consider its default values. In
+            other words, if the a inner dictionary of the `spark_sql_pipeline`
+            list doesn't have any of the mentioned keys, it means that a
+            temporary view will be created after running the step's query and
+            it will be named as "step_N", where N is the integer that identify
+            the step.
+
+        Args:
+            spark_session (pyspark.sql.SparkSession):
+                A SparkSession object to be used to run SparkSQL query for
+                grouping data
+
+            spark_sql_pipeline (list):
+                A list made by dictionaries that defines details of the steps
+                to be executed using SparkSQL queries. Check the tip above for
+                more details on how passing this argument
+
+        Returns:
+            A Spark DataFrame that is the result of the execution of the last\
+            step (query) defined in the spark_sql_pipeline list.
+
+        Raises:
+            ValueError: An exception raises in two different situations:\
+            first, if the user defines any dictionary in `spark_sql_pipeline`\
+            list doesn't have the required keys ("step" and "query"). Second,\
+            if any dictionary in the `spark_sql_pipeline` list has any value\
+            for the "step" key that isn't an integer. Those validations are\
+            important to ensure that users are correctly defining the\
+            arguments for the method .
+        """
+
+        # Applying some validations on the sql pipeline argument
+        required_keys = ["step", "query"]
+
+        # Getting a list with keys of all inner dicts from sql pipeline list
+        inner_pipe_keys = [list(pipe.keys()) for pipe in spark_sql_pipeline]
+
+        # Checking if the required arguments are in all inner dict keys
+        for inner_key in inner_pipe_keys:
+            if not all(key in inner_key for key in required_keys):
+                raise ValueError("The sql_pipeline argument doesn't have the "
+                                 "required keys for all its elements. Check "
+                                 "if all inner dictionaries on the "
+                                 "spark_sql_pipeline list have at least the "
+                                 "'step' and the 'query' keys")
+
+        # Checking if all step keys are integers
+        step_types_validation = list(set(
+            [isinstance(pipe["step"], int) for pipe in spark_sql_pipeline]
+        ))[0]
+        if not step_types_validation:
+            raise ValueError("The steps in the sql_pipeline argument must be "
+                             "integers. Check if all the 'step' keys in the "
+                             "inner dictionaries are integers.")
+
+        # Going to the method: sorting the steps in an ascending order
+        sorted_spark_sql_pipeline = sorted(
+            spark_sql_pipeline,
+            key=lambda x: x["step"]
+        )
+
+        # Iterating over the pipeline elements to execute the statements
+        for pipe in sorted_spark_sql_pipeline:
+            # Executing the queries in sequence
+            df_step = spark_session.sql(pipe["query"])
+
+            # Creating a temporary view with the step result (if applicable)
+            if "create_temp_view" not in pipe\
+                    or bool(pipe["create_temp_view"]):
+                # Assigning a name for result temporary view
+                if "temp_view_name" not in pipe\
+                        or pipe["temp_view_name"].strip().lower() == "auto":
+                    temp_view_name = "step_" + str(pipe["step"])
+                else:
+                    temp_view_name = pipe["temp_view_name"]
+
+                # Creating the temporary view
+                df_step.createOrReplaceTempView(temp_view_name)
+
+        # Returning the DataFrame from the last step
+        return df_step
```

### Comparing `sparksnake-0.1.9/tests/test_glue_module.py` & `sparksnake-0.2.0/tests/test_glue_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,213 @@
-"""Test cases for GlueJobManager class features.
+"""Test cases for features defined on glue.py module.
 
 This file handles the definition of all test cases for testing GlueJobManager
 class and its features. The idea is to isolate a test script for testing
 sparksnake features delivered for users who want to develop Spark applications
-using AWS Glue service.
+using AWS Glue environment through a SparkETLManager class object with
+mode="glue".
 
 ___
 """
 
 # Importing libraries
 import pytest
 import logging
 
-from tests.helpers.user_inputs import FAKE_ARGV_LIST
+from sparksnake.manager import SparkETLManager
 
 from pyspark.context import SparkContext
 from pyspark.sql import SparkSession
 
 from awsglue.context import GlueContext
 from awsglue.job import Job
 
+from tests.helpers.user_inputs import EXPECTED_START_JOB_MSG
 
-@pytest.mark.glue_job_manager
-def test_type_of_args_class_attribute_is_dictionary(
-    job_manager
+
+@pytest.mark.spark_manager_glue
+@pytest.mark.constructor
+def test_error_on_using_glue_mode_and_not_providing_essential_attributes():
+    """
+    G: Given that an user wants to initialize a Glue job on AWS
+    W: When the class SparkETLManager is initialized with mode="glue" but
+       without argv_list or data_dict attributes on object construction
+    T: Then a TypeError exception must be raised
+    """
+
+    # Trying to initialize SparkETLManager with glue mode and without argv_list
+    with pytest.raises(TypeError):
+        _ = SparkETLManager(mode="glue")
+
+
+@pytest.mark.spark_manager_glue
+@pytest.mark.constructor
+def test_args_attribute_for_class_on_glue_mode_must_be_dict(
+    spark_manager_glue
 ):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when the class GlueJobManager is called to create an object
-    T: then args attribute created must be of dict type
+    G: Given that an user wants to initialize a Glue job on AWS
+    W: When an object of class SparkETLManager is initialized with
+       mode="glue"
+    T: Then the self.args class attribute must be a Python dictionary
     """
 
-    assert type(job_manager.args) is dict
+    assert type(spark_manager_glue.args) is dict
 
 
-@pytest.mark.glue_job_manager
-def test_args_class_attribute_has_user_defined_arguments(
-    job_manager
+@pytest.mark.spark_manager_glue
+@pytest.mark.constructor
+def test_args_attribute_contains_user_defined_arguments(
+    spark_manager_glue
 ):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when the class GlueJobManager is called to create an object
-    T: then the arguments previous defined by user on argv_list must be into
-       self.args dictionary attribute
+    G: Given that a user wants to initialize a Glue job on AWS
+    W: When the class SparkETLManager is initialized with mode="glue"
+    T: Then the arguments passed on argv_list parameter must be contained on
+       self.args class attribute
     """
 
     # Getting argument job names
-    job_arg_names = list(job_manager.args.keys())
+    job_arg_names = list(spark_manager_glue.args.keys())
 
-    assert all(a in job_arg_names for a in FAKE_ARGV_LIST)
+    assert all(a in job_arg_names for a in spark_manager_glue.argv_list)
 
 
-@pytest.mark.glue_job_manager
-@pytest.mark.job_inital_log_message
-def test_content_of_initial_log_message_match_expected(
-    job_manager, caplog
+@pytest.mark.spark_manager_glue
+@pytest.mark.job_initial_log_message
+def test_content_of_initial_log_message_match_the_expected(
+    spark_manager_glue,
+    caplog
 ):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when the job_initial_message() is called
-    T: then the log message captured must match the expected value based on
-       data_dict attribute used on object creation from GlueJobManager class
+    G: Given that a user wants to initialize a Glue job on AWS
+    W: When the job_initial_message() is called from SparkETLManager with
+       glue mode
+    T: Then the log message captured must match a expected value
     """
 
-    # Degining the expected log message based on data_dict_dictionary used
-    expected_log_msg = "Initializing the execution of a-fake-arg-value job. "\
-        "Data sources used in this ETL process:\n\n"\
-        "Table some-fake-database.orders-fake-table without push down "\
-        "predicate\n"\
-        "Table some-fake-database.customers-fake-table with the following "\
-        "push down predicate info: anomesdia=20221201\n"
-
     # Calling the method for logging the initial message
     with caplog.at_level(logging.INFO):
-        job_manager.job_initial_log_message()
+        spark_manager_glue.job_initial_log_message()
 
-    assert caplog.records[-1].message == expected_log_msg
+    assert caplog.records[-1].message == EXPECTED_START_JOB_MSG
 
 
-@pytest.mark.glue_job_manager
+@pytest.mark.spark_manager_glue
 @pytest.mark.print_args
 def test_print_args_method_really_prints_job_arguments_defined_by_user(
-    job_manager, caplog
+    spark_manager_glue,
+    caplog
 ):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when the print_args() is called
-    T: then the log message captured must have the arguments defined by user
+    G: Given that a user wants to initialize a Glue job on AWS
+    W: When the print_args() is called from SparkETLManager with glue mode
+    T: Then the log message captured must have the arguments defined by user
        on self.argv_list class attribute
     """
 
     # Creating a list for the expected message based on user defined job args
     expected_argv_msg = [f'--{arg}="a-fake-arg-value"'
-                         for arg in FAKE_ARGV_LIST]
+                         for arg in spark_manager_glue.argv_list]
 
     # Calling the method
     with caplog.at_level(logging.INFO):
-        job_manager.print_args()
+        spark_manager_glue.print_args()
 
     assert all(a in caplog.text.split("\n") for a in expected_argv_msg)
 
 
-@pytest.mark.glue_job_manager
+@pytest.mark.spark_manager_glue
 @pytest.mark.get_context_and_session
-def test_getting_context_and_session_elements(job_manager):
+def test_get_context_and_session_method_generates_context_and_session(
+    spark_manager_glue
+):
     """
-    G: given that users want to get the context and session elements
-    W: when method get_context_and_session() is called
-    T: then the object class must have new attributes identified as
+    G: Given that a user wants to get the context and session elements
+    W: When method get_context_and_session() is called from SparkETLManager
+       with glue mode
+    T: Then the object class must have new attributes identified as
        self.sc, self.glueContext and self.spark
     """
 
     # Calling the method for getting context and session elements
-    job_manager.get_context_and_session()
+    spark_manager_glue.get_context_and_session()
 
     # Getting class attributes and defining an assertion list
-    class_attribs = job_manager.__dict__
+    class_attribs = spark_manager_glue.__dict__
     attribs_names = ["sc", "glueContext", "spark"]
 
     # Asserting class has now new attributes
     assert all(a in list(class_attribs.keys()) for a in attribs_names)
 
 
-@pytest.mark.glue_job_manager
+@pytest.mark.spark_manager_glue
 @pytest.mark.get_context_and_session
-def test_type_of_context_and_session_elements_match_expected(job_manager):
+def test_correct_type_of_context_and_session_elements_gotten_in_class(
+    spark_manager_glue
+):
     """
-    G: given that users want to get the context and session elements
-    W: when method get_context_and_session() is called
-    T: then the self.sc must be of type SparkContext, the self.glueContext
+    G: Given that users want to get the context and session elements
+    W: When method get_context_and_session() is called from SparkETLManager
+       with glue mode
+    T: Then the self.sc must be of type SparkContext, the self.glueContext
        attrib must be of type GlueContext and the self.spark attribute must be
        of type SparkSession
     """
 
     # Calling the method for getting context and session elements
-    job_manager.get_context_and_session()
+    spark_manager_glue.get_context_and_session()
 
     # Getting class attributes dictionary
-    class_attribs = job_manager.__dict__
+    class_attribs = spark_manager_glue.__dict__
 
     # Asserting type of each element
     assert type(class_attribs["sc"]) == SparkContext
     assert type(class_attribs["glueContext"]) == GlueContext
     assert type(class_attribs["spark"]) == SparkSession
 
 
-@pytest.mark.glue_job_manager
+@pytest.mark.spark_manager_glue
 @pytest.mark.init_job
-def test_init_job_method_generates_context_and_session_elements(job_manager):
+def test_init_job_method_generates_context_and_session_elements(
+    spark_manager_glue
+):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when method init_job() is called
-    T: then context and session elements from Glue and Spark must exist and
+    G: Given that users want to initialize a Glue job on AWS
+    W: When method init_job() is called from SparkETLManager with glue mode
+    T: Then context and session elements from Glue and Spark must exist and
        its types must match
     """
 
     # Calling method for job initialization
-    job_manager.init_job()
+    spark_manager_glue.init_job()
 
     # Getting class attribs and setting up a assertion list
-    class_attribs = job_manager.__dict__
+    class_attribs = spark_manager_glue.__dict__
     attribs_names = ["sc", "glueContext", "spark"]
 
     # Asserting if the new attributes really exist
     assert all(a in list(class_attribs.keys()) for a in attribs_names)
 
     # Asserting if types match
     assert type(class_attribs["sc"]) == SparkContext
     assert type(class_attribs["glueContext"]) == GlueContext
     assert type(class_attribs["spark"]) == SparkSession
 
 
-@pytest.mark.glue_job_manager
+@pytest.mark.spark_manager_glue
 @pytest.mark.init_job
-def test_init_job_methods_generates_a_job_type_attribute(job_manager):
+def test_init_job_methods_generates_a_job_type_attribute(spark_manager_glue):
     """
-    G: given that users want to initialize a Glue job on AWS
-    W: when method init_job() is called
-    T: then a new class attribute self.job of type awsglue.jobJob must exists
+    G: Given that users want to initialize a Glue job on AWS
+    W: When method init_job() is called from SparkETLManager with glue mode
+    T: Then a new class attribute self.job of type awsglue.job.Job must exists
     """
 
     # Calling method for job initialization
-    job_manager.init_job()
+    spark_manager_glue.init_job()
 
     # Getting class attributes
-    class_attribs = job_manager.__dict__
+    class_attribs = spark_manager_glue.__dict__
 
     assert "job" in class_attribs.keys()
     assert type(class_attribs["job"]) is Job
```

