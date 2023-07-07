# Comparing `tmp/delayed_image-0.2.7-py3-none-any.whl.zip` & `tmp/delayed_image-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,26 @@
-Zip file size: 73023 bytes, number of entries: 13
--rw-r--r--  2.0 unx    15467 b- defN 23-May-02 19:30 delayed_image/__init__.py
--rw-r--r--  2.0 unx    61766 b- defN 23-May-02 19:30 delayed_image/channel_spec.py
--rw-r--r--  2.0 unx    13085 b- defN 23-May-02 19:30 delayed_image/delayed_base.py
--rw-r--r--  2.0 unx    13590 b- defN 23-May-02 19:30 delayed_image/delayed_leafs.py
--rw-r--r--  2.0 unx    99022 b- defN 23-May-02 19:30 delayed_image/delayed_nodes.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-02 19:30 delayed_image/demo.py
--rw-r--r--  2.0 unx    33248 b- defN 23-May-02 19:30 delayed_image/helpers.py
--rw-r--r--  2.0 unx    26215 b- defN 23-May-02 19:30 delayed_image/lazy_loaders.py
--rw-r--r--  2.0 unx    22747 b- defN 23-May-02 19:30 delayed_image/sensorchan_spec.py
--rw-r--r--  2.0 unx    30203 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1092 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/RECORD
-13 files, 317441 bytes uncompressed, 71211 bytes compressed:  77.6%
+Zip file size: 83062 bytes, number of entries: 24
+-rw-r--r--  2.0 unx    15115 b- defN 23-Jul-07 18:26 delayed_image/__init__.py
+-rw-r--r--  2.0 unx    61793 b- defN 23-Jul-07 18:26 delayed_image/channel_spec.py
+-rw-rw-rw-  2.0 unx     4354 b- defN 23-Jul-07 18:26 delayed_image/channel_spec.pyi
+-rw-r--r--  2.0 unx    13207 b- defN 23-Jul-07 18:26 delayed_image/delayed_base.py
+-rw-rw-rw-  2.0 unx     1887 b- defN 23-Jul-07 18:26 delayed_image/delayed_base.pyi
+-rw-r--r--  2.0 unx    13806 b- defN 23-Jul-07 18:26 delayed_image/delayed_leafs.py
+-rw-rw-rw-  2.0 unx     1504 b- defN 23-Jul-07 18:26 delayed_image/delayed_leafs.pyi
+-rw-r--r--  2.0 unx   100766 b- defN 23-Jul-07 18:26 delayed_image/delayed_nodes.py
+-rw-rw-rw-  2.0 unx     6370 b- defN 23-Jul-07 18:26 delayed_image/delayed_nodes.pyi
+-rw-r--r--  2.0 unx      900 b- defN 23-Jul-07 18:26 delayed_image/demo.py
+-rw-rw-rw-  2.0 unx       33 b- defN 23-Jul-07 18:26 delayed_image/demo.pyi
+-rw-r--r--  2.0 unx    14153 b- defN 23-Jul-07 18:26 delayed_image/helpers.py
+-rw-rw-rw-  2.0 unx      409 b- defN 23-Jul-07 18:26 delayed_image/helpers.pyi
+-rw-r--r--  2.0 unx    26437 b- defN 23-Jul-07 18:26 delayed_image/lazy_loaders.py
+-rw-rw-rw-  2.0 unx     2217 b- defN 23-Jul-07 18:26 delayed_image/lazy_loaders.pyi
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-07 18:26 delayed_image/py.typed
+-rw-r--r--  2.0 unx    22894 b- defN 23-Jul-07 18:26 delayed_image/sensorchan_spec.py
+-rw-rw-rw-  2.0 unx     2764 b- defN 23-Jul-07 18:26 delayed_image/sensorchan_spec.pyi
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 18:26 delayed_image/util/__init__.py
+-rw-r--r--  2.0 unx    32085 b- defN 23-Jul-07 18:26 delayed_image/util/util_network_text.py
+-rw-r--r--  2.0 unx    32200 b- defN 23-Jul-07 18:26 delayed_image-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 18:26 delayed_image-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-07 18:26 delayed_image-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2035 b- defN 23-Jul-07 18:26 delayed_image-0.2.8.dist-info/RECORD
+24 files, 355035 bytes uncompressed, 79768 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,40 +1,73 @@
 Filename: delayed_image/__init__.py
 Comment: 
 
 Filename: delayed_image/channel_spec.py
 Comment: 
 
+Filename: delayed_image/channel_spec.pyi
+Comment: 
+
 Filename: delayed_image/delayed_base.py
 Comment: 
 
+Filename: delayed_image/delayed_base.pyi
+Comment: 
+
 Filename: delayed_image/delayed_leafs.py
 Comment: 
 
+Filename: delayed_image/delayed_leafs.pyi
+Comment: 
+
 Filename: delayed_image/delayed_nodes.py
 Comment: 
 
+Filename: delayed_image/delayed_nodes.pyi
+Comment: 
+
 Filename: delayed_image/demo.py
 Comment: 
 
+Filename: delayed_image/demo.pyi
+Comment: 
+
 Filename: delayed_image/helpers.py
 Comment: 
 
+Filename: delayed_image/helpers.pyi
+Comment: 
+
 Filename: delayed_image/lazy_loaders.py
 Comment: 
 
+Filename: delayed_image/lazy_loaders.pyi
+Comment: 
+
+Filename: delayed_image/py.typed
+Comment: 
+
 Filename: delayed_image/sensorchan_spec.py
 Comment: 
 
-Filename: delayed_image-0.2.7.dist-info/METADATA
+Filename: delayed_image/sensorchan_spec.pyi
+Comment: 
+
+Filename: delayed_image/util/__init__.py
+Comment: 
+
+Filename: delayed_image/util/util_network_text.py
+Comment: 
+
+Filename: delayed_image-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: delayed_image-0.2.7.dist-info/WHEEL
+Filename: delayed_image-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: delayed_image-0.2.7.dist-info/top_level.txt
+Filename: delayed_image-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: delayed_image-0.2.7.dist-info/RECORD
+Filename: delayed_image-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## delayed_image/__init__.py

```diff
@@ -26,37 +26,55 @@
     >>> dimg = dimg.warp({'scale': 1.1})
     >>> dimg = dimg.warp({'scale': 1.1})
     >>> dimg = dimg.warp({'scale': 2.1})
     >>> dimg = dimg[0:200, 1:200]
     >>> dimg = dimg[1:200, 2:200]
     >>> dimg.write_network_text()
     ╙── Crop dsize=(128,130),space_slice=(slice(1,131,None),slice(2,130,None))
-        └─╼ Crop dsize=(130,131),space_slice=(slice(0,131,None),slice(1,131,None))
-            └─╼ Warp dsize=(131,131),transform={scale=2.1000}
-                └─╼ Warp dsize=(62,62),transform={scale=1.1000}
-                    └─╼ Warp dsize=(56,56),transform={scale=1.1000}
-                        └─╼ Warp dsize=(50,50),transform={scale=0.5000}
-                            └─╼ Crop dsize=(99,100),space_slice=(slice(0,100,None),slice(1,100,None))
-                                └─╼ Warp dsize=(100,100),transform={scale=0.5000}
-                                    └─╼ Crop dsize=(199,200),space_slice=(slice(0,200,None),slice(1,200,None))
-                                        └─╼ Warp dsize=(200,200),transform={scale=0.5000}
-                                            └─╼ Crop dsize=(399,400),space_slice=(slice(0,400,None),slice(1,400,None))
-                                                └─╼ Warp dsize=(621,621),transform={scale=1.1000}
-                                                    └─╼ Warp dsize=(564,564),transform={scale=1.1000}
-                                                        └─╼ Dequantize dsize=(512,512),quantization={quant_max=255,nodata=0}
-                                                            └─╼ Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
+        ╽
+        Crop dsize=(130,131),space_slice=(slice(0,131,None),slice(1,131,None))
+        ╽
+        Warp dsize=(131,131),transform={scale=2.1000}
+        ╽
+        Warp dsize=(62,62),transform={scale=1.1000}
+        ╽
+        Warp dsize=(56,56),transform={scale=1.1000}
+        ╽
+        Warp dsize=(50,50),transform={scale=0.5000}
+        ╽
+        Crop dsize=(99,100),space_slice=(slice(0,100,None),slice(1,100,None))
+        ╽
+        Warp dsize=(100,100),transform={scale=0.5000}
+        ╽
+        Crop dsize=(199,200),space_slice=(slice(0,200,None),slice(1,200,None))
+        ╽
+        Warp dsize=(200,200),transform={scale=0.5000}
+        ╽
+        Crop dsize=(399,400),space_slice=(slice(0,400,None),slice(1,400,None))
+        ╽
+        Warp dsize=(621,621),transform={scale=1.1000}
+        ╽
+        Warp dsize=(564,564),transform={scale=1.1000}
+        ╽
+        Dequantize dsize=(512,512),quantization={quant_max=255,nodata=0}
+        ╽
+        Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
 
     >>> # Optimize the chain
     >>> dopt = dimg.optimize()
     >>> dopt.write_network_text()
-    ╙── Warp dsize=(128,130),transform={offset=(-0.6...,-1.0...),scale=1.5373}
-        └─╼ Dequantize dsize=(80,83),quantization={quant_max=255,nodata=0}
-            └─╼ Crop dsize=(80,83),space_slice=(slice(0,83,None),slice(3,83,None))
-                └─╼ Overview dsize=(128,128),overview=2
-                    └─╼ Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
+    ╙── Warp dsize=(128,130),transform={offset=(-0.6115,-1.0000),scale=1.5373}
+        ╽
+        Dequantize dsize=(80,83),quantization={quant_max=255,nodata=0}
+        ╽
+        Crop dsize=(80,83),space_slice=(slice(0,83,None),slice(3,83,None))
+        ╽
+        Overview dsize=(128,128),overview=2
+        ╽
+        Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
 
     >>> final0 = dimg.finalize(optimize=False)
     >>> final1 = dopt.finalize()
     >>> assert final0.shape == final1.shape
     >>> # xdoctest: +REQUIRES(--show)
     >>> import kwplot
     >>> kwplot.autompl()
@@ -80,19 +98,19 @@
     >>> delayed = orig.optimize()
     >>> print('Orig')
     >>> orig.write_network_text()
     >>> print('Delayed')
     >>> delayed.write_network_text()
     >>> # Get the transform that would bring us back to the leaf
     >>> tf_root_from_leaf = delayed.get_transform_from_leaf()
-    >>> print('tf_root_from_leaf =\n{}'.format(ub.repr2(tf_root_from_leaf, nl=1)))
+    >>> print('tf_root_from_leaf =\n{}'.format(ub.urepr(tf_root_from_leaf, nl=1)))
     >>> undo_all = tf_root_from_leaf.inv()
-    >>> print('undo_all =\n{}'.format(ub.repr2(undo_all, nl=1)))
+    >>> print('undo_all =\n{}'.format(ub.urepr(undo_all, nl=1)))
     >>> undo_scale = kwimage.Affine.coerce(ub.dict_diff(undo_all.concise(), ['offset']))
-    >>> print('undo_scale =\n{}'.format(ub.repr2(undo_scale, nl=1)))
+    >>> print('undo_scale =\n{}'.format(ub.urepr(undo_scale, nl=1)))
     >>> print('Undone All')
     >>> undone_all = delayed.warp(undo_all).optimize()
     >>> undone_all.write_network_text()
     >>> # Discard translation components
     >>> print('Undone Scale')
     >>> undone_scale = delayed.warp(undo_scale).optimize()
     >>> undone_scale.write_network_text()
@@ -197,17 +215,17 @@
     >>>     print(ub.color_text(spec, color))
     >>>     print(ub.color_text('============', color))
     >>>     chosen_band.write_network_text()
     >>>     tf_root_from_leaf = chosen_band.get_transform_from_leaf()
     >>>     tf_leaf_from_root = tf_root_from_leaf.inv()
     >>>     undo_all = tf_leaf_from_root
     >>>     undo_scale = kwimage.Affine.coerce(ub.dict_diff(undo_all.concise(), ['offset', 'theta']))
-    >>>     print('tf_root_from_leaf = {}'.format(ub.repr2(tf_root_from_leaf.concise(), nl=1)))
-    >>>     print('undo_all = {}'.format(ub.repr2(undo_all.concise(), nl=1)))
-    >>>     print('undo_scale = {}'.format(ub.repr2(undo_scale.concise(), nl=1)))
+    >>>     print('tf_root_from_leaf = {}'.format(ub.urepr(tf_root_from_leaf.concise(), nl=1)))
+    >>>     print('undo_all = {}'.format(ub.urepr(undo_all.concise(), nl=1)))
+    >>>     print('undo_scale = {}'.format(ub.urepr(undo_scale.concise(), nl=1)))
     >>>     print('Undone All')
     >>>     undone_all = chosen_band.warp(undo_all, interpolation='lanczos').optimize()
     >>>     undone_all.write_network_text()
     >>>     # Discard translation components
     >>>     print('Undone Scale')
     >>>     undone_scale = chosen_band.warp(undo_scale).optimize()
     >>>     undone_scale.write_network_text()
@@ -230,15 +248,15 @@
     >>> stack = kwimage.stack_images(tostack_rows, axis=0, bg_value=(5, 100, 10), pad=10)
     >>> kwplot.imshow(stack, title='notice how the "undone all" crops are shifted to the right' + chr(10) + 'such that they align with the original image')
     >>> kwplot.show_if_requested()
 
 """
 
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 __author__ = 'Jon Crall'
 __author_email__ = 'jon.crall@kitware.com'
 
 
 __mkinit__ = """
 mkinit -m delayed_image
 """
```

