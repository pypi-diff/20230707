# Comparing `tmp/catencfamily-0.0.86.tar.gz` & `tmp/catencfamily-0.0.87.tar.gz`

## Comparing `catencfamily-0.0.86.tar` & `catencfamily-0.0.87.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89935 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 catencfamily-0.0.86/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.86/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.86/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.86/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.86/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89962 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.87/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.87/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.87/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.87/PKG-INFO
```

### Comparing `catencfamily-0.0.86/src/catencfamily/encoders.py` & `catencfamily-0.0.87/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 5th July, 2023
+# 7th July, 2023
 """
 References:
 Coding standard:
     https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
     
 Developing sklearn estimators:
     https://scikit-learn.org/stable/developers/develop.html 
@@ -1785,19 +1785,19 @@
             # has cat col as index, but sorted.
             #-----
             # Expt:29th June, 2023
             r = t.copy()
             r['target'] = target
             #-----
             yu = list(r[key])
-            r = r.groupby(by = yu, sort = True).mean()
+            # First column is key. Can be integer or category
+            r = r.iloc[:,1:].groupby(by = yu, sort = True).mean()
             #r = r.groupby(by = [key], sort = True).mean()
             # Get also index ('app') as one of the columns
-            # commencted out on 7th July, 2023
-            #r.reset_index(inplace = True)
+            r.reset_index(inplace = True)
             r=r.rename(columns = {'index' : key})
             if take_mean:
                 # Our vector dataframe is now ready
                 vec[key] = r
             else:
                 vec[key] = t
                 # Add target col also
@@ -2124,8 +2124,8 @@
                 ax.title.set_size(20)  # title font size
                 ax.title.set_weight('bold')
                 pos = nx.spring_layout(G, k = k)
                 nx.draw_networkx(G,pos = pos, node_size=30, with_labels =  withLabels, font_size=fontSize, node_color = 'r', ax =ax)
         return
     
  ###############333##################               
-       
+
```

### Comparing `catencfamily-0.0.86/src/catencfamily/utils.py` & `catencfamily-0.0.87/src/catencfamily/utils.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.86/LICENSE` & `catencfamily-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.86/README.md` & `catencfamily-0.0.87/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.86/pyproject.toml` & `catencfamily-0.0.87/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.86"
+version = "0.0.87"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.86/PKG-INFO` & `catencfamily-0.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.86
+Version: 0.0.87
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

