# Comparing `tmp/clize-5.0.0b2.tar.gz` & `tmp/clize-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clize-5.0.0b2.tar", last modified: Wed Oct 12 08:30:56 2022, max compression
+gzip compressed data, was "clize-5.0.1.tar", last modified: Fri Jul  7 06:53:52 2023, max compression
```

## Comparing `clize-5.0.0b2.tar` & `clize-5.0.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.550267 clize-5.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-10-12 08:30:47.000000 clize-5.0.0b2/.bzrignore
--rw-r--r--   0 runner    (1001) docker     (116)      200 2022-10-12 08:30:47.000000 clize-5.0.0b2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.526266 clize-5.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.530266 clize-5.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      333 2022-10-12 08:30:47.000000 clize-5.0.0b2/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1261 2022-10-12 08:30:47.000000 clize-5.0.0b2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (116)      101 2022-10-12 08:30:47.000000 clize-5.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      311 2022-10-12 08:30:47.000000 clize-5.0.0b2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      552 2022-10-12 08:30:47.000000 clize-5.0.0b2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2022-10-12 08:30:47.000000 clize-5.0.0b2/COPYING
--rw-r--r--   0 runner    (1001) docker     (116)     1066 2022-10-12 08:30:47.000000 clize-5.0.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       71 2022-10-12 08:30:47.000000 clize-5.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3901 2022-10-12 08:30:56.550267 clize-5.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2477 2022-10-12 08:30:47.000000 clize-5.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.534267 clize-5.0.0b2/clize/
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2913 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (116)     4224 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/converters.py
--rw-r--r--   0 runner    (1001) docker     (116)     4995 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    30556 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/help.py
--rw-r--r--   0 runner    (1001) docker     (116)     5670 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/legacy.py
--rw-r--r--   0 runner    (1001) docker     (116)    15722 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    49704 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)    14392 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.538267 clize-5.0.0b2/clize/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      384 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11184 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (116)    58088 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (116)    12770 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3563 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_legacy_py3k.py
--rw-r--r--   0 runner    (1001) docker     (116)    26151 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    34022 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)    21995 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_testutil.py
--rw-r--r--   0 runner    (1001) docker     (116)     7314 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     3441 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     9523 2022-10-12 08:30:47.000000 clize-5.0.0b2/clize/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.534267 clize-5.0.0b2/clize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3901 2022-10-12 08:30:56.000000 clize-5.0.0b2/clize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2022-10-12 08:30:56.000000 clize-5.0.0b2/clize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-12 08:30:56.000000 clize-5.0.0b2/clize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      185 2022-10-12 08:30:56.000000 clize-5.0.0b2/clize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-10-12 08:30:56.000000 clize-5.0.0b2/clize.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.546267 clize-5.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.546267 clize-5.0.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)       77 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/_static/clize_style.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.546267 clize-5.0.0b2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (116)      306 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)    15141 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3270 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     8399 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7253 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/compositing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9124 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3400 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4692 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/dispatching.rst
--rw-r--r--   0 runner    (1001) docker     (116)    15258 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/docstring-reference.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5959 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (116)     8594 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2755 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3770 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/interop.rst
--rw-r--r--   0 runner    (1001) docker     (116)  1242077 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/json
--rw-r--r--   0 runner    (1001) docker     (116)     5094 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)    18373 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/parser.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4036 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/porting.rst
--rw-r--r--   0 runner    (1001) docker     (116)    18209 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5963 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/releases.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5851 2022-10-12 08:30:47.000000 clize-5.0.0b2/docs/why.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:56.550267 clize-5.0.0b2/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/altcommands.py
--rw-r--r--   0 runner    (1001) docker     (116)      516 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/argdeco.py
--rw-r--r--   0 runner    (1001) docker     (116)     1261 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/bfparam.py
--rw-r--r--   0 runner    (1001) docker     (116)      602 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/deco_add_param.py
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/deco_provide_arg.py
--rw-r--r--   0 runner    (1001) docker     (116)      877 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/echo.py
--rw-r--r--   0 runner    (1001) docker     (116)      432 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/hello.py
--rw-r--r--   0 runner    (1001) docker     (116)      117 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (116)      531 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/interop.py
--rw-r--r--   0 runner    (1001) docker     (116)     1662 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/logparam.py
--rw-r--r--   0 runner    (1001) docker     (116)      415 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/mapped.py
--rw-r--r--   0 runner    (1001) docker     (116)      275 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/multi.py
--rw-r--r--   0 runner    (1001) docker     (116)      386 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/multicommands.py
--rw-r--r--   0 runner    (1001) docker     (116)     1548 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/naval.py
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2022-10-12 08:30:47.000000 clize-5.0.0b2/examples/typed_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      140 2022-10-12 08:30:47.000000 clize-5.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      113 2022-10-12 08:30:56.550267 clize-5.0.0b2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     2063 2022-10-12 08:30:47.000000 clize-5.0.0b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      968 2022-10-12 08:30:47.000000 clize-5.0.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.369161 clize-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 06:53:43.000000 clize-5.0.1/.bzrignore
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-07 06:53:43.000000 clize-5.0.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.353161 clize-5.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-07 06:53:43.000000 clize-5.0.1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-07 06:53:43.000000 clize-5.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 06:53:43.000000 clize-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 06:53:43.000000 clize-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 06:53:43.000000 clize-5.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-07 06:53:43.000000 clize-5.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 06:53:43.000000 clize-5.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 06:53:43.000000 clize-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-07 06:53:52.369161 clize-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 06:53:43.000000 clize-5.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/clize/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 06:53:43.000000 clize-5.0.1/clize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-07 06:53:43.000000 clize-5.0.1/clize/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-07 06:53:43.000000 clize-5.0.1/clize/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-07 06:53:43.000000 clize-5.0.1/clize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-07-07 06:53:43.000000 clize-5.0.1/clize/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-07 06:53:43.000000 clize-5.0.1/clize/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-07 06:53:43.000000 clize-5.0.1/clize/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49704 2023-07-07 06:53:43.000000 clize-5.0.1/clize/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-07 06:53:43.000000 clize-5.0.1/clize/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.361161 clize-5.0.1/clize/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_legacy_py3k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26151 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34022 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23083 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-07-07 06:53:43.000000 clize-5.0.1/clize/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/clize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-07 06:53:43.000000 clize-5.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 06:53:43.000000 clize-5.0.1/docs/_static/clize_style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-07 06:53:43.000000 clize-5.0.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-07-07 06:53:43.000000 clize-5.0.1/docs/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 06:53:43.000000 clize-5.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-07 06:53:43.000000 clize-5.0.1/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-07 06:53:43.000000 clize-5.0.1/docs/compositing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-07 06:53:43.000000 clize-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 06:53:43.000000 clize-5.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-07 06:53:43.000000 clize-5.0.1/docs/dispatching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-07 06:53:43.000000 clize-5.0.1/docs/docstring-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-07 06:53:43.000000 clize-5.0.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-07 06:53:43.000000 clize-5.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-07 06:53:43.000000 clize-5.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-07 06:53:43.000000 clize-5.0.1/docs/interop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1242077 2023-07-07 06:53:43.000000 clize-5.0.1/docs/json
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-07 06:53:43.000000 clize-5.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-07 06:53:43.000000 clize-5.0.1/docs/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-07 06:53:43.000000 clize-5.0.1/docs/porting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-07-07 06:53:43.000000 clize-5.0.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-07 06:53:43.000000 clize-5.0.1/docs/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-07 06:53:43.000000 clize-5.0.1/docs/why.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.369161 clize-5.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-07 06:53:43.000000 clize-5.0.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:43.000000 clize-5.0.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 06:53:43.000000 clize-5.0.1/examples/altcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 06:53:43.000000 clize-5.0.1/examples/argdeco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-07 06:53:43.000000 clize-5.0.1/examples/bfparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-07 06:53:43.000000 clize-5.0.1/examples/deco_add_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-07 06:53:43.000000 clize-5.0.1/examples/deco_provide_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 06:53:43.000000 clize-5.0.1/examples/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 06:53:43.000000 clize-5.0.1/examples/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-07 06:53:43.000000 clize-5.0.1/examples/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-07 06:53:43.000000 clize-5.0.1/examples/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 06:53:43.000000 clize-5.0.1/examples/logparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-07 06:53:43.000000 clize-5.0.1/examples/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 06:53:43.000000 clize-5.0.1/examples/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-07 06:53:43.000000 clize-5.0.1/examples/multicommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-07 06:53:43.000000 clize-5.0.1/examples/naval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 06:53:43.000000 clize-5.0.1/examples/typed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 06:53:43.000000 clize-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 06:53:52.369161 clize-5.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-07-07 06:53:43.000000 clize-5.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 06:53:43.000000 clize-5.0.1/tox.ini
```

### Comparing `clize-5.0.0b2/.github/workflows/ci.yml` & `clize-5.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/AUTHORS` & `clize-5.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/COPYING` & `clize-5.0.1/COPYING`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2015 by Yann Kaiser and contributors. See AUTHORS for
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS for
 # details.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `clize-5.0.0b2/LICENSE.txt` & `clize-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/PKG-INFO` & `clize-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clize
