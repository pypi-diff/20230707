# Comparing `tmp/saxonche_stubs-0.5.0.tar.gz` & `tmp/saxonche_stubs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saxonche_stubs-0.5.0.tar", max compression
+gzip compressed data, was "saxonche_stubs-0.6.0.tar", max compression
```

## Comparing `saxonche_stubs-0.5.0.tar` & `saxonche_stubs-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.5.0/README.md
--rw-r--r--   0        0        0     1572 2023-05-16 17:34:34.747572 saxonche_stubs-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11580 2023-05-16 17:33:26.788581 saxonche_stubs-0.5.0/saxonche-stubs/__init__.pyi
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.5.0/setup.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.6.0/README.md
+-rw-r--r--   0        0        0     1572 2023-07-07 13:11:40.217582 saxonche_stubs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13094 2023-07-07 13:10:53.082080 saxonche_stubs-0.6.0/saxonche-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.6.0/setup.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.6.0/PKG-INFO
```

### Comparing `saxonche_stubs-0.5.0/pyproject.toml` & `saxonche_stubs-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saxonche-stubs"
-version = "0.5.0"
+version = "0.6.0"
 description = "Type stubs for saxonche"
 authors = ["Bpolitycki <bastian.politycki@unisg.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "saxonche-stubs"}]
 
 classifiers = [
```

### Comparing `saxonche_stubs-0.5.0/saxonche-stubs/__init__.pyi` & `saxonche_stubs-0.6.0/saxonche-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,44 @@
     def exception_occurred(self) -> bool:
         """Check whether an exception has been raised internally within Saxon/C.
 
         Returns:
             bool: True if an exception has been raised, False otherwise
         """
         ...
+    def make_boolean_value(self, value: bool) -> PyXdmAtomicValue:
+        """Create an XdmValue from a boolean.
+
+        Args:
+            value (bool): The boolean value
+
+        Returns:
+            PyXdmAtomicValue: The XdmAtomicValue representing the boolean value.
+        """
+        ...
+    def make_integer_value(self, value: int) -> PyXdmAtomicValue:
+        """Create Int64Value or a BigIntegerValue from an integer.
+
+        Args:
+            value (int): The integer value
+
+        Returns:
+            PyXdmAtomicValue: The XdmAtomicValue representing the integer value.
+        """
+        ...
+    def make_string_value(self, str_: str) -> PyXdmAtomicValue:
+        """Create an XdmValue from a string.
+
+        Args:
+            str_ (str): The string value. NULL is taken as equivalent to "".
+
+        Returns:
+            PyXdmAtomicValue: The XdmAtomicValue representing the string value.
+        """
+        ...
     def new_xpath_processor(self) -> PyXPathProcessor:
         """Creates a new XPath processor, which used to evaluate XPath expressions."""
         ...
     def new_xquery_processor(self) -> PyXQueryProcessor:
         """Creates a new XQuery processor, which used to evaluate XQuery expressions."""
         ...
     def new_xslt30_processor(self) -> PyXslt30Processor: ...
@@ -160,14 +190,29 @@
         """An PyXQueryProcessor object represents factory to compile, load and execute queries."""
     ...
 
 class PyXslt30Processor:
     def __init__(self) -> None:
         """An PyXslt30Processor represents factory to compile, load and execute a stylesheet."""
         ...
+    def clear_parameters(self) -> None:
+        """Clear all parameters that have been set"""
+        ...
+    def set_parameter(self, name: str, value: PyXdmValue) -> None:
+        """Set the value of a stylesheet parameter.
+
+        Args:
+            name (str): The name of the stylesheet parameter, as a string.
+                        For namespaced parameter use the JClark notation, that is "{uri}local".
+            value (PyXdmValue): The value of the stylesheet parameter, or None to clear a previously set value.
+
+        Returns:
+            None
+        """
+        ...
 
 class PyXdmValue:
     def __init__(self) -> None:
         """Value in the XDM data model. A value is a sequence of one or more items."""
         ...
     def __iter__(self) -> Iterator[PyXdmItem]:
         """Iterate over the items in the sequence.
```

### Comparing `saxonche_stubs-0.5.0/setup.py` & `saxonche_stubs-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['saxonche>=12.1.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'saxonche-stubs',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Type stubs for saxonche',
     'long_description': '# saxonche-stubs\n\nType stubs for the [saxonche](https://pypi.org/project/saxonche/) python package. This package has no functionality itself, but is merely an addition to the completion within IDEs. The basis for type annotations and comments is the documentation of [the Saxon Python API](https://www.saxonica.com/saxon-c/doc11/html/saxonc.html).\n\nAt the moment not all APIs are fully typed.\n\n## Author / Contact\n\n- [Bastian Politycki](https://github.com/Bpolitycki) – Swiss Law Sources\n',
     'author': 'Bpolitycki',
     'author_email': 'bastian.politycki@unisg.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `saxonche_stubs-0.5.0/PKG-INFO` & `saxonche_stubs-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saxonche-stubs
-Version: 0.5.0
+Version: 0.6.0
 Summary: Type stubs for saxonche
 License: GPL-3.0-or-later
 Author: Bpolitycki
 Author-email: bastian.politycki@unisg.ch
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

