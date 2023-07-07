# Comparing `tmp/cleanvision-0.3.0.tar.gz` & `tmp/cleanvision-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanvision-0.3.0.tar", last modified: Wed May 24 22:27:52 2023, max compression
+gzip compressed data, was "cleanvision-0.3.1.tar", last modified: Fri Jul  7 19:58:16 2023, max compression
```

## Comparing `cleanvision-0.3.0.tar` & `cleanvision-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-24 22:27:43.000000 cleanvision-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-24 22:27:43.000000 cleanvision-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-24 22:27:43.000000 cleanvision-0.3.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-24 22:27:43.000000 cleanvision-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 22:27:43.000000 cleanvision-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-05-24 22:27:52.661222 cleanvision-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-24 22:27:43.000000 cleanvision-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-24 22:27:43.000000 cleanvision-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:27:52.661222 cleanvision-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/folder_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/imagelab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/src/cleanvision/issue_managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/duplicate_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/image_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/issue_managers/image_property_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/src/cleanvision/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/base_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-24 22:27:43.000000 cleanvision-0.3.0/src/cleanvision/utils/viz_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.657222 cleanvision-0.3.0/src/cleanvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 22:27:52.000000 cleanvision-0.3.0/src/cleanvision.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:52.661222 cleanvision-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_duplicate_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_image_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_image_property_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 22:27:43.000000 cleanvision-0.3.0/tests/test_viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.090724 cleanvision-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 19:58:04.000000 cleanvision-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-07 19:58:04.000000 cleanvision-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-07 19:58:04.000000 cleanvision-0.3.1/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 19:58:04.000000 cleanvision-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 19:58:04.000000 cleanvision-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50513 2023-07-07 19:58:16.090724 cleanvision-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-07-07 19:58:04.000000 cleanvision-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-07 19:58:04.000000 cleanvision-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:58:16.090724 cleanvision-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.078724 cleanvision-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.082724 cleanvision-0.3.1/src/cleanvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/folder_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/imagelab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/issue_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/image_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/base_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.082724 cleanvision-0.3.1/src/cleanvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50513 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.090724 cleanvision-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_image_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_viz_manager.py
```

### Comparing `cleanvision-0.3.0/CODE_OF_CONDUCT.md` & `cleanvision-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/CONTRIBUTING.md` & `cleanvision-0.3.1/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 All kinds of contributions to CleanVision are greatly appreciated. If you're not looking to write code, submitting a [feature request](#feature-requests) or
 [bug report](#bug-reports) is a great way to contribute. If you want to get
 your hands dirty, you can submit [Pull Requests](#pull-requests), either working on your
 own ideas or addressing [existing issues][issues].
 
 If you are unsure or confused about anything, please go ahead and submit your
 issue or pull request anyways! We appreciate all contributions, and we'll do
-our best to incorporate your feedback or code into CleanVision. 
-You can also chat with our developers in [Slack](https://cleanlab.ai/slack).
+our best to incorporate your feedback or code into CleanVision.
+You can also chat with our developers in [Slack][slack].
 
 Detailed contributing instructions can be found in the [Development Guide](DEVELOPMENT.md), please read this carefully!
 
 
 ## Feature Requests
 
 Do you have an idea for an awesome new feature for CleanVision? Let us know by
@@ -45,14 +45,14 @@
 
 Detailed development instructions, such as how to run the tests, are available
 in [DEVELOPMENT.md](DEVELOPMENT.md).
 
 ---
 
 If you have any questions about contributing to CleanVision, feel free to
-[ask][discussions]!
+[ask][slack]!
 
 [issue]: https://github.com/cleanlab/cleanvision/issues/new
 [issues]: https://github.com/cleanlab/cleanvision/issues
 [fork]: https://github.com/cleanlab/cleanvision/fork
 [pr]: https://github.com/cleanlab/cleanvision/pulls
-[discussions]: https://github.com/cleanlab/cleanvision/discussions
+[slack]: https://cleanlab.ai/slack
```

### Comparing `cleanvision-0.3.0/DEVELOPMENT.md` & `cleanvision-0.3.1/DEVELOPMENT.md`

 * *Files 5% similar despite different names*

```diff
@@ -82,21 +82,31 @@
 mypy --strict --install-types --non-interactive --python-version 3.11  src
 ```
 
 ## How to style new code contributions
 
 CleanVision follows the [Black](https://black.readthedocs.io/) code style. This is
 enforced by CI, so please format your code by invoking `black` before submitting a pull request.
+Use the following command to format your code.
+
+```shell
+python -m black src
+```
 
 Generally aim to follow the [PEP-8 coding style](https://peps.python.org/pep-0008/).
 Please do not use wildcard `import *` in any files, instead you should always import the specific functions that you need from a module.
+Use the following command to check for style errors.
+
+```shell
+flake8 --ignore=E203,E501,E722,E401,W503 src tests --count --show-source --statistics
+```
 
 ### Pre-commit hook
 
-This repo uses the [pre-commit framework](https://pre-commit.com/) to easily
+You can also use [pre-commit framework](https://pre-commit.com/) to easily
 set up code style checks that run automatically whenever you make a commit.
 You can install the git hook scripts with:
 
 ```shell
 pre-commit install
 ```
```

### Comparing `cleanvision-0.3.0/LICENSE` & `cleanvision-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/PKG-INFO` & `cleanvision-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.3.0
+Version: 0.3.1
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -746,17 +746,17 @@
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
 
 ## More resources on how to use CleanVision
 
-- [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
-- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Tutorial](https://cleanvision.readthedocs.io/en/latest/tutorials/tutorial.html)
+- [Run CleanVision on a HuggingFace dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/huggingface_dataset.html)
+- [Run CleanVision on a Torchvision dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/torchvision_dataset.html)
 - [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
@@ -765,24 +765,25 @@
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
 To detect issues in the labels of your image data, you can instead
 use the [cleanlab](https://github.com/cleanlab/cleanlab/) package.
 
 In any collection of image files (most [formats](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html) supported), CleanVision can detect the following types of issues:
 
-|     | Issue Type       | Description                                               | Issue Key        | Example                                                                                                             |
-|-----|------------------|-----------------------------------------------------------|------------------|---------------------------------------------------------------------------------------------------------------------|
-| 1   | Exact Duplicates | Images that are identical to each other            | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png) |
-| 2   | Near Duplicates  | Images that are visually almost identical          | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)  |
-| 3   | Blurry           | Images where details are fuzzy (out of focus)                             | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)           |
-| 4   | Low Information  | Images lacking content (little entropy in pixel values) | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)  |
-| 5   | Dark             | Irregularly dark images (*under*exposed)                                   | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)             |
-| 6   | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)            |
-| 7   | Grayscale        | Images lacking color                                      | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)        |
-| 8   | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)            | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg) |
+|   | Issue Type       | Description                                                     | Issue Key        | Example                                                                                                                                 |
+|---|------------------|-----------------------------------------------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
+| 1 | Exact Duplicates | Images that are identical to each other                         | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png)                     |
+| 2 | Near Duplicates  | Images that are visually almost identical                       | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)                      |
+| 3 | Blurry           | Images where details are fuzzy (out of focus)                   | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)                               |
+| 4 | Low Information  | Images lacking content (little entropy in pixel values)         | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)                      |
+| 5 | Dark             | Irregularly dark images (*under*exposed)                        | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)                                 |
+| 6 | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)                                |
+| 7 | Grayscale        | Images lacking color                                            | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)                            |
+| 8 | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)        | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg)                     |
+| 9 | Odd Size         | Images that are abnormally large or small | odd_size         | <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_size.png" width=20% height=20%> |
 
 This package is still a work in progress, so expect sharp edges.
 Feel free to submit any found bugs or desired functionality as an [issue][issue]!
 
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
@@ -812,8 +813,11 @@
 version.
 
 cleanvision is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 See [GNU Affero General Public LICENSE](https://github.com/cleanlab/cleanvision/blob/main/LICENSE) for details.
 
+For enterprise teams that want to use CleanVision in production workflows but are unable to open-source their code, you can contact us to discuss alternative commercial licensing: team@cleanlab.ai
+
+
 [issue]: https://github.com/cleanlab/cleanvision/issues/new
```

### Comparing `cleanvision-0.3.0/README.md` & `cleanvision-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
 
 ## More resources on how to use CleanVision
 
-- [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
-- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Tutorial](https://cleanvision.readthedocs.io/en/latest/tutorials/tutorial.html)
+- [Run CleanVision on a HuggingFace dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/huggingface_dataset.html)
+- [Run CleanVision on a Torchvision dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/torchvision_dataset.html)
 - [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
@@ -74,24 +74,25 @@
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
 To detect issues in the labels of your image data, you can instead
 use the [cleanlab](https://github.com/cleanlab/cleanlab/) package.
 
 In any collection of image files (most [formats](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html) supported), CleanVision can detect the following types of issues:
 
-|     | Issue Type       | Description                                               | Issue Key        | Example                                                                                                             |
-|-----|------------------|-----------------------------------------------------------|------------------|---------------------------------------------------------------------------------------------------------------------|
-| 1   | Exact Duplicates | Images that are identical to each other            | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png) |
-| 2   | Near Duplicates  | Images that are visually almost identical          | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)  |
-| 3   | Blurry           | Images where details are fuzzy (out of focus)                             | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)           |
-| 4   | Low Information  | Images lacking content (little entropy in pixel values) | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)  |
-| 5   | Dark             | Irregularly dark images (*under*exposed)                                   | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)             |
-| 6   | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)            |
-| 7   | Grayscale        | Images lacking color                                      | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)        |
-| 8   | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)            | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg) |
+|   | Issue Type       | Description                                                     | Issue Key        | Example                                                                                                                                 |
+|---|------------------|-----------------------------------------------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
+| 1 | Exact Duplicates | Images that are identical to each other                         | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png)                     |
+| 2 | Near Duplicates  | Images that are visually almost identical                       | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)                      |
+| 3 | Blurry           | Images where details are fuzzy (out of focus)                   | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)                               |
+| 4 | Low Information  | Images lacking content (little entropy in pixel values)         | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)                      |
+| 5 | Dark             | Irregularly dark images (*under*exposed)                        | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)                                 |
+| 6 | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)                                |
+| 7 | Grayscale        | Images lacking color                                            | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)                            |
+| 8 | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)        | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg)                     |
+| 9 | Odd Size         | Images that are abnormally large or small | odd_size         | <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_size.png" width=20% height=20%> |
 
 This package is still a work in progress, so expect sharp edges.
 Feel free to submit any found bugs or desired functionality as an [issue][issue]!
 
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
@@ -121,8 +122,11 @@
 version.
 
 cleanvision is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 See [GNU Affero General Public LICENSE](https://github.com/cleanlab/cleanvision/blob/main/LICENSE) for details.
 
+For enterprise teams that want to use CleanVision in production workflows but are unable to open-source their code, you can contact us to discuss alternative commercial licensing: team@cleanlab.ai
+
+
 [issue]: https://github.com/cleanlab/cleanvision/issues/new
```

### Comparing `cleanvision-0.3.0/pyproject.toml` & `cleanvision-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cleanvision"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "Cleanlab Inc.", email = "team@cleanlab.ai" },
 ]
 description = "Find issues in image datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["computer_vision", "cv", "image_data", "issue_detection", "data_quality", "image_quality", "machine_learning", "data_cleaning", "image_deduplication"]
