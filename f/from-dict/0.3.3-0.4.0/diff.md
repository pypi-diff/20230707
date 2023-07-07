# Comparing `tmp/from-dict-0.3.3.tar.gz` & `tmp/from-dict-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "from-dict-0.3.3.tar", last modified: Thu Dec  8 07:45:27 2022, max compression
+gzip compressed data, was "from-dict-0.4.0.tar", last modified: Fri Jul  7 05:52:54 2023, max compression
```

## Comparing `from-dict-0.3.3.tar` & `from-dict-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 monoid    (1001) users      (100)        0 2022-12-08 07:45:27.819652 from-dict-0.3.3/
--rw-r--r--   0 monoid    (1001) users      (100)     1070 2022-08-06 07:52:59.000000 from-dict-0.3.3/LICENSE
--rw-r--r--   0 monoid    (1001) users      (100)     3911 2022-12-08 07:45:27.819652 from-dict-0.3.3/PKG-INFO
--rw-r--r--   0 monoid    (1001) users      (100)     3215 2022-11-08 22:09:12.000000 from-dict-0.3.3/README.md
-drwxr-xr-x   0 monoid    (1001) users      (100)        0 2022-12-08 07:45:27.818653 from-dict-0.3.3/from_dict/
--rw-r--r--   0 monoid    (1001) users      (100)       53 2022-08-11 15:49:35.000000 from-dict-0.3.3/from_dict/__init__.py
--rw-r--r--   0 monoid    (1001) users      (100)    20874 2022-12-08 07:29:07.000000 from-dict-0.3.3/from_dict/_from_dict.py
-drwxr-xr-x   0 monoid    (1001) users      (100)        0 2022-12-08 07:45:27.819652 from-dict-0.3.3/from_dict.egg-info/
--rw-r--r--   0 monoid    (1001) users      (100)     3911 2022-12-08 07:45:27.000000 from-dict-0.3.3/from_dict.egg-info/PKG-INFO
--rw-r--r--   0 monoid    (1001) users      (100)      204 2022-12-08 07:45:27.000000 from-dict-0.3.3/from_dict.egg-info/SOURCES.txt
--rw-r--r--   0 monoid    (1001) users      (100)        1 2022-12-08 07:45:27.000000 from-dict-0.3.3/from_dict.egg-info/dependency_links.txt
--rw-r--r--   0 monoid    (1001) users      (100)       10 2022-12-08 07:45:27.000000 from-dict-0.3.3/from_dict.egg-info/top_level.txt
--rw-r--r--   0 monoid    (1001) users      (100)       38 2022-12-08 07:45:27.819652 from-dict-0.3.3/setup.cfg
--rw-r--r--   0 monoid    (1001) users      (100)      974 2022-12-08 07:45:07.000000 from-dict-0.3.3/setup.py
+drwxr-xr-x   0 monoid    (1001) users      (100)        0 2023-07-07 05:52:54.750494 from-dict-0.4.0/
+-rw-r--r--   0 monoid    (1001) users      (100)     1070 2022-08-06 07:52:59.000000 from-dict-0.4.0/LICENSE
+-rw-r--r--   0 monoid    (1001) users      (100)     3999 2023-07-07 05:52:54.750494 from-dict-0.4.0/PKG-INFO
+-rw-r--r--   0 monoid    (1001) users      (100)     3353 2023-07-07 05:47:54.000000 from-dict-0.4.0/README.md
+drwxr-xr-x   0 monoid    (1001) users      (100)        0 2023-07-07 05:52:54.748494 from-dict-0.4.0/from_dict/
+-rw-r--r--   0 monoid    (1001) users      (100)       79 2023-07-07 05:47:54.000000 from-dict-0.4.0/from_dict/__init__.py
+-rw-r--r--   0 monoid    (1001) users      (100)    22207 2023-07-07 05:47:54.000000 from-dict-0.4.0/from_dict/_from_dict.py
+drwxr-xr-x   0 monoid    (1001) users      (100)        0 2023-07-07 05:52:54.749493 from-dict-0.4.0/from_dict.egg-info/
+-rw-r--r--   0 monoid    (1001) users      (100)     3999 2023-07-07 05:52:54.000000 from-dict-0.4.0/from_dict.egg-info/PKG-INFO
+-rw-r--r--   0 monoid    (1001) users      (100)      451 2023-07-07 05:52:54.000000 from-dict-0.4.0/from_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 monoid    (1001) users      (100)        1 2023-07-07 05:52:54.000000 from-dict-0.4.0/from_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 monoid    (1001) users      (100)       10 2023-07-07 05:52:54.000000 from-dict-0.4.0/from_dict.egg-info/top_level.txt
+-rw-r--r--   0 monoid    (1001) users      (100)       38 2023-07-07 05:52:54.750494 from-dict-0.4.0/setup.cfg
+-rw-r--r--   0 monoid    (1001) users      (100)      926 2023-07-07 05:47:54.000000 from-dict-0.4.0/setup.py
+drwxr-xr-x   0 monoid    (1001) users      (100)        0 2023-07-07 05:52:54.750494 from-dict-0.4.0/tests/
+-rw-r--r--   0 monoid    (1001) users      (100)     2826 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_caching.py
+-rw-r--r--   0 monoid    (1001) users      (100)    17119 2023-07-07 05:47:54.000000 from-dict-0.4.0/tests/test_from_dict.py
+-rw-r--r--   0 monoid    (1001) users      (100)     4884 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_generics_with_dataclasses.py
+-rw-r--r--   0 monoid    (1001) users      (100)     3656 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_namespaces_class.py
+-rw-r--r--   0 monoid    (1001) users      (100)     1063 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_readme_example.py
+-rw-r--r--   0 monoid    (1001) users      (100)     1642 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_self_references_global.py
+-rw-r--r--   0 monoid    (1001) users      (100)     1683 2022-11-08 22:09:12.000000 from-dict-0.4.0/tests/test_self_references_local.py
+-rw-r--r--   0 monoid    (1001) users      (100)    16969 2023-07-07 05:47:54.000000 from-dict-0.4.0/tests/test_type_checking.py
```

### Comparing `from-dict-0.3.3/LICENSE` & `from-dict-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `from-dict-0.3.3/PKG-INFO` & `from-dict-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: from-dict
-Version: 0.3.3
+Version: 0.4.0
 Summary: Create data structures from dictionaries.
 Home-page: https://github.com/wchresta/from-dict
 Author: Wanja Chresta
 Author-email: wanja.hs@chrummibei.ch
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # from-dict
 Create data structures from partially known dictionaries.
 
 ## Features
 * Transform dicts to `attr.s`, `dataclass`, `NamedTuple`, and normal classes that have type-hints for all their __init__ parameters.
 * Supports nested structures when using `typing.List` and `typing.Dict` type hints.
 * Insert additional fields existing in dict into structure with `fd_copy_unknown=True`
 * Optional run-time type-checking with `fd_check_types=True`
 * Supports forward references
+* Raise an exception if there are more arguments supplied than are required with `fd_error_on_unknown=True`
+* Supports Literal type hints
 
 
 ## Example
 ```python
 from dataclasses import dataclass
 from typing import List, Optional
 from from_dict import from_dict
