# Comparing `tmp/cellmap-1.0.1.dev202307070805-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202307070810-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 22403 bytes, number of entries: 5
+Zip file size: 22341 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   135974 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1914 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070805.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070805.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307070805.dist-info/RECORD
-5 files, 138433 bytes uncompressed, 21649 bytes compressed:  84.4%
+-rw-r--r--  2.0 unx   135883 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1914 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070810.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070810.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307070810.dist-info/RECORD
+5 files, 138342 bytes uncompressed, 21587 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070805.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202307070810.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070805.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202307070810.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070805.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202307070810.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -2426,15 +2426,15 @@
     target_clusters,
     path_key="path",
     exp_key=None,
     gene_dynamics_key="gene_dynamics",
     bifurcation_diagram_key="bifurcation_diagram",
     target_genes=[],
     n_div=100,
-    figsize=(12, 8.57),
+    figsize=(14, 10),
     fontsize_label=14,
     fontsize_text=12,
     fontsize_nDEG=18,
     fontsize_legend=10,
     DEG_min=1.0,
     DEG_rate=0.3,
     max_num_annotations=10,
@@ -2776,15 +2776,15 @@
                     i,
                     j,
                     k,
                 ),
                 frames=n_div + 1,
                 repeat=False,
             )
-            if show = True:
+            if show == True:
                 IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             if save:
                 filename = (
                     "%s_%s_%s" % (save_filename, target_clusters[i], target_clusters[j])
                     if save_dir == None
                     else "%s/%s_%s_%s"
                     % (save_dir, save_filename, target_clusters[i], target_clusters[j])
@@ -2818,14 +2818,15 @@
     target_clusters,
     path_key="path",
     exp_key=None,
     gene_dynamics_key="gene_dynamics",
     bifurcation_diagram_key="bifurcation_diagram",
     target_genes=[],
     n_div=100,
+    figsize=(14, 10),
     fontsize_label=14,
     fontsize_text=12,
     fontsize_nDEG=18,
     fontsize_legend=10,
     DEG_min=1.0,
     DEG_rate=0.3,
     max_num_annotations=10,
@@ -3151,16 +3152,15 @@
         ax3.axis("off")
 
     k = 0
     for i in range(len(target_clusters)):
         for j in range(i + 1, len(target_clusters)):
             name_i_ = source_cluster + "_" + target_clusters[i]
             name_j_ = source_cluster + "_" + target_clusters[j]
-            # fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
-            fig = plt.figure(figsize=(14, 10), tight_layout=True)
+            fig = plt.figure(figsize=figsize, tight_layout=True)
             grid = plt.GridSpec(10, 14)
             ax1 = fig.add_subplot(grid[0:2, 0:12])
             ax2 = fig.add_subplot(grid[2:10, 0:8])
             ax3 = fig.add_subplot(grid[2:10, 8:14])
             max_val_ = max(
                 np.max(gene_dynamics_[name_i_]), np.max(gene_dynamics_[name_j_])
             )
@@ -3199,15 +3199,15 @@
                     ani.save(filename)
                 elif save_type in ["image", "png", "jpg", "jpeg"]:
                     matplotlib.use("Agg")
                     if save_type == "image":
                         save_type = "png"
                     print("\nSaving gif animation as %s" % filename)
                     for t in range(n_div + 1):
-                        fig = plt.figure(figsize=(14, 10), tight_layout=True)
+                        fig = plt.figure(figsize=figsize, tight_layout=True)
                         grid = plt.GridSpec(10, 14)
                         ax1 = fig.add_subplot(grid[0:2, 0:12])
                         ax2 = fig.add_subplot(grid[2:10, 0:8])
                         ax3 = fig.add_subplot(grid[2:10, 8:14])
                         update(t, name_i_, name_j_, max_val_, lim, i, j, k)
                         filename_ = "%s_%03d.%s" % (filename, t, save_type)
                         fig.savefig(filename_, bbox_inches="tight")
```

## Comparing `cellmap-1.0.1.dev202307070805.dist-info/METADATA` & `cellmap-1.0.1.dev202307070810.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202307070805
+Version: 1.0.1.dev202307070810
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

