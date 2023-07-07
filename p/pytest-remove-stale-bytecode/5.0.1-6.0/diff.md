# Comparing `tmp/pytest-remove-stale-bytecode-5.0.1.tar.gz` & `tmp/pytest-remove-stale-bytecode-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-remove-stale-bytecode-5.0.1.tar", last modified: Wed Mar  4 12:49:51 2020, max compression
+gzip compressed data, was "pytest-remove-stale-bytecode-6.0.tar", last modified: Fri Jul  7 14:11:19 2023, max compression
```

## Comparing `pytest-remove-stale-bytecode-5.0.1.tar` & `pytest-remove-stale-bytecode-6.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/
--rw-r--r--   0 mac        (501) staff       (20)       96 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)      212 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/.travis.yml
--rw-r--r--   0 mac        (501) staff       (20)     1464 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)     1070 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)      197 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)     5346 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1625 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     1512 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/plugin.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     5346 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      487 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       41 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       18 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       67 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1800 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/setup.py
--rw-r--r--   0 mac        (501) staff       (20)     3834 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/test_plugin.py
--rw-r--r--   0 mac        (501) staff       (20)      637 2020-03-04 12:49:51.000000 pytest-remove-stale-bytecode-5.0.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-07 14:11:19.355296 pytest-remove-stale-bytecode-6.0/
+-rw-r--r--   0 mac        (513) staff       (20)      113 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)     1762 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1070 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      197 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     4631 2023-07-07 14:11:19.355428 pytest-remove-stale-bytecode-6.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1623 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1512 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/plugin.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-07 14:11:19.354971 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     4631 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      475 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)       40 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       18 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-07 14:11:19.000000 pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-07 14:11:19.355807 pytest-remove-stale-bytecode-6.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1838 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/setup.py
+-rw-r--r--   0 mac        (513) staff       (20)     3849 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/test_plugin.py
+-rw-r--r--   0 mac        (513) staff       (20)      402 2023-07-07 14:11:18.000000 pytest-remove-stale-bytecode-6.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/CHANGES.rst` & `pytest-remove-stale-bytecode-6.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,34 @@
 =======
 CHANGES
 =======
 
 
