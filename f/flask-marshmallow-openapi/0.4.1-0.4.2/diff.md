# Comparing `tmp/flask-marshmallow-openapi-0.4.1.tar.gz` & `tmp/flask-marshmallow-openapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.4.1.tar", last modified: Sun Jul  2 16:56:55 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.4.2.tar", last modified: Fri Jul  7 06:34:57 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.4.1.tar` & `flask-marshmallow-openapi-0.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.838029 flask-marshmallow-openapi-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/flask_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/schemas_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.169074 flask-marshmallow-openapi-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-07 06:34:57.169074 flask-marshmallow-openapi-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:34:57.169074 flask-marshmallow-openapi-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.157074 flask-marshmallow-openapi-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.157074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.161074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.161074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.165074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.165074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-07 06:34:44.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:57.161074 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-07 06:34:57.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-07 06:34:57.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:34:57.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:34:56.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 06:34:57.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 06:34:57.000000 flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.4.1/.gitignore` & `flask-marshmallow-openapi-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/LICENSE` & `flask-marshmallow-openapi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/MANIFEST.in` & `flask-marshmallow-openapi-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/PKG-INFO` & `flask-marshmallow-openapi-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.4.1/README.md` & `flask-marshmallow-openapi-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/pyproject.toml` & `flask-marshmallow-openapi-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.4.1"
+version = "0.4.2"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_get.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_get.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_post.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/decorate_post.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/helpers.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/flask_paths.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/flask_paths.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/middleware.py`

 * *Files 16% similar despite different names*

```diff
@@ -117,17 +117,73 @@
             name="open_api",
             import_name=__name__,
             url_prefix="/docs",
             template_folder="./templates",
             static_folder="./static",
         )
         self.config = config
+
+        self._map_to_openapi_types = []
+        self._attribute_functions = []
+
         if app:
             self.init_app(app)
 
+    def add_map_to_openapi_types(self, data):
+        """
+        Call this as many times needed, but before calling `init_app()`.
+
+        Example:
+            class CustomInteger(Integer):
+                pass
+
+            open_api = OpenAPI(config=_open_api_conf)
+            open_api.add_map_to_openapi_types((IntegerLike, Integer,))
+
+            # ...
+
+            open_api.init_app(app)
+
+        See:
+            https://apispec.readthedocs.io/en/latest/using_plugins.html#custom-fields
+        """
+        self._map_to_openapi_types.append(data)
+
+    def add_attribute_function(self, f):
+        """
+        Call this as many times needed, but before calling `init_app()`.
+
+        Example:
+            def ULID_field2properties(self, field, **kwargs):
+                ret = {}
+                if isinstance(field, MyULIDField):
+                    ret["format"] = "ULID"
+                    ret["examples"] = [
+                        "01H4QG7F1XB3MGW7GHB5PA4P89",
+                        "01H4QG7FMQCE8DAPV6EQZREDX4",
+                        "01H4QG7VE3BY903B5DNJ442RDN",
+                        "01H4QG7XCPGCPB3BYN0QPFX61S",
+                        "01H4QG80AHN36H1X1R2FEG61V4",
+                        "01H4QG8294DFA2S9CZTBGEPCNE",
+                        "01H4QG847Q1KVSQE6F8GXKRTJH",
+                    ]
+                return ret
+
+            open_api = OpenAPI(config=_open_api_conf)
+            open_api.add_attribute_function(ULID_field2properties)
+
+            # ...
+
+            open_api.init_app(app)
+
+        See:
+            https://apispec.readthedocs.io/en/latest/using_plugins.html#custom-fields
+        """
+        self._attribute_functions.append(f)
+
     def init_app(self, app: flask.Flask):
         self._add_own_endpoints()
 
         full_url_prefix = (
             Path(self.config.mounted_at or "/") / f"./{self.blueprint.url_prefix}"
         )
 
@@ -139,17 +195,23 @@
                 if self.config.swagger_json_template_loader_kwargs:
                     initial_swagger_json = self.config.swagger_json_template_loader(
                         **self.config.swagger_json_template_loader_kwargs
                     )
                 else:
                     initial_swagger_json = self.config.swagger_json_template_loader()
 
+            ma_plugin = MarshmallowPlugin()
             self._apispec = apispec.APISpec(
-                plugins=[MarshmallowPlugin()], **(initial_swagger_json)
+                plugins=[ma_plugin], **(initial_swagger_json)
             )
+            for _ in self._map_to_openapi_types:
+                ma_plugin.map_to_openapi_type(*_)
+            for _ in self._attribute_functions:
+                ma_plugin.converter.add_attribute_function(_)
+
             for name, klass in SchemasRegistry.all_schemas().items():
                 # apispec automatically registers all nested schema so we must prevent
                 # registering them ourselves because of DuplicateSchemaError
                 x_tags = getattr(klass.opts, "x_tags", None)
 
                 try:
                     if x_tags:
```

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/schemas_registry.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.4.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