```

### Comparing `from-dict-0.3.3/README.md` & `from-dict-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 ## Features
 * Transform dicts to `attr.s`, `dataclass`, `NamedTuple`, and normal classes that have type-hints for all their __init__ parameters.
 * Supports nested structures when using `typing.List` and `typing.Dict` type hints.
 * Insert additional fields existing in dict into structure with `fd_copy_unknown=True`
 * Optional run-time type-checking with `fd_check_types=True`
 * Supports forward references
+* Raise an exception if there are more arguments supplied than are required with `fd_error_on_unknown=True`
+* Supports Literal type hints
 
 
 ## Example
 ```python
 from dataclasses import dataclass
 from typing import List, Optional
 from from_dict import from_dict
```

### Comparing `from-dict-0.3.3/from_dict/_from_dict.py` & `from-dict-0.4.0/from_dict/_from_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import functools
 import sys
 import typing
+from collections import ChainMap
 from dataclasses import is_dataclass
-from typing import Any, Callable, Dict, ForwardRef, Mapping, Optional, Type
-from typing import TypeVar, Union
+from typing import Any, Callable, Dict, ForwardRef, Mapping, Optional, Type, Literal
+from typing import TypeVar, Union, List, get_args, get_origin
 
 PYTHON_VERSION = sys.version_info[:2]
