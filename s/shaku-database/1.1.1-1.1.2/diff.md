# Comparing `tmp/shaku-database-1.1.1.tar.gz` & `tmp/shaku-database-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.1.tar", last modified: Wed Jul  5 06:31:46 2023, max compression
+gzip compressed data, was "shaku-database-1.1.2.tar", last modified: Fri Jul  7 09:42:02 2023, max compression
```

## Comparing `shaku-database-1.1.1.tar` & `shaku-database-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.632696 shaku-database-1.1.1/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.1/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 06:31:46.632506 shaku-database-1.1.1/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.1/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.630556 shaku-database-1.1.1/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.630780 shaku-database-1.1.1/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.1/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631016 shaku-database-1.1.1/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.1/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631160 shaku-database-1.1.1/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631383 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631638 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    10772 2023-07-05 06:31:10.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-05 06:31:46.632734 shaku-database-1.1.1/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-05 06:31:11.000000 shaku-database-1.1.1/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.632312 shaku-database-1.1.1/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      565 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.358436 shaku-database-1.1.2/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.2/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-07 09:42:02.358236 shaku-database-1.1.2/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.2/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.355414 shaku-database-1.1.2/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.355983 shaku-database-1.1.2/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.2/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.2/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356388 shaku-database-1.1.2/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.2/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.2/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356620 shaku-database-1.1.2/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.356880 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.357277 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    11602 2023-07-07 09:40:26.000000 shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-07 09:42:02.358480 shaku-database-1.1.2/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-07 09:40:50.000000 shaku-database-1.1.2/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:42:02.358044 shaku-database-1.1.2/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-07 09:42:02.000000 shaku-database-1.1.2/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.1/LICENSE` & `shaku-database-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.1/PKG-INFO` & `shaku-database-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.1
+Version: 1.1.2
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.1/README.md` & `shaku-database-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.1/database/bigquery/util.py` & `shaku-database-1.1.2/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.1/database/cloud_sql/crud.py` & `shaku-database-1.1.2/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.2/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.2/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaIoBaseDownload
 from googleapiclient.http import MediaIoBaseUpload
 from google.oauth2 import service_account
 import pandas as pd
 import io
 from pathlib import Path
-import os
+from zipfile import ZipFile
 
 
 class GDriveToolkit:
     def __init__(self, shared_drive_id, key_file_path):
         self.SCOPES = ['https://www.googleapis.com/auth/drive']
         self.KEY_FILE_PATH = key_file_path
         self.creds = service_account.Credentials.from_service_account_file(self.KEY_FILE_PATH, scopes=self.SCOPES)
@@ -145,30 +145,50 @@
                     downloaded = io.BytesIO()
                     downloader = MediaIoBaseDownload(downloaded, request)
                     done = False
                     while done is False:
                         status, done = downloader.next_chunk()
                         print(f"Download {int(status.progress() * 100)}%.")
                     downloaded.seek(0)
+                    try:
+                        if item['name'].endswith('.csv'):
+                            df = pd.read_csv(downloaded)
+                        else:
+                            df = pd.read_excel(downloaded, engine='openpyxl')
+                    except:
 
-                    if item['name'].endswith('.csv'):
-                        df = pd.read_csv(downloaded)
-                    else:
-                        df = pd.read_excel(downloaded, engine='openpyxl')
+                        self.read_as_xml(downloaded)
+                        df = pd.read_excel("tmp.xlsx", engine="openpyxl")
 
-                    # file_name_without_extension = os.path.splitext(item['name'])[0]
                     output[(file_name, file_id)] = df
 
             return output
 
         except HttpError as error:
             raise f'An error occurred:{error}'
         except Exception as e:
             raise f'An error occurred:{e}'
 
+    def read_as_xml(self, data):
+        with ZipFile(data, 'r') as ZIP:
+            list_files = ZIP.namelist()
+            for f in list_files:
+                ZIP.extract(f)
+            style_xml = ZIP.read('xl/styles.xml')
+            new_style_str = str(style_xml).replace('horizontal="left"', '"horizontal="center"')
+
+            with open("xl/styles_new.xml", "w") as binary_file:
+                binary_file.write(new_style_str)
+            with ZipFile('tmp.xlsx', mode='w') as zf:
+                # 加入要壓縮的檔案
+                for f in ZIP.namelist():
+                    if f != 'xl/styles.xml':
+                        zf.write(f)
+                zf.write("xl/styles_new.xml")
+
     def move_file(self, file_name, old_path, new_path):
 
         old_path_parts = Path(old_path)
         new_path_parts = Path(new_path)
 
         old_folder_name = old_path_parts.name
         new_folder_name = new_path_parts.name
@@ -243,15 +263,14 @@
                                                includeItemsFromAllDrives=True,
                                                driveId=self.shared_drive_id, corpora='drive'
                                                ).execute()
             files = result.get('files', [])
 
             media = MediaIoBaseUpload(data_buffer, mimetype=mimetype, resumable=True)
 
-
             if len(files) > 0:
                 file_metadata = {
                     'name': file_name
                 }
                 # file already exists, update it
                 file_id = files[0].get('id')
                 print(f"'{file_name}' is existed, update it")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shaku-database-1.1.1/setup.py` & `shaku-database-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.1",
+    version="1.1.2",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.1/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.2/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.1
+Version: 1.1.2
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.1/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.2/shaku_database.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 database/__init__.py
 database/bigquery/__init__.py
+database/bigquery/bq_sql_parser.py
 database/bigquery/util.py
 database/cloud_sql/__init__.py
 database/cloud_sql/crud.py
 gdrive_gcs_toolkit/__init__.py
 gdrive_gcs_toolkit/cloud_storage/__init__.py
 gdrive_gcs_toolkit/cloud_storage/util.py
 gdrive_gcs_toolkit/google_shared_drive/__init__.py
```

### Comparing `shaku-database-1.1.1/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.2/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

