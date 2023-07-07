# Comparing `tmp/execnet-1.9.0.tar.gz` & `tmp/execnet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/execnet-1.9.0.tar", last modified: Sun Jun 13 13:47:15 2021, max compression
+gzip compressed data, last modified: Thu Jul  6 18:59:09 2023, max compression
```

## Comparing `execnet-1.9.0.tar` & `execnet-2.0.0.tar`

### file list

```diff
@@ -1,95 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2021-06-13 13:47:12.000000 execnet-1.9.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-06-13 13:47:12.000000 execnet-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-06-13 13:47:12.000000 execnet-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    15282 2021-06-13 13:47:12.000000 execnet-1.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2021-06-13 13:47:12.000000 execnet-1.9.0/ISSUES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-06-13 13:47:12.000000 execnet-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2021-06-13 13:47:15.000000 execnet-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2021-06-13 13:47:12.000000 execnet-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-06-13 13:47:12.000000 execnet-1.9.0/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    24123 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_static/basic1.png
--rw-r--r--   0 runner    (1001) docker     (121)    10202 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_static/codespeak.png
--rw-r--r--   0 runner    (1001) docker     (121)    36750 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_static/execnet.png
--rw-r--r--   0 runner    (1001) docker     (121)    17805 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_static/pythonring.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_templates/indexsidebar.html
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     8214 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6184 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/doc/example/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/funcmultiplier.py
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/hybridpython.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/popen_read_multiple.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/py3topy2.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/redirect_remote_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/remote1.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/remotecmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/servefiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3736 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/svn-sync-repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/taskserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_debug.rst
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_funcmultiplier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_group.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6301 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_info.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_multi.rst
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_proxy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      574 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/example/test_ssh_fileserver.rst
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/implnotes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-06-13 13:47:12.000000 execnet-1.9.0/doc/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet/
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    51156 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/gateway_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/gateway_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     7537 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/gateway_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/gateway_socket.py
--rw-r--r--   0 runner    (1001) docker     (121)    10313 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/rsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/rsync_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet/script/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/loop_socketserver.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/quitserver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2487 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3833 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/socketserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/socketserverservice.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/script/xx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-06-13 13:47:12.000000 execnet-1.9.0/execnet/xspec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-13 13:47:15.000000 execnet-1.9.0/execnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2021-06-13 13:47:12.000000 execnet-1.9.0/scripts/install-pypy.bat
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-06-13 13:47:15.000000 execnet-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2021-06-13 13:47:12.000000 execnet-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 13:47:15.000000 execnet-1.9.0/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12153 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (121)    13831 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_compatibility_regressions.py
--rw-r--r--   0 runner    (1001) docker     (121)    17308 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     7562 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     7840 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_termination.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_threadpool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8376 2021-06-13 13:47:12.000000 execnet-1.9.0/testing/test_xspec.py
--rw-r--r--   0 runner    (1001) docker     (121)      543 2021-06-13 13:47:12.000000 execnet-1.9.0/tox.ini
+-rw-r--r--   0        0        0      958 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/_version.py
+-rw-r--r--   0        0        0     7115 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/gateway.py
+-rw-r--r--   0        0        0    51114 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/gateway_base.py
+-rw-r--r--   0        0        0     2990 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/gateway_bootstrap.py
+-rw-r--r--   0        0        0     6836 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/gateway_io.py
+-rw-r--r--   0        0        0     2501 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/gateway_socket.py
+-rw-r--r--   0        0        0    10291 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/multi.py
+-rw-r--r--   0        0        0     7611 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/rsync.py
+-rw-r--r--   0        0        0     3828 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/rsync_remote.py
+-rw-r--r--   0        0        0     1788 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/xspec.py
+-rw-r--r--   0        0        0        2 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/loop_socketserver.py
+-rw-r--r--   0        0        0      306 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/quitserver.py
+-rw-r--r--   0        0        0     2480 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/shell.py
+-rw-r--r--   0        0        0     3696 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/socketserver.py
+-rw-r--r--   0        0        0     3044 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/socketserverservice.py
+-rw-r--r--   0        0        0      186 2023-07-06 18:59:09.000000 execnet-2.0.0/src/execnet/script/xx.py
+-rw-r--r--   0        0        0      188 2023-07-06 18:59:09.000000 execnet-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1054 2023-07-06 18:59:09.000000 execnet-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1593 2023-07-06 18:59:09.000000 execnet-2.0.0/README.rst
+-rw-r--r--   0        0        0     1525 2023-07-06 18:59:09.000000 execnet-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2923 2023-07-06 18:59:09.000000 execnet-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `execnet-1.9.0/LICENSE` & `execnet-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `execnet-1.9.0/README.rst` & `execnet-2.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 execnet: distributed Python deployment and communication
 ========================================================
 
 Important
 ---------
 
-**execnet currently is in maintenance-only mode, mostly because it is still the backend
-of the pytest-xdist plugin. Do not use in new projects.**
-
 .. image:: https://img.shields.io/pypi/v/execnet.svg
     :target: https://pypi.org/project/execnet/
 
 .. image:: https://anaconda.org/conda-forge/execnet/badges/version.svg
     :target: https://anaconda.org/conda-forge/execnet
 
 .. image:: https://img.shields.io/pypi/pyversions/execnet.svg
     :target: https://pypi.org/project/execnet/
 
-.. image:: https://github.com/pytest-dev/execnet/workflows/build/badge.svg
-    :target: https://github.com/pytest-dev/execnet/actions?query=workflow%3Abuild
+.. image:: https://github.com/pytest-dev/execnet/workflows/test/badge.svg
+    :target: https://github.com/pytest-dev/execnet/actions?query=workflow%3Atest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/python/black
 
 .. _execnet: http://codespeak.net/execnet
 
 execnet_ provides carefully tested means to ad-hoc interact with Python
 interpreters across version, platform and network barriers.  It provides
-a minimal and fast API targetting the following uses:
+a minimal and fast API targeting the following uses:
 
 * distribute tasks to local or remote processes
 * write and deploy hybrid multi-process applications
 * write scripts to administer multiple hosts
 
 Features
-------------------
+--------
 
 * zero-install bootstrapping: no remote installation required!
 
 * flexible communication: send/receive as well as
   callback/queue mechanisms supported
 
 * simple serialization of python builtin types (no pickling)
```

### Comparing `execnet-1.9.0/execnet/__init__.py` & `execnet-2.0.0/src/execnet/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-# -*- coding: utf-8 -*-
 """
 execnet
 -------
 
 pure python lib for connecting to local and remote Python Interpreters.
 
 (c) 2012, Holger Krekel and others
 """
 from ._version import version as __version__
-from .deprecated import PopenGateway
-from .deprecated import SocketGateway
-from .deprecated import SshGateway
 from .gateway_base import DataFormatError
 from .gateway_base import dump
 from .gateway_base import dumps
 from .gateway_base import load
 from .gateway_base import loads
 from .gateway_base import RemoteError
 from .gateway_base import TimeoutError
@@ -26,17 +22,14 @@
 from .multi import set_execmodel
 from .rsync import RSync
 from .xspec import XSpec
 
 
 __all__ = [
     "__version__",
-    "PopenGateway",
-    "SocketGateway",
-    "SshGateway",
     "makegateway",
     "set_execmodel",
     "HostNotFound",
     "RemoteError",
     "TimeoutError",
     "XSpec",
     "Group",
```

### Comparing `execnet-1.9.0/execnet/gateway.py` & `execnet-2.0.0/src/execnet/gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 gateway code for initiating popen, socket and ssh connections.
 (c) 2004-2013, Holger Krekel and others
 """
 import inspect
 import linecache
 import os
@@ -15,18 +14,18 @@
 from . import gateway_base
 from .gateway_base import Message
 
 importdir = os.path.dirname(os.path.dirname(execnet.__file__))
 
 
 class Gateway(gateway_base.BaseGateway):
-    """Gateway to a local or remote Python Intepreter."""
+    """Gateway to a local or remote Python Interpreter."""
 
     def __init__(self, io, spec):
-        super(Gateway, self).__init__(io=io, id=spec.id, _startcount=1)
+        super().__init__(io=io, id=spec.id, _startcount=1)
         self.spec = spec
         self._initreceive()
 
     @property
     def remoteaddress(self):
         return self._io.remoteaddress
 
@@ -53,15 +52,15 @@
             return
         self._group._unregister(self)
         try:
             self._trace("--> sending GATEWAY_TERMINATE")
             self._send(Message.GATEWAY_TERMINATE)
             self._trace("--> io.close_write")
             self._io.close_write()
-        except (ValueError, EOFError, IOError):
+        except (ValueError, EOFError, OSError):
             v = sys.exc_info()[1]
             self._trace("io-error: could not send termination sequence")
             self._trace(" exception: %r" % v)
 
     def reconfigure(self, py2str_as_py3str=True, py3str_as_py2str=False):
         """
         set the string coercion for this gateway
@@ -166,57 +165,49 @@
             pid=os.getpid(),
         )
     )
 
 
 def _find_non_builtin_globals(source, codeobj):
     import ast
-
-    try:
-        import __builtin__
-    except ImportError:
-        import builtins as __builtin__
+    import builtins
 
     vars = dict.fromkeys(codeobj.co_varnames)
     return [
         node.id
         for node in ast.walk(ast.parse(source))
         if isinstance(node, ast.Name)
         and node.id not in vars
-        and node.id not in __builtin__.__dict__
+        and node.id not in builtins.__dict__
     ]
 
 
 def _source_of_function(function):
     if function.__name__ == "<lambda>":
         raise ValueError("can't evaluate lambda functions'")
-    # XXX: we dont check before remote instanciation
-    #      if arguments are used propperly
+    # XXX: we dont check before remote instantiation
+    #      if arguments are used properly
     try:
         sig = inspect.getfullargspec(function)
     except AttributeError:
         args = inspect.getargspec(function)[0]
     else:
         args = sig.args
     if not args or args[0] != "channel":
         raise ValueError("expected first function argument to be `channel`")
 
-    if gateway_base.ISPY3:
-        closure = function.__closure__
-        codeobj = function.__code__
-    else:
-        closure = function.func_closure
-        codeobj = function.func_code
+    closure = function.__closure__
+    codeobj = function.__code__
 
     if closure is not None:
         raise ValueError("functions with closures can't be passed")
 
     try:
         source = inspect.getsource(function)