-# Support for typing.get_args and typing.get_origin
-IS_GE_PYTHON38 = PYTHON_VERSION >= (3, 8)
 IS_GE_PYTHON39 = PYTHON_VERSION >= (3, 9)
 C = TypeVar("C")
 
 
 class FromDictTypeError(TypeError):
     def __init__(self, location, expected_type, found_type):
         self.location = location
@@ -21,14 +20,26 @@
     def __str__(self):
         return f"For \"{'.'.join(self.location)}\", expected {self.expected_type} but found {self.found_type}"
 
     def __repr__(self):
         return f"FromDictTypeError({self.location!r}, {self.expected_type!r}, {self.found_type!r})"
 
 
+class FromDictUnknownArgsError(ValueError):
+    def __init__(self, unknown_args: List[str]):
+        self.unknown_args = unknown_args
+
+    def __str__(self):
+        names = ",".join((repr(a) for a in self.unknown_args))
+        return f"'fd_error_on_unknown' is set and the following extra arguments were supplied {names}"
+
+    def __repr__(self):
+        return f"FromDictUnknownArgsError({self.unknown_args!r})"
+
+
 class NamespaceTypes:
     def __init__(self, global_ns: Optional[dict], local_ns: Optional[dict]) -> None:
         """We only care about the entries with classes in them.
         For local namespaces if a class is defined inline it will not compare
         equal to itself.
         """
 
@@ -59,33 +70,17 @@
             self is o
             or self._hash == o._hash
             and self._global_types == o._global_types
             and self._local_types == o._local_types
         )
 
 
-if IS_GE_PYTHON38:
-    from typing import get_args, get_origin
-else:
-
-    def get_origin(tp) -> Optional[type]:
-        if hasattr(tp, "__origin__"):
-            return tp.__origin__
-        else:
-            return None
-
-    def get_args(tp) -> tuple:
-        if hasattr(tp, "__args__"):
-            return tp.__args__
-        else:
-            return ()
-
-
 def type_check(check_stack: list, v: Any, t: type) -> None:
     """Raise FromDictTypeError if given value does not agree with given type"""
+
     # This uses typing.get_args and typing.get_origin
     def location():
         return ["".join(check_stack)]
 
     try:
         passed_isinstance = isinstance(v, t)
     except TypeError:  # Could happen if t is of sort List[x], etc.
@@ -103,14 +98,18 @@
         for targ in type_args:
             try:
                 type_check(check_stack, v, targ)
                 return  # Successfully type checked
             except FromDictTypeError:
                 pass
         raise FromDictTypeError(location(), t, type(v))
+    if origin == Literal:
+        if any(a == v for a in type_args):
+            return  # Successfully type checked
+        raise FromDictTypeError(location(), f"literal value(s) {type_args}", repr(v))
 
     if not isinstance(v, origin):  # list ~ List[x], dict ~ Dict[x,y]
         raise FromDictTypeError(location(), t, type(v))
 
     if origin == list:
         targ = type_args[0]
         if not isinstance(v, list):
