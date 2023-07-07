# Comparing `tmp/catencfamily-0.0.85.tar.gz` & `tmp/catencfamily-0.0.86.tar.gz`

## Comparing `catencfamily-0.0.85.tar` & `catencfamily-0.0.86.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.85/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89886 2020-02-02 00:00:00.000000 catencfamily-0.0.85/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 catencfamily-0.0.85/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.85/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.85/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.85/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.85/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89935 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.86/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.86/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.86/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.86/PKG-INFO
```

### Comparing `catencfamily-0.0.85/src/catencfamily/encoders.py` & `catencfamily-0.0.86/src/catencfamily/encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1788,15 +1788,16 @@
             r = t.copy()
             r['target'] = target
             #-----
             yu = list(r[key])
             r = r.groupby(by = yu, sort = True).mean()
             #r = r.groupby(by = [key], sort = True).mean()
             # Get also index ('app') as one of the columns
-            r.reset_index(inplace = True)
+            # commencted out on 7th July, 2023
+            #r.reset_index(inplace = True)
             r=r.rename(columns = {'index' : key})
             if take_mean:
                 # Our vector dataframe is now ready
                 vec[key] = r
             else:
                 vec[key] = t
                 # Add target col also
```

### Comparing `catencfamily-0.0.85/src/catencfamily/utils.py` & `catencfamily-0.0.86/src/catencfamily/utils.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.85/LICENSE` & `catencfamily-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.85/README.md` & `catencfamily-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.85/pyproject.toml` & `catencfamily-0.0.86/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.85"
+version = "0.0.86"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.85/PKG-INFO` & `catencfamily-0.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.85
+Version: 0.0.86
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