-    except IOError:
+    except OSError:
         raise ValueError("can't find source file for %s" % function)
 
     source = textwrap.dedent(source)  # just for inner functions
 
     used_globals = _find_non_builtin_globals(source, codeobj)
     if used_globals:
         raise ValueError("the use of non-builtin globals isn't supported", used_globals)
```

### Comparing `execnet-1.9.0/execnet/gateway_base.py` & `execnet-2.0.0/src/execnet/gateway_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,196 +1,272 @@
-# -*- coding: utf-8 -*-
 """
 base execnet gateway code send to the other side for bootstrapping.
 
 NOTE: aims to be compatible to Python 2.5-3.X, Jython and IronPython
 
 :copyright: 2004-2015
 :authors:
     - Holger Krekel
     - Armin Rigo
     - Benjamin Peterson
     - Ronny Pfannschmidt
     - many others
 """
-from __future__ import with_statement
+from __future__ import annotations
 
+import abc
 import os
 import struct
 import sys
 import traceback
 import weakref
+from _thread import interrupt_main
+from io import BytesIO
+from typing import Callable
 
-# NOTE that we want to avoid try/except style importing
-# to avoid setting sys.exc_info() during import
-#
 
-ISPY3 = sys.version_info >= (3, 0)
-if ISPY3:
-    from io import BytesIO
+class ExecModel(metaclass=abc.ABCMeta):
+    @property
+    @abc.abstractmethod
+    def backend(self):
+        raise NotImplementedError()
 
-    exec("do_exec = exec")
+    def __repr__(self):
+        return "<ExecModel %r>" % self.backend
 
-    def reraise(cls, val, tb):
-        raise val.with_traceback(tb)
+    @property
+    @abc.abstractmethod
+    def queue(self):
+        raise NotImplementedError()
 
-    unicode = str
-    _long_type = int
-    from _thread import interrupt_main
+    @property
+    @abc.abstractmethod
+    def subprocess(self):
+        raise NotImplementedError()
 
-    SUBPROCESS32 = False
-else:
-    from StringIO import StringIO as BytesIO
+    @property
+    @abc.abstractmethod
+    def socket(self):
+        raise NotImplementedError()
 
-    exec(
-        "def do_exec(co, loc): exec co in loc\n"
-        "def reraise(cls, val, tb): raise cls, val, tb\n"
-    )
-    bytes = str
-    _long_type = long
-    try:
-        from thread import interrupt_main
-    except ImportError:
-        interrupt_main = None
-    try:
-        import subprocess32  # NOQA
+    @abc.abstractmethod
+    def start(self, func, args=()):
+        raise NotImplementedError()
 
-        SUBPROCESS32 = True
-    except ImportError:
-        SUBPROCESS32 = False
-        sys.exc_clear()
+    @abc.abstractmethod
+    def get_ident(self):
+        raise NotImplementedError()
 
+    @abc.abstractmethod
+    def sleep(self, delay):
+        raise NotImplementedError()
 
-# f = open("/tmp/execnet-%s" % os.getpid(), "w")
-# def log_extra(*msg):
-#     f.write(" ".join([str(x) for x in msg]) + "\n")
+    @abc.abstractmethod
+    def fdopen(self, fd, mode, bufsize=1):
+        raise NotImplementedError()
 
+    @abc.abstractmethod
+    def Lock(self):
+        raise NotImplementedError()
 
-class EmptySemaphore:
-    acquire = release = lambda self: None
+    @abc.abstractmethod
+    def RLock(self):
+        raise NotImplementedError()
 
+    @abc.abstractmethod
+    def Event(self):
+        raise NotImplementedError()
 
-def get_execmodel(backend):
-    if hasattr(backend, "backend"):
-        return backend
-    if backend == "thread":
-        importdef = {
-            "get_ident": ["thread::get_ident", "_thread::get_ident"],
-            "_start_new_thread": [
-                "thread::start_new_thread",
-                "_thread::start_new_thread",
-            ],
-            "threading": ["threading"],
-            "queue": ["queue" if ISPY3 else "Queue"],
-            "sleep": ["time::sleep"],
-            "subprocess": ["subprocess32" if SUBPROCESS32 else "subprocess"],
-            "socket": ["socket"],
-            "_fdopen": ["os::fdopen"],
-            "_lock": ["threading"],
-            "_event": ["threading"],
-        }
 
-        def exec_start(self, func, args=()):
-            self._start_new_thread(func, args)
+class ThreadExecModel(ExecModel):
+    backend = "thread"
 
-    elif backend == "eventlet":
-        importdef = {
-            "get_ident": ["eventlet.green.thread::get_ident"],
-            "_spawn_n": ["eventlet::spawn_n"],
-            "threading": ["eventlet.green.threading"],
-            "queue": ["eventlet.queue"],
-            "sleep": ["eventlet::sleep"],
-            "subprocess": ["eventlet.green.subprocess"],
-            "socket": ["eventlet.green.socket"],
-            "_fdopen": ["eventlet.green.os::fdopen"],
-            "_lock": ["eventlet.green.threading"],
-            "_event": ["eventlet.green.threading"],
-        }
+    @property
+    def queue(self):
+        import queue
 
-        def exec_start(self, func, args=()):
-            self._spawn_n(func, *args)
+        return queue
 
-    elif backend == "gevent":
-        importdef = {
-            "get_ident": ["gevent.thread::get_ident"],
-            "_spawn_n": ["gevent::spawn"],
-            "threading": ["threading"],
-            "queue": ["gevent.queue"],
-            "sleep": ["gevent::sleep"],
-            "subprocess": ["gevent.subprocess"],
-            "socket": ["gevent.socket"],
-            # XXX
-            "_fdopen": ["gevent.fileobject::FileObjectThread"],
-            "_lock": ["gevent.lock"],
-            "_event": ["gevent.event"],
-        }
+    @property
+    def subprocess(self):
+        import subprocess
 
-        def exec_start(self, func, args=()):
-            self._spawn_n(func, *args)
+        return subprocess
 
-    else:
-        raise ValueError("unknown execmodel {!r}".format(backend))
+    @property
+    def socket(self):
+        import socket
 
-    class ExecModel:
-        def __init__(self, name):
-            self._importdef = importdef
-            self.backend = name
-            self._count = 0
-
-        def __repr__(self):
-            return "<ExecModel %r>" % self.backend
-
-        def __getattr__(self, name):
-            locs = self._importdef.get(name)
-            if locs is None:
-                raise AttributeError(name)
-            for loc in locs:
-                parts = loc.split("::")
-                loc = parts.pop(0)
-                try:
-                    mod = __import__(loc, None, None, "__doc__")
-                except ImportError:
-                    pass
-                else:
-                    if parts:
-                        mod = getattr(mod, parts[0])
-                    setattr(self, name, mod)
-                    return mod
-            raise AttributeError(name)
+        return socket
+
+    def get_ident(self):
+        import _thread
+
+        return _thread.get_ident()
+
+    def sleep(self, delay):
+        import time
+
+        time.sleep(delay)
+
+    def start(self, func, args=()):
+        import _thread
+
+        return _thread.start_new_thread(func, args)
+
+    def fdopen(self, fd, mode, bufsize=1):
+        import os
+
+        return os.fdopen(fd, mode, bufsize, encoding="utf-8")
+
+    def Lock(self):
+        import threading
+
+        return threading.RLock()
+
+    def RLock(self):
+        import threading
+
+        return threading.RLock()
+
+    def Event(self):
+        import threading
+
+        return threading.Event()
+
+
+class EventletExecModel(ExecModel):
+    backend = "eventlet"
+
+    @property
+    def queue(self):
+        import eventlet
+
+        return eventlet.queue
 
-        start = exec_start
+    @property
+    def subprocess(self):
+        import eventlet.green.subprocess
 
-        def fdopen(self, fd, mode, bufsize=1):
-            return self._fdopen(fd, mode, bufsize)
+        return eventlet.green.subprocess
 
-        def WorkerPool(self, hasprimary=False):
-            return WorkerPool(self, hasprimary=hasprimary)
+    @property
+    def socket(self):
+        import eventlet.green.socket
 
-        def Semaphore(self, size=None):
-            if size is None:
-                return EmptySemaphore()
-            return self._lock.Semaphore(size)
+        return eventlet.green.socket
 
-        def Lock(self):
-            return self._lock.RLock()
+    def get_ident(self):
+        import eventlet.green.thread
 
-        def RLock(self):
-            return self._lock.RLock()
+        return eventlet.green.thread.get_ident()
 
-        def Event(self):
-            return self._event.Event()
+    def sleep(self, delay):
+        import eventlet
 
-        def PopenPiped(self, args):
-            PIPE = self.subprocess.PIPE
-            return self.subprocess.Popen(args, stdout=PIPE, stdin=PIPE)
+        eventlet.sleep(delay)
 
-    return ExecModel(backend)
+    def start(self, func, args=()):
+        import eventlet
+
+        return eventlet.spawn_n(func, *args)
+
+    def fdopen(self, fd, mode, bufsize=1):
+        import eventlet.green.os
+
+        return eventlet.green.os.fdopen(fd, mode, bufsize)
+
+    def Lock(self):
+        import eventlet.green.threading
+
+        return eventlet.green.threading.RLock()
+
+    def RLock(self):
+        import eventlet.green.threading
+
+        return eventlet.green.threading.RLock()
+
+    def Event(self):
+        import eventlet.green.threading
+
+        return eventlet.green.threading.Event()
+
+
+class GeventExecModel(ExecModel):
+    backend = "gevent"
+
+    @property
+    def queue(self):
+        import gevent.queue
+
+        return gevent.queue
+
+    @property
+    def subprocess(self):
+        import gevent.subprocess
+
+        return gevent.subprocess
+
+    @property
+    def socket(self):
+        import gevent
+
+        return gevent.socket
+
+    def get_ident(self):
+        import gevent.thread
+
+        return gevent.thread.get_ident()
+
+    def sleep(self, delay):
+        import gevent
+
+        gevent.sleep(delay)
+
+    def start(self, func, args=()):
+        import gevent
+
+        return gevent.spawn(func, *args)
+
+    def fdopen(self, fd, mode, bufsize=1):
+        # XXX
+        import gevent.fileobject
+
+        return gevent.fileobject.FileObjectThread(fd, mode, bufsize)
+
+    def Lock(self):
+        import gevent.lock
+
+        return gevent.lock.RLock()
+
+    def RLock(self):
+        import gevent.lock
+
+        return gevent.lock.RLock()
+
+    def Event(self):
+        import gevent.event
+
+        return gevent.event.Event()
+
+
+def get_execmodel(backend):
+    if hasattr(backend, "backend"):
+        return backend
+    if backend == "thread":
+        return ThreadExecModel()
+    elif backend == "eventlet":
+        return EventletExecModel()
+    elif backend == "gevent":
+        return GeventExecModel()
+    else:
+        raise ValueError(f"unknown execmodel {backend!r}")
 
 
-class Reply(object):
+class Reply:
     """reply instances provide access to the result
     of a function execution that got dispatched
     through WorkerPool.spawn()
     """
 
     def __init__(self, task, threadmodel):
         self.task = task
