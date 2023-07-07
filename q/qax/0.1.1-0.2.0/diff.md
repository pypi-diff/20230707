# Comparing `tmp/qax-0.1.1.tar.gz` & `tmp/qax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qax-0.1.1.tar", max compression
+gzip compressed data, was "qax-0.2.0.tar", max compression
```

## Comparing `qax-0.1.1.tar` & `qax-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-06-08 20:47:12.247149 qax-0.1.1/LICENSE
--rw-r--r--   0        0        0    18302 2023-06-22 23:21:33.376187 qax-0.1.1/README.md
--rw-r--r--   0        0        0      510 2023-06-22 23:15:39.106185 qax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      206 2023-06-22 23:12:31.506184 qax-0.1.1/qax/__init__.py
--rw-r--r--   0        0        0     1614 2023-06-20 23:31:51.135379 qax-0.1.1/qax/constants.py
--rw-r--r--   0        0        0    16469 2023-06-22 23:20:50.242853 qax-0.1.1/qax/implicit_array.py
--rw-r--r--   0        0        0     1453 2023-06-21 05:01:53.078806 qax-0.1.1/qax/primitives.py
--rw-r--r--   0        0        0       47 2023-06-11 06:41:11.698121 qax-0.1.1/qax/quantization/__init__.py
--rw-r--r--   0        0        0     1069 2023-06-11 06:41:11.698121 qax-0.1.1/qax/quantization/pack.py
--rw-r--r--   0        0        0     2944 2023-06-11 06:41:11.698121 qax-0.1.1/qax/quantization/quant_utils.py
--rw-r--r--   0        0        0     1694 2023-06-11 06:41:11.698121 qax-0.1.1/qax/quantization/quantized_matrix.py
--rw-r--r--   0        0        0     1089 2023-06-11 06:41:11.698121 qax-0.1.1/qax/tracer.py
--rw-r--r--   0        0        0     9508 2023-06-22 23:17:19.179519 qax-0.1.1/qax/utils.py
--rw-r--r--   0        0        0    18921 1970-01-01 00:00:00.000000 qax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-08 20:47:12.247149 qax-0.2.0/LICENSE
+-rw-r--r--   0        0        0    17645 2023-07-07 07:18:08.791979 qax-0.2.0/README.md
+-rw-r--r--   0        0        0      510 2023-07-07 07:19:58.518646 qax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-07-07 03:27:51.361914 qax-0.2.0/qax/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-25 23:40:04.084072 qax-0.2.0/qax/common/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-25 05:10:00.853760 qax-0.2.0/qax/common/type_utils.py
+-rw-r--r--   0        0        0     3594 2023-07-06 20:35:25.445132 qax-0.2.0/qax/common/utils.py
+-rw-r--r--   0        0        0     1614 2023-06-25 19:57:29.517343 qax-0.2.0/qax/constants.py
+-rw-r--r--   0        0        0        0 2023-06-25 23:36:00.000738 qax-0.2.0/qax/implicit/__init__.py
+-rw-r--r--   0        0        0    16822 2023-06-25 23:54:33.850743 qax-0.2.0/qax/implicit/implicit_array.py
+-rw-r--r--   0        0        0     7530 2023-06-25 23:44:36.620740 qax-0.2.0/qax/implicit/implicit_utils.py
+-rw-r--r--   0        0        0     5000 2023-06-25 07:31:02.103799 qax-0.2.0/qax/old_symbols.py
+-rw-r--r--   0        0        0     1436 2023-06-25 05:43:35.367103 qax-0.2.0/qax/primitives.py
+-rw-r--r--   0        0        0       47 2023-06-11 06:41:11.698121 qax-0.2.0/qax/quantization/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-11 06:41:11.698121 qax-0.2.0/qax/quantization/pack.py
+-rw-r--r--   0        0        0     2944 2023-06-11 06:41:11.698121 qax-0.2.0/qax/quantization/quant_utils.py
+-rw-r--r--   0        0        0     1694 2023-06-11 06:41:11.698121 qax-0.2.0/qax/quantization/quantized_matrix.py
+-rw-r--r--   0        0        0     6534 2023-07-07 03:28:50.545248 qax-0.2.0/qax/symbols.py
+-rw-r--r--   0        0        0     1089 2023-06-11 06:41:11.698121 qax-0.2.0/qax/tracer.py
+-rw-r--r--   0        0        0       67 2023-07-07 03:29:41.718581 qax-0.2.0/qax/utils.py
+-rw-r--r--   0        0        0    18264 1970-01-01 00:00:00.000000 qax-0.2.0/PKG-INFO
```

### Comparing `qax-0.1.1/LICENSE` & `qax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/README.md` & `qax-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/davisyoshida/qax/blob/master/examples/How_to_Qax.ipynb)
+
 # Qax: If it quacks like a tensor...
