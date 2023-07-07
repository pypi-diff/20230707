# Comparing `tmp/sfst-transduce-1.0.1.tar.gz` & `tmp/sfst-transduce-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfst-transduce-1.0.1.tar", last modified: Mon Dec 13 15:26:32 2021, max compression
+gzip compressed data, was "sfst-transduce-1.0.2.tar", last modified: Fri Jul  7 14:21:27 2023, max compression
```

## Comparing `sfst-transduce-1.0.1.tar` & `sfst-transduce-1.0.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:32.012455 sfst-transduce-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15127 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2021-12-13 15:26:32.012455 sfst-transduce-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:31.996455 sfst-transduce-1.0.1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/python/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/python/sfst_transduce.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:31.996455 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-13 15:26:31.000000 sfst-transduce-1.0.1/python/sfst_transduce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-12-13 15:26:32.012455 sfst-transduce-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:32.004455 sfst-transduce-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/Socket.h
--rw-r--r--   0 runner    (1001) docker     (121)    24996 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/alphabet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8917 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/alphabet.h
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/basic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/basic.h
--rw-r--r--   0 runner    (1001) docker     (121)    19706 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/compact.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/compact.h
--rw-r--r--   0 runner    (1001) docker     (121)     5612 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/default-scanner.ll
--rw-r--r--   0 runner    (1001) docker     (121)     8146 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/determinise.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-compact.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-compare.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12426 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-compiler.yy
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-generate.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-infl.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9796 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-infl2-daemon.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12320 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-infl2.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-infl3.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-lattice.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-lowmem.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-match.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-mor.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5509 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-parse.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-parse2.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-print.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-text2bin.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6395 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst-train.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    37500 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12261 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/fst.h
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/generate.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19019 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/hopcroft.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    58639 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/interface.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6417 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/interface.h
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/lowmem.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/lowmem.h
--rw-r--r--   0 runner    (1001) docker     (121)     9683 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/make-compact.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/make-compact.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:32.008455 sfst-transduce-1.0.1/src/man1/
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-compact.1
--rw-r--r--   0 runner    (1001) docker     (121)      527 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-compare.1
--rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-compiler-utf8.1
--rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-compiler.1
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-generate.1
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-infl.1
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-infl2.1
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-infl3.1
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-lattice.1
--rw-r--r--   0 runner    (1001) docker     (121)      780 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-lowmem.1
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-match.1
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-mor.1
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-parse.1
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-parse2.1
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-print.1
--rw-r--r--   0 runner    (1001) docker     (121)      972 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-text2bin.1
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/man1/fst-train.1
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/mem.h
--rw-r--r--   0 runner    (1001) docker     (121)    38582 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/operators.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10303 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/robust.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      623 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/scanner.h
--rw-r--r--   0 runner    (1001) docker     (121)     6424 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/scanner.ll
--rwxr-xr-x   0 runner    (1001) docker     (121)     1068 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/socket-client.pl
--rw-r--r--   0 runner    (1001) docker     (121)     6048 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/utf8-scanner.ll
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/utf8.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/utf8.h
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/src/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:32.008455 sfst-transduce-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 15:26:32.012455 sfst-transduce-1.0.1/tests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/conftest.cpython-38-pytest-6.2.4.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/conftest.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/fixtures.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.4.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/easy.a
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/easy.ca
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-12-13 15:26:17.000000 sfst-transduce-1.0.1/tests/test_transducers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.193894 sfst-transduce-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 14:21:27.193894 sfst-transduce-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.181893 sfst-transduce-1.0.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/python/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/python/sfst_transduce.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.181893 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 14:21:27.000000 sfst-transduce-1.0.2/python/sfst_transduce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 14:21:27.193894 sfst-transduce-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.189894 sfst-transduce-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/Socket.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24996 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/alphabet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/alphabet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19706 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/compact.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/default-scanner.ll
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/determinise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-compare.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-compiler.yy
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-generate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-infl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-infl2-daemon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-infl2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-infl3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-lattice.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-lowmem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-match.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-mor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-parse2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-print.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-text2bin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst-train.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/fst.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/generate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/hopcroft.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    58639 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/lowmem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/lowmem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/make-compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/make-compact.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.189894 sfst-transduce-1.0.2/src/man1/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-compact.1
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-compare.1
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-compiler-utf8.1
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-compiler.1
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-generate.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-infl.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-infl2.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-infl3.1
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-lattice.1
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-lowmem.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-match.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-mor.1
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-parse.1
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-parse2.1
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-print.1
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-text2bin.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/man1/fst-train.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38582 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/operators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/robust.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/scanner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/scanner.ll
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/socket-client.pl
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/utf8-scanner.ll
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/utf8.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/src/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.189894 sfst-transduce-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:21:27.193894 sfst-transduce-1.0.2/tests/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/conftest.cpython-38-pytest-6.2.4.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/conftest.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/fixtures.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.4.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/easy.a
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/easy.ca
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 14:21:15.000000 sfst-transduce-1.0.2/tests/test_transducers.py
```

### Comparing `sfst-transduce-1.0.1/CMakeLists.txt` & `sfst-transduce-1.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/COPYING` & `sfst-transduce-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/PKG-INFO` & `sfst-transduce-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sfst-transduce
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python bindings for SFST focusing on transducer usage
 Home-page: https://github.com/gremid/sfst-transduce
 Author: Gregor Middell
 Author-email: gregor@middell.net
 License: GPLv2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
 
 # sfst-transduce
 
 _Python bindings for SFST focusing on transducer usage_
 