@@ -203,35 +279,35 @@
         then calling get() will reraise that exception
         including its traceback.
         """
         self.waitfinish(timeout)
         try:
             return self._result
         except AttributeError:
-            reraise(*(self._excinfo[:3]))  # noqa
+            raise self._excinfo[1].with_traceback(self._excinfo[2])
 
     def waitfinish(self, timeout=None):
         if not self._result_ready.wait(timeout):
-            raise IOError("timeout waiting for {!r}".format(self.task))
+            raise OSError(f"timeout waiting for {self.task!r}")
 
     def run(self):
         func, args, kwargs = self.task
         try:
             try:
                 self._result = func(*args, **kwargs)
-            except:
+            except BaseException:
                 # sys may be already None when shutting down the interpreter
                 if sys is not None:
                     self._excinfo = sys.exc_info()
         finally:
             self._result_ready.set()
             self.running = False
 
 
-class WorkerPool(object):
+class WorkerPool:
     """A WorkerPool allows to spawn function executions
     to threads, returning a reply object on which you
     can ask for the result (and get exceptions reraised).
 
     This implementation allows the main thread to integrate
     itself into performing function execution through
     calling integrate_as_primary_thread() which will return
@@ -339,20 +415,19 @@
 DEBUG = os.environ.get("EXECNET_DEBUG")
 pid = os.getpid()
 if DEBUG == "2":
 
     def trace(*msg):
         try:
             line = " ".join(map(str, msg))
-            sys.stderr.write("[{}] {}\n".format(pid, line))
+            sys.stderr.write(f"[{pid}] {line}\n")
             sys.stderr.flush()
         except Exception:
             pass  # nothing we can do, likely interpreter-shutdown
 
-
 elif DEBUG:
     import tempfile
     import os
 
     fn = os.path.join(tempfile.gettempdir(), "execnet-debug-%d" % pid)
     # sys.stderr.write("execnet-debug at %r" % (fn,))
     debugfile = open(fn, "w")
@@ -361,19 +436,18 @@
         try:
             line = " ".join(map(str, msg))
             debugfile.write(line + "\n")
             debugfile.flush()
         except Exception:
             try:
                 v = sys.exc_info()[1]
-                sys.stderr.write("[{}] exception during tracing: {!r}\n".format(pid, v))
+                sys.stderr.write(f"[{pid}] exception during tracing: {v!r}\n")
             except Exception:
                 pass  # nothing we can do, likely interpreter-shutdown
 
-
 else:
     notrace = trace = lambda *msg: None
 
 
 class Popen2IO:
     error = (IOError, OSError, EOFError)
 
@@ -382,24 +456,24 @@
         self.outfile, self.infile = outfile, infile
         if sys.platform == "win32":
             import msvcrt
 
             try:
                 msvcrt.setmode(infile.fileno(), os.O_BINARY)
                 msvcrt.setmode(outfile.fileno(), os.O_BINARY)
-            except (AttributeError, IOError):
+            except (AttributeError, OSError):
                 pass
         self._read = getattr(infile, "buffer", infile).read
         self._write = getattr(outfile, "buffer", outfile).write
         self.execmodel = execmodel
 
     def read(self, numbytes):
         """Read exactly 'numbytes' bytes from the pipe."""
         # a file in non-blocking mode may return less bytes, so we loop
-        buf = bytes()
+        buf = b""
         while numbytes > len(buf):
             data = self._read(numbytes - len(buf))
             if not data:
                 raise EOFError("expected %d bytes, got %d" % (numbytes, len(buf)))
             buf += data
         return buf
 
@@ -415,154 +489,162 @@
     def close_write(self):
         self.outfile.close()
 
 
 class Message:
     """encapsulates Messages and their wire protocol."""
 
-    _types = []
+    # message code -> name, handler
+    _types: dict[int, tuple[str, Callable[[Message, BaseGateway], None]]] = {}
 
-    def __init__(self, msgcode, channelid=0, data=""):
+    def __init__(self, msgcode, channelid=0, data=b""):
         self.msgcode = msgcode
         self.channelid = channelid
         self.data = data
 
     @staticmethod
     def from_io(io):
         try:
             header = io.read(9)  # type 1, channel 4, payload 4
             if not header:
                 raise EOFError("empty read")
         except EOFError:
             e = sys.exc_info()[1]
-            raise EOFError("couldnt load message header, " + e.args[0])
+            raise EOFError("couldn't load message header, " + e.args[0])
         msgtype, channel, payload = struct.unpack("!bii", header)
         return Message(msgtype, channel, io.read(payload))
 
     def to_io(self, io):
         header = struct.pack("!bii", self.msgcode, self.channelid, len(self.data))
         io.write(header + self.data)
 
     def received(self, gateway):
-        self._types[self.msgcode](self, gateway)
+        handler = self._types[self.msgcode][1]
+        handler(self, gateway)
 
     def __repr__(self):
-        name = self._types[self.msgcode].__name__.upper()
+        name = self._types[self.msgcode][0]
         return "<Message {} channel={} lendata={}>".format(
             name, self.channelid, len(self.data)
         )
 
-
-class GatewayReceivedTerminate(Exception):
-    """Receiverthread got termination message."""
-
-
-def _setupmessages():
-    def status(message, gateway):
+    def _status(message, gateway):
         # we use the channelid to send back information
         # but don't instantiate a channel object
         d = {
             "numchannels": len(gateway._channelfactory._channels),
             "numexecuting": gateway._execpool.active_count(),
             "execmodel": gateway.execmodel.backend,
         }
         gateway._send(Message.CHANNEL_DATA, message.channelid, dumps_internal(d))
         gateway._send(Message.CHANNEL_CLOSE, message.channelid)
 
-    def channel_exec(message, gateway):
+    STATUS = 0
+    _types[STATUS] = ("STATUS", _status)
+
+    def _reconfigure(message, gateway):
+        if message.channelid == 0:
+            target = gateway
+        else:
+            target = gateway._channelfactory.new(message.channelid)
+        target._strconfig = loads_internal(message.data, gateway)
+
+    RECONFIGURE = 1
+    _types[RECONFIGURE] = ("RECONFIGURE", _reconfigure)
+
+    def _gateway_terminate(message, gateway):
+        raise GatewayReceivedTerminate(gateway)
+
+    GATEWAY_TERMINATE = 2
+    _types[GATEWAY_TERMINATE] = ("GATEWAY_TERMINATE", _gateway_terminate)
+
+    def _channel_exec(message, gateway):
         channel = gateway._channelfactory.new(message.channelid)
         gateway._local_schedulexec(channel=channel, sourcetask=message.data)
 
-    def channel_data(message, gateway):
+    CHANNEL_EXEC = 3
+    _types[CHANNEL_EXEC] = ("CHANNEL_EXEC", _channel_exec)
+
+    def _channel_data(message, gateway):
         gateway._channelfactory._local_receive(message.channelid, message.data)
 
-    def channel_close(message, gateway):
+    CHANNEL_DATA = 4
+    _types[CHANNEL_DATA] = ("CHANNEL_DATA", _channel_data)
+
+    def _channel_close(message, gateway):
         gateway._channelfactory._local_close(message.channelid)
 
-    def channel_close_error(message, gateway):
+    CHANNEL_CLOSE = 5
+    _types[CHANNEL_CLOSE] = ("CHANNEL_CLOSE", _channel_close)
+
+    def _channel_close_error(message, gateway):
         remote_error = RemoteError(loads_internal(message.data))
         gateway._channelfactory._local_close(message.channelid, remote_error)
 
-    def channel_last_message(message, gateway):
-        gateway._channelfactory._local_close(message.channelid, sendonly=True)
-
-    def gateway_terminate(message, gateway):
-        raise GatewayReceivedTerminate(gateway)
+    CHANNEL_CLOSE_ERROR = 6
+    _types[CHANNEL_CLOSE_ERROR] = ("CHANNEL_CLOSE_ERROR", _channel_close_error)
 
-    def reconfigure(message, gateway):
-        if message.channelid == 0:
-            target = gateway
-        else:
-            target = gateway._channelfactory.new(message.channelid)
-        target._strconfig = loads_internal(message.data, gateway)
+    def _channel_last_message(message, gateway):
+        gateway._channelfactory._local_close(message.channelid, sendonly=True)
 
-    types = [
-        status,
-        reconfigure,
-        gateway_terminate,
-        channel_exec,
-        channel_data,
-        channel_close,
-        channel_close_error,
-        channel_last_message,
-    ]
-    for i, handler in enumerate(types):
-        Message._types.append(handler)
-        setattr(Message, handler.__name__.upper(), i)
+    CHANNEL_LAST_MESSAGE = 7
+    _types[CHANNEL_LAST_MESSAGE] = ("CHANNEL_LAST_MESSAGE", _channel_last_message)
 
 
-_setupmessages()
+class GatewayReceivedTerminate(Exception):
+    """Receiverthread got termination message."""
 
 
 def geterrortext(excinfo, format_exception=traceback.format_exception, sysex=sysex):
     try:
         l = format_exception(*excinfo)
         errortext = "".join(l)
     except sysex:
         raise
-    except:
-        errortext = "{}: {}".format(excinfo[0].__name__, excinfo[1])
+    except BaseException:
+        errortext = f"{excinfo[0].__name__}: {excinfo[1]}"
     return errortext
 
 
 class RemoteError(Exception):
     """Exception containing a stringified error from the other side."""
 
     def __init__(self, formatted):
+        super().__init__()
         self.formatted = formatted
-        Exception.__init__(self)
 
     def __str__(self):
         return self.formatted
 
     def __repr__(self):
-        return "{}: {}".format(self.__class__.__name__, self.formatted)
+        return f"{self.__class__.__name__}: {self.formatted}"
 
     def warn(self):
         if self.formatted != INTERRUPT_TEXT:
             # XXX do this better