-Version: 5.0.0b2
+Version: 5.0.1
 Summary: Turn functions into command-line interfaces
 Home-page: https://github.com/epsy/clize
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: CLI,options,arguments,getopts,getopt,argparse,introspection,flags,decorator,subcommands
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clize-5.0.0b2/README.rst` & `clize-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/clize/__init__.py` & `clize-5.0.1/clize/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 """procedurally generate command-line interfaces from callables"""
 
 from clize.parser import Parameter
 from clize.runner import Clize, SubcommandDispatcher, run
 from clize.legacy import clize, make_flag
```

### Comparing `clize-5.0.0b2/clize/_sphinx.py` & `clize-5.0.1/clize/_sphinx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 """Adds auto- and domain directives that don't clash the referencing system"""
 from sphinx.domains import python
 from sphinx.ext import autodoc
```

### Comparing `clize-5.0.0b2/clize/converters.py` & `clize-5.0.1/clize/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 import contextlib
 import sys
 import io
 import os
 import warnings
 from functools import partial
```

### Comparing `clize-5.0.0b2/clize/errors.py` & `clize-5.0.1/clize/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 from functools import partial
 
 
 class UserError(ValueError):
     """An error to be printed to the user."""
```

### Comparing `clize-5.0.0b2/clize/help.py` & `clize-5.0.1/clize/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 """
 `clize.help` manages the generation of help messages obtained using ``--help``.
 
 `.HelpCli` is the command-line interface for it. It is injected as an extra
 alternate option by `.Clize`. It can be replaced using `.Clize`'s
```

### Comparing `clize-5.0.0b2/clize/legacy.py` & `clize-5.0.1/clize/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import warnings
 from functools import partial
 from itertools import chain
 from collections import defaultdict
```

### Comparing `clize-5.0.0b2/clize/parameters.py` & `clize-5.0.1/clize/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import inspect
 from functools import update_wrapper
 
 from sigtools import modifiers, specifiers, signatures
```

### Comparing `clize-5.0.0b2/clize/parser.py` & `clize-5.0.1/clize/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 """
 interpret function signatures and read commandline arguments
 """
 
 import itertools
```

### Comparing `clize-5.0.0b2/clize/runner.py` & `clize-5.0.1/clize/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 import contextlib
 import pathlib
 import sys
 import os
 import typing
 import warnings
@@ -74,15 +74,15 @@
         :type helper_class: a type like `.ClizeHelp`
         :param bool hide_help: Mark the parameters used to trigger the help
             as undocumented.
         """
         update_wrapper(self, fn)
         self.func = fn
         self.owner = owner
