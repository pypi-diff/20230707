# Comparing `tmp/tableau_utilities-2.0.2.tar.gz` & `tmp/tableau_utilities-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.0.2.tar", last modified: Thu Jun 29 22:18:42 2023, max compression
+gzip compressed data, was "tableau_utilities-2.0.3.tar", last modified: Thu Jul  6 16:47:23 2023, max compression
```

## Comparing `tableau_utilities-2.0.2.tar` & `tableau_utilities-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.837285 tableau_utilities-2.0.2/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.2/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-06-29 22:18:42.836897 tableau_utilities-2.0.2/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2023-06-29 22:18:42.837426 tableau_utilities-2.0.2/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1107 2023-06-29 22:18:13.000000 tableau_utilities-2.0.2/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.818758 tableau_utilities-2.0.2/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.825055 tableau_utilities-2.0.2/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.831061 tableau_utilities-2.0.2/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     7391 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.833255 tableau_utilities-2.0.2/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    11142 2023-06-29 22:18:13.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    35146 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.835904 tableau_utilities-2.0.2/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)    10138 2023-06-28 16:57:49.000000 tableau_utilities-2.0.2/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-06-29 22:18:42.822377 tableau_utilities-2.0.2/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1205 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      112 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2023-06-29 22:18:42.000000 tableau_utilities-2.0.2/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.718644 tableau_utilities-2.0.3/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.3/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-06 16:47:23.718353 tableau_utilities-2.0.3/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-06 16:47:23.718754 tableau_utilities-2.0.3/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1107 2023-07-06 16:46:52.000000 tableau_utilities-2.0.3/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.703985 tableau_utilities-2.0.3/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.708883 tableau_utilities-2.0.3/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/general/funcs.py
+-rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.714093 tableau_utilities-2.0.3/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     7391 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.715765 tableau_utilities-2.0.3/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    11142 2023-06-29 22:18:13.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    35088 2023-07-06 16:46:52.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.717531 tableau_utilities-2.0.3/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.3/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)    10844 2023-07-06 16:46:52.000000 tableau_utilities-2.0.3/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-06 16:47:23.706818 tableau_utilities-2.0.3/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-06 16:47:23.000000 tableau_utilities-2.0.3/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.0.2/LICENSE` & `tableau_utilities-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/PKG-INFO` & `tableau_utilities-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.0.2
+Version: 2.0.3
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.2/README.md` & `tableau_utilities-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/setup.py` & `tableau_utilities-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.0.2",
+    version="2.0.3",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.scripts'
     ],
```

### Comparing `tableau_utilities-2.0.2/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.0.3/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.0.3/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.0.3/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/general/funcs.py` & `tableau_utilities-2.0.3/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.0.3/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/datasource.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.0.3/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.0.3/tableau_utilities/tableau_file/tableau_file.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.0.3/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,18 +251,16 @@
         if self.aliases and isinstance(self.aliases, dict):
             if isinstance(self.aliases['alias'], list):
                 self.aliases = self.aliases['alias']
             else:
                 self.aliases = [self.aliases['alias']]
         if self.desc and isinstance(self.desc, dict):
             self.desc = self.desc['formatted-text']['run']
-        if self.calculation and isinstance(self.calculation, dict) and self.calculation['@class'] == 'tableau':
-            self.calculation = self.calculation['@formula']
-        elif self.calculation:
-            self.calculation = None
+        if self.calculation and isinstance(self.calculation, dict):
+            self.calculation = self.calculation['@formula'] if self.calculation['@class'] == 'tableau' else None
         super().__post_init__()
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
     def __eq__(self, other):
         name = ''
```

### Comparing `tableau_utilities-2.0.2/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.0.3/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.0.3/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.2/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.0.3/tableau_utilities/test_tableau_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,59 +45,79 @@
         '--list_format', 'ids_names',
         '--list_sort_field', 'id',
     ]
     args = tu.cli.parser.parse_args(argv)
     assert args.server == 'us-east-1'
 
 