+6.0 (2023-07-07)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 3.5 and 3.6.
+
+Features
+--------
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Update tests to ``pytest >= 6.2``.
+
+Other changes
+-------------
+
+- Use Github actions as CI.
+
+
+
 5.0.1 (2020-03-04)
 ==================
 
 - Calling `pytest --help` no longer breaks when this plug-in is installed.
 
 
 5.0 (2020-01-17)
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/LICENSE.txt` & `pytest-remove-stale-bytecode-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-remove-stale-bytecode-5.0.1/PKG-INFO` & `pytest-remove-stale-bytecode-6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,185 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-remove-stale-bytecode
-Version: 5.0.1
+Version: 6.0
 Summary: py.test plugin to remove stale byte code files.
 Home-page: https://github.com/gocept/pytest-remove-stale-bytecode/
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: MIT
-Description: =======================================
-        py.test plugin to remove stale bytecode
-        =======================================
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-remove-stale-bytecode.svg
-            :target: https://pypi.org/project/pytest-remove-stale-bytecode/
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pytest-remove-stale-bytecode.svg
-            :target: https://pypi.org/project/pytest-remove-stale-bytecode/
-        
-        .. image:: https://travis-ci.com/gocept/pytest-remove-stale-bytecode.svg?branch=master
-            :target: https://travis-ci.com/gocept/pytest-remove-stale-bytecode
-        
-        .. image:: https://dev.azure.com/gocept/pytest-remove-stale-bytecode/_apis/build/status/gocept.pytest-remove-stale-bytecode?branchName=master
-            :target: https://dev.azure.com/gocept/pytest-remove-stale-bytecode
-        
-        
-        Description
-        ===========
-        
-        This plugin removes all stale bytecode files before running tests. This makes
-        sure that Python modules -- whose source was deleted -- are not accidentally visible
-        to the test runner anymore due to a left-over bytecode file (``*.pyc``,
-        ``*.pyo``).
-        
-        Usage
-        =====
-        
-        To use this plugin you just have to install it, so it is accessible by the
-        pytest you are using:
-        
-        + If you are using `buildout`, add ``pytest-remove-stale-bytecode`` to the
-          buildout section of your pytest runner.
-        
-        + If you are using `pip` add it to your test requirements.
-        
-        Per default, there is no output generated, but if pytest is invoked in verbose
-        mode (``-v``), information about the deleted files is printed.
-        
-        This plugin was inspired by a feature of `zope.testrunner`_.
-        
-        .. _`zope.testrunner`: https://pypi.python.org/pypi/zope.testrunner
-        
-        
-        =======
-        CHANGES
-        =======
-        
-        
-        5.0.1 (2020-03-04)
-        ==================
-        
-        - Calling `pytest --help` no longer breaks when this plug-in is installed.
-        
-        
-        5.0 (2020-01-17)
-        ================
-        
-        Backwards incompatible changes
-        ------------------------------
-        
-        - Drop support for Python 2.7 and PyPy2.
-        
-        Features
-        --------
-        
-        - Add support for Python 3.8.
-        
-        - Migrate to Github.
-        
-        - Improve for new pytest versions.
-        
-        Bug fixes
-        ---------
-        
-        - Fix problems when running tests jobs in parallel.
-          (`#2 <https://github.com/gocept/pytest-remove-stale-bytecode/issues/2>`_)
-        
-        
-        4.0 (2019-09-13)
-        ================
-        
-        Backwards incompatible changes
-        ------------------------------
-        
-        - Drop support for Python 3.4.
-        
-        Features
-        --------
-        
-        - Make work with py.test >=3.10 again.
-        
-        - Add support for Python 3.7.
-        
-        
-        3.0.1 (2019-03-21)
-        ==================
-        
-        - This plug-in only works in py.test < version 3.10.
-          It is broken since the merge of
-          `pytest-dev/pytest#4250 <https://github.com/pytest-dev/pytest/pull/4250>`_
-        
-        - Drop support for Python 3.3.
-        
-        
-        3.0 (2017-05-12)
-        ================
-        
-        - Add support for Python 3.6, PyPy2 and PyPy3.
-        
-        - Do not show output by default anymore. It can be turned on with ``-v``
-          option.
-        
-        - Change the license from ZPL to MIT.
-        
-        
-        2.1 (2015-10-01)
-        ================
-        
-        - Also remove bytecode files under Python 3, that end with ``-PYTEST``.
-        
-        
-        2.0 (2015-10-01)
-        ================
-        
-        - Add support for removing byte code files under Python 3.
-        
-        
-        1.0 (2014-10-29)
-        ================
-        
-        - initial release
-        
 Keywords: pytest pyc bytecode artefacts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >= 3.5
