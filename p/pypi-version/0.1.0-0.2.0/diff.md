# Comparing `tmp/pypi-version-0.1.0.tar.gz` & `tmp/pypi-version-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypi-version-0.1.0.tar", last modified: Sat Apr  6 14:35:13 2019, max compression
+gzip compressed data, was "dist/pypi-version-0.2.0.tar", last modified: Tue Apr 30 16:14:27 2019, max compression
```

## Comparing `pypi-version-0.1.0.tar` & `pypi-version-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:35:13.000000 pypi-version-0.1.0/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2019-03-28 10:10:32.000000 pypi-version-0.1.0/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       83 2019-04-06 14:34:56.000000 pypi-version-0.1.0/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    11824 2019-04-06 14:35:13.000000 pypi-version-0.1.0/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     9111 2019-04-06 14:34:56.000000 pypi-version-0.1.0/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       22 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1311 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/cli.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     2139 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/config.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      529 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/constants.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      367 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/errors.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     2230 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/main.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      497 2019-04-06 14:34:56.000000 pypi-version-0.1.0/pypi_version/utils.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    11824 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      498 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       55 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/entry_points.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       57 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       19 2019-04-06 14:35:13.000000 pypi-version-0.1.0/pypi_version.egg-info/top_level.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       57 2019-04-06 14:34:56.000000 pypi-version-0.1.0/requirements.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      358 2019-04-06 14:35:13.000000 pypi-version-0.1.0/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1297 2019-04-06 14:34:56.000000 pypi-version-0.1.0/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:35:13.000000 pypi-version-0.1.0/tests/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:34:56.000000 pypi-version-0.1.0/tests/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      630 2019-04-06 14:34:56.000000 pypi-version-0.1.0/tests/conftest.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3521 2019-04-06 14:34:56.000000 pypi-version-0.1.0/tests/test_main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:27.000000 pypi-version-0.2.0/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2019-03-28 10:10:32.000000 pypi-version-0.2.0/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       83 2019-04-30 16:14:10.000000 pypi-version-0.2.0/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    16711 2019-04-30 16:14:27.000000 pypi-version-0.2.0/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    13280 2019-04-30 16:14:10.000000 pypi-version-0.2.0/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       22 2019-04-21 20:41:50.000000 pypi-version-0.2.0/pypi_version/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     2305 2019-04-30 16:14:10.000000 pypi-version-0.2.0/pypi_version/cis.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1311 2019-04-21 20:08:17.000000 pypi-version-0.2.0/pypi_version/cli.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     2139 2019-04-21 20:08:17.000000 pypi-version-0.2.0/pypi_version/config.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      464 2019-04-30 16:14:10.000000 pypi-version-0.2.0/pypi_version/constants.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      367 2019-04-06 14:34:56.000000 pypi-version-0.2.0/pypi_version/errors.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     2097 2019-04-30 16:14:10.000000 pypi-version-0.2.0/pypi_version/main.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      497 2019-04-21 20:08:17.000000 pypi-version-0.2.0/pypi_version/utils.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    16711 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      610 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       55 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/entry_points.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       57 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       19 2019-04-30 16:14:27.000000 pypi-version-0.2.0/pypi_version.egg-info/top_level.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      246 2019-04-30 16:14:10.000000 pypi-version-0.2.0/requirements-dev.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       57 2019-04-21 20:08:17.000000 pypi-version-0.2.0/requirements.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      358 2019-04-30 16:14:27.000000 pypi-version-0.2.0/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1248 2019-04-30 16:14:10.000000 pypi-version-0.2.0/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:27.000000 pypi-version-0.2.0/tests/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-06 14:34:56.000000 pypi-version-0.2.0/tests/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1023 2019-04-30 16:14:10.000000 pypi-version-0.2.0/tests/conftest.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:27.000000 pypi-version-0.2.0/tests/main/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2019-04-30 16:14:10.000000 pypi-version-0.2.0/tests/main/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      968 2019-04-30 16:14:10.000000 pypi-version-0.2.0/tests/main/test_package_version.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5389 2019-04-30 16:14:10.000000 pypi-version-0.2.0/tests/main/test_pull_request.py
```

### Comparing `pypi-version-0.1.0/LICENSE` & `pypi-version-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi-version-0.1.0/PKG-INFO` & `pypi-version-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-version
-Version: 0.1.0
+Version: 0.2.0
 Summary: Check if you haven't forgotten to bump the PyPi package version number before you merge a release pull request.
 Home-page: https://github.com/dmytrostriletskyi/pypi-version
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Description: # pypi-version
         
