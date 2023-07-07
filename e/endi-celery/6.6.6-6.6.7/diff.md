# Comparing `tmp/endi_celery-6.6.6.tar.gz` & `tmp/endi_celery-6.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endi_celery-6.6.6.tar", last modified: Sat Jul  1 10:57:21 2023, max compression
+gzip compressed data, was "endi_celery-6.6.7.tar", last modified: Fri Jul  7 10:15:19 2023, max compression
```

## Comparing `endi_celery-6.6.6.tar` & `endi_celery-6.6.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.453736 endi_celery-6.6.6/
--rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-07-01 10:57:05.000000 endi_celery-6.6.6/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.6/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.6/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-07-01 10:57:21.453736 endi_celery-6.6.6/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.6/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.6/development.ini
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.445736 endi_celery-6.6.6/endi_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.6/endi_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.6/endi_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.6/endi_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.6/endi_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.6/endi_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.6/endi_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.6/endi_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.6/endi_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.449735 endi_celery-6.6.6/endi_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.6/endi_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.6/endi_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.6/endi_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3103 2023-06-15 14:04:15.000000 endi_celery-6.6.6/endi_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.6/endi_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.450736 endi_celery-6.6.6/endi_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.6/endi_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.6/endi_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.452736 endi_celery-6.6.6/endi_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)    10123 2023-07-01 10:55:57.000000 endi_celery-6.6.6/endi_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-07-01 10:56:00.000000 endi_celery-6.6.6/endi_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.6/endi_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.6/endi_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    16393 2023-06-26 11:09:42.000000 endi_celery-6.6.6/endi_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.6/endi_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.6/endi_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.6/endi_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.6/endi_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.6/endi_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-01 10:57:21.446735 endi_celery-6.6.6/endi_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-07-01 10:57:20.000000 endi_celery-6.6.6/endi_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-07-01 10:57:21.000000 endi_celery-6.6.6/endi_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-07-01 10:57:20.000000 endi_celery-6.6.6/endi_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-07-01 10:57:21.000000 endi_celery-6.6.6/endi_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.6/endi_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-07-01 10:57:21.000000 endi_celery-6.6.6/endi_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-07-01 10:57:21.000000 endi_celery-6.6.6/endi_celery.egg-info/top_level.txt
--rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.6/prod_example.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.6/pytest.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.6/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-07-01 10:57:21.453736 endi_celery-6.6.6/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-06-26 11:47:38.000000 endi_celery-6.6.6/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:19.002561 endi_celery-6.6.7/
+-rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-07-07 10:13:16.000000 endi_celery-6.6.7/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.7/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.7/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-07-07 10:15:19.002561 endi_celery-6.6.7/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.7/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.7/development.ini
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:18.997561 endi_celery-6.6.7/endi_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.7/endi_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.7/endi_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.7/endi_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.7/endi_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.7/endi_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.7/endi_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.7/endi_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.7/endi_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:18.999561 endi_celery-6.6.7/endi_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.7/endi_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.7/endi_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.7/endi_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3103 2023-06-15 14:04:15.000000 endi_celery-6.6.7/endi_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.7/endi_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:19.000561 endi_celery-6.6.7/endi_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.7/endi_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.7/endi_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:19.002561 endi_celery-6.6.7/endi_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)    10633 2023-07-07 10:08:01.000000 endi_celery-6.6.7/endi_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-07-04 13:07:30.000000 endi_celery-6.6.7/endi_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.7/endi_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.7/endi_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    16393 2023-06-26 11:09:42.000000 endi_celery-6.6.7/endi_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.7/endi_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.7/endi_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.7/endi_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.7/endi_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.7/endi_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-07-07 10:15:18.998561 endi_celery-6.6.7/endi_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.7/endi_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-07-07 10:15:18.000000 endi_celery-6.6.7/endi_celery.egg-info/top_level.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.7/prod_example.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.7/pytest.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.7/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-07-07 10:15:19.002561 endi_celery-6.6.7/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-06-26 11:47:38.000000 endi_celery-6.6.7/setup.py
```

### Comparing `endi_celery-6.6.6/LICENSE.txt` & `endi_celery-6.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/PKG-INFO` & `endi_celery-6.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi_celery
-Version: 6.6.6
+Version: 6.6.7
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.6/README.rst` & `endi_celery-6.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/development.ini` & `endi_celery-6.6.7/development.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/__init__.py` & `endi_celery-6.6.7/endi_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/conf.py` & `endi_celery-6.6.7/endi_celery/conf.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/exception.py` & `endi_celery-6.6.7/endi_celery/exception.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/interfaces.py` & `endi_celery-6.6.7/endi_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/mail.py` & `endi_celery-6.6.7/endi_celery/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/models.py` & `endi_celery-6.6.7/endi_celery/models.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/parsers/__init__.py` & `endi_celery-6.6.7/endi_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/parsers/isacompta.py` & `endi_celery-6.6.7/endi_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/parsers/quadra.py` & `endi_celery-6.6.7/endi_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/parsers/sage.py` & `endi_celery-6.6.7/endi_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/parsers/sage_generation_expert.py` & `endi_celery-6.6.7/endi_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/__init__.py` & `endi_celery-6.6.7/endi_celery/tasks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from endi.models.accounting.bookeeping import CustomInvoiceBookEntryModule
 from endi.models.user.userdatas import UserDatas
 from endi.models.third_party.customer import Customer
 from endi.models.third_party.supplier import Supplier
 from endi.models.supply import SupplierInvoice, InternalSupplierInvoice
 from endi.models.tva import Tva
 from endi.models.task import Task
+from endi.models.accounting.operations import AccountingOperation
 
 
 def _add_userdatas_custom_headers(writer, query):
     """
     Specific to userdatas exports
 
     Add custom headers that are not added through automation
@@ -321,7 +322,24 @@
                 "remote_invoice_number",
                 "exported",
                 "cae_percentage",
                 "payer",
             ),
         },
     )
+    config.register_export_model(
+        key="accounting_operations",
+        model=AccountingOperation,
+        options={
+            "foreign_key_name": "id",
+            "order": (
+                "date",
+                "general_account",
+                "label",
+                "debit",
+                "credit",
+                "balance",
+                "analytical_account",
+                "company",
+            ),
+        },
+    )
```

### Comparing `endi_celery-6.6.6/endi_celery/tasks/accounting_measure_compute.py` & `endi_celery-6.6.7/endi_celery/tasks/accounting_measure_compute.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/accounting_parser.py` & `endi_celery-6.6.7/endi_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/csv_import.py` & `endi_celery-6.6.7/endi_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/export.py` & `endi_celery-6.6.7/endi_celery/tasks/export.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/mail.py` & `endi_celery-6.6.7/endi_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/notification.py` & `endi_celery-6.6.7/endi_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/tasks.py` & `endi_celery-6.6.7/endi_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/tasks/utils.py` & `endi_celery-6.6.7/endi_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery/transactional_task.py` & `endi_celery-6.6.7/endi_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/endi_celery.egg-info/PKG-INFO` & `endi_celery-6.6.7/endi_celery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi-celery
-Version: 6.6.6
+Version: 6.6.7
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.6/endi_celery.egg-info/SOURCES.txt` & `endi_celery-6.6.7/endi_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/prod_example.ini` & `endi_celery-6.6.7/prod_example.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.6/setup.py` & `endi_celery-6.6.7/setup.py`

 * *Files identical despite different names*