-        self.alt = util.maybe_iter(alt)
+        self.alt = util.dict_from_names(alt)
         self.extra = extra
         self.help_names = help_names
         self.help_aliases = [util.name_py2cli(s, kw=True) for s in help_names]
         self.helper_class = helper_class
         self.hide_help = hide_help
 
     def __class_getitem__(cls, item):
@@ -99,15 +99,15 @@
             'hide_help': self.hide_help,
             }
 
     def _key(self):
         return (
             self.func,
             self.owner,
-            tuple(self.alt),
+            tuple(self.alt.items()),
             tuple(self.extra),
             tuple(self.help_names),
             tuple(self.help_aliases),
             self.helper_class,
             self.hide_help,
         )
 
@@ -211,15 +211,15 @@
         else:
             class_ = self.helper_class
         return class_(self, self.owner)
 
     @util.property_once
     def signature(self):
         """The `.parser.CliSignature` object used to parse arguments."""
-        extra = itertools.chain(self._process_alt(self.alt), self.extra)
+        extra = itertools.chain(self._process_alt(), self.extra)
         with self._move_warnings_to_func():
             return parser.CliSignature.from_signature(
                 self.func_signature,
                 extra=extra)
 
     @util.property_once
     def func_signature(self):
@@ -238,22 +238,22 @@
         else:
             with warnings.catch_warnings(record=True) as caught_warnings:
                 yield
             for warning in caught_warnings:
                 registry = module_globals.setdefault("__warningregistry__", {})
                 warnings.warn_explicit(warning.message, warning.category, filename, lineno, module, registry, module_globals)
 
