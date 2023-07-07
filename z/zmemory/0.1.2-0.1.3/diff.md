# Comparing `tmp/zmemory-0.1.2.tar.gz` & `tmp/zmemory-0.1.3.tar.gz`

## Comparing `zmemory-0.1.2.tar` & `zmemory-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 zmemory-0.1.2/src/zmemory/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zmemory-0.1.2/LICENSE
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 zmemory-0.1.2/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zmemory-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 zmemory-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 zmemory-0.1.3/src/zmemory/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zmemory-0.1.3/LICENSE
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 zmemory-0.1.3/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zmemory-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 zmemory-0.1.3/PKG-INFO
```

### Comparing `zmemory-0.1.2/src/zmemory/__init__.py` & `zmemory-0.1.3/src/zmemory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.instance = Redis(decode_responses=True, **config)
 
     def get(self, k):
         """获取值
         c.get('access_token_00b73bbe23f34a468b2a5f158701f17f_wx')
         """
         v = self.instance.get(k)
-        return json.loads(v)
+        return json.loads(v) if v else {}
 
     def set(self, k, v, seconds=0):
         """修改值
         c.get('access_token_00b73bbe23f34a468b2a5f158701f17f_wx')
         """
         v = json.dumps(v, ensure_ascii=False)
         self.instance.set(k, v)
```

### Comparing `zmemory-0.1.2/LICENSE` & `zmemory-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zmemory-0.1.2/pyproject.toml` & `zmemory-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zmemory"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen memory library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zmemory-0.1.2/PKG-INFO` & `zmemory-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zmemory
-Version: 0.1.2
+Version: 0.1.3
 Summary: zen memory library
 Project-URL: Homepage, https://github.com/inspirare6/zmemory
 Project-URL: Bug Tracker, https://github.com/inspirare6/zmemory/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

