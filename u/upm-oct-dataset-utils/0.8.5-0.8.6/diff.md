# Comparing `tmp/upm_oct_dataset_utils-0.8.5-py3-none-any.whl.zip` & `tmp/upm_oct_dataset_utils-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 28908 bytes, number of entries: 10
+Zip file size: 28906 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jan-20 12:05 upm_oct_dataset_utils/__init__.py
--rw-rw-rw-  2.0 fat    56107 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils/dataset_classes.py
+-rw-rw-rw-  2.0 fat    56099 b- defN 22-Mar-16 13:13 upm_oct_dataset_utils/dataset_classes.py
 -rw-rw-rw-  2.0 fat     4284 b- defN 21-Dec-20 18:27 upm_oct_dataset_utils/oct_processing_lib.py
 -rw-rw-rw-  2.0 fat     3481 b- defN 21-Dec-24 12:26 upm_oct_dataset_utils/visualization_lib.py
 -rw-rw-rw-  2.0 fat     1802 b- defN 22-Mar-14 00:37 upm_oct_dataset_utils/xml_processing_lib.py
--rw-rw-rw-  2.0 fat    35821 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils-0.8.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    10044 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils-0.8.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils-0.8.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils-0.8.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      946 b- defN 22-Mar-16 13:09 upm_oct_dataset_utils-0.8.5.dist-info/RECORD
-10 files, 112599 bytes uncompressed, 27258 bytes compressed:  75.8%
+-rw-rw-rw-  2.0 fat    35821 b- defN 22-Mar-16 13:14 upm_oct_dataset_utils-0.8.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    10044 b- defN 22-Mar-16 13:14 upm_oct_dataset_utils-0.8.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Mar-16 13:14 upm_oct_dataset_utils-0.8.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 22-Mar-16 13:14 upm_oct_dataset_utils-0.8.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      946 b- defN 22-Mar-16 13:14 upm_oct_dataset_utils-0.8.6.dist-info/RECORD
+10 files, 112591 bytes uncompressed, 27256 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: upm_oct_dataset_utils/visualization_lib.py
 Comment: 
 
 Filename: upm_oct_dataset_utils/xml_processing_lib.py
 Comment: 
 
-Filename: upm_oct_dataset_utils-0.8.5.dist-info/LICENSE.txt
+Filename: upm_oct_dataset_utils-0.8.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: upm_oct_dataset_utils-0.8.5.dist-info/METADATA
+Filename: upm_oct_dataset_utils-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: upm_oct_dataset_utils-0.8.5.dist-info/WHEEL
+Filename: upm_oct_dataset_utils-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: upm_oct_dataset_utils-0.8.5.dist-info/top_level.txt
+Filename: upm_oct_dataset_utils-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: upm_oct_dataset_utils-0.8.5.dist-info/RECORD
+Filename: upm_oct_dataset_utils-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## upm_oct_dataset_utils/dataset_classes.py

