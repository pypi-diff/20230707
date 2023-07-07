# Comparing `tmp/cpi_tools-0.2.7.tar.gz` & `tmp/cpi_tools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.2.7.tar", last modified: Tue Jul  4 09:28:45 2023, max compression
+gzip compressed data, was "cpi_tools-0.2.8.tar", last modified: Fri Jul  7 15:59:52 2023, max compression
```

## Comparing `cpi_tools-0.2.7.tar` & `cpi_tools-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:28:45.859775 cpi_tools-0.2.7/
--rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      956 2023-07-04 09:28:45.860767 cpi_tools-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:28:45.822059 cpi_tools-0.2.7/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/cpi_tools/aws_tools.py
--rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/cpi_tools/cpi_validation.py
--rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/cpi_tools/fuzzy_matching_cpi.py
--rw-rw-rw-   0        0        0    15809 2023-07-04 09:05:45.000000 cpi_tools-0.2.7/cpi_tools/tracking_processing_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:28:45.856933 cpi_tools-0.2.7/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      956 2023-07-04 09:28:45.000000 cpi_tools-0.2.7/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-04 09:28:45.000000 cpi_tools-0.2.7/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:28:45.000000 cpi_tools-0.2.7/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 09:28:45.000000 cpi_tools-0.2.7/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0      581 2023-07-04 09:28:45.863747 cpi_tools-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 15:59:52.500520 cpi_tools-0.2.8/
+-rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-07-07 15:59:52.500520 cpi_tools-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 15:59:52.489916 cpi_tools-0.2.8/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/cpi_tools/aws_tools.py
+-rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/cpi_tools/cpi_validation.py
+-rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/cpi_tools/fuzzy_matching_cpi.py
+-rw-rw-rw-   0        0        0    16144 2023-07-07 15:51:32.000000 cpi_tools-0.2.8/cpi_tools/tracking_processing_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:59:52.499529 cpi_tools-0.2.8/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-07-07 15:59:52.000000 cpi_tools-0.2.8/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-07 15:59:52.000000 cpi_tools-0.2.8/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:59:52.000000 cpi_tools-0.2.8/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 15:59:52.000000 cpi_tools-0.2.8/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0      581 2023-07-07 15:59:52.500520 cpi_tools-0.2.8/setup.cfg
```

### Comparing `cpi_tools-0.2.7/LICENSE` & `cpi_tools-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.7/PKG-INFO` & `cpi_tools-0.2.8/cpi_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi_tools
-Version: 0.2.7
+Name: cpi-tools
+Version: 0.2.8
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.7/cpi_tools/aws_tools.py` & `cpi_tools-0.2.8/cpi_tools/aws_tools.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.7/cpi_tools/cpi_validation.py` & `cpi_tools-0.2.8/cpi_tools/cpi_validation.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.7/cpi_tools/fuzzy_matching_cpi.py` & `cpi_tools-0.2.8/cpi_tools/fuzzy_matching_cpi.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.7/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.2.8/cpi_tools/tracking_processing_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,14 +326,17 @@
     
     # Foreign exchange rates
     ref_fx =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_fx.csv', encoding='utf-8')
     
     # Gender table
     ref_gender =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gender.csv', encoding='utf-8')
     
+    # Gearing table
+    ref_gearing =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_gearing.csv', encoding='utf-8')
+    
     # CPI Geography Names
     ref_geog_list_cpi =  pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_geog_list_cpi.csv', encoding='utf-8')
     
     # Data Source Institution names
     ref_institution_list_all = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_institution_list_all.csv', encoding='utf-8')
     
     # CPI Institution names
@@ -347,23 +350,26 @@
     
     # Sector table
     ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
     
     # Instrument table
     ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
     
+    # Capacity multiplier tables
+    ref_multiplier = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_multiplier.csv', encoding='utf-8')
+    
     # Recipient table
     ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
     
     # Data source
     ref_data_source = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_data_source.csv', encoding='utf-8')
 
     # Return all the DataFrames as a tuple
-    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
-    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient, ref_data_source
+    return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_gearing, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
+    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_multiplier, ref_recipient, ref_data_source
 
 
 def generate_glcf_id(df:pd.DataFrame, year:int):
     '''
     This function generates a unique ID for each entry in the dataset processed. 
     
     Parameters:
```

### Comparing `cpi_tools-0.2.7/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi-tools
-Version: 0.2.7
+Name: cpi_tools
+Version: 0.2.8
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.7/setup.cfg` & `cpi_tools-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7069 5f74 6f6f 6c73 0d0a 7665   = cpi_tools..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 370d 0a61  rsion = 0.2.7..a
+00000020: 7273 696f 6e20 3d20 302e 322e 380d 0a61  rsion = 0.2.8..a
 00000030: 7574 686f 7220 3d20 4a61 6b65 2043 6f6e  uthor = Jake Con
 00000040: 6e6f 6c6c 792c 204e 696b 6974 6120 4d61  nolly, Nikita Ma
 00000050: 7269 6e69 0d0a 6175 7468 6f72 5f65 6d61  rini..author_ema
 00000060: 696c 203d 2064 6174 6173 6369 656e 6365  il = datascience
 00000070: 4063 7069 676c 6f62 616c 2e6f 7267 0d0a  @cpiglobal.org..
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 5265  description = Re
 00000090: 706f 7369 746f 7279 206f 6620 6675 6e63  pository of func
```