@@ -228,14 +227,15 @@
 def from_dict(
     cls: Type[C],
     fd_from: Optional[dict] = None,
     fd_check_types: bool = False,
     fd_copy_unknown: bool = True,
     fd_global_ns: Optional[dict] = None,
     fd_local_ns: Optional[dict] = None,
+    fd_error_on_unknown: bool = False,
     **overwrite_kwargs: Any,
 ) -> C:
     """Instantiate a class with parameters given by a dict.
 
     The dict is searched for fitting parameters. Keys that are not named like a parameter are ignored.
 
     If cls has generic type annotations with type arguments being classes themselves (like typing.List[SubClass]),
@@ -246,33 +246,44 @@
     :param fd_from: Dictionary from which to read parameters.
     :param fd_check_types: Should type-checking at run-time be performed.
     :param fd_copy_unknown:
         Should additional keys not used in constructor be inserted into __dict__. This is on by default. This will only
         have an effect if constructed object has a __dict__.
     :param fd_global_ns: global namespace to help with handling of forward references encoded as string literals
     :param fd_local_ns: local namespace to help with handling of forward references encoded as string literals
+    :param fd_error_on_unknown:
+        Should a 'FromDictUnknownArgsError' exception be raised if additional arguments are supplied that are not
+        used in constructor. If this is True, fd_copy_unknown has to be set to False
     :param overwrite_kwargs: All additional keys will overwrite whatever is given in the dictionary.
     :return: Object of cls constructed with keys extracted from fd_from.
     """
+    if fd_copy_unknown and fd_error_on_unknown:
+        raise ValueError(
+            "'fd_copy_unknown' and 'fd_error_on_unknown' can't both be true"
+        )
+
     ns_types = NamespaceTypes(fd_global_ns, fd_local_ns)
     given_args = {}
     if fd_from:
         if not isinstance(fd_from, dict):
             raise TypeError(f"fd_from must be dict but was found to be {type(fd_from)}")
         given_args.update(fd_from)
     if overwrite_kwargs:
         given_args.update(overwrite_kwargs)
-    return _from_dict_inner(cls, given_args, fd_check_types, fd_copy_unknown, ns_types)
+    return _from_dict_inner(
+        cls, given_args, fd_check_types, fd_copy_unknown, fd_error_on_unknown, ns_types
+    )
 
 
 def _from_dict_inner(
     cls: Type[C],
     given_args: Union[dict, Any],
     fd_check_types: bool,
     fd_copy_unknown: bool,
+    fd_error_on_unknown: bool,
     ns_types: NamespaceTypes,
 ) -> C:
     if not isinstance(given_args, dict):
         return given_args
 
     _get_constructor_type_hints = functools.partial(
         get_constructor_type_hints, ns_types=ns_types
@@ -280,14 +291,15 @@
     _resolve_str_forward_ref = functools.partial(
         resolve_str_forward_ref, cls=cls, ns_types=ns_types
     )
     _from_dict = functools.partial(
         _from_dict_inner,
         fd_check_types=fd_check_types,
         fd_copy_unknown=fd_copy_unknown,
+        fd_error_on_unknown=fd_error_on_unknown,
         ns_types=ns_types,
     )
 
     cls_constructor_argument_types = _get_constructor_type_hints(cls)
     if not cls_constructor_argument_types:
         raise TypeError(f"Given class {cls} is not supported by from_dict")
 
@@ -317,21 +329,27 @@
         if fd_check_types:
             type_check([cls_argument_name], argument_value, cls_argument_type)
 
         ckwargs[cls_argument_name] = argument_value
 
     created_object = cls(**ckwargs)
 
-    # Check if created_object has a dictionary:
-    if fd_copy_unknown and given_args and hasattr(created_object, "__dict__"):
-        # Add the rest of the arguments to the dict, if possible.
-        # Do not overwrite existing keys
-        for arg, val in given_args.items():
-            if arg not in ckwargs and arg not in created_object.__dict__:
-                created_object.__dict__[arg] = val
+    if given_args and (fd_copy_unknown or fd_error_on_unknown):
+        created_object_dict = getattr(created_object, "__dict__", None)
+        known_args = ChainMap(ckwargs, created_object_dict or {})
+
+        # Check if created_object has a dictionary:
+        if fd_copy_unknown and created_object_dict is not None:
+            # Add the rest of the arguments to the dict, if possible.
+            # Do not overwrite existing keys
+            unknown_args = {k: v for k, v in given_args.items() if k not in known_args}
+            created_object.__dict__.update(unknown_args)
+        elif fd_error_on_unknown and set(given_args).difference(known_args):
+            unknown_args = [k for k in given_args if k not in known_args]
+            raise FromDictUnknownArgsError(unknown_args)
 
     return created_object
 
 
 def handle_item(
     _get_constructor_type_hints: Callable[[Type], Mapping[str, Type]],
     _resolve_str_forward_ref,
@@ -419,14 +437,16 @@
                         _resolve_str_forward_ref,
                         _from_dict,
                         value_type,
                         v,
                     )
                     for k, v in given_argument.items()
                 }
