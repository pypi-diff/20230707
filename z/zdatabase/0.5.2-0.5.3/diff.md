# Comparing `tmp/zdatabase-0.5.2.tar.gz` & `tmp/zdatabase-0.5.3.tar.gz`

## Comparing `zdatabase-0.5.2.tar` & `zdatabase-0.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/model.py
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 zdatabase-0.5.2/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.2/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.3/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.3/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 zdatabase-0.5.3/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.3/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.3/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 zdatabase-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 zdatabase-0.5.3/PKG-INFO
```

### Comparing `zdatabase-0.5.2/src/zdatabase/__init__.py` & `zdatabase-0.5.3/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.2/src/zdatabase/model.py` & `zdatabase-0.5.3/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.2/src/zdatabase/utility.py` & `zdatabase-0.5.3/src/zdatabase/utility.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.2/LICENSE` & `zdatabase-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.2/pyproject.toml` & `zdatabase-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "flask_sqlalchemy==2.5.1",
+  "sqlalchemy==1.4.39",
   "jsonschema==4.17.3",
   "inspirare"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `zdatabase-0.5.2/PKG-INFO` & `zdatabase-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.2
+Version: 0.5.3
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: flask-sqlalchemy==2.5.1
 Requires-Dist: inspirare
 Requires-Dist: jsonschema==4.17.3
+Requires-Dist: sqlalchemy==1.4.39
 Description-Content-Type: text/markdown
 
 # zdb
 
 Zen database library.
```