+[![PyPI](https://img.shields.io/pypi/v/sfst-transduce.svg "PyPI")](https://pypi.org/project/sfst-transduce/)
+
 A Python library providing bindings for the Stuttgart Finite State Transducer
 system with a focus on the usage of compiled and serialized transducers,
 excluding code for transducer development and testing, which reduces compile and
 runtime dependencies.
 
 Should you need the [SFST
 tools](https://www.cis.uni-muenchen.de/~schmid/tools/SFST/) for transducer
@@ -85,9 +86,7 @@
 Schmid, Helmut. "A programming language for finite state transducers." FSMNLP.
 Vol. 4002. 2005.
 [pdf](https://www.cis.uni-muenchen.de/~schmid/papers/SFST-PL.pdf)
 
 This Python library is a fork of the excellent [SFST
 adaptation](https://github.com/santhoshtr/sfst) by Santhosh Thottingal, changing
 the focus of the Python part.
-
-
```

### Comparing `sfst-transduce-1.0.1/README.md` & `sfst-transduce-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
 # sfst-transduce
 
 _Python bindings for SFST focusing on transducer usage_
 
+[![PyPI](https://img.shields.io/pypi/v/sfst-transduce.svg "PyPI")](https://pypi.org/project/sfst-transduce/)
+
 A Python library providing bindings for the Stuttgart Finite State Transducer
 system with a focus on the usage of compiled and serialized transducers,
 excluding code for transducer development and testing, which reduces compile and
 runtime dependencies.
 
 Should you need the [SFST
 tools](https://www.cis.uni-muenchen.de/~schmid/tools/SFST/) for transducer
```

### Comparing `sfst-transduce-1.0.1/python/sfst_transduce.cpp` & `sfst-transduce-1.0.2/python/sfst_transduce.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/python/sfst_transduce.egg-info/PKG-INFO` & `sfst-transduce-1.0.2/python/sfst_transduce.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sfst-transduce
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python bindings for SFST focusing on transducer usage
 Home-page: https://github.com/gremid/sfst-transduce
 Author: Gregor Middell
 Author-email: gregor@middell.net
 License: GPLv2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
 
 # sfst-transduce
 
 _Python bindings for SFST focusing on transducer usage_
 
+[![PyPI](https://img.shields.io/pypi/v/sfst-transduce.svg "PyPI")](https://pypi.org/project/sfst-transduce/)
+
 A Python library providing bindings for the Stuttgart Finite State Transducer
 system with a focus on the usage of compiled and serialized transducers,
 excluding code for transducer development and testing, which reduces compile and
 runtime dependencies.
 
 Should you need the [SFST
 tools](https://www.cis.uni-muenchen.de/~schmid/tools/SFST/) for transducer
@@ -85,9 +86,7 @@
 Schmid, Helmut. "A programming language for finite state transducers." FSMNLP.
 Vol. 4002. 2005.
 [pdf](https://www.cis.uni-muenchen.de/~schmid/papers/SFST-PL.pdf)
 
 This Python library is a fork of the excellent [SFST
 adaptation](https://github.com/santhoshtr/sfst) by Santhosh Thottingal, changing
 the focus of the Python part.
-
-
```

### Comparing `sfst-transduce-1.0.1/python/sfst_transduce.egg-info/SOURCES.txt` & `sfst-transduce-1.0.2/python/sfst_transduce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/setup.py` & `sfst-transduce-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/CMakeLists.txt` & `sfst-transduce-1.0.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/Socket.h` & `sfst-transduce-1.0.2/src/Socket.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/alphabet.cpp` & `sfst-transduce-1.0.2/src/alphabet.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/alphabet.h` & `sfst-transduce-1.0.2/src/alphabet.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/basic.cpp` & `sfst-transduce-1.0.2/src/basic.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/basic.h` & `sfst-transduce-1.0.2/src/basic.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/compact.cpp` & `sfst-transduce-1.0.2/src/compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/compact.h` & `sfst-transduce-1.0.2/src/compact.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/default-scanner.ll` & `sfst-transduce-1.0.2/src/default-scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/determinise.cpp` & `sfst-transduce-1.0.2/src/determinise.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-compact.cpp` & `sfst-transduce-1.0.2/src/fst-compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-compare.cpp` & `sfst-transduce-1.0.2/src/fst-compare.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-compiler.yy` & `sfst-transduce-1.0.2/src/fst-compiler.yy`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-generate.cpp` & `sfst-transduce-1.0.2/src/fst-generate.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-infl.cpp` & `sfst-transduce-1.0.2/src/fst-infl.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-infl2-daemon.cpp` & `sfst-transduce-1.0.2/src/fst-infl2-daemon.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-infl2.cpp` & `sfst-transduce-1.0.2/src/fst-infl2.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-infl3.cpp` & `sfst-transduce-1.0.2/src/fst-infl3.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-lattice.cpp` & `sfst-transduce-1.0.2/src/fst-lattice.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-lowmem.cpp` & `sfst-transduce-1.0.2/src/fst-lowmem.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-match.cpp` & `sfst-transduce-1.0.2/src/fst-match.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-mor.cpp` & `sfst-transduce-1.0.2/src/fst-mor.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-parse.cpp` & `sfst-transduce-1.0.2/src/fst-parse.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-parse2.cpp` & `sfst-transduce-1.0.2/src/fst-parse2.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-print.cpp` & `sfst-transduce-1.0.2/src/fst-print.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-text2bin.cpp` & `sfst-transduce-1.0.2/src/fst-text2bin.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst-train.cpp` & `sfst-transduce-1.0.2/src/fst-train.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst.cpp` & `sfst-transduce-1.0.2/src/fst.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/fst.h` & `sfst-transduce-1.0.2/src/fst.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/generate.cpp` & `sfst-transduce-1.0.2/src/generate.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/hopcroft.cpp` & `sfst-transduce-1.0.2/src/hopcroft.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/interface.cpp` & `sfst-transduce-1.0.2/src/interface.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/interface.h` & `sfst-transduce-1.0.2/src/interface.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/lowmem.cpp` & `sfst-transduce-1.0.2/src/lowmem.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/lowmem.h` & `sfst-transduce-1.0.2/src/lowmem.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/make-compact.cpp` & `sfst-transduce-1.0.2/src/make-compact.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/make-compact.h` & `sfst-transduce-1.0.2/src/make-compact.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-compact.1` & `sfst-transduce-1.0.2/src/man1/fst-compact.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-compare.1` & `sfst-transduce-1.0.2/src/man1/fst-compare.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-compiler-utf8.1` & `sfst-transduce-1.0.2/src/man1/fst-compiler-utf8.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-compiler.1` & `sfst-transduce-1.0.2/src/man1/fst-compiler.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-generate.1` & `sfst-transduce-1.0.2/src/man1/fst-generate.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-infl.1` & `sfst-transduce-1.0.2/src/man1/fst-infl.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-infl2.1` & `sfst-transduce-1.0.2/src/man1/fst-infl2.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-infl3.1` & `sfst-transduce-1.0.2/src/man1/fst-infl3.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-lattice.1` & `sfst-transduce-1.0.2/src/man1/fst-lattice.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-lowmem.1` & `sfst-transduce-1.0.2/src/man1/fst-lowmem.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-match.1` & `sfst-transduce-1.0.2/src/man1/fst-match.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-mor.1` & `sfst-transduce-1.0.2/src/man1/fst-mor.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-parse.1` & `sfst-transduce-1.0.2/src/man1/fst-parse.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-parse2.1` & `sfst-transduce-1.0.2/src/man1/fst-parse2.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-print.1` & `sfst-transduce-1.0.2/src/man1/fst-print.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-text2bin.1` & `sfst-transduce-1.0.2/src/man1/fst-text2bin.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/man1/fst-train.1` & `sfst-transduce-1.0.2/src/man1/fst-train.1`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/mem.h` & `sfst-transduce-1.0.2/src/mem.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/operators.cpp` & `sfst-transduce-1.0.2/src/operators.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/robust.cpp` & `sfst-transduce-1.0.2/src/robust.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/scanner.h` & `sfst-transduce-1.0.2/src/scanner.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/scanner.ll` & `sfst-transduce-1.0.2/src/scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/socket-client.pl` & `sfst-transduce-1.0.2/src/socket-client.pl`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/utf8-scanner.ll` & `sfst-transduce-1.0.2/src/utf8-scanner.ll`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/utf8.cpp` & `sfst-transduce-1.0.2/src/utf8.cpp`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/src/utf8.h` & `sfst-transduce-1.0.2/src/utf8.h`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/tests/__pycache__/fixtures.cpython-38-pytest-6.2.5.pyc` & `sfst-transduce-1.0.2/tests/__pycache__/fixtures.cpython-38-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.4.pyc` & `sfst-transduce-1.0.2/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.4.pyc`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.5.pyc` & `sfst-transduce-1.0.2/tests/__pycache__/test_transducers.cpython-38-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sfst-transduce-1.0.1/tests/easy.a` & `sfst-transduce-1.0.2/tests/easy.a`

 * *Files identical despite different names*

