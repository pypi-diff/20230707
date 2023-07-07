# Comparing `tmp/histcmp-0.6.0.tar.gz` & `tmp/histcmp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcmp-0.6.0.tar", max compression
+gzip compressed data, was "histcmp-0.6.1.tar", max compression
```

## Comparing `histcmp-0.6.0.tar` & `histcmp-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      771 2023-07-07 07:04:14.562865 histcmp-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:18:44.246598 histcmp-0.6.0/src/histcmp/__init__.py
--rw-r--r--   0        0        0    13656 2023-06-30 09:18:44.246755 histcmp-0.6.0/src/histcmp/checks.py
--rw-r--r--   0        0        0     6167 2023-06-30 09:18:44.246865 histcmp-0.6.0/src/histcmp/cli.py
--rw-r--r--   0        0        0    10682 2023-06-30 09:18:44.247012 histcmp-0.6.0/src/histcmp/compare.py
--rw-r--r--   0        0        0      500 2023-06-30 09:18:44.247080 histcmp-0.6.0/src/histcmp/config.py
--rw-r--r--   0        0        0      726 2023-06-30 09:18:44.247146 histcmp-0.6.0/src/histcmp/console.py
--rw-r--r--   0        0        0      186 2023-06-30 09:18:44.247219 histcmp-0.6.0/src/histcmp/github.py
--rw-r--r--   0        0        0      117 2023-06-30 09:18:44.247287 histcmp-0.6.0/src/histcmp/icons.py
--rw-r--r--   0        0        0     4949 2023-06-30 09:18:44.247371 histcmp-0.6.0/src/histcmp/plot.py
--rw-r--r--   0        0        0     3773 2023-06-30 09:18:44.247444 histcmp-0.6.0/src/histcmp/report.py
--rw-r--r--   0        0        0     5791 2023-06-30 09:18:44.247521 histcmp-0.6.0/src/histcmp/root_helpers.py
--rw-r--r--   0        0        0      878 2023-06-30 09:18:44.247624 histcmp-0.6.0/src/histcmp/static/alpinejs.intersect.min.js
--rw-r--r--   0        0        0    37696 2023-06-30 09:18:44.247838 histcmp-0.6.0/src/histcmp/static/alpinejs.min.js
--rw-r--r--   0        0        0   244777 2023-06-30 09:18:44.248465 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.css
--rw-r--r--   0        0        0    98265 2023-06-30 09:18:44.248906 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.css.map
--rw-r--r--   0        0        0   206763 2023-06-30 09:18:44.249377 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.min.css
--rw-r--r--   0        0        0   244630 2023-06-30 09:18:44.249966 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.css
--rw-r--r--   0        0        0    98250 2023-06-30 09:18:44.250404 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.css.map
--rw-r--r--   0        0        0   206620 2023-06-30 09:18:44.250953 histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.min.css
--rw-r--r--   0        0        0      315 2023-06-30 09:18:44.251025 histcmp-0.6.0/src/histcmp/static/css/main.css
--rw-r--r--   0        0        0     2088 2023-06-30 09:18:44.251134 histcmp-0.6.0/src/histcmp/templates/base.html.j2
--rw-r--r--   0        0        0     2399 2023-06-30 09:18:44.251228 histcmp-0.6.0/src/histcmp/templates/main.html.j2
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 histcmp-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-07-07 07:39:51.878310 histcmp-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:18:44.246598 histcmp-0.6.1/src/histcmp/__init__.py
+-rw-r--r--   0        0        0    13656 2023-06-30 09:18:44.246755 histcmp-0.6.1/src/histcmp/checks.py
+-rw-r--r--   0        0        0     6167 2023-06-30 09:18:44.246865 histcmp-0.6.1/src/histcmp/cli.py
+-rw-r--r--   0        0        0    10682 2023-06-30 09:18:44.247012 histcmp-0.6.1/src/histcmp/compare.py
+-rw-r--r--   0        0        0      500 2023-06-30 09:18:44.247080 histcmp-0.6.1/src/histcmp/config.py
+-rw-r--r--   0        0        0      726 2023-06-30 09:18:44.247146 histcmp-0.6.1/src/histcmp/console.py
+-rw-r--r--   0        0        0      186 2023-06-30 09:18:44.247219 histcmp-0.6.1/src/histcmp/github.py
+-rw-r--r--   0        0        0      117 2023-06-30 09:18:44.247287 histcmp-0.6.1/src/histcmp/icons.py
+-rw-r--r--   0        0        0     4949 2023-06-30 09:18:44.247371 histcmp-0.6.1/src/histcmp/plot.py
+-rw-r--r--   0        0        0     3773 2023-06-30 09:18:44.247444 histcmp-0.6.1/src/histcmp/report.py
+-rw-r--r--   0        0        0     5791 2023-06-30 09:18:44.247521 histcmp-0.6.1/src/histcmp/root_helpers.py
+-rw-r--r--   0        0        0      878 2023-06-30 09:18:44.247624 histcmp-0.6.1/src/histcmp/static/alpinejs.intersect.min.js
+-rw-r--r--   0        0        0    37696 2023-06-30 09:18:44.247838 histcmp-0.6.1/src/histcmp/static/alpinejs.min.js
+-rw-r--r--   0        0        0   244777 2023-06-30 09:18:44.248465 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.css
+-rw-r--r--   0        0        0    98265 2023-06-30 09:18:44.248906 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.css.map
+-rw-r--r--   0        0        0   206763 2023-06-30 09:18:44.249377 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.min.css
+-rw-r--r--   0        0        0   244630 2023-06-30 09:18:44.249966 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.css
+-rw-r--r--   0        0        0    98250 2023-06-30 09:18:44.250404 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.css.map
+-rw-r--r--   0        0        0   206620 2023-06-30 09:18:44.250953 histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.min.css
+-rw-r--r--   0        0        0      315 2023-06-30 09:18:44.251025 histcmp-0.6.1/src/histcmp/static/css/main.css
+-rw-r--r--   0        0        0     2088 2023-06-30 09:18:44.251134 histcmp-0.6.1/src/histcmp/templates/base.html.j2
+-rw-r--r--   0        0        0     2399 2023-06-30 09:18:44.251228 histcmp-0.6.1/src/histcmp/templates/main.html.j2
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 histcmp-0.6.1/PKG-INFO
```

### Comparing `histcmp-0.6.0/pyproject.toml` & `histcmp-0.6.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "histcmp"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "histcmp", from = "src" },
 ]
 
 [tool.poetry.scripts]
 histcmp = 'histcmp.cli:app'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-typer = "^0.4.0"