-            sys.stderr.write("[%s] Warning: unhandled %r\n" % (os.getpid(), self))
+            sys.stderr.write(f"[{os.getpid()}] Warning: unhandled {self!r}\n")
 
 
 class TimeoutError(IOError):
     """Exception indicating that a timeout was reached."""
 
 
 NO_ENDMARKER_WANTED = object()
 
 
-class Channel(object):
+class Channel:
     "Communication channel between two Python Interpreter execution points."
     RemoteError = RemoteError
     TimeoutError = TimeoutError
     _INTERNALWAKEUP = 1000
     _executing = False
 
     def __init__(self, gateway, id):
         assert isinstance(id, int)
+        assert not isinstance(gateway, type)
         self.gateway = gateway
         # XXX: defaults copied from Unserializer
         self._strconfig = getattr(gateway, "_strconfig", (True, False))
         self.id = id
         self._items = self.gateway.execmodel.queue.Queue()
         self._closed = False
         self._receiveclosed = self.gateway.execmodel.Event()
@@ -580,15 +662,15 @@
         raise an error.
         If an endmarker is specified the callback will eventually
         be called with the endmarker when the channel closes.
         """
         _callbacks = self.gateway._channelfactory._callbacks
         with self.gateway._receivelock:
             if self._items is None:
-                raise IOError("{!r} has callback already registered".format(self))
+                raise OSError(f"{self!r} has callback already registered")
             items = self._items
             self._items = None
             while 1:
                 try:
                     olditem = items.get(block=False)
                 except self.gateway.execmodel.queue.Empty:
                     if not (self._closed or self._receiveclosed.is_set()):
@@ -629,15 +711,15 @@
             if Message is not None:
                 if self._items is None:  # has_callback
                     msgcode = Message.CHANNEL_LAST_MESSAGE
                 else:
                     msgcode = Message.CHANNEL_CLOSE
                 try:
                     self.gateway._send(msgcode, self.id)
-                except (IOError, ValueError):  # ignore problems with sending
+                except (OSError, ValueError):  # ignore problems with sending
                     pass
 
     def _getremoteerror(self):
         try:
             return self._remoteerrors.pop(0)
         except IndexError:
             try:
@@ -660,24 +742,24 @@
         mode can be 'w' or 'r' for writeable/readable files.
         if proxyclose is true file.close() will also close the channel.
         """
         if mode == "w":
             return ChannelFileWrite(channel=self, proxyclose=proxyclose)
         elif mode == "r":
             return ChannelFileRead(channel=self, proxyclose=proxyclose)
-        raise ValueError("mode {!r} not availabe".format(mode))
+        raise ValueError(f"mode {mode!r} not available")
 
     def close(self, error=None):
         """close down this channel with an optional error message.
         Note that closing of a channel tied to remote_exec happens
         automatically at the end of execution and cannot
-        be done explicitely.
+        be done explicitly.
         """
         if self._executing:
-            raise IOError("cannot explicitly close channel within remote_exec")
+            raise OSError("cannot explicitly close channel within remote_exec")
         if self._closed:
             self.gateway._trace(self, "ignoring redundant call to close()")
         if not self._closed:
             # state transition "opened/sendonly" --> "closed"
             # threads warning: the channel might be closed under our feet,
             # but it's never damaging to send too many CHANNEL_CLOSE messages
             # however, if the other side triggered a close already, we
@@ -721,29 +803,29 @@
         """sends the given item to the other side of the channel,
         possibly blocking if the sender queue is full.
         The item must be a simple python type and will be
         copied to the other side by value.  IOError is
         raised if the write pipe was prematurely closed.
         """
         if self.isclosed():
-            raise IOError("cannot send to {!r}".format(self))
+            raise OSError(f"cannot send to {self!r}")
         self.gateway._send(Message.CHANNEL_DATA, self.id, dumps_internal(item))
 
     def receive(self, timeout=None):
         """receive a data item that was sent from the other side.
         timeout: None [default] blocked waiting.  A positive number
         indicates the number of seconds after which a channel.TimeoutError
         exception will be raised if no item was received.
         Note that exceptions from the remotely executing code will be
         reraised as channel.RemoteError exceptions containing
         a textual representation of the remote traceback.
         """
         itemqueue = self._items
         if itemqueue is None:
-            raise IOError("cannot receive(), channel has receiver callback")
+            raise OSError("cannot receive(), channel has receiver callback")
         try:
             x = itemqueue.get(timeout=timeout)
         except self.gateway.execmodel.queue.Empty:
             raise self.TimeoutError("no item after %r seconds" % timeout)
         if x is ENDMARKER:
             itemqueue.put(x)  # for other receivers
             raise self._getremoteerror() or EOFError()
@@ -772,29 +854,29 @@
         self.gateway._send(Message.RECONFIGURE, self.id, data=data)
 
 
 ENDMARKER = object()
 INTERRUPT_TEXT = "keyboard-interrupted"
 
 
-class ChannelFactory(object):
+class ChannelFactory:
     def __init__(self, gateway, startcount=1):
         self._channels = weakref.WeakValueDictionary()
         self._callbacks = {}
         self._writelock = gateway.execmodel.Lock()
         self.gateway = gateway
         self.count = startcount
         self.finished = False
         self._list = list  # needed during interp-shutdown
 
     def new(self, id=None):
         """create a new Channel with 'id' (or create new id if None)."""
         with self._writelock:
             if self.finished:
-                raise IOError("connexion already closed: {}".format(self.gateway))
+                raise OSError(f"connection already closed: {self.gateway}")
             if id is None:
                 id = self.count
                 self.count += 2
             try:
                 channel = self._channels[id]
             except KeyError:
                 channel = self._channels[id] = Channel(self.gateway, id)
@@ -868,15 +950,15 @@
             self.finished = True
         for id in self._list(self._channels):
             self._local_close(id, sendonly=True)
         for id in self._list(self._callbacks):
             self._no_longer_opened(id)
 
 
-class ChannelFile(object):
+class ChannelFile:
     def __init__(self, channel, proxyclose=True):
         self.channel = channel
         self._proxyclose = proxyclose
 
     def isatty(self):
         return False
 
@@ -895,15 +977,15 @@
 
     def flush(self):
         pass
 
 
 class ChannelFileRead(ChannelFile):
     def __init__(self, channel, proxyclose=True):
-        super(ChannelFileRead, self).__init__(channel, proxyclose)
+        super().__init__(channel, proxyclose)
         self._buffer = None
 
     def read(self, n):
         try:
             if self._buffer is None:
                 self._buffer = self.channel.receive()
             while len(self._buffer) < n:
@@ -929,30 +1011,30 @@
             c = self.read(1)
             if not c:
                 break
             line += c
         return line
 
 
-class BaseGateway(object):
+class BaseGateway:
     exc_info = sys.exc_info
     _sysex = sysex
     id = "<worker>"
 
     def __init__(self, io, id, _startcount=2):
         self.execmodel = io.execmodel
         self._io = io
         self.id = id
         self._strconfig = (Unserializer.py2str_as_py3str, Unserializer.py3str_as_py2str)
         self._channelfactory = ChannelFactory(self, _startcount)
         self._receivelock = self.execmodel.RLock()
         # globals may be NONE at process-termination
         self.__trace = trace
         self._geterrortext = geterrortext
-        self._receivepool = self.execmodel.WorkerPool()
+        self._receivepool = WorkerPool(self.execmodel)
 
     def _trace(self, *msg):
         self.__trace(self.id, *msg)
 
     def _initreceive(self):
         self._receivepool.spawn(self._thread_receiver)
 
@@ -987,24 +1069,24 @@
         self._io.close_write()
         log("terminating our receive pseudo pool")
         self._receivepool.trigger_shutdown()
 
     def _terminate_execution(self):
         pass
 
-    def _send(self, msgcode, channelid=0, data=bytes()):
+    def _send(self, msgcode, channelid=0, data=b""):
         message = Message(msgcode, channelid, data)
         try:
             message.to_io(self._io)
             self._trace("sent", message)
-        except (IOError, ValueError):
+        except (OSError, ValueError):
             e = sys.exc_info()[1]
             self._trace("failed to send", message, e)
             # ValueError might be because the IO is already closed
-            raise IOError("cannot send (already closed?)")
+            raise OSError("cannot send (already closed?)")
 
     def _local_schedulexec(self, channel, sourcetask):
         channel.close("execution disallowed")
 
     # _____________________________________________________________________
     #
     # High Level Interface
@@ -1046,15 +1128,15 @@
                 os._exit(1)
 
     def serve(self):
         def trace(msg):
             self._trace("[serve] " + msg)
 
         hasprimary = self.execmodel.backend == "thread"
-        self._execpool = self.execmodel.WorkerPool(hasprimary=hasprimary)
+        self._execpool = WorkerPool(self.execmodel, hasprimary=hasprimary)
         trace("spawning receiver thread")
         self._initreceive()
         try:
             if hasprimary:
                 # this will return when we are in shutdown
                 trace("integrating as primary thread")
                 self._execpool.integrate_as_primary_thread()
@@ -1063,44 +1145,35 @@
         except KeyboardInterrupt:
             # in the worker we can't really do anything sensible
             trace("swallowing keyboardinterrupt, serve finished")
 
     def executetask(self, item):
         try:
             channel, (source, file_name, call_name, kwargs) = item
-            if not ISPY3 and kwargs:
-                # some python2 versions do not accept unicode keyword params
-                # note: Unserializer generally turns py2-str to py3-str objects
-                newkwargs = {}
-                for name, value in kwargs.items():
-                    if isinstance(name, unicode):
-                        name = name.encode("ascii")
-                    newkwargs[name] = value
-                kwargs = newkwargs
             loc = {"channel": channel, "__name__": "__channelexec__"}
-            self._trace("execution starts[%s]: %s" % (channel.id, repr(source)[:50]))
+            self._trace(f"execution starts[{channel.id}]: {repr(source)[:50]}")
             channel._executing = True
             try:
                 co = compile(source + "\n", file_name or "<remote exec>", "exec")
-                do_exec(co, loc)  # noqa
+                exec(co, loc)
                 if call_name:
                     self._trace("calling %s(**%60r)" % (call_name, kwargs))
                     function = loc[call_name]
                     function(channel, **kwargs)
             finally:
                 channel._executing = False
                 self._trace("execution finished")
         except KeyboardInterrupt:
             channel.close(INTERRUPT_TEXT)
             raise