## delayed_image/channel_spec.py

```diff
@@ -787,15 +787,15 @@
         """
         Look up component indices within this stream
 
         Example:
             >>> FCS = FusedChannelSpec.coerce
             >>> self = FCS('disparity|rgb|flowx|flowy')
             >>> component_indices = self.component_indices()
-            >>> print('component_indices = {}'.format(ub.repr2(component_indices, nl=1)))
+            >>> print('component_indices = {}'.format(ub.urepr(component_indices, nl=1, _dict_sort_behavior='old')))
             component_indices = {
                 'disparity': (slice(...), slice(...), slice(0, 1, None)),
                 'flowx': (slice(...), slice(...), slice(4, 5, None)),
                 'flowy': (slice(...), slice(...), slice(5, 6, None)),
                 'rgb': (slice(...), slice(...), slice(1, 4, None)),
             }
         """
@@ -864,23 +864,23 @@
 
         >>> # early and late fused input spec
         >>> ChannelSpec.coerce('rgb|ir,disprity')
         <ChannelSpec(rgb|ir,disprity) ...>
 
     Example:
         >>> self = ChannelSpec('gray')
-        >>> print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>> print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
         >>> self = ChannelSpec('rgb')
-        >>> print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>> print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
         >>> self = ChannelSpec('rgb|disparity')
-        >>> print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>> print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
         >>> self = ChannelSpec('rgb|disparity,disparity')
-        >>> print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>> print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
         >>> self = ChannelSpec('rgb,disparity,flowx|flowy')
-        >>> print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>> print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
 
     Example:
         >>> specs = [
         >>>     'rgb',              # and rgb input
         >>>     'rgb|disprity',     # rgb early fused with disparity
         >>>     'rgb,disprity',     # rgb early late with disparity
         >>>     'rgb|ir,disprity',  # rgb early fused with ir and late fused with disparity
@@ -890,26 +890,26 @@
         >>>     print('=======================')
         >>>     print('spec = {!r}'.format(spec))
         >>>     #
         >>>     self = ChannelSpec.coerce(spec)
         >>>     print('self = {!r}'.format(self))
         >>>     sizes = self.sizes()
         >>>     print('sizes = {!r}'.format(sizes))
-        >>>     print('self.info = {}'.format(ub.repr2(self.info, nl=1)))
+        >>>     print('self.info = {}'.format(ub.urepr(self.info, nl=1)))
         >>>     #
         >>>     item = self._demo_item((1, 1), rng=0)
         >>>     inputs = self.encode(item)
         >>>     components = self.decode(inputs)
         >>>     input_shapes = ub.map_vals(lambda x: x.shape, inputs)
         >>>     component_shapes = ub.map_vals(lambda x: x.shape, components)
-        >>>     print('item = {}'.format(ub.repr2(item, precision=1)))
-        >>>     print('inputs = {}'.format(ub.repr2(inputs, precision=1)))
-        >>>     print('input_shapes = {}'.format(ub.repr2(input_shapes)))
-        >>>     print('components = {}'.format(ub.repr2(components, precision=1)))
-        >>>     print('component_shapes = {}'.format(ub.repr2(component_shapes, nl=1)))
+        >>>     print('item = {}'.format(ub.urepr(item, precision=1)))
+        >>>     print('inputs = {}'.format(ub.urepr(inputs, precision=1)))
+        >>>     print('input_shapes = {}'.format(ub.urepr(input_shapes)))
+        >>>     print('components = {}'.format(ub.urepr(components, precision=1)))
+        >>>     print('component_shapes = {}'.format(ub.urepr(component_shapes, nl=1)))
 
     """
 
     def __init__(self, spec, parsed=None):
         # TODO: allow integer specs
         self._spec = spec
         self._info = {
@@ -1338,35 +1338,35 @@
             >>>     'flowx': np.random.rand(1, *dims),
             >>>     'flowy': np.random.rand(1, *dims),
             >>> }
             >>> # Complex Case
             >>> self = ChannelSpec('rgb,disparity,rgb|disparity|flowx|flowy,flowx|flowy')
             >>> fused = self.encode(item)
             >>> input_shapes = ub.map_vals(lambda x: x.shape, fused)
-            >>> print('input_shapes = {}'.format(ub.repr2(input_shapes, nl=1)))
+            >>> print('input_shapes = {}'.format(ub.urepr(input_shapes, nl=1)))
             >>> # Simpler case
             >>> self = ChannelSpec('rgb|disparity')
             >>> fused = self.encode(item)
             >>> input_shapes = ub.map_vals(lambda x: x.shape, fused)
-            >>> print('input_shapes = {}'.format(ub.repr2(input_shapes, nl=1)))
+            >>> print('input_shapes = {}'.format(ub.urepr(input_shapes, nl=1)))
 
         Example:
             >>> # Case where we have to break up early fused data
             >>> import numpy as np
             >>> dims = (40, 40)
             >>> item = {
             >>>     'rgb|disparity': np.random.rand(4, *dims),
             >>>     'flowx': np.random.rand(1, *dims),
             >>>     'flowy': np.random.rand(1, *dims),
             >>> }
             >>> # Complex Case
             >>> self = ChannelSpec('rgb,disparity,rgb|disparity,rgb|disparity|flowx|flowy,flowx|flowy,flowx,disparity')
             >>> inputs = self.encode(item)
             >>> input_shapes = ub.map_vals(lambda x: x.shape, inputs)
-            >>> print('input_shapes = {}'.format(ub.repr2(input_shapes, nl=1)))
+            >>> print('input_shapes = {}'.format(ub.urepr(input_shapes, nl=1)))
 
             >>> # xdoctest: +REQUIRES(--bench)
             >>> #self = ChannelSpec('rgb|disparity,flowx|flowy')
             >>> import timerit
             >>> ti = timerit.Timerit(100, bestof=10, verbose=2)
             >>> for timer in ti.reset('mode=simple'):
             >>>     with timer:
@@ -1485,15 +1485,15 @@
         Look up component indices within fused streams
 
         Example:
             >>> dims = (4, 4)
             >>> inputs = ['flowx', 'flowy', 'disparity']
             >>> self = ChannelSpec('disparity,flowx|flowy')
             >>> component_indices = self.component_indices()
-            >>> print('component_indices = {}'.format(ub.repr2(component_indices, nl=1)))
+            >>> print('component_indices = {}'.format(ub.urepr(component_indices, nl=1)))
             component_indices = {
                 'disparity': ('disparity', (slice(None, None, None), slice(None, None, None), slice(0, 1, None))),
                 'flowx': ('flowx|flowy', (slice(None, None, None), slice(None, None, None), slice(0, 1, None))),
                 'flowy': ('flowx|flowy', (slice(None, None, None), slice(None, None, None), slice(1, 2, None))),
             }
 
         """
```

## delayed_image/delayed_base.py

```diff
@@ -94,15 +94,15 @@
                 sub_meta.pop('jagged', None)
                 sub_meta.pop('border_value', None)
                 sub_meta.pop('antialias', None)
                 sub_meta.pop('interpolation', None)
                 sub_meta.pop('noop_eps', None)
             if 'fpath' in sub_meta:
                 sub_meta['fname'] = ub.Path(sub_meta.pop('fpath')).name
-            param_key = ub.repr2(sub_meta, sort=0, compact=1, nl=0, precision=4)
+            param_key = ub.urepr(sub_meta, sort=0, compact=1, nl=0, precision=4)
             short_type = item.__class__.__name__.replace('Delayed', '')
             node_data['label'] = f'{short_type} {param_key}'
         return graph
 
     @profile
     def _traverse(self):
         """
@@ -233,32 +233,32 @@
             node_data['meta'] = sub_meta
             node_data['obj'] = item
 
             for child in list(item.children())[::-1]:
                 stack.append((node_id, child))
         return graph
 
-    def print_graph(self, fields='auto', with_labels=True, rich='auto'):
+    def print_graph(self, fields='auto', with_labels=True, rich='auto', vertical_chains=True):
         """
         Alias for write_network_text
         """
-        self.write_network_text(fields=fields, with_labels=with_labels, rich=rich)
+        self.write_network_text(fields=fields, with_labels=with_labels, rich=rich, vertical_chains=vertical_chains)
 
-    def write_network_text(self, fields='auto', with_labels=True, rich='auto'):
+    def write_network_text(self, fields='auto', with_labels=True, rich='auto', vertical_chains=True):
         # TODO: remove once this is merged into networkx itself
-        from delayed_image.helpers import write_network_text
+        from delayed_image.util.util_network_text import write_network_text
         graph = self.as_graph(fields=fields)
         path = None
         end = '\n'
         if rich == 'auto':
             rich = rich_mod is not None
         if rich:
             path = rich_mod.print
             end = ''
-        write_network_text(graph, with_labels=with_labels, path=path, end=end)
+        write_network_text(graph, with_labels=with_labels, path=path, end=end, vertical_chains=vertical_chains)
 
     @property
     def shape(self):
         """
         Returns:
             None | Tuple[int | None, ...]
         """
@@ -275,15 +275,15 @@
     def prepare(self):
         """
         If metadata is missing, perform minimal IO operations in order to
         prepopulate metadata that could help us better optimize the operation
         tree.
 
         Returns:
-            DelayedOperation2
+            DelayedOperation
         """
         for child in self.children():
             child.prepare()
         return self
 
     def _finalize(self):
         """
@@ -314,15 +314,15 @@
                 in-place modification of select nested parameters.
 
         Returns:
             ArrayLike
 
         Notes:
             Do not overload this method. Overload
-            :func:`DelayedOperation2._finalize` instead.
+            :func:`DelayedOperation._finalize` instead.
         """
         if kwargs:
             """
             show dep warnings
 
             import warnings
             for item in list(warnings.filters):
@@ -345,15 +345,15 @@
         final = final[:]
         # final = np.asanyarray(final) # does not work with xarray
         return final
 
     def optimize(self):
         """
         Returns:
-            DelayedOperation2
+            DelayedOperation
         """
         raise NotImplementedError
 
     @profile
     def _set_nested_params(self, **kwargs):
         """
         Hack to override nested params on all warps for things like
```

## delayed_image/delayed_leafs.py

```diff
@@ -10,14 +10,18 @@
 # from delayed_image.delayed_nodes import DelayedArray
 
 try:
     from xdev import profile
 except ImportError:
     from ubelt import identity as profile
 
+__docstubs__ = """
+from delayed_image.channel_spec import FusedChannelSpec
+"""
+
 
 class DelayedImageLeaf(DelayedImage):
 
     def get_transform_from_leaf(self):
         """
         Returns the transformation that would align data with the leaf
 
@@ -192,16 +196,18 @@
             >>> print(f'delayed={delayed}')
             >>> delayed = DelayedLoad.demo(channels='r|g|b', nodata_method='float')
             >>> print(f'delayed={delayed}')
             >>> delayed.prepare()
             >>> print(f'delayed={delayed}')
             >>> delayed.finalize()
         """
-        fpath = kwimage.grab_test_image_fpath(key, dsize=dsize)
-        self = DelayedLoad(fpath, channels=channels)
+        fpath = kwimage.grab_test_image_fpath(key, dsize=dsize,
+                                              overviews=overviews)
+        self = DelayedLoad(fpath, channels=channels, dsize=dsize,
+                           nodata_method=nodata_method)
         return self
 
     @profile
     def _load_reference(self):
         nodata_method = self.meta.get('nodata_method', None)
         if self.lazy_ref is None:
             from delayed_image import lazy_loaders
```

