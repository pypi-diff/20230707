# Comparing `tmp/flake8-mock-0.3.tar.gz` & `tmp/flake8-mock-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-mock-0.3.tar", last modified: Sat Sep 10 15:49:56 2016, max compression
+gzip compressed data, was "flake8-mock-0.4.tar", last modified: Fri Jul  7 09:47:03 2023, max compression
```

## Comparing `flake8-mock-0.3.tar` & `flake8-mock-0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 alepereira  (1000) alepereira  (1000)        0 2016-09-10 15:49:56.000000 flake8-mock-0.3/
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)     1762 2016-09-10 15:24:39.000000 flake8-mock-0.3/flake8_mock.py
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)     2460 2016-09-10 15:46:18.000000 flake8-mock-0.3/README.rst
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)       59 2016-09-10 15:49:56.000000 flake8-mock-0.3/setup.cfg
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)     1478 2016-08-12 17:57:20.000000 flake8-mock-0.3/setup.py
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)     3942 2016-09-10 15:49:56.000000 flake8-mock-0.3/PKG-INFO
-drwxrwxr-x   0 alepereira  (1000) alepereira  (1000)        0 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)        1 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)       58 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/entry_points.txt
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)      246 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)        1 2016-08-12 18:27:06.000000 flake8-mock-0.3/flake8_mock.egg-info/not-zip-safe
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)       12 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/top_level.txt
--rw-rw-r--   0 alepereira  (1000) alepereira  (1000)     3942 2016-09-10 15:49:56.000000 flake8-mock-0.3/flake8_mock.egg-info/PKG-INFO
+drwxr-xr-x   0 yekol      (501) staff       (20)        0 2023-07-07 09:47:03.921250 flake8-mock-0.4/
+-rw-r--r--   0 yekol      (501) staff       (20)    18047 2023-07-07 09:32:05.000000 flake8-mock-0.4/LICENSE
+-rw-r--r--   0 yekol      (501) staff       (20)     3435 2023-07-07 09:47:03.921001 flake8-mock-0.4/PKG-INFO
+-rw-r--r--   0 yekol      (501) staff       (20)     2666 2023-07-07 09:43:09.000000 flake8-mock-0.4/README.rst
+drwxr-xr-x   0 yekol      (501) staff       (20)        0 2023-07-07 09:47:03.920705 flake8-mock-0.4/flake8_mock.egg-info/
+-rw-r--r--   0 yekol      (501) staff       (20)     3435 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/PKG-INFO
+-rw-r--r--   0 yekol      (501) staff       (20)      254 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 yekol      (501) staff       (20)        1 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 yekol      (501) staff       (20)       47 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/entry_points.txt
+-rw-r--r--   0 yekol      (501) staff       (20)        1 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/not-zip-safe
+-rw-r--r--   0 yekol      (501) staff       (20)       12 2023-07-07 09:47:03.000000 flake8-mock-0.4/flake8_mock.egg-info/top_level.txt
+-rw-r--r--   0 yekol      (501) staff       (20)     1779 2023-07-07 09:39:31.000000 flake8-mock-0.4/flake8_mock.py
+-rw-r--r--   0 yekol      (501) staff       (20)       38 2023-07-07 09:47:03.921317 flake8-mock-0.4/setup.cfg
+-rw-r--r--   0 yekol      (501) staff       (20)     1468 2023-07-07 09:39:31.000000 flake8-mock-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flake8-mock-0.3/flake8_mock.py` & `flake8-mock-0.4/flake8_mock.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 from sys import stdin
 
 import ast
 import tokenize
 
 
-__version__ = '0.3'
+__version__ = '0.4'
 
 NON_EXISTENT_METHODS = [
     'assert_calls',
     'not_called',
     'called_once',
     'called_once_with',
+    'has_calls',
 ]
 MOCK_ERROR_CODE = 'M001'
 ERROR_MESSAGE = "%s %s is a non-existent mock method."
 
 
 def get_noqa_lines(code):
     tokens = tokenize.generate_tokens(lambda L=iter(code): next(L))
