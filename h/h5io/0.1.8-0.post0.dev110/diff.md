# Comparing `tmp/h5io-0.1.8.tar.gz` & `tmp/h5io-0.post0.dev110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5io-0.1.8.tar", last modified: Fri Jul  7 18:38:58 2023, max compression
+gzip compressed data, was "dist/h5io-0.post0.dev110.tar", last modified: Tue Aug 14 06:04:59 2018, max compression
```

## Comparing `h5io-0.1.8.tar` & `h5io-0.post0.dev110.tar`

### file list

```diff
@@ -1,26 +1,20 @@
-drwxrwxr-x   0 larsoner  (1000) larsoner  (1000)        0 2023-07-07 18:38:58.594373 h5io-0.1.8/
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)       93 2019-01-11 15:48:26.000000 h5io-0.1.8/.coveragerc
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)       30 2019-01-11 15:48:26.000000 h5io-0.1.8/.gitattributes
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)       97 2019-01-11 15:48:26.000000 h5io-0.1.8/.gitignore
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     2042 2022-02-11 19:41:56.000000 h5io-0.1.8/.travis.yml
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)     1514 2019-01-11 15:48:26.000000 h5io-0.1.8/LICENSE.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      839 2023-04-21 14:55:40.000000 h5io-0.1.8/Makefile
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     4157 2023-07-07 18:38:58.594373 h5io-0.1.8/PKG-INFO
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)     3421 2019-01-11 15:48:26.000000 h5io-0.1.8/README.rst
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      999 2022-03-21 14:37:31.000000 h5io-0.1.8/azure-pipelines.yml
-drwxrwxr-x   0 larsoner  (1000) larsoner  (1000)        0 2023-07-07 18:38:58.594373 h5io-0.1.8/h5io/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      224 2022-02-11 19:41:56.000000 h5io-0.1.8/h5io/__init__.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)    24366 2023-07-07 18:38:48.000000 h5io-0.1.8/h5io/_h5io.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)       22 2023-07-07 18:38:48.000000 h5io-0.1.8/h5io/_version.py
-drwxrwxr-x   0 larsoner  (1000) larsoner  (1000)        0 2023-07-07 18:38:58.594373 h5io-0.1.8/h5io/tests/
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)        0 2019-01-11 15:48:26.000000 h5io-0.1.8/h5io/tests/__init__.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)    10602 2023-07-07 18:38:48.000000 h5io-0.1.8/h5io/tests/test_io.py
-drwxrwxr-x   0 larsoner  (1000) larsoner  (1000)        0 2023-07-07 18:38:58.594373 h5io-0.1.8/h5io.egg-info/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     4157 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/PKG-INFO
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      379 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/SOURCES.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        1 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/dependency_links.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        1 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/not-zip-safe
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)       11 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/requires.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        5 2023-07-07 18:38:58.000000 h5io-0.1.8/h5io.egg-info/top_level.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      245 2023-07-07 18:38:58.594373 h5io-0.1.8/setup.cfg
--rwxrwxr-x   0 larsoner  (1000) larsoner  (1000)     2009 2022-03-21 14:37:31.000000 h5io-0.1.8/setup.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io/tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/h5io/tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7491 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/h5io/tests/test_io.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      283 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/h5io/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    22659 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/h5io/_h5io.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      505 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io/_version.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4882 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      287 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (2000) travis    (2000)        5 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/h5io.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       47 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     3421 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)      406 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/setup.cfg
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     1752 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    68611 2018-08-14 06:02:59.000000 h5io-0.post0.dev110/versioneer.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4882 2018-08-14 06:04:59.000000 h5io-0.post0.dev110/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `h5io-0.1.8/PKG-INFO` & `h5io-0.post0.dev110/h5io.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,115 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: h5io
-Version: 0.1.8
+Version: 0.post0.dev110
 Summary: Python Objects Onto HDF5
 Home-page: http://h5io.github.io
-Download-URL: http://github.com/h5io/h5io
 Maintainer: Eric Larson
 Maintainer-email: larson.eric.d@gmail.com
 License: BSD (3-clause)
+Download-URL: http://github.com/h5io/h5io
+Description: .. -*- mode: rst -*-
+        
+        |Travis|_ |Appveyor|_ |Codecov|_
+        
+        .. |Travis| image:: https://api.travis-ci.org/h5io/h5io.png?branch=master
+        .. _Travis: https://travis-ci.org/h5io/h5io
+        
+        .. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/puwaarmllxq5wfvm?svg=true
+        .. _Appveyor: https://ci.appveyor.com/project/larsoner/h5io/branch/master
+        
+        .. |Codecov| image:: https://codecov.io/gh/h5io/h5io/branch/master/graph/badge.svg
+        .. _Codecov: https://codecov.io/gh/h5io/h5io
+        
+        `h5io <http://h5io.github.io>`_
+        =======================================================
+        
+        h5io is a package designed to facilitate saving some standard Python
+        objects into the forward-compatible HDF5 format. It is a higher-level
+        package than ``h5py``.
+        
+        Get the latest code
+        ^^^^^^^^^^^^^^^^^^^
+        
+        To get the latest code using git, simply type::
+        
+            git clone git://github.com/h5io/h5io.git
+        
+        If you don't have git installed, you can download a zip or tarball
+        of the latest code: https://github.com/h5io/h5io/archives/master
+        
+        Install h5io
+        ^^^^^^^^^^^^
+        
+        As any Python packages, to install h5io, go in the source code directory
+        and do::
+        
+            python setup.py install
+        
+        or if you don't have admin access to your python setup (permission denied
+        when install) use::
+        
+            python setup.py install --user
+        
+        You can also install the latest release version with pip::
+        
+            pip install h5io --upgrade
+        
+        or for the latest development version (the most up to date)::
+        
+            pip install -e git+https://github.com/h5io/h5io#egg=h5io-dev --user
+        
+        Dependencies
+        ^^^^^^^^^^^^
+        
+        The required dependencies to build the software are ``h5py`` and ``numpy``.
+        ``scipy`` is required for sparse matrix IO support.
+        
+        Licensing
+        ^^^^^^^^^
+        
+        h5io is **BSD-licenced** (3 clause):
+        
+            This software is OSI Certified Open Source Software.
+            OSI Certified is a certification mark of the Open Source Initiative.
+        
+            Copyright (c) 2011, authors of h5io
+            All rights reserved.
+        
+            Redistribution and use in source and binary forms, with or without
+            modification, are permitted provided that the following conditions are met:
+        
+            * Redistributions of source code must retain the above copyright notice,
+              this list of conditions and the following disclaimer.
+        
+            * Redistributions in binary form must reproduce the above copyright notice,
+              this list of conditions and the following disclaimer in the documentation
+              and/or other materials provided with the distribution.
+        
+            * Neither the names of h5io authors nor the names of any
+              contributors may be used to endorse or promote products derived from
+              this software without specific prior written permission.
+        
+            **This software is provided by the copyright holders and contributors
+            "as is" and any express or implied warranties, including, but not
+            limited to, the implied warranties of merchantability and fitness for
+            a particular purpose are disclaimed. In no event shall the copyright
+            owner or contributors be liable for any direct, indirect, incidental,
+            special, exemplary, or consequential damages (including, but not
+            limited to, procurement of substitute goods or services; loss of use,
+            data, or profits; or business interruption) however caused and on any
+            theory of liability, whether in contract, strict liability, or tort
+            (including negligence or otherwise) arising in any way out of the use
+            of this software, even if advised of the possibility of such
+            damage.**
+        
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-License-File: LICENSE.txt
-
-.. -*- mode: rst -*-
-
-|Travis|_ |Appveyor|_ |Codecov|_
-
-.. |Travis| image:: https://api.travis-ci.org/h5io/h5io.png?branch=master
-.. _Travis: https://travis-ci.org/h5io/h5io
-
-.. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/puwaarmllxq5wfvm?svg=true
-.. _Appveyor: https://ci.appveyor.com/project/larsoner/h5io/branch/master
-
-.. |Codecov| image:: https://codecov.io/gh/h5io/h5io/branch/master/graph/badge.svg
-.. _Codecov: https://codecov.io/gh/h5io/h5io
-
-`h5io <http://h5io.github.io>`_
-=======================================================
-
-h5io is a package designed to facilitate saving some standard Python
-objects into the forward-compatible HDF5 format. It is a higher-level
-package than ``h5py``.
-
-Get the latest code
-^^^^^^^^^^^^^^^^^^^
-
-To get the latest code using git, simply type::
-
-    git clone git://github.com/h5io/h5io.git
-
-If you don't have git installed, you can download a zip or tarball
-of the latest code: https://github.com/h5io/h5io/archives/master
-
-Install h5io
-^^^^^^^^^^^^
-
-As any Python packages, to install h5io, go in the source code directory
-and do::
-
-    python setup.py install
-
-or if you don't have admin access to your python setup (permission denied
-when install) use::
-
-    python setup.py install --user
-
-You can also install the latest release version with pip::
-
-    pip install h5io --upgrade
-
-or for the latest development version (the most up to date)::
-
-    pip install -e git+https://github.com/h5io/h5io#egg=h5io-dev --user
-
-Dependencies
-^^^^^^^^^^^^
-
-The required dependencies to build the software are ``h5py`` and ``numpy``.
-``scipy`` is required for sparse matrix IO support.
-
-Licensing
-^^^^^^^^^
-
-h5io is **BSD-licenced** (3 clause):
-
-    This software is OSI Certified Open Source Software.
-    OSI Certified is a certification mark of the Open Source Initiative.
-
-    Copyright (c) 2011, authors of h5io
-    All rights reserved.
-
-    Redistribution and use in source and binary forms, with or without
-    modification, are permitted provided that the following conditions are met:
-
-    * Redistributions of source code must retain the above copyright notice,
-      this list of conditions and the following disclaimer.
-
-    * Redistributions in binary form must reproduce the above copyright notice,
-      this list of conditions and the following disclaimer in the documentation
-      and/or other materials provided with the distribution.
-
-    * Neither the names of h5io authors nor the names of any
-      contributors may be used to endorse or promote products derived from
-      this software without specific prior written permission.
-
-    **This software is provided by the copyright holders and contributors
-    "as is" and any express or implied warranties, including, but not
-    limited to, the implied warranties of merchantability and fitness for
-    a particular purpose are disclaimed. In no event shall the copyright
-    owner or contributors be liable for any direct, indirect, incidental,
-    special, exemplary, or consequential damages (including, but not
-    limited to, procurement of substitute goods or services; loss of use,
-    data, or profits; or business interruption) however caused and on any
-    theory of liability, whether in contract, strict liability, or tort
-    (including negligence or otherwise) arising in any way out of the use
-    of this software, even if advised of the possibility of such
-    damage.**
```

### Comparing `h5io-0.1.8/README.rst` & `h5io-0.post0.dev110/README.rst`

 * *Files identical despite different names*

### Comparing `h5io-0.1.8/h5io/_h5io.py` & `h5io-0.post0.dev110/h5io/_h5io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # -*- coding: utf-8 -*-
 # Authors: Eric Larson <larson.eric.d@gmail.com>
 #
 # License: BSD (3-clause)
 