## delayed_image/delayed_nodes.py

```diff
@@ -17,17 +17,51 @@
 except Exception:
     from ubelt import identity as profile
 
 # --------
 # Stacking
 # --------
 
+__docstubs__ = """
+from delayed_image.channel_spec import FusedChannelSpec
+from delayed_image.delayed_leafs import DelayedIdentity
+from delayed_image.delayed_base import DelayedOperation
+"""
+
 TRACE_OPTIMIZE = 0  # TODO: make this a local setting
 
 
+class DelayedArray(DelayedUnaryOperation):
+    """
+    A generic NDArray.
+    """
+    def __init__(self, subdata=None):
+        """
+        Args:
+            subdata (DelayedArray):
+        """
+        super().__init__(subdata=subdata)
+
+    def __nice__(self):
+        """
+        Returns:
+            str
+        """
+        return '{}'.format(self.shape)
+
+    @property
+    def shape(self):
+        """
+        Returns:
+            None | Tuple[int | None, ...]
+        """
+        shape = self.subdata.shape
+        return shape
+
+
 class DelayedStack(DelayedNaryOperation):
     """
     Stacks multiple arrays together.
     """
 
     def __init__(self, parts, axis):
         """
@@ -307,18 +341,41 @@
 
     def dequantize(self, quantization):
         """
         Rescales image intensities from int to floats.
 
         Args:
             quantization (Dict[str, Any]):
+                quantization information dictionary to undo.
                 see :func:`delayed_image.helpers.dequantize`
+                Expected keys are:
+                orig_dtype (str)
+                orig_min (float)
+                orig_max (float)
+                quant_min (float)
+                quant_max (float)
+                nodata (None | int)
 
         Returns:
             DelayedDequantize
+
+        Example:
+            >>> from delayed_image.delayed_leafs import DelayedLoad
+            >>> self = DelayedLoad.demo().prepare()
+            >>> quantization = {
+            >>>     'orig_dtype': 'float32',
+            >>>     'orig_min': 0,
+            >>>     'orig_max': 1,
+            >>>     'quant_min': 0,
+            >>>     'quant_max': 255,
+            >>>     'nodata': None,
+            >>> }
+            >>> new = self.dequantize(quantization)
+            >>> assert self.finalize().max() > 1
+            >>> assert new.finalize().max() <= 1
         """
         new = DelayedDequantize(self, quantization)
         return new
 
     def get_overview(self, overview):
         """
         Downsamples an image by a factor of two.
@@ -747,17 +804,17 @@
             return_warps (bool):
                 if True, return the transforms we applied. I.e. the transform
                 from the ``self`` to the returned ``parts``.
                 This is useful when you need to warp objects in the original
                 space into the jagged space.
 
         Returns:
-            List[DelayedImage] | Tuple[List[DelayedImage] | List[Affine]]:
+            List[DelayedImage] | Tuple[List[DelayedImage] | List[kwimage.Affine]]:
                 The List[DelayedImage] are the ``parts`` i.e. the new images with the warping undone.
-                The List[Affine]: is the transforms from ``self`` to each item in ``parts``
+                The List[kwimage.Affine]: is the transforms from ``self`` to each item in ``parts``
 
         Example:
             >>> from delayed_image.delayed_nodes import *  # NOQA
             >>> from delayed_image.delayed_leafs import DelayedLoad
             >>> from delayed_image.delayed_leafs import DelayedNans
             >>> import ubelt as ub
             >>> import kwimage
@@ -824,42 +881,14 @@
             for part in self.parts:
                 undone_part = part.undo_warp(
                     retain=retain, squash_nans=squash_nans)
                 unwarped_parts.append(undone_part)
             return unwarped_parts
 
 
-class DelayedArray(DelayedUnaryOperation):
-    """
-    A generic NDArray.
-    """
-    def __init__(self, subdata=None):
-        """
-        Args:
-            subdata (DelayedArray):
-        """
-        super().__init__(subdata=subdata)
-
-    def __nice__(self):
-        """
-        Returns:
-            str
-        """
-        return '{}'.format(self.shape)
-
-    @property
-    def shape(self):
-        """
-        Returns:
-            None | Tuple[int | None, ...]
-        """
-        shape = self.subdata.shape
-        return shape
-
-
 class DelayedImage(ImageOpsMixin, DelayedArray):
     """
     For the case where an array represents a 2D image with multiple channels
     """
     def __init__(self, subdata=None, dsize=None, channels=None):
         """
         Args:
@@ -1267,16 +1296,16 @@
         >>> from delayed_image.delayed_nodes import *  # NOQA
         >>> from delayed_image import DelayedLoad
         >>> self = DelayedLoad.demo(dsize=(16, 16)).prepare()
         >>> warp1 = self.warp({'scale': 3})
         >>> warp2 = warp1.warp({'theta': 0.1})
         >>> warp3 = warp2._opt_fuse_warps()
         >>> warp3._validate()
-        >>> print(ub.repr2(warp2.nesting(), nl=-1, sort=0))
-        >>> print(ub.repr2(warp3.nesting(), nl=-1, sort=0))
+        >>> print(ub.urepr(warp2.nesting(), nl=-1, sort=0))
+        >>> print(ub.urepr(warp3.nesting(), nl=-1, sort=0))
     """
     def __init__(self, subdata, transform, dsize='auto', antialias=True,
                  interpolation='linear', border_value='auto', noop_eps=0):
         """
         Args:
             subdata (DelayedArray): data to operate on
 
@@ -1661,21 +1690,21 @@
             >>> # xdoctest: +REQUIRES(module:osgeo)
             >>> from delayed_image.delayed_nodes import *  # NOQA
             >>> from delayed_image import DelayedLoad
             >>> import kwimage
             >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
             >>> self = DelayedLoad(fpath, channels='r|g|b').prepare()
             >>> print(f'self={self}')
-            >>> print('self.meta = {}'.format(ub.repr2(self.meta, nl=1)))
+            >>> print('self.meta = {}'.format(ub.urepr(self.meta, nl=1)))
             >>> warp0 = self.warp({'scale': 0.2})
             >>> warp1 = warp0._opt_split_warp_overview()
             >>> warp2 = self.warp({'scale': 0.25})._opt_split_warp_overview()
-            >>> print(ub.repr2(warp0.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(warp1.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(warp2.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(warp0.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(warp1.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(warp2.nesting(), nl=-1, sort=0))
             >>> warp0_nodes = [d['type'] for d in warp0.as_graph().nodes.values()]
             >>> warp1_nodes = [d['type'] for d in warp1.as_graph().nodes.values()]
             >>> warp2_nodes = [d['type'] for d in warp2.as_graph().nodes.values()]
             >>> assert warp0_nodes == ['DelayedWarp', 'DelayedLoad']
             >>> assert warp1_nodes == ['DelayedWarp', 'DelayedOverview', 'DelayedLoad']
             >>> assert warp2_nodes == ['DelayedOverview', 'DelayedLoad']
 
@@ -1684,16 +1713,16 @@
             >>> from delayed_image.delayed_nodes import *  # NOQA
             >>> from delayed_image import DelayedLoad
             >>> import kwimage
             >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
             >>> self = DelayedLoad(fpath, channels='r|g|b').prepare()
             >>> warp0 = self.warp({'scale': 1 / 2 ** 6})
             >>> opt = warp0.optimize()
-            >>> print(ub.repr2(warp0.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(opt.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(warp0.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(opt.nesting(), nl=-1, sort=0))
             >>> warp0_nodes = [d['type'] for d in warp0.as_graph().nodes.values()]
             >>> opt_nodes = [d['type'] for d in opt.as_graph().nodes.values()]
             >>> assert warp0_nodes == ['DelayedWarp', 'DelayedLoad']
             >>> assert opt_nodes == ['DelayedWarp', 'DelayedOverview', 'DelayedLoad']
         """
         inner_data = self.subdata
         num_overviews = inner_data.num_overviews
@@ -2074,16 +2103,16 @@
             >>>                     'theta': np.pi / 3,
             >>>                     'about': (80, 80),
             >>>                     'shearx': .3,
             >>>                     'offset': (-50, -50)})
             >>> node2 = node1[10:50, 1:40]
             >>> self = node2
             >>> new_outer = node2._opt_warp_after_crop()
-            >>> print(ub.repr2(node2.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(new_outer.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(node2.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(new_outer.nesting(), nl=-1, sort=0))
             >>> final0 = self._finalize()
             >>> final1 = new_outer._finalize()
             >>> # xdoctest: +REQUIRES(--show)
             >>> import kwplot
             >>> kwplot.autompl()
             >>> kwplot.imshow(final0, pnum=(2, 2, 1), fnum=1, title='raw')
             >>> kwplot.imshow(final1, pnum=(2, 2, 2), fnum=1, title='optimized')
@@ -2094,16 +2123,16 @@
             >>> from delayed_image.delayed_leafs import DelayedLoad
             >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
             >>> node0 = DelayedLoad(fpath, channels='r|g|b').prepare()
             >>> node1 = node0.warp({'scale': 1000 / 512})
             >>> node2 = node1[250:750, 0:500]
             >>> self = node2
             >>> new_outer = node2._opt_warp_after_crop()
-            >>> print(ub.repr2(node2.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(new_outer.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(node2.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(new_outer.nesting(), nl=-1, sort=0))
         """
         assert isinstance(self.subdata, DelayedWarp)
         # Inner is the data closer to the leaf (disk), outer is the data closer
         # to the user (output).
         outer_slices = self.meta['space_slice']
         outer_chan_idxs = self.meta['chan_idxs']
         inner_transform = self.subdata.meta['transform']
@@ -2159,15 +2188,15 @@
         >>> dimg = dimg.get_overview(1)
         >>> dimg = dimg.get_overview(1)
         >>> dopt = dimg.optimize()
         >>> if 1:
         >>>     import networkx as nx
         >>>     dimg.write_network_text()
         >>>     dopt.write_network_text()
-        >>> print(ub.repr2(dopt.nesting(), nl=-1, sort=0))
+        >>> print(ub.urepr(dopt.nesting(), nl=-1, sort=0))
         >>> final0 = dimg._finalize()[:]
         >>> final1 = dopt._finalize()[:]
         >>> assert final0.shape == final1.shape
         >>> # xdoctest: +REQUIRES(--show)
         >>> import kwplot
         >>> kwplot.autompl()
         >>> kwplot.imshow(final0, pnum=(1, 2, 1), fnum=1, title='raw')
@@ -2290,45 +2319,60 @@
             >>> from delayed_image import *  # NOQA
             >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
             >>> node0 = DelayedLoad(fpath, channels='r|g|b').prepare()
             >>> node1 = node0[100:400, 120:450]
             >>> node2 = node1.get_overview(2)
             >>> self = node2
             >>> new_outer = node2.optimize()
-            >>> print(ub.repr2(node2.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(new_outer.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(node2.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(new_outer.nesting(), nl=-1, sort=0))
             >>> final0 = self._finalize()
             >>> final1 = new_outer._finalize()
             >>> # xdoctest: +REQUIRES(--show)
             >>> import kwplot
             >>> kwplot.autompl()
             >>> kwplot.imshow(final0, pnum=(1, 2, 1), fnum=1, title='raw')
             >>> kwplot.imshow(final1, pnum=(1, 2, 2), fnum=1, title='optimized')
+
+        Example:
+            >>> # xdoctest: +REQUIRES(module:osgeo)
+            >>> from delayed_image import *  # NOQA
+            >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
+            >>> node0 = DelayedLoad(fpath, channels='r|g|b').prepare()
+            >>> node1 = node0[:, :, 0:2]
+            >>> node2 = node1.get_overview(2)
+            >>> self = node2
+            >>> new_outer = node2.optimize()
+            >>> node2.write_network_text()
+            >>> new_outer.write_network_text()
+            >>> assert node2.shape[2] == 2
+            >>> assert new_outer.shape[2] == 2
         """
         from delayed_image.helpers import _swap_crop_after_warp
         assert isinstance(self.subdata, DelayedCrop)
         # Inner is the data closer to the leaf (disk), outer is the data closer
         # to the user (output).
         outer_overview = self.meta['overview']
         inner_slices = self.subdata.meta['space_slice']
+        chan_idxs = self.subdata.meta['chan_idxs']
 
         sf = 1 / 2 ** outer_overview
         outer_transform = kwimage.Affine.scale(sf)
 
         inner_region = kwimage.Boxes.from_slice(inner_slices)
         inner_region = inner_region.to_polygons()[0]
 
         new_inner_warp, outer_crop, new_outer_warp = _swap_crop_after_warp(
             inner_region, outer_transform)
 
         # Move the overview to the inside, it should be unchanged
         new = self.subdata.subdata.get_overview(outer_overview)
 
         # Move the crop to the outside
-        new = new.crop(outer_crop)
+        new = new.crop(outer_crop, chan_idxs=chan_idxs)
 
         if not np.all(np.isclose(np.eye(3), new_outer_warp)):
             # we might have to apply an additional warp at the end.
             new = new.warp(new_outer_warp)
         if TRACE_OPTIMIZE:
             new._opt_logs.append('_opt_crop_after_overview')
         return new
@@ -2367,16 +2411,16 @@
             >>> from delayed_image import *  # NOQA
             >>> fpath = kwimage.grab_test_image_fpath(overviews=3)
             >>> node0 = DelayedLoad(fpath, channels='r|g|b').prepare()
             >>> node1 = node0.warp({'scale': (2.1, .7), 'offset': (20, 40)})
             >>> node2 = node1.get_overview(2)
             >>> self = node2
             >>> new_outer = node2.optimize()
-            >>> print(ub.repr2(node2.nesting(), nl=-1, sort=0))
-            >>> print(ub.repr2(new_outer.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(node2.nesting(), nl=-1, sort=0))
+            >>> print(ub.urepr(new_outer.nesting(), nl=-1, sort=0))
             >>> final0 = self._finalize()
             >>> final1 = new_outer._finalize()
             >>> # xdoctest: +REQUIRES(--show)
             >>> import kwplot
             >>> kwplot.autompl()
             >>> kwplot.imshow(final0, pnum=(1, 2, 1), fnum=1, title='raw')
             >>> kwplot.imshow(final1, pnum=(1, 2, 2), fnum=1, title='optimized')
```