@@ -14,137 +14,102 @@
         [![codecov](https://codecov.io/gh/dmytrostriletskyi/pypi-version/branch/develop/graph/badge.svg)](https://codecov.io/gh/dmytrostriletskyi/pypi-version)
         
         [![Downloads](https://pepy.tech/badge/pypi-version)](https://pepy.tech/project/pypi-version)
         [![PyPI license](https://img.shields.io/pypi/l/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
         
           * [Getting started](#getting-started)
-            * [What is pypi-version](#what-is-pypi-version)
-              * [Gitflow workflow](#gitflow-workflow)
-              * [Upload to PyPi](#upload-to-pypi)
-              * [Motivation](#motivation)
             * [How to install](#how-to-install)
+            * [What is pypi-version](#what-is-pypi-version)
+            * [Motivation](#motivation)
+            * [Examples](#examples)
           * [Usage](#usage)
             * [Command line interface](#command-line-interface)
             * [Configuration file](#configuration-file)
+            * [Continuous integration services](#continuous-integration-services)
+              * [Travis-CI](#travis-ci)
+              * [CircleCI](#circleci)
           * [Contributing](#contributing)
+          * [References](#references)
+            * [Python package](#python-package)
+            * [Gitflow workflow](#gitflow-workflow)
+            * [Upload to PyPi](#upload-to-pypi)
+            * [Continuous integration services](#references-continuous-integration-services)
         
         ## Getting started
         
+        ### How to install
+        
+        Install the `pypi-version` with the following command using `pip3`:
+        
+        ```bash
+        $ pip3 install pypi-version
+        ```
+        
         ### What is pypi-version
         
         ``pypi-version`` checks if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
         pull request. 
         
         It would be useful if you:
         
         * develop [Python package](https://packaging.python.org/overview/),
         * follow [Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow),
         * upload package to the [Python Package Index (PyPi)](https://pypi.org/),
-        * use the following continuous integration services: [Travis CI](https://travis-ci.com/dashboard).
+        * use the following continuous integration services: [Travis-CI](https://travis-ci.com), [CircleCI](https://circleci.com)
         
-        #### Python package
-        
-        `Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
-        you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+        If you do not know these concepts, go ahead to the [references section](https://github.com/dmytrostriletskyi/pypi-version/tree/develop#references) first. After, start reading from the next section.
         
-        #### Gitflow workflow
-        
-        Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
-        
-        <img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
-        
-        So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request (from `develop` to `master`) to new features and bumped version numbers become to the release branch together.
-        
-        ![Example of the release pull request](https://habrastorage.org/webt/5c/xw/_0/5cxw_0splygaifsyxlur3cxupx0.png)
-        
-        As you illustrated above, there is a pull request from `develop` branch to `master` branch. `develop` branch contains 
-        a couple of features and the last commit is bumping the version commit.
-        
-        #### Upload to PyPi
-        
-        When you features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
-        
-        Being in the root of you project,
+        ### Motivation
         
-        ```
-        package
-         |
-         - ...
-         - source
-         - README.md
-         - setup.py
-         ...
-        ```
-        
-        you do the following command:
+        `Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
+        Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
+        So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
+        you develop the package locally and alone, you just modify the version number and upload it again. But if you 
+        develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
+        services — then you should create separated pull request to bump the version, the resources and time you will spend 
+        on it are increasing in few times. The cost of the mistake is high.
         
-        ```
-        $ python3 setup.py sdist
-        $ twine upload dist/*
-        ```
+        So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow your pull request to be merged if you forget to increase the version.
         
-        And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+        ### Examples
         
-        <img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+        There is the test repository of the ``Python package`` that has integrated `pypi-version` — [test-pypi-version-travis-ci](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci). It uses `Travis CI` as continuous integration service.
         
-        #### Continuous integration services
+        It contains:
         
-        Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
-        For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
-        of `Python`. The configuration file example for `Travis CI` is presented below.
+        * `develop` and `master` branches,
+        * `master` branch contains file [setup.py where version is 0.1.0](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/setup.py#L7),
         
-        ```yml
-        language: python
+        ![Version number in the setup.py](https://habrastorage.org/webt/du/wa/ox/duwaox015d_cim8_wd58gvkmem0.png)
         
-        python:
-          - "3.4"
-          - "3.5"
-          - "3.6"
-          - "3.7-dev"
+        * according to the version number in the `master` branch (release branch), package is [uploaded to the PyPi with version 0.1.0](https://pypi.org/project/test-pypi-version-travis-ci/),
         
-        install:
-          - pip install -r requirements-dev.txt
-          - pip install -r requirements-tests.txt
+        ![Version number on the PyPi](https://habrastorage.org/webt/q_/qb/fz/q_qbfzof0fdbg-thoq-l7y4bizi.png)
         
-        script:
-          - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
-          - radon cc accessify -nb --total-average
-          - isort -rc accessify --diff && isort -rc tests --diff
-          - flake8 accessify
-          - coverage run -m pytest -vv tests
+        * there is a [pull request from develop branch to master branch](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1) — it is a release pull request that intend increasing of the version number,
         
-        after_success:
-          - coverage report -m && coverage xml
-          - bash <(curl -s https://codecov.io/bash)
-        ```
+        ![Release pull request](https://habrastorage.org/webt/bo/1k/by/bo1kbyddvba5lvlhtpj9bprhadc.png)
         
-        Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+        * but in the changes [version number in setup.py isn't increased](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1/files#diff-2eeaed663bd0d25b7e608891384b7298R8),
         
-        ![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
+        ![Not increased version number in the setup.py](https://habrastorage.org/webt/yw/o_/iz/ywo_izjqiydy9nyaxfpqbjhtrik.png)
         
-        #### Motivation
+        * that's because [pull request's continuous integration checking](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/builds/107324550) is failed — there is `pypi-version` checking integrated.
         
-        `Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
-        Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
-        So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
-        you develop the package locally and alone, you just modify the version number and upload it again. But if you work 
-        develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
-        services — then you should create separated pull request to bump the version, the resources and time you will spend 
-        on it are increasing in few times. The cost of the mistake is high.
+        ![CI failed](https://habrastorage.org/webt/ou/nm/dp/ounmdpsu45gtdtikovraqpd27cs.png)
         
-        So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow you pull request to be merged if you forget to increase the version.
+        * as configured, there are an [installing of the pypi-version and checking the version by using it](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/.travis.yml),
         
-        ### How to install
+        ![Travis CI configuration file](https://habrastorage.org/webt/2k/wo/yv/2kwoyvxdvvpuj2_fk1ykp2ov5b4.png)
         
-        Install the `pypi-package` with the following command using `pip3`:
+        * as the result, `pypi-version` [checks](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/jobs/190875378#L482) if release pull request's (from `develop` to `master`) changes contain an increasing the ``package version number`` before it will be merged. In the example that is described above there is no increasing the version — 
+        `pypi-version check` is failed. If one of the declared checking in the configuration file is failed — it means pull request continuous integration checking is failed and pull request does not allowed to be merged with wrong version number.
         
-        ```bash
-        $ pip3 install pypi-version
-        ```
+        ![PyPi version checking](https://habrastorage.org/webt/hj/en/k8/hjenk81ytwmjcmmbytthtmlloq8.png)
         
         ## Usage
         
         ### Command line interface
         
         To check if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
         pull request:
@@ -174,65 +139,113 @@
         
         Commands:
           check  Check if you haven't forgotten to bump the PyPi package version.
         ```
         
         ### Configuration file
         
-        `pypi-version` requires a configuration file called `.pypi-verion.yml` to be located in the root of the project:
+        `pypi-version` requires a configuration file called `.pypi-version.yml` to be located in the root of the project:
         
         ```
         package
          |
          - ...
          - source
          - README.md
          - setup.py
-         - .pypi-verion.yml
+         - .pypi-version.yml
          ...
         ```
         
-        The configuration file should contains the section with your `PyPi package` name that is the same with the name in the 
-        `setup.py`:
-         
+        The configuration file should contains:
+        
+        * the section with your `PyPi package name` that is the same with the name in the `setup.py`:
+        
         ```yml
         package:
-          name: pypi-version
+          name: test-pypi-version-travis-ci
         ```
         
-        The configuration file should contains name of the continuous integration service you use. Available options are: `travis`.
+        * name of the continuous integration service you use. Available options are: `travis`.
         
         ```yml
         ci:
           name: travis
         ```
         
-        The configuration file should contains `development` and `release` branch names. In the illustration below configurations
-        means `package version number` will be checked only when you do a pull request from `develop` to `master`.
+        * `development` and `release` branch names. In the configurations which are illustrated below means 
+        `package version number` will be checked only when you do a pull request from `develop` to `master`.
         
         ```yml
         branches:
           development: develop
           release: master
         ```
         
-        The example of the configuration file is:
+        The full example of the configuration file is:
         
         ```yml
         package:
           name: pypi-version
         
         ci:
           name: travis
         
         branches:
           development: develop
           release: master
         ```
         
+        ### Continuous integration services
+        
+        #### Travis-CI
+        
+        The example of the configuration file which install and use `pypi-version`:
+        
+        ```yml
+        language: python
+        
+        python:
+          - "3.6"
+        
+        install:
+          - pip install pypi-version
+        
+        script:
+          - pypi-version check
+        ```
+        
+        The example of the failed build (version hasn't been bumped):
+        
+        ![The example of the Travis-CI failed build](https://habrastorage.org/webt/1p/4o/pk/1p4opk_pzxswouvdd0ooioj8o7w.png)
+        
+        #### CircleCI
+        
+        The example of the configuration file which install and use `pypi-version`:
+        
+        ```yml
+        version: 2
+        jobs:
+          build:
+            docker:
+              - image: circleci/python:3.6.4
+            steps:
+              - checkout
+              - run:
+                  name: Install pypi-version package
+                  command: sudo pip3 install pypi-version
+              - run:
+                  name: Check if PyPi should be bumped
+                  command: sudo -H -E pypi-version check
+        ```
+        
+        The example of the failed build (version hasn't been bumped):
+        
+        ![The example of the CircleCI failed build:](https://habrastorage.org/webt/bf/pq/uh/bfpquh7yta1w-__0yblr7jmbaau.png)
+        
         ## Contributing
         
         Clone the project and install requirements:
         
         ```bash
         $ git clone git@github.com:dmytrostriletskyi/pypi-version.git && cd pypi-version
         $ pip3 install -r requirements.txt
@@ -244,17 +257,99 @@
         
         If you are new for the contribution, please read:
         
         * Read about pull requests — https://help.github.com/en/articles/about-pull-requests
         * Read how to provide pull request — https://help.github.com/en/articles/creating-a-pull-request-from-a-fork
         * Also the useful article about how to contribute — https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/
         
+        ## References
+        
+        ### Python package
+        
+        `Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
+        you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+        
+        ### Gitflow workflow
+        
+        Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
+        
+        <img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
+        
+        So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. 
+        
+        ![Example of the release pull request](https://habrastorage.org/webt/xu/j2/e8/xuj2e8giwaniunm0fnvh9bztb8m.png)
+        
+        According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request. 
+        
+        ![Increase version in setup.pt](https://habrastorage.org/webt/m7/er/rj/m7errjk5h7bkaztm95ibhgjyfai.png)
+        
+        ### Upload to PyPi
+        
+        When your features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
+        
+        Being in the root of you project,
+        
+        ```
+        package
+         |
+         - ...
+         - source
+         - README.md
+         - setup.py
+         ...
+        ```
+        
+        you do the following command:
+        
+        ```
+        $ python3 setup.py sdist
+        $ twine upload dist/*
+        ```
+        
+        And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+        
+        <img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+        
+        <h3 id="references-continuous-integration-services">Continuous integration services</h3>
+        
+        Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
+        For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
+        of `Python`. The configuration file example for `Travis CI` is presented below.
+        
+        ```yml
+        language: python
+        
+        python:
+          - "3.4"
+          - "3.5"
+          - "3.6"
+          - "3.7-dev"
+        
+        install:
+          - pip install -r requirements-dev.txt
+          - pip install -r requirements-tests.txt
+        
+        script:
+          - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
+          - radon cc accessify -nb --total-average
+          - isort -rc accessify --diff && isort -rc tests --diff
+          - flake8 accessify
+          - coverage run -m pytest -vv tests
+        
+        after_success:
+          - coverage report -m && coverage xml
+          - bash <(curl -s https://codecov.io/bash)
+        ```
+        
+        Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+        
+        ![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
+        
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `pypi-version-0.1.0/README.md` & `pypi-version-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,137 +6,102 @@
 [![codecov](https://codecov.io/gh/dmytrostriletskyi/pypi-version/branch/develop/graph/badge.svg)](https://codecov.io/gh/dmytrostriletskyi/pypi-version)
 
 [![Downloads](https://pepy.tech/badge/pypi-version)](https://pepy.tech/project/pypi-version)
 [![PyPI license](https://img.shields.io/pypi/l/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
 
   * [Getting started](#getting-started)
-    * [What is pypi-version](#what-is-pypi-version)
-      * [Gitflow workflow](#gitflow-workflow)
-      * [Upload to PyPi](#upload-to-pypi)
-      * [Motivation](#motivation)
     * [How to install](#how-to-install)
+    * [What is pypi-version](#what-is-pypi-version)
+    * [Motivation](#motivation)
+    * [Examples](#examples)
   * [Usage](#usage)
     * [Command line interface](#command-line-interface)
     * [Configuration file](#configuration-file)
+    * [Continuous integration services](#continuous-integration-services)
+      * [Travis-CI](#travis-ci)
+      * [CircleCI](#circleci)
   * [Contributing](#contributing)
+  * [References](#references)
+    * [Python package](#python-package)
+    * [Gitflow workflow](#gitflow-workflow)
+    * [Upload to PyPi](#upload-to-pypi)
+    * [Continuous integration services](#references-continuous-integration-services)
 
 ## Getting started
 
+### How to install
+
+Install the `pypi-version` with the following command using `pip3`:
+
+```bash
+$ pip3 install pypi-version
+```
+
 ### What is pypi-version
 
 ``pypi-version`` checks if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
 pull request. 
 
 It would be useful if you:
 
 * develop [Python package](https://packaging.python.org/overview/),
 * follow [Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow),
 * upload package to the [Python Package Index (PyPi)](https://pypi.org/),
-* use the following continuous integration services: [Travis CI](https://travis-ci.com/dashboard).
+* use the following continuous integration services: [Travis-CI](https://travis-ci.com), [CircleCI](https://circleci.com)
 
-#### Python package
-
-`Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
-you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+If you do not know these concepts, go ahead to the [references section](https://github.com/dmytrostriletskyi/pypi-version/tree/develop#references) first. After, start reading from the next section.
 
-#### Gitflow workflow
-
-Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
-
-<img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
-
-So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request (from `develop` to `master`) to new features and bumped version numbers become to the release branch together.
-
-![Example of the release pull request](https://habrastorage.org/webt/5c/xw/_0/5cxw_0splygaifsyxlur3cxupx0.png)
-
-As you illustrated above, there is a pull request from `develop` branch to `master` branch. `develop` branch contains 
-a couple of features and the last commit is bumping the version commit.
-
-#### Upload to PyPi
-
-When you features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
-
-Being in the root of you project,
+### Motivation
 
-```
-package
- |
- - ...
- - source
- - README.md
- - setup.py
- ...
-```
-
-you do the following command:
+`Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
+Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
+So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
+you develop the package locally and alone, you just modify the version number and upload it again. But if you 
+develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
+services — then you should create separated pull request to bump the version, the resources and time you will spend 
+on it are increasing in few times. The cost of the mistake is high.
 
-```
-$ python3 setup.py sdist
-$ twine upload dist/*
-```
+So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow your pull request to be merged if you forget to increase the version.
 
-And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+### Examples
 
-<img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+There is the test repository of the ``Python package`` that has integrated `pypi-version` — [test-pypi-version-travis-ci](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci). It uses `Travis CI` as continuous integration service.
 
-#### Continuous integration services
+It contains:
 
-Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
-For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
-of `Python`. The configuration file example for `Travis CI` is presented below.
+* `develop` and `master` branches,
+* `master` branch contains file [setup.py where version is 0.1.0](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/setup.py#L7),
 
-```yml
-language: python
+![Version number in the setup.py](https://habrastorage.org/webt/du/wa/ox/duwaox015d_cim8_wd58gvkmem0.png)
 
-python:
-  - "3.4"
-  - "3.5"
-  - "3.6"
-  - "3.7-dev"
+* according to the version number in the `master` branch (release branch), package is [uploaded to the PyPi with version 0.1.0](https://pypi.org/project/test-pypi-version-travis-ci/),
 
-install:
-  - pip install -r requirements-dev.txt
-  - pip install -r requirements-tests.txt
+![Version number on the PyPi](https://habrastorage.org/webt/q_/qb/fz/q_qbfzof0fdbg-thoq-l7y4bizi.png)
 
-script:
-  - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
-  - radon cc accessify -nb --total-average
-  - isort -rc accessify --diff && isort -rc tests --diff
-  - flake8 accessify
-  - coverage run -m pytest -vv tests
+* there is a [pull request from develop branch to master branch](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1) — it is a release pull request that intend increasing of the version number,
 
-after_success:
-  - coverage report -m && coverage xml
-  - bash <(curl -s https://codecov.io/bash)
-```
+![Release pull request](https://habrastorage.org/webt/bo/1k/by/bo1kbyddvba5lvlhtpj9bprhadc.png)
 
-Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+* but in the changes [version number in setup.py isn't increased](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1/files#diff-2eeaed663bd0d25b7e608891384b7298R8),
 
-![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
+![Not increased version number in the setup.py](https://habrastorage.org/webt/yw/o_/iz/ywo_izjqiydy9nyaxfpqbjhtrik.png)
 
-#### Motivation
+* that's because [pull request's continuous integration checking](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/builds/107324550) is failed — there is `pypi-version` checking integrated.
 
-`Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
-Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
-So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
-you develop the package locally and alone, you just modify the version number and upload it again. But if you work 
-develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
-services — then you should create separated pull request to bump the version, the resources and time you will spend 
-on it are increasing in few times. The cost of the mistake is high.
+![CI failed](https://habrastorage.org/webt/ou/nm/dp/ounmdpsu45gtdtikovraqpd27cs.png)
 
-So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow you pull request to be merged if you forget to increase the version.
+* as configured, there are an [installing of the pypi-version and checking the version by using it](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/.travis.yml),
 
-### How to install
+![Travis CI configuration file](https://habrastorage.org/webt/2k/wo/yv/2kwoyvxdvvpuj2_fk1ykp2ov5b4.png)
 
-Install the `pypi-package` with the following command using `pip3`:
+* as the result, `pypi-version` [checks](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/jobs/190875378#L482) if release pull request's (from `develop` to `master`) changes contain an increasing the ``package version number`` before it will be merged. In the example that is described above there is no increasing the version — 
+`pypi-version check` is failed. If one of the declared checking in the configuration file is failed — it means pull request continuous integration checking is failed and pull request does not allowed to be merged with wrong version number.
 
-```bash
-$ pip3 install pypi-version
-```
+![PyPi version checking](https://habrastorage.org/webt/hj/en/k8/hjenk81ytwmjcmmbytthtmlloq8.png)
 
 ## Usage
 
 ### Command line interface
 
 To check if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
 pull request:
@@ -166,65 +131,113 @@
 
 Commands:
   check  Check if you haven't forgotten to bump the PyPi package version.
 ```
 
 ### Configuration file
 
-`pypi-version` requires a configuration file called `.pypi-verion.yml` to be located in the root of the project:
+`pypi-version` requires a configuration file called `.pypi-version.yml` to be located in the root of the project:
 
 ```
 package
  |
  - ...
  - source
  - README.md
  - setup.py
- - .pypi-verion.yml
+ - .pypi-version.yml
  ...
 ```
 
-The configuration file should contains the section with your `PyPi package` name that is the same with the name in the 
-`setup.py`:
- 
+The configuration file should contains:
+
+* the section with your `PyPi package name` that is the same with the name in the `setup.py`:
+
 ```yml
 package:
-  name: pypi-version
+  name: test-pypi-version-travis-ci
 ```
 
-The configuration file should contains name of the continuous integration service you use. Available options are: `travis`.
+* name of the continuous integration service you use. Available options are: `travis`.
 
 ```yml
 ci:
   name: travis
 ```
 
-The configuration file should contains `development` and `release` branch names. In the illustration below configurations
-means `package version number` will be checked only when you do a pull request from `develop` to `master`.
+* `development` and `release` branch names. In the configurations which are illustrated below means 
+`package version number` will be checked only when you do a pull request from `develop` to `master`.
 
 ```yml
 branches:
   development: develop
   release: master
 ```
 
-The example of the configuration file is:
+The full example of the configuration file is:
 
 ```yml
 package:
   name: pypi-version
 
 ci:
   name: travis
 
 branches:
   development: develop
   release: master
 ```
 
+### Continuous integration services
+
+#### Travis-CI
+
+The example of the configuration file which install and use `pypi-version`:
+
+```yml
+language: python
+
+python:
+  - "3.6"
+
+install:
+  - pip install pypi-version
+
+script:
+  - pypi-version check
+```
+
+The example of the failed build (version hasn't been bumped):
+
+![The example of the Travis-CI failed build](https://habrastorage.org/webt/1p/4o/pk/1p4opk_pzxswouvdd0ooioj8o7w.png)
+
+#### CircleCI
+
+The example of the configuration file which install and use `pypi-version`:
+
+```yml
+version: 2
+jobs:
+  build:
+    docker:
+      - image: circleci/python:3.6.4
+    steps:
+      - checkout
+      - run:
+          name: Install pypi-version package
+          command: sudo pip3 install pypi-version
+      - run:
+          name: Check if PyPi should be bumped
+          command: sudo -H -E pypi-version check
+```
+
+The example of the failed build (version hasn't been bumped):
+
+![The example of the CircleCI failed build:](https://habrastorage.org/webt/bf/pq/uh/bfpquh7yta1w-__0yblr7jmbaau.png)
+
 ## Contributing
 
 Clone the project and install requirements:
 
 ```bash
 $ git clone git@github.com:dmytrostriletskyi/pypi-version.git && cd pypi-version
 $ pip3 install -r requirements.txt
@@ -235,7 +248,90 @@
 When you will make changes, ensure your code pass [the checkers](https://github.com/dmytrostriletskyi/pypi-version/blob/develop/.travis.yml#L15) and is covered by tests using [pytest](https://docs.pytest.org/en/latest).
 
 If you are new for the contribution, please read:
 
 * Read about pull requests — https://help.github.com/en/articles/about-pull-requests
 * Read how to provide pull request — https://help.github.com/en/articles/creating-a-pull-request-from-a-fork
 * Also the useful article about how to contribute — https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/
+
+## References
+
+### Python package
+
+`Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
+you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+
+### Gitflow workflow
+
+Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
+
+<img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
+
+So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. 
+
+![Example of the release pull request](https://habrastorage.org/webt/xu/j2/e8/xuj2e8giwaniunm0fnvh9bztb8m.png)
+
+According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request. 
+
+![Increase version in setup.pt](https://habrastorage.org/webt/m7/er/rj/m7errjk5h7bkaztm95ibhgjyfai.png)
+
+### Upload to PyPi
+
+When your features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
+
+Being in the root of you project,
+
+```
+package
+ |
+ - ...
+ - source
+ - README.md
+ - setup.py
+ ...
+```
+
+you do the following command:
+
+```
+$ python3 setup.py sdist
+$ twine upload dist/*
+```
+
+And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+
+<img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+
+<h3 id="references-continuous-integration-services">Continuous integration services</h3>
+
+Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
+For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
+of `Python`. The configuration file example for `Travis CI` is presented below.
+
+```yml
+language: python
+
+python:
+  - "3.4"
+  - "3.5"
+  - "3.6"
+  - "3.7-dev"
+
+install:
+  - pip install -r requirements-dev.txt
+  - pip install -r requirements-tests.txt
+
+script:
+  - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
+  - radon cc accessify -nb --total-average
+  - isort -rc accessify --diff && isort -rc tests --diff
+  - flake8 accessify
+  - coverage run -m pytest -vv tests
+
+after_success:
+  - coverage report -m && coverage xml
+  - bash <(curl -s https://codecov.io/bash)
+```
+
+Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+
+![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
```

### Comparing `pypi-version-0.1.0/pypi_version/cli.py` & `pypi-version-0.2.0/pypi_version/cli.py`

 * *Files identical despite different names*

### Comparing `pypi-version-0.1.0/pypi_version/config.py` & `pypi-version-0.2.0/pypi_version/config.py`

 * *Files identical despite different names*

### Comparing `pypi-version-0.1.0/pypi_version/main.py` & `pypi-version-0.2.0/pypi_version/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Provide implementation of the PyPi version checking.
 """
-import os
-
 import requests
 from accessify import private
 
+from pypi_version.cis import (
+    CircleCi,
+    TravisCi,
+)
 from pypi_version.constants import (
     FETCH_PYPI_PACKAGE_URL,
     HTTP_STATUS_OK,
-    TravisCi,
 )
 from pypi_version.errors import (
     NOT_SUPPORTED_CONTINUOUS_INTEGRATION_ERROR_MESSAGE,
     NotSupportedContinuousIntegrationError,
 )
 
 
@@ -46,36 +47,36 @@
 
     @private
     @staticmethod
     def get_ci(name):
         """
         Get continuous integration class with related data.
         """
-        if name == TravisCi.NAME:
-            return TravisCi
+        if name == TravisCi().name:
+            return TravisCi()
+
+        if name == CircleCi().name:
+            return CircleCi()
 
         raise NotSupportedContinuousIntegrationError(
             NOT_SUPPORTED_CONTINUOUS_INTEGRATION_ERROR_MESSAGE.format(ci_name=name),
         )
 
     def is_for_check(self, ci_name, develop_branch, release_branch):
         """
-        Check if current pull request match pull request data in the configuration file.
-
-        If environment variable of pull request branch you want merge to is empty, it means
-        continuous integration run the job for the just branch, not pull request.
+        Check if current pull request matches pull request configurations in the configuration file.
 
-        If current pull request branches matches pull request branches in the configuration file — return true,
-        else — return false.
+        If current pull request configurations matches pull request configurations in the configuration file,
+        then return true, else return false.
         """
         ci = self.get_ci(name=ci_name)
 
-        if not os.environ.get(ci.ENV_VARIABLE_PR_BRANCH_TO_NAME):
+        if not ci.is_pull_request():
             return False
 
-        if release_branch != os.environ.get(ci.ENV_VARIABLE_PR_BRANCH_TO_NAME):
+        if develop_branch != ci.pr_branch_from_name:
             return False
 
-        if develop_branch != os.environ.get(ci.ENV_VARIABLE_PR_BRANCH_FROM_NAME):
+        if release_branch != ci.pr_branch_to_name:
             return False
 
         return True
```

### Comparing `pypi-version-0.1.0/pypi_version.egg-info/PKG-INFO` & `pypi-version-0.2.0/pypi_version.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-version
-Version: 0.1.0
+Version: 0.2.0
 Summary: Check if you haven't forgotten to bump the PyPi package version number before you merge a release pull request.
 Home-page: https://github.com/dmytrostriletskyi/pypi-version
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Description: # pypi-version
         
@@ -14,137 +14,102 @@
         [![codecov](https://codecov.io/gh/dmytrostriletskyi/pypi-version/branch/develop/graph/badge.svg)](https://codecov.io/gh/dmytrostriletskyi/pypi-version)
         
         [![Downloads](https://pepy.tech/badge/pypi-version)](https://pepy.tech/project/pypi-version)
         [![PyPI license](https://img.shields.io/pypi/l/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pypi-version.svg)](https://pypi.python.org/pypi/pypi-version/)
         
           * [Getting started](#getting-started)
-            * [What is pypi-version](#what-is-pypi-version)
-              * [Gitflow workflow](#gitflow-workflow)
-              * [Upload to PyPi](#upload-to-pypi)
-              * [Motivation](#motivation)
             * [How to install](#how-to-install)
+            * [What is pypi-version](#what-is-pypi-version)
+            * [Motivation](#motivation)
+            * [Examples](#examples)
           * [Usage](#usage)
             * [Command line interface](#command-line-interface)
             * [Configuration file](#configuration-file)
+            * [Continuous integration services](#continuous-integration-services)
+              * [Travis-CI](#travis-ci)
+              * [CircleCI](#circleci)
           * [Contributing](#contributing)
+          * [References](#references)
+            * [Python package](#python-package)
+            * [Gitflow workflow](#gitflow-workflow)
+            * [Upload to PyPi](#upload-to-pypi)
+            * [Continuous integration services](#references-continuous-integration-services)
         
         ## Getting started
         
+        ### How to install
+        
+        Install the `pypi-version` with the following command using `pip3`:
+        
+        ```bash
+        $ pip3 install pypi-version
+        ```
+        
         ### What is pypi-version
         
         ``pypi-version`` checks if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
         pull request. 
         
         It would be useful if you:
         
         * develop [Python package](https://packaging.python.org/overview/),
         * follow [Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow),
         * upload package to the [Python Package Index (PyPi)](https://pypi.org/),
-        * use the following continuous integration services: [Travis CI](https://travis-ci.com/dashboard).
+        * use the following continuous integration services: [Travis-CI](https://travis-ci.com), [CircleCI](https://circleci.com)
         
-        #### Python package
-        
-        `Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
-        you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+        If you do not know these concepts, go ahead to the [references section](https://github.com/dmytrostriletskyi/pypi-version/tree/develop#references) first. After, start reading from the next section.
         
-        #### Gitflow workflow
-        
-        Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
-        
-        <img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
-        
-        So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request (from `develop` to `master`) to new features and bumped version numbers become to the release branch together.
-        
-        ![Example of the release pull request](https://habrastorage.org/webt/5c/xw/_0/5cxw_0splygaifsyxlur3cxupx0.png)
-        
-        As you illustrated above, there is a pull request from `develop` branch to `master` branch. `develop` branch contains 
-        a couple of features and the last commit is bumping the version commit.
-        
-        #### Upload to PyPi
-        
-        When you features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
-        
-        Being in the root of you project,
+        ### Motivation
         
-        ```
-        package
-         |
-         - ...
-         - source
-         - README.md
-         - setup.py
-         ...
-        ```
-        
-        you do the following command:
+        `Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
+        Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
+        So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
+        you develop the package locally and alone, you just modify the version number and upload it again. But if you 
+        develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
+        services — then you should create separated pull request to bump the version, the resources and time you will spend 
+        on it are increasing in few times. The cost of the mistake is high.
         
-        ```
-        $ python3 setup.py sdist
-        $ twine upload dist/*
-        ```
+        So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow your pull request to be merged if you forget to increase the version.
         
-        And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+        ### Examples
         
-        <img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+        There is the test repository of the ``Python package`` that has integrated `pypi-version` — [test-pypi-version-travis-ci](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci). It uses `Travis CI` as continuous integration service.
         
-        #### Continuous integration services
+        It contains:
         
-        Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
-        For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
-        of `Python`. The configuration file example for `Travis CI` is presented below.
+        * `develop` and `master` branches,
+        * `master` branch contains file [setup.py where version is 0.1.0](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/setup.py#L7),
         
-        ```yml
-        language: python
+        ![Version number in the setup.py](https://habrastorage.org/webt/du/wa/ox/duwaox015d_cim8_wd58gvkmem0.png)
         
-        python:
-          - "3.4"
-          - "3.5"
-          - "3.6"
-          - "3.7-dev"
+        * according to the version number in the `master` branch (release branch), package is [uploaded to the PyPi with version 0.1.0](https://pypi.org/project/test-pypi-version-travis-ci/),
         
-        install:
-          - pip install -r requirements-dev.txt
-          - pip install -r requirements-tests.txt
+        ![Version number on the PyPi](https://habrastorage.org/webt/q_/qb/fz/q_qbfzof0fdbg-thoq-l7y4bizi.png)
         
-        script:
-          - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
-          - radon cc accessify -nb --total-average
-          - isort -rc accessify --diff && isort -rc tests --diff
-          - flake8 accessify
-          - coverage run -m pytest -vv tests
+        * there is a [pull request from develop branch to master branch](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1) — it is a release pull request that intend increasing of the version number,
         
-        after_success:
-          - coverage report -m && coverage xml
-          - bash <(curl -s https://codecov.io/bash)
-        ```
+        ![Release pull request](https://habrastorage.org/webt/bo/1k/by/bo1kbyddvba5lvlhtpj9bprhadc.png)
         
-        Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+        * but in the changes [version number in setup.py isn't increased](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/pull/1/files#diff-2eeaed663bd0d25b7e608891384b7298R8),
         
-        ![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
+        ![Not increased version number in the setup.py](https://habrastorage.org/webt/yw/o_/iz/ywo_izjqiydy9nyaxfpqbjhtrik.png)
         
-        #### Motivation
+        * that's because [pull request's continuous integration checking](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/builds/107324550) is failed — there is `pypi-version` checking integrated.
         
-        `Python packages` have version number such as `0.1.0` or `1.3.3`. `Python packages` commonly are uploaded to `PyPi`.
-        Sometimes after adding new functionality to your package you forget to increase the version number of the package. 
-        So when you try to upload it, you get the error message `Package version number already in use`. It is okay if 
-        you develop the package locally and alone, you just modify the version number and upload it again. But if you work 
-        develop the package using particular development flow such as `Gitflow workflow` and continuous integration 
-        services — then you should create separated pull request to bump the version, the resources and time you will spend 
-        on it are increasing in few times. The cost of the mistake is high.
+        ![CI failed](https://habrastorage.org/webt/ou/nm/dp/ounmdpsu45gtdtikovraqpd27cs.png)
         
-        So if you integrate the `pypi-version` to your continuous integration service by checking the version using simple command line tool, it will `never` allow you pull request to be merged if you forget to increase the version.
+        * as configured, there are an [installing of the pypi-version and checking the version by using it](https://github.com/dmytrostriletskyi/test-pypi-version-travis-ci/blob/master/.travis.yml),
         
-        ### How to install
+        ![Travis CI configuration file](https://habrastorage.org/webt/2k/wo/yv/2kwoyvxdvvpuj2_fk1ykp2ov5b4.png)
         
-        Install the `pypi-package` with the following command using `pip3`:
+        * as the result, `pypi-version` [checks](https://travis-ci.com/dmytrostriletskyi/test-pypi-version-travis-ci/jobs/190875378#L482) if release pull request's (from `develop` to `master`) changes contain an increasing the ``package version number`` before it will be merged. In the example that is described above there is no increasing the version — 
+        `pypi-version check` is failed. If one of the declared checking in the configuration file is failed — it means pull request continuous integration checking is failed and pull request does not allowed to be merged with wrong version number.
         
-        ```bash
-        $ pip3 install pypi-version
-        ```
+        ![PyPi version checking](https://habrastorage.org/webt/hj/en/k8/hjenk81ytwmjcmmbytthtmlloq8.png)
         
         ## Usage
         
         ### Command line interface
         
         To check if you haven't forgotten to bump the ``PyPi package version number`` before you merge a release 
         pull request:
@@ -174,65 +139,113 @@
         
         Commands:
           check  Check if you haven't forgotten to bump the PyPi package version.
         ```
         
         ### Configuration file
         
-        `pypi-version` requires a configuration file called `.pypi-verion.yml` to be located in the root of the project:
+        `pypi-version` requires a configuration file called `.pypi-version.yml` to be located in the root of the project:
         
         ```
         package
          |
          - ...
          - source
          - README.md
          - setup.py
-         - .pypi-verion.yml
+         - .pypi-version.yml
          ...
         ```
         
-        The configuration file should contains the section with your `PyPi package` name that is the same with the name in the 
-        `setup.py`:
-         
+        The configuration file should contains:
+        
+        * the section with your `PyPi package name` that is the same with the name in the `setup.py`:
+        
         ```yml
         package:
-          name: pypi-version
+          name: test-pypi-version-travis-ci
         ```
         
-        The configuration file should contains name of the continuous integration service you use. Available options are: `travis`.
+        * name of the continuous integration service you use. Available options are: `travis`.
         
         ```yml
         ci:
           name: travis
         ```
         
-        The configuration file should contains `development` and `release` branch names. In the illustration below configurations
-        means `package version number` will be checked only when you do a pull request from `develop` to `master`.
+        * `development` and `release` branch names. In the configurations which are illustrated below means 
+        `package version number` will be checked only when you do a pull request from `develop` to `master`.
         
         ```yml
         branches:
           development: develop
           release: master
         ```
         
-        The example of the configuration file is:
+        The full example of the configuration file is:
         
         ```yml
         package:
           name: pypi-version
         
         ci:
           name: travis
         
         branches:
           development: develop
           release: master
         ```
         
+        ### Continuous integration services
+        
+        #### Travis-CI
+        
+        The example of the configuration file which install and use `pypi-version`:
+        
+        ```yml
+        language: python
+        
+        python:
+          - "3.6"
+        
+        install:
+          - pip install pypi-version
+        
+        script:
+          - pypi-version check
+        ```
+        
+        The example of the failed build (version hasn't been bumped):
+        
+        ![The example of the Travis-CI failed build](https://habrastorage.org/webt/1p/4o/pk/1p4opk_pzxswouvdd0ooioj8o7w.png)
+        
+        #### CircleCI
+        
+        The example of the configuration file which install and use `pypi-version`:
+        
+        ```yml
+        version: 2
+        jobs:
+          build:
+            docker:
+              - image: circleci/python:3.6.4
+            steps:
+              - checkout
+              - run:
+                  name: Install pypi-version package
+                  command: sudo pip3 install pypi-version
+              - run:
+                  name: Check if PyPi should be bumped
+                  command: sudo -H -E pypi-version check
+        ```
+        
+        The example of the failed build (version hasn't been bumped):
+        
+        ![The example of the CircleCI failed build:](https://habrastorage.org/webt/bf/pq/uh/bfpquh7yta1w-__0yblr7jmbaau.png)
+        
         ## Contributing
         
         Clone the project and install requirements:
         
         ```bash
         $ git clone git@github.com:dmytrostriletskyi/pypi-version.git && cd pypi-version
         $ pip3 install -r requirements.txt
@@ -244,17 +257,99 @@
         
         If you are new for the contribution, please read:
         
         * Read about pull requests — https://help.github.com/en/articles/about-pull-requests
         * Read how to provide pull request — https://help.github.com/en/articles/creating-a-pull-request-from-a-fork
         * Also the useful article about how to contribute — https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/
         
+        ## References
+        
+        ### Python package
+        
+        `Python package` is redistributed and reused couple of the `Python` scripts. They exist to solve the typical problems. So if
+        you have common problem in your project — instead of writing own code and spend a time for it, use the package that already have required functionality. The examples of `Python packages` you should know are [requests](https://github.com/kennethreitz/requests) and [Django](https://github.com/django/django). 
+        
+        ### Gitflow workflow
+        
+        Instead of a single `master` branch, this workflow uses two branches to record the history of the project. The `master` branch stores the official release history, and the `develop` branch serves as an integration branch for features.
+        
+        <img src="https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=le" width="700" height="300">
+        
+        So when you complete the feature, you open the pull request from `feature` branch to the `develop` branch. When you complete the bunch of features, you open the pull request from `develop` branch to `master` branch which are going to merge this bunch of features that means you do new release. 
+        
+        ![Example of the release pull request](https://habrastorage.org/webt/xu/j2/e8/xuj2e8giwaniunm0fnvh9bztb8m.png)
+        
+        According to the changes that contains new features, you should increase your version number (e.g. from `1.0.0` to `1.1.0`) in the file called `setup.py` in the same pull request. 
+        
+        ![Increase version in setup.pt](https://habrastorage.org/webt/m7/er/rj/m7errjk5h7bkaztm95ibhgjyfai.png)
+        
+        ### Upload to PyPi
+        
+        When your features with increased version number have been merged to the `master` branch, you are going to upload your source code to the `Python Package Index`. 
+        
+        Being in the root of you project,
+        
+        ```
+        package
+         |
+         - ...
+         - source
+         - README.md
+         - setup.py
+         ...
+        ```
+        
+        you do the following command:
+        
+        ```
+        $ python3 setup.py sdist
+        $ twine upload dist/*
+        ```
+        
+        And if you haven't forgotten to bump the ``PyPi package version number``, the upload is successful. 
+        
+        <img src="https://habrastorage.org/webt/55/pk/jn/55pkjnoezzvidqcyordvtyyhgw0.png" width="700" height="300">
+        
+        <h3 id="references-continuous-integration-services">Continuous integration services</h3>
+        
+        Continuous integration services are useful when you want add some robotic checking for your pull request changes. 
+        For instance, you can run checking code style with [flake8](https://github.com/PyCQA/flake8) and run tests with [pytest](https://github.com/pytest-dev/pytest) to check your changes does not break existing functionality on the few version 
+        of `Python`. The configuration file example for `Travis CI` is presented below.
+        
+        ```yml
+        language: python
+        
+        python:
+          - "3.4"
+          - "3.5"
+          - "3.6"
+          - "3.7-dev"
+        
+        install:
+          - pip install -r requirements-dev.txt
+          - pip install -r requirements-tests.txt
+        
+        script:
+          - cat requirements-tests.txt requirements-dev.txt | safety check --stdin
+          - radon cc accessify -nb --total-average
+          - isort -rc accessify --diff && isort -rc tests --diff
+          - flake8 accessify
+          - coverage run -m pytest -vv tests
+        
+        after_success:
+          - coverage report -m && coverage xml
+          - bash <(curl -s https://codecov.io/bash)
+        ```
+        
+        Each pull request the checking report will be presented. By clicking on the `details` you will see full report.
+        
+        ![Pull request checks](https://habrastorage.org/webt/jj/ux/1b/jjux1b8mezmnnf8g8zq3elr9fv8.png)
+        
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `pypi-version-0.1.0/setup.py` & `pypi-version-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open('README.md', 'r') as read_me:
     long_description = read_me.read()
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.1.0',
+    version='0.2.0',
     name='pypi-version',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/pypi-version',
     license='MIT',
     author='Dmytro Striletskyi',
@@ -30,14 +30,13 @@
         ]
     },
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
 
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
 )
```