```

### Comparing `cleanvision-0.3.0/src/cleanvision/dataset/base_dataset.py` & `cleanvision-0.3.1/src/cleanvision/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/dataset/folder_dataset.py` & `cleanvision-0.3.1/src/cleanvision/dataset/folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/dataset/hf_dataset.py` & `cleanvision-0.3.1/src/cleanvision/dataset/hf_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return len(self._data)
 
     def __getitem__(self, item: Union[int, str]) -> Optional[Image.Image]:
         try:
             image = self._data[item][self._image_key]
             return image
         except Exception as e:
-            print(f"Could not load image at index: {item}", e)
+            print(f"Could not load image at index: {item}\n", e)
             return None
 
     def _set_index(self) -> None:
         self.index = [i for i in range(len(self._data))]
 
     def get_name(self, item: Union[int, str]) -> str:
         return f"idx: {item}"
```

### Comparing `cleanvision-0.3.0/src/cleanvision/dataset/torch_dataset.py` & `cleanvision-0.3.1/src/cleanvision/dataset/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/dataset/utils.py` & `cleanvision-0.3.1/src/cleanvision/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/imagelab.py` & `cleanvision-0.3.1/src/cleanvision/imagelab.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
 Imagelab is the core class in CleanVision for finding all types of issues in an image dataset.
 The methods in this module should suffice for most use-cases,
 but advanced users can get extra flexibility via the code in other CleanVision modules.
 """
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, TypeVar, List, Dict, Any, Optional, Tuple, Type
+import random
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 import cleanvision
 from cleanvision.dataset.torch_dataset import TorchDataset
 from cleanvision.dataset.utils import build_dataset
 from cleanvision.issue_managers import (
-    IssueType,
-    IssueManagerFactory,
     ISSUE_MANAGER_REGISTRY,
+    IssueManagerFactory,
+    IssueType,
 )
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import (
-    IMAGE_PROPERTY,
+    DEFAULT_ISSUE_TYPES,
     DUPLICATE,
-    IMAGE_PROPERTY_ISSUE_TYPES_LIST,
     DUPLICATE_ISSUE_TYPES_LIST,
+    IMAGE_PROPERTY,
+    IMAGE_PROPERTY_ISSUE_TYPES_LIST,
     SETS,
 )
 from cleanvision.utils.serialize import Serializer
 from cleanvision.utils.utils import (
     deep_update_dict,
     get_is_issue_colname,
+    get_max_n_jobs,
     get_score_colname,
     update_df,
-    get_max_n_jobs,
 )
 from cleanvision.utils.viz_manager import VizManager
 
 if TYPE_CHECKING:  # pragma: no cover
     import datasets
     from torchvision.datasets.vision import VisionDataset
 
@@ -131,93 +133,85 @@
             columns=["issue_type", "num_images"]
         ).astype({"issue_type": str, "num_images": np.int64})
 
         self.issues: pd.DataFrame = pd.DataFrame(index=self._dataset.index)
         self._issue_types: List[str] = []
         self._issue_managers: Dict[str, IssueManager] = {}
 
-        # can be loaded from a file later
+        # TODO: can be loaded from a file later
         self._config: Dict[str, Any] = self._set_default_config()
         self.cleanvision_version: str = cleanvision.__version__
 
     def _set_default_config(self) -> Dict[str, Any]:
         """Sets default values for various config variables used in Imagelab class
         The naming convention for methods is {method_name}_{config_variable_name}
 
         Returns
         -------
         Dict[str, Any]
             Returns a dict with keys as config variables and their values as dict values
         """
         return {
             "visualize_num_images_per_row": 4,
-            "report_examples_per_issue_values": [4, 8, 16, 32],
+            "report_num_images": 4,
             "report_max_prevalence": 0.5,
-            "default_issue_types": [
-                IssueType.DARK,
-                IssueType.LIGHT,
-                IssueType.ODD_ASPECT_RATIO,
-                IssueType.LOW_INFORMATION,
-                IssueType.EXACT_DUPLICATES,
-                IssueType.NEAR_DUPLICATES,
-                IssueType.BLURRY,
-                IssueType.GRAYSCALE,
-            ],
+            "report_cell_size": (2, 2),
         }
 
-    def list_default_issue_types(self) -> None:
-        """Prints list of the issue types detected by default if no types are specified in :py:meth:`Imagelab.find_issues`"""
-
-        print("Default issue type checked by Imagelab:\n")
-        print(
-            *[issue_type.value for issue_type in self._config["default_issue_types"]],
-            sep="\n",
-        )
-
-    def list_possible_issue_types(self) -> None:
-        """Prints list of all possible issue types that can be detected in a dataset.
-        This list will also include custom issue types if you properly add them.
+    @staticmethod
+    def list_default_issue_types() -> List[str]:
+        """Returns a list of the issue types that are run by default in :py:meth:`Imagelab.find_issues`"""
+        return DEFAULT_ISSUE_TYPES
+
+    @staticmethod
+    def list_possible_issue_types() -> List[str]:
+        """Returns a list of all the possible issue types that can be run in :py:meth:`Imagelab.find_issues`
+        This list will also include custom issue types if properly added.
         """