```

### Comparing `flake8-mock-0.3/README.rst` & `flake8-mock-0.4/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     * ``called_once``
     * ``called_once_with``
 
 
 Plugin for Flake8
 -----------------
 
-When both ``flake8 2.4`` and ``flake8-mock`` are installed, the plugin is
+When both ``flake8`` and ``flake8-mock`` are installed, the plugin is
 available in ``flake8``::
 
     $ flake8 --version
-    2.4.1 (pep8: 1.5.7, flake8-mock: 0.3, pyflakes: 0.8.1)
+    5.0.4 (flake8-mock: 0.4, ...)
 
 
 Example output
 --------------
 
 Once you run flake8, you can have something like::
 
@@ -53,27 +53,33 @@
     test_file.py:27:1: M001 assert_calls is a non-existent mock method.
     test_file.py:28:1: M001 called_once_with is a non-existent mock method.
     test_file.py:39:1: M001 not_called is a non-existent mock method.
     test_file.py:40:1: M001 assert_called is a non-existent mock method.
 
 Credits
 -------
-    * Alejandro Gabriel Pereira is the main author.
-    * Nejc Zupan (`NiteoWeb Ltd. <http://www.niteoweb.com>`_) provided the idea
+    * `Alejandro Gabriel Pereira <https://github.com/aleGpereira>`_ is the main author.
+    * `Nejc Zupan <https://github.com/zupo>`_ (`Niteo <https://niteo.co>`_) provided the idea
       and proof-reading.
 
 Collaborators
 -------------
     * `John Vandenberg <https://github.com/jayvdb>`_
     * `Tom Prince <https://github.com/tomprince>`_
+    * `Gasper Vozel <https://github.com/karantan>`_
+    * `Bjørnar Myrheim <https://github.com/myrheimb>`_
 
 
 Changes
 -------
 
