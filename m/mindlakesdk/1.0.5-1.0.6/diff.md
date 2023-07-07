# Comparing `tmp/mindlakesdk-1.0.5.tar.gz` & `tmp/mindlakesdk-1.0.6.tar.gz`

## Comparing `mindlakesdk-1.0.5.tar` & `mindlakesdk-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/README.md
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/message.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/mindlakesdk/utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/LICENSE
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mindlakesdk-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/message.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/PKG-INFO
```

### Comparing `mindlakesdk-1.0.5/mindlakesdk/LICENSE` & `mindlakesdk-1.0.6/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/mindlakesdk/__init__.py` & `mindlakesdk-1.0.6/mindlakesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/mindlakesdk/cryptor.py` & `mindlakesdk-1.0.6/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/mindlakesdk/datalake.py` & `mindlakesdk-1.0.6/mindlakesdk/datalake.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,8 +42,10 @@
         return mindlakesdk.message.sendQuery(self.__session, executeSql)
     
     def dropCocoon(self, cocoonName: str) -> ResultType:
         return mindlakesdk.message.sendDropCocoon(self.__session, cocoonName)
     
     def dropTable(self, tableName: str) -> ResultType:
         return mindlakesdk.message.sendDropTable(self.__session, tableName)  
-    
+    
+    def queryForDataAndMeta(self, executeSql: str) -> ResultType:
+        return mindlakesdk.message.sendQueryForDataAndMeta(self.__session, executeSql)
```

### Comparing `mindlakesdk-1.0.5/mindlakesdk/keyhelper.py` & `mindlakesdk-1.0.6/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/mindlakesdk/message.py` & `mindlakesdk-1.0.6/mindlakesdk/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
     data = {"bizType":121, 'cocoonName': cocoonName}
     return __requestCommon(session, data)
 
 def sendQuery(session: Session, executeSql) -> ResultType:
     data = {"bizType":114, 'executeSql': executeSql}
     return __requestCommon(session, data)
 
+def sendQueryForDataAndMeta(session: Session, executeSql) -> ResultType:
+    data = {"bizType":113, 'executeSql': executeSql}
+    return __requestCommon(session, data)
+
 def sendDropCocoon(session: Session, cocoonName: str) -> ResultType:
     data = {"bizType":129, 'cocoonName': cocoonName}
     return __requestCommon(session, data)
 
 def sendDropTable(session: Session, tableName: str) -> ResultType:
     data = {"bizType":128, 'tableName': tableName}
     return __requestCommon(session, data)
```

### Comparing `mindlakesdk-1.0.5/mindlakesdk/permission.py` & `mindlakesdk-1.0.6/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/mindlakesdk/settings.py` & `mindlakesdk-1.0.6/mindlakesdk/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,8 +66,8 @@
                                 "type": "bytes"
                         }
                 ],
                 "stateMutability": "view",
                 "type": "function"
         }
 ]
-VERSION = 'v1.0.5'
+VERSION = 'v1.0.6'
```

### Comparing `mindlakesdk-1.0.5/mindlakesdk/utils.py` & `mindlakesdk-1.0.6/mindlakesdk/utils.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/LICENSE` & `mindlakesdk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.5/README.md` & `mindlakesdk-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -68,11 +68,13 @@
     * Initial Release
 * v1.0.1
     * Fix bug
 * v1.0.2
     * Improve performances
 * v1.0.5
     * Keep up the version number with TypeScript SDK
+* v1.0.6
+    * Add support for Mind DataPack
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `mindlakesdk-1.0.5/pyproject.toml` & `mindlakesdk-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v1.0.5"
+version = "v1.0.6"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mindlakesdk-1.0.5/PKG-INFO` & `mindlakesdk-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
@@ -86,11 +86,13 @@
     * Initial Release
 * v1.0.1
     * Fix bug
 * v1.0.2
     * Improve performances
 * v1.0.5
     * Keep up the version number with TypeScript SDK
+* v1.0.6
+    * Add support for Mind DataPack
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

