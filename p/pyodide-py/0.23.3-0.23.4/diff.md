# Comparing `tmp/pyodide-py-0.23.3.tar.gz` & `tmp/pyodide-py-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-py-0.23.3.tar", last modified: Sun Jun 18 02:24:23 2023, max compression
+gzip compressed data, was "pyodide-py-0.23.4.tar", last modified: Fri Jul  7 07:32:15 2023, max compression
```

## Comparing `pyodide-py-0.23.3.tar` & `pyodide-py-0.23.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.975789 pyodide-py-0.23.3/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_core_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/docs_argspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.979789 pyodide-py-0.23.3/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_package_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_run_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.979789 pyodide-py-0.23.3/pyodide/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/ffi/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/webloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/pyodide_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:15.882385 pyodide-py-0.23.4/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42535 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/_core_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/docs_argspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/_pyodide/docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/_package_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/_run_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/pyodide/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/ffi/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyodide/webloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/pyodide_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-07 07:32:15.000000 pyodide-py-0.23.4/pyodide_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 07:32:15.000000 pyodide-py-0.23.4/pyodide_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:32:15.000000 pyodide-py-0.23.4/pyodide_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 07:32:15.000000 pyodide-py-0.23.4/pyodide_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 07:32:15.886385 pyodide-py-0.23.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-07 07:31:58.000000 pyodide-py-0.23.4/webbrowser.py
```

### Comparing `pyodide-py-0.23.3/PKG-INFO` & `pyodide-py-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.3
+Version: 0.23.4
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.3/README.md` & `pyodide-py-0.23.4/README.md`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/_pyodide/_base.py` & `pyodide-py-0.23.4/_pyodide/_base.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/_pyodide/_core_docs.py` & `pyodide-py-0.23.4/_pyodide/_core_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,14 +983,18 @@
     def _new_exc(cls, name: str, message: str = "", stack: str = "") -> "JsException":
         result = super().__new__(JsException, _instantiate_token)
         result.name = name
         result.message = message
         result.stack = stack
         return result
 
+    @classmethod
+    def new(cls, *args: Any) -> "JsException":
+        return cls()
+
     def __str__(self):
         return f"{self.name}: {self.message}"
 
     name: str
     """The name of the error type"""
 
     message: str
```

### Comparing `pyodide-py-0.23.3/_pyodide/_importhook.py` & `pyodide-py-0.23.4/_pyodide/_importhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sys
-from collections.abc import Sequence
+from collections.abc import Callable, Sequence
 from importlib.abc import Loader, MetaPathFinder
 from importlib.machinery import ModuleSpec
 from importlib.util import spec_from_loader
 from types import ModuleType
 from typing import Any
 
 from ._core_docs import JsProxy
 
 
 class JsFinder(MetaPathFinder):
     def __init__(self) -> None:
         self.jsproxies: dict[str, Any] = {}
+        self.hook: Callable[[JsProxy], None] = lambda _: None
 
     def find_spec(
         self,
         fullname: str,
         path: Sequence[bytes | str] | None,
         target: ModuleType | None = None,
     ) -> ModuleSpec | None:
@@ -65,14 +66,15 @@
             raise TypeError(
                 f"Argument 'name' must be a str, not {type(name).__name__!r}"
             )
         if not isinstance(jsproxy, JsProxy):
             raise TypeError(
                 f"Argument 'jsproxy' must be a JsProxy, not {type(jsproxy).__name__!r}"
             )
+        self.hook(jsproxy)
         self.jsproxies[name] = jsproxy
 
     def unregister_js_module(self, name: str) -> None:
         """
         Unregisters a JavaScript module with given name that has been previously
         registered with :js:func:`pyodide.registerJsModule` or
         :py:func:`pyodide.ffi.register_js_module`. If a JavaScript module with that name
@@ -110,30 +112,30 @@
 
 
 jsfinder: JsFinder = JsFinder()
 register_js_module = jsfinder.register_js_module
 unregister_js_module = jsfinder.unregister_js_module
 
 
-def register_js_finder() -> None:
+def register_js_finder(*, hook: Callable[[JsProxy], None]) -> None:
     """A bootstrap function, called near the end of Pyodide initialization.
 
     It is called in ``loadPyodide`` in ``pyodide.js`` once ``_pyodide_core`` is ready
     to set up the js import mechanism.
 
         1. Put the right value into the global variable ``JsProxy`` so that
            ``JsFinder.find_spec`` can decide whether parent module is a Js module.
         2. Add ``jsfinder`` to metapath to allow js imports.
 
     This needs to be a function to allow the late import from ``_pyodide_core``.
     """
     for importer in sys.meta_path:
         if isinstance(importer, JsFinder):
             raise RuntimeError("JsFinder already registered")
-
+    jsfinder.hook = hook
     sys.meta_path.append(jsfinder)
 
 
 STDLIBS = sys.stdlib_module_names | {"test"}
 UNVENDORED_STDLIBS_AND_TEST: set[str] = set()
```

### Comparing `pyodide-py-0.23.3/_pyodide/docs_argspec.py` & `pyodide-py-0.23.4/_pyodide/docs_argspec.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/_pyodide/docstring.py` & `pyodide-py-0.23.4/_pyodide/docstring.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/__init__.py` & `pyodide-py-0.23.4/pyodide/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # All pure Python code that does not require js or pyodide_js should go in
 # the _pyodide package.
 #
 # This package is imported by the test suite as well, and currently we don't use
 # pytest mocks for js or pyodide_js, so make sure to test "if IN_BROWSER" before
 # importing from these.
-__version__ = "0.23.3"
+__version__ = "0.23.4"
 
 __all__ = ["__version__", "console", "code", "ffi", "http", "webloop"]
 
 from . import _state  # noqa: F401
 from .webloop import _initialize_event_loop
 
 _initialize_event_loop()
```

### Comparing `pyodide-py-0.23.3/pyodide/_package_loader.py` & `pyodide-py-0.23.4/pyodide/_package_loader.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/_state.py` & `pyodide-py-0.23.4/pyodide/_state.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/code.py` & `pyodide-py-0.23.4/pyodide/code.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/console.py` & `pyodide-py-0.23.4/pyodide/console.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/ffi/__init__.py` & `pyodide-py-0.23.4/pyodide/ffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/ffi/wrappers.py` & `pyodide-py-0.23.4/pyodide/ffi/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/http.py` & `pyodide-py-0.23.4/pyodide/http.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide/webloop.py` & `pyodide-py-0.23.4/pyodide/webloop.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/pyodide_py.egg-info/PKG-INFO` & `pyodide-py-0.23.4/pyodide_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.3
+Version: 0.23.4
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.3/pyodide_py.egg-info/SOURCES.txt` & `pyodide-py-0.23.4/pyodide_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.3/setup.cfg` & `pyodide-py-0.23.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyodide-py
-version = 0.23.3
+version = 0.23.4
 author = Pyodide developers
 description = "A Python package providing core interpreter functionality for Pyodide."
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyodide/pyodide
 project_urls = 
 	Bug Tracker = https://github.com/pyodide/pyodide/issues
```