-import datetime
 import json
+import sys
 import tempfile
 from shutil import rmtree
 from os import path as op
-from pathlib import PurePath
-from io import UnsupportedOperation
 
 import numpy as np
-
-_path_like = (str, PurePath)
+try:
+    from scipy import sparse
+except ImportError:
+    sparse = None
+
+# Adapted from six
+PY3 = sys.version_info[0] == 3
+text_type = str if PY3 else unicode  # noqa
+string_types = str if PY3 else basestring  # noqa
 
 special_chars = {'{FWDSLASH}': '/'}
 tab_str = '----'
 
 
-def _import_sparse():
-    try:
-        from scipy import sparse
-    except ImportError:
-        sparse = None
-    return sparse
-
-
 ##############################################################################
 # WRITING
 
 def _check_h5py():
     """Helper to check if h5py is installed"""
     try:
         import h5py
@@ -60,25 +57,23 @@
     data.to_hdf(fname, rootpath)
     with h5py.File(fname, mode='a') as fid:
         fid[rootpath].attrs['TITLE'] = 'pd_dataframe'
 
 
 def write_hdf5(fname, data, overwrite=False, compression=4,
                title='h5io', slash='error', use_json=False):
-    """Write python object to HDF5 format using h5py.
+    """Write python object to HDF5 format using h5py
 
     Parameters
     ----------
     fname : str
         Filename to use.
     data : object
         Object to write. Can be of any of these types:
-
-            {ndarray, dict, list, tuple, int, float, str, datetime, timezone}
-
+            {ndarray, dict, list, tuple, int, float, str}
         Note that dict objects must only have ``str`` keys. It is recommended
         to use ndarrays where possible, as it is handled most efficiently.
     overwrite : True | False | 'update'
         If True, overwrite file (if it exists). If 'update', appends the title
         to the file (or replace value if title exists).
     compression : int
         Compression level to use (0-9) to compress data using gzip.