-    def _process_alt(self, alt):
+    def _process_alt(self):
         if self.help_names:
             p = parser.FallbackCommandParameter(
                 func=self.helper.cli, undocumented=self.hide_help,
                 aliases=self.help_aliases)
             yield p
 
-        for name, func in util.dict_from_names(alt).items():
+        for name, func in self.alt.items():
             func = self.get_cli(func)
             param = parser.AlternateCommandParameter(
                 undocumented=False, func=func,
                 aliases=[util.name_py2cli(name, kw=True)])
             yield param
 
     def __call__(self, *args):
```

### Comparing `clize-5.0.0b2/clize/tests/test_converters.py` & `clize-5.0.1/clize/tests/test_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 import unittest
 from datetime import datetime
 import tempfile
 import shutil
 import os
 import stat
```

### Comparing `clize-5.0.0b2/clize/tests/test_help.py` & `clize-5.0.1/clize/tests/test_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import sys
 import io
 import inspect
 import typing
 import unittest
```

### Comparing `clize-5.0.0b2/clize/tests/test_legacy.py` & `clize-5.0.1/clize/tests/test_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import sys
 import unittest
 import warnings
 from io import StringIO
```

### Comparing `clize-5.0.0b2/clize/tests/test_legacy_py3k.py` & `clize-5.0.1/clize/tests/test_legacy_py3k.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 from sigtools import modifiers
 from clize import clize, errors
 
 from clize.tests.test_legacy import OldInterfaceTests
```

### Comparing `clize-5.0.0b2/clize/tests/test_parameters.py` & `clize-5.0.1/clize/tests/test_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 from sigtools import support, modifiers
 
 from clize import parser, errors, Parameter, runner, parameters
 from clize.tests.util import SignatureFixtures, FunctionFixtures
```

### Comparing `clize-5.0.0b2/clize/tests/test_parser.py` & `clize-5.0.1/clize/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 import functools
 import inspect
 import os
 import pathlib
 import typing
 import warnings
```

### Comparing `clize-5.0.0b2/clize/tests/test_runner.py` & `clize-5.0.1/clize/tests/test_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import pathlib
 import sys
 import unittest
 from io import StringIO
 
@@ -487,14 +487,40 @@
         stdout, stderr = self.crun(func1, alt=func2, args=['test'])
         self.assertFalse(stderr.getvalue())
         self.assertEqual(stdout.getvalue(), '1\n')
         stdout, stderr = self.crun(func1, alt=func2, args=['test', '--func2'])
         self.assertFalse(stderr.getvalue())
         self.assertEqual(stdout.getvalue(), '2\n')
 
