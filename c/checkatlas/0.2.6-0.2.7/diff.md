# Comparing `tmp/checkatlas-0.2.6.tar.gz` & `tmp/checkatlas-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.2.6.tar", max compression
+gzip compressed data, was "checkatlas-0.2.7.tar", max compression
```

## Comparing `checkatlas-0.2.6.tar` & `checkatlas-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1211 2023-07-07 13:52:57.938636 checkatlas-0.2.6/LICENSE
--rw-r--r--   0        0        0     3841 2023-07-07 13:52:57.938636 checkatlas-0.2.6/README.md
--rw-r--r--   0        0        0      117 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/__init__.py
--rw-r--r--   0        0        0    21675 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/atlas.py
--rw-r--r--   0        0        0    17277 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/atlas_seurat.py
--rw-r--r--   0        0        0     6682 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     1905 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/folders.py
--rw-r--r--   0        0        0        0 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4103 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-07 13:52:57.942636 checkatlas-0.2.6/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0     1239 2023-07-07 13:52:58.142641 checkatlas-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 checkatlas-0.2.6/setup.py
--rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 checkatlas-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-07 15:50:04.167115 checkatlas-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-07 15:50:04.167115 checkatlas-0.2.7/README.md
+-rw-r--r--   0        0        0      117 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/__init__.py
+-rw-r--r--   0        0        0    21675 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/atlas.py
+-rw-r--r--   0        0        0    17277 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/atlas_seurat.py
+-rw-r--r--   0        0        0     6631 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     1905 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/folders.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4103 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-07 15:50:04.167115 checkatlas-0.2.7/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0     1257 2023-07-07 15:50:04.355118 checkatlas-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 checkatlas-0.2.7/setup.py
+-rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 checkatlas-0.2.7/PKG-INFO
```

### Comparing `checkatlas-0.2.6/LICENSE` & `checkatlas-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/README.md` & `checkatlas-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/atlas.py` & `checkatlas-0.2.7/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/atlas_seurat.py` & `checkatlas-0.2.7/checkatlas/atlas_seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/checkatlas.py` & `checkatlas-0.2.7/checkatlas/checkatlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,19 +153,18 @@
          list: list of functions to run
     """
     checkatlas_functions = list()
 
     if not args.NOADATA:
         checkatlas_functions.append(module.create_anndata_table)
     if not args.NOQC:
-        # if "violin_plot" in args.qc_display:
-        #    checkatlas_functions.append(module.create_qc_plots)
+        if "violin_plot" in args.qc_display:
+            checkatlas_functions.append(module.create_qc_plots)
         if (
             "total-counts" in args.qc_display
-            or "violin_plot" in args.qc_display
             or "n_genes_by_counts" in args.qc_display
             or "pct_counts_mt" in args.qc_display
         ):
             checkatlas_functions.append(module.create_qc_tables)
     if not args.NOREDUCTION:
         checkatlas_functions.append(module.create_umap_fig)
         checkatlas_functions.append(module.create_tsne_fig)
```

### Comparing `checkatlas-0.2.6/checkatlas/folders.py` & `checkatlas-0.2.7/checkatlas/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.2.7/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/metrics.py` & `checkatlas-0.2.7/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.2.7/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.2.7/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.2.7/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.2.7/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.6/pyproject.toml` & `checkatlas-0.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.2.6"
+version = "0.2.7"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
@@ -18,14 +18,15 @@
 scikit-learn = "^1.2.1"
 rpy2 = "^3.5.8"
 llvmlite = "^0.39.1"
 numba = "^0.56.4"
 types-pyyaml = "^6.0.12.6"
 scanpy = "^1.9.1"
 numpy = "^1.23.5"
+poetry = "^1.5.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.3.2"
 gitchangelog = "^3.0.4"
```

### Comparing `checkatlas-0.2.6/setup.py` & `checkatlas-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['llvmlite>=0.39.1,<0.40.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
+ 'poetry>=1.5.1,<2.0.0',
  'rpy2>=3.5.8,<4.0.0',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "\n# CheckAtlas\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.2.6/PKG-INFO` & `checkatlas-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.2.6
+Version: 0.2.7
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: MIT
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
 Requires-Dist: rpy2 (>=3.5.8,<4.0.0)
 Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.6,<7.0.0.0)
 Project-URL: Documentation, https://checkatlas.readthedocs.io/
 Project-URL: Repository, https://github.com/becavin-lab/checkatlas/
 Description-Content-Type: text/markdown
```

