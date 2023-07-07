# Comparing `tmp/metal_sdk-1.0.9.tar.gz` & `tmp/metal_sdk-2.0.0.tar.gz`

## Comparing `metal_sdk-1.0.9.tar` & `metal_sdk-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_metal.py
--rw-r--r--   0        0        0     9962 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_metal_async.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_motorhead.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_motorhead_async.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/fixtures/sample.csv
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/LICENSE
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_metal.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_motorhead.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/LICENSE
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/PKG-INFO
```

### Comparing `metal_sdk-1.0.9/.github/workflows/publish.yml` & `metal_sdk-2.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/.github/workflows/test.yml` & `metal_sdk-2.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/examples/example.py` & `metal_sdk-2.0.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/examples/example_async.py` & `metal_sdk-2.0.0/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/src/metal_sdk/metal.py` & `metal_sdk-2.0.0/src/metal_sdk/metal.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,18 +147,23 @@
 
         res = self.request("delete", url)
         res.raise_for_status()
 
         return None
 
     def delete_many(self, ids: List[str], index_id=None):
+        index = index_id or self.index_id
+
+        if index is None:
+            raise TypeError("index_id required")
+
         if ids is None:
             raise TypeError("ids required")
 
-        url = "/v1/documents/bulk"
+        url = f'/v1/indexes/{index}/documents/bulk'
 
         res = self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
 
         return None
 
     def __sanitize_filename(self, filename):
@@ -188,25 +193,29 @@
                 'content-length': str(file_size),
             }
             res = self.request("put", url, data=f, headers=headers)
 
         res.raise_for_status()  # Raise exception if the request failed
         return res
 
-    def upload_file(self, index_id, file_path):
+    def upload_file(self, file_path, index_id=None):
+        index = index_id or self.index_id
+        if index is None:
+            raise TypeError("index_id required")
+
         file_size = os.path.getsize(file_path)
         filename = os.path.basename(file_path)
         file_type, _ = mimetypes.guess_type(file_path)
 
         if file_type not in [
             'application/pdf',
             'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
             'application/vnd.ms-excel',
             'text/csv',
         ]:
             raise ValueError("Invalid file type. Supported types are: pdf, docx, csv.")
 
         # Create resource on the server
-        resource = self.__create_resource(index_id, filename, file_type, file_size)
+        resource = self.__create_resource(index, filename, file_type, file_size)
 
         # Upload the file to the returned url
         self.__upload_file_to_url(resource['data']['url'], file_path, file_type, file_size)
```

### Comparing `metal_sdk-1.0.9/src/metal_sdk/metal_async.py` & `metal_sdk-2.0.0/src/metal_sdk/metal_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,19 +145,24 @@
 
         url = "/v1/indexes/" + index + "/documents/" + id
 
         res = await self.request("delete", url)
         res.raise_for_status()
         return None
 
-    async def delete_many(self, ids: List[str]):
+    async def delete_many(self, ids: List[str], index_id=None):
+        index = index_id or self.index_id
+
+        if index is None:
+            raise TypeError("index_id required")
+
         if ids is None:
             raise TypeError("ids required")
 
