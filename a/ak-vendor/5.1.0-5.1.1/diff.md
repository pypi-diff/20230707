# Comparing `tmp/ak_vendor-5.1.0.tar.gz` & `tmp/ak_vendor-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_vendor-5.1.0.tar", max compression
+gzip compressed data, was "ak_vendor-5.1.1.tar", max compression
```

## Comparing `ak_vendor-5.1.0.tar` & `ak_vendor-5.1.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1088 2019-07-25 16:08:45.967494 ak_vendor-5.1.0/LICENSE
--rw-r--r--   0        0        0        0 2019-07-25 16:08:45.990527 ak_vendor-5.1.0/ak_vendor/__init__.py
--rw-r--r--   0        0        0        0 2020-11-02 16:45:33.019813 ak_vendor-5.1.0/ak_vendor/admin.py
--rw-r--r--   0        0        0       90 2021-09-24 10:47:53.366785 ak_vendor-5.1.0/ak_vendor/apps.py
--rw-r--r--   0        0        0    11231 2021-09-24 10:47:53.368286 ak_vendor-5.1.0/ak_vendor/blocklist.py
--rw-r--r--   0        0        0        0 2021-09-06 08:47:06.563995 ak_vendor-5.1.0/ak_vendor/compliances/__init__.py
--rw-r--r--   0        0        0    98520 2021-09-24 10:47:53.369769 ak_vendor-5.1.0/ak_vendor/compliances/asvs.py
--rw-r--r--   0        0        0    89431 2021-09-06 08:47:06.566017 ak_vendor-5.1.0/ak_vendor/compliances/cwe.py
--rw-r--r--   0        0        0      753 2021-09-24 10:47:53.370556 ak_vendor-5.1.0/ak_vendor/compliances/gdpr.py
--rw-r--r--   0        0        0    22386 2021-09-24 10:47:53.371224 ak_vendor-5.1.0/ak_vendor/compliances/hipaa.py
--rw-r--r--   0        0        0    24621 2021-09-24 10:47:53.372026 ak_vendor-5.1.0/ak_vendor/compliances/mstg.py
--rw-r--r--   0        0        0     4402 2021-09-06 08:47:06.567407 ak_vendor-5.1.0/ak_vendor/compliances/owasp.py
--rw-r--r--   0        0        0    28191 2021-09-24 10:47:53.372617 ak_vendor-5.1.0/ak_vendor/compliances/pcidss.py
--rw-r--r--   0        0        0     5179 2021-09-24 10:47:53.373105 ak_vendor-5.1.0/ak_vendor/constants.py
--rw-r--r--   0        0        0     9484 2022-04-19 08:18:01.679967 ak_vendor-5.1.0/ak_vendor/enums.py
--rw-r--r--   0        0        0    39227 2022-01-04 11:54:05.885949 ak_vendor-5.1.0/ak_vendor/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   148428 2022-01-04 11:54:05.890512 ak_vendor-5.1.0/ak_vendor/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-11-02 16:45:33.033234 ak_vendor-5.1.0/ak_vendor/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-11-02 16:45:33.033403 ak_vendor-5.1.0/ak_vendor/models.py
--rw-r--r--   0        0        0     3828 2021-09-24 10:47:53.375619 ak_vendor-5.1.0/ak_vendor/pnguncrush.py
--rw-r--r--   0        0        0      859 2022-11-03 15:24:55.007346 ak_vendor-5.1.0/ak_vendor/report/__init__.py
--rw-r--r--   0        0        0    28352 2022-12-08 14:35:35.956536 ak_vendor-5.1.0/ak_vendor/report/report.py
--rw-r--r--   0        0        0     1145 2022-01-04 11:54:05.891851 ak_vendor-5.1.0/ak_vendor/report_sample.py
--rw-r--r--   0        0        0   256726 2021-09-06 08:47:06.592553 ak_vendor-5.1.0/ak_vendor/report_sample1.json
--rw-r--r--   0        0        0     9685 2021-09-24 10:47:53.379799 ak_vendor-5.1.0/ak_vendor/seed.py
--rw-r--r--   0        0        0    44481 2022-11-03 15:24:55.010006 ak_vendor-5.1.0/ak_vendor/templates/report_template.html
--rw-r--r--   0        0        0   134696 2019-07-25 16:08:46.010294 ak_vendor-5.1.0/ak_vendor/translations/ja/vulnerability.xlsx
--rw-r--r--   0        0        0      584 2021-09-24 10:47:53.380294 ak_vendor-5.1.0/ak_vendor/utils.py
--rw-r--r--   0        0        0        0 2020-11-02 16:45:33.035943 ak_vendor-5.1.0/ak_vendor/views.py
--rw-r--r--   0        0        0     1135 2022-12-08 14:36:06.209617 ak_vendor-5.1.0/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 ak_vendor-5.1.0/setup.py
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 ak_vendor-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-15 08:59:35.562406 ak_vendor-5.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.562952 ak_vendor-5.1.1/ak_vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.563042 ak_vendor-5.1.1/ak_vendor/admin.py
+-rw-r--r--   0        0        0       90 2023-05-15 08:59:35.563262 ak_vendor-5.1.1/ak_vendor/apps.py
+-rw-r--r--   0        0        0    11231 2023-05-15 08:59:35.563471 ak_vendor-5.1.1/ak_vendor/blocklist.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.563609 ak_vendor-5.1.1/ak_vendor/compliances/__init__.py
+-rw-r--r--   0        0        0    98520 2023-05-15 08:59:35.564370 ak_vendor-5.1.1/ak_vendor/compliances/asvs.py
+-rw-r--r--   0        0        0    89565 2023-07-07 08:44:43.272676 ak_vendor-5.1.1/ak_vendor/compliances/cwe.py
+-rw-r--r--   0        0        0      753 2023-05-15 08:59:35.564875 ak_vendor-5.1.1/ak_vendor/compliances/gdpr.py
+-rw-r--r--   0        0        0    22386 2023-05-15 08:59:35.565086 ak_vendor-5.1.1/ak_vendor/compliances/hipaa.py
+-rw-r--r--   0        0        0    24621 2023-05-15 08:59:35.565416 ak_vendor-5.1.1/ak_vendor/compliances/mstg.py
+-rw-r--r--   0        0        0     4402 2023-05-15 08:59:35.565663 ak_vendor-5.1.1/ak_vendor/compliances/owasp.py
+-rw-r--r--   0        0        0    28191 2023-05-15 08:59:35.565927 ak_vendor-5.1.1/ak_vendor/compliances/pcidss.py
+-rw-r--r--   0        0        0     5179 2023-05-15 08:59:35.566111 ak_vendor-5.1.1/ak_vendor/constants.py
+-rw-r--r--   0        0        0     9484 2023-05-15 08:59:35.566332 ak_vendor-5.1.1/ak_vendor/enums.py
+-rw-r--r--   0        0        0    39227 2023-05-15 08:59:35.584929 ak_vendor-5.1.1/ak_vendor/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   148428 2023-05-15 08:59:35.586847 ak_vendor-5.1.1/ak_vendor/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.587204 ak_vendor-5.1.1/ak_vendor/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.587345 ak_vendor-5.1.1/ak_vendor/models.py
+-rw-r--r--   0        0        0     3828 2023-05-15 08:59:35.587650 ak_vendor-5.1.1/ak_vendor/pnguncrush.py
+-rw-r--r--   0        0        0      859 2023-05-15 08:59:35.588032 ak_vendor-5.1.1/ak_vendor/report/__init__.py
+-rw-r--r--   0        0        0    28352 2023-05-15 08:59:35.588631 ak_vendor-5.1.1/ak_vendor/report/report.py
+-rw-r--r--   0        0        0     1145 2023-05-15 08:59:35.589079 ak_vendor-5.1.1/ak_vendor/report_sample.py
+-rw-r--r--   0        0        0   256726 2023-05-15 08:59:35.591005 ak_vendor-5.1.1/ak_vendor/report_sample1.json
+-rw-r--r--   0        0        0     9685 2023-05-15 08:59:35.592265 ak_vendor-5.1.1/ak_vendor/seed.py
+-rw-r--r--   0        0        0    44481 2023-05-15 08:59:35.593385 ak_vendor-5.1.1/ak_vendor/templates/report_template.html
+-rw-r--r--   0        0        0   134696 2023-05-15 08:59:35.595294 ak_vendor-5.1.1/ak_vendor/translations/ja/vulnerability.xlsx
+-rw-r--r--   0        0        0      584 2023-05-15 08:59:35.595610 ak_vendor-5.1.1/ak_vendor/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:59:35.595685 ak_vendor-5.1.1/ak_vendor/views.py
+-rw-r--r--   0        0        0     1135 2023-07-07 12:10:49.689101 ak_vendor-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 ak_vendor-5.1.1/PKG-INFO
```

### Comparing `ak_vendor-5.1.0/LICENSE` & `ak_vendor-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/blocklist.py` & `ak_vendor-5.1.1/ak_vendor/blocklist.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/asvs.py` & `ak_vendor-5.1.1/ak_vendor/compliances/asvs.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/cwe.py` & `ak_vendor-5.1.1/ak_vendor/compliances/cwe.py`

 * *Files 0% similar despite different names*

```diff
@@ -3401,14 +3401,19 @@
     },
     {
         "id": "CWE_1004",
         "code": "CWE-1004",
         "url": "https://cwe.mitre.org/data/definitions/1004.html",
     },
     {
+        "id": "CWE_1021",
+        "code": "CWE-1021",
+        "url": "https://cwe.mitre.org/data/definitions/1021.html",
+    },
+    {
         "id": "CWE_1299",
         "code": "CWE-1299",
         "url": "https://cwe.mitre.org/data/definitions/1299.html",
     },
 ]
