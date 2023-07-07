# Comparing `tmp/dopplrSDK-2.9.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5195 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    11861 b- defN 23-Jul-06 09:40 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-06 09:42 dopplrSDK-2.9.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-06 09:42 dopplrSDK-2.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 09:42 dopplrSDK-2.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-06 09:42 dopplrSDK-2.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jul-06 09:42 dopplrSDK-2.9.0.dist-info/RECORD
-6 files, 14140 bytes uncompressed, 4329 bytes compressed:  69.4%
+Zip file size: 5202 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    11892 b- defN 23-Jul-07 13:20 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/RECORD
+6 files, 14171 bytes uncompressed, 4336 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.9.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-3.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.9.0.dist-info/METADATA
+Filename: dopplrSDK-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.9.0.dist-info/WHEEL
+Filename: dopplrSDK-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.9.0.dist-info/top_level.txt
+Filename: dopplrSDK-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.9.0.dist-info/RECORD
+Filename: dopplrSDK-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -91,14 +91,15 @@
         
 
         UserKey=results[1]
         OrgName=results[0]
         
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
+
         #file_name1=file_name.split('.')
         query="select count(\"TableName\") from doppler.\"DopplerLake\" DL join doppler.\"DopplerUser\" US on DL.\"UserKey\"=US.\"UserKey\" where \"TableName\"="+"'"+file_name+"'"+" and US.\"LoginName\"="+"'"+loginName+"'"
         cur.execute(query)
         results = cur.fetchone()
         if results[0]<1:
             insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'','Uploaded')"
             cur.execute(insert_query)
@@ -110,15 +111,15 @@
         insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name+"'"
         
         cur1.execute(insert_query1)
         results = cur1.fetchone()
         SourceKey=results[0]
         SourceKey=str(SourceKey)
 
-        df = pd.read_csv(filePath)
+        df = pd.read_csv(filePath+'.'+file_type)
         cur_del=cnxn.cursor()
         delete="DELETE FROM Doppler.\"DopplerSchema\" WHERE\"SourceKey\"="+SourceKey
         cur_del.execute(delete)
         cnxn.commit()
         cur_sch=cnxn.cursor()
         for name, dtype in df.dtypes.items():
             if(dtype == 'datetime64[ns]'):
@@ -136,29 +137,29 @@
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
 
         
         if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
-            
-            client.upload_file(filePath, ContainerName, ConnectionString)
+
+            client.upload_file(filePath+'.'+file_type, ContainerName, ConnectionString)
              # Generate a pre-signed URL        
             client.put_object_acl(ACL='public-read',
                               Bucket=ContainerName,
                               Key=ConnectionString)
             
             url = f"s3://{ContainerName}/{ConnectionString}"
             print("uri : ",url)
             cnxn.close()
             #print("done")
         else:
-            print(keys['Cloud'])
+            #print(keys['Cloud'])
             blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
-            with open(filePath, "rb") as data:
+            with open(filePath+'.'+file_type, "rb") as data:
                 blob_client.upload_blob(data)
             
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
@@ -254,8 +255,7 @@
                     file.write(blob_client.download_blob().readall())
             print("downloaded")
 
         
     except Exception as error:
         print("Error : ",error)
 
-
```

## Comparing `dopplrSDK-2.9.0.dist-info/LICENSE.txt` & `dopplrSDK-3.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.9.0.dist-info/METADATA` & `dopplrSDK-3.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.9.0
+Version: 3.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

