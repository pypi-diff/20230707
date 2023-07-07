# Comparing `tmp/checkatlas-0.2.4.tar.gz` & `tmp/checkatlas-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.2.4.tar", max compression
+gzip compressed data, was "checkatlas-0.2.5.tar", max compression
```

## Comparing `checkatlas-0.2.4.tar` & `checkatlas-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1211 2023-07-07 07:28:54.139178 checkatlas-0.2.4/LICENSE
--rw-r--r--   0        0        0     3841 2023-07-07 07:28:54.139178 checkatlas-0.2.4/README.md
--rw-r--r--   0        0        0      130 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/__init__.py
--rw-r--r--   0        0        0     8445 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/__main__.py
--rw-r--r--   0        0        0    20197 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/atlas.py
--rw-r--r--   0        0        0    17277 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/atlas_seurat.py
--rw-r--r--   0        0        0    12728 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/checkatlas.py
--rw-r--r--   0        0        0      931 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/checkatlas_workflow.nf
--rw-r--r--   0        0        0    10123 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0     1127 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/convertSeurat.R
--rw-r--r--   0        0        0     1905 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/folders.py
--rw-r--r--   0        0        0        0 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4103 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0      721 2023-07-07 07:28:54.139178 checkatlas-0.2.4/checkatlas/multiqc.py
--rw-r--r--   0        0        0     1414 2023-07-07 07:28:54.327178 checkatlas-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 checkatlas-0.2.4/setup.py
--rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 checkatlas-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-07 09:44:48.184445 checkatlas-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-07 09:44:48.184445 checkatlas-0.2.5/README.md
+-rw-r--r--   0        0        0      130 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/__init__.py
+-rw-r--r--   0        0        0     8445 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/__main__.py
+-rw-r--r--   0        0        0    20197 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/atlas.py
+-rw-r--r--   0        0        0    17277 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/atlas_seurat.py
+-rw-r--r--   0        0        0    12728 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0      931 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas_workflow.nf
+-rw-r--r--   0        0        0    10123 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0     1127 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/convertSeurat.R
+-rw-r--r--   0        0        0     1905 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/folders.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4103 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0      721 2023-07-07 09:44:48.184445 checkatlas-0.2.5/checkatlas/multiqc.py
+-rw-r--r--   0        0        0     1431 2023-07-07 09:44:48.384444 checkatlas-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 checkatlas-0.2.5/setup.py
+-rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 checkatlas-0.2.5/PKG-INFO
```

### Comparing `checkatlas-0.2.4/LICENSE` & `checkatlas-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/README.md` & `checkatlas-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/__main__.py` & `checkatlas-0.2.5/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/atlas.py` & `checkatlas-0.2.5/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/atlas_seurat.py` & `checkatlas-0.2.5/checkatlas/atlas_seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/checkatlas.py` & `checkatlas-0.2.5/checkatlas/checkatlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/checkatlas_workflow.nf` & `checkatlas-0.2.5/checkatlas/checkatlas_workflow.nf`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/checkatlas_workflow.py` & `checkatlas-0.2.5/checkatlas/checkatlas_workflow.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/convertSeurat.R` & `checkatlas-0.2.5/checkatlas/convertSeurat.R`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/folders.py` & `checkatlas-0.2.5/checkatlas/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.2.5/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/metrics.py` & `checkatlas-0.2.5/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.2.5/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.2.5/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.2.5/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.2.5/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/checkatlas/multiqc.py` & `checkatlas-0.2.5/checkatlas/multiqc.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.4/pyproject.toml` & `checkatlas-0.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.2.4"
+version = "0.2.5"
 description="One liner tool to check the quality of your single-cell atlases."
-authors = ["becavin-lab"]
+authors = ["becavinlab"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/convertSeurat.R", "checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
 homepage = "https://checkatlas.readthedocs.io/"
 repository = "https://github.com/becavin-lab/checkatlas/"
@@ -19,14 +19,15 @@
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

### Comparing `checkatlas-0.2.4/setup.py` & `checkatlas-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,31 @@
 {'': ['*']}
 
 install_requires = \
 ['llvmlite>=0.39.1,<0.40.0',
  'multiqc>=1.14,<2.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
+ 'poetry>=1.5.1,<2.0.0',
  'rpy2>=3.5.8,<4.0.0',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:workflow']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "\n# CheckAtlas\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
-    'author': 'becavin-lab',
+    'author': 'becavinlab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
```

### Comparing `checkatlas-0.2.4/PKG-INFO` & `checkatlas-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.2.4
+Version: 0.2.5
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: MIT
-Author: becavin-lab
+Author: becavinlab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: multiqc (>=1.14,<2.0)
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

