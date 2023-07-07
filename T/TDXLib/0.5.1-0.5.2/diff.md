# Comparing `tmp/TDXLib-0.5.1.tar.gz` & `tmp/TDXLib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDXLib-0.5.1.tar", last modified: Fri Jun  9 19:03:38 2023, max compression
+gzip compressed data, was "TDXLib-0.5.2.tar", last modified: Fri Jul  7 12:10:17 2023, max compression
```

## Comparing `TDXLib-0.5.1.tar` & `TDXLib-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 19:03:21.000000 TDXLib-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 19:03:21.000000 TDXLib-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-09 19:03:38.802640 TDXLib-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-09 19:03:21.000000 TDXLib-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.798640 TDXLib-0.5.1/TDXLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 19:03:38.000000 TDXLib-0.5.1/TDXLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 19:03:21.000000 TDXLib-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:03:38.802640 TDXLib-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-09 19:03:21.000000 TDXLib-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/tdxlib/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    54083 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_asset_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    46059 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_ticket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-09 19:03:21.000000 TDXLib-0.5.1/tdxlib/tdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:38.802640 TDXLib-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 19:03:21.000000 TDXLib-0.5.1/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 19:03:21.000000 TDXLib-0.5.1/test/test_tdx_ticket_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:17.316747 TDXLib-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 12:10:03.000000 TDXLib-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 12:10:03.000000 TDXLib-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-07 12:10:17.316747 TDXLib-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-07-07 12:10:03.000000 TDXLib-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:17.316747 TDXLib-0.5.2/TDXLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-07-07 12:10:17.000000 TDXLib-0.5.2/TDXLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-07 12:10:17.000000 TDXLib-0.5.2/TDXLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:10:17.000000 TDXLib-0.5.2/TDXLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 12:10:17.000000 TDXLib-0.5.2/TDXLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 12:10:17.000000 TDXLib-0.5.2/TDXLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 12:10:03.000000 TDXLib-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:10:17.316747 TDXLib-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 12:10:03.000000 TDXLib-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:17.316747 TDXLib-0.5.2/tdxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54083 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_asset_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46070 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_ticket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 12:10:03.000000 TDXLib-0.5.2/tdxlib/tdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:17.316747 TDXLib-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-07 12:10:03.000000 TDXLib-0.5.2/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-07 12:10:03.000000 TDXLib-0.5.2/test/test_tdx_ticket_integration.py
```

### Comparing `TDXLib-0.5.1/LICENSE` & `TDXLib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/PKG-INFO` & `TDXLib-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDXLib
-Version: 0.5.1
+Version: 0.5.2
 Summary: a python library for interacting with the TeamDynamix Web API
 Home-page: https://github.com/cedarville-university/tdxlib
 Author: Nat Biggs, Stephen Gaines, Josiah Lansford
 Author-email: tdxlib@cedarville.edu
 License: GNU General Public License v3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `TDXLib-0.5.1/README.md` & `TDXLib-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/TDXLib.egg-info/PKG-INFO` & `TDXLib-0.5.2/TDXLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDXLib
-Version: 0.5.1
+Version: 0.5.2
 Summary: a python library for interacting with the TeamDynamix Web API
 Home-page: https://github.com/cedarville-university/tdxlib
 Author: Nat Biggs, Stephen Gaines, Josiah Lansford
 Author-email: tdxlib@cedarville.edu
 License: GNU General Public License v3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `TDXLib-0.5.1/setup.py` & `TDXLib-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", 'r', encoding='utf-8"') as fh:
     outer_long_description = fh.read()
 
 setup(
     name='TDXLib',
     description='a python library for interacting with the TeamDynamix Web API',
-    version='0.5.1',
+    version='0.5.2',
     author='Nat Biggs, Stephen Gaines, Josiah Lansford',
     author_email='tdxlib@cedarville.edu',
     packages=['tdxlib'],
     url='https://github.com/cedarville-university/tdxlib',
     license='GNU General Public License v3.0',
     long_description_content_type='text/markdown',
     long_description=outer_long_description,
```

### Comparing `TDXLib-0.5.1/tdxlib/tdx_asset_integration.py` & `TDXLib-0.5.2/tdxlib/tdx_asset_integration.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/tdxlib/tdx_config.py` & `TDXLib-0.5.2/tdxlib/tdx_config.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/tdxlib/tdx_constants.py` & `TDXLib-0.5.2/tdxlib/tdx_constants.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/tdxlib/tdx_integration.py` & `TDXLib-0.5.2/tdxlib/tdx_integration.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/tdxlib/tdx_ticket.py` & `TDXLib-0.5.2/tdxlib/tdx_ticket.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/tdxlib/tdx_ticket_integration.py` & `TDXLib-0.5.2/tdxlib/tdx_ticket_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     
         :return: Edited TDXTicket object, if the operation was successful
 
         :rtype: tdxlib.tdx_ticket.TDXTicket
     
         """
         if group:
-            reassign = {'GroupID': self.get_group_by_name(responsible)['ID']}
+            reassign = {'ResponsibleGroupID': self.get_group_by_name(responsible)['ID']}
         else:
             reassign = {'ResponsibleUid': self.get_person_by_name_email(responsible)['UID']}
         return self.edit_ticket(ticket_id, reassign)
 
     def reschedule_ticket(self, ticket_id: Union[str, int], start_date: datetime.datetime = False,
                           end_date: datetime.datetime = False) -> tdxlib.tdx_ticket.TDXTicket:
         """
```

### Comparing `TDXLib-0.5.1/tdxlib/tdx_utils.py` & `TDXLib-0.5.2/tdxlib/tdx_utils.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/test/test_setup.py` & `TDXLib-0.5.2/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.5.1/test/test_tdx_ticket_integration.py` & `TDXLib-0.5.2/test/test_tdx_ticket_integration.py`

 * *Files identical despite different names*