```

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/gdpr.py` & `ak_vendor-5.1.1/ak_vendor/compliances/gdpr.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/hipaa.py` & `ak_vendor-5.1.1/ak_vendor/compliances/hipaa.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/mstg.py` & `ak_vendor-5.1.1/ak_vendor/compliances/mstg.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/owasp.py` & `ak_vendor-5.1.1/ak_vendor/compliances/owasp.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/compliances/pcidss.py` & `ak_vendor-5.1.1/ak_vendor/compliances/pcidss.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/constants.py` & `ak_vendor-5.1.1/ak_vendor/constants.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/enums.py` & `ak_vendor-5.1.1/ak_vendor/enums.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/locale/ja/LC_MESSAGES/django.mo` & `ak_vendor-5.1.1/ak_vendor/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/locale/ja/LC_MESSAGES/django.po` & `ak_vendor-5.1.1/ak_vendor/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/pnguncrush.py` & `ak_vendor-5.1.1/ak_vendor/pnguncrush.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/report/__init__.py` & `ak_vendor-5.1.1/ak_vendor/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/report/report.py` & `ak_vendor-5.1.1/ak_vendor/report/report.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/report_sample.py` & `ak_vendor-5.1.1/ak_vendor/report_sample.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/report_sample1.json` & `ak_vendor-5.1.1/ak_vendor/report_sample1.json`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/seed.py` & `ak_vendor-5.1.1/ak_vendor/seed.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/templates/report_template.html` & `ak_vendor-5.1.1/ak_vendor/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/translations/ja/vulnerability.xlsx` & `ak_vendor-5.1.1/ak_vendor/translations/ja/vulnerability.xlsx`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/ak_vendor/utils.py` & `ak_vendor-5.1.1/ak_vendor/utils.py`

 * *Files identical despite different names*

### Comparing `ak_vendor-5.1.0/pyproject.toml` & `ak_vendor-5.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ak-vendor"
-version = "5.1.0"
+version = "5.1.1"
 description = "Some vendor scripts that we use here at Appknox"
 authors = ["Appknox <engineering@appknox.com>"]
 license = "MIT"
 keywords = ["appknox", "vendor"]
 classifiers=[
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

### Comparing `ak_vendor-5.1.0/PKG-INFO` & `ak_vendor-5.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak-vendor
-Version: 5.1.0
+Version: 5.1.1
 Summary: Some vendor scripts that we use here at Appknox
 Home-page: https://github.com/appknox/vendor
 License: MIT
 Keywords: appknox,vendor
 Author: Appknox
 Author-email: engineering@appknox.com
 Requires-Python: >=3.8,<4.0
@@ -13,17 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: attrs (>=21.1.0)
 Requires-Dist: cvss (>=2.0)
 Requires-Dist: html2text (==2020.1.16)
 Requires-Dist: maya (>=0.6.0)
 Requires-Dist: orm-choices (==0.3.0)
 Project-URL: Repository, https://github.com/appknox/vendor
```

