# Comparing `tmp/up_paraspace-0.0.5.tar.gz` & `tmp/up_paraspace-0.0.6.tar.gz`

## Comparing `up_paraspace-0.0.5.tar` & `up_paraspace-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/src/up_paraspace/__about__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/src/up_paraspace/__init__.py
--rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/src/up_paraspace/up_paraspace.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 up_paraspace-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/src/up_paraspace/__about__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/src/up_paraspace/__init__.py
+-rw-r--r--   0        0        0    14642 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/src/up_paraspace/up_paraspace.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 up_paraspace-0.0.6/PKG-INFO
```

### Comparing `up_paraspace-0.0.5/src/up_paraspace/up_paraspace.py` & `up_paraspace-0.0.6/src/up_paraspace/up_paraspace.py`

 * *Files identical despite different names*

### Comparing `up_paraspace-0.0.5/LICENSE.txt` & `up_paraspace-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `up_paraspace-0.0.5/README.md` & `up_paraspace-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pip install unified-planning up-paraspace
 ```
 
 ## Usage
 
 ```
 from unified_planning.shortcuts import *
-import up-paraspace
+import up_paraspace
 
 problem = Problem('myproblem')
 # specify the problem (e.g. fluents, initial state, actions, goal)
 ...
 
 planner = OneshotPlanner(name="paraspace")
 result = planner.solve(problem)
```

### Comparing `up_paraspace-0.0.5/pyproject.toml` & `up_paraspace-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `up_paraspace-0.0.5/PKG-INFO` & `up_paraspace-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-paraspace
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/luteberget/up-paraspace#readme
 Project-URL: Issues, https://github.com/luteberget/up-paraspace/issues
 Project-URL: Source, https://github.com/luteberget/up-paraspace
 Author-email: Bjørnar Luteberget <bjornar.luteberget@sintef.no>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 pip install unified-planning up-paraspace
 ```
 
 ## Usage
 
 ```
 from unified_planning.shortcuts import *
-import up-paraspace
+import up_paraspace
 
 problem = Problem('myproblem')
 # specify the problem (e.g. fluents, initial state, actions, goal)
 ...
 
 planner = OneshotPlanner(name="paraspace")
 result = planner.solve(problem)
```

