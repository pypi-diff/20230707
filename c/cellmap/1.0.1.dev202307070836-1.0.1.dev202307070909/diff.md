# Comparing `tmp/cellmap-1.0.1.dev202307070836-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202307070909-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 22345 bytes, number of entries: 5
+Zip file size: 22377 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   135883 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1914 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070836.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070836.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307070836.dist-info/RECORD
-5 files, 138342 bytes uncompressed, 21591 bytes compressed:  84.4%
+-rw-r--r--  2.0 unx   136201 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1914 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070909.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202307070909.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202307070909.dist-info/RECORD
+5 files, 138660 bytes uncompressed, 21623 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070836.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202307070909.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070836.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202307070909.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202307070836.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202307070909.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -2007,15 +2007,15 @@
     n_neighbors=10,
     contribution_rate_pca=0.95,
     cutedge_vol=None,
     cutedge_length=None,
     figsize=(10, 8),
     save=False,
     save_dir=None,
-    save_filename="trajectory",
+    save_filename="Trajectory",
 ):
     kwargs_arg = _check_arguments(adata, verbose=True, basis=basis)
     basis = kwargs_arg["basis"]
 
     if sum(adata.obs[cluster_key].values == source_cluster) == 0:
         raise KeyError("Cluster %s was not found" % source_cluster)
     for trg_ in target_clusters:
@@ -2334,15 +2334,15 @@
     n_div=100,
     figsize=(10, 4),
     fontsize_title=16,
     fontsize_label=14,
     fontsize_legend=12,
     save=False,
     save_dir=None,
-    save_filename="gene_dynamics_plot",
+    save_filename="Gene_dynamics",
 ):
 
     if gene_dynamics_key not in adata.uns.keys():
         calc_gene_dynamics(
             adata,
             source_cluster,
             target_clusters,
@@ -3271,15 +3271,15 @@
     n_div=100,
     figsize=(12, 3),
     fontsize_label=14,
     adjusttext=False,
     PC=1,
     save=False,
     save_dir=None,
-    save_filename="bifurcation_diagram",
+    save_filename="Bifurcation_diagram",
 ):
     if gene_dynamics_key not in adata.uns.keys():
         calc_gene_dynamics(
             adata,
             source_cluster,
             target_clusters,
             path_key=path_key,
@@ -3469,15 +3469,15 @@
     seed=0,
     threshold_min=1,
     n_clusters=20,
     n_components=2,
     pt_size=5,
     save=False,
     save_dir=None,
-    save_filename="gene_atlas",
+    save_filename="Gene_atlas",
     save_type="html",
 ):
     if gene_atlas_key not in adata.uns.keys():
         calc_gene_atlas(
             adata,
             source_cluster,
             target_clusters,
@@ -3779,15 +3779,15 @@
     path_key="path",
     exp_key=None,
     gene_dynamics_key="gene_dynamics",
     n_div=100,
     fontsize_label=10,
     save=False,
     save_dir=None,
-    save_filename="key_gene_dynamics",
+    save_filename="Key_gene_dynamics",
 ):
     if gene_dynamics_key not in adata.uns.keys():
         calc_gene_dynamics(
             adata,
             source_cluster,
             target_clusters,
             path_key=path_key,
@@ -3979,14 +3979,17 @@
     adata,
     source_cluster,
     target_clusters,
     exp_key=None,
     grn_key="GRN",
     genes=None,
     n_genes=20,
+    save=False,
+    save_dir=None,
+    save_filename="GRN",
 ):
     if genes == None:
         data_exp = _set_expression_data(adata, exp_key)
         data_exp_var_div_mean = np.nan_to_num(
             np.var(data_exp, axis=0) / np.mean(data_exp, axis=0)
         )
         idx_rank_ = np.argsort(data_exp_var_div_mean)[::-1][:n_genes]
@@ -4009,8 +4012,15 @@
             robust=True,
             vmin=vmin,
             vmax=vmax,
             center=0,
         )
         ax.set_title(name_i_)
         ax.set_xlabel("Target")
-        ax.set_ylabel("Source")
+        ax.set_ylabel("Source")
+        if save:
+            filename = (
+                "%s_%s" % (save_filename,name_i_)
+                if save_dir == None
+                else "%s/%s" % (save_dir, save_filename)
+            )
+            fig.savefig(filename + ".png", bbox_inches="tight")
```

## Comparing `cellmap-1.0.1.dev202307070836.dist-info/METADATA` & `cellmap-1.0.1.dev202307070909.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202307070836
+Version: 1.0.1.dev202307070909
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

