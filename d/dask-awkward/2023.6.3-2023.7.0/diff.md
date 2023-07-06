# Comparing `tmp/dask_awkward-2023.6.3.tar.gz` & `tmp/dask_awkward-2023.7.0.tar.gz`

## Comparing `dask_awkward-2023.6.3.tar` & `dask_awkward-2023.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    69121 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    26852 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/README.md
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/pyproject.toml
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 dask_awkward-2023.6.3/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    76062 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    16603 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    28922 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/README.md
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/PKG-INFO
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.7.0/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/typing.py` & `dask_awkward-2023.7.0/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/utils.py` & `dask_awkward-2023.7.0/src/dask_awkward/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Mapping
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
+
+if TYPE_CHECKING:
+    from dask_awkward.lib.core import Array
+
 
 T = TypeVar("T")
 
 
 class DaskAwkwardNotImplemented(NotImplementedError):
     NOT_SUPPORTED_MSG = """
 
@@ -15,33 +19,33 @@
 
     def __init__(self, msg: str | None = None) -> None:
         msg = f"{msg or ''}{self.NOT_SUPPORTED_MSG}"
         super().__init__(msg)
 
 
 class IncompatiblePartitions(ValueError):
-    def __init__(self, name, *args):
+    def __init__(self, name: str, *args: Array) -> None:
         msg = self.divisions_msg(name, *args)
         super().__init__(msg)
 
     @staticmethod
-    def divisions_msg(name: str, *args: Any) -> str:
+    def divisions_msg(name: str, *args: Array) -> str:
         msg = f"The inputs to {name} are incompatibly partitioned\n"
         for i, arg in enumerate(args):
             msg += f"- arg{i} divisions: {arg.divisions}\n"
         return msg
 
 
 class LazyInputsDict(Mapping):
     """Dictionary with lazy key value pairs
 
     Parameters
     ----------
     inputs : list[Any]