-        print("All possible issues checked by Imagelab:\n")
-        issue_types = {issue_type.value for issue_type in IssueType}
-        issue_types.update(ISSUE_MANAGER_REGISTRY.keys())
-        print(*issue_types, sep="\n")
-        print("\n")
+        issue_types = Imagelab.list_default_issue_types()
+        for key in ISSUE_MANAGER_REGISTRY:
+            if key not in [IMAGE_PROPERTY, DUPLICATE]:
+                issue_types.append(key)
+        return list(set(issue_types))
 
     def _get_issues_to_compute(
         self, issue_types_with_params: Optional[Dict[str, Any]]
     ) -> Dict[str, Any]:
         if not issue_types_with_params:
             to_compute_issues_with_params: Dict[str, Any] = {
-                issue_type.value: {}
-                for issue_type in self._config["default_issue_types"]
+                issue_type: {} for issue_type in self.list_default_issue_types()
             }
         else:
             to_compute_issues_with_params = {
                 issue_type_str: params
                 for issue_type_str, params in issue_types_with_params.items()
             }
         return to_compute_issues_with_params
 
     def find_issues(
-        self, issue_types: Optional[Dict[str, Any]] = None, n_jobs: Optional[int] = None
+        self,
+        issue_types: Optional[Dict[str, Any]] = None,
+        n_jobs: Optional[int] = None,
+        verbose: bool = True,
     ) -> None:
         """Finds issues in the dataset.
         If `issue_types` is not provided, dataset is checked for a default set of issue types.
         To see default set: :py:meth:`Imagelab.list_default_issue_types`
 
         Parameters
         ----------
         issue_types : Dict[str, Any], optional
             Dict with issue types to check as keys.
             The value of this dict is a dict containing hyperparameters for each issue type.
         n_jobs :  int, default=None
             Number of processing threads used by multiprocessing.
             Default None sets to the number of cores on your CPU (physical cores if you have psutil package installed, otherwise logical cores).
             Set this to 1 to disable parallel processing (if its causing issues). Windows users may see a speed-up with n_jobs=1.
+        verbose : bool, default=True
+            If True, prints helpful information while checking for issues.
 
         Examples
         --------
         To check for all default issue types use
 
         .. code-block:: python
 
@@ -243,17 +237,18 @@
             }
             imagelab.find_issues(issue_types)
 
 
 
         """
         to_compute_issues_with_params = self._get_issues_to_compute(issue_types)
