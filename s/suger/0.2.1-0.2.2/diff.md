# Comparing `tmp/suger-0.2.1.tar.gz` & `tmp/suger-0.2.2.tar.gz`

## Comparing `suger-0.2.1.tar` & `suger-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 suger-0.2.1/RoadMap.md
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.2.1/setup.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.2.1/upload.sh
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.2.1/安装.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.2.1/suger/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/FileUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/StringUtils.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.2.1/suger/common/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/CsvUtils.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/ExcelUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/JsonUtils.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/XmlUtils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.2.1/suger/data_operator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.2.1/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 suger-0.2.1/suger/stream/Stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/suger/stream/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/SSH.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/TerminalUtils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.2.1/suger/terminal/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_ExcelUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_FileUtils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_SSH.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_Stream.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_StringUtils.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_XmlUtils.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.2.1/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.1/tests/decorator/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.2.1/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.2.1/LICENSE
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 suger-0.2.1/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 suger-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 suger-0.2.2/RoadMap.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 suger-0.2.2/setup.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.2.2/upload.sh
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.2.2/安装.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.2.2/suger/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.2.2/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.2.2/suger/common/FileUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.2.2/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 suger-0.2.2/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.2.2/suger/common/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 suger-0.2.2/suger/data_operator/CsvUtils.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.2.2/suger/data_operator/ExcelUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.2.2/suger/data_operator/JsonUtils.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.2.2/suger/data_operator/XmlUtils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.2.2/suger/data_operator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.2/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.2.2/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.2.2/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 suger-0.2.2/suger/stream/Stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.2/suger/stream/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.2.2/suger/terminal/SSH.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.2.2/suger/terminal/TerminalUtils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.2.2/suger/terminal/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_ExcelUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_SSH.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_Stream.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_StringUtils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_XmlUtils.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 suger-0.2.2/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.2.2/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 suger-0.2.2/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 suger-0.2.2/PKG-INFO
```

### Comparing `suger-0.2.1/RoadMap.md` & `suger-0.2.2/RoadMap.md`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/common/FileCompareUtils.py` & `suger-0.2.2/suger/common/FileCompareUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/common/FileUtils.py` & `suger-0.2.2/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/common/ObjectUtils.py` & `suger-0.2.2/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/common/StringUtils.py` & `suger-0.2.2/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/data_operator/CsvUtils.py` & `suger-0.2.2/suger/data_operator/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/data_operator/ExcelUtils.py` & `suger-0.2.2/suger/data_operator/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/data_operator/JsonUtils.py` & `suger-0.2.2/suger/data_operator/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/data_operator/XmlUtils.py` & `suger-0.2.2/suger/data_operator/XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/decorator/csv_decorator.py` & `suger-0.2.2/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/terminal/SSH.py` & `suger-0.2.2/suger/terminal/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/suger/terminal/TerminalUtils.py` & `suger-0.2.2/suger/terminal/TerminalUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/tests/test_CsvUtils.py` & `suger-0.2.2/tests/test_CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/tests/test_ExcelUtils.py` & `suger-0.2.2/tests/test_ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/tests/test_JsonUtils.py` & `suger-0.2.2/tests/test_JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/tests/test_Stream.py` & `suger-0.2.2/tests/test_Stream.py`

 * *Files 19% similar despite different names*

```diff
@@ -76,7 +76,31 @@
     def test_to_dictionary(self):
         result = Stream(globalData).toDictionary(lambda x: x, lambda x: x * 2)
         self.assertEqual(result, {1: 2, 2: 4, 3: 6, 4: 8, 5: 10})
 
     def test_to_set(self):
         result = Stream(globalData).toSet()
         self.assertEqual(result, {1, 2, 3, 4, 5})
+
+
+
+    def test_reduce(self):
+        stream = Stream([1, 2, 3, 4, 5])
+        result = stream.reduce(lambda x, y: x + y, 0)
+        self.assertEqual(result, 15)
+
+    def test_reduce_with_initial_value(self):
+        stream = Stream([1, 2, 3, 4, 5])
+        result = stream.reduce(lambda x, y: x + y, 10)
+        self.assertEqual(result, 25)
+
+    def test_group_by(self):
+        stream = Stream(['apple', 'banana', 'cherry', 'date'])
+        result = stream.groupBy(lambda x: len(x))
+        expected = {4: ['date'], 5: ['apple'], 6: ['banana', 'cherry']}
+        self.assertEqual(result, expected)
+
+    def test_group_by_multiple_keys(self):
+        stream = Stream(['apple', 'banana', 'cherry', 'date'])
+        result = stream.groupBy(lambda x: x[0])
+        expected = {'a': ['apple'], 'b': ['banana'], 'c': ['cherry'], 'd': ['date']}
+        self.assertEqual(result, expected)
```