-        The list of dicionary values.
+        The list of dictionary values.
 
     """
 
     def __init__(self, inputs: list[Any], **kwargs: Any) -> None:
         self.inputs = inputs
         self.kwargs = kwargs
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.7.0/src/dask_awkward/layers/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from awkward.typetracer import TypeTracerReport
 
 
 class AwkwardBlockwiseLayer(Blockwise):
     """Just like upstream Blockwise, except we override pickling"""
 
     @classmethod
-    def from_blockwise(cls, layer) -> AwkwardBlockwiseLayer:
+    def from_blockwise(cls, layer: Blockwise) -> AwkwardBlockwiseLayer:
         ob = object.__new__(cls)
         ob.__dict__.update(layer.__dict__)
         return ob
 
     def mock(self) -> tuple[AwkwardBlockwiseLayer, Any | None]:
         layer = copy.copy(self)
         nb = layer.numblocks
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from dask_awkward.lib.core import Array, Record, Scalar
+from dask_awkward.lib.core import Array, PartitionCompatibility, Record, Scalar
 from dask_awkward.lib.core import _type as type
-from dask_awkward.lib.core import map_partitions, typetracer_from_form
+from dask_awkward.lib.core import (
+    compatible_partitions,
+    map_partitions,
+    partition_compatibility,
+    typetracer_from_form,
+)
 from dask_awkward.lib.describe import fields
 from dask_awkward.lib.inspect import necessary_columns, sample
 from dask_awkward.lib.io.io import (
     ImplementsFormTransformation,
     from_awkward,
     from_dask_array,
     from_delayed,
@@ -43,14 +48,15 @@
     argcartesian,
     argcombinations,
     argsort,
     broadcast_arrays,
     cartesian,
     combinations,
     copy,
+    drop_none,
     fill_none,
     firsts,
     flatten,
     from_regular,
     full_like,
     is_none,
     isclose,
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/core.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import keyword
 import logging
 import math
 import operator
 import sys
 import warnings
 from collections.abc import Callable, Hashable, Mapping, Sequence
+from enum import IntEnum
 from functools import cached_property, partial
 from numbers import Number
-from typing import TYPE_CHECKING, Any, Literal, TypeVar, overload
+from typing import TYPE_CHECKING, Any, Literal, TypeVar, Union, overload
 
 import awkward as ak
 import dask.config
 import numpy as np
 from awkward._nplikes.typetracer import (
     MaybeNone,
     OneOf,
@@ -31,15 +32,15 @@
 )
 from dask.blockwise import BlockwiseDep
 from dask.blockwise import blockwise as dask_blockwise
 from dask.context import globalmethod
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as threaded_get
-from dask.utils import IndexCallable, funcname, key_split
+from dask.utils import IndexCallable, funcname, is_arraylike, key_split
 from tlz import first
 
 from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardMaterializedLayer
 from dask_awkward.lib.optimize import all_optimizations
 from dask_awkward.typing import AwkwardDaskCollection
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
@@ -72,15 +73,15 @@
 
     # a sequence of arrays that need to be concatenated.
     elif any(isinstance(r, ak.Array) for r in results):
         return ak.concatenate(results)
 
     # sometimes we just check the length of partitions so all results
     # will be integers, just make an array out of that.
-    elif isinstance(results, tuple) and all(
+    elif isinstance(results, (tuple, list)) and all(
         isinstance(r, (int, np.integer)) for r in results
     ):
         return ak.Array(list(results))
 
     # sometimes all partition results will be None (some write-to-disk
     # operations)
     elif all(r is None for r in results):
@@ -556,14 +557,48 @@
             raise ValueError("rename= unsupported in dask-awkward")
         return Array(dsk, name, self._meta, divisions=self.divisions)
 
     def reset_meta(self) -> None:
         """Assign an empty typetracer array as the collection metadata."""
         self._meta = empty_typetracer()
 
+    def repartition(self, npartitions=None, divisions=None, rows_per_partition=None):
+        from dask_awkward.layers import AwkwardMaterializedLayer
+        from dask_awkward.lib.structure import repartition_layer
+
+        if sum(bool(_) for _ in [npartitions, divisions, rows_per_partition]) != 1:
+            raise ValueError("Please specify exactly one of the inputs")
+        if not self.known_divisions:
+            self.eager_compute_divisions()
+        nrows = self.divisions[-1]
+        if npartitions:
+            rows_per_partition = math.ceil(nrows / npartitions)
+        if rows_per_partition:
+            divisions = list(range(0, nrows, rows_per_partition))
+            divisions.append(nrows)
+
+        token = tokenize(self, divisions)
+        key = f"repartition-{token}"
+
+        new_layer_raw = repartition_layer(self, key, divisions)
+        new_layer = AwkwardMaterializedLayer(
+            new_layer_raw,
+            previous_layer_names=[self.name],
+        )
+        new_graph = HighLevelGraph.from_collections(
+            key, new_layer, dependencies=(self,)
+        )
+        return new_array_object(
+            new_graph,
+            key,
+            meta=self._meta,
+            behavior=self.behavior,
+            divisions=divisions,
+        )
+
     def __len__(self) -> int:
         if not self.known_divisions:
             self.eager_compute_divisions()
         return self.divisions[-1]  # type: ignore
 
     def _shorttypestr(self, max: int = 10) -> str:
         return str(_type(self))[0:max]
@@ -696,14 +731,15 @@
 
     @cached_property
     def keys_array(self) -> np.ndarray:
         """NumPy array of task graph keys."""
         return np.array(self.__dask_keys__(), dtype=object)
 
     def _partitions(self, index: Any) -> Array:
+        # TODO: this produces a materialized layer, but could work like repartition() and slice()
         if not isinstance(index, tuple):
             index = (index,)
         token = tokenize(self, index)
         from dask.array.slicing import normalize_index
 
         raw = normalize_index(index, (self.npartitions,))
         index = tuple(slice(k, k + 1) if isinstance(k, Number) else k for k in raw)  # type: ignore
@@ -714,14 +750,15 @@
             name,
             AwkwardMaterializedLayer(dsk, previous_layer_names=[self.name]),
             dependencies=(self,),
         )
 
         # if a single partition was requested we trivially know the new divisions.
         if len(raw) == 1 and isinstance(raw[0], int) and self.known_divisions:
+            # TODO: don't we always know the divisions?
             new_divisions = (
                 0,
                 self.divisions[raw[0] + 1] - self.divisions[raw[0]],  # type: ignore
             )
         # otherwise nullify the known divisions
         else:
             new_divisions = (None,) * (len(new_keys) + 1)  # type: ignore
@@ -778,15 +815,15 @@
             label=label,
         )
 
     def _getitem_outer_bool_or_int_lazy_array(
         self, where: Array | tuple[Any, ...]
     ) -> Any:
         ba = where if isinstance(where, Array) else where[0]
-        if not compatible_partitions(self, ba):
+        if partition_compatibility(self, ba) == PartitionCompatibility.NO:
             raise IncompatiblePartitions("getitem", self, ba)
 
         new_meta: Any | None = None
         if self._meta is not None:
             if isinstance(where, tuple):
                 raise DaskAwkwardNotImplemented(
                     "tuple style input boolean/int selection is not supported."
@@ -1202,46 +1239,43 @@
         """Force a compute of the divisions."""
         self._divisions = calculate_known_divisions(self)
 
     def clear_divisions(self) -> None:
         """Clear the divisions of a Dask Awkward Collection."""
         self._divisions = (None,) * (self.npartitions + 1)
 
-    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
-        if method != "__call__":
-            raise RuntimeError("Array ufunc supports only method == '__call__'")
+    def __awkward_function__(self, func, array_likes, args, kwargs):
+        import dask_awkward
 
-        new_meta = None
+        if any(isinstance(arg, ak.Array) for arg in array_likes):
+            raise TypeError("cannot mix awkward.Array and dask_awkward.Array")
 
-        # divisions need to be compat. (identical for now?)
+        fn_name = func.__qualname__
+        try:
+            fn = getattr(dask_awkward, fn_name)
+        except AttributeError:
+            return NotImplemented
+        return fn(*args, **kwargs)
 
-        inputs_meta = []
-        for inp in inputs:
-            # if input is a Dask Awkward Array collection, grab it's meta
-            if isinstance(inp, Array):
-                inputs_meta.append(inp._meta)
-            # if input is a concrete Awkward Array, grab it's typetracer
-            elif isinstance(inp, ak.Array):
-                inputs_meta.append(typetracer_array(inp))
-            # otherwise pass along
-            else:
-                inputs_meta.append(inp)
+    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+        if method != "__call__":
+            raise RuntimeError("Array ufunc supports only method == '__call__'")
 
-        # compute new meta from inputs
-        new_meta = ufunc(*inputs_meta)
+        dak_arrays = tuple(a for a in inputs if isinstance(a, Array))
+        if partition_compatibility(*dak_arrays) == PartitionCompatibility.NO:
+            raise IncompatiblePartitions(*dak_arrays)
 
         return map_partitions(
             ufunc,
             *inputs,
-            meta=new_meta,
             output_divisions=1,
             **kwargs,
         )
 
-    def __array__(self, *args, **kwargs):
+    def __array__(self, *_, **__):
         raise NotImplementedError
 
     def to_delayed(self, optimize_graph: bool = True) -> list[Delayed]:
         """Convert the collection to a list of delayed objects.
 
         One dask.delayed.Delayed object per partition.
 