-        print(
-            f"Checking for {', '.join([issue_type for issue_type in to_compute_issues_with_params.keys()])} images ..."
-        )
+        if verbose:
+            print(
+                f"Checking for {', '.join([issue_type for issue_type in to_compute_issues_with_params.keys()])} images ..."
+            )
 
         # update issue_types
         self._issue_types = list(
             set(self._issue_types).union(set(to_compute_issues_with_params.keys()))
         )
 
         # set issue managers
@@ -281,17 +276,18 @@
             self._update_issue_summary(issue_manager.summary)
             self._update_info(issue_manager.info)
 
         self.issue_summary = self.issue_summary.sort_values(
             by=["num_images"], ascending=False
         )
         self.issue_summary = self.issue_summary.reset_index(drop=True)
-        print(
-            "Issue checks completed. To see a detailed report of issues found, use imagelab.report()."
-        )
+        if verbose:
+            print(
+                f"Issue checks completed. {self.issue_summary['num_images'].sum()} issues found in the dataset. To see a detailed report of issues found, use imagelab.report()."
+            )
         return
 
     def _update_info(self, issue_manager_info: Dict[str, Any]) -> None:
         deep_update_dict(self.info, issue_manager_info)
 
     def _update_issue_summary(self, issue_manager_summary: pd.DataFrame) -> None:
         # Remove results for issue types computed again
@@ -347,36 +343,34 @@
             else:
                 print(
                     f"Removing {getattr(row, 'issue_type')} from potential issues in the dataset as it exceeds "
                     f"max_prevalence={max_prevalence} "
                 )
         return issue_to_report
 
