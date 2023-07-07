# Comparing `tmp/newspy-1.2.0.tar.gz` & `tmp/newspy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newspy-1.2.0.tar", max compression
+gzip compressed data, was "newspy-1.2.1.tar", max compression
```

## Comparing `newspy-1.2.0.tar` & `newspy-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2023-04-08 09:15:34.021134 newspy-1.2.0/LICENSE
--rw-r--r--   0        0        0     1064 2023-04-08 09:15:34.021134 newspy-1.2.0/README.md
--rw-r--r--   0        0        0       41 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/__init__.py
--rw-r--r--   0        0        0      506 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/client.py
--rw-r--r--   0        0        0     1762 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/models.py
--rw-r--r--   0        0        0        0 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/newsorg/__init__.py
--rw-r--r--   0        0        0     3574 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/newsorg/client.py
--rw-r--r--   0        0        0     2154 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/newsorg/models.py
--rw-r--r--   0        0        0        0 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/rss/__init__.py
--rw-r--r--   0        0        0      207 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/rss/client.py
--rw-r--r--   0        0        0     1259 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/rss/models.py
--rw-r--r--   0        0        0        0 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/shared/__init__.py
--rw-r--r--   0        0        0      817 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/shared/exceptions.py
--rw-r--r--   0        0        0     5241 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/shared/http_client.py
--rw-r--r--   0        0        0      894 2023-04-08 09:15:34.021134 newspy-1.2.0/newspy/shared/utils.py
--rw-r--r--   0        0        0      769 2023-04-08 09:16:02.133586 newspy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 newspy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-07 06:14:46.680868 newspy-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1064 2023-07-07 06:14:46.680868 newspy-1.2.1/README.md
+-rw-r--r--   0        0        0       41 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/__init__.py
+-rw-r--r--   0        0        0      613 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/client.py
+-rw-r--r--   0        0        0     1762 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/models.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/newsorg/__init__.py
+-rw-r--r--   0        0        0     3574 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/newsorg/client.py
+-rw-r--r--   0        0        0     2154 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/newsorg/models.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/rss/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/rss/client.py
+-rw-r--r--   0        0        0     1259 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/rss/models.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/shared/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/shared/exceptions.py
+-rw-r--r--   0        0        0     5241 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/shared/http_client.py
+-rw-r--r--   0        0        0      894 2023-07-07 06:14:46.680868 newspy-1.2.1/newspy/shared/utils.py
+-rw-r--r--   0        0        0      770 2023-07-07 06:14:46.680868 newspy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 newspy-1.2.1/PKG-INFO
```

### Comparing `newspy-1.2.0/LICENSE` & `newspy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/README.md` & `newspy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/models.py` & `newspy-1.2.1/newspy/models.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/newsorg/client.py` & `newspy-1.2.1/newspy/newsorg/client.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/newsorg/models.py` & `newspy-1.2.1/newspy/newsorg/models.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/rss/models.py` & `newspy-1.2.1/newspy/rss/models.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/shared/exceptions.py` & `newspy-1.2.1/newspy/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/shared/http_client.py` & `newspy-1.2.1/newspy/shared/http_client.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/newspy/shared/utils.py` & `newspy-1.2.1/newspy/shared/utils.py`

 * *Files identical despite different names*

### Comparing `newspy-1.2.0/pyproject.toml` & `newspy-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "newspy"
-version = "1.2.0"
+version = "v1.2.1"
 description = "The news client written in Python that fetches and curates the world news across the web."
 authors = ["Sechaba Mofokeng <sechaba@onemoola.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/onemoola/newspy"
 repository = "https://github.com/onemoola/newspy"
 documentation = "https://github.com/onemoola/newspy#readme"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/onemoola/newspy/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-requests = "2.28.2"
+requests = "2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.1.0"
-pre-commit = "3.2.1"
-pytest = "7.2.2"
-pytest-cov = "4.0.0"
+black = "23.3.0"
+pre-commit = "3.3.3"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
 responses = "0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `newspy-1.2.0/PKG-INFO` & `newspy-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: newspy
-Version: 1.2.0
+Version: 1.2.1
 Summary: The news client written in Python that fetches and curates the world news across the web.
 Home-page: https://github.com/onemoola/newspy
 License: MIT
 Author: Sechaba Mofokeng
 Author-email: sechaba@onemoola.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Bug Tracker, https://github.com/onemoola/newspy/issues
 Project-URL: Documentation, https://github.com/onemoola/newspy#readme
 Project-URL: Repository, https://github.com/onemoola/newspy
 Description-Content-Type: text/markdown
 
 # Newspy
```