@@ -86,85 +81,70 @@
         The top-level directory name to use. Typically it is useful to make
         this your package name, e.g. ``'mnepython'``.
     slash : 'error' | 'replace'
         Whether to replace forward-slashes ('/') in any key found nested within
         keys in data. This does not apply to the top level name (title).
         If 'error', '/' is not allowed in any lower-level keys.
     use_json : bool
-        To accelerate the read and write performance of small dictionaries and
+        To accelerate the read and write perfromance of small dictionaries and
         lists they can be combined to JSON objects and stored as strings.
     """
     h5py = _check_h5py()
-    if isinstance(fname, _path_like):
-        mode = 'w'
-        if op.isfile(fname):
-            if isinstance(overwrite, str):
-                if overwrite != 'update':
-                    raise ValueError('overwrite must be "update" or a bool')
-                mode = 'a'
-            elif not overwrite:
-                raise IOError(
-                    'file "%s" exists, use overwrite=True to overwrite' % fname
-                )
-    elif isinstance(fname, h5py.File):
-        if fname.mode == 'r':
-            raise UnsupportedOperation('not writable')
-    else:
-        raise ValueError(f'fname must be str or h5py.File, got {type(fname)}')
-    if not isinstance(title, str):
+    mode = 'w'
+    if op.isfile(fname):
+        if isinstance(overwrite, string_types):
+            if overwrite != 'update':
+                raise ValueError('overwrite must be "update" or a bool')
+            mode = 'a'
+        elif not overwrite:
+            raise IOError('file "%s" exists, use overwrite=True to overwrite'
+                          % fname)
+    if not isinstance(title, string_types):
         raise ValueError('title must be a string')
     comp_kw = dict()
     if compression > 0:
         comp_kw = dict(compression='gzip', compression_opts=compression)
-
-    def _write(fid, cleanup_data):
+    with h5py.File(fname, mode=mode) as fid:
         if title in fid:
             del fid[title]
+        cleanup_data = []
         _triage_write(title, data, fid, comp_kw, str(type(data)),
-                      cleanup_data, slash=slash, title=title,
+                      cleanup_data=cleanup_data, slash=slash, title=title,
                       use_json=use_json)
-    cleanup_data = []
-    if isinstance(fname, h5py.File):
-        _write(fname, cleanup_data)
-    else:
-        with h5py.File(fname, mode=mode) as fid:
-            _write(fid, cleanup_data)
 
     # Will not be empty if any extra data to be written
     for data in cleanup_data:
         # In case different extra I/O needs different inputs
         title = list(data.keys())[0]
         if title in ['pd_dataframe', 'pd_series']:
             rootname, key, value = data[title]
             _create_pandas_dataset(fname, rootname, key, title, value)
 
 
 def _triage_write(key, value, root, comp_kw, where,
-                  cleanup_data, slash='error', title=None,
-                  use_json=False):
-    sparse = _import_sparse()
+                  cleanup_data=[], slash='error', title=None, use_json=False):
     if key != title and '/' in key:
         if slash == 'error':
             raise ValueError('Found a key with "/", '
                              'this is not allowed if slash == error')
         elif slash == 'replace':
             # Auto-replace keys with proper values
             for key_spec, val_spec in special_chars.items():
                 key = key.replace(val_spec, key_spec)
         else:
             raise ValueError("slash must be one of ['error', 'replace'")
 
     if use_json and isinstance(value, (list, dict)) and \
-            _json_compatible(value, slash=slash):
+            json_compatible(value, slash=slash):
         value = np.frombuffer(json.dumps(value).encode('utf-8'), np.uint8)
         _create_titled_dataset(root, key, 'json', value, comp_kw)
     elif isinstance(value, dict):
         sub_root = _create_titled_group(root, key, 'dict')
         for key, sub_value in value.items():
-            if not isinstance(key, str):
+            if not isinstance(key, string_types):
                 raise TypeError('All dict keys must be strings')
             _triage_write(
                 'key_{0}'.format(key), sub_value, sub_root, comp_kw,
                 where + '["%s"]' % key, cleanup_data=cleanup_data, slash=slash)
     elif isinstance(value, (list, tuple)):
         title = 'list' if isinstance(value, list) else 'tuple'
         sub_root = _create_titled_group(root, key, title)
@@ -176,27 +156,19 @@
         _create_titled_dataset(root, key, 'None', [False])
     elif isinstance(value, (int, float)):
         if isinstance(value, int):
             title = 'int'
         else:  # isinstance(value, float):
             title = 'float'
         _create_titled_dataset(root, key, title, np.atleast_1d(value))
-    elif isinstance(value, datetime.datetime):
-        title = 'datetime'
-        value = np.frombuffer(value.isoformat().encode('utf-8'), np.uint8)
-        _create_titled_dataset(root, key, title, value)
-    elif isinstance(value, datetime.timezone):
-        title = 'timezone'  # the __repr__ is complete
-        value = np.frombuffer(repr(value).encode('utf-8'), np.uint8)
-        _create_titled_dataset(root, key, title, value)
     elif isinstance(value, (np.integer, np.floating, np.bool_)):
         title = 'np_{0}'.format(value.__class__.__name__)
         _create_titled_dataset(root, key, title, np.atleast_1d(value))
-    elif isinstance(value, str):
-        if isinstance(value, str):  # unicode
+    elif isinstance(value, string_types):
+        if isinstance(value, text_type):  # unicode
             value = np.frombuffer(value.encode('utf-8'), np.uint8)
             title = 'unicode'
         else:
             value = np.frombuffer(value.encode('ASCII'), np.uint8)
             title = 'ascii'
         _create_titled_dataset(root, key, title, value, comp_kw)
     elif isinstance(value, np.ndarray):
@@ -272,47 +244,32 @@
 
     Returns
     -------
     data : object
         The loaded data. Can be of any type supported by ``write_hdf5``.
     """
     h5py = _check_h5py()
-    if isinstance(fname, _path_like):
-        if not op.isfile(fname):
-            raise IOError('file "%s" not found' % fname)
-    elif isinstance(fname, h5py.File):
-        if fname.mode == 'w':
-            raise UnsupportedOperation(
-                'file must not be opened be opened with "w"'
-            )
-        print(fname.mode)
-    else:
-        raise ValueError(f'fname must be str or h5py.File, got {type(fname)}')
-    if not isinstance(title, str):
+    if not op.isfile(fname):
+        raise IOError('file "%s" not found' % fname)
+    if not isinstance(title, string_types):
         raise ValueError('title must be a string')