-    def _get_report_args(
-        self, verbosity: int, user_supplied_args: Dict[str, Any]
-    ) -> Dict[str, Any]:
+    def _get_report_args(self, user_supplied_args: Dict[str, Any]) -> Dict[str, Any]:
         report_args = {
             "max_prevalence": self._config["report_max_prevalence"],
-            "examples_per_issue": self._config["report_examples_per_issue_values"][
-                verbosity - 1
-            ],
+            "num_images": self._config["report_num_images"],
+            "cell_size": self._config["report_cell_size"],
         }
 
         non_none_args = {
             arg: value for arg, value in user_supplied_args.items() if value is not None
         }
 
         return {**report_args, **non_none_args}
 
     def report(
         self,
         issue_types: Optional[List[str]] = None,
         max_prevalence: Optional[float] = None,
         num_images: Optional[int] = None,
         verbosity: int = 1,
+        print_summary: bool = True,
     ) -> None:
         """Prints summary of the issues found in your dataset.
         By default, this method depicts the images representing top-most severe instances of each issue type.
 
         Parameters
         ----------
         issue_types : List[str], optional
@@ -390,14 +384,17 @@
 
         num_images : int, default=4
             Maximum number of images to show for issue type reported. These are examples of the top-most severe instances of the issue in your dataset.
 
         verbosity : int, {1, 2, 3, 4}
             Increasing verbosity increases the detail of the report. Set this to 1 to report less information, or to 4 to report the most information.
 
+        print_summary : bool, default=True
+            If True, prints the summary of issues found in the dataset.
+
         Examples
         --------
         Default usage
 
         .. code-block:: python
 
             imagelab.report()
@@ -406,50 +403,58 @@
 
         .. code-block:: python
 
             issue_types = ["dark", "near_duplicates"]
             imagelab.report(issue_types=issue_types)
 
         """
-        assert isinstance(verbosity, int) and 0 < verbosity < 5
+        assert isinstance(verbosity, int) and 0 <= verbosity < 5
 
         user_supplied_args = locals()
-        report_args = self._get_report_args(verbosity, user_supplied_args)
+        report_args = self._get_report_args(user_supplied_args)
 
-        if issue_types:
-            issue_types_to_report = issue_types
-        else:
-            # Remove issues with zero images from the report
-            non_zero_issue_types = self.issue_summary[
-                self.issue_summary["num_images"] > 0
-            ]["issue_type"].tolist()
-            issue_types_to_report = non_zero_issue_types
+        issue_types_to_report = (
+            issue_types if issue_types else self.issue_summary["issue_type"].tolist()
+        )
 
         # filter issues based on max_prevalence in the dataset
         filtered_issue_types = self._filter_report(
             issue_types_to_report, report_args["max_prevalence"]
         )
 
         issue_summary = self.issue_summary[
             self.issue_summary["issue_type"].isin(filtered_issue_types)
         ]
         if len(issue_summary) > 0:
-            print("Issues found in order of severity in the dataset\n")
-            self._pprint_issue_summary(issue_summary)
-
-            self.visualize(
-                issue_types=filtered_issue_types,
-                num_images=(
-                    report_args["examples_per_issue"]
-                    if num_images is None
-                    else num_images
-                ),
-            )
+            if verbosity:
+                print("Issues found in images in order of severity in the dataset\n")
+            if print_summary:
+                self._pprint_issue_summary(issue_summary)
+            for issue_type in filtered_issue_types:
+                if (
+                    self.issue_summary.query(f"issue_type == '{issue_type}'")[
+                        "num_images"
+                    ].values[0]
+                    == 0
+                ):
+                    continue
+                print(f"{' ' + issue_type + ' images ':-^60}\n")
+                print(
+                    f"Number of examples with this issue: {self.issues[get_is_issue_colname(issue_type)].sum()}\n"
+                    f"Examples representing most severe instances of this issue:\n"
+                )
+                self._visualize(
+                    issue_type,
+                    report_args["num_images"],
+                    report_args["cell_size"],
+                )
         else:
-            print("No issues found.")
+            print(
+                "Please specify some issue_types to check for in imagelab.find_issues()."
+            )
 
     def _pprint_issue_summary(self, issue_summary: pd.DataFrame) -> None:
         issue_summary_copy = issue_summary.copy()
         issue_summary_copy.dropna(axis=1, how="all", inplace=True)
         issue_summary_copy.fillna("N/A", inplace=True)
         print(issue_summary_copy.to_markdown(), "\n")
 
@@ -471,55 +476,45 @@
         issue_manager = self._get_issue_manager(issue_type)
         viz_name = issue_manager.visualization
 
         if viz_name == "individual_images":
             sorted_df = self.issues.sort_values(by=get_score_colname(issue_type))
             sorted_df = sorted_df[sorted_df[get_is_issue_colname(issue_type)] == 1]
 
-            examples_str = "examples" if len(sorted_df) > 1 else "example"
-            if len(sorted_df) < num_images:
-                print(
-                    f"Found {len(sorted_df)} {examples_str} with {issue_type} issue in the dataset."
-                )
-            else:
-                print(
-                    f"\nTop {num_images} {examples_str} with {issue_type} issue in the dataset."
-                )
-
             scores = sorted_df.head(num_images)[get_score_colname(issue_type)]
-            titles = [f"score : {x:.4f}" for x in scores]
             indices = scores.index.tolist()
             images = [self._dataset[i] for i in indices]
+
+            titles = [f"score : {x:.4f}" for x in scores]
+
+            # Add size information for odd sized images
+            additional_info = None
+            if issue_type == IssueType.ODD_SIZE.value:
+                additional_info = []
+                for image in images:
+                    additional_info.append(f"original size: {image.size}")
+
             if images:
                 VizManager.individual_images(
                     images=images,
                     titles=titles,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
+                    additional_info=additional_info,
                 )
 
         elif viz_name == "image_sets":
             image_sets_indices = sorted(
                 self.info[issue_type][SETS], key=len, reverse=True
             )
             image_sets_indices = image_sets_indices[:num_images]
             image_sets = []
             for indices in image_sets_indices:
                 image_sets.append([self._dataset[index] for index in indices])
 
