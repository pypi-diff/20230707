# Comparing `tmp/gradio_test_client_pypi-48.0.0.tar.gz` & `tmp/gradio_test_client_pypi-48.0.1.tar.gz`

## Comparing `gradio_test_client_pypi-48.0.0.tar` & `gradio_test_client_pypi-48.0.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/README.md
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/requirements.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/version.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/.gitignore
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/pyproject.toml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/README.md
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/requirements.txt
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/gradio-test-client-pypi/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/gradio-test-client-pypi/package.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/gradio-test-client-pypi/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/gradio-test-client-pypi/version.txt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/.gitignore
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gradio_test_client_pypi-48.0.1/PKG-INFO
```

### Comparing `gradio_test_client_pypi-48.0.0/pyproject.toml` & `gradio_test_client_pypi-48.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -34,34 +34,33 @@
   'Topic :: Software Development :: User Interfaces',
 ]
 
 [project.urls]
 Homepage = "https://github.com/gradio-app/gradio"
 
 [tool.hatch.version]
-path = "version.txt"
+path = "gradio-test-client-pypi/version.txt"
 pattern = "(?P<version>.+)"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 filename = "requirements.txt"
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 fragments = [
   { path = "README.md" },
 ]
 
 [tool.hatch.build.targets.sdist]
 include = [
-  "/gradio_client",
+  "/gradio-test-client-pypi",
   "/README.md",
   "/requirements.txt",
-  "version.txt",
 ]
 
 [tool.ruff]
 extend = "../../pyproject.toml"
 
 [tool.ruff.isort]
 known-first-party = [
-  "gradio_client"
+  "gradio-test-client-pypi"
 ]
```

### Comparing `gradio_test_client_pypi-48.0.0/PKG-INFO` & `gradio_test_client_pypi-48.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio-test-client-pypi
-Version: 48.0.0
+Version: 48.0.1
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