### Comparing `suger-0.2.1/tests/test_StringUtils.py` & `suger-0.2.2/tests/test_StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/tests/test_XmlUtils.py` & `suger-0.2.2/tests/test_XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/LICENSE` & `suger-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.2.1/README.md` & `suger-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 # suger
 
-version = 0.2.1
+version = 0.2.2
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
-use python with @decorator/@Annotation Like Java、C#、TypeScript 
-
-@author SolarisNeko
-
-
-# What is it
-Use Python in Decorator / Annotation Like Java Lombok / C# Annotation / TypeScript Decorator
-
-作者是写 Java / TypeScript 习惯了注解
-
-Use Like Other Language:
-1. Java Lombok @Data
-2. TypeScript  @Async
-3. C#  [Required(ErrorMessage = "{0} is required")]
-
-顺手写
+Feature:
+1. python @decorator = Java @annotation / C# [Required(ErrorMessage = "{0} is required")]
+2. python Stream = Java Stream / C# LinQ
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
-## Stream 流式计算 / from v0.2.1 
+## Stream 流式计算 / from v0.2.0
 ```python
 from suger.stream.Stream import Stream
 
     def test_demo(self):
         data = [1, 2, 3, 3, 4, 5]
-        result = Stream(data).filter(lambda x: x % 2 == 0) \
+        result = Stream(data)\
+            .filter(lambda x: x % 2 == 0) \
             .sort(reverse=True) \
             .map(lambda x: x * 2) \
             .toSet()
         self.assertEqual(result, {8, 4})
 
 ```
```

### Comparing `suger-0.2.1/pyproject.toml` & `suger-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.2.1/PKG-INFO` & `suger-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.2.1
+Version: 0.2.2
 Summary: suger is a sugar. use python in @decorator/@Annotation like other languages~
 Project-URL: Homepage, https://github.com/SolarisNeko/python-suger
 Project-URL: Bug Tracker, https://github.com/SolarisNeko/python-suger/issues
 Author-email: SolarisNeko <1417015340@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # suger
 
-version = 0.2.1
+version = 0.2.2
 
 ## Introduce 介绍
 
 suger is a sugar ~ 
 
-use python with @decorator/@Annotation Like Java、C#、TypeScript 
-
-@author SolarisNeko
-
-
-# What is it
-Use Python in Decorator / Annotation Like Java Lombok / C# Annotation / TypeScript Decorator
-
-作者是写 Java / TypeScript 习惯了注解
-
-Use Like Other Language:
-1. Java Lombok @Data
-2. TypeScript  @Async
-3. C#  [Required(ErrorMessage = "{0} is required")]
-
-顺手写
+Feature:
+1. python @decorator = Java @annotation / C# [Required(ErrorMessage = "{0} is required")]
+2. python Stream = Java Stream / C# LinQ
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
-## Stream 流式计算 / from v0.2.1 
+## Stream 流式计算 / from v0.2.0
 ```python
 from suger.stream.Stream import Stream
 
     def test_demo(self):
         data = [1, 2, 3, 3, 4, 5]
-        result = Stream(data).filter(lambda x: x % 2 == 0) \
+        result = Stream(data)\
+            .filter(lambda x: x % 2 == 0) \
             .sort(reverse=True) \
             .map(lambda x: x * 2) \
             .toSet()
         self.assertEqual(result, {8, 4})
 
 ```
```

