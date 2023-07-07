# Comparing `tmp/dopplrSDK-3.0.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5202 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    11892 b- defN 23-Jul-07 13:20 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jul-07 13:22 dopplrSDK-3.0.0.dist-info/RECORD
-6 files, 14171 bytes uncompressed, 4336 bytes compressed:  69.4%
+Zip file size: 5209 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    11914 b- defN 23-Jul-07 13:39 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jul-07 13:41 dopplrSDK-3.1.0.dist-info/RECORD
+6 files, 14193 bytes uncompressed, 4343 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-3.0.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-3.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-3.0.0.dist-info/METADATA
+Filename: dopplrSDK-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-3.0.0.dist-info/WHEEL
+Filename: dopplrSDK-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-3.0.0.dist-info/top_level.txt
+Filename: dopplrSDK-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-3.0.0.dist-info/RECORD
+Filename: dopplrSDK-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -129,15 +129,15 @@
             tp=str(dtype)
             insert1="INSERT INTO doppler.\"DopplerSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
             cur_sch.execute(insert1)
             cnxn.commit()
 
 
         ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type)
-        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type+"',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
+        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type+"',\"Source\"= 'MLStudio' ,\"Status\"='Uploaded',\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
 
         
         if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
```

## Comparing `dopplrSDK-3.0.0.dist-info/LICENSE.txt` & `dopplrSDK-3.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-3.0.0.dist-info/METADATA` & `dopplrSDK-3.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 3.0.0
+Version: 3.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