-# TEST 3: Datasource().DatasourceItems
+# TEST 3: Column()
+def test_column_attributes():
+    column_attributes = {
+        'name': '[FRIENDLY_CALC]',
+        'caption': 'Friendly Calc',
+        'datatype': 'integer',
+        'type': 'ordinal',
+        'role': 'dimension',
+        'desc': 'Nice and friendly',
+    }
+    column1 = tfo.Column(calculation='count(1)', **column_attributes)
+    column2 = tfo.Column(calculation={'@formula': 'count(1)', '@class': 'tableau'}, **column_attributes)
+    for attr, value in column_attributes.items():
+        assert value == getattr(column1, attr)
+        if attr == 'calculation':
+            assert 'count(1)' == getattr(column2, attr)
+        else:
+            assert value == getattr(column2, attr)
+
+
+# TEST 4: Datasource().DatasourceItems
 def test_datasource_items():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     assert datasource.columns is not None and datasource.columns != []
     assert datasource.folders_common is not None and datasource.folders_common != []
     assert datasource.aliases is not None and datasource.aliases != []
     assert datasource.connection is not None and datasource.connection != []
     assert datasource.extract is not None and datasource.extract != []
 
 
-# TEST 4: Datasource().unzip()
+# TEST 5: Datasource().unzip()
 def test_unzip_tableau_file():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     path = tu.Datasource(EXTRACT_PATH).unzip()
     with open(path) as f:
         content = f.read()
     os.remove(EXTRACT_PATH)
     os.remove(path)
     assert content is not None
 
 
-# TEST 5: Datasource().save()
+# TEST 6: Datasource().save()
 def test_datasource_save():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource_before = tu.Datasource(EXTRACT_PATH)
     datasource_before.save()
     datasource_after = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     for before, after in zip(datasource_before.sections(), datasource_after.sections()):
         assert before == after
 
 
-# TEST 6: Datasource().columns.add()
+# TEST 7: Datasource().columns.add()
 def test_add_column():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.columns.add(COLUMN)
     column = datasource.columns.get(COLUMN)
     assert column is not None
 
 