+typer = "^0.9.0"
 wasabi = "^0.9.0"
 rich = "^11.0.0"
 numpy = "^1.23.2"
 Jinja2 = "^3.0.3"
 requests = "^2.27.1"
 matplotlib = "^3.5.1"
 hist = {extras = ["plot"], version = "^2.6.0"}
```

### Comparing `histcmp-0.6.0/src/histcmp/checks.py` & `histcmp-0.6.1/src/histcmp/checks.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/cli.py` & `histcmp-0.6.1/src/histcmp/cli.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/compare.py` & `histcmp-0.6.1/src/histcmp/compare.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/console.py` & `histcmp-0.6.1/src/histcmp/console.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/plot.py` & `histcmp-0.6.1/src/histcmp/plot.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/report.py` & `histcmp-0.6.1/src/histcmp/report.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/root_helpers.py` & `histcmp-0.6.1/src/histcmp/root_helpers.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/alpinejs.intersect.min.js` & `histcmp-0.6.1/src/histcmp/static/alpinejs.intersect.min.js`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/alpinejs.min.js` & `histcmp-0.6.1/src/histcmp/static/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.css` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.css.map` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.css.map`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma-rtl.min.css` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma-rtl.min.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.css` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.css.map` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.css.map`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/static/css/bulma/bulma.min.css` & `histcmp-0.6.1/src/histcmp/static/css/bulma/bulma.min.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/templates/base.html.j2` & `histcmp-0.6.1/src/histcmp/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/src/histcmp/templates/main.html.j2` & `histcmp-0.6.1/src/histcmp/templates/main.html.j2`

 * *Files identical despite different names*

### Comparing `histcmp-0.6.0/PKG-INFO` & `histcmp-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcmp
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,9 +19,9 @@
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: mplhep (>=0.3.26,<0.4.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=11.0.0,<12.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
-Requires-Dist: typer (>=0.4.0,<0.5.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: wasabi (>=0.9.0,<0.10.0)
```