-        except:
+        except BaseException:
             excinfo = self.exc_info()
             if not isinstance(excinfo[1], EOFError):
                 if not channel.gateway._channelfactory.finished:
-                    self._trace("got exception: {!r}".format(excinfo[1]))
+                    self._trace(f"got exception: {excinfo[1]!r}")
                     errortext = self._geterrortext(excinfo)
                     channel.close(errortext)
                     return
             self._trace("ignoring EOFError because receiving finished")
         channel.close()
 
 
@@ -1117,39 +1190,60 @@
     """Error while serializing an object."""
 
 
 class LoadError(DataFormatError):
     """Error while unserializing an object."""
 
 
-if ISPY3:
-
-    def bchr(n):
-        return bytes([n])
-
+def bchr(n):
+    return bytes([n])
 
-else:
-    bchr = chr
 
-DUMPFORMAT_VERSION = bchr(1)
+DUMPFORMAT_VERSION = bchr(2)
 
 FOUR_BYTE_INT_MAX = 2147483647
 
 FLOAT_FORMAT = "!d"
 FLOAT_FORMAT_SIZE = struct.calcsize(FLOAT_FORMAT)
 COMPLEX_FORMAT = "!dd"
 COMPLEX_FORMAT_SIZE = struct.calcsize(COMPLEX_FORMAT)
 
 
 class _Stop(Exception):
     pass
 
 
-class Unserializer(object):
-    num2func = {}  # is filled after this class definition
+class opcode:
+    """container for name -> num mappings."""
+
+    BUILDTUPLE = b"@"
+    BYTES = b"A"
+    CHANNEL = b"B"
+    FALSE = b"C"
+    FLOAT = b"D"
+    FROZENSET = b"E"
+    INT = b"F"
+    LONG = b"G"
+    LONGINT = b"H"
+    LONGLONG = b"I"
+    NEWDICT = b"J"
+    NEWLIST = b"K"
+    NONE = b"L"
+    PY2STRING = b"M"
+    PY3STRING = b"N"
+    SET = b"O"
+    SETITEM = b"P"
+    STOP = b"Q"
+    TRUE = b"R"
+    UNICODE = b"S"
+    COMPLEX = b"T"
+
+
+class Unserializer:
+    num2func: dict[bytes, Callable[[Unserializer], None]] = {}
     py2str_as_py3str = True  # True
     py3str_as_py2str = False  # false means py2 will get unicode
 
     def __init__(self, stream, channel_or_gateway=None, strconfig=None):
         gateway = getattr(channel_or_gateway, "gateway", channel_or_gateway)
         strconfig = getattr(channel_or_gateway, "_strconfig", strconfig)
         if strconfig:
@@ -1168,158 +1262,162 @@
                 opcode = self.stream.read(1)
                 if not opcode:
                     raise EOFError
                 try:
                     loader = self.num2func[opcode]
                 except KeyError:
                     raise LoadError(
-                        "unkown opcode %r - " "wire protocol corruption?" % (opcode,)
+                        "unknown opcode %r - " "wire protocol corruption?" % (opcode,)
                     )
                 loader(self)
         except _Stop:
             if len(self.stack) != 1:
                 raise LoadError("internal unserialization error")
             return self.stack.pop(0)
         else:
             raise LoadError("didn't get STOP")
 
     def load_none(self):
         self.stack.append(None)
 
+    num2func[opcode.NONE] = load_none
+
     def load_true(self):
         self.stack.append(True)
 
+    num2func[opcode.TRUE] = load_true
+
     def load_false(self):
         self.stack.append(False)
 
+    num2func[opcode.FALSE] = load_false
+
     def load_int(self):
         i = self._read_int4()
         self.stack.append(i)
 
+    num2func[opcode.INT] = load_int
+
     def load_longint(self):
         s = self._read_byte_string()
         self.stack.append(int(s))
 
-    if ISPY3:
-        load_long = load_int
-        load_longlong = load_longint
-    else:
+    num2func[opcode.LONGINT] = load_longint
 
-        def load_long(self):
-            i = self._read_int4()
-            self.stack.append(long(i))
-
-        def load_longlong(self):
-            l = self._read_byte_string()
-            self.stack.append(long(l))
+    load_long = load_int
+    num2func[opcode.LONG] = load_long
+    load_longlong = load_longint
+    num2func[opcode.LONGLONG] = load_longlong
 
     def load_float(self):
         binary = self.stream.read(FLOAT_FORMAT_SIZE)
         self.stack.append(struct.unpack(FLOAT_FORMAT, binary)[0])
 
+    num2func[opcode.FLOAT] = load_float
+
     def load_complex(self):
         binary = self.stream.read(COMPLEX_FORMAT_SIZE)
         self.stack.append(complex(*struct.unpack(COMPLEX_FORMAT, binary)))
 
+    num2func[opcode.COMPLEX] = load_complex
+
     def _read_int4(self):
         return struct.unpack("!i", self.stream.read(4))[0]
 
     def _read_byte_string(self):
         length = self._read_int4()
         as_bytes = self.stream.read(length)
         return as_bytes
 
     def load_py3string(self):
         as_bytes = self._read_byte_string()
-        if not ISPY3 and self.py3str_as_py2str:
+        if self.py3str_as_py2str:
             # XXX Should we try to decode into latin-1?
             self.stack.append(as_bytes)
         else:
             self.stack.append(as_bytes.decode("utf-8"))
 
+    num2func[opcode.PY3STRING] = load_py3string
+
     def load_py2string(self):
         as_bytes = self._read_byte_string()
-        if ISPY3 and self.py2str_as_py3str:
+        if self.py2str_as_py3str:
             s = as_bytes.decode("latin-1")
         else:
             s = as_bytes
         self.stack.append(s)
 
+    num2func[opcode.PY2STRING] = load_py2string
+
     def load_bytes(self):
         s = self._read_byte_string()
         self.stack.append(s)
 
+    num2func[opcode.BYTES] = load_bytes
+
     def load_unicode(self):
         self.stack.append(self._read_byte_string().decode("utf-8"))
 
+    num2func[opcode.UNICODE] = load_unicode
+
     def load_newlist(self):
         length = self._read_int4()
         self.stack.append([None] * length)
 
+    num2func[opcode.NEWLIST] = load_newlist
+
     def load_setitem(self):
         if len(self.stack) < 3:
             raise LoadError("not enough items for setitem")
         value = self.stack.pop()
         key = self.stack.pop()
         self.stack[-1][key] = value
 
+    num2func[opcode.SETITEM] = load_setitem
+
     def load_newdict(self):
         self.stack.append({})
 
+    num2func[opcode.NEWDICT] = load_newdict
+
     def _load_collection(self, type_):
         length = self._read_int4()
         if length:
             res = type_(self.stack[-length:])
             del self.stack[-length:]
             self.stack.append(res)
         else:
             self.stack.append(type_())
 
     def load_buildtuple(self):
         self._load_collection(tuple)
 
+    num2func[opcode.BUILDTUPLE] = load_buildtuple
+
     def load_set(self):
         self._load_collection(set)
 
+    num2func[opcode.SET] = load_set
+
     def load_frozenset(self):
         self._load_collection(frozenset)
 
+    num2func[opcode.FROZENSET] = load_frozenset
+
     def load_stop(self):
         raise _Stop
 
+    num2func[opcode.STOP] = load_stop
+
     def load_channel(self):
         id = self._read_int4()
         newchannel = self.channelfactory.new(id)
         self.stack.append(newchannel)
 
-
-# automatically build opcodes and byte-encoding
-
-
-class opcode:
-    """container for name -> num mappings."""
-
-
-def _buildopcodes():
-    l = []
-    later_added = {"COMPLEX": 1}
-    for name, func in Unserializer.__dict__.items():
-        if name.startswith("load_"):
-            opname = name[5:].upper()
-            l.append((opname, func))
-    l.sort(key=lambda x: (later_added.get(x[0], 0), x[0]))
-
-    for i, (opname, func) in enumerate(l):
-        assert i < 26, "xxx"
-        i = bchr(64 + i)
-        Unserializer.num2func[i] = func
-        setattr(opcode, opname, i)
-
-
-_buildopcodes()
+    num2func[opcode.CHANNEL] = load_channel
 
 
 def dumps(obj):
     """return a serialized bytestring of the given obj.
 
     The obj and all contained objects must be of a builtin
     python type (so nested dicts, sets, etc. are all ok but
@@ -1367,46 +1465,46 @@
     return Unserializer(io, channelfactory, strconfig).load()
 
 
 def dumps_internal(obj):
     return _Serializer().save(obj)
 
 
-class _Serializer(object):
-    _dispatch = {}
+class _Serializer:
+    _dispatch: dict[type, Callable[[_Serializer, object], None]] = {}
 
     def __init__(self, write=None):
         if write is None:
             self._streamlist = []
             write = self._streamlist.append
         self._write = write
 
     def save(self, obj, versioned=False):
         # calling here is not re-entrant but multiple instances
         # may write to the same stream because of the common platform
-        # atomic-write guaruantee (concurrent writes each happen atomicly)
+        # atomic-write guarantee (concurrent writes each happen atomically)
         if versioned:
             self._write(DUMPFORMAT_VERSION)
         self._save(obj)
         self._write(opcode.STOP)
         try:
             streamlist = self._streamlist
         except AttributeError:
             return None
-        return type(streamlist[0])().join(streamlist)
+        return b"".join(streamlist)
 
     def _save(self, obj):
         tp = type(obj)
         try:
             dispatch = self._dispatch[tp]
         except KeyError:
             methodname = "save_" + tp.__name__
             meth = getattr(self.__class__, methodname, None)
             if meth is None:
-                raise DumpError("can't serialize {}".format(tp))
+                raise DumpError(f"can't serialize {tp}")
             dispatch = self._dispatch[tp] = meth
         dispatch(self, obj)
 
     def save_NoneType(self, non):
         self._write(opcode.NONE)
 
     def save_bool(self, boolean):
@@ -1415,29 +1513,17 @@
         else:
             self._write(opcode.FALSE)
 
     def save_bytes(self, bytes_):
         self._write(opcode.BYTES)
         self._write_byte_sequence(bytes_)
 
-    if ISPY3:
-
-        def save_str(self, s):
-            self._write(opcode.PY3STRING)
-            self._write_unicode_string(s)
-
-    else:
-
-        def save_str(self, s):
-            self._write(opcode.PY2STRING)
-            self._write_byte_sequence(s)
-
-        def save_unicode(self, s):
-            self._write(opcode.UNICODE)
-            self._write_unicode_string(s)
+    def save_str(self, s):
+        self._write(opcode.PY3STRING)
+        self._write_unicode_string(s)
 
     def _write_unicode_string(self, s):
         try:
             as_bytes = s.encode("utf-8")
         except UnicodeEncodeError:
             raise DumpError("strings must be utf-8 encodable")
         self._write_byte_sequence(as_bytes)
@@ -1546,9 +1632,9 @@
         io = Popen2IO(stdout, stdin, execmodel)
         sys.stdin = execmodel.fdopen(0, "r", 1)
         sys.stdout = execmodel.fdopen(1, "w", 1)
     return io
 
 
 def serve(io, id):
-    trace("creating workergateway on {!r}".format(io))
+    trace(f"creating workergateway on {io!r}")
     WorkerGateway(io=io, id=id, _startcount=2).serve()
```

### Comparing `execnet-1.9.0/execnet/gateway_bootstrap.py` & `execnet-2.0.0/src/execnet/gateway_bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 code to initialize the remote side of a gateway once the io is created
 """
 import inspect
 import os
 
 import execnet
