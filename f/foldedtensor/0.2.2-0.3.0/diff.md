# Comparing `tmp/foldedtensor-0.2.2.tar.gz` & `tmp/foldedtensor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldedtensor-0.2.2.tar", last modified: Mon Jun  5 12:41:39 2023, max compression
+gzip compressed data, was "foldedtensor-0.3.0.tar", last modified: Fri Jul  7 15:45:33 2023, max compression
```

## Comparing `foldedtensor-0.2.2.tar` & `foldedtensor-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.712626 foldedtensor-0.2.2/foldedtensor/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/foldedtensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/foldedtensor/functions.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/foldedtensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/tests/test_folded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:45:33.681702 foldedtensor-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-07 15:45:33.681702 foldedtensor-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:45:33.677702 foldedtensor-0.3.0/foldedtensor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/foldedtensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/foldedtensor/functions.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:45:33.681702 foldedtensor-0.3.0/foldedtensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-07 15:45:33.000000 foldedtensor-0.3.0/foldedtensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 15:45:33.000000 foldedtensor-0.3.0/foldedtensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:45:33.000000 foldedtensor-0.3.0/foldedtensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 15:45:33.000000 foldedtensor-0.3.0/foldedtensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:45:33.000000 foldedtensor-0.3.0/foldedtensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:45:33.681702 foldedtensor-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:45:33.681702 foldedtensor-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-07 15:45:21.000000 foldedtensor-0.3.0/tests/test_folded_tensor.py
```

### Comparing `foldedtensor-0.2.2/LICENSE` & `foldedtensor-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.2.2/PKG-INFO` & `foldedtensor-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedtensor
-Version: 0.2.2
+Version: 0.3.0
 Summary: PyTorch extension for handling deeply nested sequences of variable length
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2023 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -23,16 +23,22 @@
 License-File: LICENSE
 
 <div align="center">
 <p align="center">
   <img src="https://github.com/aphp/foldedtensor/raw/main/banner.png" width="70%">
 </p>
 </div>
+<br/>
 
