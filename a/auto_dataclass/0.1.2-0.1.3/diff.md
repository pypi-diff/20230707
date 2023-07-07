# Comparing `tmp/auto_dataclass-0.1.2.tar.gz` & `tmp/auto_dataclass-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dataclass-0.1.2.tar", last modified: Fri Jun 30 06:09:11 2023, max compression
+gzip compressed data, was "auto_dataclass-0.1.3.tar", last modified: Fri Jul  7 07:17:17 2023, max compression
```

## Comparing `auto_dataclass-0.1.2.tar` & `auto_dataclass-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.2/.gitignore
--rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.2/LICENSE
--rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.2/README.md
--rw-r--r--   0        0        0      106 2023-06-30 06:05:54.881375 auto_dataclass-0.1.2/auto_dataclass/__init__.py
--rw-r--r--   0        0        0     4911 2023-06-30 06:04:30.217816 auto_dataclass-0.1.2/auto_dataclass/dj_model_to_dataclass.py
--rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.2/poetry.lock
--rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6722 2023-06-30 06:05:16.597558 auto_dataclass-0.1.2/tests/tests_errors.py
--rw-r--r--   0        0        0     3299 2023-06-26 13:25:12.265667 auto_dataclass-0.1.2/tests/tests_to_dto_func.py
--rw-r--r--   0        0        0     3400 2023-06-29 21:34:19.675579 auto_dataclass-0.1.2/tests/tests_to_dto_func_with_recursive.py
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.3/README.md
+-rw-r--r--   0        0        0      106 2023-07-07 07:17:11.863140 auto_dataclass-0.1.3/auto_dataclass/__init__.py
+-rw-r--r--   0        0        0     5091 2023-07-07 07:15:22.971138 auto_dataclass-0.1.3/auto_dataclass/dj_model_to_dataclass.py
+-rw-r--r--   0        0        0      150 2023-07-07 06:32:16.675179 auto_dataclass-0.1.3/auto_dataclass/exceptions.py
+-rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.3/poetry.lock
+-rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6824 2023-07-07 06:32:16.687179 auto_dataclass-0.1.3/tests/tests_errors.py
+-rw-r--r--   0        0        0     3809 2023-07-07 07:13:49.279129 auto_dataclass-0.1.3/tests/tests_to_dto_func.py
+-rw-r--r--   0        0        0     4120 2023-07-07 06:12:51.136314 auto_dataclass-0.1.3/tests/tests_to_dto_func_with_recursive.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.3/PKG-INFO
```

### Comparing `auto_dataclass-0.1.2/.github/workflows/tests.yml` & `auto_dataclass-0.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.2/LICENSE` & `auto_dataclass-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.2/README.md` & `auto_dataclass-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.2/auto_dataclass/dj_model_to_dataclass.py` & `auto_dataclass-0.1.3/auto_dataclass/dj_model_to_dataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import dataclasses
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, is_dataclass
+from types import UnionType
 from typing import Type, ForwardRef, List, get_origin, Union
 from django.db.models.manager import Manager
 from django.db.models import Model
 
+from auto_dataclass.exceptions import ConversionError
 
 T = Type["T"]
 
 
 class ToDTOConverter(ABC):
     @abstractmethod
     def to_dto(self, data, dc: dataclass):
@@ -48,21 +50,22 @@
                     obj_for_dataclass[field.name] = field_data
         return dc(**obj_for_dataclass)
 
     @staticmethod
     def _is_field_name_exists_in_data(data: Model, field_name: str) -> bool | None:
         if hasattr(data, field_name):
             return True
-        raise AttributeError(
+        raise ConversionError(
             f"Field name '{field_name}' doesn't exist in {data}"
         )
 
     def _get_origin_field_type(self, field_type):
         is_list = False
-        if get_origin(field_type) is Union:
+        origin_type = get_origin(field_type)
+        if origin_type is Union or origin_type is UnionType:
             field_type = field_type.__args__[0]
         if hasattr(field_type, "__origin__") and field_type.__origin__ is list:
             field_type = field_type.__args__[0]
             is_list = True
         if isinstance(field_type, ForwardRef):
             field_type = field_type.__forward_arg__
             field_type = self._get_future_object_type(field_type)
@@ -77,48 +80,48 @@
         self, field_data: Manager, field_type: T
     ) -> List[dataclass]:
         values_lst = []
         try:
             for orm_obj in field_data.all():
                 values_lst.append(self._to_dataclass_obj(orm_obj, field_type))
         except AttributeError:
-            raise TypeError(f"The {field_data} is not iterable, but specified type is List[{field_type}]")
+            raise ConversionError(f"The {field_data} is not iterable, but specified type is List[{field_type}]")
         return values_lst
 
     def _get_future_object_type(self, obj_type: str) -> dataclass:
         if self._future_dataclasses:
             for dc in self._future_dataclasses:
                 if dc.__name__ == obj_type:
                     return dc
-            raise TypeError(
-                f"The 'future_dataclasses' arguments must be defined for future reference '{obj_type}'."
+            raise ConversionError(
+                f"The 'future_dataclasses' argument must be defined for future reference '{obj_type}'."
             )
 
     @staticmethod
     def _check_dataclass_arg(dc: dataclass) -> dataclass:
         if dataclasses.is_dataclass(dc):
             return dc
-        raise TypeError(f"The 'dc' arg should be dataclass type, not {type(dc)} type")
+        raise ConversionError(f"The 'dc' arg should be dataclass type, not {type(dc)} type")
 
     def _check_future_dataclasses_arg(self, future_dataclasses: List[dataclass]) -> None:
         if future_dataclasses is None:
             return
         if not isinstance(future_dataclasses, list):
-            raise TypeError(
+            raise ConversionError(
                 f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes or "
                 f"None type, not {type(future_dataclasses)}."
             )
         for dc in future_dataclasses:
             if not is_dataclass(dc):
-                raise TypeError(
+                raise ConversionError(
                     f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
                     f"Received {dc} with type {type(dc)}."
                 )
             self._future_dataclasses.append(dc)
 
     @staticmethod
     def _is_data_dj_model_type(data: Model):
         if isinstance(data, Model):
             return data
-        raise TypeError(
+        raise ConversionError(
             f"Data must be a django.db.models.Model type. Instead, received '{type(data)}'"
         )
```

### Comparing `auto_dataclass-0.1.2/poetry.lock` & `auto_dataclass-0.1.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.2/pyproject.toml` & `auto_dataclass-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.2/tests/tests_errors.py` & `auto_dataclass-0.1.3/tests/tests_errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 from typing import List
 from unittest import TestCase
 from unittest.mock import Mock, MagicMock
 
 from django.db.models import Model, QuerySet
 
 from auto_dataclass.dj_model_to_dataclass import FromOrmToDataclass
+from auto_dataclass.exceptions import ConversionError
 
 
 class TestErrorToDTOFunc(TestCase):
     @dataclass
     class TestDataclass:
         id: int
         name: str
 
     def setUp(self) -> None:
         self.converter = FromOrmToDataclass()
 
     def test_error_to_dto_incorrect_data_type(self) -> None:
         queryset = Mock(spec=QuerySet)
 
-        with self.assertRaises(TypeError):
+        with self.assertRaises(ConversionError):
             self.converter.to_dto({"test": "dict"}, self.TestDataclass)
 
-        with self.assertRaises(TypeError):
+        with self.assertRaises(ConversionError):
             self.converter.to_dto(queryset, self.TestDataclass)
 
     def test_error_to_dto_incorrect_dataclass(self) -> None:
         class IsNotDataclass:
             id: int
             name: str
 
         mock_model = Mock(spec=Model)
         mock_model.id = 1
         mock_model.name = "first"
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(mock_model, IsNotDataclass)
         self.assertEqual(
             f"The 'dc' arg should be dataclass type, not {type(IsNotDataclass)} type",
             str(cm.exception)
         )
 
     def test_error_to_dto_incorrect_dataclass_field_name(self) -> None:
@@ -53,15 +54,15 @@
 
         mock_model = Mock(spec=Model)
         mock_related_manager = MagicMock()
         mock_related_manager.all.return_value = self.get_list_db_model_objects()
         mock_model.id = 1
         mock_model.dc = mock_related_manager
 
-        with self.assertRaises(AttributeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(mock_model, OuterTestDataclass)
         self.assertEqual(
             f"Field name 'non_existed_field_name' doesn't exist in {mock_model}",
             str(cm.exception)
         )
 
     def test_error_to_dto_incorrect_future_dataclasses_arg_type(self):
@@ -79,15 +80,15 @@
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
         future_dataclass = "future_dataclasses"
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass,
                 future_dataclasses=future_dataclass
             )
         self.assertEqual(
             f"The 'future_dataclasses' arguments should be a list of 'dataclass' classes or "
@@ -109,15 +110,15 @@
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
         future_dataclass = "future_dataclasses"
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass,
                 future_dataclasses=[future_dataclass]
             )
         self.assertEqual(
             "The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
@@ -136,15 +137,15 @@
         outer_mock_model = Mock(spec=Model)
         inner_mock_model = Mock(spec=Model)
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass,
                 future_dataclasses=[FutureTestClass]
             )
         self.assertEqual(
             "The 'future_dataclasses' arguments should be a list of 'dataclass' classes. "
@@ -164,21 +165,21 @@
         outer_mock_model = Mock(spec=Model)
         inner_mock_model = Mock(spec=Model)
         inner_mock_model.id = 2
         inner_mock_model.dc = None
         outer_mock_model.id = 1
         outer_mock_model.dc = inner_mock_model
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(
                 outer_mock_model,
                 RecursiveTestDataclass
             )
         self.assertEqual(
-            f"The 'future_dataclasses' arguments must be defined for future reference 'FutureTestDataclass'.",
+            f"The 'future_dataclasses' argument must be defined for future reference 'FutureTestDataclass'.",
             str(cm.exception)
         )
 
     def test_error_to_dto_incorrect_field_type(self) -> None:
 
         InnerTestDataclass = self.TestDataclass
 
@@ -187,15 +188,15 @@
             id: int
             dc: List[InnerTestDataclass]
 
         mock_model = Mock(spec=Model)
         mock_model.id = 1
         mock_model.dc = self.get_list_db_model_objects()[0]
 
-        with self.assertRaises(TypeError) as cm:
+        with self.assertRaises(ConversionError) as cm:
             self.converter.to_dto(mock_model, OuterTestDataclass)
         self.assertEqual(
             f"The {mock_model.dc} is not iterable, but specified type is List[{InnerTestDataclass}]",
             str(cm.exception)
         )
 
     @staticmethod
```

### Comparing `auto_dataclass-0.1.2/tests/tests_to_dto_func.py` & `auto_dataclass-0.1.3/tests/tests_to_dto_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,28 @@
         mock_model = Mock(spec=Model)
         mock_model.dc = None
         result = self.converter.to_dto(mock_model, OuterTestDataclass)
 
         self.assertIsInstance(result, OuterTestDataclass)
         self.assertEqual(result.dc, None)
 
+    def test__to_dto_db_related_object_or_none(self) -> None:
+        InnerTestDataclass = self.TestDataclass
+
+        @dataclass
+        class OuterTestDataclass:
+            dc: InnerTestDataclass | None = None
+
+        mock_model = Mock(spec=Model)
+        mock_model.dc = self.get_db_model_object()
+        result = self.converter.to_dto(mock_model, OuterTestDataclass)
+
+        self.assertIsInstance(result, OuterTestDataclass)
+        self.assertEqual(result.dc, InnerTestDataclass(id=1, name="first"))
+
     @staticmethod
     def get_db_model_object():
         model = Mock(spec=Model)
         model.id = 1
         model.name = "first"
         return model
```

### Comparing `auto_dataclass-0.1.2/tests/tests_to_dto_func_with_recursive.py` & `auto_dataclass-0.1.3/tests/tests_to_dto_func_with_recursive.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,7 +98,29 @@
             future_dataclasses=[RecursiveDataclass, RecursiveTestDataclass]
         )
 
         self.assertIsInstance(result, RecursiveTestDataclass)
         self.assertEqual(result.id, 1)
         self.assertEqual(result.dc[1], RecursiveTestDataclass(id=2, dc=None, double_dc=None))
         self.assertEqual(result.double_dc, RecursiveDataclass(id=3, name="name"))
+
+    def test_to_dto_recursive_relation_optional(self) -> None:
+        @dataclass
+        class RecursiveTestDataclass:
+            id: int
+            dc: Optional['RecursiveTestDataclass']
+
+        outer_mock_model = Mock(spec=Model)
+        inner_mock_model = Mock(spec=Model)
+        inner_mock_model.id = 2
+        inner_mock_model.dc = None
+        outer_mock_model.id = 1
+        outer_mock_model.dc = inner_mock_model
+
+        result = self.converter.to_dto(
+            outer_mock_model,
+            RecursiveTestDataclass
+        )
+
+        self.assertIsInstance(result, RecursiveTestDataclass)
+        self.assertEqual(result.id, 1)
+        self.assertEqual(result.dc, RecursiveTestDataclass(id=2, dc=None))
```

### Comparing `auto_dataclass-0.1.2/PKG-INFO` & `auto_dataclass-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_dataclass
-Version: 0.1.2
+Version: 0.1.3
 Summary: The package, helps to automatically transform data to DTO (DataClass) object
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/OleksandrZhydyk/Auto-Dataclass.git
 
 ## Auto dataclass
```