+Requires-Python: >= 3.7
+License-File: LICENSE.txt
+
+=======================================
+py.test plugin to remove stale bytecode
+=======================================
+
+.. image:: https://img.shields.io/pypi/v/pytest-remove-stale-bytecode.svg
+    :target: https://pypi.org/project/pytest-remove-stale-bytecode/
+
+.. image:: https://img.shields.io/pypi/pyversions/pytest-remove-stale-bytecode.svg
+    :target: https://pypi.org/project/pytest-remove-stale-bytecode/
+
+.. image:: https://github.com/gocept/pytest-remove-stale-bytecode/workflows/tests/badge.svg
+    :target: https://github.com/gocept/pytest-remove-stale-bytecode/actions?query=workflow%3Atests
+
+
+Description
+===========
+
+This plugin removes stale bytecode files of the packages under test before running tests. This makes
+sure that Python modules -- whose source was deleted -- are not accidentally visible
+to the test runner anymore due to a left-over bytecode file (``*.pyc``,
+``*.pyo``).
+
+.. caution::
+
+   This plug-in only looks into the packages you are testing. If there is a stale bytecode file
+   in another package it does not remove it.
+
+Usage
+=====
+
+To use this plugin you just have to install it, so it is accessible by the
+pytest you are using:
+
++ If you are using `buildout`, add ``pytest-remove-stale-bytecode`` to the
+  buildout section of your pytest runner.
+
++ If you are using `pip` add it to your test requirements.
+
+Per default, there is no output generated, but if pytest is invoked in verbose
+mode (``-v``), information about the deleted files is printed.
+
+This plugin was inspired by a feature of `zope.testrunner`_.
+
+.. _`zope.testrunner`: https://pypi.python.org/pypi/zope.testrunner
+
+
+=======
+CHANGES
+=======
+
+
+6.0 (2023-07-07)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 3.5 and 3.6.
+
+Features
+--------
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Update tests to ``pytest >= 6.2``.
+
+Other changes
+-------------
+
+- Use Github actions as CI.
+
+
+
+5.0.1 (2020-03-04)
+==================
+
+- Calling `pytest --help` no longer breaks when this plug-in is installed.
+
+
+5.0 (2020-01-17)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 2.7 and PyPy2.
+
+Features
+--------
+
+- Add support for Python 3.8.
+
+- Migrate to Github.
+
+- Improve for new pytest versions.
+
+Bug fixes
+---------
+
+- Fix problems when running tests jobs in parallel.
+  (`#2 <https://github.com/gocept/pytest-remove-stale-bytecode/issues/2>`_)
+
+
+4.0 (2019-09-13)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 3.4.
+
+Features
+--------
+
+- Make work with py.test >=3.10 again.
+
+- Add support for Python 3.7.
+
+
+3.0.1 (2019-03-21)
+==================
+
+- This plug-in only works in py.test < version 3.10.
+  It is broken since the merge of
+  `pytest-dev/pytest#4250 <https://github.com/pytest-dev/pytest/pull/4250>`_
+
+- Drop support for Python 3.3.
+
+
+3.0 (2017-05-12)
+================
+
+- Add support for Python 3.6, PyPy2 and PyPy3.
+
+- Do not show output by default anymore. It can be turned on with ``-v``
+  option.
+
+- Change the license from ZPL to MIT.
+
+
+2.1 (2015-10-01)
+================
+
+- Also remove bytecode files under Python 3, that end with ``-PYTEST``.
+
+
+2.0 (2015-10-01)
+================
+
+- Add support for removing byte code files under Python 3.
+
+
+1.0 (2014-10-29)
+================
+
+- initial release
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/plugin.py` & `pytest-remove-stale-bytecode-6.0/plugin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pkg_resources
 import os
 import os.path
