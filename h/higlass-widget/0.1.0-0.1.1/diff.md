# Comparing `tmp/higlass_widget-0.1.0.tar.gz` & `tmp/higlass_widget-0.1.1.tar.gz`

## Comparing `higlass_widget-0.1.0.tar` & `higlass_widget-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/__init__.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/widget.js
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/widget.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/notebooks/Widget.ipynb
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/LICENSE
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/widget.js
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/higlass_widget/widget.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/notebooks/Widget.ipynb
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 higlass_widget-0.1.1/PKG-INFO
```

### Comparing `higlass_widget-0.1.0/.github/workflows/ci.yml` & `higlass_widget-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/.github/workflows/release.yml` & `higlass_widget-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/higlass_widget/widget.js` & `higlass_widget-0.1.1/higlass_widget/widget.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -11,33 +11,36 @@
     yDomain
 }) {
     let [x, xe] = xDomain;
     let [y, ye] = yDomain;
     return [x, xe, y, ye];
 }
 
-export async function render(view) {
-    let viewconf = JSON.parse(view.model.get("_viewconf"));
-    let api = await hglib.viewer(view.el, viewconf);
+export async function render({
+    model,
+    el
+}) {
+    let viewconf = JSON.parse(model.get("_viewconf"));
+    let api = await hglib.viewer(el, viewconf);
 
-    view.model.on("msg:custom", (msg) => {
+    model.on("msg:custom", (msg) => {
         msg = JSON.parse(msg);
         let [fn, ...args] = msg;
         api[fn](...args);
     });
 
     if (viewconf.views.length === 1) {
         api.on("location", (loc) => {
-            view.model.set("location", toPts(loc));
-            view.model.save_changes();
+            model.set("location", toPts(loc));
+            model.save_changes();
         }, viewconf.views[0].uid);
     } else {
-        viewconf.views.forEach((view, idx) => {
+        viewconf.views.forEach((_view, idx) => {
             api.on("location", (loc) => {
-                let copy = view.model.get("location").slice();
+                let copy = model.get("location").slice();
                 copy[idx] = toPts(loc);
-                view.model.set("location", copy);
-                view.model.save_changes();
-            }, view.uid);
+                model.set("location", copy);
+                model.save_changes();
+            }, uid);
         });
     }
 }
```

### Comparing `higlass_widget-0.1.0/higlass_widget/widget.py` & `higlass_widget-0.1.1/higlass_widget/widget.py`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/notebooks/Widget.ipynb` & `higlass_widget-0.1.1/notebooks/Widget.ipynb`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/LICENSE` & `higlass_widget-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/README.md` & `higlass_widget-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `higlass_widget-0.1.0/pyproject.toml` & `higlass_widget-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     { name = "Trevor Manz", email = "trevor.j.manz@gmail.com" },
 ]
 license = { text = "MIT" }
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "anywidget",
+    "anywidget>=0.6",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black[jupyter]",
     "ruff",
     "jupyterlab",
```

### Comparing `higlass_widget-0.1.0/PKG-INFO` & `higlass_widget-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: higlass-widget
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jupyter Widget for HiGlass
 Project-URL: homepage, https://github.com/higlass/higlass-widget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
-Requires-Dist: anywidget
+Requires-Dist: anywidget>=0.6
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Description-Content-Type: text/markdown
```

