# Comparing `tmp/up_paraspace-0.0.1.tar.gz` & `tmp/up_paraspace-0.0.2.tar.gz`

## Comparing `up_paraspace-0.0.1.tar` & `up_paraspace-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/src/up_paraspace/__about__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/src/up_paraspace/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 up_paraspace-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/src/up_paraspace/__about__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/src/up_paraspace/__init__.py
+-rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/src/up_paraspace/up_paraspace.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 up_paraspace-0.0.2/PKG-INFO
```

### Comparing `up_paraspace-0.0.1/LICENSE.txt` & `up_paraspace-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `up_paraspace-0.0.1/README.md` & `up_paraspace-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `up_paraspace-0.0.1/pyproject.toml` & `up_paraspace-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pyparaspace==0.1.5"
+  "pyparaspace==0.1.5",
+  "unified-planning~=1.0"
 ]
 
 [project.urls]
 Documentation = "https://github.com/luteberget/up-paraspace#readme"
 Issues = "https://github.com/luteberget/up-paraspace/issues"
 Source = "https://github.com/luteberget/up-paraspace"
```

### Comparing `up_paraspace-0.0.1/PKG-INFO` & `up_paraspace-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: up-paraspace
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/luteberget/up-paraspace#readme
 Project-URL: Issues, https://github.com/luteberget/up-paraspace/issues
 Project-URL: Source, https://github.com/luteberget/up-paraspace
 Author-email: Bjørnar Luteberget <bjornar.luteberget@sintef.no>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pyparaspace==0.1.5
+Requires-Dist: unified-planning~=1.0
 Description-Content-Type: text/markdown
 
 # Integration of ParaSpace with the Unified Planning Library
 
 The aim of this project is to make the
 [ParaSpace](https://github.com/luteberget/paraspace) planning engine available
 in the [unified_planning library](https://github.com/aiplan4eu/unified-planning)
```

