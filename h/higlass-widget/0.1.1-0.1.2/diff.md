# Comparing `tmp/higlass_widget-0.1.1.tar.gz` & `tmp/higlass_widget-0.1.2.tar.gz`

## Comparing `higlass_widget-0.1.1.tar` & `higlass_widget-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/__init__.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/widget.js
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/widget.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/notebooks/Widget.ipynb
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/LICENSE
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/higlass_widget/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/higlass_widget/widget.js
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/higlass_widget/widget.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/notebooks/Widget.ipynb
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 higlass_widget-0.1.2/PKG-INFO
```

### Comparing `higlass_widget-0.1.1/.github/workflows/ci.yml` & `higlass_widget-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/.github/workflows/release.yml` & `higlass_widget-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/higlass_widget/widget.js` & `higlass_widget-0.1.2/higlass_widget/widget.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -30,17 +30,17 @@
 
     if (viewconf.views.length === 1) {
         api.on("location", (loc) => {
             model.set("location", toPts(loc));
             model.save_changes();
         }, viewconf.views[0].uid);
     } else {
-        viewconf.views.forEach((_view, idx) => {
+        viewconf.views.forEach((view, idx) => {
             api.on("location", (loc) => {
                 let copy = model.get("location").slice();
                 copy[idx] = toPts(loc);
                 model.set("location", copy);
                 model.save_changes();
-            }, uid);
+            }, view.uid);
         });
     }
 }
```

### Comparing `higlass_widget-0.1.1/higlass_widget/widget.py` & `higlass_widget-0.1.2/higlass_widget/widget.py`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/notebooks/Widget.ipynb` & `higlass_widget-0.1.2/notebooks/Widget.ipynb`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/LICENSE` & `higlass_widget-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/README.md` & `higlass_widget-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/pyproject.toml` & `higlass_widget-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.1/PKG-INFO` & `higlass_widget-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: higlass-widget
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jupyter Widget for HiGlass
 Project-URL: homepage, https://github.com/higlass/higlass-widget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: anywidget>=0.6
```