+import pkg_resources
 import sys
 
 
 __version__ = pkg_resources.get_distribution(
     'pytest-remove-stale-bytecode').version
 python_version = '{0.major}{0.minor}'.format(sys.version_info)
 pytest_version = pkg_resources.get_distribution('pytest').version
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/pytest_remove_stale_bytecode.egg-info/PKG-INFO` & `pytest-remove-stale-bytecode-6.0/pytest_remove_stale_bytecode.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,185 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-remove-stale-bytecode
-Version: 5.0.1
+Version: 6.0
 Summary: py.test plugin to remove stale byte code files.
 Home-page: https://github.com/gocept/pytest-remove-stale-bytecode/
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: MIT
-Description: =======================================
-        py.test plugin to remove stale bytecode
-        =======================================
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-remove-stale-bytecode.svg
-            :target: https://pypi.org/project/pytest-remove-stale-bytecode/
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pytest-remove-stale-bytecode.svg
-            :target: https://pypi.org/project/pytest-remove-stale-bytecode/
-        
-        .. image:: https://travis-ci.com/gocept/pytest-remove-stale-bytecode.svg?branch=master
-            :target: https://travis-ci.com/gocept/pytest-remove-stale-bytecode
-        
-        .. image:: https://dev.azure.com/gocept/pytest-remove-stale-bytecode/_apis/build/status/gocept.pytest-remove-stale-bytecode?branchName=master
-            :target: https://dev.azure.com/gocept/pytest-remove-stale-bytecode
-        
-        
-        Description
-        ===========
-        
-        This plugin removes all stale bytecode files before running tests. This makes
-        sure that Python modules -- whose source was deleted -- are not accidentally visible
-        to the test runner anymore due to a left-over bytecode file (``*.pyc``,
-        ``*.pyo``).
-        
-        Usage
-        =====
-        
-        To use this plugin you just have to install it, so it is accessible by the
-        pytest you are using:
-        
-        + If you are using `buildout`, add ``pytest-remove-stale-bytecode`` to the
-          buildout section of your pytest runner.
-        
-        + If you are using `pip` add it to your test requirements.
-        
-        Per default, there is no output generated, but if pytest is invoked in verbose
-        mode (``-v``), information about the deleted files is printed.
-        
-        This plugin was inspired by a feature of `zope.testrunner`_.
-        
-        .. _`zope.testrunner`: https://pypi.python.org/pypi/zope.testrunner
-        
-        
-        =======
-        CHANGES
-        =======
-        
-        
-        5.0.1 (2020-03-04)
-        ==================
-        
-        - Calling `pytest --help` no longer breaks when this plug-in is installed.
-        
-        
-        5.0 (2020-01-17)
-        ================
-        
-        Backwards incompatible changes
-        ------------------------------
-        
-        - Drop support for Python 2.7 and PyPy2.
-        
-        Features
-        --------
-        
-        - Add support for Python 3.8.
-        
-        - Migrate to Github.
-        
-        - Improve for new pytest versions.
-        
-        Bug fixes
-        ---------
-        
-        - Fix problems when running tests jobs in parallel.
-          (`#2 <https://github.com/gocept/pytest-remove-stale-bytecode/issues/2>`_)
-        
-        
-        4.0 (2019-09-13)
-        ================
-        
-        Backwards incompatible changes
-        ------------------------------
-        
-        - Drop support for Python 3.4.
-        
-        Features
-        --------
-        
-        - Make work with py.test >=3.10 again.
-        
-        - Add support for Python 3.7.
-        
-        
-        3.0.1 (2019-03-21)
-        ==================
-        
-        - This plug-in only works in py.test < version 3.10.
-          It is broken since the merge of
-          `pytest-dev/pytest#4250 <https://github.com/pytest-dev/pytest/pull/4250>`_
-        
-        - Drop support for Python 3.3.
-        
-        
-        3.0 (2017-05-12)
-        ================
-        
-        - Add support for Python 3.6, PyPy2 and PyPy3.
-        
-        - Do not show output by default anymore. It can be turned on with ``-v``
-          option.
-        
-        - Change the license from ZPL to MIT.
-        
-        
-        2.1 (2015-10-01)
-        ================
-        
-        - Also remove bytecode files under Python 3, that end with ``-PYTEST``.
-        
-        
-        2.0 (2015-10-01)
-        ================
-        
-        - Add support for removing byte code files under Python 3.
-        
-        
-        1.0 (2014-10-29)
-        ================
-        
-        - initial release
-        
 Keywords: pytest pyc bytecode artefacts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >= 3.5
