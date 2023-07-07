# Comparing `tmp/ktz-0.2.0rc0.tar.gz` & `tmp/ktz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktz-0.2.0rc0.tar", last modified: Mon Oct  3 13:52:09 2022, max compression
+gzip compressed data, was "ktz-0.3.0.tar", last modified: Fri Jul  7 12:55:22 2023, max compression
```

## Comparing `ktz-0.2.0rc0.tar` & `ktz-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:52:09.961973 ktz-0.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-03 13:52:09.961973 ktz-0.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:52:09.957973 ktz-0.2.0rc0/ktz/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     5836 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/functools.py
--rw-r--r--   0 runner    (1001) docker     (121)    11166 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/ktz/string.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 13:52:09.957973 ktz-0.2.0rc0/ktz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-03 13:52:09.000000 ktz-0.2.0rc0/ktz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-03 13:52:09.000000 ktz-0.2.0rc0/ktz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 13:52:09.000000 ktz-0.2.0rc0/ktz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-03 13:52:09.000000 ktz-0.2.0rc0/ktz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-03 13:52:09.000000 ktz-0.2.0rc0/ktz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-10-03 13:52:09.961973 ktz-0.2.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-03 13:51:39.000000 ktz-0.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:22.934343 ktz-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 12:54:13.000000 ktz-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-07 12:55:22.934343 ktz-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-07 12:54:13.000000 ktz-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:22.934343 ktz-0.3.0/ktz/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-07 12:54:13.000000 ktz-0.3.0/ktz/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:55:22.934343 ktz-0.3.0/ktz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-07 12:55:22.000000 ktz-0.3.0/ktz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-07 12:55:22.000000 ktz-0.3.0/ktz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:55:22.000000 ktz-0.3.0/ktz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-07 12:55:22.000000 ktz-0.3.0/ktz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 12:55:22.000000 ktz-0.3.0/ktz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-07 12:55:22.934343 ktz-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 12:54:13.000000 ktz-0.3.0/setup.py
```

### Comparing `ktz-0.2.0rc0/LICENSE` & `ktz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ktz-0.2.0rc0/PKG-INFO` & `ktz-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktz
-Version: 0.2.0rc0
+Version: 0.3.0
 Summary: KTZ Python Tools
 Home-page: https://github.com/kantholtz/ktz
 Author: Felix Hamann
 Author-email: felix@hamann.xyz
 Project-URL: Bug Tracker, https://github.com/kantholtz/ktz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # KTZ - Python Tools
 
 [![Documentation](https://img.shields.io/badge/Documentation-Latest-success?style=for-the-badge)](https://kantholtz.github.io/ktz/)
-[![Master Checks](https://img.shields.io/github/workflow/status/kantholtz/ktz/Current%20Master%20Checks?style=for-the-badge&label=Master%20Checks)](https://github.com/kantholtz/ktz/actions/workflows/development.yml)
 [![KTZ on PyPI](https://img.shields.io/pypi/v/ktz?style=for-the-badge)](https://pypi.org/project/ktz)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 
 
 Kantholtz' personal Python toolbox. Check out the [documentation here](https://kantholtz.github.io/ktz/).
```

### Comparing `ktz-0.2.0rc0/README.md` & `ktz-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # KTZ - Python Tools
 
 [![Documentation](https://img.shields.io/badge/Documentation-Latest-success?style=for-the-badge)](https://kantholtz.github.io/ktz/)
-[![Master Checks](https://img.shields.io/github/workflow/status/kantholtz/ktz/Current%20Master%20Checks?style=for-the-badge&label=Master%20Checks)](https://github.com/kantholtz/ktz/actions/workflows/development.yml)
 [![KTZ on PyPI](https://img.shields.io/pypi/v/ktz?style=for-the-badge)](https://pypi.org/project/ktz)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 
 
 Kantholtz' personal Python toolbox. Check out the [documentation here](https://kantholtz.github.io/ktz/).
```

### Comparing `ktz-0.2.0rc0/ktz/collections.py` & `ktz-0.3.0/ktz/collections.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# -*- coding: utf-8 -*-
 """Tools for working with collection types."""
 
-
 import copy
 import logging
 import warnings
 from collections import defaultdict
 from collections.abc import Collection, Generator, Iterable, Mapping
 from functools import partial
+from inspect import signature
 from itertools import count
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 
 import yaml
 
-from ktz.filesystem import path as kpath
+from ktz.filesystem import path as path
 
 log = logging.getLogger(__name__)
 
 
 #
 #   COLLECTIONS
 #
@@ -111,30 +110,31 @@
     >>> unbucket(parts)
     [(False, 1), (False, 3), (False, 5), (True, 2), (True, 4)]
 
     """
     return [(key, el) for key, lis in buckets.items() for el in lis]
 
 
-Nested = Union[Iterable[A], A]
+# cannot get Union[list, tuple] to be a Generic
+Nested = Union[list[A], A]
 
 
-def flat(
-    col: Iterable[Nested],
+def lflat(
+    col: Nested,
     depth: int = -1,
 ) -> Generator[A, None, None]:
-    """Flattens a collection.
+    """Flattens a tuple or list.
 
-    Consumes the given iterable and flattens it up to
+    Consumes the given sequence and flattens it up to
     n levels deep or completely.
 
     Parameters
     ----------
-    col : Iterable[Nested]
-        Nested collection
+    col : Nested
+        Nested list or tuple
     depth : int
         Maximum depth to flatten
 
     Returns
     -------
     Generator[A, None, None]
         Generator with flattened collection
@@ -142,49 +142,71 @@
     Examples
     --------
     >>> from ktz.collections import flat
     >>> flat([[1], [[2]]], depth=2)
     <generator object flat at 0x7f2886aeccf0>
     >>> list(flat([[1], [[2]]], depth=2))
     [1, [2]]
+    >>> list(flat([["foo"], [["bar"]]]))
+    ["foo", "bar"]
 
     """
-    if depth == 0:
+    isseq = isinstance(col, list) or isinstance(col, tuple)
+    if depth == 0 or not isseq:
         yield col
         return
 
     try:
         for elem in col:
-            yield from flat(col=elem, depth=depth - 1)
+            yield from lflat(col=elem, depth=depth - 1)
     except TypeError:
         yield col
 
 
 class Incrementer(dict):
-    """
-    Automatically assign unique ids.
+    """Automatically assign unique ids.
+
+    This is basically a defaultdict using a state which remembers the
+    latest assigned id and assigns its increment when queried for a
+    missing item. It can be frozen to error out on unknown keys. You
+    can overwrite the built-in incrementer by providing your own iterable
+    upon instantiation using the fn kwarg.
+
+    Parameters
+    ----------
+    dict : dict
+        Base dictionary
+    fn : Iterable
+        Custom iterable to use instead of count()
+
+    Raises
+    ------
+    NameError
+        Thrown if the dict is frozen and an unknown key is accessed
+    KeyError
+        Thrown for invalid explicit setting of values
+    StopIteration
+        Thrown for depleted custom iterators given to __init__
 
     Examples
     --------
     >>> from ktz.collections import Incrementer
-    >>> incr = Incrementer()
-    >>> incr['a']
-    0
-    >>> incr['b']
-    1
-    >>> incr['a']
-    0
-    >>> incr['c']
-    2
-    >>> incr.freeze()
-    >>> incr['d']
-    NameError: Key 'd' not present and incrementer is frozen.
-    >>> incr.unfreeze()
-    >>> incr['d']
-    3
+    >>> # using a custom fn to control the assigned ids
+    >>> from itertools import count
+    >>> ids = Incrementer(fn=count(10))
+    >>> ids[4]
+    10
+    >>> ids[10]
+    11
+    >>> ids
+    {4: 10, 10: 11}
+    >>> ids.freeze()
+    >>> ids[3]
+    NameError: Key '3' not present and incrementer is frozen.
+
     """
 
     def __init__(self, *args, fn: Iterable[A] = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.unfreeze()
 
         # iter() is idempotent and iterators are iterable
@@ -200,27 +222,49 @@
         if key not in self:
             val = next(self._iterator)
             super().__setitem__(key, val)
 
         return super().__getitem__(key)
 
     def freeze(self):
-        """
-        Freeze the incrementer.
+        """Freeze the incrementer.
 
         It is no longer possible to automatically create new keys.
 
+        Examples
+        --------
+        >>> from ktz.collections import Incrementer
+        >>> ids = Incrementer()
+        >>> ids[1]
+        0
+        >>> ids.freeze()
+        >>> ids[1]
+        0
+        >>> ids[2]
+        NameError: Key '2' not present and incrementer is frozen.
+
         """
         self._frozen = True
 
     def unfreeze(self):
         """Unfreeze the incrementer.
 
         Allows the creation of new keys again
 
+        Examples
+        --------
+        >>> from ktz.collections import Incrementer
+        >>> ids = Incrementer()
+        >>> ids.freeze()
+        >>> ids[2]
+        NameError: Key '2' not present and incrementer is frozen.
+        >>> ids.unfreeze()
+        >>> ids[2]
+        0
+
         """
         self._frozen = False
 
 
 # --
 
 
@@ -236,16 +280,20 @@
     """
     Resolve string trails in deep dictionaries.
 
     For example, with sep="." and collapse=0
     foo.bar.baz -> dic['foo']['bar']['baz']. Setting
     collapse=1 would return dic['foo']['bar'] = {'baz': ...}
 
-    Parameters:
-    -----------
+    It is also possible to use wildcards in the querz string
+    to skip unknown but unambiguous (i.e. single-key dict)
+    entries.
+
+    Parameters
+    ----------
     dic : Mapping
         Data to be looked up
     chain : str
         Query string
     sep : str
         How the chain needs to be split
     collapse : Optional[int]
@@ -272,46 +320,55 @@
       File ~/Complex/scm/ktz/ktz/collections.py:264 in drslv
         dic = dic[key]
     KeyError: 'not'
 
     >>> drslv(dic, 'not.there', default=None)
     >>> drslv(dic, 'not.there', default=1)
     1
-
+    >>> drslv(dic, 'foo.*.a')  # only works for single-element dicts
+    1
     """
     if skiplast:
         warnings.warn(
             "'skiplast' is deprecated; use 'collapse' instead",
             DeprecationWarning,
             stacklevel=2,
         )
         collapse = skiplast
 
     crumbs = chain.split(sep)
 
     try:
         trail = []
         for key in crumbs:
+            if not isinstance(dic, dict):
+                raise KeyError
+
             trail.append(dic)
+
+            if key == "*":
+                if len(dic) > 1:
+                    raise KeyError(f"Multiple candidates for wildcard: {list(dic)}")
+                key = list(dic)[0]
+
             dic = dic[key]
 
     except KeyError as err:
         if default == KeyError:
-            raise err
+            raise KeyError(f"drsvl: {err} not found for {chain}")
 
         return default
 
     return trail[-collapse] if collapse else dic
 
 
 def dflat(
     dic,
     sep: str = ".",
     only: Optional[int] = None,
-    # skiplast: Optional[int] = None,
 ):
     """
     Flatten a deep dictionary with string keys.
 
     Takes a deeply nested dictionary and flattens it by concatenating
     its keys using the provided separator. For example a dictionary
     d['foo']['bar'] = 3 becomes d['foo.bar'] = 3. Keys are transformed
@@ -321,16 +378,14 @@
     ----------
     dic : Mapping[str, XXXX]
         The dictionary to be flattened
     sep : str
         Separator to concatenate the keys with
     only : Optional[int]
         Stops flattening after the provided depth
-    skiplast : Optional[int]
-        Do not flatten up to n hops from each leaf
 
     Examples
     --------
     >>> from ktz.collections import dflat
     >>> dic = dict(foo=dict(bar=dict(a=1,b=2),c=3),d=4)
     >>> dflat(dic)
     {'foo.bar.a': 1, 'foo.bar.b': 2, 'foo.c': 3, 'd': 4}
@@ -338,18 +393,18 @@
     {'foo bar a': 1, 'foo bar b': 2, 'foo c': 3, 'd': 4}
     >>> dflat(dic, only=2)
     {'foo.bar': {'a': 1, 'b': 2}, 'foo.c': 3, 'd': 4}
 
     """
 
     def descend(v, depth):
-        if not isinstance(v, Mapping):
+        if not isinstance(v, Mapping) or len(v) == 0:
             return False
 
-        if only is None or depth < only:
+        if (only is None) or (depth < only):
             return True
 
         return False
 
     def rec(src: Mapping, tar: Mapping, trail: list[str]):
         for k, v in src.items():
             subtrail = trail + [str(k)]
@@ -357,15 +412,15 @@
                 rec(v, tar, subtrail)
             else:
                 tar[sep.join(subtrail)] = v
 
         return tar
 
     # step 1: flatten completely
-    return rec(dic, {}, [])
+    return rec(dic, tar={}, trail=[])
 
 
 def dmerge(*ds: Mapping):
     """
     Deeply merge mappings.
 
     A new deep copy is created from the keys and values from the
@@ -375,15 +430,19 @@
     Parameters
     ----------
     ds : Mapping
         Deep mappings to be merged
 
     Examples
     --------
-    FIXME: Add docs.
+    >>> from ktz.collections import dmerge
+    >>> d1 = dict(foo=dict(a=1, b=2), bar=3)
+    >>> d2 = dict(foo=dict(a=3, c=4), xyz=5)
+    >>> dmerge(d1, d2)
+    {'foo': {'a': 3, 'b': 2, 'c': 4}, 'bar': 3, 'xyz': 5}
 
     """
     if len(ds) == 0:
         return {}
 
     if len(ds) == 1:
         return copy.deepcopy(ds[0])
@@ -402,27 +461,84 @@
             else:
                 curr[k] = dmerge(curr[k] or {}, last[k])
 
         last = curr
     return curr
 
 
+def _dconv(dic: dict, fns):
+    res = {}
+    for k, v in dic.items():
+        if isinstance(v, Mapping):
+            res[k] = _dconv(v, fns)
+            continue
+
+        res[k] = v
+        for fn, argc in fns:
+            assert argc in {1, 2}, "converter functions accept 1 or 2 arguments"
+            res[k] = fn(res[k]) if argc == 1 else fn(res[k], k)
+
+    return res
+
+
+def dconv(dic: dict, *convert: Callable[[A, B], C]):
+    """
+    Convert a dictionary deeply.
+
+    A pipeline of converter functions may be provided which transform
+    the values of the given mapping. It always returns a deep copy of
+    the mapping as a dictionary. The converter functions are applied
+    in the given order.
+
+    Parameters
+    ----------
+    dic : dict
+        Mapping to be copied and transformed
+    *convert : Callable[[A, B], C]
+        Converter functions
+
+    Examples
+    --------
+    >>> from ktz.collections import dconv
+    >>> dconv(dict(a=1, d=dict(b=2, c=3)), lambda v: v + 2)
+    {'a': 3, 'd': {'b': 4, 'c': 5}}
+    >>> dconv(dict(a=1, d=dict(b=2, c=3)), lambda v, k: True if k == 'b' else False)
+    {'a': False, 'd': {'b': True, 'c': False}}
+
+    """
+
+    # Obtain function signatures for converter functions to determine
+    # whether additionally the key needs to be given to the converter.
+    # As with nearly all cases, "don't ask for permission but for
+    # forgiveness" is a bad anti-pattern because we never know whether
+    # we accidentally catch a TypeError produced by the invoker.
+    fns = [(fn, len(signature(fn).parameters)) for fn in convert]
+    return _dconv(dic, fns)
+
+
 def ryaml(*configs: Union[Path, str], **overwrites) -> dict:
     """
     Load and join configurations from yaml and kwargs.
 
     First, all provided configuration files are loaded
     and joined together. Afterwards, all provided kwargs
     overwrite the joined configuration dict.
 
+    Parameters
+    ----------
+    *configs : Union[Path, str]
+        Config files to be read and merged
+    **overwrites : Any
+        To overwrite loaded values
+
     """
-    as_path = partial(kpath, is_file=True)
+    as_path = partial(path, is_file=True)
 
     # first join all yaml configs into one dictionary;
     # later dictionaries overwrite earlier ones
     loaded = []
-    for path in map(as_path, configs):
-        with path.open(mode="r") as fd:
+    for filepath in map(as_path, configs):
+        with filepath.open(mode="r") as fd:
             loaded.append(yaml.safe_load(fd) or {})
 
     work = loaded + [overwrites]
     return dmerge(*work)
```

### Comparing `ktz-0.2.0rc0/ktz/filesystem.py` & `ktz-0.3.0/ktz/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # -*- coding: utf-8 -*-
 
 """Things to do with the filesystem."""
 
-import ktz
-
-import pathlib
 import logging
+import pathlib
+import warnings
+from typing import Optional, Union
 
-import git
-
-
-from typing import Union
-from typing import Optional
-
+import ktz
 
 log = logging.getLogger(__name__)
 
 
 def path(
     name: Union[str, pathlib.Path],
     create: bool = False,
@@ -173,10 +168,14 @@
     Examples
     --------
     >>> from ktz.filesystem import git_hash
     >>> git_hash()
     'bedee821a4c1e1217cee783b33ad3bea98dbbb9d'
 
     """
+    warnings.warn("to be removed in 0.4", DeprecationWarning)
+
+    import git
+
     repo = git.Repo(search_parent_directories=True)
     # dirty = '-dirty' if repo.is_dirty else ''
     return str(repo.head.object.hexsha)
```

### Comparing `ktz-0.2.0rc0/ktz/functools.py` & `ktz-0.3.0/ktz/functools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 # -*- coding: utf-8 -*-
 
 """Nice function-functions."""
 
-import pickle
 import logging
-from pathlib import Path
+import pickle
+from dataclasses import dataclass, field, replace
 from functools import wraps
-from dataclasses import field
-from dataclasses import replace
-from dataclasses import dataclass
-
-from ktz.filesystem import path as kpath
-
-from typing import Union
-from typing import TypeVar
-from typing import Generic
+from pathlib import Path
+from typing import Generic, TypeVar, Union
 
+from ktz.filesystem import path
 
 T = TypeVar("T")
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Maybe(Generic[T]):
@@ -57,27 +51,85 @@
         return (
             f"Maybe {self.cache} "
             f"skip={self.skip} loaded={self.loaded} cached={self.cached}"
         )
 
 
 class Cascade:
-    """
-    Cascading and cached function execution.
+    """Cascading cached function execution.
 
     This class is used to iteratively work with data. If a long
     pipeline requires much data to be processed linearly but some
     steps are very resoure intensive, this cascade is used to
     automatically resume the latest step and omit all previous
     steps. This is heavily used for iterative development of data
     processing pipelines in ipython notebooks.
 
+    Raises
+    ------
+    KeyError
+        Thrown if a value is requested which has not been cached yet
+
     Examples
     --------
-    FIXME: add docs
+    >>> # FIRST SESSION:
+    >>> !mkdir .cache
+    >>> from ktz.functools import Cascade                                                                                [70/193]
+    >>> # this defines two to be cached values x and y
+    >>> # where y depends on x
+    >>> run = Cascade(prefix='.cache', x='x.pkl', y='y.pkl')
+    >>> outside = 1
+    >>> @run.cache("x")
+    ... def f():
+    ...     return outside
+    ...
+    >>> @run.cache("y")
+    ... def g(a):
+    ...     return a + 1
+    ...
+    >>> x = f()
+    >>> x
+    1
+    >>> outside += 1
+    >>> outside
+    2
+    >>> # x is cached now!
+    >>> x = f()
+    >>> x
+    1
+    >>> # executing g is now preventing f
+    >>> # to be run in the future
+    >>> y = g(x)
+    >>> y
+    2
+    >>>
+    Do you really want to exit ([y]/n)? y
+    >>> # SECOND SESSION:
+    >>> from ktz.functools import Cascade                                                                                [70/193]
+    >>> # this defines two to be cached values x and y
+    >>> # where y depends on x
+    >>> run = Cascade(prefix='.cache', x='x.pkl', y='y.pkl')
+    >>> outside = 100
+    >>> @run.cache("x")
+    ... def f():
+    ...     return outside
+    ...
+    >>> @run.cache("y")
+    ... def g(a):
+    ...     return a + 1
+    >>> # f is not executed as g has already
+    >>> # computed and cached a value
+    >>> x = f()
+    >>> x is None
+    True
+    >>> # g is not executed and the cached value
+    >>> # is used instead
+    >>> y = g(x)
+    >>> y
+    2
 
     """
 
     path: Path
     data: dict[str, Maybe]
 
     def get(self, name: str):
@@ -164,15 +216,15 @@
 
         return decorator
 
     def when(self, *names: str):
         """
         Decorate conditionally executed function.
 
-        This decorator handles whether a function is invooked at all.
+        This decorator handles whether a function is invoked at all.
         It does not work with any returned data. Decorated functions
         always return None.
 
         """
         assert all(
             name in self.data for name in names
         ), f"cascade: unregistered names {names}"
@@ -189,29 +241,29 @@
 
             return maybe_execute
 
         return decorator
 
     def __init__(
         self,
-        path: Union[str, Path] = None,
+        prefix: Union[str, Path] = None,
         **kwargs: Union[str, Path],
     ):
         """
         Create a cached function cascade.
 
         Parameters
         ----------
-        path : Union[str, Path]
+        prefix : Union[str, Path]
             Optional basepath to be prepended to all cache files
         **kwargs : Union[str, Path]
             Register data keys
 
         """
-        self.path = kpath(path) if path else kpath(".")
+        self.path = path(prefix) if path else path(".")
         self.data = {}
 
         found = False
         while kwargs:
 
             name, cachefile = kwargs.popitem()  # lifo
             cache = self.path / cachefile
```

### Comparing `ktz-0.2.0rc0/ktz/multiprocessing.py` & `ktz-0.3.0/ktz/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `ktz-0.2.0rc0/ktz/string.py` & `ktz-0.3.0/ktz/string.py`

 * *Files identical despite different names*

### Comparing `ktz-0.2.0rc0/ktz.egg-info/PKG-INFO` & `ktz-0.3.0/ktz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktz
-Version: 0.2.0rc0
+Version: 0.3.0
 Summary: KTZ Python Tools
 Home-page: https://github.com/kantholtz/ktz
 Author: Felix Hamann
 Author-email: felix@hamann.xyz
 Project-URL: Bug Tracker, https://github.com/kantholtz/ktz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # KTZ - Python Tools
 
 [![Documentation](https://img.shields.io/badge/Documentation-Latest-success?style=for-the-badge)](https://kantholtz.github.io/ktz/)
-[![Master Checks](https://img.shields.io/github/workflow/status/kantholtz/ktz/Current%20Master%20Checks?style=for-the-badge&label=Master%20Checks)](https://github.com/kantholtz/ktz/actions/workflows/development.yml)
 [![KTZ on PyPI](https://img.shields.io/pypi/v/ktz?style=for-the-badge)](https://pypi.org/project/ktz)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
 
 
 Kantholtz' personal Python toolbox. Check out the [documentation here](https://kantholtz.github.io/ktz/).
```

### Comparing `ktz-0.2.0rc0/setup.cfg` & `ktz-0.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ktz
-version = 0.2.0rc0
+version = 0.3.0
 author = Felix Hamann
 author_email = felix@hamann.xyz
 description = KTZ Python Tools
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/kantholtz/ktz
 project_urls = 
@@ -22,21 +22,26 @@
 
 [options.extras_require]
 dev = 
 	build
 	ipdb
 	ipython
 	sphinx
+	sphinx-toolbox
 	numpydoc
+	pydata-sphinx-theme
 	black
 	pytest
 	pytest-watch
-	coverage
+	pytest-cov
 	tqdm
 	jupyter
+	pyls-isort
+	python-lsp-black
+	python-lsp-server[flake8]
 
 [flake8]
 max-line-length = 89
 ignore = D105, D107
 
 [coverage:report]
 exclude_lines =
```

