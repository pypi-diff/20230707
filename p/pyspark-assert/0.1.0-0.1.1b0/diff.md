# Comparing `tmp/pyspark_assert-0.1.0.tar.gz` & `tmp/pyspark_assert-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_assert-0.1.0.tar", max compression
+gzip compressed data, was "pyspark_assert-0.1.1b0.tar", max compression
```

## Comparing `pyspark_assert-0.1.0.tar` & `pyspark_assert-0.1.1b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/LICENSE
--rw-r--r--   0        0        0     4274 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/README.md
--rw-r--r--   0        0        0      419 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      120 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyspark_assert/__init__.py
--rw-r--r--   0        0        0     1752 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyspark_assert/_assertions.py
--rw-r--r--   0        0        0     7886 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyspark_assert/_testing.py
--rw-r--r--   0        0        0     3003 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyspark_assert/_utils.py
--rw-r--r--   0        0        0    11288 2023-03-31 21:16:09.744700 pyspark_assert-0.1.0/pyspark_assert/_wrappers.py
--rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 pyspark_assert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/LICENSE
+-rw-r--r--   0        0        0     4332 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/README.md
+-rw-r--r--   0        0        0      424 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyspark_assert/__init__.py
+-rw-r--r--   0        0        0     1804 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyspark_assert/_assertions.py
+-rw-r--r--   0        0        0     9148 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyspark_assert/_testing.py
+-rw-r--r--   0        0        0     4281 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyspark_assert/_utils.py
+-rw-r--r--   0        0        0    11412 2023-07-07 18:15:20.835959 pyspark_assert-0.1.1b0/pyspark_assert/_wrappers.py
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 pyspark_assert-0.1.1b0/PKG-INFO
```

### Comparing `pyspark_assert-0.1.0/LICENSE` & `pyspark_assert-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_assert-0.1.0/README.md` & `pyspark_assert-0.1.1b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 Simple unit testing library for PySpark.
 
 This library is intended for performing unit testing with PySpark on small DataFrames with 
 functions similar to Pandas' testing module. The API provides two functions, `assert_frame_equal`
 and `assert_schema_equal`, which can be used in tests. The former compares two DataFrames and
 raises an `AssertionError` if they are not equal. The latter does the same, but with schemas.
 
+## Installation
+
+```shell
+pip install pyspark-assert
+```
+
 ## Usage
 
 Let's say we are testing some custom functionality over PySpark using Pytest.
 
 ```python
 from pyspark.sql import functions as f
```

### Comparing `pyspark_assert-0.1.0/pyspark_assert/_assertions.py` & `pyspark_assert-0.1.1b0/pyspark_assert/_assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         '\tActual   : {0}'
     )
 
 
 class ListTemplatedAssertionError(TemplatedAssertionError):
 
     def __init__(self, left, right):
+        self.left = left
+        self.right = right
         left_msg = self._construct_msg(left)
         right_msg = self._construct_msg(right)
 
         super().__init__(left_msg, right_msg)
 
     @staticmethod
     def _construct_msg(data):
```

### Comparing `pyspark_assert-0.1.0/pyspark_assert/_testing.py` & `pyspark_assert-0.1.1b0/pyspark_assert/_testing.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ._assertions import (
     DifferentLengthAssertionError,
     IncorrectTypeAssertionError,
     DifferentSchemaAssertionError,
     DifferentDataAssertionError,
 )
