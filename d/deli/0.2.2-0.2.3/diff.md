# Comparing `tmp/deli-0.2.2.tar.gz` & `tmp/deli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deli-0.2.2.tar", last modified: Wed Jul  5 16:43:01 2023, max compression
+gzip compressed data, was "deli-0.2.3.tar", last modified: Fri Jul  7 10:14:37 2023, max compression
```

## Comparing `deli-0.2.2.tar` & `deli-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.870432 deli-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 16:42:49.000000 deli-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 16:42:49.000000 deli-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-05 16:43:01.870432 deli-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-05 16:42:49.000000 deli-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-05 16:42:49.000000 deli-0.2.2/deli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 16:42:49.000000 deli-0.2.2/deli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-05 16:42:49.000000 deli-0.2.2/deli/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/nifty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/numpy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-05 16:42:49.000000 deli-0.2.2/deli/serializers/packaged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/deli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 16:43:01.000000 deli-0.2.2/deli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-05 16:42:49.000000 deli-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:42:49.000000 deli-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:43:01.870432 deli-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-05 16:42:49.000000 deli-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:43:01.866432 deli-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-05 16:42:49.000000 deli-0.2.2/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:37.219762 deli-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 10:14:22.000000 deli-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 10:14:22.000000 deli-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-07 10:14:37.219762 deli-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 10:14:22.000000 deli-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:37.215762 deli-0.2.3/deli/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 10:14:22.000000 deli-0.2.3/deli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 10:14:22.000000 deli-0.2.3/deli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-07 10:14:22.000000 deli-0.2.3/deli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:37.219762 deli-0.2.3/deli/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/nifty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/numpy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-07 10:14:22.000000 deli-0.2.3/deli/serializers/packaged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:37.215762 deli-0.2.3/deli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-07 10:14:37.000000 deli-0.2.3/deli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 10:14:37.000000 deli-0.2.3/deli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:14:37.000000 deli-0.2.3/deli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 10:14:37.000000 deli-0.2.3/deli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 10:14:37.000000 deli-0.2.3/deli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 10:14:22.000000 deli-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:22.000000 deli-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:14:37.219762 deli-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-07 10:14:22.000000 deli-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:14:37.219762 deli-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:14:22.000000 deli-0.2.3/tests/test_serializers.py
```

### Comparing `deli-0.2.2/LICENSE` & `deli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/PKG-INFO` & `deli-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
-Download-URL: https://github.com/maxme1/deli/archive/v0.2.2.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.3.tar.gz
 Author-email: Max <maxs987@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 maxme1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `deli-0.2.2/deli/interface.py` & `deli-0.2.3/deli/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import json
+from io import RawIOBase, BufferedIOBase
 import os
-import pickle
 from gzip import GzipFile
 from os import PathLike
-from typing import Any, Union, BinaryIO
+from typing import Any, Optional, Union, BinaryIO
 
 from .serializer import MaybeHint, WrongSerializer, REGISTRY, Hint
 from .serializers.choice import Choice
 
 __all__ = [
     'load', 'save',
     'load_json', 'save_json',
@@ -34,15 +33,15 @@
         if strict:
             loader = choice.match_load_path(source, hint, kwargs)
             if loader is None:
                 raise WrongSerializer(f"Couldn't load from value using {hint!r} as hint")
 
         return loader.load_path(source, hint, kwargs)
 
-    if not isinstance(source, BinaryIO):
+    if not is_binary_io(source):
         raise TypeError(f'Need a binary buffer, not {type(source).__name__}')
 
     # TODO: reuse
     loader = choice
     if strict:
         loader = choice.match_load_buffer(hint, True, kwargs)
         if loader is None:
@@ -57,25 +56,25 @@
     `hint` is used to override the format detection.
     `kwargs` are format-specific keyword arguments.
     """
     choice = Choice(*REGISTRY)
 
     hint = _resolve_hint(hint, destination)
     strict = hint is not None
-    # TODO: what is it's both BinaryIO and PathLike?
+    # TODO: what if it's both BinaryIO and PathLike?
     if isinstance(destination, (str, PathLike)):
         loader = choice
         if strict:
             loader = choice.match_save_path(value, destination, hint, kwargs)
             if loader is None:
                 raise WrongSerializer(f"Couldn't save value using {hint!r} as hint")
 
         return loader.save_path(value, destination, hint, kwargs)
 
-    if not isinstance(destination, BinaryIO):
+    if not is_binary_io(destination):
         raise TypeError(f'Need a binary buffer, not {type(destination).__name__}')
 
     # TODO: reuse
     loader = choice
     if strict:
         loader = choice.match_save_buffer(value, hint, kwargs)
         if loader is None:
@@ -93,24 +92,22 @@
     if not hint:
         return None
     if isinstance(path, (str, PathLike)):
         return os.path.basename(os.fspath(path))
     return None
 
 
-# TODO: rewrite as generic calls with hints
 def load_json(path: PathLike):
     """Load the contents of a json file."""
     return load(path, hint='.json')
 
 
-def save_json(value, path: PathLike, *, indent: int = None):
+def save_json(value, path: PathLike, *, indent: Optional[int] = None):
     """Dump a json-serializable object to a json file."""
-    with open(path, 'w') as f:
-        json.dump(value, f, indent=indent)
+    save(value, path, hint='.json', indent=indent)
 
 
 def save_numpy(value, path: PathLike, *, allow_pickle: bool = True, fix_imports: bool = True, compression: int = None,
                timestamp: int = None):
     """A wrapper around ``np.save`` that matches the interface ``save(what, where)``."""
     import numpy as np
 
@@ -130,40 +127,39 @@
             return load_numpy(file, allow_pickle=allow_pickle, fix_imports=fix_imports)
 
     return np.load(path, allow_pickle=allow_pickle, fix_imports=fix_imports)
 
 
 def save_pickle(value, path: PathLike):
     """Pickle a ``value`` to ``path``."""
-    with open(path, 'wb') as file:
-        pickle.dump(value, file)
+    save(value, path, hint='.pkl')
 
 
 def load_pickle(path: PathLike):
     """Load a pickled value from ``path``."""
-    with open(path, 'rb') as file:
-        return pickle.load(file)
+    return load(path, hint='.pkl')
 
 
 def save_text(value: str, path: PathLike):
-    with open(path, mode='w') as file:
-        file.write(value)
-
+    save(value, path, hint='.txt')
+    
 
 def load_text(path: PathLike):
-    with open(path, mode='r') as file:
-        return file.read()
+    return load(path, hint='.txt')
 
 
-def save_csv(value, path: PathLike, *, compression: int = None, **kwargs):
+def save_csv(value, path: PathLike, *, compression: Optional[int] = None, **kwargs):
     if compression is not None:
         kwargs['compression'] = {
             'method': 'gzip',
             'compresslevel': compression,
         }
 
     value.to_csv(path, **kwargs)
 
 
 def load_csv(path: PathLike, **kwargs):
-    import pandas as pd
-    return pd.read_csv(path, **kwargs)
+    return load(path, hint='.csv', **kwargs)
+
+
+def is_binary_io(x):
+    return isinstance(x, (BinaryIO, RawIOBase, BufferedIOBase))
```

### Comparing `deli-0.2.2/deli/serializer.py` & `deli-0.2.3/deli/serializer.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/choice.py` & `deli-0.2.3/deli/serializers/choice.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/csv.py` & `deli-0.2.3/deli/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/dicom.py` & `deli-0.2.3/deli/serializers/dicom.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/helpers.py` & `deli-0.2.3/deli/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/images.py` & `deli-0.2.3/deli/serializers/images.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/nifty.py` & `deli-0.2.3/deli/serializers/nifty.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/numpy_.py` & `deli-0.2.3/deli/serializers/numpy_.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli/serializers/packaged.py` & `deli-0.2.3/deli/serializers/packaged.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/deli.egg-info/PKG-INFO` & `deli-0.2.3/deli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
-Download-URL: https://github.com/maxme1/deli/archive/v0.2.2.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.3.tar.gz
 Author-email: Max <maxs987@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 maxme1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `deli-0.2.2/deli.egg-info/SOURCES.txt` & `deli-0.2.3/deli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/pyproject.toml` & `deli-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/setup.py` & `deli-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.2/tests/test_serializers.py` & `deli-0.2.3/tests/test_serializers.py`

 * *Files identical despite different names*