+Requires-Python: >= 3.7
+License-File: LICENSE.txt
+
+=======================================
+py.test plugin to remove stale bytecode
+=======================================
+
+.. image:: https://img.shields.io/pypi/v/pytest-remove-stale-bytecode.svg
+    :target: https://pypi.org/project/pytest-remove-stale-bytecode/
+
+.. image:: https://img.shields.io/pypi/pyversions/pytest-remove-stale-bytecode.svg
+    :target: https://pypi.org/project/pytest-remove-stale-bytecode/
+
+.. image:: https://github.com/gocept/pytest-remove-stale-bytecode/workflows/tests/badge.svg
+    :target: https://github.com/gocept/pytest-remove-stale-bytecode/actions?query=workflow%3Atests
+
+
+Description
+===========
+
+This plugin removes stale bytecode files of the packages under test before running tests. This makes
+sure that Python modules -- whose source was deleted -- are not accidentally visible
+to the test runner anymore due to a left-over bytecode file (``*.pyc``,
+``*.pyo``).
+
+.. caution::
+
+   This plug-in only looks into the packages you are testing. If there is a stale bytecode file
+   in another package it does not remove it.
+
+Usage
+=====
+
+To use this plugin you just have to install it, so it is accessible by the
+pytest you are using:
+
++ If you are using `buildout`, add ``pytest-remove-stale-bytecode`` to the
+  buildout section of your pytest runner.
+
++ If you are using `pip` add it to your test requirements.
+
+Per default, there is no output generated, but if pytest is invoked in verbose
+mode (``-v``), information about the deleted files is printed.
+
+This plugin was inspired by a feature of `zope.testrunner`_.
+
+.. _`zope.testrunner`: https://pypi.python.org/pypi/zope.testrunner
+
+
+=======
+CHANGES
+=======
+
+
+6.0 (2023-07-07)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 3.5 and 3.6.
+
+Features
+--------
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Update tests to ``pytest >= 6.2``.
+
+Other changes
+-------------
+
+- Use Github actions as CI.
+
+
+
+5.0.1 (2020-03-04)
+==================
+
+- Calling `pytest --help` no longer breaks when this plug-in is installed.
+
+
+5.0 (2020-01-17)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 2.7 and PyPy2.
+
+Features
+--------
+
+- Add support for Python 3.8.
+
+- Migrate to Github.
+
+- Improve for new pytest versions.
+
+Bug fixes
+---------
+
+- Fix problems when running tests jobs in parallel.
+  (`#2 <https://github.com/gocept/pytest-remove-stale-bytecode/issues/2>`_)
+
+
+4.0 (2019-09-13)
+================
+
+Backwards incompatible changes
+------------------------------
+
+- Drop support for Python 3.4.
+
+Features
+--------
+
+- Make work with py.test >=3.10 again.
+
+- Add support for Python 3.7.
+
+
+3.0.1 (2019-03-21)
+==================
+
+- This plug-in only works in py.test < version 3.10.
+  It is broken since the merge of
+  `pytest-dev/pytest#4250 <https://github.com/pytest-dev/pytest/pull/4250>`_
+
+- Drop support for Python 3.3.
+
+
+3.0 (2017-05-12)
+================
+
+- Add support for Python 3.6, PyPy2 and PyPy3.
+
+- Do not show output by default anymore. It can be turned on with ``-v``
+  option.
+
+- Change the license from ZPL to MIT.
+
+
+2.1 (2015-10-01)
+================
+
+- Also remove bytecode files under Python 3, that end with ``-PYTEST``.
+
+
+2.0 (2015-10-01)
+================
+
+- Add support for removing byte code files under Python 3.
+
+
+1.0 (2014-10-29)
+================
+
+- initial release
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/setup.py` & `pytest-remove-stale-bytecode-6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def project_path(*names):
     return os.path.join(os.path.dirname(__file__), *names)
 
 
 setup(
     name='pytest-remove-stale-bytecode',
-    version='5.0.1',
+    version='6.0',
 
     install_requires=[
         'pytest',
         'setuptools',
     ],
 
     extras_require={
@@ -42,24 +42,25 @@
 Environment :: Console
 Intended Audience :: Developers
 License :: OSI Approved :: MIT License
 Natural Language :: English
 Operating System :: OS Independent
 Programming Language :: Python :: 3
 Programming Language :: Python :: 3 :: Only
-Programming Language :: Python :: 3.5
-Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
+Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Programming Language :: Python :: Implementation :: CPython
 Programming Language :: Python :: Implementation :: PyPy
 Topic :: Software Development :: Libraries :: Python Modules
 Topic :: Software Development :: Testing
 """[:-1].split('\n'),
-    python_requires='>= 3.5',
+    python_requires='>= 3.7',
     description=__doc__.strip(),
     long_description='\n\n'.join(open(project_path(name)).read() for name in (
         'README.rst',
         'CHANGES.rst',
     )),
 
     zip_safe=False,
```

### Comparing `pytest-remove-stale-bytecode-5.0.1/test_plugin.py` & `pytest-remove-stale-bytecode-6.0/test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from plugin import pytest_version
 from plugin import python_version
 from unittest import mock
 import pytest
 
+
 pytest_plugins = "pytester",
 
 
 def test_version():
     import plugin
     assert plugin.__version__
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_bytecode_files(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     fooco = testdir.makefile(ext, foo='')
     bar = testdir.makefile(ext, bar='')
 
     assert len(testdir.tmpdir.listdir()) == 3
 
     result = testdir.runpytest()
 
@@ -25,96 +26,96 @@
         line.startswith("Removing stale bytecode file")
         for line in result.outlines)
     assert not bar.exists()
     assert fooco.exists()
     assert foo.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_bytecode_files_verbosely(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     fooco = testdir.makefile(ext, foo='')
     bar = testdir.makefile(ext, bar='')
 
     assert len(testdir.tmpdir.listdir()) == 3
 
     result = testdir.runpytest("-v")
 
     result.stdout.fnmatch_lines([
-        "Removing stale bytecode file *bar.{}".format(ext),
+        "Removing stale bytecode file *bar{}".format(ext),
     ])
     assert not bar.exists()
     assert fooco.exists()
     assert foo.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_PYTEST_bytecode_files(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     foopytest = testdir.makefile(ext, foo_PYTEST='')
     bar = testdir.makefile(ext, bar_PYTEST='')
     testdir.runpytest("-v")
     assert foo.exists()
     assert foopytest.exists()
     assert not bar.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_minus_PYTEST_bytecode_files(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     foopytest = testdir.makefile(ext, **{'foo-PYTEST': ''})
     bar = testdir.makefile(ext, **{'bar-PYTEST': ''})
     testdir.runpytest("-v")
     assert foo.exists()
     assert foopytest.exists()
     assert not bar.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_pytest_version_bytecode_files(testdir, ext):
     foo = testdir.makefile('.py', foo='')
     pycache = testdir.mkdir('__pycache__')
-    fooco_name = 'foo.cpython-{}-pytest-{}.{}'.format(
+    fooco_name = 'foo.cpython-{}-pytest-{}{}'.format(
         python_version, pytest_version, ext)
     fooco = pycache.ensure(fooco_name)
-    barco_name = 'bar.cpython-{}-pytest-{}.{}'.format(
+    barco_name = 'bar.cpython-{}-pytest-{}{}'.format(
         python_version, pytest_version, ext)
     barco = pycache.ensure(barco_name)
     testdir.runpytest("-v")
     assert foo.exists()
     assert fooco.exists()
     assert not barco.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_python3_bytecode_files(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     pycache = testdir.mkdir('__pycache__')
-    fooco_name = 'foo.cpython-{}.{}'.format(python_version, ext)
+    fooco_name = 'foo.cpython-{}{}'.format(python_version, ext)
     fooco = pycache.ensure(fooco_name)
-    barco_name = 'bar.cpython-{}.{}'.format(python_version, ext)
+    barco_name = 'bar.cpython-{}{}'.format(python_version, ext)
     barco = pycache.ensure(barco_name)
     testdir.runpytest("-v")
     assert foo.exists()
     assert fooco.exists()
     assert not barco.exists()
 
 
-@pytest.mark.parametrize("ext", ['pyc', 'pyo'])
+@pytest.mark.parametrize("ext", ['.pyc', '.pyo'])
 def test_plugin_removes_python3_PYTEST_bytecode_files(testdir, ext):
-    foo = testdir.makefile('py', foo='')
+    foo = testdir.makefile('.py', foo='')
     pycache = testdir.mkdir('__pycache__')
-    fooco_name = 'foo.cpython-{}-PYTEST.{}'.format(python_version, ext)
+    fooco_name = 'foo.cpython-{}-PYTEST{}'.format(python_version, ext)
     fooco = pycache.ensure(fooco_name)
-    barco_name = 'bar.cpython-{}-PYTEST.{}'.format(python_version, ext)
+    barco_name = 'bar.cpython-{}-PYTEST{}'.format(python_version, ext)
     barco = pycache.ensure(barco_name)
     testdir.runpytest("-v")
     assert foo.exists()
     assert fooco.exists()
     assert not barco.exists()
 
 
 def test_plugin_does_not_break_if_file_is_removed_externally(testdir):
-    bar = testdir.makefile('pyc', bar='')
+    bar = testdir.makefile('.pyc', bar='')
     with mock.patch('plugin.delete_file', side_effect=FileNotFoundError):
         testdir.runpytest("-v")
     assert bar.exists()
```