-        url = "/v1/documents/bulk"
+        url = "/v1/indexes/" + index + "/documents/bulk"
 
         res = await self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
         return None
 
     def __sanitize_filename(self, filename):
         """
@@ -186,25 +191,30 @@
                 'content-length': str(file_size),
             }
             res = await self.request("put", url, data=f, headers=headers)
 
         res.raise_for_status()  # Raise exception if the request failed
         return res
 
-    async def upload_file(self, index_id, file_path):
+    async def upload_file(self, file_path, index_id=None):
+        index = index_id or self.index_id
+
+        if index is None:
+            raise TypeError("index_id required")
+
         file_size = os.path.getsize(file_path)
         filename = os.path.basename(file_path)
         file_type, _ = mimetypes.guess_type(file_path)
 
         if file_type not in [
             'application/pdf',
             'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
             'application/vnd.ms-excel',
             'text/csv',
         ]:
             raise ValueError("Invalid file type. Supported types are: pdf, docx, csv.")
 
         # Create resource on the server
-        resource = await self.__create_resource(index_id, filename, file_type, file_size)
+        resource = await self.__create_resource(index, filename, file_type, file_size)
 
         # Upload the file to the returned url
         await self.__upload_file_to_url(resource['data']['url'], file_path, file_type, file_size)
```

### Comparing `metal_sdk-1.0.9/src/metal_sdk/motorhead.py` & `metal_sdk-2.0.0/src/metal_sdk/motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/src/metal_sdk/motorhead_async.py` & `metal_sdk-2.0.0/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/src/metal_sdk/typings.py` & `metal_sdk-2.0.0/src/metal_sdk/typings.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,29 @@
     metadata: NotRequired[dict]
 
 
 class BulkIndexPayload(TypedDict):
     data: List[BulkIndexItem]
 
 
-class SearchFilter(TypedDict):
+class SearchClause(TypedDict):
     field: str
     value: str | int | float
+    operator: str
+
+
+SearchFilter = TypedDict('SearchFilter', {'and': List[SearchClause], 'or': List[SearchClause]})
 
 
 class SearchPayload(TypedDict):
     imageBase64: NotRequired[str]
     imageUrl: NotRequired[str]
     text: NotRequired[str]
     embedding: NotRequired[List[float]]
-    filters: NotRequired[List[SearchFilter]]
+    filters: NotRequired[SearchFilter]
 
 
 class TunePayload(TypedDict):
     idA: str
     idB: str
     label: TuneLabel
```

### Comparing `metal_sdk-1.0.9/tests/test_metal.py` & `metal_sdk-2.0.0/tests/test_metal.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,36 +88,36 @@
         self.assertEqual(str(ctx.exception), "index_id required")
 
     def test_metal_search_without_payload(self):
         my_index = "my-index"
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal.request = mock.MagicMock(return_value=mock.Mock(status_code=200))
-        metal.search({"filters": [{"field": "foo", "value": "bar"}]}, limit=666)
+        metal.search({"filters": {"and": [{"field": "foo", "value": "bar", "operator": "eq"}]}}, limit=666)
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
             metal.request.call_args[0][0],
             "post",
         )
         self.assertEqual(
             metal.request.call_args[0][1],
             "/v1/search?limit=666",
         )
         self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
         self.assertEqual(metal.request.call_args[1]["json"].get("text"), None)
         self.assertEqual(
-            metal.request.call_args[1]["json"]["filters"], [{"field": "foo", "value": "bar"}]
+            metal.request.call_args[1]["json"]["filters"]["and"], [{"field": "foo", "value": "bar", "operator": "eq"}]
         )
 
     def test_metal_search_with_text(self):
         my_index = "my-index"
         payload = {
             "text": "some text",
-            "filters": [{"field": "number_of_the_beast", "value": 666}],
+            "filters": {"and": [{"field": "number_of_the_beast", "value": 666, "operator": "lt"}]},
         }
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
 
         metal.search(payload, ids_only=True)
@@ -200,15 +200,15 @@
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         metal.delete_many([id])
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/bulk")
         self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
 
     def test_upload_file(self):
         my_index = "my-index"
         # Get the directory containing this file
         this_dir = os.path.dirname(os.path.abspath(__file__))
 
@@ -217,15 +217,15 @@
         # mock_file_path = "./fixtures/sample.csv"
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal._Metal__create_resource = mock.MagicMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
         metal._Metal__upload_file_to_url = mock.MagicMock()
 
-        metal.upload_file(my_index, mock_file_path)
+        metal.upload_file(mock_file_path)
 
         self.assertEqual(metal._Metal__create_resource.call_count, 1)
         self.assertEqual(metal._Metal__upload_file_to_url.call_count, 1)
 
         create_args = metal._Metal__create_resource.call_args[0]
         self.assertEqual(create_args[0], my_index)
         self.assertEqual(create_args[1], "sample.csv")
```

### Comparing `metal_sdk-1.0.9/tests/test_metal_async.py` & `metal_sdk-2.0.0/tests/test_metal_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,29 +225,29 @@
 
         metal.request = mock.AsyncMock(return_value=mock_response)
 
         await metal.delete_many([id])
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
-        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/bulk")
         self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
 
     async def test_upload_file(self):
         my_index = "my-index"
         mock_file_path = "/path/to/mockfile.csv"
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal._Metal__create_resource = mock.AsyncMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
         metal._Metal__upload_file_to_url = mock.AsyncMock()
         os.path.getsize = mock.MagicMock(return_value=1000)
         os.path.basename = mock.MagicMock(return_value="mockfile.csv")
 
-        await metal.upload_file(my_index, mock_file_path)
+        await metal.upload_file(mock_file_path)
 
         self.assertEqual(metal._Metal__create_resource.call_count, 1)
         self.assertEqual(metal._Metal__upload_file_to_url.call_count, 1)
 
         create_args = metal._Metal__create_resource.call_args[0]
         self.assertEqual(create_args[0], my_index)
         self.assertEqual(create_args[1], "mockfile.csv")
```

### Comparing `metal_sdk-1.0.9/tests/test_motorhead.py` & `metal_sdk-2.0.0/tests/test_motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/tests/test_motorhead_async.py` & `metal_sdk-2.0.0/tests/test_motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/.gitignore` & `metal_sdk-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/LICENSE` & `metal_sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/README.md` & `metal_sdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.9/pyproject.toml` & `metal_sdk-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.9"
+version = "2.0.0"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.9/PKG-INFO` & `metal_sdk-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.9
+Version: 2.0.0
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