-# TEST 7: Datasource().enforce_column()
+# TEST 8: Datasource().enforce_column()
 def test_enforce_column():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     col = tfo.Column(
         name='renamed_name',
         datatype='string',
@@ -110,76 +130,76 @@
     folder = datasource.folders_common.get('A New Folder')
     metadata = datasource.connection.metadata_records.get('NAME')
     assert column == col
     assert folder is not None
     assert metadata.local_name == '[renamed_name]'
 
 
-# TEST 8: Datasource().columns.add()
+# TEST 9: Datasource().columns.add()
 def test_add_existing_column():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.columns.add(COLUMN)
     datasource.columns.add(COLUMN)
     assert len([c for c in datasource.columns if c == COLUMN]) == 1
 
 
-# TEST 9: Datasource().folders_common.folder.add()
+# TEST 10: Datasource().folders_common.folder.add()
 def test_add_folder_tdsx_has_folder():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.folders_common.add(FOLDER)
     found_folder = datasource.folders_common.get(FOLDER)
     assert found_folder is not None
 
 
-# TEST 10: Datasource().folders_common.folder.add()
+# TEST 11: Datasource().folders_common.folder.add()
 def test_add_folder_tdsx_does_not_have_folder():
     shutil.copyfile(f'resources/{NO_FOLDER_PATH}', NO_FOLDER_PATH)
     datasource = tu.Datasource(NO_FOLDER_PATH)
     os.remove(NO_FOLDER_PATH)
     datasource.folders_common.add(FOLDER)
     found_folder = datasource.folders_common.get(FOLDER)
     assert found_folder is not None
 
 
-# TEST 11: Datasource().folders_common.folder.add()
+# TEST 12: Datasource().folders_common.folder.add()
 def test_add_folder_tdsx_has_one_folder():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.folders_common.add(FOLDER)
     found_folder = datasource.folders_common.get(FOLDER)
     assert found_folder is not None
 
 
-# TEST 12: Datasource().folders_common.add()
+# TEST 13: Datasource().folders_common.add()
 def test_add_existing_folder():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.folders_common.add(FOLDER)
     datasource.folders_common.add(FOLDER)
     assert len([f for f in datasource.folders_common if f == FOLDER]) == 1
 
 
-# TEST 13: Datasource().folders_common.delete()
+# TEST 14: Datasource().folders_common.delete()
 def test_delete_folder():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     datasource.folders_common.add(FOLDER)
     datasource.folders_common.delete(FOLDER)
     found_folder = datasource.folders_common.get(FOLDER)
     assert not found_folder
 
 
-# TEST 14: Datasource().columns.update()
+# TEST 15: Datasource().columns.update()
 def test_update_column():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     datasource = tu.Datasource(EXTRACT_PATH)
     os.remove(EXTRACT_PATH)
     column = tfo.Column(
         name='QUANTITY',
         caption='Quantity Renamed',
@@ -188,15 +208,15 @@
         type="quantitative"
     )
     datasource.columns.update(column)
     col = datasource.columns.get(column)
     assert col.caption == 'Quantity Renamed'
 
 
-# TEST 15: Datasource().folders_common.get()
+# TEST 16: Datasource().folders_common.get()
 def test_get_folder():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     shutil.copyfile(f'resources/{ONE_FOLDER_PATH}', ONE_FOLDER_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     ds_one_folder = tu.Datasource(ONE_FOLDER_PATH)
@@ -204,15 +224,15 @@
     os.remove(LIVE_PATH)
     os.remove(ONE_FOLDER_PATH)
     assert ds_extract.folders_common.get('tidy') is not None
     assert ds_live.folders_common.get('tidy') is None
     assert ds_one_folder.folders_common.get('neat') is not None
 
 
-# TEST 16: Datasource().folders_common
+# TEST 17: Datasource().folders_common
 def test_find_all_folders():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     shutil.copyfile(f'resources/{ONE_FOLDER_PATH}', ONE_FOLDER_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     ds_one_folder = tu.Datasource(ONE_FOLDER_PATH)
@@ -224,15 +244,15 @@
     _folder_live = ds_live.folders_common
     _folder_one_folder = ds_one_folder.folders_common
     assert _folder == ['neat', 'tidy']
     assert _folder_live == []
     assert _folder_one_folder == ['neat']
 
 
-# TEST 17: Datasource().columns
+# TEST 18: Datasource().columns
 def test_find_all_columns():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     os.remove(EXTRACT_PATH)
     os.remove(LIVE_PATH)
@@ -246,39 +266,39 @@
     ]
     assert ds_live.columns == [
         'Number of Records',
         '[__tableau_internal_object_id__].[Migrated Data]'
     ]
 
 
-# TEST 18: Datasource().connection.relation.connection
+# TEST 19: Datasource().connection.relation.connection
 def test_find_all_connections():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     os.remove(EXTRACT_PATH)
     os.remove(LIVE_PATH)
     assert ds_extract.connection.named_connections == ['snowflake']
     assert ds_live.connection.named_connections == ['snowflake']
 
 
-# TEST 19: get_connections()
+# TEST 20: get_connections()
 def test_get_connection():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     os.remove(EXTRACT_PATH)
     os.remove(LIVE_PATH)
     assert ds_extract.connection.named_connections.get('snowflake') is not None
     assert ds_live.connection.named_connections.get('snowflake') is not None
 
 
-# TEST 20: Datasource().connection.update()
+# TEST 21: Datasource().connection.update()
 def test_update_connection():
     shutil.copyfile(f'resources/{EXTRACT_PATH}', EXTRACT_PATH)
     shutil.copyfile(f'resources/{LIVE_PATH}', LIVE_PATH)
     ds_extract = tu.Datasource(EXTRACT_PATH)
     ds_live = tu.Datasource(LIVE_PATH)
     os.remove(EXTRACT_PATH)
     os.remove(LIVE_PATH)
```

### Comparing `tableau_utilities-2.0.2/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.0.3/tableau_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-utilities
-Version: 2.0.2
+Version: 2.0.3
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.2/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.0.3/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