@@ -1433,14 +1467,17 @@
             pairs.extend([arg.name, "i"])
             numblocks[arg.name] = (arg.npartitions,)
         elif isinstance(arg, BlockwiseDep):
             if len(arg.numblocks) == 1:
                 pairs.extend([arg, "i"])
             elif len(arg.numblocks) == 2:
                 pairs.extend([arg, "ij"])
+        elif is_arraylike(arg) and is_dask_collection(arg) and arg.ndim == 1:
+            pairs.extend([arg.name, "i"])
+            numblocks[arg.name] = arg.numblocks
         elif is_dask_collection(arg):
             raise DaskAwkwardNotImplemented(
                 "Use of Array with other Dask collections is currently unsupported."
             )
         else:
             pairs.extend([arg, None])
     layer = dask_blockwise(
@@ -1941,14 +1978,18 @@
     5
     >>> meta_or_identity("foo")
     'foo'
 
     """
     if is_awkward_collection(obj):
         return obj._meta
+    elif is_dask_collection(obj) and is_arraylike(obj):
+        return ak.Array(
+            ak.from_numpy(obj._meta).layout.to_typetracer(forget_length=True)
+        )
     return obj
 
 
 @overload
 def to_meta(objects: Sequence[Any]) -> tuple[Any, ...]:
     ...
 
@@ -1987,15 +2028,15 @@
     return obj
 
 
 def to_length_zero_arrays(objects: Sequence[Any]) -> tuple[Any, ...]:
     return tuple(map(length_zero_array_or_identity, objects))
 
 
-def map_meta(fn: Callable, *deps: Any) -> ak.Array | None:
+def map_meta(fn: ArgsKwargsPackedFunction, *deps: Any) -> ak.Array | None:
     # NOTE: fn is assumed to be a *packed* function
     #       as defined up in map_partitions. be careful!
     try:
         meta = fn(*to_meta(deps))
         return meta
     except Exception as err:
         # if compute-unknown-meta is False then we don't care about
@@ -2059,49 +2100,14 @@
         msg = (
             "`a` should be an awkward array or a Dask awkward collection.\n"
             f"Got type {type(a)}"
         )
         raise TypeError(msg)
 
 
-def compatible_partitions(*args: Array) -> bool:
-    """Check if all arguments are compatibly partitioned.
-
-    In operations where the blocks of multiple collections are used
-    simultaneously, we need the collections to be equally partitioned.
-    If the first argument has known divisions, other collections with
-    known divisions will be tested against the first arguments
-    divisions.
-
-    Parameters
-    ----------
-    *args : Array
-        Array collections of interest.
-
-    Returns
-    -------
-    bool
-        ``True`` if the collections appear to be equally partitioned.
-
-    """
-    a = args[0]
-
-    for arg in args[1:]:
-        if a.npartitions != arg.npartitions:
-            return False
-
-    if a.known_divisions:
-        for arg in args[1:]:
-            if arg.known_divisions:
-                if a.divisions != arg.divisions:
-                    return False
-
-    return True
-
-
 def empty_typetracer() -> ak.Array:
     """Instantiate a typetracer array with unknown length.
 
     Returns
     -------
     ak.Array
         Length-less typetracer array (content-less array).
@@ -2197,7 +2203,182 @@
     Returns
     -------
     ak.Array
         Highlevel typetracer Array with unknown length.
 
     """
     return ak.Array(ak.to_layout(array).to_typetracer(forget_length=True))
+
+
+class PartitionCompatibility(IntEnum):
+    """Sum type for describing partition compatibility.
+
+    Use the :func:`partition_compatibility` function as an entry point
+    to instances of this class.
+
+    Attributes
+    ----------
+    NO
+        The compatibility is absolutely false; either an unequal
+        number of partitions or known divisions do not match
+    MAYBE
+        The compatibility is possible; the total number of partitions
+        are equal but some divisions are unknown so therefore it's
+        possible that partitions are not compatible, but this cannot
+        be determined without some compute.
+    YES
+        The compatibility is absolutely true; equal number of
+        partitions and known divisions match.
+
+    See Also
+    --------
+    dask_awkward.partition_compatibility
+
+    """
+
+    NO = 0
+    MAYBE = 1
+    YES = 2
+
+    @staticmethod
+    def _check(*args: Array) -> PartitionCompatibility:
+        # first check to see if all arguments have the same number of
+        # partitions; this is _always_ defined.
+        for arg in args[1:]:
+            if args[0].npartitions != arg.npartitions:
+                return PartitionCompatibility.NO
+
+        # now we check if divisions are compatible. Sometimes divisions
+        # are unknown and we just have a tuple of Nones; but if divisions
+        # are known we want to check if they are compatible.
+        refarr: Array | None = None
+        for arg in args:
+            if arg.known_divisions:
+                refarr = arg
+                break
+        # if we never hit the break just return True because we have no
+        # known division Arrays.
+        else:
+            return PartitionCompatibility.MAYBE
+
+        # at this point we have a reference array to compare divisions
+        ngood = 0
+        for arg in args:
+            if arg.known_divisions:
+                if arg.divisions != refarr.divisions:
+                    return PartitionCompatibility.NO
+                else:
+                    ngood += 1
+
+        # the ngood counter tells us if all divisions were present and are equal
+        if ngood == len(args):
+            return PartitionCompatibility.YES
+
+        # if ngood is less than len(args) then we fall back on maybe compatible
+        return PartitionCompatibility.MAYBE
+
+
+def partition_compatibility(*args: Array) -> PartitionCompatibility:
+    """Check if multiple collections have compatible partitions.
+
+    Parameters
+    ----------
+    *args : Array
+        Any number of array collections to check.
+
+    Returns
+    -------
+    PartitionCompatibility
+        Result of the check.
+
+    Examples
+    --------
+
+    Starting with an absolutely compatible comparison:
+
+    >>> import dask_awkward as dak
+    >>> import awkward as ak
+    >>> concrete = ak.Array([[1, 2, 3], [4], [5, 6], [0, 0, 0, 0]])
+    >>> lazy = dak.from_awkward(concrete npartitions=2)
+    >>> selection = dak.sum(lazy, axis=1) == 0
+    >>> dak.partition_compatibility(lazy, selection)
+    <PartitionCompatibility.YES: 0>
+
+    The selection doesn't change the length of the arrays at each
+    partition, so the divisions are known to be conserved for those
+    operations (the sum on ``axis=1`` along with the equality
+    comparison).
+
+    In general we have no way of knowing what the resulting divisions
+    will be after a boolean selection, but the total number of
+    partitions will be conserved, so we have to report ``MAYBE``:
+
+    >>> selected_lazy = lazy[selection]
+    >>> dak.partition_compatibility(lazy, lazy_selection)
+    <PartitionCompatibility.MAYBE: 2>
+
+    Due the simple nature of this example we know that after the
+    selection the partitions will not be compatible (because it's
+    clear only 1 element of the original array will survive the
+    selection, so the divisions will change after that compute). Now
+    we can eagerly compute what the divisions will be on the
+    ``lazy_selection`` collection and get a ``NO`` result:
+
+    >>> lazy_selection.eager_compute_divisions()
+    >>> dak.partition_compatibility(lazy, lazy_selection)
+    <PartitionCompatibility.NO: 1>
+
+    Remember that :func:`Array.eager_compute_divisions` is going to
+    trigger a compute to determine the divisions (to know divisions we
+    need to know the length of each partition)
+
+    """
+    return PartitionCompatibility._check(*args)
+
+
+HowStrictT = Union[Literal[1], Literal[2], PartitionCompatibility]
+
+
+def compatible_partitions(
+    *args: Array,
+    how_strict: HowStrictT = PartitionCompatibility.MAYBE,
+) -> bool:
+    """Check if all arguments are compatibly partitioned.
+
+    In operations where the blocks of multiple collections are used
+    simultaneously, we need the collections to be equally partitioned.
+    If the first argument has known divisions, other collections with
+    known divisions will be tested against the first arguments
+    divisions.
+
+    Parameters
+    ----------
+    *args : Array
+        Array collections of interest.
+    how_strict : PartitionCompatibility or Literal[1] or Literal[2]
+        Strictness level for the compatibility. If
+        ``PartitionCompatbility.MAYBE`` or the integer 1, the check
+        will return ``True`` if the arrays are maybe compatible (that
+        is, some unknown divisions exist but the total number of
+        partitions are compatible). If ``PartitionCompatibility.YES``
+        or the integer 2, the check will return ``True`` if and only
+        if the arrays are absolutely compatible (that is, all
+        divisions are known and they are equal).
+
+    Returns
+    -------
+    bool
+        ``True`` if the collections have compatible partitions at the
+        level of requested strictness.
+
+    See Also
+    --------
+    dask_awkward.PartitionCompatibility
+    dask_awkward.partition_compatibility
+
+    """
+    partcomp = partition_compatibility(*args)
+    if partcomp == PartitionCompatibility.NO:
+        return False
+    elif partcomp == PartitionCompatibility.MAYBE:
+        return how_strict == 1
+    return True
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import awkward as ak
 from dask.base import tokenize
 from dask.highlevelgraph import HighLevelGraph
 
 from dask_awkward.layers import AwkwardMaterializedLayer
 from dask_awkward.lib.core import (
     Array,
-    compatible_partitions,
+    PartitionCompatibility,
     map_partitions,
     new_array_object,
+    partition_compatibility,
 )
 from dask_awkward.utils import DaskAwkwardNotImplemented, IncompatiblePartitions
 
 
 class _ConcatenateFnAxisGT0:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
@@ -56,15 +57,15 @@
             previous_layer_names=prev_names,
             fn=_concatenate_axis0_multiarg,
         )
         hlg = HighLevelGraph.from_collections(name, g, dependencies=arrays)
         return new_array_object(hlg, name, meta=meta, npartitions=npartitions)
 
     if axis > 0:
-        if not compatible_partitions(*arrays):
+        if partition_compatibility(*arrays) == PartitionCompatibility.NO:
             raise IncompatiblePartitions("concatenate", *arrays)
 
         fn = _ConcatenateFnAxisGT0(axis=axis)
         return map_partitions(fn, *arrays)
 
     else:
         raise DaskAwkwardNotImplemented("TODO")
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -345,14 +345,16 @@
     if not _has_projectable_awkward_io_layer(dsk):
         return {}
 
     import awkward as ak
 
     layers = dsk.layers.copy()  # type: ignore
     deps = dsk.dependencies.copy()  # type: ignore
+    dependents = dsk.dependents
+
     reports = {}
 
     # make labelled report
     projectable = _projectable_input_layer_names(dsk)
     for name, lay in dsk.layers.copy().items():
         if name in projectable:
             layers[name], report = lay.mock()
@@ -363,20 +365,38 @@
     for name in _ak_output_layer_names(dsk):
         layers[name] = _mock_output(layers[name])
 
     for name in _opt_touch_all_layer_names(dsk):
         layers[name] = _touch_and_call(layers[name])
 
     hlg = HighLevelGraph(layers, deps)
-    outlayer = hlg.layers[hlg._toposort_layers()[-1]]
 
+    # this loop builds up what are the possible final leaf nodes by
+    # inspecting the dependents dictionary. If something does not have
+    # a dependent, it must be the end of a graph. These are the things
+    # we need to compute for; we only use a single partition (the
+    # first). for a single collection `.compute()` this list will just
+    # be length 1; but if we are using `dask.compute` to pass in
+    # multiple collections to be computed simultaneously, this list
+    # will increase in length.
+    leaf_layers_keys = [
+        (k, 0) for k, v in dependents.items() if isinstance(v, set) and len(v) == 0
+    ]
+
+    # now we try to compute for each possible output layer key (leaf
+    # node on partition 0); this will cause the typetacer reports to
+    # get correct fields/columns touched. If the result is a record or
+    # an array we of course want to touch all of the data/fields.
     try:
         for layer in hlg.layers.values():
             layer.__dict__.pop("_cached_dict", None)
-        out = get_sync(hlg, list(outlayer.keys())[0])
+        for outlayerkey in leaf_layers_keys:
+            out = get_sync(hlg, outlayerkey)
+            if isinstance(out, (ak.Array, ak.Record)):
+                out.layout._touch_data(recursive=True)
     except Exception as err:
         on_fail = dask.config.get("awkward.optimization.on-fail")
         # this is the default, throw a warning but skip the optimization.
         if on_fail == "warn":
             warnings.warn(
                 COLUMN_OPT_FAILED_WARNING_MSG.format(exception=type(err), message=err)
             )
@@ -390,16 +410,14 @@
             raise
         else:
             raise ValueError(
                 f"Invalid awkward.optimization.on-fail option: {on_fail}.\n"
                 "Valid options are 'warn', 'pass', or 'raise'."
             )
 
-    if isinstance(out, (ak.Array, ak.Record)):
-        out.layout._touch_data(recursive=True)
     return reports
 
 
 def _necessary_columns(dsk: HighLevelGraph) -> dict[str, list[str]]:
     """Pair layer names with lists of necessary columns."""
     kv = {}
     for name, report in _get_column_reports(dsk).items():
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 from collections.abc import Sequence
 from numbers import Number
 from typing import TYPE_CHECKING, Any
 
 import awkward as ak
 from dask.base import is_dask_collection
 
-from dask_awkward.lib.core import Array, compatible_partitions, map_partitions
+from dask_awkward.lib.core import (
+    Array,
+    PartitionCompatibility,
+    map_partitions,
+    partition_compatibility,
+)
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     borrow_docstring,
 )
 
 if TYPE_CHECKING:
@@ -25,14 +30,15 @@
     "argcartesian",
     "argcombinations",
     "argsort",
     "broadcast_arrays",
     "cartesian",
     "combinations",
     "copy",
+    "drop_none",
     "fill_none",
     "firsts",
     "flatten",
     "from_regular",
     "full_like",
     "isclose",
     "is_none",
@@ -196,15 +202,15 @@
 
 
 @borrow_docstring(ak.broadcast_arrays)
 def broadcast_arrays(*arrays, highlevel=True, **kwargs):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
-    if not compatible_partitions(*arrays):
+    if partition_compatibility(*arrays) == PartitionCompatibility.NO:
         raise IncompatiblePartitions("broadcast_arrays", *arrays)
 
     array_metas = (array._meta for array in arrays)
 
     metas = ak.broadcast_arrays(*array_metas, highlevel=highlevel, **kwargs)
 
     # here we return the list of broadcasted arrays
@@ -330,14 +336,36 @@
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
     fn = _FillNoneFn(value, axis=axis, highlevel=highlevel, behavior=behavior)
     return map_partitions(fn, array, label="fill-none", output_divisions=1)
 
 
+class _DropNoneFn:
+    def __init__(self, **kwargs):
+        self.kwargs = kwargs
+
+    def __call__(self, arr):
+        return ak.drop_none(arr, **self.kwargs)
+
+
+@borrow_docstring(ak.drop_none)
+def drop_none(
+    array: Array,
+    axis: int | None = None,
+    highlevel: bool = True,
+    behavior: dict | None = None,
+) -> Array:
+    if not highlevel:
+        raise ValueError("Only highlevel=True is supported")
+
+    fn = _DropNoneFn(axis=axis, highlevel=highlevel, behavior=behavior)
+    return map_partitions(fn, array, label="drop-none", output_divisions=1)
+
+
 class _FirstsFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, array):
         return ak.firsts(array, **self.kwargs)
 
@@ -427,37 +455,39 @@
     return map_partitions(
         ak.full_like,
         array,
         fill_value,
         highlevel=highlevel,
         behavior=behavior,
         dtype=dtype,
+        output_divisions=1,
     )
 
 
 @borrow_docstring(ak.isclose)
 def isclose(
     a, b, rtol=1e-05, atol=1e-08, equal_nan=False, highlevel=True, behavior=None
 ):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
 
-    if not compatible_partitions(a, b):
+    if partition_compatibility(a, b) == PartitionCompatibility.NO:
         raise IncompatiblePartitions("isclose", a, b)
 
     return map_partitions(
         ak.isclose,
         a,
         b,
         rtol=rtol,
         atol=atol,
         equal_nan=equal_nan,
         highlevel=highlevel,
         behavior=behavior,
         label="is-close",
+        output_divisions=1,
     )
 
 
 class _IsNoneFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
@@ -485,15 +515,15 @@
             highlevel=highlevel,
             behavior=behavior,
         )
 
 
 @borrow_docstring(ak.mask)
 def mask(array, mask, valid_when=True, highlevel=True, behavior=None):
-    if not compatible_partitions(array, mask):
+    if partition_compatibility(array, mask) == PartitionCompatibility.NO:
         raise IncompatiblePartitions("mask", array, mask)
     return map_partitions(
         ak.mask,
         array,
         mask,
         valid_when=valid_when,
         highlevel=highlevel,
@@ -537,14 +567,15 @@
     if axis and axis != 0:
         return map_partitions(
             ak.num,
             array,
             axis=axis,
             highlevel=highlevel,
             behavior=behavior,
+            output_divisions=1,
         )
     if axis == 0:
         return len(array)
     raise DaskAwkwardNotImplemented("TODO")
 
 
 @borrow_docstring(ak.ones_like)
@@ -555,18 +586,18 @@
     dtype: DTypeLike | None = None,
 ) -> Array:
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
     return map_partitions(
         ak.ones_like,
         array,
-        output_divisions=1,
         label="ones-like",
         behavior=behavior,
         dtype=dtype,
+        output_divisions=1,
     )
 
 
 @borrow_docstring(ak.to_packed)
 def to_packed(array, highlevel=True, behavior=None):
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
@@ -811,15 +842,15 @@
     dask_args = tuple(arg for arg in maybe_dask_args if is_dask_collection(arg))
 
     if not isinstance(condition, Array):
         raise ValueError(
             "The condition argugment to where must be a dask_awkward.Array"
         )
 
-    if not compatible_partitions(*dask_args):
+    if partition_compatibility(*dask_args) == PartitionCompatibility.NO:
         raise IncompatiblePartitions("where", *dask_args)
 
     return map_partitions(
         _WhereFn(mergebool=mergebool, highlevel=highlevel, behavior=behavior),
         condition,
         x,
         y,
@@ -860,16 +891,16 @@
         raise ValueError(
             "with_field cannot accept string, bytes, list, or dict values yet"
         )
 
     maybe_dask_args = [base, what]
     dask_args = tuple(arg for arg in maybe_dask_args if is_dask_collection(arg))
 
-    if not compatible_partitions(*dask_args):
-        raise IncompatiblePartitions("with_field", base, what)
+    if partition_compatibility(*dask_args) == PartitionCompatibility.NO:
+        raise IncompatiblePartitions("with_field", *dask_args)
     return map_partitions(
         _WithFieldFn(where=where, highlevel=highlevel, behavior=behavior),
         base,
         what,
         label="with-field",
         output_divisions=1,
     )
@@ -963,18 +994,18 @@
     dtype: DTypeLike | None = None,
 ) -> Array:
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
     return map_partitions(
         ak.zeros_like,
         array,
-        output_divisions=1,
         label="zeros-like",
         behavior=behavior,
         dtype=dtype,
+        output_divisions=1,
     )
 
 
 class _ZipDictInputFn:
     def __init__(self, keys: Sequence[str], **kwargs: Any) -> None:
         self.keys = keys
         self.kwargs = kwargs
@@ -1059,7 +1090,55 @@
             label="zip",
         )
 
     else:
         raise DaskAwkwardNotImplemented(
             "only sized iterables are supported by dak.zip (dict, list, or tuple)"
         )
+
+
+def _repartition_func(*stuff):
+    import builtins
+
+    import awkward as ak
+
+    *data, slices = stuff
+    data = [
+        d[sl[0] : sl[1]] if sl is not None else d
+        for d, sl in builtins.zip(data, slices)
+    ]
+    return ak.concatenate(data)
+
+
+def repartition_layer(arr: Array, key: str, divisions: list[int, ...]):
+    layer = {}
+
+    indivs = arr.divisions
+    i = 0
+    for index, (start, end) in enumerate(builtins.zip(divisions[:-1], divisions[1:])):
+        pp = []
+        ss = []
+        while indivs[i] <= start:
+            i += 1
+        j = i
+        i -= 1
+        while indivs[j] < end:
+            j += 1
+        for k in range(i, j):
+            if start < indivs[k]:
+                st = None
+            elif start < indivs[k + 1]:
+                st = start - indivs[k]
+            else:
+                continue
+            if end < indivs[k]:
+                continue
+            elif end < indivs[k + 1]:
+                en = end - indivs[k]
+            else:
+                en = None
+            pp.append(k)
+            ss.append((st, en))
+        layer[(key, index)] = (
+            (_repartition_func,) + tuple((arr.name, part) for part in pp) + (ss,)
+        )
+    return layer
```

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/unproject_layout.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.7.0/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/.gitignore` & `dask_awkward-2023.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/LICENSE` & `dask_awkward-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/README.md` & `dask_awkward-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.3/pyproject.toml` & `dask_awkward-2023.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,46 +23,42 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "awkward >=2.2.2",
+  "awkward >=2.2.4",
   "dask >=2023.04.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
 
 [project.optional-dependencies]
 io = [
   "aiohttp",
   "pyarrow",
 ]
 complete = [
-  "aiohttp",
-  "pyarrow",
+  "dask-awkward[io]",
 ]
 # `docs` and `test` are separate from user installs
 docs = [
+  "dask-awkard[complete]",
   "dask-sphinx-theme >=3.0.2",
-  "pyarrow",
   "sphinx-design",
-  "pytest >=6.0",
-  "pytest-cov >=3.0.0",
   "requests >=2.27.1",
 ]
 test = [
-  "aiohttp",
+  "dask-awkward[complete]",
   "distributed",
   "pandas",
-  "pyarrow",
   "pytest >=6.0",
   "pytest-cov >=3.0.0",
   "requests >=2.27.1",
 ]
 
 [project.entry-points."dask.sizeof"]
 awkward = "dask_awkward.sizeof:register"
```

### Comparing `dask_awkward-2023.6.3/PKG-INFO` & `dask_awkward-2023.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.6.3
+Version: 2023.7.0
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,34 +13,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.2.2
+Requires-Dist: awkward>=2.2.4
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
-Requires-Dist: aiohttp; extra == 'complete'
-Requires-Dist: pyarrow; extra == 'complete'
+Requires-Dist: dask-awkward[io]; extra == 'complete'
 Provides-Extra: docs
+Requires-Dist: dask-awkard[complete]; extra == 'docs'
 Requires-Dist: dask-sphinx-theme>=3.0.2; extra == 'docs'
-Requires-Dist: pyarrow; extra == 'docs'
-Requires-Dist: pytest-cov>=3.0.0; extra == 'docs'
-Requires-Dist: pytest>=6.0; extra == 'docs'
 Requires-Dist: requests>=2.27.1; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Provides-Extra: io
 Requires-Dist: aiohttp; extra == 'io'
 Requires-Dist: pyarrow; extra == 'io'
 Provides-Extra: test
-Requires-Dist: aiohttp; extra == 'test'
+Requires-Dist: dask-awkward[complete]; extra == 'test'
 Requires-Dist: distributed; extra == 'test'
 Requires-Dist: pandas; extra == 'test'
-Requires-Dist: pyarrow; extra == 'test'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Requires-Dist: requests>=2.27.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 dask-awkward
 ============
```