## delayed_image/helpers.py

```diff
@@ -1,21 +1,23 @@
 import kwimage
 import ubelt as ub
 import numpy as np
-import sys
-from collections import defaultdict
+from .util import util_network_text
 
 
 try:
     import xdev
     profile = xdev.profile
 except Exception:
     profile = ub.identity
 
 
+write_network_text = util_network_text.write_network_text
+
+
 def _auto_dsize(transform, sub_dsize):
     sub_w, sub_h = sub_dsize
     sub_bounds = kwimage.Coords(
         np.array([[0,     0], [sub_w, 0],
                   [0, sub_h], [sub_w, sub_h]])
     )
     bounds = sub_bounds.warp(transform.matrix)
@@ -73,14 +75,15 @@
 
     Returns:
         Tuple[Tuple[slice, slice], kwimage.Affine]:
             leaf_crop_slices - the crop that happens before the warp
             tf_newleaf_to_newroot - warp that happens after the crop.
 
     Example:
+        >>> from delayed_image.helpers import *  # NOQA
         >>> region_slices = (slice(33, 100), slice(22, 62))
         >>> region_shape = (100, 100, 1)
         >>> root_region_box = kwimage.Boxes.from_slice(region_slices, shape=region_shape)
         >>> root_region_bounds = root_region_box.to_polygons()[0]
         >>> tf_leaf_to_root = kwimage.Affine.affine(scale=7).matrix
         >>> slices, tf_new = _swap_warp_after_crop(root_region_bounds, tf_leaf_to_root)
         >>> print('tf_new =\n{!r}'.format(tf_new))
@@ -107,15 +110,15 @@
         >>> print('slices = {!r}'.format(slices))
     """
     # Transform the region bounds into the sub-image space
     tf_leaf_to_root = kwimage.Affine.coerce(tf_leaf_to_root)
     tf_root_to_leaf = tf_leaf_to_root.inv()
     tf_root_to_leaf = tf_root_to_leaf.__array__()
     leaf_region_bounds = root_region_bounds.warp(tf_root_to_leaf)
-    leaf_region_box = leaf_region_bounds.bounding_box().to_ltrb()
+    leaf_region_box = leaf_region_bounds.box().to_ltrb()
 
     # Quantize to a region that is possible to sample from
     leaf_crop_box = leaf_region_box.quantize(inplace=True)
 
     # is this ok?
     # leaf_crop_box = leaf_crop_box.clip(0, 0, None, None, inplace=True)
     # Optimized clip
@@ -123,38 +126,38 @@
     np.clip(ltrb, 0, None, out=ltrb)
 
     # Because we sampled a large quantized region, we need to modify the
     # transform to nudge it a bit to the left, undoing the quantization,
     # which has a bit of extra padding on the left, before applying the
     # final transform.
     # subpixel_offset = leaf_region_box.data[0, 0:2]
-    crop_offset = leaf_crop_box.data[0, 0:2]
+    crop_offset = leaf_crop_box.data[0:2]
     root_offset = root_region_bounds.exterior.data.min(axis=0)
 
     # TODO: could optimize this logic
     tf_root_to_newroot = kwimage.Affine.translate(offset=-root_offset).matrix
     tf_newleaf_to_leaf = kwimage.Affine.translate(offset=crop_offset).matrix
 
     # Resample the smaller region to align it with the root region
     # Note: The right most transform is applied first
     tf_newleaf_to_newroot = (
         tf_root_to_newroot @
         tf_leaf_to_root @
         tf_newleaf_to_leaf
     )
 
-    lt_x, lt_y, rb_x, rb_y = leaf_crop_box.data[0, 0:4]
+    lt_x, lt_y, rb_x, rb_y = leaf_crop_box.data
 
     if 1:
         # Candidate fix
-        root_region_box = root_region_bounds.bounding_box()
-        old_w = root_region_box.width.ravel()[0]
-        old_h = root_region_box.height.ravel()[0]
-        leaf_w = leaf_region_box.width.ravel()[0]
-        leaf_h = leaf_region_box.height.ravel()[0]
+        root_region_box = root_region_bounds.box()
+        old_w = root_region_box.width
+        old_h = root_region_box.height
+        leaf_w = leaf_region_box.width
+        leaf_h = leaf_region_box.height
 
         padw = int(np.ceil(leaf_w / old_w))
         padh = int(np.ceil(leaf_h / old_h))
     else:
         padw, padh = 1, 1
     # padw, padh = 0, 0
 
@@ -203,42 +206,42 @@
         >>> from delayed_image.helpers import *  # NOQA
         >>> region_slices = (slice(33, 100), slice(22, 62))
         >>> region_shape = (100, 100, 1)
         >>> inner_region = kwimage.Boxes.from_slice(region_slices)
         >>> inner_region = inner_region.to_polygons()[0]
         >>> outer_transform = kwimage.Affine.affine(scale=1/4)
         >>> new_inner_warp, outer_crop, new_outer_warp = _swap_crop_after_warp(inner_region, outer_transform)
-        >>> print('new_inner_warp = {}'.format(ub.repr2(new_inner_warp, nl=1)))
-        >>> print('outer_crop = {}'.format(ub.repr2(outer_crop, nl=1)))
-        >>> print('new_outer_warp = {}'.format(ub.repr2(new_outer_warp, nl=1)))
+        >>> print('new_inner_warp = {}'.format(ub.urepr(new_inner_warp, nl=1)))
+        >>> print('outer_crop = {}'.format(ub.urepr(outer_crop, nl=1)))
+        >>> print('new_outer_warp = {}'.format(ub.urepr(new_outer_warp, nl=1)))
     """
     # Find where the inner region maps to after the transform is applied
     outer_region = inner_region.warp(outer_transform)
 
     # Transform the region bounds into the sub-image space
-    outer_box = outer_region.bounding_box().to_ltrb()
+    outer_box = outer_region.box().to_ltrb()
 
     # Quantize to a region that is possible to sample from
     outer_crop_box = outer_box.quantize()
 
     # is this ok?
     outer_crop_box = outer_crop_box.clip(0, 0, None, None)
 
     # Because the new crop might not be perfectly aligned, we might need to
     # nudge it a bit after we crop out its bounds.
-    crop_offset = outer_crop_box.data[0, 0:2]
+    crop_offset = outer_crop_box.data[0:2]
     outer_offset = outer_region.exterior.data.min(axis=0)
 
     # Compute the extra transform that will realign the quantized croped data
     # with the original warped inner crop.
     tf_crop_to_box = kwimage.Affine.affine(
         offset=crop_offset - outer_offset
     )
 
-    lt_x, lt_y, rb_x, rb_y = outer_crop_box.data[0, 0:4]
+    lt_x, lt_y, rb_x, rb_y = outer_crop_box.data
     outer_crop = (slice(lt_y, rb_y), slice(lt_x, rb_x))
     new_outer_warp = tf_crop_to_box
 
     # The inner warp will be the same as the original outer warp.
     new_inner_warp = outer_transform
 
     return new_inner_warp, outer_crop, new_outer_warp
@@ -380,555 +383,7 @@
         new_imdata = (imdata.clip(old_min, old_max) - old_min) * quant_factor + quantize_min
         new_imdata = new_imdata.astype(quantize_dtype)
         new_imdata[invalid_mask] = quantize_nan
     else:
         new_imdata = None
 
     return new_imdata, quantization
-
-
-### See: https://github.com/networkx/networkx/pull/5602
-
-
-class _AsciiBaseGlyphs:
-    empty = "+"
-    newtree_last = "+-- "
-    newtree_mid = "+-- "
-    endof_forest = "    "
-    within_forest = ":   "
-    within_tree = "|   "
-
-
-class AsciiDirectedGlyphs(_AsciiBaseGlyphs):
-    last = "L-> "
-    mid = "|-> "
-    backedge = "<-"
-
-
-class AsciiUndirectedGlyphs(_AsciiBaseGlyphs):
-    last = "L-- "
-    mid = "|-- "
-    backedge = "-"
-
-
-class _UtfBaseGlyphs:
-    # Notes on available box and arrow characters
-    # https://en.wikipedia.org/wiki/Box-drawing_character
-    # https://stackoverflow.com/questions/2701192/triangle-arrow
-    empty = "╙"
-    newtree_last = "╙── "
-    newtree_mid = "╟── "
-    endof_forest = "    "
-    within_forest = "╎   "
-    within_tree = "│   "
-
-
-class UtfDirectedGlyphs(_UtfBaseGlyphs):
-    last = "└─╼ "
-    mid = "├─╼ "
-    backedge = "╾"
-
-
-class UtfUndirectedGlyphs(_UtfBaseGlyphs):
-    last = "└── "
-    mid = "├── "
-    backedge = "─"
-
-
-def generate_network_text(
-    graph, with_labels=True, sources=None, max_depth=None, ascii_only=False
-):
-    """Generate lines in the "network text" format
-
-    This works via a depth-first traversal of the graph and writing a line for
-    each unique node encountered. Non-tree edges are written to the right of
-    each node, and connection to a non-tree edge is indicated with an ellipsis.
-    This representation works best when the input graph is a forest, but any
-    graph can be represented.
-
-    This notation is original to networkx, although it is simple enough that it
-    may be known in existing literature. See #5602 for details. The procedure
-    is summarized as follows:
-
-    1. Given a set of source nodes (which can be specified, or automatically
-    discovered via finding the (strongly) connected components and choosing one
-    node with minimum degree from each), we traverse the graph in depth first
-    order.
-
-    2. Each reachable node will be printed exactly once on it's own line.
-
-    3. Edges are indicated in one of three ways:
-
-        a. a parent "L-style" connection on the upper left. This corresponds to
-        a traversal in the directed DFS tree.
-
-        b. a backref "<-style" connection shown directly on the right. For
-        directed graphs, these are drawn for any incoming edges to a node that
-        is not a parent edge. For undirected graphs, these are drawn for only
-        the non-parent edges that have already been represented (The edges that
-        have not been represented will be handled in the recursive case).
-
-        c. a child "L-style" connection on the lower right. Drawing of the
-        children are handled recursively.
-
-    4. The children of each node (wrt the directed DFS tree) are drawn
-    underneath and to the right of it. In the case that a child node has already
-    been drawn the connection is replaced with an ellipsis ("...") to indicate
-    that there is one or more connections represented elsewhere.
-
-    5. If a maximum depth is specified, an edge to nodes past this maximum
-    depth will be represented by an ellipsis.
-
-    Parameters
-    ----------
-    graph : nx.DiGraph | nx.Graph
-        Graph to represent
-
-    with_labels : bool | str
-        If True will use the "label" attribute of a node to display if it
-        exists otherwise it will use the node value itself. If given as a
-        string, then that attribte name will be used instead of "label".
-        Defaults to True.
-
-    sources : List
-        Specifies which nodes to start traversal from. Note: nodes that are not
-        reachable from one of these sources may not be shown. If unspecified,
-        the minimal set of nodes needed to reach all others will be used.
-
-    max_depth : int | None
-        The maximum depth to traverse before stopping. Defaults to None.
-
-    ascii_only : Boolean
-        If True only ASCII characters are used to construct the visualization
-
-    Yields
-    ------
-    str : a line of generated text
-    """
-    is_directed = graph.is_directed()
-
-    if is_directed:
-        glyphs = AsciiDirectedGlyphs if ascii_only else UtfDirectedGlyphs
-        succ = graph.succ
-        pred = graph.pred
-    else:
-        glyphs = AsciiUndirectedGlyphs if ascii_only else UtfUndirectedGlyphs
-        succ = graph.adj
-        pred = graph.adj
-
-    if isinstance(with_labels, str):
-        label_attr = with_labels
-    elif with_labels:
-        label_attr = "label"
-    else:
-        label_attr = None
-
-    if max_depth == 0:
-        yield glyphs.empty + " ..."
-    elif len(graph.nodes) == 0:
-        yield glyphs.empty
-    else:
-
-        # If the nodes to traverse are unspecified, find the minimal set of
-        # nodes that will reach the entire graph
-        if sources is None:
-            sources = _find_sources(graph)
-
-        # Populate the stack with each:
-        # 1. parent node in the DFS tree (or None for root nodes),
-        # 2. the current node in the DFS tree
-        # 2. a list of indentations indicating depth
-        # 3. a flag indicating if the node is the final one to be written.
-        # Reverse the stack so sources are popped in the correct order.
-        last_idx = len(sources) - 1
-        stack = [
-            (None, node, [], (idx == last_idx)) for idx, node in enumerate(sources)
-        ][::-1]
-
-        num_skipped_children = defaultdict(lambda: 0)
-        seen_nodes = set()
-        while stack:
-            parent, node, indents, this_islast = stack.pop()
-
-            if node is not Ellipsis:
-                skip = node in seen_nodes
-                if skip:
-                    # Mark that we skipped a parent's child
-                    num_skipped_children[parent] += 1
-
-                if this_islast:
-                    # If we reached the last child of a parent, and we skipped
-                    # any of that parents children, then we should emit an
-                    # ellipsis at the end after this.
-                    if num_skipped_children[parent] and parent is not None:
-
-                        # Append the ellipsis to be emitted last
-                        next_islast = True
-                        try_frame = (node, Ellipsis, indents, next_islast)
-                        stack.append(try_frame)
-
-                        # Redo this frame, but not as a last object
-                        next_islast = False
-                        try_frame = (parent, node, indents, next_islast)
-                        stack.append(try_frame)
-                        continue
-
-                if skip:
-                    continue
-                seen_nodes.add(node)
-
-            if not indents:
-                # Top level items (i.e. trees in the forest) get different
-                # glyphs to indicate they are not actually connected
-                if this_islast:
-                    this_prefix = indents + [glyphs.newtree_last]
-                    next_prefix = indents + [glyphs.endof_forest]
-                else:
-                    this_prefix = indents + [glyphs.newtree_mid]
-                    next_prefix = indents + [glyphs.within_forest]
-
-            else:
-                # For individual tree edges distinguish between directed and
-                # undirected cases
-                if this_islast:
-                    this_prefix = indents + [glyphs.last]
-                    next_prefix = indents + [glyphs.endof_forest]
-                else:
-                    this_prefix = indents + [glyphs.mid]
-                    next_prefix = indents + [glyphs.within_tree]
-
-            if node is Ellipsis:
-                label = " ..."
-                suffix = ""
-                children = []
-            else:
-                if label_attr is not None:
-                    label = str(graph.nodes[node].get(label_attr, node))
-                else:
-                    label = str(node)
-
-                # Determine:
-                # (1) children to traverse into after showing this node.
-                # (2) parents to immediately show to the right of this node.
-                if is_directed:
-                    # In the directed case we must show every successor node
-                    # note: it may be skipped later, but we don't have that
-                    # information here.
-                    children = list(succ[node])
-                    # In the directed case we must show every predecessor
-                    # except for parent we directly traversed from.
-                    handled_parents = {parent}
-                else:
-                    # Showing only the unseen children results in a more
-                    # concise representation for the undirected case.
-                    children = [
-                        child for child in succ[node] if child not in seen_nodes
-                    ]
-
-                    # In the undirected case, parents are also children, so we
-                    # only need to immediately show the ones we can no longer
-                    # traverse
-                    handled_parents = {*children, parent}
-
-                if max_depth is not None and len(indents) == max_depth - 1:
-                    # Use ellipsis to indicate we have reached maximum depth
-                    if children:
-                        children = [Ellipsis]
-                    handled_parents = {parent}
-
-                # The other parents are other predecessors of this node that
-                # are not handled elsewhere.
-                other_parents = [p for p in pred[node] if p not in handled_parents]
-                if other_parents:
-                    if label_attr is not None:
-                        other_parents_labels = ", ".join(
-                            [
-                                str(graph.nodes[p].get(label_attr, p))
-                                for p in other_parents
-                            ]
-                        )
-                    else:
-                        other_parents_labels = ", ".join(
-                            [str(p) for p in other_parents]
-                        )
-                    suffix = " ".join(["", glyphs.backedge, other_parents_labels])
-                else:
-                    suffix = ""
-
-            # Emit the line for this node, this will be called for each node
-            # exactly once.
-            yield "".join(this_prefix + [label, suffix])
-
-            # Push children on the stack in reverse order so they are popped in
-            # the original order.
-            for idx, child in enumerate(children[::-1]):
-                next_islast = idx == 0
-                try_frame = (node, child, next_prefix, next_islast)
-                stack.append(try_frame)
-
-
-# @open_file(1, "w")
-def write_network_text(
-    graph,
-    path=None,
-    with_labels=True,
-    sources=None,
-    max_depth=None,
-    ascii_only=False,
-    end="\n",
-):
-    """Creates a nice text representation of a graph
-
-    This works via a depth-first traversal of the graph and writing a line for
-    each unique node encountered. Non-tree edges are written to the right of
-    each node, and connection to a non-tree edge is indicated with an ellipsis.
-    This representation works best when the input graph is a forest, but any
-    graph can be represented.
-
-    Parameters
-    ----------
-    graph : nx.DiGraph | nx.Graph
-        Graph to represent
-
-    path : string or file or callable or None
-       Filename or file handle for data output.
-       if a function, then it will be called for each generated line.
-       if None, this will default to "sys.stdout.write"
-
-    with_labels : bool | str
-        If True will use the "label" attribute of a node to display if it
-        exists otherwise it will use the node value itself. If given as a
-        string, then that attribte name will be used instead of "label".
-        Defaults to True.
-
-    sources : List
-        Specifies which nodes to start traversal from. Note: nodes that are not
-        reachable from one of these sources may not be shown. If unspecified,
-        the minimal set of nodes needed to reach all others will be used.
-
-    max_depth : int | None
-        The maximum depth to traverse before stopping. Defaults to None.
-
-    ascii_only : Boolean
-        If True only ASCII characters are used to construct the visualization
-
-    end : string
-        The line ending characater
-
-    Example
-    -------
-    >>> import networkx as nx
-    >>> graph = nx.balanced_tree(r=2, h=2, create_using=nx.DiGraph)
-    >>> write_network_text(graph)
-    ╙── 0
-        ├─╼ 1
-        │   ├─╼ 3
-        │   └─╼ 4
-        └─╼ 2
-            ├─╼ 5
-            └─╼ 6
-
-    >>> # A near tree with one non-tree edge
-    >>> graph.add_edge(5, 1)
-    >>> write_network_text(graph)
-    ╙── 0
-        ├─╼ 1 ╾ 5
-        │   ├─╼ 3
-        │   └─╼ 4
-        └─╼ 2
-            ├─╼ 5
-            │   └─╼  ...
-            └─╼ 6
-
-    >>> graph = nx.cycle_graph(5)
-    >>> write_network_text(graph)
-    ╙── 0
-        ├── 1
-        │   └── 2
-        │       └── 3
-        │           └── 4 ─ 0
-        └──  ...
-
-    >>> graph = nx.generators.barbell_graph(4, 2)
-    >>> write_network_text(graph)
-    ╙── 4
-        ├── 5
-        │   └── 6
-        │       ├── 7
-        │       │   ├── 8 ─ 6
-        │       │   │   └── 9 ─ 6, 7
-        │       │   └──  ...
-        │       └──  ...
-        └── 3
-            ├── 0
-            │   ├── 1 ─ 3
-            │   │   └── 2 ─ 0, 3
-            │   └──  ...
-            └──  ...
-
-    >>> graph = nx.complete_graph(5, create_using=nx.Graph)
-    >>> write_network_text(graph)
-    ╙── 0
-        ├── 1
-        │   ├── 2 ─ 0
-        │   │   ├── 3 ─ 0, 1
-        │   │   │   └── 4 ─ 0, 1, 2
-        │   │   └──  ...
-        │   └──  ...
-        └──  ...
-
-    >>> graph = nx.complete_graph(3, create_using=nx.DiGraph)
-    >>> write_network_text(graph)
-    ╙── 0 ╾ 1, 2
-        ├─╼ 1 ╾ 2
-        │   ├─╼ 2 ╾ 0
-        │   │   └─╼  ...
-        │   └─╼  ...
-        └─╼  ...
-    """
-    if path is None:
-        # The path is unspecified, write to stdout
-        _write = sys.stdout.write
-    elif hasattr(path, "write"):
-        # The path is already an open file
-        _write = path.write
-    elif callable(path):
-        # The path is a custom callable
-        _write = path
-    else:
-        raise TypeError(type(path))
-
-    for line in generate_network_text(
-        graph,
-        with_labels=with_labels,
-        sources=sources,
-        max_depth=max_depth,
-        ascii_only=ascii_only,
-    ):
-        _write(line + end)
-
-
-def _find_sources(graph):
-    """
-    Determine a minimal set of nodes such that the entire graph is reachable
-    """
-    # For each connected part of the graph, choose at least
-    # one node as a starting point, preferably without a parent
-    import networkx as nx
-    if graph.is_directed():
-        # Choose one node from each SCC with minimum in_degree
-        sccs = list(nx.strongly_connected_components(graph))
-        # condensing the SCCs forms a dag, the nodes in this graph with
-        # 0 in-degree correspond to the SCCs from which the minimum set
-        # of nodes from which all other nodes can be reached.
-        scc_graph = nx.condensation(graph, sccs)
-        supernode_to_nodes = {sn: [] for sn in scc_graph.nodes()}
-        # Note: the order of mapping differs between pypy and cpython
-        # so we have to loop over graph nodes for consistency
-        mapping = scc_graph.graph["mapping"]
-        for n in graph.nodes:
-            sn = mapping[n]
-            supernode_to_nodes[sn].append(n)
-        sources = []
-        for sn in scc_graph.nodes():
-            if scc_graph.in_degree[sn] == 0:
-                scc = supernode_to_nodes[sn]
-                node = min(scc, key=lambda n: graph.in_degree[n])
-                sources.append(node)
-    else:
-        # For undirected graph, the entire graph will be reachable as
-        # long as we consider one node from every connected component
-        sources = [
-            min(cc, key=lambda n: graph.degree[n])
-            for cc in nx.connected_components(graph)
-        ]
-        sources = sorted(sources, key=lambda n: graph.degree[n])
-    return sources
-
-
-def graph_str(graph, with_labels=True, sources=None, write=None, ascii_only=False):
-    """Creates a nice utf8 representation of a forest
-
-    This function has been superseded by
-    :func:`nx.readwrite.text.generate_network_text`, which should be used
-    instead.
-
-    Parameters
-    ----------
-    graph : nx.DiGraph | nx.Graph
-        Graph to represent (must be a tree, forest, or the empty graph)
-
-    with_labels : bool
-        If True will use the "label" attribute of a node to display if it
-        exists otherwise it will use the node value itself. Defaults to True.
-
-    sources : List
-        Mainly relevant for undirected forests, specifies which nodes to list
-        first. If unspecified the root nodes of each tree will be used for
-        directed forests; for undirected forests this defaults to the nodes
-        with the smallest degree.
-
-    write : callable
-        Function to use to write to, if None new lines are appended to
-        a list and returned. If set to the `print` function, lines will
-        be written to stdout as they are generated. If specified,
-        this function will return None. Defaults to None.
-
-    ascii_only : Boolean
-        If True only ASCII characters are used to construct the visualization
-
-    Returns
-    -------
-    str | None :
-        utf8 representation of the tree / forest
-
-    Example
-    -------
-    >>> import networkx as nx
-    >>> graph = nx.balanced_tree(r=2, h=3, create_using=nx.DiGraph)
-    >>> print(graph_str(graph))
-    ╙── 0
-        ├─╼ 1
-        │   ├─╼ 3
-        │   │   ├─╼ 7
-        │   │   └─╼ 8
-        │   └─╼ 4
-        │       ├─╼ 9
-        │       └─╼ 10
-        └─╼ 2
-            ├─╼ 5
-            │   ├─╼ 11
-            │   └─╼ 12
-            └─╼ 6
-                ├─╼ 13
-                └─╼ 14
-
-
-    >>> graph = nx.balanced_tree(r=1, h=2, create_using=nx.Graph)
-    >>> print(graph_str(graph))
-    ╙── 0
-        └── 1
-            └── 2
-
-    >>> print(graph_str(graph, ascii_only=True))
-    +-- 0
-        L-- 1
-            L-- 2
-    """
-    printbuf = []
-    if write is None:
-        _write = printbuf.append
-    else:
-        _write = write
-
-    write_network_text(
-        graph,
-        _write,
-        with_labels=with_labels,
-        sources=sources,
-        ascii_only=ascii_only,
-        end="",
-    )
-
-    if write is None:
-        # Only return a string if the custom write function was not specified
-        return "\n".join(printbuf)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## delayed_image/lazy_loaders.py

```diff
@@ -59,17 +59,25 @@
 
 # Only can use this cache if we assume we are in readonly mode
 # GLOBAL_GDAL_CACHE = CacheDict(cache_len=32)
 GLOBAL_GDAL_CACHE = None
 
 
 @ub.memoize