-----
+---
+
+![Tests](https://img.shields.io/github/actions/workflow/status/aphp/foldedtensor/tests.yml?branch=main&label=tests&style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/foldedtensor?color=blue&style=flat-square)](https://pypi.org/project/foldedtensor/)
+[![Codecov](https://img.shields.io/codecov/c/github/aphp/foldedtensor?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/foldedtensor)
+[![License](https://img.shields.io/github/license/aphp/foldedtensor?color=x&style=flat-square)](https://github.com/aphp/foldedtensor/blob/main/LICENSE)
 
 # FoldedTensor: PyTorch extension for handling deeply nested sequences of variable length
 
 `foldedtensor` is a PyTorch extension that provides efficient handling of tensors containing deeply nested sequences variable sizes. It enables the flattening/unflattening (or unfolding/folding) of data dimensions based on a inner structure of sequence lengths. This library is particularly useful when working with data that can be split in different ways and enables you to avoid choosing a fixed representation.
 
 ## Installation
 
@@ -100,13 +106,13 @@
 ## Comparison with alternatives
 
 Unlike other ragged or nested tensor implementations, a FoldedTensor does not enforce a specific structure on the nested data, and does not require padding all dimensions. This provides the user with greater flexibility when working with data that can be arranged in multiple ways depending on the data transformation. Moreover, the C++ optimization ensures high performance, making it ideal for handling deeply nested tensors efficiently.
 
 Here is a comparison with other common implementations for handling nested sequences of variable length:
 
 | Feature                   | NestedTensor | MaskedTensor | FoldedTensor |
-| ------------------------- | ------------ | ------------ | ------------ |
+|---------------------------|--------------|--------------|--------------|
 | Inner data structure      | Flat         | Padded       | Arbitrary    |
 | Max nesting level         | 1            | 1            | ∞            |
 | From nested python lists  | No           | No           | Yes          |
 | Layout conversion         | To padded    | No           | Any          |
 | Reduction ops w/o padding | Yes          | No           | No           |
```

### Comparing `foldedtensor-0.2.2/README.md` & `foldedtensor-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 <div align="center">
 <p align="center">
   <img src="https://github.com/aphp/foldedtensor/raw/main/banner.png" width="70%">
 </p>
 </div>
+<br/>
 
-----
+---
+
+![Tests](https://img.shields.io/github/actions/workflow/status/aphp/foldedtensor/tests.yml?branch=main&label=tests&style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/foldedtensor?color=blue&style=flat-square)](https://pypi.org/project/foldedtensor/)
+[![Codecov](https://img.shields.io/codecov/c/github/aphp/foldedtensor?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/foldedtensor)
+[![License](https://img.shields.io/github/license/aphp/foldedtensor?color=x&style=flat-square)](https://github.com/aphp/foldedtensor/blob/main/LICENSE)
 
 # FoldedTensor: PyTorch extension for handling deeply nested sequences of variable length
 
 `foldedtensor` is a PyTorch extension that provides efficient handling of tensors containing deeply nested sequences variable sizes. It enables the flattening/unflattening (or unfolding/folding) of data dimensions based on a inner structure of sequence lengths. This library is particularly useful when working with data that can be split in different ways and enables you to avoid choosing a fixed representation.
 
 ## Installation
 
@@ -76,13 +82,13 @@
 ## Comparison with alternatives
 
 Unlike other ragged or nested tensor implementations, a FoldedTensor does not enforce a specific structure on the nested data, and does not require padding all dimensions. This provides the user with greater flexibility when working with data that can be arranged in multiple ways depending on the data transformation. Moreover, the C++ optimization ensures high performance, making it ideal for handling deeply nested tensors efficiently.
 
 Here is a comparison with other common implementations for handling nested sequences of variable length:
 
 | Feature                   | NestedTensor | MaskedTensor | FoldedTensor |
-| ------------------------- | ------------ | ------------ | ------------ |
+|---------------------------|--------------|--------------|--------------|
 | Inner data structure      | Flat         | Padded       | Arbitrary    |
 | Max nesting level         | 1            | 1            | ∞            |
 | From nested python lists  | No           | No           | Yes          |
 | Layout conversion         | To padded    | No           | Any          |
 | Reduction ops w/o padding | Yes          | No           | No           |
```

### Comparing `foldedtensor-0.2.2/foldedtensor/__init__.py` & `foldedtensor-0.3.0/foldedtensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     torch.float64: np.float64,
     torch.complex64: np.complex64,
     torch.complex128: np.complex128,
 }
 
 from . import _C
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 
 # noinspection PyMethodOverriding
 class Refold(Function):
     @staticmethod
     def forward(
         ctx,
@@ -119,15 +119,25 @@
     data_dims = tuple(
         dim if isinstance(dim, int) else full_names.index(dim) for dim in data_dims
     )
     if (data_dims[-1] + 1) != len(full_names):
         raise ValueError(
             "The last dimension of `data_dims` must be the last variable dimension."
         )
-    if isinstance(data, Sequence):
+    elif isinstance(data, torch.Tensor) and lengths is not None:
+        np_indexer, shape = _C.make_refolding_indexer(lengths, data_dims)
+        assert shape == list(data.shape[: len(data_dims)])
+        result = FoldedTensor(
+            data=data,
+            lengths=lengths,
+            data_dims=data_dims,
+            full_names=full_names,
+            indexer=torch.from_numpy(np_indexer).to(data.device),
+        )
+    elif isinstance(data, Sequence):
         if dtype is None:
             raise ValueError("dtype must be provided when `data` is a sequence")
         dtype = numpy_to_torch_dtype_dict.get(dtype, dtype)
         padded, indexer, lengths = _C.nested_py_list_to_padded_array(
             data,
             data_dims,
             np.dtype(dtype),
@@ -137,24 +147,14 @@
         result = FoldedTensor(
             data=padded,
             lengths=lengths,
             data_dims=data_dims,
             full_names=full_names,
             indexer=indexer,
         )
-    elif isinstance(data, torch.Tensor) and lengths is not None:
-        np_indexer, shape = _C.make_refolding_indexer(lengths, data_dims)
-        assert shape == list(data.shape[: len(data_dims)])
-        result = FoldedTensor(
-            data=data,
-            lengths=lengths,
-            data_dims=data_dims,
-            full_names=full_names,
-            indexer=torch.from_numpy(np_indexer).to(data.device),
-        )
     else:
         raise ValueError(
             "as_folded_tensor expects:"
             "- a `data` (optionally nested) sequence"
             "- a `data_dims` sequence of names for padded dimensions"
             "- a `full_names` sequence of names for variable dimensions"
         )
@@ -255,22 +255,26 @@
         ft = None
         for arg in (*args, *(kwargs or {}).values()):
             if isinstance(arg, FoldedTensor):
                 assert (
                     ft is None or ft.data_dims == arg.data_dims
                 ), "Cannot perform operation on FoldedTensors with different structure"
                 ft = arg
-            if isinstance(arg, list):
+            if isinstance(arg, (list, tuple)):
                 for item in arg:
-                    assert (
-                        ft is None or ft.data_dims == item.data_dims
-                    ), "Cannot perform operation on FoldedTensors with different structure"
-                    ft = item
-
-        if ft.shape[: len(ft.data_dims)] != result.shape[: len(ft.data_dims)]:
+                    if isinstance(item, FoldedTensor):
+                        assert (
+                            ft is None or ft.data_dims == item.data_dims
+                        ), "Cannot perform operation on FoldedTensors with different structure"
+                        ft = item
+
+        if (
+            ft is not None
+            and ft.shape[: len(ft.data_dims)] != result.shape[: len(ft.data_dims)]
+        ):
             return result.as_subclass(torch.Tensor)
 
         result = FoldedTensor(
             data=result,
             lengths=ft.lengths,
             data_dims=ft.data_dims,
             full_names=ft.full_names,
```

### Comparing `foldedtensor-0.2.2/foldedtensor/functions.cpp` & `foldedtensor-0.3.0/foldedtensor/functions.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -109,75 +109,89 @@
 
 #pragma clang diagnostic push
 #pragma ide diagnostic ignored "misc-no-recursion"
 
 size_t flatten_py_list(
         py::list nested_list,
         std::vector<std::vector<int64_t>> &lengths,
-        std::vector<std::tuple<std::vector<int64_t>, PyObject *>> &operations,
+        std::vector<std::tuple<std::vector<int64_t>, int64_t, PyObject *>> &operations,
         std::vector<int64_t> &current_indices,
         std::vector<int64_t> &data_dim_map,
         std::vector<int64_t> &shape,
-        int dim) {
+        int dim,
+        int total) {
     if (nested_list.empty()) {
-        return 0;
+        return total;
     }
 
-    size_t total = 0;
-
-    bool is_data_dim = dim < data_dim_map.size() && data_dim_map[dim] >= 0;
+    bool is_data_dim = dim >= data_dim_map.size() || data_dim_map[dim] >= 0;
+    bool next_is_foldable_dim = dim + 1 < data_dim_map.size();
 
     if (!py::isinstance<py::list>(nested_list[0])) {
-        operations.emplace_back(current_indices, PySequence_Fast(nested_list.ptr(), "Something when wrong when reading one of the inner list"));
+        if (dim < data_dim_map.size() - 1) {
+            throw py::value_error(
+                    "The provided data_dims have too many entries compared "
+                    "to the nesting of the input."
+            );
+        }
+        operations.emplace_back(
+                current_indices,
+                total,
+                PySequence_Fast(nested_list.ptr(), "Something when wrong when reading one of the inner lists"));
+        if (dim + 1 == data_dim_map.size()) {
+            total += nested_list.size();
+        }
         current_indices.back() += nested_list.size();
-        total += nested_list.size();
     } else {
-
-        if (lengths.size() <= dim + 1) {
+        if (next_is_foldable_dim && lengths.size() <= dim + 1) {
             lengths.emplace_back();
         }
 
         for (auto &&i: nested_list) {
 
             auto sublist = i.cast<py::list>();
-            lengths[dim + 1].push_back(sublist.size());
+
+            if (next_is_foldable_dim) {
+                lengths[dim + 1].push_back(sublist.size());
+            }
 
             if (is_data_dim) {
                 current_indices.push_back(0);
             }
 
-            total += flatten_py_list(
+            total = flatten_py_list(
                     sublist,
                     lengths,
                     operations,
                     current_indices,
                     data_dim_map,
                     shape,
-                    dim + 1);
+                    dim + 1,
+                    total);
+
+            if (current_indices.size() > shape.size()) {
+                shape.push_back(0);
+            }
+
+            shape[current_indices.size() - 1] = std::max(shape[current_indices.size() - 1], current_indices.back());
 
             if (is_data_dim) {
 
                 current_indices.pop_back();
                 current_indices.back() += 1;
+            }
 
-            } else {
-                // current_indices.back() = offset;
-
-                if (current_indices.size() > shape.size()) {
-                    shape.push_back(0);
-                }
-
-                shape[current_indices.size() - 1] = std::max(shape[current_indices.size() - 1], current_indices.back());
+            if (dim + 1 == data_dim_map.size()) {
+                total += 1;
             }
         }
     }
 
-    if (is_data_dim) {
-        shape[data_dim_map[dim]] = std::max(shape[data_dim_map[dim]], current_indices.back());
-    }
+    shape[current_indices.size() - 1] = std::max(shape[current_indices.size() - 1], current_indices.back());
+
     return total;
 }
 
 #pragma clang diagnostic pop
 
 std::tuple<
         py::array,                        // padded array
@@ -191,15 +205,15 @@
     // Will contain the variable lengths of the nested lists
     // One sequence per dimension, containing the lengths of the lists at that dimension
     std::vector<std::vector<int64_t>> lengths;
 
     // Operations to perform to assign the values to the padded array
     // Each operation is a tuple of the indices of the first element to assign
     // and a list of values to assign contiguously from that position
-    std::vector<std::tuple<std::vector<int64_t>, PyObject *>> operations;
+    std::vector<std::tuple<std::vector<int64_t>, int64_t, PyObject *>> operations;
 
     // Index from the data dimension to the dim in the theoretically fully padded list
     std::vector<int64_t> data_dim_map(*std::max_element(data_dims.begin(), data_dims.end()) + 1, -1);
     for (unsigned long i = 0; i < data_dims.size(); i++) {
         data_dim_map[data_dims[i]] = i;
     }
     lengths.emplace_back(1, nested_list.size());
@@ -210,29 +224,34 @@
     size_t num_elements = flatten_py_list(
             nested_list,
             lengths,
             operations,
             current_indices,
             data_dim_map,
             shape,
+            0,
             0);
 
     // Create the padded array from the shape inferred during `flatten_py_list`
     py::array padded_array = py::array(py::dtype(dtype), shape);
     padded_array[py::make_tuple(py::ellipsis())] = 0;
 
     // Get the strides of the array
     const py::ssize_t *array_strides = padded_array.strides();
     const size_t itemsize = padded_array.itemsize();
 
-    size_t offset = 0;
+    size_t element_size = 1;
+    for (int i = data_dims.size(); i < shape.size(); ++i) {
+        element_size *= shape[i];
+    }
     py::array indexer = py::array(py::dtype::of<int64_t>(), num_elements);
     for (const auto &op: operations) {
         auto indices = std::get<0>(op);
-        auto flat_list = std::get<1>(op);
+        auto element_idx = std::get<1>(op);
+        auto flat_list = std::get<2>(op);
 
         // Byte pointers to elements in the array and the mask
         // Since we cannot know the size of elements in the array (as it's handled
         // dynamically by numpy), we use byte pointers to move around in `padded_array`
         // and will increase the pointer by `itemsize` to move from one element
         // to the next.
 
@@ -241,33 +260,40 @@
         // indexer (which can be used to get the elements position in the padded array).
         size_t begin_byte = 0;
         for (size_t dim = 0; dim < indices.size(); ++dim) {
             // Since mask is boolean, every element is 1 byte, therefore
             // we can use strides to count the number of elements
             begin_byte += array_strides[dim] * indices[dim];
         }
-        size_t begin_idx = begin_byte / itemsize;
+        size_t begin_idx = begin_byte / (itemsize * element_size);
         auto *array_ptr = (char *) padded_array.mutable_data() + begin_byte;
-        auto indexer_ptr = ((int64_t *) indexer.mutable_data()) + offset;
+        int64_t *indexer_ptr;
+        if (element_size > 1) {
+            *(((int64_t *) indexer.mutable_data()) + element_idx) = begin_idx;
+        } else {
+            indexer_ptr = ((int64_t *) indexer.mutable_data()) + element_idx;
+        }
 
         PyObject **items = PySequence_Fast_ITEMS(flat_list);
         const int length = PySequence_Fast_GET_SIZE(flat_list);
         for (int i = 0; i < length; ++i) {
             // Set the element in the array and move to the next element
             // Since array elements can be of any size, we use the element size (in
             // bytes) to move from one element to the next
             PyArray_SETITEM(padded_array.ptr(), array_ptr, items[i]);
             array_ptr += itemsize;
 
             // Assign the current index to the indexer and move to the next element
-            *indexer_ptr = begin_idx + i;
-            indexer_ptr += 1;
+            if (element_size == 1) {
+                *indexer_ptr = begin_idx + i;
+                indexer_ptr += 1;
+            }
         }
+
         Py_DECREF(flat_list);
-        offset += length;
     }
 
     return {padded_array, indexer, lengths};
 }
 
 PYBIND11_MODULE(_C, m) {
     m.def("make_refolding_indexer", &make_refolding_indexer, "Build an indexer to refold data into a different shape");
```

### Comparing `foldedtensor-0.2.2/foldedtensor.egg-info/PKG-INFO` & `foldedtensor-0.3.0/foldedtensor.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedtensor
-Version: 0.2.2
+Version: 0.3.0
 Summary: PyTorch extension for handling deeply nested sequences of variable length
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2023 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -23,16 +23,22 @@
 License-File: LICENSE
 
 <div align="center">
 <p align="center">
   <img src="https://github.com/aphp/foldedtensor/raw/main/banner.png" width="70%">
 </p>
 </div>
+<br/>
 
-----
+---
+
+![Tests](https://img.shields.io/github/actions/workflow/status/aphp/foldedtensor/tests.yml?branch=main&label=tests&style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/foldedtensor?color=blue&style=flat-square)](https://pypi.org/project/foldedtensor/)
+[![Codecov](https://img.shields.io/codecov/c/github/aphp/foldedtensor?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/foldedtensor)
+[![License](https://img.shields.io/github/license/aphp/foldedtensor?color=x&style=flat-square)](https://github.com/aphp/foldedtensor/blob/main/LICENSE)
 
 # FoldedTensor: PyTorch extension for handling deeply nested sequences of variable length
 
 `foldedtensor` is a PyTorch extension that provides efficient handling of tensors containing deeply nested sequences variable sizes. It enables the flattening/unflattening (or unfolding/folding) of data dimensions based on a inner structure of sequence lengths. This library is particularly useful when working with data that can be split in different ways and enables you to avoid choosing a fixed representation.
 
 ## Installation
 
@@ -100,13 +106,13 @@
 ## Comparison with alternatives
 
 Unlike other ragged or nested tensor implementations, a FoldedTensor does not enforce a specific structure on the nested data, and does not require padding all dimensions. This provides the user with greater flexibility when working with data that can be arranged in multiple ways depending on the data transformation. Moreover, the C++ optimization ensures high performance, making it ideal for handling deeply nested tensors efficiently.
 
 Here is a comparison with other common implementations for handling nested sequences of variable length:
 
 | Feature                   | NestedTensor | MaskedTensor | FoldedTensor |
-| ------------------------- | ------------ | ------------ | ------------ |
+|---------------------------|--------------|--------------|--------------|
 | Inner data structure      | Flat         | Padded       | Arbitrary    |
 | Max nesting level         | 1            | 1            | ∞            |
 | From nested python lists  | No           | No           | Yes          |
 | Layout conversion         | To padded    | No           | Any          |
 | Reduction ops w/o padding | Yes          | No           | No           |
```

### Comparing `foldedtensor-0.2.2/pyproject.toml` & `foldedtensor-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.2.2/tests/test_folded_tensor.py` & `foldedtensor-0.3.0/tests/test_folded_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,49 @@
                 [[1, 1], [0, 0], [0, 0], [0, 0], [0, 0]],
             ]
         ).bool()
     ).all()
     assert ft.mask.dtype == torch.bool
 
 
+def test_embedding_from_nested_list():
+    ft = as_folded_tensor(
+        [
+            [[[1, 1, 1]], [], [], [], [[2, 2, 2], [3, 3, 3]]],
+            [[[4, 4, 4], [3, 3, 3]]],
+        ],
+        data_dims=("samples", "lines", "words"),
+        full_names=("samples", "lines", "words"),
+        dtype=torch.long,
+    )
+    assert ft.data.shape == (2, 5, 2, 3)
+    assert ft.lengths == [[2], [5, 1], [1, 0, 0, 0, 2, 2]]
+    assert ft.data_dims == (0, 1, 2)
+    assert ft.full_names == ("samples", "lines", "words")
+    assert (
+        ft.data[..., 0]
+        == torch.tensor(
+            [
+                [[1, 0], [0, 0], [0, 0], [0, 0], [2, 3]],
+                [[4, 3], [0, 0], [0, 0], [0, 0], [0, 0]],
+            ]
+        )
+    ).all()
+    assert (
+        ft.mask
+        == torch.tensor(
+            [
+                [[1, 0], [0, 0], [0, 0], [0, 0], [1, 1]],
+                [[1, 1], [0, 0], [0, 0], [0, 0], [0, 0]],
+            ]
+        ).bool()
+    ).all()
+    assert ft.mask.dtype == torch.bool
+
+
 def test_as_folded_tensor_from_tensor():
     ft = as_folded_tensor(
         torch.tensor(
             [
                 [[1, 0], [0, 0], [0, 0], [0, 0], [2, 3]],
                 [[4, 3], [0, 0], [0, 0], [0, 0], [0, 0]],
             ]
@@ -235,7 +270,42 @@
     embedder = torch.nn.Embedding(10, 16)
     embedding = embedder(ft.refold("words"))
     cat_ft = torch.cat([embedding, embedding], dim=-1)
     assert isinstance(cat_ft, FoldedTensor)
     assert cat_ft.data.shape == (5, 32)
     refolded = cat_ft.refold("samples", "words")
     assert refolded.data.shape == (2, 3, 32)
+
+
+def test_too_deep():
+    with pytest.raises(ValueError) as excinfo:
+        as_folded_tensor(
+            [
+                [0, 1, 2],
+                [3, 4],
+            ],
+            full_names=("sample", "line", "token"),
+            data_dims=("sample", "line", "token"),
+            dtype=torch.long,
+        )
+    assert "nesting" in str(excinfo.value)
+
+
+def test_pad_embedding():
+    ft = as_folded_tensor(
+        [
+            [0, 1, 2],
+            [3, 4],
+        ],
+        full_names=("token",),
+        data_dims=("token",),
+        dtype=torch.long,
+    )
+    assert (
+        ft.data
+        == torch.tensor(
+            [
+                [0, 1, 2],
+                [3, 4, 0],
+            ]
+        )
+    ).all()
```