@@ -29,29 +28,29 @@
         "from execnet.gateway_base import serve, init_popen_io, get_execmodel",
         "sys.stdout.write('1')",
         "sys.stdout.flush()",
         "execmodel = get_execmodel(%r)" % spec.execmodel,
         "serve(init_popen_io(execmodel), id='%s-worker')" % spec.id,
     )
     s = io.read(1)
-    assert s == "1".encode("ascii"), repr(s)
+    assert s == b"1", repr(s)
 
 
 def bootstrap_exec(io, spec):
     try:
         sendexec(
             io,
             inspect.getsource(gateway_base),
             "execmodel = get_execmodel(%r)" % spec.execmodel,
             "io = init_popen_io(execmodel)",
             "io.write('1'.encode('ascii'))",
             "serve(io, id='%s-worker')" % spec.id,
         )
         s = io.read(1)
-        assert s == "1".encode("ascii")
+        assert s == b"1"
     except EOFError:
         ret = io.wait()
         if ret == 255:
             raise HostNotFound(io.remoteaddress)
 
 
 def bootstrap_socket(io, id):
@@ -67,20 +66,20 @@
         "except NameError:",
         "   execmodel = get_execmodel('thread')",
         "io = SocketIO(clientsock, execmodel)",
         "io.write('1'.encode('ascii'))",
         "serve(io, id='%s-worker')" % id,
     )
     s = io.read(1)
-    assert s == "1".encode("ascii")
+    assert s == b"1"
 
 
 def sendexec(io, *sources):
     source = "\n".join(sources)
-    io.write((repr(source) + "\n").encode("ascii"))
+    io.write((repr(source) + "\n").encode("utf-8"))
 
 
 def fix_pid_for_jython_popen(gw):
     """
     fix for jython 2.5.1
     """
     spec, io = gw.spec, gw._io
@@ -100,11 +99,11 @@
         else:
             bootstrap_import(io, spec)
     elif spec.ssh or spec.vagrant_ssh:
         bootstrap_exec(io, spec)
     elif spec.socket:
         bootstrap_socket(io, spec)
     else:
-        raise ValueError("unknown gateway type, cant bootstrap")
+        raise ValueError("unknown gateway type, can't bootstrap")
     gw = Gateway(io, spec)
     fix_pid_for_jython_popen(gw)
     return gw
```

### Comparing `execnet-1.9.0/execnet/gateway_io.py` & `execnet-2.0.0/src/execnet/gateway_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,48 @@
-# -*- coding: utf-8 -*-
 """
 execnet io initialization code
 
 creates io instances used for gateway io
 """
 import os
 import shlex
 import sys
 
 try:
     from execnet.gateway_base import Popen2IO, Message
 except ImportError:
-    from __main__ import Popen2IO, Message
+    from __main__ import Popen2IO, Message  # type: ignore[no-redef]
 
 from functools import partial
 
 
 class Popen2IOMaster(Popen2IO):
     def __init__(self, args, execmodel):
-        self.popen = p = execmodel.PopenPiped(args)
-        Popen2IO.__init__(self, p.stdin, p.stdout, execmodel=execmodel)
+        PIPE = execmodel.subprocess.PIPE
+        self.popen = p = execmodel.subprocess.Popen(args, stdout=PIPE, stdin=PIPE)
+        super().__init__(p.stdin, p.stdout, execmodel=execmodel)
 
     def wait(self):
         try:
             return self.popen.wait()
         except OSError:
             pass  # subprocess probably dead already
 
     def kill(self):
         killpopen(self.popen)
 
 
 def killpopen(popen):
     try:
-        if hasattr(popen, "kill"):
-            popen.kill()
-        else:
-            killpid(popen.pid)
-    except EnvironmentError:
-        sys.stderr.write("ERROR killing: %s\n" % (sys.exc_info()[1]))
+        popen.kill()
+    except OSError as e:
+        sys.stderr.write("ERROR killing: %s\n" % e)
         sys.stderr.flush()
 
 
-def killpid(pid):
-    if hasattr(os, "kill"):
-        os.kill(pid, 15)
-    elif sys.platform == "win32" or getattr(os, "_name", None) == "nt":
-        import ctypes
-
-        PROCESS_TERMINATE = 1
-        handle = ctypes.windll.kernel32.OpenProcess(PROCESS_TERMINATE, False, pid)
-        ctypes.windll.kernel32.TerminateProcess(handle, -1)
-        ctypes.windll.kernel32.CloseHandle(handle)
-    else:
-        raise EnvironmentError("no method to kill {}".format(pid))
-
-
 popen_bootstrapline = "import sys;exec(eval(sys.stdin.readline()))"
 
 
 def shell_split_path(path):
     """
     Use shell lexer to split the given path into a list of components,
     taking care to handle Windows' '\' correctly.
@@ -69,33 +52,31 @@
         path = path.replace("\\", "/")
     return shlex.split(path)
 
 
 def popen_args(spec):
     args = shell_split_path(spec.python) if spec.python else [sys.executable]
     args.append("-u")
-    if spec is not None and spec.dont_write_bytecode:
+    if spec.dont_write_bytecode:
         args.append("-B")
-    # Slight gymnastics in ordering these arguments because CPython (as of
-    # 2.7.1) ignores -B if you provide `python -c "something" -B`
     args.extend(["-c", popen_bootstrapline])
     return args
 
 
 def ssh_args(spec):
     # NOTE: If changing this, you need to sync those changes to vagrant_args
     # as well, or, take some time to further refactor the commonalities of
     # ssh_args and vagrant_args.
     remotepython = spec.python or "python"
     args = ["ssh", "-C"]
     if spec.ssh_config is not None:
         args.extend(["-F", str(spec.ssh_config)])
 
     args.extend(spec.ssh.split())
-    remotecmd = '{} -c "{}"'.format(remotepython, popen_bootstrapline)
+    remotecmd = f'{remotepython} -c "{popen_bootstrapline}"'
     args.append(remotecmd)
     return args
 
 
 def vagrant_ssh_args(spec):
     # This is the vagrant-wrapped version of SSH. Unfortunately the
     # command lines are incompatible to just channel through ssh_args
@@ -103,15 +84,15 @@
     # NOTE: This should be kept in sync with the ssh_args behaviour.
     # spec.vagrant is identical to spec.ssh in that they both carry
     # the remote host "address".
     remotepython = spec.python or "python"
     args = ["vagrant", "ssh", spec.vagrant_ssh, "--", "-C"]
     if spec.ssh_config is not None:
         args.extend(["-F", str(spec.ssh_config)])
-    remotecmd = '{} -c "{}"'.format(remotepython, popen_bootstrapline)
+    remotecmd = f'{remotepython} -c "{popen_bootstrapline}"'
     args.extend([remotecmd])
     return args
 
 
 def create_io(spec, execmodel):
     if spec.popen:
         args = popen_args(spec)
@@ -137,15 +118,15 @@
 
 RIO_KILL = 1
 RIO_WAIT = 2
 RIO_REMOTEADDRESS = 3
 RIO_CLOSE_WRITE = 4
 
 
-class ProxyIO(object):
+class ProxyIO:
     """A Proxy IO object allows to instantiate a Gateway
     through another "via" gateway.  A master:ProxyIO object
     provides an IO object effectively connected to the sub
     via the forwarder.  To achieve this, master:ProxyIO interacts
     with forwarder:serve_proxy_io() which itself
     instantiates and interacts with the sub.
     """
@@ -179,15 +160,15 @@
         return self._controll(RIO_WAIT)
 
     @property
     def remoteaddress(self):
         return self._controll(RIO_REMOTEADDRESS)
 
     def __repr__(self):
-        return "<RemoteIO via {}>".format(self.iochan.gateway.id)
+        return f"<RemoteIO via {self.iochan.gateway.id}>"
 
 
 class PseudoSpec:
     def __init__(self, vars):
         self.__dict__.update(vars)
 
     def __getattr__(self, name):
@@ -209,33 +190,33 @@
     # XXX writing might block, thus blocking the receiver thread
     def forward_to_sub(data):
         log("forward data to sub, size %s" % len(data))
         sub_io.write(data)
 
     proxy_channelX.setcallback(forward_to_sub)
 
-    def controll(data):
+    def control(data):
         if data == RIO_WAIT:
             control_chan.send(sub_io.wait())
         elif data == RIO_KILL:
             control_chan.send(sub_io.kill())
         elif data == RIO_REMOTEADDRESS:
             control_chan.send(sub_io.remoteaddress)
         elif data == RIO_CLOSE_WRITE:
             control_chan.send(sub_io.close_write())
 
-    control_chan.setcallback(controll)
+    control_chan.setcallback(control)
 
     # write data to the master coming from the sub
     forward_to_master_file = proxy_channelX.makefile("w")
 
     # read bootstrap byte from sub, send it on to master
     log("reading bootstrap byte from sub", spec.id)
     initial = sub_io.read(1)
-    assert initial == "1".encode("ascii"), initial
+    assert initial == b"1", initial
     log("forwarding bootstrap byte from sub", spec.id)
     forward_to_master_file.write(initial)
 
     # enter message forwarding loop
     while True:
         try:
             message = Message.from_io(sub_io)
@@ -243,8 +224,8 @@
             log("EOF from sub, terminating proxying loop", spec.id)
             break
         message.to_io(forward_to_master_file)
     # proxy_channelX will be closed from remote_exec's finalization code
 
 
 if __name__ == "__channelexec__":
-    serve_proxy_io(channel)  # noqa
+    serve_proxy_io(channel)  # type: ignore[name-defined]
```

### Comparing `execnet-1.9.0/execnet/gateway_socket.py` & `execnet-2.0.0/src/execnet/gateway_socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-# -*- coding: utf-8 -*-
 import sys
 
 from execnet.gateway_bootstrap import HostNotFound
 
-try:
-    bytes
-except NameError:
-    bytes = str
-
 
 class SocketIO:
     def __init__(self, sock, execmodel):
         self.sock = sock
         self.execmodel = execmodel
         socket = execmodel.socket
         try:
             # IPTOS_LOWDELAY
             sock.setsockopt(socket.SOL_IP, socket.IP_TOS, 0x10)
             sock.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
-        except (AttributeError, socket.error):
+        except (AttributeError, OSError):
             sys.stderr.write("WARNING: cannot set socketoption")
 
     def read(self, numbytes):
         "Read exactly 'bytes' bytes from the socket."
-        buf = bytes()
+        buf = b""
         while len(buf) < numbytes:
             t = self.sock.recv(numbytes - len(buf))
             if not t:
                 raise EOFError
             buf += t
         return buf
 
@@ -51,15 +45,15 @@
 
     def kill(self):
         pass
 
 
 def start_via(gateway, hostport=None):
     """return a host, port tuple,