+            if value_type_origin is Literal:
+                return given_argument
 
         # Any object that has type-hints in the constructor
         if _get_constructor_type_hints(value_type):
             return {k: _from_dict(value_type, v) for k, v in given_argument.items()}
 
         # The dictionary value's type does not need to be converted
         # Examples: int, str, or dict (with no type-hints)
@@ -496,25 +516,27 @@
                         _from_dict,
                         element_type,
                         element,
                     )
                     for element in given_argument
                 ]
 
-            if get_origin(element_type) is Union:
+            if element_type_origin is Union:
                 return [
                     _handle_union(
                         _get_constructor_type_hints,
                         _resolve_str_forward_ref,
                         _from_dict,
                         element_type,
                         v,
                     )
                     for v in given_argument
                 ]
+            if element_type_origin is Literal:
+                return given_argument
 
         # Any object that has type-hints in the constructor
         if _get_constructor_type_hints(element_type):
             return [_from_dict(element_type, x) for x in given_argument]
 
         # The list value's type does not need to be converted
         # Examples: int, str, or dict (with no type-hints)
```

### Comparing `from-dict-0.3.3/from_dict.egg-info/PKG-INFO` & `from-dict-0.4.0/from_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: from-dict
-Version: 0.3.3
+Version: 0.4.0
 Summary: Create data structures from dictionaries.
 Home-page: https://github.com/wchresta/from-dict
 Author: Wanja Chresta
 Author-email: wanja.hs@chrummibei.ch
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # from-dict
 Create data structures from partially known dictionaries.
 
 ## Features
 * Transform dicts to `attr.s`, `dataclass`, `NamedTuple`, and normal classes that have type-hints for all their __init__ parameters.
 * Supports nested structures when using `typing.List` and `typing.Dict` type hints.
 * Insert additional fields existing in dict into structure with `fd_copy_unknown=True`
 * Optional run-time type-checking with `fd_check_types=True`
 * Supports forward references
+* Raise an exception if there are more arguments supplied than are required with `fd_error_on_unknown=True`
+* Supports Literal type hints
 
 
 ## Example
 ```python
 from dataclasses import dataclass
 from typing import List, Optional
 from from_dict import from_dict
```

### Comparing `from-dict-0.3.3/setup.py` & `from-dict-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="from-dict",
-    version="0.3.3",
+    version="0.4.0",
     packages=find_packages(),
     author="Wanja Chresta",
     author_email="wanja.hs@chrummibei.ch",
     url="https://github.com/wchresta/from-dict",
     description="Create data structures from dictionaries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[],
-    tests_require=["pytest", "attr"],
+    tests_require=["pytest", "attrs"],
 )
```

