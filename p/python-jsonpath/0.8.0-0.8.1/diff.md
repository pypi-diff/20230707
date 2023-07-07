# Comparing `tmp/python_jsonpath-0.8.0.tar.gz` & `tmp/python_jsonpath-0.8.1.tar.gz`

## Comparing `python_jsonpath-0.8.0.tar` & `python_jsonpath-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/__about__.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/__init__.py
--rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/env.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/exceptions.py
--rw-r--r--   0        0        0    19524 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/filter.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/lex.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/match.py
--rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/parse.py
--rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/patch.py
--rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/path.py
--rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/pointer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/py.typed
--rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/stream.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/token.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/count.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/is_instance.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/typeof.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/README.md
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/__about__.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/__init__.py
+-rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/env.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    19524 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/lex.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/match.py
+-rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/parse.py
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/patch.py
+-rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/path.py
+-rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/pointer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/py.typed
+-rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/stream.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/README.md
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/PKG-INFO
```

### Comparing `python_jsonpath-0.8.0/jsonpath/__init__.py` & `python_jsonpath-0.8.1/jsonpath/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/env.py` & `python_jsonpath-0.8.1/jsonpath/env.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/exceptions.py` & `python_jsonpath-0.8.1/jsonpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/filter.py` & `python_jsonpath-0.8.1/jsonpath/filter.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/lex.py` & `python_jsonpath-0.8.1/jsonpath/lex.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/match.py` & `python_jsonpath-0.8.1/jsonpath/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/parse.py` & `python_jsonpath-0.8.1/jsonpath/parse.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/patch.py` & `python_jsonpath-0.8.1/jsonpath/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,17 +511,17 @@
         self,
         data: Union[str, IOBase, MutableSequence[object], MutableMapping[str, object]],
     ) -> Union[MutableSequence[object], MutableMapping[str, object]]:
         """Apply all operations from this patch to _data_.
 
         If _data_ is a string or file-like object, it will be loaded with
         _json.loads_. Otherwise _data_ should be a JSON-like data structure and
-        will be modified in-place.
+        will be modified in place.
 
-        When modifying _data_ in-place, we return modified data too. This is
+        When modifying _data_ in place, we return modified data too. This is
         to allow for replacing _data's_ root element, which is allowed by some
         patch operations.
 
         Arguments:
             data: The target JSON "document" or equivalent Python objects.
 
         Returns:
```

### Comparing `python_jsonpath-0.8.0/jsonpath/path.py` & `python_jsonpath-0.8.1/jsonpath/path.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/pointer.py` & `python_jsonpath-0.8.1/jsonpath/pointer.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,19 +228,24 @@
     @classmethod
     def from_match(
         cls,
         match: JSONPathMatch,
     ) -> JSONPointer:
         """Return a JSON Pointer for the path from a JSONPathMatch instance."""
         # A rfc6901 string representation of match.parts.
-        return cls(
-            "/"
-            + "/".join(
+        if not match.parts:
+            # This should not happen, unless the JSONPathMatch has been tampered with.
+            pointer = ""
+        else:
+            pointer = "/" + "/".join(
                 str(p).replace("~", "~0").replace("/", "~1") for p in match.parts
-            ),
+            )
+
+        return cls(
+            pointer,
             parts=match.parts,
             unicode_escape=False,
             uri_decode=False,
         )
 
     @classmethod
     def from_parts(
@@ -265,17 +270,26 @@
         if unicode_escape:
             _parts = (
                 codecs.decode(p.replace("\\/", "/"), "unicode-escape")
                 .encode("utf-16", "surrogatepass")
                 .decode("utf-16")
                 for p in _parts
             )
+
         __parts = tuple(_parts)
+
+        if __parts:
+            pointer = "/" + "/".join(
+                p.replace("~", "~0").replace("/", "~1") for p in __parts
+            )
+        else:
+            pointer = ""
+
         return cls(
-            "/" + "/".join(p.replace("~", "~0").replace("/", "~1") for p in __parts),
+            pointer,
             parts=__parts,
             unicode_escape=False,
             uri_decode=False,
         )
 
     def is_relative_to(self, other: JSONPointer) -> bool:
         """Return _True_ if this pointer points to a child of _other_."""
```

### Comparing `python_jsonpath-0.8.0/jsonpath/selectors.py` & `python_jsonpath-0.8.1/jsonpath/selectors.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/stream.py` & `python_jsonpath-0.8.1/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/token.py` & `python_jsonpath-0.8.1/jsonpath/token.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/count.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/count.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/is_instance.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/is_instance.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/match.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/search.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/search.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/jsonpath/function_extensions/typeof.py` & `python_jsonpath-0.8.1/jsonpath/function_extensions/typeof.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/.gitignore` & `python_jsonpath-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/LICENSE.txt` & `python_jsonpath-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/README.md` & `python_jsonpath-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/pyproject.toml` & `python_jsonpath-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.0/PKG-INFO` & `python_jsonpath-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jsonpath
-Version: 0.8.0
+Version: 0.8.1
 Summary: Another JSONPath implementation for Python.
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-jsonpath Version: 0.8.0 Summary: Another
+Metadata-Version: 2.1 Name: python-jsonpath Version: 0.8.1 Summary: Another
 JSONPath implementation for Python. Project-URL: Documentation, https://jg-
 rp.github.io/python-jsonpath/ Project-URL: Issues, https://github.com/jg-rp/
 python-jsonpath/issues Project-URL: Source, https://github.com/jg-rp/python-
 jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