+def _import_gdal():
+    from osgeo import gdal
+    if getattr(gdal, '_UserHasSpecifiedIfUsingExceptions', lambda: False)():
+        gdal.UseExceptions()
+    return gdal
+
+
+@ub.memoize
 def _have_gdal():
     try:
-        from osgeo import gdal
+        gdal = _import_gdal()
     except ImportError:
         return False
     else:
         return gdal is not None
 
 
 @ub.memoize
@@ -380,15 +388,16 @@
         """
         Returns True if this backend is available
         """
         return _have_gdal()
 
     @profile
     def _reload_cache(self):
-        from osgeo import gdal
+        gdal = _import_gdal()
+        # from osgeo import gdal
         _fpath = os.fspath(self.fpath)
         if _fpath.endswith('.hdr'):
             # Use spectral-like process to point gdal to the correct file given
             # the hdr
             ext = '.' + _read_envi_header(_fpath)['interleave']
             _fpath = ub.augpath(_fpath, ext=ext)
 
@@ -565,15 +574,15 @@
             >>> for overview in range(0, 4):
             >>>     import timerit
             >>>     for timer in ti.reset('time'):
             >>>         with timer:
             >>>             self = LazyGDalFrameFile(fpath, overview=overview)
             >>>             imdata = self[100:200, 100:200]
             >>>     sec = ti.mean()