-    after instanciating a socketserver on the given gateway
+    after instantiating a socketserver on the given gateway
     """
     if hostport is None:
         host, port = ("localhost", 0)
     else:
         host, port = hostport
 
     from execnet.script import socketserver
```

### Comparing `execnet-1.9.0/execnet/multi.py` & `execnet-2.0.0/src/execnet/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
 """
 Managing Gateway Groups and interactions with multiple channels.
 
 (c) 2008-2014, Holger Krekel and others
 """
 import atexit
 import sys
 from functools import partial
 from threading import Lock
 
 from . import gateway_bootstrap
 from . import gateway_io
 from .gateway_base import get_execmodel
-from .gateway_base import reraise
 from .gateway_base import trace
+from .gateway_base import WorkerPool
 from .xspec import XSpec
 
 NO_ENDMARKER_WANTED = object()
 
 
-class Group(object):
+class Group:
     """Gateway Groups."""
 
     defaultspec = "popen"
 
     def __init__(self, xspecs=(), execmodel="thread"):
         """initialize group and make gateways as specified.
         execmodel can be 'thread' or 'eventlet'.
@@ -134,15 +133,15 @@
             gw = gateway_bootstrap.bootstrap(io, spec)
         elif spec.socket:
             from . import gateway_socket
 
             io = gateway_socket.create_io(spec, self, execmodel=self.execmodel)
             gw = gateway_bootstrap.bootstrap(io, spec)
         else:
