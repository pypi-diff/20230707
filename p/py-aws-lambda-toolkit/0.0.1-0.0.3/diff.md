# Comparing `tmp/py-aws-lambda-toolkit-0.0.1.tar.gz` & `tmp/py-aws-lambda-toolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aws-lambda-toolkit-0.0.1.tar", last modified: Wed Jul  5 21:12:08 2023, max compression
+gzip compressed data, was "py-aws-lambda-toolkit-0.0.3.tar", last modified: Fri Jul  7 19:16:43 2023, max compression
```

## Comparing `py-aws-lambda-toolkit-0.0.1.tar` & `py-aws-lambda-toolkit-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:12:07.997352 py-aws-lambda-toolkit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-05 21:12:07.997352 py-aws-lambda-toolkit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:12:07.993352 py-aws-lambda-toolkit-0.0.1/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/__tests__/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:12:07.993352 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-05 21:12:07.000000 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-05 21:12:07.000000 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:12:07.000000 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-05 21:12:07.000000 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 21:12:07.000000 py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:12:07.997352 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 21:11:57.000000 py-aws-lambda-toolkit-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-05 21:12:07.997352 py-aws-lambda-toolkit-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-07 19:16:43.803566 py-aws-lambda-toolkit-0.0.3/setup.cfg
```

### Comparing `py-aws-lambda-toolkit-0.0.1/LICENSE` & `py-aws-lambda-toolkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/PKG-INFO` & `py-aws-lambda-toolkit-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.1
+Version: 0.0.3
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit,python,sls
 Classifier: Development Status :: 1 - Planning
@@ -34,15 +34,15 @@
 - Validator: Validate a dictionary with specified rules.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
-pip install py-sls-lambda-toolkit
+pip install py-aws-lambda-toolkit
 ```
 
 ## Usage
 
 Use the package in your code:
 
 ```python
@@ -69,15 +69,15 @@
 
     return response
 
 ```
 
 ## Contributing
 
-Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-sls-lambda-toolkit/issues). For code contributions please create a pull request.
+Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-aws-lambda-toolkit/issues). For code contributions please create a pull request.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Further Reading
```

### Comparing `py-aws-lambda-toolkit-0.0.1/README.md` & `py-aws-lambda-toolkit-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Validator: Validate a dictionary with specified rules.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
-pip install py-sls-lambda-toolkit
+pip install py-aws-lambda-toolkit
 ```
 
 ## Usage
 
 Use the package in your code:
 
 ```python
@@ -49,15 +49,15 @@
 
     return response
 
 ```
 
 ## Contributing
 
-Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-sls-lambda-toolkit/issues). For code contributions please create a pull request.
+Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-aws-lambda-toolkit/issues). For code contributions please create a pull request.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Further Reading
```

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_http_event.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_http_event.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_http_response.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_http_response.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_jwt.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_jwt.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_mappers.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_mappers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_parsers.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_parsers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_password.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_password.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/__tests__/test_validators.py` & `py-aws-lambda-toolkit-0.0.3/__tests__/test_validators.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/PKG-INFO` & `py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.1
+Version: 0.0.3
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit,python,sls
 Classifier: Development Status :: 1 - Planning
@@ -34,15 +34,15 @@
 - Validator: Validate a dictionary with specified rules.
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
-pip install py-sls-lambda-toolkit
+pip install py-aws-lambda-toolkit
 ```
 
 ## Usage
 
 Use the package in your code:
 
 ```python
@@ -69,15 +69,15 @@
 
     return response
 
 ```
 
 ## Contributing
 
-Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-sls-lambda-toolkit/issues). For code contributions please create a pull request.
+Contributions are welcome! For bug reports or requests please [submit an issue](https://github.com/0riion/py-aws-lambda-toolkit/issues). For code contributions please create a pull request.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Further Reading
```

### Comparing `py-aws-lambda-toolkit-0.0.1/py_aws_lambda_toolkit.egg-info/SOURCES.txt` & `py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/http_event.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/http_response.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/jwt.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/jwt.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/mappers.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/parsers.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/password.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/password.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/settings.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/status_code.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/py_sls_lambda_toolkit/validators.py` & `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.1/setup.cfg` & `py-aws-lambda-toolkit-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-aws-lambda-toolkit
-version = 0.0.1
+version = 0.0.3
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
@@ -31,14 +31,14 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	boto3==1.26.118
 	jsonschema==4.17.3
 	camel-converter==3.0.0
 	PyJWT==2.6.0
-	ruff==0.1.0
+	ruff==0.0.277
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