+0.4 (05-12-2023)
+````````````````
+* Fix compatibility with flake8 >= 5.0.0.
+
 0.3 (09-10-2016)
 ````````````````
 * Don't warn on `assert_not_called`, `assert_called` or `assert_called_once`.
 * Use ASCII only in README.rst
 
 0.2 (12-16-2015)
 ````````````````
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flake8-mock-0.3/setup.py` & `flake8-mock-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     author_email='alepereira.dev@gmail.com',
     url='https://github.com/aleGpereira/flake8-mock',
     license='GNU',
     py_modules=['flake8_mock'],
     zip_safe=False,
     entry_points={
         'flake8.extension': [
-            'flake8_mock = flake8_mock:MockChecker',
+            'M = flake8_mock:MockChecker',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
```

### Comparing `flake8-mock-0.3/PKG-INFO` & `flake8-mock-0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: flake8-mock
-Version: 0.3
+Version: 0.4
 Summary: Provides checking for non-existent mock methods
 Home-page: https://github.com/aleGpereira/flake8-mock
 Author: Alejandro Pereira
 Author-email: alepereira.dev@gmail.com
 License: GNU
-Description: Flake8 Mock plugin
-        ==================
-        
-        Remember that a mock's job is to say, "You got it, boss" whenever anyone calls
-        it. It will do real work, like raising an exception, when one of its
-        convenience methods is called, like ``assert_called_once_with``. But it won't
-        do real work when you call a method that only *resembles* a convenience method,
-        such as ``assert_called_once`` (no ``_with``!). Sometimes developers may not
-        notice that they are using a non-existent mock method, because they are not
-        getting an output error telling them so. And for some reason they can also
-        forget to verify that the test cases fail before writing implementation code.
-        
-        This plugin checks for possible non-existent mock methods when you run
-        ``flake8``, the Python code checker.
-        
-        Inspired by http://engineeringblog.yelp.com/2015/02/assert_called_once-threat-or-menace.html.
-        
-        
-        Installation
-        ------------
-        
-        You can install or upgrade ``flake8-mock`` with these commands::
-        
-          $ pip install flake8-mock
-          $ pip install --upgrade flake8-mock
-        
-        
-        List of non-existent methods checked
-        ------------------------------------
-        
-            * ``assert_calls``
-            * ``not_called``
-            * ``called_once``
-            * ``called_once_with``
-        
-        
-        Plugin for Flake8
-        -----------------
-        
-        When both ``flake8 2.4`` and ``flake8-mock`` are installed, the plugin is
-        available in ``flake8``::
-        
-            $ flake8 --version
-            2.4.1 (pep8: 1.5.7, flake8-mock: 0.3, pyflakes: 0.8.1)
-        
-        
-        Example output
-        --------------
-        
-        Once you run flake8, you can have something like::
-        
-            $ flake8 test_file.py
-            test_file.py:27:1: M001 assert_calls is a non-existent mock method.
-            test_file.py:28:1: M001 called_once_with is a non-existent mock method.
-            test_file.py:39:1: M001 not_called is a non-existent mock method.
-            test_file.py:40:1: M001 assert_called is a non-existent mock method.
-        
-        Credits
-        -------
-            * Alejandro Gabriel Pereira is the main author.
-            * Nejc Zupan (`NiteoWeb Ltd. <http://www.niteoweb.com>`_) provided the idea
-              and proof-reading.
-        
-        Collaborators
-        -------------
-            * `John Vandenberg <https://github.com/jayvdb>`_
-            * `Tom Prince <https://github.com/tomprince>`_
-        
-        
-        Changes
-        -------
-        
-        0.3 (09-10-2016)
-        ````````````````
-        * Don't warn on `assert_not_called`, `assert_called` or `assert_called_once`.
-        * Use ASCII only in README.rst
-        
-        0.2 (12-16-2015)
-        ````````````````
-        * Add Python 3 compatibility.
-        
-        0.1 (10-20-2015)
-        ````````````````
-        * First release.
-        
-        0.1dev0 (10-19-2015)
-        ````````````````````
-        * First dev release.
-        
 Keywords: flake8,mock,testing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
+License-File: LICENSE
+
+Flake8 Mock plugin
+==================
+
+Remember that a mock's job is to say, "You got it, boss" whenever anyone calls
+it. It will do real work, like raising an exception, when one of its
+convenience methods is called, like ``assert_called_once_with``. But it won't
+do real work when you call a method that only *resembles* a convenience method,
+such as ``assert_called_once`` (no ``_with``!). Sometimes developers may not
+notice that they are using a non-existent mock method, because they are not
+getting an output error telling them so. And for some reason they can also
+forget to verify that the test cases fail before writing implementation code.
+
+This plugin checks for possible non-existent mock methods when you run
+``flake8``, the Python code checker.
+
+Inspired by http://engineeringblog.yelp.com/2015/02/assert_called_once-threat-or-menace.html.
+
+
+Installation
+------------
+
+You can install or upgrade ``flake8-mock`` with these commands::
+
+  $ pip install flake8-mock
+  $ pip install --upgrade flake8-mock
+
+
+List of non-existent methods checked
+------------------------------------
+
+    * ``assert_calls``
+    * ``not_called``
+    * ``called_once``
+    * ``called_once_with``
+
+
+Plugin for Flake8
+-----------------
+
+When both ``flake8`` and ``flake8-mock`` are installed, the plugin is
+available in ``flake8``::
+
+    $ flake8 --version
+    5.0.4 (flake8-mock: 0.4, ...)
+
+
+Example output
+--------------
+
+Once you run flake8, you can have something like::
+
+    $ flake8 test_file.py
+    test_file.py:27:1: M001 assert_calls is a non-existent mock method.
+    test_file.py:28:1: M001 called_once_with is a non-existent mock method.
+    test_file.py:39:1: M001 not_called is a non-existent mock method.
+    test_file.py:40:1: M001 assert_called is a non-existent mock method.
+
+Credits
+-------
+    * `Alejandro Gabriel Pereira <https://github.com/aleGpereira>`_ is the main author.
+    * `Nejc Zupan <https://github.com/zupo>`_ (`Niteo <https://niteo.co>`_) provided the idea
+      and proof-reading.
+
+Collaborators
+-------------
+    * `John Vandenberg <https://github.com/jayvdb>`_
+    * `Tom Prince <https://github.com/tomprince>`_
+    * `Gasper Vozel <https://github.com/karantan>`_
+    * `Bjørnar Myrheim <https://github.com/myrheimb>`_
+
+
+Changes
+-------
+
+0.4 (05-12-2023)
+````````````````
+* Fix compatibility with flake8 >= 5.0.0.
+
+0.3 (09-10-2016)
+````````````````
+* Don't warn on `assert_not_called`, `assert_called` or `assert_called_once`.
+* Use ASCII only in README.rst
+
+0.2 (12-16-2015)
+````````````````
+* Add Python 3 compatibility.
+
+0.1 (10-20-2015)
+````````````````
+* First release.
+
+0.1dev0 (10-19-2015)
+````````````````````
+* First dev release.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flake8-mock-0.3/flake8_mock.egg-info/PKG-INFO` & `flake8-mock-0.4/flake8_mock.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: flake8-mock
-Version: 0.3
+Version: 0.4
 Summary: Provides checking for non-existent mock methods
 Home-page: https://github.com/aleGpereira/flake8-mock
 Author: Alejandro Pereira
 Author-email: alepereira.dev@gmail.com
 License: GNU
-Description: Flake8 Mock plugin
-        ==================
-        
-        Remember that a mock's job is to say, "You got it, boss" whenever anyone calls
-        it. It will do real work, like raising an exception, when one of its
-        convenience methods is called, like ``assert_called_once_with``. But it won't
-        do real work when you call a method that only *resembles* a convenience method,
-        such as ``assert_called_once`` (no ``_with``!). Sometimes developers may not
-        notice that they are using a non-existent mock method, because they are not
-        getting an output error telling them so. And for some reason they can also
-        forget to verify that the test cases fail before writing implementation code.
-        
-        This plugin checks for possible non-existent mock methods when you run
-        ``flake8``, the Python code checker.
-        
-        Inspired by http://engineeringblog.yelp.com/2015/02/assert_called_once-threat-or-menace.html.
-        
-        
-        Installation
-        ------------
-        
-        You can install or upgrade ``flake8-mock`` with these commands::
-        
-          $ pip install flake8-mock
-          $ pip install --upgrade flake8-mock
-        
-        
-        List of non-existent methods checked
-        ------------------------------------
-        
-            * ``assert_calls``
-            * ``not_called``
-            * ``called_once``
-            * ``called_once_with``
-        
-        
-        Plugin for Flake8
-        -----------------
-        
-        When both ``flake8 2.4`` and ``flake8-mock`` are installed, the plugin is
-        available in ``flake8``::
-        
-            $ flake8 --version
-            2.4.1 (pep8: 1.5.7, flake8-mock: 0.3, pyflakes: 0.8.1)
-        
-        
-        Example output
-        --------------
-        
-        Once you run flake8, you can have something like::
-        
-            $ flake8 test_file.py
-            test_file.py:27:1: M001 assert_calls is a non-existent mock method.
-            test_file.py:28:1: M001 called_once_with is a non-existent mock method.
-            test_file.py:39:1: M001 not_called is a non-existent mock method.
-            test_file.py:40:1: M001 assert_called is a non-existent mock method.
-        
-        Credits
-        -------
-            * Alejandro Gabriel Pereira is the main author.
-            * Nejc Zupan (`NiteoWeb Ltd. <http://www.niteoweb.com>`_) provided the idea
-              and proof-reading.
-        
-        Collaborators
-        -------------
-            * `John Vandenberg <https://github.com/jayvdb>`_
-            * `Tom Prince <https://github.com/tomprince>`_
-        
-        
-        Changes
-        -------
-        
-        0.3 (09-10-2016)
-        ````````````````
-        * Don't warn on `assert_not_called`, `assert_called` or `assert_called_once`.
-        * Use ASCII only in README.rst
-        
-        0.2 (12-16-2015)
-        ````````````````
-        * Add Python 3 compatibility.
-        
-        0.1 (10-20-2015)
-        ````````````````
-        * First release.
-        
-        0.1dev0 (10-19-2015)
-        ````````````````````
-        * First dev release.
-        
 Keywords: flake8,mock,testing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
+License-File: LICENSE
+
+Flake8 Mock plugin
+==================
+
+Remember that a mock's job is to say, "You got it, boss" whenever anyone calls
+it. It will do real work, like raising an exception, when one of its
+convenience methods is called, like ``assert_called_once_with``. But it won't
+do real work when you call a method that only *resembles* a convenience method,
+such as ``assert_called_once`` (no ``_with``!). Sometimes developers may not
+notice that they are using a non-existent mock method, because they are not
+getting an output error telling them so. And for some reason they can also
+forget to verify that the test cases fail before writing implementation code.
+
+This plugin checks for possible non-existent mock methods when you run
+``flake8``, the Python code checker.
+
+Inspired by http://engineeringblog.yelp.com/2015/02/assert_called_once-threat-or-menace.html.
+
+
+Installation
+------------
+
+You can install or upgrade ``flake8-mock`` with these commands::
+
+  $ pip install flake8-mock
+  $ pip install --upgrade flake8-mock
+
+
+List of non-existent methods checked
+------------------------------------
+
+    * ``assert_calls``
+    * ``not_called``
+    * ``called_once``
+    * ``called_once_with``
+
+
+Plugin for Flake8
+-----------------
+
+When both ``flake8`` and ``flake8-mock`` are installed, the plugin is
+available in ``flake8``::
+
+    $ flake8 --version
+    5.0.4 (flake8-mock: 0.4, ...)
+
+
+Example output
+--------------
+
+Once you run flake8, you can have something like::
+
+    $ flake8 test_file.py
+    test_file.py:27:1: M001 assert_calls is a non-existent mock method.
+    test_file.py:28:1: M001 called_once_with is a non-existent mock method.
+    test_file.py:39:1: M001 not_called is a non-existent mock method.
+    test_file.py:40:1: M001 assert_called is a non-existent mock method.
+
+Credits
+-------
+    * `Alejandro Gabriel Pereira <https://github.com/aleGpereira>`_ is the main author.
+    * `Nejc Zupan <https://github.com/zupo>`_ (`Niteo <https://niteo.co>`_) provided the idea
+      and proof-reading.
+
+Collaborators
+-------------
+    * `John Vandenberg <https://github.com/jayvdb>`_
+    * `Tom Prince <https://github.com/tomprince>`_
+    * `Gasper Vozel <https://github.com/karantan>`_
+    * `Bjørnar Myrheim <https://github.com/myrheimb>`_
+
+
+Changes
+-------
+
+0.4 (05-12-2023)
+````````````````
+* Fix compatibility with flake8 >= 5.0.0.
+
+0.3 (09-10-2016)
+````````````````
+* Don't warn on `assert_not_called`, `assert_called` or `assert_called_once`.
+* Use ASCII only in README.rst
+
+0.2 (12-16-2015)
+````````````````
+* Add Python 3 compatibility.
+
+0.1 (10-20-2015)
+````````````````
+* First release.
+
+0.1dev0 (10-19-2015)
+````````````````````
+* First dev release.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