```diff
@@ -476,16 +476,16 @@
                 raise DatasetAccessError('data_types parameter must be a list of strings')
             for dtype in data_type:
                 if dtype not in self.data_types:
                     raise DatasetAccessError(f"'{dtype}' is not a valid data type")
         print(f"+ RAW DATASET INFO (Path -> '{self.dataset_path}')")
         raw_dataset_info = """
         - Adquisitions per patient study:
-            -> 4 OCT (macular_OD, macular_OS, optic-nerve_OD, optic-nerve_OS)
-            -> 4 OCTA (macular_OD, macular_OS, optic-nerve_OD, optic-nerve_OS)
+            -> 4 OCT (macular_OD, macular_OS, optic-disc_OD, optic-disc_OS)
+            -> 4 OCTA (macular_OD, macular_OS, optic-disc_OD, optic-disc_OS)
             -> 2 retinographies (OD, OS)
             -> 8 scans XML analysis report
         """
         print(raw_dataset_info)
         data_paths:dict = self.get_data_paths(group=group, patient_num=patient_num)
         for group, group_info in data_paths.items():
             print('----------------------------------------------------')
@@ -956,16 +956,16 @@
                 raise DatasetAccessError('data_types parameter must be a list of strings')
             for dtype in data_type:
                 if dtype not in self.data_types:
                     raise DatasetAccessError(f"'{dtype}' is not a valid data type")
         print(f"+ CLEAN DATASET INFO (Path -> '{self.dataset_path}')")
         clean_dataset_info = """
         - Adquisitions per patient:
-            -> 4 OCT (macular_OD, macular_OS, optic-nerve_OD, optic-nerve_OS)
-            -> 4 OCTA (macular_OD, macular_OS, optic-nerve_OD, optic-nerve_OS)
+            -> 4 OCT (macular_OD, macular_OS, optic-disc_OD, optic-disc_OS)
+            -> 4 OCTA (macular_OD, macular_OS, optic-disc_OD, optic-disc_OS)
             -> 2 retinographies (OD, OS)
             -> 8 scans in JSON analysis report
         """
         print(clean_dataset_info)
         data_paths:dict = self.get_data_paths(group=group, patient_num=patient_num)
         for group, group_info in data_paths.items():
             print('----------------------------------------------------')
```

## Comparing `upm_oct_dataset_utils-0.8.5.dist-info/LICENSE.txt` & `upm_oct_dataset_utils-0.8.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `upm_oct_dataset_utils-0.8.5.dist-info/METADATA` & `upm_oct_dataset_utils-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upm-oct-dataset-utils
-Version: 0.8.5
+Version: 0.8.6
 Summary: Dataset utility package for UPM OCT/OCTA study (MS, NMO and RIS)
 Home-page: https://github.com/pgmesa-upm/upm_oct_dataset_utils
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `upm_oct_dataset_utils-0.8.5.dist-info/RECORD` & `upm_oct_dataset_utils-0.8.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 upm_oct_dataset_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-upm_oct_dataset_utils/dataset_classes.py,sha256=u21vMZWUhw_sIs0lNCGXLWNaIbGmzHNNBEMROD5LEMc,56107
+upm_oct_dataset_utils/dataset_classes.py,sha256=iyD47MRgHlv_c_VF5X6b4CxGJBL2h_BDRh1KBtFza_U,56099
 upm_oct_dataset_utils/oct_processing_lib.py,sha256=8a6IzF3B3HKLkNK7u71TO8ikiZ2pm6FeQOfeMhaLe4M,4284
 upm_oct_dataset_utils/visualization_lib.py,sha256=SZTU2NNYYIthysBxHS6zO8xg9ZDIH5iojCrUWvK4qn8,3481
 upm_oct_dataset_utils/xml_processing_lib.py,sha256=ib1qaMcBG2KuwWfK_xVTE9BUVzQRK8lEnV0YWT1qb7k,1802
-upm_oct_dataset_utils-0.8.5.dist-info/LICENSE.txt,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-upm_oct_dataset_utils-0.8.5.dist-info/METADATA,sha256=jKwvbaScUi7bfe01MbGGciXWojxKbTnDhQB5Lr1-PPo,10044
-upm_oct_dataset_utils-0.8.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-upm_oct_dataset_utils-0.8.5.dist-info/top_level.txt,sha256=ohZHiY_uKIxnaNirtBZW9VxUFF-GZy_CVXhpuTc6CBs,22
-upm_oct_dataset_utils-0.8.5.dist-info/RECORD,,
+upm_oct_dataset_utils-0.8.6.dist-info/LICENSE.txt,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+upm_oct_dataset_utils-0.8.6.dist-info/METADATA,sha256=S-LN91ozjLX4oEwqCwT6ck7nnzuCKRczZDlgcpfeMRo,10044
+upm_oct_dataset_utils-0.8.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+upm_oct_dataset_utils-0.8.6.dist-info/top_level.txt,sha256=ohZHiY_uKIxnaNirtBZW9VxUFF-GZy_CVXhpuTc6CBs,22
+upm_oct_dataset_utils-0.8.6.dist-info/RECORD,,
```