+    def test_alt_list(self):
+        def base(): return '0'
+        def func1(): return '1'
+        def func2(): return '2'
+        alt = [func1, func2]
+        self.crun(base, alt=alt, args=['test'])
+        stdout, stderr = self.crun(base, alt=alt, args=['test', '--func1'])
+        self.assertFalse(stderr.getvalue())
+        self.assertEqual(stdout.getvalue(), '1\n')
+        stdout, stderr = self.crun(base, alt=alt, args=['test', '--func2'])
+        self.assertFalse(stderr.getvalue())
+        self.assertEqual(stdout.getvalue(), '2\n')
+
+    def test_alt_dict(self):
+        def base(): return '0'
+        def func1(): return '1'
+        def func2(): return '2'
+        alt = {'1': func1, '2': func2}
+        self.crun(base, alt=alt, args=['test'])
+        stdout, stderr = self.crun(base, alt=alt, args=['test', '-1'])
+        self.assertFalse(stderr.getvalue())
+        self.assertEqual(stdout.getvalue(), '1\n')
+        stdout, stderr = self.crun(base, alt=alt, args=['test', '-2'])
+        self.assertFalse(stderr.getvalue())
+        self.assertEqual(stdout.getvalue(), '2\n')
+
     def test_disable_help(self):
         def func1(): raise NotImplementedError
         stdout, stderr = self.crun(
             func1, help_names=[], args=['test', '--help'])
         self.assertTrue(stderr.getvalue())
         self.assertFalse(stdout.getvalue())
```

### Comparing `clize-5.0.0b2/clize/tests/test_testutil.py` & `clize-5.0.1/clize/tests/test_testutil.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/clize/tests/test_util.py` & `clize-5.0.1/clize/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 from clize import util
 from clize.tests.util import Fixtures
 
 
 def formatter(**kwargs):
```

### Comparing `clize-5.0.0b2/clize/tests/util.py` & `clize-5.0.1/clize/tests/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 import __future__
 import os
 import sys
 import inspect
 import unittest
```

### Comparing `clize-5.0.0b2/clize/util.py` & `clize-5.0.1/clize/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # clize -- A command-line argument parser for Python
-# Copyright (C) 2011-2016 by Yann Kaiser and contributors. See AUTHORS and
+# Copyright (C) 2011-2022 by Yann Kaiser and contributors. See AUTHORS and
 # COPYING for details.
 
 """various"""
 
 import os
 from functools import partial, update_wrapper
 import itertools
```

### Comparing `clize-5.0.0b2/clize.egg-info/PKG-INFO` & `clize-5.0.1/clize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clize
-Version: 5.0.0b2
+Version: 5.0.1
 Summary: Turn functions into command-line interfaces
 Home-page: https://github.com/epsy/clize
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: CLI,options,arguments,getopts,getopt,argparse,introspection,flags,decorator,subcommands
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clize-5.0.0b2/clize.egg-info/SOURCES.txt` & `clize-5.0.1/clize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/Makefile` & `clize-5.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/alternatives.rst` & `clize-5.0.1/docs/alternatives.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/api.rst` & `clize-5.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/basics.rst` & `clize-5.0.1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/compositing.rst` & `clize-5.0.1/docs/compositing.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/conf.py` & `clize-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/contributing.rst` & `clize-5.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/dispatching.rst` & `clize-5.0.1/docs/dispatching.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/docstring-reference.rst` & `clize-5.0.1/docs/docstring-reference.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/faq.rst` & `clize-5.0.1/docs/faq.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 Using ``pip`` to install Clize from PyPI as in :ref:`install` will
 automatically install the right dependencies for you.
 
 If you still need the list, Clize always requires:
 
 * `sigtools <https://pypi.org/pypi/sigtools/>`_:
