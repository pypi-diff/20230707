# Comparing `tmp/ochsner_web2com-0.1.4.tar.gz` & `tmp/ochsner_web2com-0.1.5.tar.gz`

## Comparing `ochsner_web2com-0.1.4.tar` & `ochsner_web2com-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/ochsner_web2com/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/ochsner_web2com/web2com.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/LICENSE
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/ochsner_web2com/__init__.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/ochsner_web2com/web2com.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/PKG-INFO
```

### Comparing `ochsner_web2com-0.1.4/ochsner_web2com/web2com.py` & `ochsner_web2com-0.1.5/ochsner_web2com/web2com.py`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.4/LICENSE` & `ochsner_web2com-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.4/README.md` & `ochsner_web2com-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.4/PKG-INFO` & `ochsner_web2com-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ochsner_web2com
-Version: 0.1.4
+Version: 0.1.5
 Summary: Access to the ochsner web2com interface
 Project-URL: Homepage, https://github.com/ahackl/pypi_ochsner_web2com
 Project-URL: Bug Tracker, https://github.com/ahackl/pypi_ochsner_web2com/issues
 Author-email: Alexander Hackl <pypi@eccoz.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: enum
 Requires-Dist: requests
 Requires-Dist: xmltodict
 Description-Content-Type: text/markdown
 
 # ochsner_web2com
 
 `ochsner_web2com` is a Python module that read or write paramters of a web2com interface from ochser heat pump via SOAP requests.
```

