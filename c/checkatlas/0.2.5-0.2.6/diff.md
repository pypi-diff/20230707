# Comparing `tmp/checkatlas-0.2.5.tar.gz` & `tmp/checkatlas-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.2.5.tar", max compression
+gzip compressed data, was "checkatlas-0.2.6.tar", max compression
```

## Comparing `checkatlas-0.2.5.tar` & `checkatlas-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,30 @@
--rw-r--r--   0        0        0     1211 2023-07-07 09:44:48.184445 checkatlas-0.2.5/LICENSE
--rw-r--r--   0        0        0     3841 2023-07-07 09:44:48.184445 checkatlas-0.2.5/README.md
--rw-r--r--   0        0        0      130 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/__init__.py
--rw-r--r--   0        0        0     8445 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/__main__.py
--rw-r--r--   0        0        0    20197 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/atlas.py
--rw-r--r--   0        0        0    17277 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/atlas_seurat.py
--rw-r--r--   0        0        0    12728 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas.py
--rw-r--r--   0        0        0      931 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas_workflow.nf
--rw-r--r--   0        0        0    10123 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0     1127 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/convertSeurat.R
--rw-r--r--   0        0        0     1905 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/folders.py
--rw-r--r--   0        0        0        0 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4103 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0      721 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/multiqc.py
--rw-r--r--   0        0        0     1431 2023-07-07 09:44:48.384444 checkatlas-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 checkatlas-0.2.5/setup.py
--rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 checkatlas-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-07 13:52:57.938636 checkatlas-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-07 13:52:57.938636 checkatlas-0.2.6/README.md
+-rw-r--r--   0        0        0      117 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/__init__.py
+-rw-r--r--   0        0        0    21675 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/atlas.py
+-rw-r--r--   0        0        0    17277 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/atlas_seurat.py
+-rw-r--r--   0        0        0     6682 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     1905 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/folders.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4103 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0     1239 2023-07-07 13:52:58.142641 checkatlas-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 checkatlas-0.2.6/setup.py
+-rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 checkatlas-0.2.6/PKG-INFO
```

### Comparing `checkatlas-0.2.5/LICENSE` & `checkatlas-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/README.md` & `checkatlas-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/atlas.py` & `checkatlas-0.2.6/checkatlas/atlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
     "total_counts",
     "total_counts_mt",
     "pct_counts_mt",
     "total_counts_ribo",
     "pct_counts_ribo",
 ]
 
+CELLINDEX_HEADER = "cell_index"
+
 logger = logging.getLogger("checkatlas")
 
 
 def read_atlas(atlas_path, atlas_info):
     logger.info(f"Load {atlas_info[0]} in {atlas_info[-1]}")
     try:
         if atlas_path.endswith(".h5"):
@@ -351,26 +353,48 @@
     """
     atlas_name = atlas_info[0]
     qc_path = os.path.join(
         folders.get_folder(args.path, folders.QC),
         atlas_name + checkatlas.QC_EXTENSION,
     )
     logger.debug(f"Create QC tables for {atlas_name}")
+    qc_genes = []
     # mitochondrial genes
     adata.var["mt"] = adata.var_names.str.startswith("MT-")
+    if len(adata.var[adata.var["mt"]]) != 0:
+        qc_genes.append("mt")
+        logger.debug(f"Mitochondrial genes in {atlas_name} for QC")
+    else:
+        logger.debug(f"No mitochondrial genes in {atlas_name} for QC")
     # ribosomal genes
     adata.var["ribo"] = adata.var_names.str.startswith(("RPS", "RPL"))
+    if len(adata.var[adata.var["mt"]]) != 0:
+        qc_genes.append("ribo")
+        logger.debug(f"Ribosomal genes in {atlas_name} for QC")
+    else:
+        logger.debug(f"No ribosomal genes in {atlas_name} for QC")
+
     sc.pp.calculate_qc_metrics(
         adata,
-        qc_vars=["mt", "ribo"],
+        qc_vars=qc_genes,
         percent_top=None,
         log1p=False,
         inplace=True,
     )
     df_annot = adata.obs[get_viable_obs_qc(adata, args)]
+    # Rank cell by qc metric
+    for header in df_annot.columns:
+        if header != CELLINDEX_HEADER:
+            new_header = f"cellrank_{header}"
+            df_annot = df_annot.sort_values(header, ascending=False)
+            df_annot.loc[:, [new_header]] = range(1, adata.n_obs + 1)
+
+    # Sample QC table when more cells than args.plot_celllimit are present
+    df_annot = atlas_sampling(df_annot, "QC", args)
+    df_annot.loc[:, [CELLINDEX_HEADER]] = range(1, len(df_annot) + 1)
     df_annot.to_csv(qc_path, index=False, quoting=False, sep="\t")
 
 
 def create_qc_plots(adata, atlas_path, atlas_info, args) -> None:
     """
     Display the atlas QC
     Search for the OBS variable which correspond to the toal_RNA, total_UMI,