-from ._utils import collect_from
+from ._utils import collect_from, filter_matches
 from ._wrappers import Column, Row
 
 
 _NULLABILITY_ATTRS = [
     'nullable',
     'valueContainsNull',
     'containsNull',
@@ -29,14 +29,15 @@
         check_nullable: bool = True,
         check_metadata: bool = True,
         check_column_order: bool = True,
         check_row_order: bool = True,
         check_exact: bool = True,
         rtol: float = 1.0e-5,
         atol: float = 1.0e-8,
+        error_message_type: str = 'non_matching',
 ):
     """Asserts two PySpark DataFrames are equal.
 
     left DataFrame is intended to be the actual DataFrame found after executing some process and
     right should be the expected result.
 
     This function only works for small DataFrames for unit testing as it will collect all data
@@ -47,51 +48,51 @@
     because it has to guess some things. For instance, turning row order off makes the function
     find which row from left corresponds to which on right, but it makes the comparison more
     flexible, because the user doesn't have to guess in which order will the rows return after a
     groupBy operation.
 
     Parameters
     ----------
-    left
+    left : DataFrame
         DataFrame to compare to expected.
-    right
+    right : DataFrame
         Expected DataFrame.
-    check_types
+    check_types : bool, default=True
         Whether to check column types. If False, columns of equivalent types can be compared. For
         example, if check_types=True and there is a column of longs in left which corresponds to
         a column of ints in right, an assertion error will be raised. If check_types=False,
-        values will be compared regardless. Defaults to True.
-    check_nullable
+        values will be compared regardless.
+    check_nullable : bool, default=True
         Whether a nullable column can be compared against a non-nullable column. It also applies
         to all nested types with nullable properties, such as maps with nullable values,
-        arrays with nullable elements or structs with nullable fields. Defaults to True.
-    check_metadata
+        arrays with nullable elements or structs with nullable fields.
+    check_metadata : bool, default=True
         Whether to check struct fields' metadata for equality. It also applies to all nested
         structs. If True, metadata must be equal for all structs present in both DataFrames.
-        Defaults to True.
-    check_column_order
+    check_column_order : bool, default=True
         Whether to check left and right have columns in the same order. If False, the function
         will attempt to map each column in right to its correspondent one in left, even if they
         have duplicated column names. If there are two columns with the same name and the same
         type they won't be disambiguated and will be considered to appear in the same order in
         both DataFrames. If check_types=False and there are columns with the same name they
-        might not be found and result in an error. Defaults to True.
-    check_row_order
-        Whether to check both DataFrames have rows in the same order. Defaults to True.
-    check_exact
+        might not be found and result in an error.
+    check_row_order : bool, default=True
+        Whether to check both DataFrames have rows in the same order.
+    check_exact : bool, default=True
         Whether to check floating point columns (float and double types) exactly. If False,
         then :func:`math.isclose` will be used to compare columns with these types. It's useful for
-        calculated float columns, since computations with these types are not precise. Defaults
-        to True.
-    rtol
+        calculated float columns, since computations with these types are not precise.
+    rtol : float, default=1.0e-5
         Relative tolerance (rel_tol) to use if check_exact=False (see :func:`math.isclose`).
-        Defaults to 1.0e-5.
-    atol
+    atol : float, default=1.0e-8
         Absolute tolerance (abs_tol) to use if check_exact=False (see :func:`math.isclose`).
-        Defaults to 1.0e-8.
+    error_message_type : {'full', 'non_matching'}, default='non_matching'
+        How to represent the error message in case the assertion fails. Either 'full' to show both
+        DataFrames completely, even where left and right match, or 'non_matching' to display only
+        the values where left and right mismatch, resulting in cleaner messages.
 
     Raises
     ------
     AssertionError
         If any of the checks fails.
 
     """
@@ -103,59 +104,66 @@
     assert_schema_equal(
         left.schema,
         right.schema,
         check_types=check_types,
         check_nullable=check_nullable,
         check_metadata=check_metadata,
         check_order=check_column_order,
+        error_message_type=error_message_type,
     )
 
     _assert_data_equal(
         left,
         right,
         check_column_order=check_column_order,
         check_row_order=check_row_order,
         check_exact=check_exact,
         rtol=rtol,
         atol=atol,
+        error_message_type=error_message_type,
     )
 
 
 def assert_schema_equal(
         left: pyspark.sql.types.StructType,
         right: pyspark.sql.types.StructType,
         *,
         check_types: bool = True,
         check_nullable: bool = True,
         check_metadata: bool = True,
         check_order: bool = True,
+        error_message_type: str = 'non_matching',
 ):
     """Asserts that PySpark DataFame schemas are equal.
 
     left schema is intended to be the actual schema found after executing some process and right
     should be the expected result.
 
     Parameters
     ----------
-    left
+    left : StructType
         Schema to compare to expected.
-    right
+    right : StructType
         Expected Schema.
-    check_types
+    check_types : bool, default=True
         Whether to raise an assertion error if columns in left and right with the same names have
-        different types. Defaults to True.
-    check_nullable
+        different types.
+    check_nullable : bool, default=True
         Whether to raise an assertion error if columns in left is nullable and column in right
         with the same name is not or vice versa. It also applies to nested types, such as map,
-        array or struct. Defaults to True.
-    check_metadata
+        array or struct.
+    check_metadata : bool, default=True
         Whether to raise an assertion error if columns in left and right with the same names have
-        different metadata. It also applies to nested structs. Defaults to True.
-    check_order
+        different metadata. It also applies to nested structs.
+    check_order : bool, default=True
         Whether to raise an exception if column order is not the same. Defaults to True.
+    error_message_type : {'full', 'non_matching'}, default='non_matching'
+        How to represent the error message in case the assertion fails. Either 'full' to show both
+        schemas completely, even where left and right match, or 'non_matching' to display only the
+        columns where left and right mismatch, resulting in cleaner messages.
 
     Raises
     ------
     AssertionError
         If any of the checks fails.
 
     """
@@ -172,26 +180,29 @@
 
     if not check_order:
         # Make sure duplicated columns are considered multiple times
         left = Counter(left)
         right = Counter(right)
 
     if left != right:
+        if error_message_type == 'non_matching':
+            left, right = filter_matches(left, right)
         raise DifferentSchemaAssertionError(left, right)
 
 
 def _assert_data_equal(
         left: pyspark.sql.DataFrame,
         right: pyspark.sql.DataFrame,
         *,
         check_column_order: bool = True,
         check_row_order: bool = True,
         check_exact: bool = True,
         rtol: float = 1.0e-5,
         atol: float = 1.0e-8,
+        error_message_type: str = 'non_matching',
 ):
     """Asserts that data is equal in both DataFrames."""
     # If we already checked columns are in the correct order there's no need to complicate stuff
     left_data = left.collect() if check_column_order else collect_from(left, right.schema.fields)
     right_data = right.collect()
 
     if len(left_data) != len(right_data):
@@ -213,8 +224,10 @@
     right_data = wrap_rows(right_data)
 
     if not check_row_order:
         left_data = Counter(left_data)
         right_data = Counter(right_data)
 
     if left_data != right_data:
+        if error_message_type == 'non_matching':
+            left_data, right_data = filter_matches(left_data, right_data)
         raise DifferentDataAssertionError(left_data, right_data)
```

### Comparing `pyspark_assert-0.1.0/pyspark_assert/_wrappers.py` & `pyspark_assert-0.1.1b0/pyspark_assert/_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     """Class that represents a DataType, but with the subset of attributes needed."""
 
     def __init__(self, name: str, attrs: Optional[Dict] = None):
         """Constructs an ImposterType instance.
 
         Parameters
         ----------
-        name
+        name : str
             Name of the type, such as 'string', 'array'...
-        attrs
+        attrs : dict, optional
             Mapping from attribute name to its value. Defaults to an empty dict.
         """
         if attrs is None:
             attrs = {}
 
         self._name = name
         self._attrs = HashableDict(attrs)
@@ -68,17 +68,17 @@
             column: pyspark.sql.types.StructField,
             ignore: Optional[List[str]] = None,
     ):
         """Constructs a Column instance.
 
         Parameters
         ----------
-        column
+        column : StructField
             Top-level (column) StructField this column is wrapping.
-        ignore
+        ignore : list of str, optional
             List of (possibly nested) attributes to remove from the wrapped column.
         """
         if ignore is None:
             ignore = []
 
         self._name = column.name
         self._ignore = set(ignore)
@@ -146,24 +146,23 @@
             rtol: Optional[float] = None,
             atol: Optional[float] = None,
     ):
         """Constructs a Row instance.
 
         Parameters
         ----------
-        row
+        row : Row
             Row to wrap.
-        make_hashable
+        make_hashable : bool, default=False
             Whether to make this row hashable or not. If False hash will raise NotImplementedError.
-            Defaults to False.
-        make_less_precise
-            Whether to use ApproxFloats or simple floats for float fields. Defaults to False.
-        rtol
+        make_less_precise : bool, default=False
+            Whether to use ApproxFloats or simple floats for float fields.
+        rtol : float, optional
             If make_less_precise=True, relative tolerance passed down to ApproxFloat.
-        atol
+        atol : float, optional
             If make_less_precise=True, absolute tolerance passed down to ApproxFloat.
         """
         self._hashable = make_hashable
         self._float_converter = (
             partial(ApproxFloat, rtol=rtol, atol=atol) if make_less_precise
             else float
         )
@@ -223,19 +222,19 @@
     """
 
     def __init__(self, x: float, rtol: float, atol: float):
         """Constructs a ApproxFloat instance.
 
         Parameters
         ----------
-        x
+        x : float
             Float to wrap.
-        rtol
+        rtol : float
             Relative tolerance allowed for equality.
-        atol
+        atol : float
             Absolute tolerance allowed for equality.
         """
         self._x = x
         self._rtol = rtol
         self._atol = atol
 
     def __hash__(self) -> int:
@@ -271,16 +270,16 @@
     """List of methods that ensure the underlying object is not modified."""
 
     def __init__(self, value: T):
         """Constructs a HashableWrapper instance.
 
         Parameters
         ----------
-        value
-            Object of an non-hashable type.
+        value : T
+            Object of a non-hashable type.
         """
         self._value = value
         self._hash_value = None
         for method in self._SAFE_METHODS:
             setattr(self, method, getattr(value, method))
 
     @property
```

### Comparing `pyspark_assert-0.1.0/PKG-INFO` & `pyspark_assert-0.1.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-assert
-Version: 0.1.0
+Version: 0.1.1b0
 Summary: Simple unit testing library for PySpark.
 Author: Soy-yo
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,14 +19,20 @@
 Simple unit testing library for PySpark.
 
 This library is intended for performing unit testing with PySpark on small DataFrames with 
 functions similar to Pandas' testing module. The API provides two functions, `assert_frame_equal`
 and `assert_schema_equal`, which can be used in tests. The former compares two DataFrames and
 raises an `AssertionError` if they are not equal. The latter does the same, but with schemas.
 
+## Installation
+
+```shell
+pip install pyspark-assert
+```
+
 ## Usage
 
 Let's say we are testing some custom functionality over PySpark using Pytest.
 
 ```python
 from pyspark.sql import functions as f
```