-
-    def _read(fid):
+    with h5py.File(fname, mode='r') as fid:
         if title not in fid:
             raise ValueError('no "%s" data found' % title)
         if isinstance(fid[title], h5py.Group):
             if 'TITLE' not in fid[title].attrs:
                 raise ValueError('no "%s" data found' % title)
-        return _triage_read(fid[title], slash=slash)
-    if isinstance(fname, h5py.File):
-        return _read(fname)
-    else:
-        with h5py.File(fname, mode='r') as fid:
-            return _read(fid)
+        data = _triage_read(fid[title], slash=slash)
+    return data
 
 
 def _triage_read(node, slash='ignore'):
     if slash not in ['ignore', 'replace']:
         raise ValueError("slash must be one of 'replace', 'ignore'")
     h5py = _check_h5py()
-    sparse = _import_sparse()
     type_str = node.attrs['TITLE']
     if isinstance(type_str, bytes):
         type_str = type_str.decode()
     if isinstance(node, h5py.Group):
         if type_str == 'dict':
             data = dict()
             for key, subnode in node.items():
@@ -363,29 +320,24 @@
             raise NotImplementedError('Unknown group type: {0}'
                                       ''.format(type_str))
     elif type_str == 'ndarray':
         data = np.array(node)
     elif type_str in ('int', 'float'):
         cast = int if type_str == 'int' else float
         data = cast(np.array(node)[0])
-    elif type_str == 'datetime':
-        data = str(np.array(node).tobytes().decode('utf-8'))
-        data = datetime.datetime.fromisoformat(data)
-    elif type_str == 'timezone':
-        data = eval(str(np.array(node).tobytes().decode('utf-8')),
-                    {'datetime': datetime})
     elif type_str.startswith('np_'):
         np_type = type_str.split('_')[1]
-        cast = getattr(np, np_type) if np_type != 'bool' else bool
-        data = np.array(node)[0].astype(cast)
+        cast = getattr(np, np_type)
+        data = cast(np.array(node)[0])
     elif type_str in ('unicode', 'ascii', 'str'):  # 'str' for backward compat
         decoder = 'utf-8' if type_str == 'unicode' else 'ASCII'
-        data = str(np.array(node).tobytes().decode(decoder))
+        cast = text_type if type_str == 'unicode' else str
+        data = cast(np.array(node).tostring().decode(decoder))
     elif type_str == 'json':
-        node_unicode = str(np.array(node).tobytes().decode('utf-8'))
+        node_unicode = str(np.array(node).tostring().decode('utf-8'))
         data = json.loads(node_unicode)
     elif type_str == 'None':
         data = None
     else:
         raise TypeError('Unknown node type: {0}'.format(type_str))
     return data
 