@@ -613,7 +637,24 @@
             df_line = pd.DataFrame(dict_line)
             df_dimred = pd.concat(
                 [df_dimred, df_line], ignore_index=True, axis=0
             )
         df_dimred.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obsm_key was found for {atlas_name}")
+
+
+def atlas_sampling(df_annot, type_df, args):
+    """_summary_
+
+    Args:
+        df_annot (_type_): _description_
+        args (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    if args.plot_celllimit != 0 and args.plot_celllimit < len(df_annot):
+        logger.debug(f"Sample {type_df} table with {len(df_annot)} cells")
+        df_annot = df_annot.sample(args.plot_celllimit)
+        logger.debug(f"{type_df} table sampled to {len(df_annot)} cells")
+    return df_annot
```

### Comparing `checkatlas-0.2.5/checkatlas/atlas_seurat.py` & `checkatlas-0.2.6/checkatlas/atlas_seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/folders.py` & `checkatlas-0.2.6/checkatlas/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.2.6/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/metrics.py` & `checkatlas-0.2.6/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.2.6/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.2.6/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.2.6/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.2.6/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.5/pyproject.toml` & `checkatlas-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.2.5"
+version = "0.2.6"
 description="One liner tool to check the quality of your single-cell atlases."
-authors = ["becavinlab"]
+authors = ["becavin-lab"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "checkatlas"}]
-include = ["checkatlas/convertSeurat.R", "checkatlas/checkatlas_workflow.nf"]
+include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
 homepage = "https://checkatlas.readthedocs.io/"
 repository = "https://github.com/becavin-lab/checkatlas/"
 documentation = "https://checkatlas.readthedocs.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-multiqc = "^1.14"
 scikit-learn = "^1.2.1"
 rpy2 = "^3.5.8"
 llvmlite = "^0.39.1"
 numba = "^0.56.4"
 types-pyyaml = "^6.0.12.6"
 scanpy = "^1.9.1"
 numpy = "^1.23.5"
-poetry = "^1.5.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.3.2"
 gitchangelog = "^3.0.4"
@@ -50,11 +48,7 @@
 [tool.mypy]
 no_implicit_optional = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry.scripts]
-checkatlas = 'checkatlas.__main__:main'
-checkatlas-workflow = 'checkatlas.checkatlas_workflow:workflow'
-
```

### Comparing `checkatlas-0.2.5/setup.py` & `checkatlas-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,40 +10,32 @@
  'checkatlas.metrics.specificity']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['llvmlite>=0.39.1,<0.40.0',
- 'multiqc>=1.14,<2.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
- 'poetry>=1.5.1,<2.0.0',
  'rpy2>=3.5.8,<4.0.0',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
-entry_points = \
-{'console_scripts': ['checkatlas = checkatlas.__main__:main',
-                     'checkatlas-workflow = '
-                     'checkatlas.checkatlas_workflow:workflow']}
-
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "\n# CheckAtlas\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
-    'author': 'becavinlab',
+    'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `checkatlas-0.2.5/PKG-INFO` & `checkatlas-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.2.5
+Version: 0.2.6
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: MIT
-Author: becavinlab
+Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
-Requires-Dist: multiqc (>=1.14,<2.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: poetry (>=1.5.1,<2.0.0)
 Requires-Dist: rpy2 (>=3.5.8,<4.0.0)
 Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.6,<7.0.0.0)
 Project-URL: Documentation, https://checkatlas.readthedocs.io/
 Project-URL: Repository, https://github.com/becavin-lab/checkatlas/
 Description-Content-Type: text/markdown
```