-            >>>     imdata = kwimage.draw_header_text(imdata, f'{overview=}\n{self.shape}\n[100:200, 100:200]\n{sec:0.6f}', fit='shrink')
+            >>>     imdata = kwimage.draw_header_text(imdata, f'overview={overview}\n{self.shape}\n[100:200, 100:200]\n{sec:0.6f}', fit='shrink')
             >>>     datas.append(imdata)
             >>> for overview in range(0, 4):
             >>>     import timerit
             >>>     aff = kwimage.Affine.coerce(scale=1 / (2 ** overview))
             >>>     crop_box = kwimage.Boxes.from_slice((slice(100, 200), slice(100, 200)))
             >>>     raw_crop = crop_box.warp(aff.inv()).quantize().to_slices()[0]
             >>>     for timer in ti.reset('time'):
```

## delayed_image/sensorchan_spec.py

```diff
@@ -22,16 +22,19 @@
     cache = functools.cache
 except AttributeError:
     cache = ub.memoize
 
 try:
     from lark import Transformer
 except ImportError:
-    class Transformer:
+    class FakeTransformer:
         pass
+    # TODO: get xdev typetubs to ignore this
+    # probably need some kind of directive.
+    Transformer = FakeTransformer
 
 SENSOR_CHAN_GRAMMAR = ub.codeblock(
     '''
     // SENSOR_CHAN_GRAMMAR
     ?start: stream
 
     // An identifier can contain spaces
@@ -128,15 +131,15 @@
         >>> from delayed_image.sensorchan_spec import SensorChanSpec
         >>> self = SensorChanSpec('(L8,S2):BGR,WV:BGR,S2:nir,L8:land.0:4')
         >>> s1 = self.normalize()
         >>> s2 = self.concise()
         >>> streams = self.streams()
         >>> print(s1)
         >>> print(s2)
-        >>> print('streams = {}'.format(ub.repr2(streams, sv=1, nl=1)))
+        >>> print('streams = {}'.format(ub.urepr(streams, sv=1, nl=1)))
         L8:BGR,S2:BGR,WV:BGR,S2:nir,L8:land.0|land.1|land.2|land.3
         (L8,S2,WV):BGR,L8:land:4,S2:nir
         streams = [
             L8:BGR,
             S2:BGR,
             WV:BGR,
             S2:nir,
@@ -493,22 +496,22 @@
         basis = {
             'concise_channels': [0, 1],
             'concise_sensors': [0, 1],
         }
         for spec in cases:
             print('')
             print('=====')
-            print('spec = {}'.format(ub.repr2(spec, nl=1)))
+            print('spec = {}'.format(ub.urepr(spec, nl=1)))
             print('-----')
             for kwargs in ub.named_product(basis):
                 sensor_channel_parser = _global_sensor_chan_parser()
                 tree = sensor_channel_parser.parse(spec)
                 transformed = SensorChanTransformer(**kwargs).transform(tree)
                 print('')
-                print('kwargs = {}'.format(ub.repr2(kwargs, nl=0)))
+                print('kwargs = {}'.format(ub.urepr(kwargs, nl=0)))
                 print(f'transformed={transformed}')
             print('')
             print('=====')
 
     """
 
     def __init__(self, concise_channels=1, concise_sensors=1):
@@ -629,15 +632,15 @@
         sensor_channel_parser = lark.Lark(SENSOR_CHAN_GRAMMAR,  start='start', parser='lalr', _plugins=lark_cython.plugins)
     except ImportError:
         sensor_channel_parser = lark.Lark(SENSOR_CHAN_GRAMMAR,  start='start', parser='lalr')
     return sensor_channel_parser
 
 
 @cache
-def normalize_sensor_chan(spec):
+def normalize_sensor_chan(spec: str):
     """
     Example:
         >>> # xdoctest: +REQUIRES(module:lark)
         >>> from delayed_image.sensorchan_spec import *  # NOQA
         >>> spec = 'L8:mat:4,L8:red,S2:red,S2:forest|brush,S2:mat.0|mat.1|mat.2|mat.3'
         >>> r1 = normalize_sensor_chan(spec)
         >>> spec = 'L8:r|g|b,L8:r|g|b'
@@ -657,15 +660,15 @@
         spec = '*:'
     transformed = sensorchan_normalized_parts(spec)
     new_spec = ','.join([n.spec for n in transformed])
     return new_spec
 
 
 @cache
-def concise_sensor_chan(spec):
+def concise_sensor_chan(spec: str):
     """
     Example:
         >>> # xdoctest: +REQUIRES(module:lark)
         >>> from delayed_image.sensorchan_spec import *  # NOQA
         >>> spec = 'L8:mat.0|mat.1|mat.2|mat.3,L8:red,S2:red,S2:forest|brush,S2:mat.0|mat.1|mat.2|mat.3'
         >>> concise_spec = concise_sensor_chan(spec)
         >>> normed_spec = normalize_sensor_chan(concise_spec)
@@ -676,15 +679,15 @@
     """
     transformed = sensorchan_concise_parts(spec)
     new_spec = ','.join([str(n) for n in transformed])
     return new_spec
 
 
 # @cache
-def sensorchan_concise_parts(spec):
+def sensorchan_concise_parts(spec: str):
     """
     Ignore:
         >>> # xdoctest: +REQUIRES(module:lark)
         >>> spec = 'L8:mat.0|mat.1|mat.2|mat.3,L8:red,(MODIS,S2):a|b|c,S2:red,S2:forest|brush|bare_ground,S2:mat.0|mat.1|mat.2|mat.3'
         >>> parts = sensorchan_concise_parts(spec)
     """
     try:
@@ -693,15 +696,15 @@
         transformed = SensorChanTransformer(concise_sensors=1, concise_channels=1).transform(tree)
     except Exception:
         print(f'ERROR: Failed to condense spec={spec}')
         raise
     return transformed
 
 
-def sensorchan_normalized_parts(spec):
+def sensorchan_normalized_parts(spec: str):
     """
     Ignore:
         >>> # xdoctest: +REQUIRES(module:lark)
         >>> spec = 'L8:mat.0|mat.1|mat.2|mat.3,L8:red,(MODIS,S2):a|b|c,S2:red,S2:forest|brush|bare_ground|built_up|cropland|wetland|water|snow_or_ice_field,S2:mat.0|mat.1|mat.2|mat.3'
         >>> parts = sensorchan_normalized_parts(spec)
     """
     try:
```

## Comparing `delayed_image-0.2.7.dist-info/METADATA` & `delayed_image-0.2.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 Metadata-Version: 2.1
 Name: delayed-image
-Version: 0.2.7
+Version: 0.2.8
 Summary: The delayed_image module
 Author: Jon Crall
 Author-email: jon.crall@kitware.com
 License: Apache 2
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Requires-Dist: kwarray
-Requires-Dist: kwimage
-Requires-Dist: ubelt
-Requires-Dist: affine
-Requires-Dist: numpy ; python_version < "3.10" and python_version >= "3.9"
-Requires-Dist: numpy ; python_version < "3.11" and python_version >= "3.10"
-Requires-Dist: numpy ; python_version < "3.7" and python_version >= "3.6"
-Requires-Dist: networkx ; python_version < "3.7.0" and python_version >= "3.6.0"
-Requires-Dist: networkx ; python_version < "3.8" and python_version >= "3.7"
-Requires-Dist: numpy ; python_version < "3.8" and python_version >= "3.7"
-Requires-Dist: numpy ; python_version < "3.9" and python_version >= "3.8"
-Requires-Dist: numpy ; python_version >= "3.11"
-Requires-Dist: networkx ; python_version >= "3.8"
+Requires-Dist: kwarray (>=0.6.7)
+Requires-Dist: kwimage (>=0.9.19)
+Requires-Dist: ubelt (>=1.2.3)
+Requires-Dist: affine (>=2.3.0)
+Requires-Dist: numpy (>=1.19.3) ; python_version < "3.10" and python_version >= "3.9"
+Requires-Dist: numpy (>=1.21.6) ; python_version < "3.11" and python_version >= "3.10"
+Requires-Dist: networkx (>=2.7) ; python_version < "3.11" and python_version >= "3.8"
+Requires-Dist: numpy (>=1.19.2) ; python_version < "3.7" and python_version >= "3.6"
+Requires-Dist: networkx (<=2.5.1,>=2.2.0) ; python_version < "3.7.0" and python_version >= "3.6.0"
+Requires-Dist: networkx (>=2.6.2) ; python_version < "3.8" and python_version >= "3.7"
+Requires-Dist: numpy (>=1.19.2) ; python_version < "3.8" and python_version >= "3.7"
+Requires-Dist: numpy (>=1.19.2) ; python_version < "3.9" and python_version >= "3.8"
+Requires-Dist: networkx (>=2.8) ; python_version < "4.0" and python_version >= "3.11"
+Requires-Dist: numpy (>=1.23.2) ; python_version < "4.0" and python_version >= "3.11"
 Provides-Extra: all
-Requires-Dist: kwarray ; extra == 'all'
-Requires-Dist: kwimage ; extra == 'all'
-Requires-Dist: ubelt ; extra == 'all'
-Requires-Dist: affine ; extra == 'all'
-Requires-Dist: xdoctest ; extra == 'all'
-Requires-Dist: pytest-timeout ; extra == 'all'
-Requires-Dist: lark-cython ; extra == 'all'
-Requires-Dist: lark ; extra == 'all'
-Requires-Dist: xarray ; extra == 'all'
+Requires-Dist: kwarray (>=0.6.7) ; extra == 'all'
+Requires-Dist: kwimage (>=0.9.19) ; extra == 'all'
+Requires-Dist: ubelt (>=1.2.3) ; extra == 'all'
+Requires-Dist: affine (>=2.3.0) ; extra == 'all'
+Requires-Dist: xdoctest (>=1.1.1) ; extra == 'all'
+Requires-Dist: pytest-timeout (>=1.4.2) ; extra == 'all'
+Requires-Dist: lark-cython (>=0.0.12) ; extra == 'all'
+Requires-Dist: lark (>=1.1.2) ; extra == 'all'
+Requires-Dist: xarray (>=0.16.0) ; extra == 'all'
 Provides-Extra: all-strict
-Requires-Dist: kwarray (==0.6.0) ; extra == 'all-strict'
-Requires-Dist: kwimage (==0.9.7) ; extra == 'all-strict'
-Requires-Dist: ubelt (==1.2.1) ; extra == 'all-strict'
-Requires-Dist: affine (==2.3.1) ; extra == 'all-strict'
-Requires-Dist: xdoctest (==0.14.0) ; extra == 'all-strict'
+Requires-Dist: kwarray (==0.6.7) ; extra == 'all-strict'
+Requires-Dist: kwimage (==0.9.19) ; extra == 'all-strict'
+Requires-Dist: ubelt (==1.2.3) ; extra == 'all-strict'
+Requires-Dist: affine (==2.3.0) ; extra == 'all-strict'
+Requires-Dist: xdoctest (==1.1.1) ; extra == 'all-strict'
 Requires-Dist: pytest-timeout (==1.4.2) ; extra == 'all-strict'
 Requires-Dist: lark-cython (==0.0.12) ; extra == 'all-strict'
 Requires-Dist: lark (==1.1.2) ; extra == 'all-strict'
 Requires-Dist: xarray (==0.16.0) ; extra == 'all-strict'
 Requires-Dist: coverage (==4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'all-strict'
 Requires-Dist: pytest (<=4.6.11,==4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all-strict'
 Requires-Dist: pytest-cov (==2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all-strict'
 Requires-Dist: numpy (==1.19.3) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all-strict'
 Requires-Dist: pytest (==4.6.0) ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'all-strict'
 Requires-Dist: numpy (==1.21.6) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'all-strict'
+Requires-Dist: networkx (==2.7) ; (python_version < "3.11" and python_version >= "3.8") and extra == 'all-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'all-strict'
 Requires-Dist: coverage (==4.3.4) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'all-strict'
 Requires-Dist: pytest (<=4.6.11,==4.6.0) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all-strict'
 Requires-Dist: pytest-cov (==2.8.1) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'all-strict'
 Requires-Dist: pytest (<=6.1.2,==4.6.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all-strict'
 Requires-Dist: pytest-cov (==2.9.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all-strict'
@@ -69,110 +72,116 @@
 Requires-Dist: networkx (<=2.5.1,==2.2.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all-strict'
 Requires-Dist: pytest (==4.6.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all-strict'
 Requires-Dist: networkx (==2.6.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all-strict'
+Requires-Dist: networkx (==2.8) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'all-strict'
+Requires-Dist: numpy (==1.23.2) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'all-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version >= "3.10") and extra == 'all-strict'
 Requires-Dist: pytest (==6.2.5) ; (python_version >= "3.10.0") and extra == 'all-strict'
-Requires-Dist: numpy (==1.23.2) ; (python_version >= "3.11") and extra == 'all-strict'
 Requires-Dist: pytest-cov (==3.0.0) ; (python_version >= "3.6.0") and extra == 'all-strict'
-Requires-Dist: networkx (==2.7) ; (python_version >= "3.8") and extra == 'all-strict'
-Requires-Dist: coverage ; (python_version < "2.7" and python_version >= "2.6") and extra == 'all'
-Requires-Dist: pytest ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all'
-Requires-Dist: pytest-cov ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all'
-Requires-Dist: numpy ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all'
-Requires-Dist: pytest ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'all'
-Requires-Dist: numpy ; (python_version < "3.11" and python_version >= "3.10") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.4" and python_version >= "2.7") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.5" and python_version >= "3.4") and extra == 'all'
-Requires-Dist: pytest ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all'
-Requires-Dist: pytest-cov ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.6" and python_version >= "3.5") and extra == 'all'
-Requires-Dist: pytest ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all'
-Requires-Dist: pytest-cov ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all'
-Requires-Dist: numpy ; (python_version < "3.7" and python_version >= "3.6") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.7" and python_version >= "3.6") and extra == 'all'
-Requires-Dist: networkx ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all'
-Requires-Dist: pytest ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all'
-Requires-Dist: networkx ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
-Requires-Dist: numpy ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
-Requires-Dist: numpy ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all'
-Requires-Dist: coverage ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all'
-Requires-Dist: coverage ; (python_version >= "3.10") and extra == 'all'
-Requires-Dist: pytest ; (python_version >= "3.10.0") and extra == 'all'
-Requires-Dist: numpy ; (python_version >= "3.11") and extra == 'all'
-Requires-Dist: pytest-cov ; (python_version >= "3.6.0") and extra == 'all'
-Requires-Dist: networkx ; (python_version >= "3.8") and extra == 'all'
+Requires-Dist: coverage (>=4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'all'
+Requires-Dist: pytest (<=4.6.11,>=4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all'
+Requires-Dist: pytest-cov (>=2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all'
+Requires-Dist: numpy (>=1.19.3) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all'
+Requires-Dist: pytest (>=4.6.0) ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'all'
+Requires-Dist: numpy (>=1.21.6) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'all'
+Requires-Dist: networkx (>=2.7) ; (python_version < "3.11" and python_version >= "3.8") and extra == 'all'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'all'
+Requires-Dist: coverage (>=4.3.4) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'all'
+Requires-Dist: pytest (<=4.6.11,>=4.6.0) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all'
+Requires-Dist: pytest-cov (>=2.8.1) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'all'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'all'
+Requires-Dist: pytest (<=6.1.2,>=4.6.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all'
+Requires-Dist: pytest-cov (>=2.9.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'all'
+Requires-Dist: numpy (>=1.19.2) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'all'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'all'
+Requires-Dist: networkx (<=2.5.1,>=2.2.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all'
+Requires-Dist: pytest (>=4.6.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'all'
+Requires-Dist: networkx (>=2.6.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
+Requires-Dist: numpy (>=1.19.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'all'
+Requires-Dist: numpy (>=1.19.2) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'all'
+Requires-Dist: networkx (>=2.8) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'all'
+Requires-Dist: numpy (>=1.23.2) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'all'
+Requires-Dist: coverage (>=6.1.1) ; (python_version >= "3.10") and extra == 'all'
+Requires-Dist: pytest (>=6.2.5) ; (python_version >= "3.10.0") and extra == 'all'
+Requires-Dist: pytest-cov (>=3.0.0) ; (python_version >= "3.6.0") and extra == 'all'
 Provides-Extra: graphics
 Provides-Extra: graphics-strict
 Requires-Dist: opencv-python (==3.4.15.55) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'graphics-strict'
+Requires-Dist: opencv-python (==4.5.4.58) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.1.0.0) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.1.0.5) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.1.0.2) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.4.13.47) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.4.15.55) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'graphics-strict'
 Requires-Dist: opencv-python (==3.4.15.55) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'graphics-strict'
-Requires-Dist: opencv-python (==4.5.4.58) ; (python_version >= "3.10") and extra == 'graphics-strict'
-Requires-Dist: opencv-python ; (python_version < "3.10" and python_version >= "3.9") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.4" and python_version >= "2.7") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.5" and python_version >= "3.4") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.6" and python_version >= "3.5") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.7" and python_version >= "3.6") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.8" and python_version >= "3.7") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version < "3.9" and python_version >= "3.8") and extra == 'graphics'
-Requires-Dist: opencv-python ; (python_version >= "3.10") and extra == 'graphics'
+Requires-Dist: opencv-python (==4.5.5.64) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'graphics-strict'
+Requires-Dist: opencv-python (>=3.4.15.55) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'graphics'
+Requires-Dist: opencv-python (>=4.5.4.58) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.1.0.0) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.1.0.5) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.1.0.2) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.4.13.47) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.4.15.55) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'graphics'
+Requires-Dist: opencv-python (>=3.4.15.55) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'graphics'
+Requires-Dist: opencv-python (>=4.5.5.64) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'graphics'
 Provides-Extra: headless
 Provides-Extra: headless-strict
-Requires-Dist: opencv-python-headless (==3.4.13.47) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (==3.4.15.55) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (==4.5.4.58) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'headless-strict'
 Requires-Dist: opencv-python-headless (==3.4.2.16) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'headless-strict'
 Requires-Dist: opencv-python-headless (==3.4.2.16) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'headless-strict'
-Requires-Dist: opencv-python-headless (==3.4.11.39) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (==3.4.2.16) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'headless-strict'
 Requires-Dist: opencv-python-headless (==3.4.13.47) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'headless-strict'
-Requires-Dist: opencv-python-headless (==3.4.13.47) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'headless-strict'
-Requires-Dist: opencv-python-headless (==3.4.13.47) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'headless-strict'
-Requires-Dist: opencv-python-headless (==4.5.4.58) ; (python_version >= "3.10") and extra == 'headless-strict'
-Requires-Dist: opencv-python-headless ; (python_version < "3.10" and python_version >= "3.9") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.4" and python_version >= "2.7") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.5" and python_version >= "3.4") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.6" and python_version >= "3.5") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.7" and python_version >= "3.6") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.8" and python_version >= "3.7") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version < "3.9" and python_version >= "3.8") and extra == 'headless'
-Requires-Dist: opencv-python-headless ; (python_version >= "3.10") and extra == 'headless'
+Requires-Dist: opencv-python-headless (==3.4.15.55) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (==3.4.15.55) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (==4.5.5.64) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'headless-strict'
+Requires-Dist: opencv-python-headless (>=3.4.15.55) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=4.5.4.58) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.2.16) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.2.16) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.2.16) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.13.47) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.15.55) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=3.4.15.55) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'headless'
+Requires-Dist: opencv-python-headless (>=4.5.5.64) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'headless'
 Provides-Extra: optional
-Requires-Dist: lark-cython ; extra == 'optional'
-Requires-Dist: lark ; extra == 'optional'
-Requires-Dist: xarray ; extra == 'optional'
+Requires-Dist: lark-cython (>=0.0.12) ; extra == 'optional'
+Requires-Dist: lark (>=1.1.2) ; extra == 'optional'
+Requires-Dist: xarray (>=0.16.0) ; extra == 'optional'
 Provides-Extra: optional-strict
 Requires-Dist: lark-cython (==0.0.12) ; extra == 'optional-strict'
 Requires-Dist: lark (==1.1.2) ; extra == 'optional-strict'
 Requires-Dist: xarray (==0.16.0) ; extra == 'optional-strict'
 Provides-Extra: runtime-strict
-Requires-Dist: kwarray (==0.6.0) ; extra == 'runtime-strict'
-Requires-Dist: kwimage (==0.9.7) ; extra == 'runtime-strict'
-Requires-Dist: ubelt (==1.2.1) ; extra == 'runtime-strict'
-Requires-Dist: affine (==2.3.1) ; extra == 'runtime-strict'
+Requires-Dist: kwarray (==0.6.7) ; extra == 'runtime-strict'
+Requires-Dist: kwimage (==0.9.19) ; extra == 'runtime-strict'
+Requires-Dist: ubelt (==1.2.3) ; extra == 'runtime-strict'
+Requires-Dist: affine (==2.3.0) ; extra == 'runtime-strict'
 Requires-Dist: numpy (==1.19.3) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.21.6) ; (python_version < "3.11" and python_version >= "3.10") and extra == 'runtime-strict'
+Requires-Dist: networkx (==2.7) ; (python_version < "3.11" and python_version >= "3.8") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'runtime-strict'
 Requires-Dist: networkx (<=2.5.1,==2.2.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'runtime-strict'
 Requires-Dist: networkx (==2.6.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'runtime-strict'
-Requires-Dist: numpy (==1.23.2) ; (python_version >= "3.11") and extra == 'runtime-strict'
-Requires-Dist: networkx (==2.7) ; (python_version >= "3.8") and extra == 'runtime-strict'
+Requires-Dist: networkx (==2.8) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'runtime-strict'
+Requires-Dist: numpy (==1.23.2) ; (python_version < "4.0" and python_version >= "3.11") and extra == 'runtime-strict'
 Provides-Extra: tests
-Requires-Dist: xdoctest ; extra == 'tests'
-Requires-Dist: pytest-timeout ; extra == 'tests'
+Requires-Dist: xdoctest (>=1.1.1) ; extra == 'tests'
+Requires-Dist: pytest-timeout (>=1.4.2) ; extra == 'tests'
 Provides-Extra: tests-strict
-Requires-Dist: xdoctest (==0.14.0) ; extra == 'tests-strict'
+Requires-Dist: xdoctest (==1.1.1) ; extra == 'tests-strict'
 Requires-Dist: pytest-timeout (==1.4.2) ; extra == 'tests-strict'
 Requires-Dist: coverage (==4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'tests-strict'
 Requires-Dist: pytest (<=4.6.11,==4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests-strict'
 Requires-Dist: pytest-cov (==2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'tests-strict'
 Requires-Dist: pytest (==4.6.0) ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'tests-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'tests-strict'
@@ -185,33 +194,33 @@
 Requires-Dist: coverage (==6.1.1) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'tests-strict'
 Requires-Dist: pytest (==4.6.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'tests-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'tests-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'tests-strict'
 Requires-Dist: coverage (==6.1.1) ; (python_version >= "3.10") and extra == 'tests-strict'
 Requires-Dist: pytest (==6.2.5) ; (python_version >= "3.10.0") and extra == 'tests-strict'
 Requires-Dist: pytest-cov (==3.0.0) ; (python_version >= "3.6.0") and extra == 'tests-strict'
-Requires-Dist: coverage ; (python_version < "2.7" and python_version >= "2.6") and extra == 'tests'
-Requires-Dist: pytest ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests'
-Requires-Dist: pytest-cov ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.10" and python_version >= "3.9") and extra == 'tests'
-Requires-Dist: pytest ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.4" and python_version >= "2.7") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.5" and python_version >= "3.4") and extra == 'tests'
-Requires-Dist: pytest ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'tests'
-Requires-Dist: pytest-cov ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.6" and python_version >= "3.5") and extra == 'tests'
-Requires-Dist: pytest ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'tests'
-Requires-Dist: pytest-cov ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.7" and python_version >= "3.6") and extra == 'tests'
-Requires-Dist: pytest ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.8" and python_version >= "3.7") and extra == 'tests'
-Requires-Dist: coverage ; (python_version < "3.9" and python_version >= "3.8") and extra == 'tests'
-Requires-Dist: coverage ; (python_version >= "3.10") and extra == 'tests'
-Requires-Dist: pytest ; (python_version >= "3.10.0") and extra == 'tests'
-Requires-Dist: pytest-cov ; (python_version >= "3.6.0") and extra == 'tests'
+Requires-Dist: coverage (>=4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'tests'
+Requires-Dist: pytest (<=4.6.11,>=4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests'
+Requires-Dist: pytest-cov (>=2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'tests'
+Requires-Dist: pytest (>=4.6.0) ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'tests'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'tests'
+Requires-Dist: coverage (>=4.3.4) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'tests'
+Requires-Dist: pytest (<=4.6.11,>=4.6.0) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'tests'
+Requires-Dist: pytest-cov (>=2.8.1) ; (python_version < "3.5.0" and python_version >= "3.4.0") and extra == 'tests'
+Requires-Dist: coverage (>=5.3.1) ; (python_version < "3.6" and python_version >= "3.5") and extra == 'tests'
+Requires-Dist: pytest (<=6.1.2,>=4.6.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'tests'
+Requires-Dist: pytest-cov (>=2.9.0) ; (python_version < "3.6.0" and python_version >= "3.5.0") and extra == 'tests'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.7" and python_version >= "3.6") and extra == 'tests'
+Requires-Dist: pytest (>=4.6.0) ; (python_version < "3.7.0" and python_version >= "3.6.0") and extra == 'tests'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'tests'
+Requires-Dist: coverage (>=6.1.1) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'tests'
+Requires-Dist: coverage (>=6.1.1) ; (python_version >= "3.10") and extra == 'tests'
+Requires-Dist: pytest (>=6.2.5) ; (python_version >= "3.10.0") and extra == 'tests'
+Requires-Dist: pytest-cov (>=3.0.0) ; (python_version >= "3.6.0") and extra == 'tests'
 
 The delayed_image Module
 ========================
 
 |Pypi| |PypiDownloads| |ReadTheDocs|
 
 The delayed image module lets you describe (a tree of) image operations, but
@@ -225,15 +234,15 @@
 cropped to it.  Overviews allow delayed image to load pre-downscaled images if
 it detects a scaling operation. This is **much** faster than the naive way of
 accomplishing these operations, and **much** easier than having to remember to
 do everything in the right order yourself.
 
 Note: GDAL is optional, but recommended. Precompiled GDAL wheels are available
 on Kitware's `large image wheel repository <https://girder.github.io/large_image_wheels/>`__.
-Use ``pip install gdal -f https://girder.github.io/large_image_wheels/`` 
+Use ``pip install gdal -f https://girder.github.io/large_image_wheels/``
 to install GDAL from this server. Track status of official GDAL wheels `here
 <https://github.com/OSGeo/gdal/issues/3060>`__.
 
 
 History
 -------
 
@@ -261,15 +270,15 @@
     delayed = delayed.scale(0.1)
     delayed = delayed[128:256, 128:256]
 
     import kwplot
     kwplot.autompl()
     kwplot.imshow(delayed.finalize())
     kwimage.imwrite('foo.png', delayed.finalize())
-    
+
 .. image:: https://i.imgur.com/lsWLkPx.png
 
 See `the quickstart jupyter notebook <examples/quickstart.ipynb/>`__ for more details.
 
 Delayed Loading
 ---------------
 
@@ -296,49 +305,67 @@
     >>> dimg = dimg.warp({'scale': 1.1})
     >>> dimg = dimg.warp({'scale': 1.1})
     >>> dimg = dimg.warp({'scale': 2.1})
     >>> dimg = dimg[0:200, 1:200]
     >>> dimg = dimg[1:200, 2:200]
     >>> dimg.write_network_text()
     ╙── Crop dsize=(128,130),space_slice=(slice(1,131,None),slice(2,130,None))
-        └─╼ Crop dsize=(130,131),space_slice=(slice(0,131,None),slice(1,131,None))
-            └─╼ Warp dsize=(131,131),transform={scale=2.1000}
-                └─╼ Warp dsize=(62,62),transform={scale=1.1000}
-                    └─╼ Warp dsize=(56,56),transform={scale=1.1000}
-                        └─╼ Warp dsize=(50,50),transform={scale=0.5000}
-                            └─╼ Crop dsize=(99,100),space_slice=(slice(0,100,None),slice(1,100,None))
-                                └─╼ Warp dsize=(100,100),transform={scale=0.5000}
-                                    └─╼ Crop dsize=(199,200),space_slice=(slice(0,200,None),slice(1,200,None))
-                                        └─╼ Warp dsize=(200,200),transform={scale=0.5000}
-                                            └─╼ Crop dsize=(399,400),space_slice=(slice(0,400,None),slice(1,400,None))
-                                                └─╼ Warp dsize=(621,621),transform={scale=1.1000}
-                                                    └─╼ Warp dsize=(564,564),transform={scale=1.1000}
-                                                        └─╼ Dequantize dsize=(512,512),quantization={quant_max=255,nodata=0}
-                                                            └─╼ Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
+        ╽
+        Crop dsize=(130,131),space_slice=(slice(0,131,None),slice(1,131,None))
+        ╽
+        Warp dsize=(131,131),transform={scale=2.1000}
+        ╽
+        Warp dsize=(62,62),transform={scale=1.1000}
+        ╽
+        Warp dsize=(56,56),transform={scale=1.1000}
+        ╽
+        Warp dsize=(50,50),transform={scale=0.5000}
+        ╽
+        Crop dsize=(99,100),space_slice=(slice(0,100,None),slice(1,100,None))
+        ╽
+        Warp dsize=(100,100),transform={scale=0.5000}
+        ╽
+        Crop dsize=(199,200),space_slice=(slice(0,200,None),slice(1,200,None))
+        ╽
+        Warp dsize=(200,200),transform={scale=0.5000}
+        ╽
+        Crop dsize=(399,400),space_slice=(slice(0,400,None),slice(1,400,None))
+        ╽
+        Warp dsize=(621,621),transform={scale=1.1000}
+        ╽
+        Warp dsize=(564,564),transform={scale=1.1000}
+        ╽
+        Dequantize dsize=(512,512),quantization={quant_max=255,nodata=0}
+        ╽
+        Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
 
     >>> # Optimize the chain
     >>> dopt = dimg.optimize()
     >>> dopt.write_network_text()
-    ╙── Warp dsize=(128,130),transform={offset=(-0.6...,-1.0...),scale=1.5373}
-        └─╼ Dequantize dsize=(80,83),quantization={quant_max=255,nodata=0}
-            └─╼ Crop dsize=(80,83),space_slice=(slice(0,83,None),slice(3,83,None))
-                └─╼ Overview dsize=(128,128),overview=2
-                    └─╼ Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
+    ╙── Warp dsize=(128,130),transform={offset=(-0.6115,-1.0000),scale=1.5373}
+        ╽
+        Dequantize dsize=(80,83),quantization={quant_max=255,nodata=0}
+        ╽
+        Crop dsize=(80,83),space_slice=(slice(0,83,None),slice(3,83,None))
+        ╽
+        Overview dsize=(128,128),overview=2
+        ╽
+        Load channels=r|g|b,dsize=(512,512),num_overviews=3,fname=astro_overviews=3.tif
 
     #
     >>> final0 = dimg.finalize(optimize=False)
     >>> final1 = dopt.finalize()
     >>> assert final0.shape == final1.shape
     >>> # xdoctest: +REQUIRES(--show)
     >>> import kwplot
     >>> kwplot.autompl()
     >>> kwplot.imshow(final0, pnum=(1, 2, 1), fnum=1, title='raw')
     >>> kwplot.imshow(final1, pnum=(1, 2, 2), fnum=1, title='optimized')
 
- 
+
 .. image:: https://i.imgur.com/3SGvxtC.png
 
 
 Native Resolution Sampling
 --------------------------
 
 Consider the case where we have multiple images on disk in different
@@ -355,15 +382,15 @@
 crop. Finalizing this delayed operation is exactly the same as the previously
 described case (except that it benefits from delayed image's optimized
 operation reordering). However, we can go further. Because we know about the
 underlying operation graph we can undo the scale component while keeping the
 crop component, which results in loading the corresponding parts of the image
 inside the cropped area, but does not do any resampling. The images on disk can
 differ in more than just resolution, they could also be offset, skewed or
-rotated, and this unwarping procedure will still work. 
+rotated, and this unwarping procedure will still work.
 
 The following image illustrates an extreme example of this were we simulate a
 low resolution red band (R), a medium but rotated resolution green band (G),
 and a high but cropped resolution blue (B) band.
 
 .. image:: https://i.imgur.com/fW7Mdo1.png
 
@@ -400,15 +427,15 @@
 .. code:: python
 
     import delayed_image
     import kwimage
     fpath = kwimage.grab_test_image_fpath(overviews=3)
 
     # When you create a delayed image, you can enrich the image with
-    # information about what channels it contains by specifying the 
+    # information about what channels it contains by specifying the
     # channels attribute.
     delayed = DelayedLoad(fpath, channels='red|green|blue').prepare()
 
     # You can use this to semantically interact with the channels
     delayed_g = delayed.take_channels('green')
     assert delayed_g.shape == (512, 512, 1)
 
@@ -420,15 +447,15 @@
 Much of the Sensor/Channel spec functionality exists for the benefit of other
 projects like `kwcoco <https://gitlab.kitware.com/computer-vision/kwcoco>`_.
 Admittedly, this library isn't the perfect home for the full sensor / channel
 spec, but this is where it currently lives.
 
 The full sensor channel spec has a formal grammar defined in this package.
 
- .. code:: 
+ .. code::
 
     // SENSOR_CHAN_GRAMMAR
     ?start: stream
 
     // An identifier can contain spaces
     IDEN: ("_"|"*"|LETTER) ("_"|" "|"-"|"*"|LETTER|DIGIT)*
```