@@ -415,15 +367,15 @@
         String to prepend to each line.
 
     Returns
     -------
     diffs : str
         A string representation of the differences.
     """
-    sparse = _import_sparse()
+
     try:
         from pandas import DataFrame, Series
     except ImportError:
         DataFrame = Series = type(None)
 
     out = ''
     if type(a) != type(b):
@@ -441,15 +393,15 @@
                 out += object_diff(a[key], b[key], pre + 'd1[%s]' % repr(key))
     elif isinstance(a, (list, tuple)):
         if len(a) != len(b):
             out += pre + ' length mismatch (%s, %s)\n' % (len(a), len(b))
         else:
             for xx1, xx2 in zip(a, b):
                 out += object_diff(xx1, xx2, pre='')
-    elif isinstance(a, (str, int, float, bytes)):
+    elif isinstance(a, (string_types, int, float, bytes)):
         if a != b:
             out += pre + ' value mismatch (%s, %s)\n' % (a, b)
     elif a is None:
         pass  # b must be None due to our type checking
     elif isinstance(a, np.ndarray):
         if not np.array_equal(a, b):
             out += pre + ' array mismatch\n'
@@ -521,15 +473,16 @@
             desc_val = data.shape
         elif type_str in ['pd_dataframe', 'pd_series']:
             desc = 'Shape: %s'
             desc_val = data['values'].shape
         elif type_str in ('unicode', 'ascii', 'str'):
             desc = 'Text: %s'
             decoder = 'utf-8' if type_str == 'unicode' else 'ASCII'
-            data = str(np.array(data).tobytes().decode(decoder))
+            cast = text_type if type_str == 'unicode' else str
+            data = cast(np.array(data).tostring().decode(decoder))
             desc_val = data[:10] + '...' if len(data) > 10 else data
         else:
             desc = 'Items: %s'
             desc_val = len(data)
         this_str = ('%%s Key: %s | Type: %s | ' + desc) % (
             str_format, str_format, str_format)
         this_str = this_str % (tab_str, key, type_str, desc_val)
@@ -555,43 +508,40 @@
             _list_file_contents(f)
     else:
         if not isinstance(h5file, h5py.File):
             raise TypeError(err.format(type(h5file)))
         _list_file_contents(h5file)
 
 
-def _json_compatible(obj, slash='error'):
-    if isinstance(obj, (str, int, float, bool, type(None))):
+def json_compatible(obj, slash='error'):
+    if isinstance(obj, (string_types, int, float, bool, type(None))):
         return True
     elif isinstance(obj, list):
-        return all([_json_compatible(item) for item in obj])
+        return all([json_compatible(item) for item in obj])
     elif isinstance(obj, dict):
         _check_keys_in_dict(obj, slash=slash)
-        return all([_json_compatible(item) for item in obj.values()])
+        return all([json_compatible(item) for item in obj.values()])
     else:
         return False
 
 
 def _check_keys_in_dict(obj, slash='error'):
-    repl = list()
     for key in obj.keys():
         if '/' in key:
             key_prev = key
             if slash == 'error':
                 raise ValueError('Found a key with "/", '
                                  'this is not allowed if slash == error')
             elif slash == 'replace':
                 # Auto-replace keys with proper values
                 for key_spec, val_spec in special_chars.items():
                     key = key.replace(val_spec, key_spec)
-                repl.append((key, key_prev))
+                obj[key] = obj.pop(key_prev)
             else:
                 raise ValueError("slash must be one of ['error', 'replace'")
-    for key, key_prev in repl:
-        obj[key] = obj.pop(key_prev)
 
 
 ##############################################################################
 # Arrays with mixed dimensions
 def _validate_object_array(array):
     if not (array.dtype == np.dtype('object') and
             len(set([sub.dtype for sub in array])) == 1):
@@ -639,8 +589,8 @@
 def multiarray_load(index, array_merged):
     array_restore = []
     i_prev = 0
     for i in index[:-1]:
         array_restore.append(array_merged[i_prev:i])
         i_prev = i
     array_restore.append(array_merged[i_prev:])
-    return np.array(array_restore, dtype=object)
+    return np.array(array_restore)
```

### Comparing `h5io-0.1.8/h5io/tests/test_io.py` & `h5io-0.post0.dev110/h5io/tests/test_io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,174 @@
 # -*- coding: utf-8 -*-
-import datetime
-from pathlib import Path
 from os import path as op
-from io import UnsupportedOperation
-import pytest
+from nose.tools import assert_raises, assert_true, assert_equal
 
 import numpy as np
-from numpy.testing import assert_equal
 try:
     from scipy import sparse
 except ImportError:
     sparse = None
 
 try:
     from pandas import DataFrame, Series
 except ImportError:
     DataFrame = Series = None
 
-import h5py
 from h5io import (write_hdf5, read_hdf5,
-                  object_diff, list_file_contents)
+                  _TempDir, object_diff, list_file_contents)
 
 
-def test_hdf5(tmpdir):
-    """Test HDF5 IO."""
-    tempdir = str(tmpdir)
+def test_hdf5():
+    """Test HDF5 IO
+    """
+    tempdir = _TempDir()
     test_file = op.join(tempdir, 'test.hdf5')
     sp = np.eye(3) if sparse is None else sparse.eye(3, 3, format='csc')
     sp_csr = np.eye(3) if sparse is None else sparse.eye(3, 3, format='csr')
     df = np.eye(3) if isinstance(DataFrame, type(None)) else DataFrame(
         np.eye(3))
     sr = np.eye(3) if isinstance(Series, type(None)) else Series(
         np.random.randn(3))
     sp[2, 2] = 2
     sp_csr[2, 2] = 2
     x = dict(a=dict(b=np.zeros(3)), c=np.zeros(2, np.complex128),
              d=[dict(e=(1, -2., 'hello', u'goodbyeu\u2764')), None], f=sp,
              g=dict(dfa=df, srb=sr), h=sp_csr, i=sr, j='hi')
     write_hdf5(test_file, 1)
     assert_equal(read_hdf5(test_file), 1)
-    pytest.raises(IOError, write_hdf5, test_file, x)  # file exists
-    write_hdf5(Path(test_file), x, overwrite=True)
-    pytest.raises(IOError, read_hdf5, test_file + 'FOO')  # not found
-    xx = read_hdf5(Path(test_file))
-    assert (object_diff(x, xx) == '')  # no assert_equal, ugly output
+    assert_raises(IOError, write_hdf5, test_file, x)  # file exists
+    write_hdf5(test_file, x, overwrite=True)
+    assert_raises(IOError, read_hdf5, test_file + 'FOO')  # not found
+    xx = read_hdf5(test_file)
+    assert_true(object_diff(x, xx) == '')  # no assert_equal, ugly output
     list_file_contents(test_file)  # Testing the h5 listing
-    pytest.raises(TypeError, list_file_contents, sp)  # Only string works
+    assert_raises(TypeError, list_file_contents, sp)  # Only string works
     write_hdf5(test_file, np.bool_(True), overwrite=True)
     assert_equal(read_hdf5(test_file), np.bool_(True))
 
     # bad title
-    pytest.raises(ValueError, read_hdf5, test_file, title='nonexist')
-    pytest.raises(ValueError, write_hdf5, test_file, x, overwrite=True,
+    assert_raises(ValueError, read_hdf5, test_file, title='nonexist')
+    assert_raises(ValueError, write_hdf5, test_file, x, overwrite=True,
                   title=1)
-    pytest.raises(ValueError, read_hdf5, test_file, title=1)
+    assert_raises(ValueError, read_hdf5, test_file, title=1)
     # unsupported objects
-    pytest.raises(TypeError, write_hdf5, test_file, {1: 'foo'},
+    assert_raises(TypeError, write_hdf5, test_file, {1: 'foo'},
                   overwrite=True)
-    pytest.raises(TypeError, write_hdf5, test_file, object, overwrite=True)
+    assert_raises(TypeError, write_hdf5, test_file, object, overwrite=True)
     # special_chars
     spec_dict = {'first/second': 'third'}
-    pytest.raises(ValueError, write_hdf5, test_file, spec_dict, overwrite=True)
-    pytest.raises(ValueError, write_hdf5, test_file, spec_dict, overwrite=True,
+    assert_raises(ValueError, write_hdf5, test_file, spec_dict, overwrite=True)
+    assert_raises(ValueError, write_hdf5, test_file, spec_dict, overwrite=True,
                   slash='brains')
     write_hdf5(test_file, spec_dict, overwrite=True, slash='replace')
     assert_equal(
         read_hdf5(test_file, slash='replace').keys(), spec_dict.keys())
     in_keys = list(read_hdf5(test_file, slash='ignore').keys())
-    assert ('{FWDSLASH}' in in_keys[0])
-    pytest.raises(ValueError, read_hdf5, test_file, slash='brains')
+    assert_true('{FWDSLASH}' in in_keys[0])
+    assert_raises(ValueError, read_hdf5, test_file, slash='brains')
     # Testing that title slashes aren't replaced
     write_hdf5(
         test_file, spec_dict, title='one/two', overwrite=True, slash='replace')
     assert_equal(read_hdf5(test_file, title='one/two', slash='replace').keys(),
                  spec_dict.keys())
 
     write_hdf5(test_file, 1, title='first', overwrite=True)
     write_hdf5(test_file, 2, title='second', overwrite='update')
     assert_equal(read_hdf5(test_file, title='first'), 1)
     assert_equal(read_hdf5(test_file, title='second'), 2)
-    pytest.raises(IOError, write_hdf5, test_file, 3, title='second')
+    assert_raises(IOError, write_hdf5, test_file, 3, title='second')
     write_hdf5(test_file, 3, title='second', overwrite='update')
     assert_equal(read_hdf5(test_file, title='second'), 3)
 
     write_hdf5(test_file, 5, title='second', overwrite='update', compression=5)
     assert_equal(read_hdf5(test_file, title='second'), 5)
 
 
-def test_h5_file_object(tmpdir):
-    tempdir = str(tmpdir)
-    test_file_path = op.join(tempdir, 'test1.hdf5')
-    # test that wrong object type raises error
-    pytest.raises(ValueError, write_hdf5, fname=33, data=1)
-    # test that reading/writing are unaffected
-    with h5py.File(test_file_path, 'a') as test_file_obj:
-        data = {'a': 42}
-        write_hdf5(test_file_obj, data)
-        assert_equal(read_hdf5(test_file_obj), data)
-    # test that wrong mode raises error
-    with h5py.File(test_file_path, 'r') as test_file_obj:
-        assert test_file_obj.mode == 'r'
-        with pytest.raises(UnsupportedOperation):
-            write_hdf5(test_file_obj, data=1)
-    # at least on some OSes (e.g., macOS) opening with mode='w' leads to
-    # test_file_obj.mode == 'r+', so let's skip this for now
-    # with h5py.File(test_file_path, 'w') as test_file_obj:
-    #     print(test_file_obj.mode)
-    #     with pytest.raises(UnsupportedOperation):
-    #         read_hdf5(test_file_obj)
-
-
-def test_hdf5_use_json(tmpdir):
-    """Test HDF5 IO."""
-    tempdir = str(tmpdir)
+def test_hdf5_use_json():
+    """Test HDF5 IO
+    """
+    tempdir = _TempDir()
     test_file = op.join(tempdir, 'test.hdf5')
     splash_dict = {'first/second': {'one/more': 'value'}}
-    pytest.raises(ValueError, write_hdf5, test_file, splash_dict,
+    assert_raises(ValueError, write_hdf5, test_file, splash_dict,
                   overwrite=True, slash='error', use_json=True)
     spec_dict = {'first/second': 'third'}
     write_hdf5(test_file, spec_dict, overwrite=True, slash='replace',
                use_json=True)
     assert_equal(
         read_hdf5(test_file, slash='replace').keys(), spec_dict.keys())
     in_keys = list(read_hdf5(test_file, slash='ignore').keys())
-    assert ('{FWDSLASH}' in in_keys[0])
+    assert_true('{FWDSLASH}' in in_keys[0])
     comp_dict = {'first': [1, 2], 'second': 'str', 'third': {'a': 1}}
     write_hdf5(test_file, comp_dict, overwrite=True, use_json=True)
     assert_equal(
         sorted(read_hdf5(test_file, slash='replace').keys()),
         sorted(comp_dict.keys()))
     numpy_dict = {'first': np.array([1])}
     write_hdf5(test_file, numpy_dict, overwrite=True, use_json=True)
     assert_equal(list(read_hdf5(test_file, slash='replace').values())[0],
                  list(numpy_dict.values())[0])
-    pytest.raises(ValueError, read_hdf5, test_file, slash='brains')
+    assert_raises(ValueError, read_hdf5, test_file, slash='brains')
     # Testing that title slashes aren't replaced
     write_hdf5(test_file, spec_dict, title='one/two', overwrite=True,
                slash='replace', use_json=True)
     assert_equal(read_hdf5(test_file, title='one/two', slash='replace').keys(),
                  spec_dict.keys())
 
 
-def test_path_support(tmpdir):
-    tempdir = str(tmpdir)
+def test_path_support():
+    tempdir = _TempDir()
     test_file = op.join(tempdir, 'test.hdf5')
     write_hdf5(test_file, 1, title='first')
     write_hdf5(test_file, 2, title='second/third', overwrite='update')
-    pytest.raises(ValueError, read_hdf5, test_file, title='second')
+    assert_raises(ValueError, read_hdf5, test_file, title='second')
     assert_equal(read_hdf5(test_file, 'first'), 1)
     assert_equal(read_hdf5(test_file, 'second/third'), 2)
 
 
 def test_object_diff():
-    """Test object diff calculation."""
-    assert ('type' in object_diff(1, 1.))
-    assert ('missing' in object_diff({1: 1}, {}))
-    assert ('missing' in object_diff({}, {1: 1}))
-    assert ('length' in object_diff([], [1]))
-    assert ('value' in object_diff('a', 'b'))
-    assert ('None' in object_diff(None, 'b'))
-    assert ('array mismatch' in object_diff(np.array([1]), np.array([2])))
+    """Test object diff calculation
+    """
+    assert_true('type' in object_diff(1, 1.))
+    assert_true('missing' in object_diff({1: 1}, {}))
+    assert_true('missing' in object_diff({}, {1: 1}))
+    assert_true('length' in object_diff([], [1]))
+    assert_true('value' in object_diff('a', 'b'))
+    assert_true('None' in object_diff(None, 'b'))
+    assert_true('array mismatch' in object_diff(np.array([1]), np.array([2])))
     if sparse is not None:
         a = sparse.coo_matrix([[1]])
         b = sparse.coo_matrix([[1, 2]])
-        assert ('shape mismatch' in object_diff(a, b))
+        assert_true('shape mismatch' in object_diff(a, b))
         c = sparse.coo_matrix([[1, 1]])
-        assert ('1 element' in object_diff(b, c))
+        assert_true('1 element' in object_diff(b, c))
     if not isinstance(DataFrame, type(None)):
         for ob_type in (DataFrame, Series):
             a = ob_type([1])
             b = ob_type([1, 2])
-            assert ('shape mismatch' in object_diff(a, b))
+            assert_true('shape mismatch' in object_diff(a, b))
             c = ob_type([1, 3])
-            assert ('1 element' in object_diff(b, c))
-    pytest.raises(RuntimeError, object_diff, object, object)
+            assert_true('1 element' in object_diff(b, c))
+    assert_raises(RuntimeError, object_diff, object, object)
 
 
-def test_numpy_values(tmpdir):
-    """Test NumPy values."""
-    test_file = op.join(str(tmpdir), 'test.hdf5')
+def test_numpy_values():
+    tempdir = _TempDir()
+    test_file = op.join(tempdir, 'test.hdf5')
     for cast in [np.int8, np.int16, np.int32, np.int64, np.bool_,
                  np.float16, np.float32, np.float64]:
         value = cast(1)
         write_hdf5(test_file, value, title='first', overwrite='update')
         assert_equal(read_hdf5(test_file, 'first'), value)
 
 
-def test_multi_dim_array(tmpdir):
-    """Test multidimensional arrays."""
+def test_multi_dim_array():
     rng = np.random.RandomState(0)
-    traj = np.array([rng.randn(2, 1), rng.randn(3, 1)], dtype=object)
-    test_file = op.join(str(tmpdir), 'test.hdf5')
+    traj = np.array([rng.randn(2, 1), rng.randn(3, 1)])
+    tempdir = _TempDir()
+    test_file = op.join(tempdir, 'test.hdf5')
     write_hdf5(test_file, traj, title='first', overwrite='update')
     for traj_read, traj_sub in zip(read_hdf5(test_file, 'first'), traj):
-        assert (np.equal(traj_read, traj_sub).all())
-    traj_no_structure = np.array(
-        [rng.randn(2, 1, 1), rng.randn(3, 1, 2)], dtype=object)
-    pytest.raises(ValueError, write_hdf5, test_file, traj_no_structure,
+        assert_true(np.equal(traj_read, traj_sub).all())
+    traj_no_structure = np.array([rng.randn(2, 1, 1), rng.randn(3, 1, 2)])
+    assert_raises(ValueError, write_hdf5, test_file, traj_no_structure,
                   title='second', overwrite='update')
-
-
-class XT(datetime.tzinfo):
-
-    def utcoffset(self, dt):
-        return datetime.timedelta(hours=-5)  # Eastern on standard time
-
-    def tzname(self, dt):
-        return "UTC-05:00"
-
-    def dst(self, dt):
-        return None
-
-
-def test_datetime(tmpdir):
-    """Test datetime.datetime support."""
-    fname = op.join(str(tmpdir), 'test.hdf5')
-    # Naive
-    y, m, d, h, m, s, mu = range(1, 8)
-    dt = datetime.datetime(y, m, d, h, m, s, mu)
-    for key in ('year', 'month', 'day', 'hour', 'minute', 'second',
-                'microsecond'):
-        val = locals()[key[:1] if key != 'microsecond' else 'mu']
-        assert val == getattr(dt, key)
-    assert dt.year == y
-    assert dt.month == m
-    write_hdf5(fname, dt)
-    dt2 = read_hdf5(fname)
-    assert isinstance(dt2, datetime.datetime)
-    assert dt == dt2
-    assert dt2.tzinfo is None
-    # Aware
-    dt = dt.replace(tzinfo=datetime.timezone.utc)
-    write_hdf5(fname, dt, overwrite=True)
-    dt2 = read_hdf5(fname)
-    assert isinstance(dt2, datetime.datetime)
-    assert dt == dt2
-    assert dt2.tzinfo is datetime.timezone.utc
-    # Custom
-    dt = dt.replace(tzinfo=XT())
-    write_hdf5(fname, dt, overwrite=True)
-    dt2 = read_hdf5(fname)
-    assert isinstance(dt2, datetime.datetime)
-    assert dt == dt2
-    assert dt2.tzinfo is not None
-    assert dt2.tzinfo is not datetime.timezone.utc
-    for key in ('utcoffset', 'tzname', 'dst'):
-        v1 = getattr(dt2.tzinfo, key)(None)
-        v2 = getattr(dt.tzinfo, key)(None)
-        assert v1 == v2
-
-
-@pytest.mark.parametrize('name', (None, 'foo'))
-def test_timezone(name, tmpdir):
-    """Test datetime.timezone support."""
-    fname = op.join(str(tmpdir), 'test.hdf5')
-    kwargs = dict()
-    if name is not None:
-        kwargs['name'] = name
-    x = datetime.timezone(datetime.timedelta(hours=-7), **kwargs)
-    write_hdf5(fname, x)
-    y = read_hdf5(fname)
-    assert isinstance(y, datetime.timezone)
-    assert y == x
-    if name is not None:
-        assert y.tzname(None) == name
```

### Comparing `h5io-0.1.8/h5io.egg-info/PKG-INFO` & `h5io-0.post0.dev110/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,115 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: h5io
-Version: 0.1.8
+Version: 0.post0.dev110
 Summary: Python Objects Onto HDF5
 Home-page: http://h5io.github.io
-Download-URL: http://github.com/h5io/h5io
 Maintainer: Eric Larson
 Maintainer-email: larson.eric.d@gmail.com
 License: BSD (3-clause)
+Download-URL: http://github.com/h5io/h5io
+Description: .. -*- mode: rst -*-
+        
+        |Travis|_ |Appveyor|_ |Codecov|_
+        
+        .. |Travis| image:: https://api.travis-ci.org/h5io/h5io.png?branch=master
+        .. _Travis: https://travis-ci.org/h5io/h5io
+        
+        .. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/puwaarmllxq5wfvm?svg=true
+        .. _Appveyor: https://ci.appveyor.com/project/larsoner/h5io/branch/master
+        
+        .. |Codecov| image:: https://codecov.io/gh/h5io/h5io/branch/master/graph/badge.svg
+        .. _Codecov: https://codecov.io/gh/h5io/h5io
+        
+        `h5io <http://h5io.github.io>`_
+        =======================================================
+        
+        h5io is a package designed to facilitate saving some standard Python
+        objects into the forward-compatible HDF5 format. It is a higher-level
+        package than ``h5py``.
+        
+        Get the latest code
+        ^^^^^^^^^^^^^^^^^^^
+        
+        To get the latest code using git, simply type::
+        
+            git clone git://github.com/h5io/h5io.git
+        
+        If you don't have git installed, you can download a zip or tarball
+        of the latest code: https://github.com/h5io/h5io/archives/master
+        
+        Install h5io
+        ^^^^^^^^^^^^
+        
+        As any Python packages, to install h5io, go in the source code directory
+        and do::
+        
+            python setup.py install
+        
+        or if you don't have admin access to your python setup (permission denied
+        when install) use::
+        
+            python setup.py install --user
+        
+        You can also install the latest release version with pip::
+        
+            pip install h5io --upgrade
+        
+        or for the latest development version (the most up to date)::
+        
+            pip install -e git+https://github.com/h5io/h5io#egg=h5io-dev --user
+        
+        Dependencies
+        ^^^^^^^^^^^^
+        
+        The required dependencies to build the software are ``h5py`` and ``numpy``.
+        ``scipy`` is required for sparse matrix IO support.
+        
+        Licensing
+        ^^^^^^^^^
+        
+        h5io is **BSD-licenced** (3 clause):
+        
+            This software is OSI Certified Open Source Software.
+            OSI Certified is a certification mark of the Open Source Initiative.
+        
+            Copyright (c) 2011, authors of h5io
+            All rights reserved.
+        
+            Redistribution and use in source and binary forms, with or without
+            modification, are permitted provided that the following conditions are met:
+        
+            * Redistributions of source code must retain the above copyright notice,
+              this list of conditions and the following disclaimer.
+        
+            * Redistributions in binary form must reproduce the above copyright notice,
+              this list of conditions and the following disclaimer in the documentation
+              and/or other materials provided with the distribution.
+        
+            * Neither the names of h5io authors nor the names of any
+              contributors may be used to endorse or promote products derived from
+              this software without specific prior written permission.
+        
+            **This software is provided by the copyright holders and contributors
+            "as is" and any express or implied warranties, including, but not
+            limited to, the implied warranties of merchantability and fitness for
+            a particular purpose are disclaimed. In no event shall the copyright
+            owner or contributors be liable for any direct, indirect, incidental,
+            special, exemplary, or consequential damages (including, but not
+            limited to, procurement of substitute goods or services; loss of use,
+            data, or profits; or business interruption) however caused and on any
+            theory of liability, whether in contract, strict liability, or tort
+            (including negligence or otherwise) arising in any way out of the use
+            of this software, even if advised of the possibility of such
+            damage.**
+        
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-License-File: LICENSE.txt
-
-.. -*- mode: rst -*-
-
-|Travis|_ |Appveyor|_ |Codecov|_
-
-.. |Travis| image:: https://api.travis-ci.org/h5io/h5io.png?branch=master
-.. _Travis: https://travis-ci.org/h5io/h5io
-
-.. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/puwaarmllxq5wfvm?svg=true
-.. _Appveyor: https://ci.appveyor.com/project/larsoner/h5io/branch/master
-
-.. |Codecov| image:: https://codecov.io/gh/h5io/h5io/branch/master/graph/badge.svg
-.. _Codecov: https://codecov.io/gh/h5io/h5io
-
-`h5io <http://h5io.github.io>`_
-=======================================================
-
-h5io is a package designed to facilitate saving some standard Python
-objects into the forward-compatible HDF5 format. It is a higher-level
-package than ``h5py``.
-
-Get the latest code
-^^^^^^^^^^^^^^^^^^^
-
-To get the latest code using git, simply type::
-
-    git clone git://github.com/h5io/h5io.git
-
-If you don't have git installed, you can download a zip or tarball
-of the latest code: https://github.com/h5io/h5io/archives/master
-
-Install h5io
-^^^^^^^^^^^^
-
-As any Python packages, to install h5io, go in the source code directory
-and do::
-
-    python setup.py install
-
-or if you don't have admin access to your python setup (permission denied
-when install) use::
-
-    python setup.py install --user
-
-You can also install the latest release version with pip::
-
-    pip install h5io --upgrade
-
-or for the latest development version (the most up to date)::
-
-    pip install -e git+https://github.com/h5io/h5io#egg=h5io-dev --user
-
-Dependencies
-^^^^^^^^^^^^
-
-The required dependencies to build the software are ``h5py`` and ``numpy``.
-``scipy`` is required for sparse matrix IO support.
-
-Licensing
-^^^^^^^^^
-
-h5io is **BSD-licenced** (3 clause):
-
-    This software is OSI Certified Open Source Software.
-    OSI Certified is a certification mark of the Open Source Initiative.
-
-    Copyright (c) 2011, authors of h5io
-    All rights reserved.
-
-    Redistribution and use in source and binary forms, with or without
-    modification, are permitted provided that the following conditions are met:
-
-    * Redistributions of source code must retain the above copyright notice,
-      this list of conditions and the following disclaimer.
-
-    * Redistributions in binary form must reproduce the above copyright notice,
-      this list of conditions and the following disclaimer in the documentation
-      and/or other materials provided with the distribution.
-
-    * Neither the names of h5io authors nor the names of any
-      contributors may be used to endorse or promote products derived from
-      this software without specific prior written permission.
-
-    **This software is provided by the copyright holders and contributors
-    "as is" and any express or implied warranties, including, but not
-    limited to, the implied warranties of merchantability and fitness for
-    a particular purpose are disclaimed. In no event shall the copyright
-    owner or contributors be liable for any direct, indirect, incidental,
-    special, exemplary, or consequential damages (including, but not
-    limited to, procurement of substitute goods or services; loss of use,
-    data, or profits; or business interruption) however caused and on any
-    theory of liability, whether in contract, strict liability, or tort
-    (including negligence or otherwise) arising in any way out of the use
-    of this software, even if advised of the possibility of such
-    damage.**
```

### Comparing `h5io-0.1.8/setup.py` & `h5io-0.post0.dev110/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 #! /usr/bin/env python
 #
 
 # Copyright (C) 2011-2014 Alexandre Gramfort
 # <alexandre.gramfort@telecom-paristech.fr>
 
 import os
-import pathlib
 
-from setuptools import setup
+import setuptools  # noqa; we are using a setuptools namespace
+from numpy.distutils.core import setup
+import versioneer
 
 
 descr = """Python Objects Onto HDF5"""
 
 DISTNAME = 'h5io'
 DESCRIPTION = descr
 MAINTAINER = 'Eric Larson'
 MAINTAINER_EMAIL = 'larson.eric.d@gmail.com'
 URL = 'http://h5io.github.io'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'http://github.com/h5io/h5io'
 
-version = None
-with open(pathlib.Path('h5io') / '_version.py', 'r') as fid:
-    for line in (line.strip() for line in fid):
-        if line.startswith('__version__'):
-            version = line.split('=')[1].strip().strip('\'')
-            break
-    else:
-        raise RuntimeError('Could not determine version')
-
 
 if __name__ == "__main__":
     if os.path.exists('MANIFEST'):
         os.remove('MANIFEST')
 
     setup(name=DISTNAME,
           maintainer=MAINTAINER,
           include_package_data=True,
           maintainer_email=MAINTAINER_EMAIL,
           description=DESCRIPTION,
           license=LICENSE,
           url=URL,
-          version=version,
+          version=versioneer.get_version(),
           download_url=DOWNLOAD_URL,
-          python_requires='>=3.7',
-          install_requires=['numpy', 'h5py'],
           long_description=open('README.rst').read(),
           zip_safe=False,  # the package can run out of an .egg file
           classifiers=['Intended Audience :: Science/Research',
                        'Intended Audience :: Developers',
                        'License :: OSI Approved',
                        'Programming Language :: Python',
                        'Topic :: Software Development',
@@ -56,8 +46,9 @@
                        'Operating System :: Microsoft :: Windows',
                        'Operating System :: POSIX',
                        'Operating System :: Unix',
                        'Operating System :: MacOS'],
           platforms='any',
           packages=['h5io', 'h5io.tests'],
           package_data={},
-          scripts=[])
+          scripts=[],
+          cmdclass=versioneer.get_cmdclass())
```