-            sets_str = "sets" if len(image_sets) > 1 else "set"
-            if len(image_sets) < num_images:
-                print(
-                    f"Found {len(image_sets)} {sets_str} of images with {issue_type} issue in the dataset."
-                )
-            else:
-                print(
-                    f"\nTop {num_images} {sets_str} of images with {issue_type} issue"
-                )
-
             title_sets = [
                 [self._dataset.get_name(index) for index in s]
                 for s in image_sets_indices
             ]
 
             if image_sets:
                 VizManager.image_sets(
@@ -596,21 +591,20 @@
 
         .. code-block:: python
 
             issue_types = ["dark", "odd_aspect_ratio"]
             imagelab.visualize(issue_types=issue_types)
 
         """
-        if issue_types:
+        if issue_types is not None:
             if len(issue_types) == 0:
                 raise ValueError("issue_types list is empty")
             for issue_type in issue_types:
                 self._visualize(issue_type, num_images, cell_size)
-        elif image_files:
-            # todo: write test
+        elif image_files is not None:
             if len(image_files) == 0:
                 raise ValueError("image_files list is empty.")
             images = [Image.open(path) for path in image_files]
             titles = [path.split("/")[-1] for path in image_files]
             VizManager.individual_images(
                 images,
                 titles,
@@ -623,25 +617,19 @@
             VizManager.individual_images(
                 images,
                 titles,
                 ncols=self._config["visualize_num_images_per_row"],
                 cell_size=cell_size,
             )
         else:
-            # todo: write test
             print("Sample images from the dataset")
+
             if image_files is None:
-                image_indices = list(
-                    np.random.choice(
-                        self._dataset.index,
-                        min(
-                            num_images, len(self._dataset)
-                        ),  # in case the len(dataset) < 4
-                        replace=False,
-                    )
+                image_indices = random.sample(
+                    self._dataset.index, min(num_images, len(self._dataset))
                 )
                 images = [self._dataset[i] for i in image_indices]
                 titles = [self._dataset.get_name(i) for i in image_indices]
                 VizManager.individual_images(
                     images,
                     titles,
                     ncols=self._config["visualize_num_images_per_row"],
```

### Comparing `cleanvision-0.3.0/src/cleanvision/issue_managers/__init__.py` & `cleanvision-0.3.1/src/cleanvision/issue_managers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     LIGHT = "light"
     ODD_ASPECT_RATIO = "odd_aspect_ratio"
     LOW_INFORMATION = "low_information"
     EXACT_DUPLICATES = "exact_duplicates"
     NEAR_DUPLICATES = "near_duplicates"
     BLURRY = "blurry"
     GRAYSCALE = "grayscale"
+    ODD_SIZE = "odd_size"
 
 
 ISSUE_MANAGER_REGISTRY: Dict[str, Type[IssueManager]] = {}
 
 
 class IssueManagerFactory:
     """Factory class for constructing concrete issue managers."""
```

### Comparing `cleanvision-0.3.0/src/cleanvision/issue_managers/duplicate_issue_manager.py` & `cleanvision-0.3.1/src/cleanvision/issue_managers/duplicate_issue_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     if hash_type == "md5":
         pixels = np.asarray(image)
         return hashlib.md5(pixels.tobytes()).hexdigest()
     elif hash_type == "whash":
         return str(imagehash.whash(image, hash_size=hash_size))
     elif hash_type == "phash":
         return str(imagehash.phash(image, hash_size=hash_size))
+    elif hash_type == "ahash":
+        return str(imagehash.average_hash(image, hash_size=hash_size))
+    elif hash_type == "dhash":
+        return str(imagehash.dhash(image, hash_size=hash_size))
+    elif hash_type == "chash":
+        return str(imagehash.colorhash(image, binbits=hash_size))
     else:
         raise ValueError("Hash type not supported")
 
 
 def compute_hash(
     index: int,
     dataset: Dataset,
```

### Comparing `cleanvision-0.3.0/src/cleanvision/issue_managers/image_property.py` & `cleanvision-0.3.1/src/cleanvision/issue_managers/image_property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from abc import ABC, abstractmethod
 from typing import List, Dict, Any, Union, overload
 
 import numpy as np
 import pandas as pd
 from PIL import ImageStat, ImageFilter
 from PIL.Image import Image
@@ -288,14 +289,19 @@
     return edges
 
 
 def calc_color_space(image: Image) -> str:
     return get_image_mode(image)
 
 
+def calc_image_area_sqrt(image: Image) -> float:
+    size = image.size
+    return math.sqrt(size[0] * size[1])
+
+
 class ColorSpaceProperty(ImageProperty):
     name = "color_space"
 
     @property
     def score_columns(self) -> List[str]:
         return self._score_columns
 
@@ -325,14 +331,57 @@
         is_issue = pd.DataFrame(index=scores.index)
         is_issue[get_is_issue_colname(issue_type)] = (
             1 - scores[get_score_colname(issue_type)]
         ).astype("bool")
         return is_issue
 
 
+class SizeProperty(ImageProperty):
+    name = "size"
+
+    @property
+    def score_columns(self) -> List[str]:
+        return self._score_columns
+
+    def __init__(self) -> None:
+        self._score_columns = [self.name]
+
+    def calculate(self, image: Image) -> Dict[str, Union[float, str]]:
+        return {self.name: calc_image_area_sqrt(image)}
+
+    def get_scores(
+        self,
+        raw_scores: pd.DataFrame,
+        issue_type: str,
+        **kwargs: Any,
+    ) -> pd.DataFrame:
+        super().get_scores(raw_scores, issue_type, **kwargs)
+        assert raw_scores is not None
+        scores = pd.DataFrame(index=raw_scores.index)
+        scores[get_score_colname(issue_type)] = raw_scores[self.score_columns[0]].apply(
+            lambda x: 1.0
+            / max(
+                x / raw_scores[self.score_columns[0]].median(),
+                raw_scores[self.score_columns[0]].median() / x,
+            )
+        )
+        return scores
+
+    def mark_issue(
+        self, scores: pd.DataFrame, threshold: float, issue_type: str
+    ) -> pd.DataFrame:
+        is_issue = pd.DataFrame(index=scores.index)
+        is_issue[get_is_issue_colname(issue_type)] = np.where(
+            scores[get_score_colname(issue_type)] < 1.0 / threshold,
+            True,
+            False,
+        )
+        return is_issue
+
+
 def get_image_mode(image: Image) -> str:
     if image.mode:
         image_mode = image.mode
         assert isinstance(image_mode, str)
         return image_mode
     else:
         imarr = np.asarray(image)
```

### Comparing `cleanvision-0.3.0/src/cleanvision/issue_managers/image_property_issue_manager.py` & `cleanvision-0.3.1/src/cleanvision/issue_managers/image_property_issue_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from cleanvision.issue_managers.image_property import (
     BrightnessProperty,
     AspectRatioProperty,
     EntropyProperty,
     BlurrinessProperty,
     ColorSpaceProperty,
     ImageProperty,
+    SizeProperty,
 )
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import (
     IMAGE_PROPERTY,
     MAX_PROCS,
     IMAGE_PROPERTY_ISSUE_TYPES_LIST,
 )
@@ -67,14 +68,15 @@
             },
             IssueType.BLURRY.value: {
                 "threshold": 0.29,
                 "normalizing_factor": 0.01,
                 "color_threshold": 0.18,
             },
             IssueType.GRAYSCALE.value: {},
+            IssueType.ODD_SIZE.value: {"threshold": 10.0},
         }
 
     def update_params(self, params: Dict[str, Any]) -> None:
         for issue_type in self.params:
             non_none_params = {
                 k: v for k, v in params.get(issue_type, {}).items() if v is not None
             }
@@ -84,14 +86,15 @@
         return {
             IssueType.DARK.value: BrightnessProperty(IssueType.DARK.value),
             IssueType.LIGHT.value: BrightnessProperty(IssueType.LIGHT.value),
             IssueType.ODD_ASPECT_RATIO.value: AspectRatioProperty(),
             IssueType.LOW_INFORMATION.value: EntropyProperty(),
             IssueType.BLURRY.value: BlurrinessProperty(),
             IssueType.GRAYSCALE.value: ColorSpaceProperty(),
+            IssueType.ODD_SIZE.value: SizeProperty(),
         }
 
     def _get_defer_set(
         self, issue_types: List[str], agg_computations: pd.DataFrame
     ) -> Set[str]:
         defer_set = set()
```

### Comparing `cleanvision-0.3.0/src/cleanvision/utils/base_issue_manager.py` & `cleanvision-0.3.1/src/cleanvision/utils/base_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/utils/serialize.py` & `cleanvision-0.3.1/src/cleanvision/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision/utils/utils.py` & `cleanvision-0.3.1/src/cleanvision/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/src/cleanvision.egg-info/PKG-INFO` & `cleanvision-0.3.1/src/cleanvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.3.0
+Version: 0.3.1
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -746,17 +746,17 @@
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
 
 ## More resources on how to use CleanVision
 
-- [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
-- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Tutorial](https://cleanvision.readthedocs.io/en/latest/tutorials/tutorial.html)
+- [Run CleanVision on a HuggingFace dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/huggingface_dataset.html)
+- [Run CleanVision on a Torchvision dataset](https://cleanvision.readthedocs.io/en/latest/tutorials/torchvision_dataset.html)
 - [Example script](https://github.com/cleanlab/cleanvision/blob/main/docs/source/tutorials/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
 - [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
@@ -765,24 +765,25 @@
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
 To detect issues in the labels of your image data, you can instead
 use the [cleanlab](https://github.com/cleanlab/cleanlab/) package.
 
 In any collection of image files (most [formats](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html) supported), CleanVision can detect the following types of issues:
 
-|     | Issue Type       | Description                                               | Issue Key        | Example                                                                                                             |
-|-----|------------------|-----------------------------------------------------------|------------------|---------------------------------------------------------------------------------------------------------------------|
-| 1   | Exact Duplicates | Images that are identical to each other            | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png) |
-| 2   | Near Duplicates  | Images that are visually almost identical          | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)  |
-| 3   | Blurry           | Images where details are fuzzy (out of focus)                             | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)           |
-| 4   | Low Information  | Images lacking content (little entropy in pixel values) | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)  |
-| 5   | Dark             | Irregularly dark images (*under*exposed)                                   | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)             |
-| 6   | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)            |
-| 7   | Grayscale        | Images lacking color                                      | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)        |
-| 8   | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)            | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg) |
+|   | Issue Type       | Description                                                     | Issue Key        | Example                                                                                                                                 |
+|---|------------------|-----------------------------------------------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
+| 1 | Exact Duplicates | Images that are identical to each other                         | exact_duplicates | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/exact_duplicates.png)                     |
+| 2 | Near Duplicates  | Images that are visually almost identical                       | near_duplicates  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/near_duplicates.png)                      |
+| 3 | Blurry           | Images where details are fuzzy (out of focus)                   | blurry           | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/blurry.png)                               |
+| 4 | Low Information  | Images lacking content (little entropy in pixel values)         | low_information  | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/low_information.png)                      |
+| 5 | Dark             | Irregularly dark images (*under*exposed)                        | dark             | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/dark.jpg)                                 |
+| 6 | Light            | Irregularly bright images (*over*exposed)                       | light            | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/light.jpg)                                |
+| 7 | Grayscale        | Images lacking color                                            | grayscale        | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/grayscale.jpg)                            |
+| 8 | Odd Aspect Ratio | Images with an unusual aspect ratio (overly skinny/wide)        | odd_aspect_ratio | ![](https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_aspect_ratio.jpg)                     |
+| 9 | Odd Size         | Images that are abnormally large or small | odd_size         | <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanvision/example_issue_images/odd_size.png" width=20% height=20%> |
 
 This package is still a work in progress, so expect sharp edges.
 Feel free to submit any found bugs or desired functionality as an [issue][issue]!
 
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
@@ -812,8 +813,11 @@
 version.
 
 cleanvision is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 See [GNU Affero General Public LICENSE](https://github.com/cleanlab/cleanvision/blob/main/LICENSE) for details.
 
+For enterprise teams that want to use CleanVision in production workflows but are unable to open-source their code, you can contact us to discuss alternative commercial licensing: team@cleanlab.ai
+
+
 [issue]: https://github.com/cleanlab/cleanvision/issues/new
```

### Comparing `cleanvision-0.3.0/src/cleanvision.egg-info/SOURCES.txt` & `cleanvision-0.3.1/src/cleanvision.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 tests/test_dataset.py
 tests/test_duplicate_issue_manager.py
 tests/test_image_property_helpers.py
 tests/test_image_property_issue_manager.py
 tests/test_run.py
 tests/test_save_load.py
 tests/test_utils.py
+tests/test_visualize.py
 tests/test_viz_manager.py
```

### Comparing `cleanvision-0.3.0/tests/test_dataset.py` & `cleanvision-0.3.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/tests/test_duplicate_issue_manager.py` & `cleanvision-0.3.1/tests/test_duplicate_issue_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,10 +244,19 @@
 
     hash = get_hash(img, {"hash_type": "whash", "hash_size": 2})
     assert hash is not None
 
     hash = get_hash(img, {"hash_type": "phash", "hash_size": 2})
     assert hash is not None
 
+    hash = get_hash(img, {"hash_type": "ahash", "hash_size": 2})
+    assert hash is not None
+
+    hash = get_hash(img, {"hash_type": "dhash", "hash_size": 2})
+    assert hash is not None
+
+    hash = get_hash(img, {"hash_type": "chash", "hash_size": 2})
+    assert hash is not None
+
     # Test calling function with not a real hash
     with pytest.raises(ValueError, match="not supported"):
         get_hash(img, {"hash_type": "fake_hash"})
```

### Comparing `cleanvision-0.3.0/tests/test_image_property_helpers.py` & `cleanvision-0.3.1/tests/test_image_property_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 import pandas as pd
 import pytest
 from PIL import Image
 
 import cleanvision
+import math
 from cleanvision.issue_managers import IssueType
 from cleanvision.issue_managers.image_property import (
     BrightnessProperty,
     calculate_brightness,
     get_image_mode,
     calc_aspect_ratio,
     calc_entropy,
+    calc_image_area_sqrt,
     calc_blurriness,
 )
 from cleanvision.utils.utils import get_is_issue_colname, get_score_colname
 
 
 @pytest.mark.parametrize(
     "rgb,expected_brightness",
@@ -46,14 +48,20 @@
 
 def test_calc_bluriness():
     gray_img = Image.new("RGB", (200, 200), (0, 0, 0)).convert("L")
     blurriness = calc_blurriness(gray_img)
     assert blurriness == 0
 
 
+def test_calc_area():
+    img = Image.new("RGB", (200, 200), (255, 0, 0))
+    area = calc_image_area_sqrt(img)  # img.size[0] * img.size[1]
+    assert area == math.sqrt(200 * 200)
+
+
 @pytest.mark.parametrize(
     "image,expected_mode",
     [
         [Image.new("RGB", (164, 164), (255, 255, 255)), "RGB"],
         [Image.new("RGB", (164, 164)), "RGB"],
         [Image.new("L", (164, 164)), "L"],
         [Image.new("RGB", (164, 164), (255, 160, 255)), "RGB"],
```

### Comparing `cleanvision-0.3.0/tests/test_image_property_issue_manager.py` & `cleanvision-0.3.1/tests/test_image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/tests/test_save_load.py` & `cleanvision-0.3.1/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.0/tests/test_viz_manager.py` & `cleanvision-0.3.1/tests/test_viz_manager.py`

 * *Files identical despite different names*

