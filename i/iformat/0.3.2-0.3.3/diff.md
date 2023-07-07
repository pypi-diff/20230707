# Comparing `tmp/iformat-0.3.2.tar.gz` & `tmp/iformat-0.3.3.tar.gz`

## Comparing `iformat-0.3.2.tar` & `iformat-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.3.2/setup.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 iformat-0.3.2/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.3.2/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.3.2/LICENSE
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 iformat-0.3.2/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 iformat-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 iformat-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.3.3/setup.py
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 iformat-0.3.3/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.3.3/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 iformat-0.3.3/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 iformat-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 iformat-0.3.3/PKG-INFO
```

### Comparing `iformat-0.3.2/src/iformat/__init__.py` & `iformat-0.3.3/src/iformat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 def _isfunctionish(i):
     return _if(i) or _ib(i) or _im(i)
 
 def iformat(i, indentLevel = 0, indentDepth = 4, expansionThreshold = 0, excludedAttrs = r"__.+__"):
     il, id, et, ea = indentLevel, indentDepth, expansionThreshold, excludedAttrs
     length = _length(i)
     if type(i) in _iters:
-        return (_brackets(type(i), True if length > et else False, ((il + 1) * id) if length > et else False)[0]\
-            + ((",\n" + _indent(il + 1, id)) if length > et else (", ")).join(\
+        return (_brackets(type(i), True if length > et and len(i) > 0 else False, ((il + 1) * id) if length > et and len(i) > 0 else False)[0]\
+            + ((",\n" + _indent(il + 1, id)) if length > et and len(i) > 0 else (", ")).join(\
                     [f"{iformat(k, il + 1, id, et, ea)}: {iformat(v, il + 1, id, et, ea)}" for k, v in i.items()]\
                 if type(i) == dict else\
                     [iformat(x, il + 1, id, et, ea) for x in i])\
-            + _brackets(type(i), True if length > et else False, (il * id) if length > et else 0)[-1])
+            + _brackets(type(i), True if length > et and len(i) > 0 else False, (il * id) if length > et else 0)[-1])
     if _isfunctionish(i):
         return f"<function {i.__name__}>"
     if "iformat" in dir(i):
         return i.iformat(il, id, et, ea)
     if hasattr(i, "__dict__"):
         return (f"{icn if (icn := i.__class__.__name__) != 'type' else i.__name__}({', '.join([f'{k} = {iformat(v, il, id, et, ea)}' for k, v in i.__dict__.items() if (k not in ea if type(ea) in _iters[1:] else not _match(ea, k))])})")
     return str(i)
```

### Comparing `iformat-0.3.2/.gitignore` & `iformat-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.3.2/LICENSE` & `iformat-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.3.2/README.md` & `iformat-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #   1,
 #   2,
 #   3
 # ]
 ```
 
 **`excludedAttrs`**: *(`iprint` and `iformat`)*\
-Specifies class attributes that should not be printed. Should be a list or tuple of strings OR a regex pattern. Default `r"__.+__"`
+Specifies class attributes that should not be printed. Should be a list or tuple of strings OR a regex pattern. Default `r"__.+__"`.
 
 ## `.iformat` method for classes:
 You can add a `.iformat` method to any class to show the return value of that method instead of the default iformat output for classes. It must accept positional arguments `indentLevel`, `indentDepth`, `expansionThreshold`, and `excludedAttrs`, which will be passed the same values as those passed to the `iformat` function call that calls the method. It is reccomended that you add whitespace in front of the output corresponding to `indentLevel * indentDepth`, and that you call `iformat`, with the same passed args (maybe with `indentDepth + 1`) on any values that are part of the outputted string.
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
```

### Comparing `iformat-0.3.2/pyproject.toml` & `iformat-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.3.2/PKG-INFO` & `iformat-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.3.2
+Version: 0.3.3
 Summary: Indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 #   1,
 #   2,
 #   3
 # ]
 ```
 
 **`excludedAttrs`**: *(`iprint` and `iformat`)*\
-Specifies class attributes that should not be printed. Should be a list or tuple of strings OR a regex pattern. Default `r"__.+__"`
+Specifies class attributes that should not be printed. Should be a list or tuple of strings OR a regex pattern. Default `r"__.+__"`.
 
 ## `.iformat` method for classes:
 You can add a `.iformat` method to any class to show the return value of that method instead of the default iformat output for classes. It must accept positional arguments `indentLevel`, `indentDepth`, `expansionThreshold`, and `excludedAttrs`, which will be passed the same values as those passed to the `iformat` function call that calls the method. It is reccomended that you add whitespace in front of the output corresponding to `indentLevel * indentDepth`, and that you call `iformat`, with the same passed args (maybe with `indentDepth + 1`) on any values that are part of the outputted string.
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
```