-[Qax](https://github.com/davisyoshida/qax) is a tool for implementing types which represent tensors, but aren't actually instantiated as a single dense array on your GPU. Examples of this include:
+🦆[Qax](https://github.com/davisyoshida/qax)🦆 is a tool for implementing types which represent tensors, but aren't actually instantiated as a single dense array on your GPU. Examples of this include:
 * Quantization: A 4-bit array of integers + a small number of scale values are used to represent a full 16/32-bit array
 * LoRA: An array $W$ is replaced by the array $(W + BA^T)$ so that $A$ and $B$ may be trained while leaving $W$ frozen
 * Symbolic zeros/constants: For arrays which will consist entirely of a single repeated value, simply store that single value and the shape of the array
 * Custom kernels: If you have a custom kernel and want to use it with existing models without modifying them, Qax is an easy way to do so
 * Hopefully many more things!
 
 The goal of Qax is to make implementing custom JAX behavior much easier, so that users won't need to deal with all the details of writing a full JAX transform. All you need to do to get custom representations is:
@@ -21,15 +22,14 @@
 ```
 
 ## Example 1: A symbolic zero
 The way you specify custom behavior with Qax is to subclass the `qax.ImplicitArray` abstract class. One of the simplest things we could implement is a symbolic zero: A data type which represents an arbitrary tensor full of zeros without actually instantiating them on the GPU.
 
 
 ```python
-import qax
 class Zeros(qax.ImplicitArray):
     default_dtype = jnp.float32
 
     def materialize(self):
         # self.shape and self.dtype will be
         # populated by the ImplicitArray constructor
         return jnp.zeros(self.shape, self.dtype)
@@ -62,15 +62,15 @@
 
 ```python
 with warnings.catch_warnings():
     warnings.simplefilter('always')
     print(f(z, jnp.ones(3)))
 ```
 
-    qax/implicit_array.py:289: UserWarning: Primitive add was not handled by class Zeros, so implicit args will be materialized.
+    /home/davis/src/qax/qax/implicit/implicit_array.py:303: UserWarning: Primitive add was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
 
 
     1.0
 
 
 The cool thing is that `f` doesn't need to have any idea that it will be called with `ImplicitArray` instances, so we can use this with any pre-existing model. Right now this isn't much use, since all `z` is being materialized into a dense array as soon as it's needed for a JAX operation.
@@ -348,22 +348,22 @@
 
 
 The LoRA result is identical to the execution of the unmodified network, and we didn't get any materialization warnings so we successfully made a LoRA forward pass without ever calculating $W + AB^T$!
 
 ## Training
 So far we haven't looked at how to train a model when using Qax. The main thing to understand is that you should apply `qax.use_implicit_args` first, _then_ differentiate the resulting function. `use_implicit_args` transforms the function into one which goes from pytrees to pytrees, so all the standard JAX autodiff machinery will work.
 
-If you need to update only a subset of the elements of an ImplicitArray instance (e.g. only `a` and `b` for LoRA), Qax provides `qax.utils.freeze_qax_keys` to make this easier. Here's an end-to-end example training T5 to memorize the input/output pair from above:
+If you need to update only a subset of the elements of an ImplicitArray instance (e.g. only `a` and `b` for LoRA), Qax provides `qax.utils.freeze_keys` to make this easier. Here's an end-to-end example training T5 to memorize the input/output pair from above:
 
 
 ```python
 optimizer = optax.adam(3e-4)
 # freeze_keys_in_optimizer takes an optax optimizer, the ImplicitArray subclass to freeze for,
 # and an iterable of the keys to be frozen
-optimizer = qax.utils.freeze_qax_keys(optimizer, LoraMatrix, ['w'])
+optimizer = qax.utils.freeze_keys(optimizer, LoraMatrix, ['w'])
 
 # We're only using a single example so we'll just close over the training data
 # There are no code changes from an ordinary training loop other than decorating
 # loss_fn with @use_implicit_args
 
 @qax.use_implicit_args
 def loss_fn(params):
@@ -442,21 +442,17 @@
     print(f'With lora: {g(lora_with_symbolic_zero, x)}')
 ```
 
     Original: 15.0
     With lora: 15.0
 
 
-    qax/implicit_array.py:289: UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
-      warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
-      warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
+    UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
+    UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
 
 
 If we wanted we could write a `dot_general` handler to avoid the materialization as well, but the main point is just to illustrate that it's easy to mix and match different `ImplicitArray` subclasses. A more useful example might be using a symbolic zero as the offset for a quantization datatypes which expects both an offset and a scale.
 
 ## Other examples
-[Here's](https://github.com/davisyoshida/abnormal-floats/blob/8421c0b4677c5cd8e527ae999b00ee4a629c3318/transform.py#L17) an example of using Qax to implement a 4-bit quantized matrix representation.
+[Here's](https://github.com/davisyoshida/abnormal-floats/blob/master/transform.py) an example of using Qax to implement a 4-bit quantized matrix representation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qax-0.1.1/qax/constants.py` & `qax-0.2.0/qax/constants.py`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/qax/implicit_array.py` & `qax-0.2.0/qax/implicit/implicit_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,43 +13,57 @@
 import jax.linear_util as lu
 import jax.interpreters.partial_eval as pe
 from jax.tree_util import register_pytree_with_keys_class
 import jax.numpy as jnp
 
 from jax._src.typing import DTypeLike, Shape
 
-from . import constants
-from .primitives import ArrayValue, get_primitive_handler
-from . import utils
-
-def _use_implicit_flat(f_flat):
-    @wraps(f_flat)
-    def inner(*flat_args):
-        with core.new_main(ImplicitArrayTrace) as main:
-            trace = main.with_cur_sublevel()
-            tracers_in = [ImplicitArrayTracer(trace, val) if isinstance(val, ImplicitArray) else val for val in flat_args]
-
-            results = f_flat.call_wrapped(*tracers_in)
-            tracers_out = [trace.full_raise(t).value for t in results]
-        return tracers_out
-    return inner
+from .. import constants
+from ..primitives import ArrayValue, get_primitive_handler
+
+from . import implicit_utils as iu
+
+def _with_implicit_flat(fun: lu.WrappedFun) -> lu.WrappedFun:
+  # Splitting to avoid leaks based on https://github.com/google/jax/blob/0dffdf4645db7bf7a9fadd4bcfe9ec0368a8ecb9/jax/_src/interpreters/batching.py#L539
+    f = _implicit_inner(fun)
+    return _implicit_outer(f)
+
+@lu.transformation
+def _implicit_outer(*in_vals):
+    with core.new_main(ImplicitArrayTrace) as main:
+        outs = yield (main, *in_vals), {}
+        del main
+    yield outs
+
+@lu.transformation
+def _implicit_inner(main, *in_vals):
+    trace = main.with_cur_sublevel()
+    in_tracers = [
+        ImplicitArrayTracer(trace, val) if isinstance(val, ImplicitArray) else val
+        for val in in_vals
+    ]
+    outs = yield in_tracers, {}
+    out_vals = [trace.full_raise(t).value for t in outs]
+    yield out_vals
 
 def use_implicit_args(f):
     """
     Decorator which allows a function to accept arguments which subclass ImplicitArray, possibly
     including further ImplicitArray instances as children.
     Any number of arguments (including 0) may be ImplicitArrays.
     """
     @wraps(f)
-    def inner(*args, **kwargs):
-        flat_args, in_tree = utils.tree_flatten_with_implicit((args, kwargs))
+    def implicit_f(*args, **kwargs):
+        flat_args, in_tree = iu.tree_flatten_with_implicit((args, kwargs))
         f_flat, out_tree = flatten_fun(lu.wrap_init(f), in_tree)
-        outs_flat = _use_implicit_flat(f_flat)(*flat_args)
-        return jax.tree_util.tree_unflatten(out_tree(), outs_flat)
-    return inner
+        f_wrapped = _with_implicit_flat(f_flat)
+        outs_flat = f_wrapped.call_wrapped(*flat_args)
+        return out_tree().unflatten(outs_flat)
+
+    return implicit_f
 
 def aux_field(metadata=None, **kwargs):
     metadata = dict(metadata) if metadata else {}
     metadata['implicit_array_aux'] = True
     return field(metadata=metadata, **kwargs)
 
 class UninitializedAval(Exception):
@@ -218,15 +232,15 @@
         handler = lu.wrap_init(partial(get_primitive_handler(primitive), primitive))
         use_params = params
 
         if len(args) == 2 and self.commute_ops:
             args, use_params = _maybe_swap_args(primitive.name, args, use_params)
 
         #maybe_kwargs = {'params': params} if params else {}
-        flat_args, in_tree = utils.flatten_one_implicit_layer((args, params))
+        flat_args, in_tree = iu.flatten_one_implicit_layer((args, params))
         flat_handler, out_tree = flatten_fun(handler, in_tree)
 
         result = use_implicit_args(flat_handler.call_wrapped)(*flat_args)
         return jax.tree_util.tree_unflatten(out_tree(), result)
 
     def __init_subclass__(cls, commute_ops=True, **kwargs):
         super().__init_subclass__(**kwargs)
@@ -238,15 +252,15 @@
         return cls
 
 def _get_names_and_aux(obj):
     for val in fields(obj):
         yield val.name, bool(val.metadata.get('implicit_array_aux'))
 
 def _materialize_all(it):
-    return [utils.materialize_nested(val) if isinstance(val, ImplicitArray) else val for val in it]
+    return [iu.materialize_nested(val) if isinstance(val, ImplicitArray) else val for val in it]
 
 def _maybe_swap_args(op_name, args, params):
     if isinstance(args[0], ImplicitArray):
         return args, params
     if op_name in constants.COMMUTATIVE_OPS:
         return args[::-1], params
 
@@ -337,15 +351,15 @@
             branch_out_struct.unflatten(
                 jax.eval_shape(
                     partial(core.eval_jaxpr, new_jaxpr.jaxpr), new_jaxpr.literals, *flat_inputs
                 )
             )
         )
 
-    out_transforms = utils.get_common_prefix_transforms(out_avals)
+    out_transforms = iu.get_common_prefix_transforms(out_avals)
     new_branches = []
     out_struct = None
     for (new_jaxpr, orig_out_struct), transform in zip(new_jaxprs, out_transforms):
         new_jaxpr, out_struct = _transform_jaxpr_output(new_jaxpr, flat_inputs, orig_out_struct, transform)
         new_branches.append(new_jaxpr)
 
     return tuple(new_branches), out_struct, flat_inputs
@@ -404,15 +418,15 @@
         (tuple_val for _ in jax.tree_util.tree_leaves(tree))
         for tuple_val, tree in zip(t, trees)
     ))
 
 def _get_materialization_aval(imp_arr):
     with _aval_discovery_context(), _filter_materialization_warnings():
         result = jax.eval_shape(
-            partial(utils.materialize_nested, full=True),
+            partial(iu.materialize_nested, full=True),
             imp_arr
         )
     return result
 
 @contextmanager
 def _filter_materialization_warnings():
     with warnings.catch_warnings():
```

### Comparing `qax-0.1.1/qax/primitives.py` & `qax-0.2.0/qax/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 _primitive_ids = count()
 
 def get_lax_primitive_by_name(name):
     return getattr(jax.lax, f'{name}_p')
 
 def get_primitive_handler(primitive):
+    if isinstance(primitive, str):
+        primitive = get_lax_primitive_by_name(primitive)
     handler = _dispatch.functions.get(primitive)
     if handler is None:
         def _not_impl_handler(primitive : jax.core.Primitive, *args, **kwargs):
             return NotImplemented
         _not_impl_handler.__doc__ = 'Default handler for {primitive.name}'
         handler = Function(_not_impl_handler)
         handler.register(_not_impl_handler, precedence=-1e9)
@@ -30,17 +32,14 @@
     return handler
 
 def primitive_handler(primitives, precedence=0):
     if isinstance(primitives, (str, jax.core.Primitive)):
         primitives = [primitives]
     def decorator(fn):
         for primitive in primitives:
-            if isinstance(primitive, str):
-                primitive = get_lax_primitive_by_name(primitive)
             handler = get_primitive_handler(primitive)
             handler.register(fn, precedence=precedence)
-
     return decorator
 
 def default_handler(primitive, *args, **params):
     subfuns, bind_params = primitive.get_bind_params(params)
     return primitive.bind(*subfuns, *args, **bind_params)
```

### Comparing `qax-0.1.1/qax/quantization/pack.py` & `qax-0.2.0/qax/quantization/pack.py`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/qax/quantization/quant_utils.py` & `qax-0.2.0/qax/quantization/quant_utils.py`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/qax/quantization/quantized_matrix.py` & `qax-0.2.0/qax/quantization/quantized_matrix.py`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/qax/tracer.py` & `qax-0.2.0/qax/tracer.py`

 * *Files identical despite different names*

### Comparing `qax-0.1.1/qax/utils.py` & `qax-0.2.0/qax/implicit/implicit_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from functools import partial, wraps
 from itertools import chain
 
 import jax
-from jax import core
-from jax import tree_util
 from jax.api_util import flatten_fun_nokwargs
+from jax import core
 import jax.linear_util as lu
-import jax.numpy as jnp
-
-from jax._src.dtypes import float0
-
-import optax
+from jax import tree_util
 
 from . import implicit_array as ia
 
 class _EmptyNodeCls:
     _instance = None
     def __new__(cls):
         if cls._instance is None:
@@ -25,36 +20,14 @@
 
 tree_util.register_pytree_node(
     _EmptyNodeCls,
     lambda node: ((), None),
     lambda _, __: EmptyNode
 )
 
-def vmap_all_but_one(f, axis, out_ndim=0):
-    """
-    Repeatedly calls vmap to map over all axes except for `axis.`
-    All args will be mapped on the same dimensions.
-    """
-    @wraps(f)
-    def inner(*args):
-        n_dim = args[0].ndim
-        if axis >= n_dim:
-            raise ValueError(f'Axis {axis} is out of bounds for array of dimension {n_dim}')
-        fn = f
-        vmap_dim = 1
-        out_dim = out_ndim
-        for i in reversed(range(n_dim)):
-            if i == axis:
-                vmap_dim = 0
-                out_dim = 0
-            else:
-                fn = jax.vmap(fn, vmap_dim, out_dim)
-        return fn(*args)
-    return inner
-
 def combine_leaf_predicate(base_fn, is_leaf):
     @wraps(base_fn)
     def new_fn(*args, new_is_leaf=None):
         if new_is_leaf is None:
             combined_is_leaf = is_leaf
         else:
             def combined_is_leaf(arg):
@@ -136,19 +109,14 @@
         leaves, struct = tree_flatten_with_implicit(tree)
 
         mapped_leaves =  _map_leaves_with_implicit_path(partial(materialize_nested, full=True), leaves, is_leaf)
         return tree_util.tree_unflatten(struct, mapped_leaves)
 
     return materialize_subtrees
 
-class NodeAndPath:
-    def __init__(self, node, path):
-        self.node = node
-        self.path = path
-
 def get_common_prefix_transforms(trees):
     """
     Given an iterable of pytrees which have the same structure after all
     ImplicitArray instances are materialized, return a list of callables
     which will transform each tree into the largest common structure
     obtainable via materialization of ImplicitArrays.
     """
@@ -213,47 +181,14 @@
             continue
 
         for i, leaf_group in enumerate(zip(*all_leaves)):
             stack.append((path_prefix + (i,), leaf_group))
 
     return [_get_pruning_transform(tree, materialization_paths) for tree in trees]
 
-def freeze_keys(optimizer : optax.GradientTransformation, arr_type, freeze_keys):
-    freeze_keys = set(freeze_keys)
-    def label_leaf(leaf):
-        if not isinstance(leaf, arr_type):
-            return 'train'
-
-        children, aux_data = leaf.tree_flatten_with_keys()
-        labels = ['freeze' if key in freeze_keys else 'train' for key, _ in children]
-        struct = leaf.tree_unflatten(aux_data, labels)
-        return struct
-
-    def label_fn(root):
-        return jax.tree_map(label_leaf, root, is_leaf=lambda x: isinstance(x, arr_type))
-
-    multi_transformed_optimizer = optax.multi_transform(
-        {'freeze': optax.set_to_zero(), 'train': optimizer},
-        label_fn
-    )
-
-    def new_update(grads, opt_state, params):
-        def map_float0(param, grad):
-            if grad.dtype == float0:
-                return jnp.zeros_like(param)
-            return grad
-
-        fixed_grads = jax.tree_map(map_float0, params, grads)
-        return multi_transformed_optimizer.update(fixed_grads, opt_state, params)
-
-    return optax.GradientTransformation(
-        multi_transformed_optimizer.init,
-        new_update
-    )
-
 def materialize_nested(implicit_arr, full=False):
     """
     Materialize an ImplicitArray instance, handling the case where implicit_arr.materialize()
     involves further ImplicitArray instances.
     Arguments:
         implicit_arr: An ImplicitArray instance
         full: If True, repeatedly materialize until the result is a concrete array
@@ -267,7 +202,8 @@
         out_flat = ia.use_implicit_args(flat_fn.call_wrapped)(*flat)
         implicit_arr = jax.tree_util.tree_unflatten(out_tree(), out_flat)
 
         if not full:
             break
 
     return implicit_arr
+
```

### Comparing `qax-0.1.1/PKG-INFO` & `qax-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qax
-Version: 0.1.1
+Version: 0.2.0
 Summary: A JAX transform for writing things which pretend to be tensors
 License: MIT
 Author: Davis Yoshida
 Author-email: dyoshida@ttic.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,16 +13,17 @@
 Requires-Dist: jax (>=0.4.10,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.10,<0.5.0)
 Requires-Dist: optax (>=0.1.5,<0.2.0)
 Requires-Dist: plum-dispatch (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/davisyoshida/qax/blob/master/examples/How_to_Qax.ipynb)
+
 # Qax: If it quacks like a tensor...
-[Qax](https://github.com/davisyoshida/qax) is a tool for implementing types which represent tensors, but aren't actually instantiated as a single dense array on your GPU. Examples of this include:
+🦆[Qax](https://github.com/davisyoshida/qax)🦆 is a tool for implementing types which represent tensors, but aren't actually instantiated as a single dense array on your GPU. Examples of this include:
 * Quantization: A 4-bit array of integers + a small number of scale values are used to represent a full 16/32-bit array
 * LoRA: An array $W$ is replaced by the array $(W + BA^T)$ so that $A$ and $B$ may be trained while leaving $W$ frozen
 * Symbolic zeros/constants: For arrays which will consist entirely of a single repeated value, simply store that single value and the shape of the array
 * Custom kernels: If you have a custom kernel and want to use it with existing models without modifying them, Qax is an easy way to do so
 * Hopefully many more things!
 
 The goal of Qax is to make implementing custom JAX behavior much easier, so that users won't need to deal with all the details of writing a full JAX transform. All you need to do to get custom representations is:
@@ -39,15 +40,14 @@
 ```
 
 ## Example 1: A symbolic zero
 The way you specify custom behavior with Qax is to subclass the `qax.ImplicitArray` abstract class. One of the simplest things we could implement is a symbolic zero: A data type which represents an arbitrary tensor full of zeros without actually instantiating them on the GPU.
 
 
 ```python
-import qax
 class Zeros(qax.ImplicitArray):
     default_dtype = jnp.float32
 
     def materialize(self):
         # self.shape and self.dtype will be
         # populated by the ImplicitArray constructor
         return jnp.zeros(self.shape, self.dtype)
@@ -80,15 +80,15 @@
 
 ```python
 with warnings.catch_warnings():
     warnings.simplefilter('always')
     print(f(z, jnp.ones(3)))
 ```
 
-    qax/implicit_array.py:289: UserWarning: Primitive add was not handled by class Zeros, so implicit args will be materialized.
+    /home/davis/src/qax/qax/implicit/implicit_array.py:303: UserWarning: Primitive add was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
 
 
     1.0
 
 
 The cool thing is that `f` doesn't need to have any idea that it will be called with `ImplicitArray` instances, so we can use this with any pre-existing model. Right now this isn't much use, since all `z` is being materialized into a dense array as soon as it's needed for a JAX operation.
@@ -366,22 +366,22 @@
 
 
 The LoRA result is identical to the execution of the unmodified network, and we didn't get any materialization warnings so we successfully made a LoRA forward pass without ever calculating $W + AB^T$!
 
 ## Training
 So far we haven't looked at how to train a model when using Qax. The main thing to understand is that you should apply `qax.use_implicit_args` first, _then_ differentiate the resulting function. `use_implicit_args` transforms the function into one which goes from pytrees to pytrees, so all the standard JAX autodiff machinery will work.
 
-If you need to update only a subset of the elements of an ImplicitArray instance (e.g. only `a` and `b` for LoRA), Qax provides `qax.utils.freeze_qax_keys` to make this easier. Here's an end-to-end example training T5 to memorize the input/output pair from above:
+If you need to update only a subset of the elements of an ImplicitArray instance (e.g. only `a` and `b` for LoRA), Qax provides `qax.utils.freeze_keys` to make this easier. Here's an end-to-end example training T5 to memorize the input/output pair from above:
 
 
 ```python
 optimizer = optax.adam(3e-4)
 # freeze_keys_in_optimizer takes an optax optimizer, the ImplicitArray subclass to freeze for,
 # and an iterable of the keys to be frozen
-optimizer = qax.utils.freeze_qax_keys(optimizer, LoraMatrix, ['w'])
+optimizer = qax.utils.freeze_keys(optimizer, LoraMatrix, ['w'])
 
 # We're only using a single example so we'll just close over the training data
 # There are no code changes from an ordinary training loop other than decorating
 # loss_fn with @use_implicit_args
 
 @qax.use_implicit_args
 def loss_fn(params):
@@ -460,22 +460,18 @@
     print(f'With lora: {g(lora_with_symbolic_zero, x)}')
 ```
 
     Original: 15.0
     With lora: 15.0
 
 
-    qax/implicit_array.py:289: UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
-      warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
-      warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
+    UserWarning: Primitive dot_general was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
-    qax/implicit_array.py:289: UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
+    UserWarning: Primitive transpose was not handled by class Zeros, so implicit args will be materialized.
       warnings.warn(f'Primitive {primitive.name} was not handled by class {vals[implicit_idx].__class__.__name__}, so implicit args will be materialized.')
 
 
 If we wanted we could write a `dot_general` handler to avoid the materialization as well, but the main point is just to illustrate that it's easy to mix and match different `ImplicitArray` subclasses. A more useful example might be using a symbolic zero as the offset for a quantization datatypes which expects both an offset and a scale.
 
 ## Other examples
-[Here's](https://github.com/davisyoshida/abnormal-floats/blob/8421c0b4677c5cd8e527ae999b00ee4a629c3318/transform.py#L17) an example of using Qax to implement a 4-bit quantized matrix representation.
+[Here's](https://github.com/davisyoshida/abnormal-floats/blob/master/transform.py) an example of using Qax to implement a 4-bit quantized matrix representation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