-            raise ValueError("no gateway type found for {!r}".format(spec._spec))
+            raise ValueError(f"no gateway type found for {spec._spec!r}")
         gw.spec = spec
         self._register(gw)
         if spec.chdir or spec.nice or spec.env:
             channel = gw.remote_exec(
                 """
                 import os
                 path, nice, env = channel.receive()
@@ -165,30 +164,30 @@
     def allocate_id(self, spec):
         """(re-entrant) allocate id for the given xspec object."""
         if spec.id is None:
             with self._autoidlock:
                 id = "gw" + str(self._autoidcounter)
                 self._autoidcounter += 1
                 if id in self:
-                    raise ValueError("already have gateway with id {!r}".format(id))
+                    raise ValueError(f"already have gateway with id {id!r}")
                 spec.id = id
 
     def _register(self, gateway):
         assert not hasattr(gateway, "_group")
         assert gateway.id
-        assert id not in self
+        assert gateway.id not in self
         self._gateways.append(gateway)
         gateway._group = self
 
     def _unregister(self, gateway):
         self._gateways.remove(gateway)
         self._gateways_to_join.append(gateway)
 
     def _cleanup_atexit(self):
-        trace("=== atexit cleanup {!r} ===".format(self))
+        trace(f"=== atexit cleanup {self!r} ===")
         self.terminate(timeout=1.0)
 
     def terminate(self, timeout=None):
         """trigger exit of member gateways and wait for termination
         of member gateways and associated subprocesses.  After waiting
         timeout seconds try to to kill local sub processes of popen-
         and ssh-gateways.  Timeout defaults to None meaning
@@ -286,25 +285,25 @@
         for ch in self._channels:
             try:
                 ch.waitclose()
             except ch.RemoteError:
                 if first is None:
                     first = sys.exc_info()
         if first:
-            reraise(*first)
+            raise first[1].with_traceback(first[2])
 
 
 def safe_terminate(execmodel, timeout, list_of_paired_functions):
-    workerpool = execmodel.WorkerPool()
+    workerpool = WorkerPool(execmodel)
 
     def termkill(termfunc, killfunc):
         termreply = workerpool.spawn(termfunc)
         try:
             termreply.get(timeout=timeout)
-        except IOError:
+        except OSError:
             killfunc()
 
     replylist = []
     for termfunc, killfunc in list_of_paired_functions:
         reply = workerpool.spawn(termkill, termfunc, killfunc)
         replylist.append(reply)
     for reply in replylist:
```

### Comparing `execnet-1.9.0/execnet/rsync.py` & `execnet-2.0.0/src/execnet/rsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-# -*- coding: utf-8 -*-
 """
-1:N rsync implemenation on top of execnet.
+1:N rsync implementation on top of execnet.
 
 (c) 2006-2009, Armin Rigo, Holger Krekel, Maciej Fijalkowski
 """
 import os
 import stat
 from hashlib import md5
-
-try:
-    from queue import Queue
-except ImportError:
-    from Queue import Queue
+from queue import Queue
 
 import execnet.rsync_remote
 
 
-class RSync(object):
+class RSync:
     """This class allows to send a directory structure (recursively)
     to one or multiple remote filesystems.
 
     There is limited support for symlinks, which means that symlinks
     pointing to the sourcetree will be send "as is" while external
-    symlinks will be just copied (regardless of existance of such
+    symlinks will be just copied (regardless of existence of such
     a path on remote side).
     """
 
     def __init__(self, sourcedir, callback=None, verbose=True):
         self._sourcedir = str(sourcedir)
         self._verbose = verbose
         assert callback is None or hasattr(callback, "__call__")
@@ -39,15 +34,15 @@
         return True
 
     def _end_of_channel(self, channel):
         if channel in self._channels:
             # too early!  we must have got an error
             channel.waitclose()
             # or else we raise one
-            raise IOError("connection unexpectedly closed: {} ".format(channel.gateway))
+            raise OSError(f"connection unexpectedly closed: {channel.gateway} ")
 
     def _process_link(self, channel):
         for link in self._links:
             channel.send(link)
         # completion marker, this host is done
         channel.send(42)
 
@@ -67,15 +62,15 @@
     def _send_item(self, channel, data):
         """Send one item"""
         modified_rel_path, checksum = data
         modifiedpath = os.path.join(self._sourcedir, *modified_rel_path)
         try:
             f = open(modifiedpath, "rb")
             data = f.read()
-        except IOError:
+        except OSError:
             data = None
 
         # provide info to progress callback function
         modified_rel_path = "/".join(modified_rel_path)
         if data is not None:
             self._paths[modified_rel_path] = len(data)
         else:
@@ -91,24 +86,24 @@
                 data = None  # not really modified
             else:
                 self._report_send_file(channel.gateway, modified_rel_path)
         channel.send(data)
 
     def _report_send_file(self, gateway, modified_rel_path):
         if self._verbose:
-            print("{} <= {}".format(gateway, modified_rel_path))
+            print(f"{gateway} <= {modified_rel_path}")
 
     def send(self, raises=True):
         """Sends a sourcedir to all added targets. Flag indicates
         whether to raise an error or return in case of lack of
         targets
         """
         if not self._channels:
             if raises:
-                raise IOError(
+                raise OSError(
                     "no targets available, maybe you " "are trying call send() twice?"
                 )
             return
         # normalize a trailing '/' away
         self._sourcedir = os.path.dirname(os.path.join(self._sourcedir, "x"))
         # send directory structure and file timestamps/sizes
         self._send_directory_structure(self._sourcedir)
@@ -174,18 +169,34 @@
                 subpaths.append(p)
         mode = os.lstat(path).st_mode
         self._broadcast([mode] + names)
         for p in subpaths:
             self._send_directory_structure(p)
 
     def _send_link_structure(self, path):
-        linkpoint = os.readlink(path)
+        sourcedir = self._sourcedir
         basename = path[len(self._sourcedir) + 1 :]
-        if linkpoint.startswith(self._sourcedir):
-            self._send_link("linkbase", basename, linkpoint[len(self._sourcedir) + 1 :])
+        linkpoint = os.readlink(path)
+        # On Windows, readlink returns an extended path (//?/) for
+        # absolute links, but relpath doesn't like mixing extended
+        # and non-extended paths. So fix it up ourselves.
+        if (
+            os.path.__name__ == "ntpath"
+            and linkpoint.startswith("\\\\?\\")
+            and not self._sourcedir.startswith("\\\\?\\")
+        ):
+            sourcedir = "\\\\?\\" + self._sourcedir
+        try:
+            relpath = os.path.relpath(linkpoint, sourcedir)
+        except ValueError:
+            relpath = None
+        if relpath not in (None, os.curdir, os.pardir) and not relpath.startswith(
+            os.pardir + os.sep
+        ):
+            self._send_link("linkbase", basename, relpath)
         else:
             # relative or absolute link, just send it
             self._send_link("link", basename, linkpoint)
         self._broadcast(None)
 
     def _send_directory_structure(self, path):
         try:
@@ -197,8 +208,8 @@
             # regular file: send a mode/timestamp/size pair
             self._broadcast((st.st_mode, st.st_mtime, st.st_size))
         elif stat.S_ISDIR(st.st_mode):
             self._send_directory(path)
         elif stat.S_ISLNK(st.st_mode):
             self._send_link_structure(path)
         else:
-            raise ValueError("cannot sync {!r}".format(path))
+            raise ValueError(f"cannot sync {path!r}")
```

### Comparing `execnet-1.9.0/execnet/rsync_remote.py` & `execnet-2.0.0/src/execnet/rsync_remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 (c) 2006-2013, Armin Rigo, Holger Krekel, Maciej Fijalkowski
 """
 
 
 def serve_rsync(channel):
     import os
@@ -31,15 +30,19 @@
             if st and not stat.S_ISDIR(st.st_mode):
                 os.unlink(path)
                 st = None
             if not st:
                 os.makedirs(path)
             mode = msg.pop(0)
             if mode:
-                os.chmod(path, mode)
+                # Ensure directories are writable, otherwise a
+                # permission denied error (EACCES) would be raised
+                # when attempting to receive read-only directory
+                # structures.
+                os.chmod(path, mode | 0o700)
             entrynames = {}
             for entryname in msg:
                 destpath = os.path.join(path, entryname)
                 receive_directory_structure(destpath, relcomponents + [entryname])
                 entrynames[entryname] = True
             if options.get("delete"):
                 for othername in os.listdir(path):
@@ -55,15 +58,15 @@
                     if msg_size != st.st_size:
                         pass
                     elif msg_mtime != st.st_mtime:
                         f = open(path, "rb")
                         checksum = md5(f.read()).digest()
                         f.close()
                     elif msg_mode and msg_mode != st.st_mode:
-                        os.chmod(path, msg_mode)
+                        os.chmod(path, msg_mode | 0o700)
                         return
                     else:
                         return  # already fine
                 else:
                     remove(path)
             channel.send(("send", (relcomponents, checksum)))
             modifiedfiles.append((path, msg))
@@ -74,15 +77,15 @@
     channel.send(("list_done", None))
 
     for path, (mode, time, size) in modifiedfiles:
         data = channel.receive()
         channel.send(("ack", path[len(destdir) + 1 :]))
         if data is not None:
             if STRICT_CHECK and len(data) != size:
-                raise IOError("file modified during rsync: {!r}".format(path))
+                raise OSError(f"file modified during rsync: {path!r}")
             f = open(path, "wb")
             f.write(data)
             f.close()
         try:
             if mode:
                 os.chmod(path, mode)
             os.utime(path, (time, time))
@@ -107,8 +110,8 @@
             src = linkpoint
         os.symlink(src, path)
         msg = channel.receive()
     channel.send(("done", None))
 
 
 if __name__ == "__channelexec__":
-    serve_rsync(channel)  # noqa
+    serve_rsync(channel)  # type: ignore[name-defined]
```

### Comparing `execnet-1.9.0/execnet/script/shell.py` & `execnet-2.0.0/src/execnet/script/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #! /usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 a remote python shell
 
 for injection into startserver.py
 """
 import os
 import select
@@ -13,15 +12,15 @@
 from traceback import print_exc
 
 
 def clientside():
     print("client side starting")
     host, port = sys.argv[1].split(":")
     port = int(port)
-    myself = open(os.path.abspath(sys.argv[0]), "rU").read()
+    myself = open(os.path.abspath(sys.argv[0])).read()
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.connect((host, port))
     sock.sendall(repr(myself) + "\n")
     print("send boot string")
     inputlist = [sock, sys.stdin]
     try:
         while 1:
@@ -29,26 +28,26 @@
             if sys.stdin in r:
                 line = raw_input()
                 sock.sendall(line + "\n")
             if sock in r:
                 line = sock.recv(4096)
                 sys.stdout.write(line)
                 sys.stdout.flush()
-    except:
+    except BaseException:
         import traceback
 
         print(traceback.print_exc())
 
     sys.exit(1)
 
 
 class promptagent(Thread):
     def __init__(self, clientsock):
         print("server side starting")
-        Thread.__init__(self)
+        super.__init__()
         self.clientsock = clientsock
 
     def run(self):
         print("Entering thread prompt loop")
         clientfile = self.clientsock.makefile("w")
 
         filein = self.clientsock.makefile("r")
@@ -63,15 +62,15 @@
                     raise EOFError("nothing")
                 if line.strip():
                     oldout, olderr = sys.stdout, sys.stderr
                     sys.stdout, sys.stderr = clientfile, clientfile
                     try:
                         try:
                             exec(compile(line + "\n", "<remote pyin>", "single"))
-                        except:
+                        except BaseException:
                             print_exc()
                     finally:
                         sys.stdout = oldout
                         sys.stderr = olderr
                 clientfile.flush()
             except EOFError:
                 sys.stderr.write("connection close, prompt thread returns")
```

### Comparing `execnet-1.9.0/execnet/script/socketserver.py` & `execnet-2.0.0/src/execnet/script/socketserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #! /usr/bin/env python
-# -*- coding: utf-8 -*-
 """
     start socket based minimal readline exec server
 
     it can exeuted in 2 modes of operation
 
     1. as normal script, that listens for new connections
 
@@ -36,24 +35,18 @@
     sys.stdout = sys.stderr = f
 
 
 def print_(*args):
     print(" ".join(str(arg) for arg in args))
 
 
-if sys.version_info > (3, 0):
-    exec(
-        """def exec_(source, locs):
+exec(
+    """def exec_(source, locs):
     exec(source, locs)"""
-    )
-else:
-    exec(
-        """def exec_(source, locs):
-    exec source in locs"""
-    )
+)
 
 
 def exec_from_one_connection(serversock):
     print_(progname, "Entering Accept loop", serversock.getsockname())
     clientsock, address = serversock.accept()
     print_(progname, "got new connection from %s %s" % address)
     clientfile = clientsock.makefile("rb")
@@ -97,15 +90,15 @@
     execute_path = os.getcwd()
     try:
         while 1:
             try:
                 exec_from_one_connection(serversock)
             except (KeyboardInterrupt, SystemExit):
                 raise
-            except:
+            except BaseException:
                 if debug:
                     import traceback
 
                     traceback.print_exc()
                 else:
                     excinfo = sys.exc_info()
                     print_("got exception", excinfo[1])
```

### Comparing `execnet-1.9.0/execnet/script/socketserverservice.py` & `execnet-2.0.0/src/execnet/script/socketserverservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 A windows service wrapper for the py.execnet socketserver.
 
 To use, run:
  python socketserverservice.py register
  net start ExecNetSocketServer
 """
@@ -33,15 +32,15 @@
         # so that it also could be removed if the service is uninstalled.
         # Unfortunately it cannot be done in the 'if __name__ == "__main__"'
         # block below, because the 'frozen' exe-file does not run this code.
         #
         win32evtlogutil.AddSourceToRegistry(
             self._svc_display_name_, servicemanager.__file__, "Application"
         )
-        win32serviceutil.ServiceFramework.__init__(self, args)
+        super.__init__(args)
         self.hWaitStop = win32event.CreateEvent(None, 0, 0, None)
         self.WAIT_TIME = 1000  # in milliseconds
 
     def SvcStop(self):
         self.ReportServiceStatus(win32service.SERVICE_STOP_PENDING)
         win32event.SetEvent(self.hWaitStop)
```

### Comparing `execnet-1.9.0/execnet/xspec.py` & `execnet-2.0.0/src/execnet/xspec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 (c) 2008-2013, holger krekel
 """
 
 
 class XSpec:
     """Execution Specification: key1=value1//key2=value2 ...
@@ -26,27 +25,27 @@
             if i == -1:
                 key, value = keyvalue, True
             else:
                 key, value = keyvalue[:i], keyvalue[i + 1 :]
             if key[0] == "_":
                 raise AttributeError("%r not a valid XSpec key" % key)
             if key in self.__dict__:
-                raise ValueError("duplicate key: {!r} in {!r}".format(key, string))
+                raise ValueError(f"duplicate key: {key!r} in {string!r}")
             if key.startswith("env:"):
                 self.env[key[4:]] = value
             else:
                 setattr(self, key, value)
 
     def __getattr__(self, name):
         if name[0] == "_":
             raise AttributeError(name)
         return None
 
     def __repr__(self):
-        return "<XSpec {!r}>".format(self._spec)
+        return f"<XSpec {self._spec!r}>"
 
     def __str__(self):
         return self._spec
 
     def __hash__(self):
         return hash(self._spec)
```

### Comparing `execnet-1.9.0/setup.py` & `execnet-2.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,61 @@
-# -*- coding: utf-8 -*-
-def main():
-    from setuptools import setup
-
-    with open("README.rst") as fp:
-        readme = fp.read()
-    setup(
-        name="execnet",
-        description="execnet: rapid multi-Python deployment",
-        long_description=readme,
-        use_scm_version={"write_to": "execnet/_version.py"},
-        url="https://execnet.readthedocs.io/en/latest/",
-        license="MIT",
-        platforms=["unix", "linux", "osx", "cygwin", "win32"],
-        author="holger krekel and others",
-        classifiers=[
-            "Development Status :: 5 - Production/Stable",
-            "Intended Audience :: Developers",
-            "License :: OSI Approved :: MIT License",
-            "Operating System :: POSIX",
-            "Operating System :: Microsoft :: Windows",
-            "Operating System :: MacOS :: MacOS X",
-            "Topic :: Software Development :: Libraries",
-            "Topic :: System :: Distributed Computing",
-            "Topic :: System :: Networking",
-            "Programming Language :: Python :: 2",
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.5",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: Implementation :: CPython",
-            "Programming Language :: Python :: Implementation :: PyPy",
-        ],
-        packages=["execnet", "execnet.script"],
-        python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
-        extras_require={"testing": ["pre-commit"]},
-        setup_requires=["setuptools_scm"],
-    )
+[build-system]
+requires = [
+    "hatchling",
+    "hatch-vcs",
+]
+build-backend = "hatchling.build"
 
+[project]
+name = "execnet"
+dynamic = ["version"]
+description = "execnet: rapid multi-Python deployment"
+readme = {"file" = "README.rst", "content-type" = "text/x-rst"}
+license = "MIT"
+requires-python = ">=3.7"
+authors = [
+    { name = "holger krekel and others" },
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: System :: Distributed Computing",
+    "Topic :: System :: Networking",
+]
 
-if __name__ == "__main__":
-    main()
+[project.optional-dependencies]
+testing = [
+    "pre-commit",
+    "pytest",
+    "tox",
+    "hatch",
+]
+
+[project.urls]
+Homepage = "https://execnet.readthedocs.io/en/latest/"
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/execnet/_version.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/src/execnet",
+]
+
+
+[tool.mypy]
+python_version = "3.7"
```