-  Utilities to help manipulate function sigatures.
+  Utilities to help manipulate function signatures.
 * `od <https://pypi.org/project/od/>`_: Shorthand for OrderedDict.
 * `attrs <https://pypi.org/project/attrs>`_: Classes without boilerplate.
 * `docutils <https://pypi.org/project/docutils>`_: To parse docstrings.
 
 If you wish to use `clize.converters.datetime`, you need:
 
 * `python-dateutil <https://pypi.python.org/pypi/python-dateutil/>`_: For
```

### Comparing `clize-5.0.0b2/docs/history.rst` & `clize-5.0.1/docs/history.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/index.rst` & `clize-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/interop.rst` & `clize-5.0.1/docs/interop.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/json` & `clize-5.0.1/docs/json`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/make.bat` & `clize-5.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/parser.rst` & `clize-5.0.1/docs/parser.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/porting.rst` & `clize-5.0.1/docs/porting.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/reference.rst` & `clize-5.0.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/docs/releases.rst` & `clize-5.0.1/docs/releases.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,59 @@
 .. currentmodule:: clize
 
 .. _releases:
 
 Release notes
 =============
 
+.. _v5.0.1:
+
+5.0.1 (2023-07-06)
+------------------
+
+* Fixed ``run(..., alt={...})`` not working correctly with dicts
+
+.. _v5.0:
+.. _v5.0.0:
+
+5.0.0 (2022-10-13)
+------------------
+
+Breaking changes:
+
+* `bytes` annotation (converter) now re-encodes the corresponding parameter back to bytes
+
+Deprecations:
+
+* The ``convert_default`` argument to `~clize.parser.value_converter` is now deprecated.
+  `Parameter.cli_default` is the recommended replacement.
+  To help transition, a new ``convert_default_filter`` option has been added to `~clize.parser.value_converter`,
+  which allows converter authors to filter which values are selected for default conversion,
+  thereby not incurring a deprecation warning for the user.
+
+Updated compatibility:
+
+* Dropped support for Python 2.7, Python 3.5.
+* Verified support for Python 3.10+
+* Compatibility with Docutils 0.21+
+* Improved path support for Windows
+
+Improvements:
+
+* Automatically group identical subcommands as aliases
+* Evaluate deferred annotations from :pep:`563`
+* Basic support for `typing.Annotated`
+* `Parameter.cli_default` allows script writers to specify a default value
+  that will be converted like an argument passed in from the CLI,
+  but not supplied when the function is called from Python.
+
+Process updates:
+
+* Updated Continuous Integration and Delivery to speed up releases and move off of deprecated CI platform.
+
 .. _v4.2:
 
 .. _v4.2.1:
 
 4.2.1 (2021-11-13)
 ------------------
```

### Comparing `clize-5.0.0b2/docs/why.rst` & `clize-5.0.1/docs/why.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/README.rst` & `clize-5.0.1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/argdeco.py` & `clize-5.0.1/examples/argdeco.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/bfparam.py` & `clize-5.0.1/examples/bfparam.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/deco_add_param.py` & `clize-5.0.1/examples/deco_add_param.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/deco_provide_arg.py` & `clize-5.0.1/examples/deco_provide_arg.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/echo.py` & `clize-5.0.1/examples/echo.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/interop.py` & `clize-5.0.1/examples/interop.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/logparam.py` & `clize-5.0.1/examples/logparam.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/naval.py` & `clize-5.0.1/examples/naval.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/examples/typed_cli.py` & `clize-5.0.1/examples/typed_cli.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.0b2/setup.py` & `clize-5.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description_content_type='text/x-rst',
     license='MIT',
     url='https://github.com/epsy/clize',
     author='Yann Kaiser',
     author_email='kaiser.yann@gmail.com',
     python_requires='>=3.6',
     install_requires=[
-        'sigtools ~= 4.0.1a1',
+        'sigtools >= 4.0.1',
         'attrs>=19.1.0',
         'od',
         'docutils >= 0.17.0',
     ],
     tests_require=test_requirements,
     extras_require={
         'datetime': ['python-dateutil'],
```

### Comparing `clize-5.0.0b2/tox.ini` & `clize-5.0.1/tox.ini`

 * *Files identical despite different names*

