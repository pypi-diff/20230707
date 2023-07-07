# Comparing `tmp/cPredictor-0.1.2-py3-none-any.whl.zip` & `tmp/cPredictor-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17401 bytes, number of entries: 11
--rw-r--r--  2.0 unx    31531 b- defN 23-Jul-05 13:32 cPredictor/SVM_prediction.py
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-05 13:32 cPredictor/__init__.py
--rw-r--r--  2.0 unx     6379 b- defN 23-Jul-05 13:32 cPredictor/tests/SVM_prediction_test.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-05 13:32 cPredictor/tests/__init__.py
--rw-r--r--  2.0 unx     2347 b- defN 23-Jul-05 13:32 cPredictor/tests/cmaclp_test_model.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1666 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      937 b- defN 23-Jul-05 13:35 cPredictor-0.1.2.dist-info/RECORD
-11 files, 54907 bytes uncompressed, 15801 bytes compressed:  71.2%
+Zip file size: 17393 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    31485 b- defN 23-Jul-07 16:35 cPredictor/SVM_prediction.py
+-rw-r--r--  2.0 unx      354 b- defN 23-Jul-07 16:35 cPredictor/__init__.py
+-rw-r--r--  2.0 unx     6315 b- defN 23-Jul-07 16:35 cPredictor/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 16:35 cPredictor/tests/__init__.py
+-rw-r--r--  2.0 unx     2351 b- defN 23-Jul-07 16:35 cPredictor/tests/cPredictor_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1666 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/RECORD
+11 files, 54799 bytes uncompressed, 15785 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: cPredictor/tests/SVM_prediction_test.py
 Comment: 
 
 Filename: cPredictor/tests/__init__.py
 Comment: 
 
-Filename: cPredictor/tests/cmaclp_test_model.py
+Filename: cPredictor/tests/cPredictor_test_model.py
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/LICENSE
+Filename: cPredictor-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/METADATA
+Filename: cPredictor-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/WHEEL
+Filename: cPredictor-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/entry_points.txt
+Filename: cPredictor-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/top_level.txt
+Filename: cPredictor-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cPredictor-0.1.2.dist-info/RECORD
+Filename: cPredictor-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cPredictor/SVM_prediction.py

```diff
@@ -18,29 +18,29 @@
 from scanpy import read_h5ad
 from importlib.resources import files
 import re
 from statistics import mean
 from scipy.stats import pearsonr
 from scipy.stats import spearmanr
 
-def SVM_prediction(reference_H5AD, query_H5AD, LabelsPathTrain, OutputDir, rejected=False, Threshold_rej=0.7,meta_atlas=False):
+def SVM_predict(reference_H5AD, query_H5AD, LabelsPath, OutputDir, rejected=False, Threshold_rej=0.7,meta_atlas=False):
     '''
     run baseline classifier: SVM
     Wrapper script to run an SVM classifier with a linear kernel on a benchmark dataset with 5-fold cross validation,
     outputs lists of true and predicted cell labels as csv files, as well as computation time.
 
     Parameters:
     reference_H5AD, query_H5AD : H5AD files that produce training and testing data,
         cells-genes matrix with cell unique barcodes as row names and gene names as column names.
-    LabelsPathTrain : Cell population annotations file path matching the training data (.csv).
+    LabelsPath : Cell population annotations file path matching the training data (.csv).
     OutputDir : Output directory defining the path of the exported file.
     rejected: If the flag is added, then the SVMrejected option is chosen. Default: False.
     Threshold_rej : Threshold used when rejecting the cells, default is 0.7.
     meta_atlas : If the flag is added the predictions will use meta-atlas data.
-    meaning that reference_H5AD and LabelsPathTrain do not need to be specified.
+    meaning that reference_H5AD and LabelsPath do not need to be specified.
     '''
     print("Reading in the reference and query H5AD objects")
     
     # Load in the cma.h5ad object or use a different reference
     if meta_atlas is False:
         training=read_h5ad(reference_H5AD) 
     if meta_atlas is True:
@@ -86,17 +86,17 @@
     
     # read the data
     data_train = matrix_train2
     data_test = matrix_test2
     
     # If meta_atlas=True it will read the training_labels
     if meta_atlas is True:
-        LabelsPathTrain = 'data/training_labels_meta.csv'
+        LabelsPath = 'data/training_labels_meta.csv'
     
-    labels_train = pd.read_csv(LabelsPathTrain, header=0,index_col=None, sep=',')
+    labels_train = pd.read_csv(LabelsPath, header=0,index_col=None, sep=',')
         
     # Set threshold for rejecting cells
     if rejected is True:
         Threshold = Threshold_rej
 
     print("Log normalizing the training and testing data")
     
@@ -656,33 +656,33 @@
 def predpars():
     # Create the parser
     parser = argparse.ArgumentParser(description='Run SVM prediction')
 
     # Add arguments
     parser.add_argument('--reference_H5AD', type=str, help='Path to reference H5AD file')
     parser.add_argument('--query_H5AD', type=str, help='Path to query H5AD file')
-    parser.add_argument('--LabelsPathTrain', type=str, help='Path to cell population annotations file')
+    parser.add_argument('--LabelsPath', type=str, help='Path to cell population annotations file')
     parser.add_argument('--OutputDir', type=str, help='Path to output directory')
 
     parser.add_argument('--rejected', dest='rejected', action='store_true', help='Use SVMrejected option')
     parser.add_argument('--Threshold_rej', type=float, default=0.7, help='Threshold used when rejecting cells, default is 0.7')
     parser.add_argument('--meta_atlas', dest='meta_atlas', action='store_true', help='Use meta_atlas data')
 
     # Parse the arguments
     args = parser.parse_args()
     
     # check that output directory exists, create it if necessary
     if not os.path.isdir(args.OutputDir):
         os.makedirs(args.OutputDir)
 
     # Call the svm_prediction function with the parsed arguments
-    SVM_prediction(
+    SVM_predict(
         args.reference_H5AD,
         args.query_H5AD,
-        args.LabelsPathTrain,
+        args.LabelsPath,
         args.OutputDir,
         args.rejected,
         args.Threshold_rej,
         args.meta_atlas)
 
 
 def performpars():
@@ -732,15 +732,15 @@
 def pseudopars():
 
     parser = argparse.ArgumentParser(description="Performs individual and joined pseudobulk on two H5AD objects")
     parser.add_argument("--condition_1", type=str, help="Path to meta-atlas or other H5AD file")
     parser.add_argument("--condition_1_batch", type=str, help="Technical, biological or other replicate column in condition_1.obs")
     parser.add_argument("--condition_2", type=str, help="Path to H5AD file with SVM predictions")
     parser.add_argument("--condition_2_batch", type=str, help="Technical, biological or other replicate column in condition_2.obs")
-    parser.add_argument("--Labels_1", type=str, help="Label path for the meta-atlas (LabelsPathTrain) or condition_1.obs column with names")
+    parser.add_argument("--Labels_1", type=str, help="Label path for the meta-atlas (LabelsPath) or condition_1.obs column with names")
     parser.add_argument('--OutputDir', dest='pseudobulk_output/', action='store_true', help='Directory where pseudobulk results are outputted')
     parser.add_argument("--min_cells", type=float, default=50, help="Minimal amount of cells for each condition and replicate")
     parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
     
     args = parser.parse_args()
 
     SVM_pseudobulk(
@@ -763,9 +763,9 @@
 
 
 if __name__ == '__importpars__':
     importpars()
 
 
 if __name__ == '__pseudopars__':
-    importpars()
+    pseudopars()
```

## cPredictor/__init__.py

```diff
@@ -1,10 +1,10 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
-from .SVM_prediction import SVM_prediction
+from .SVM_prediction import SVM_predict
 from .SVM_prediction import SVM_import
 from .SVM_prediction import SVM_performance
 from .SVM_prediction import SVM_pseudobulk
 from .SVM_prediction import predpars
 from .SVM_prediction import importpars
 from .SVM_prediction import performpars
 from .SVM_prediction import pseudopars
```

## cPredictor/tests/SVM_prediction_test.py

```diff
@@ -15,15 +15,15 @@
 import re
 import matplotlib.pyplot as plt
 from statistics import mean
 from scipy.stats import pearsonr
 from scipy.stats import spearmanr
 
 # Import standalone functions for unit tests
-from cPredictor.SVM_prediction import SVM_prediction
+from cPredictor.SVM_prediction import SVM_predict
 from cPredictor.SVM_prediction import SVM_import
 from cPredictor.SVM_prediction import SVM_pseudobulk
 from cPredictor.SVM_prediction import SVM_performance
 from cPredictor.SVM_prediction import predpars
 from cPredictor.SVM_prediction import importpars
 from cPredictor.SVM_prediction import performpars
 
@@ -32,38 +32,38 @@
 reference = "data/cma_meta_atlas.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir_unit = "test_output_unit/"
 colord_tsv= "data/colord.tsv"
 
 ### UNIT TESTS
 
-def test_SVM_prediction():
-    SVM_prediction(reference_H5AD=reference,query_H5AD=query,
-      LabelsPathTrain=labels,OutputDir=outdir_unit)
+def test_SVM_predict():
+    SVM_predict(reference_H5AD=reference,query_H5AD=query,
+      LabelsPath=labels,OutputDir=outdir_unit)
 
     assert os.path.exists(f'{outdir_unit}SVM_Pred_Labels.csv') == 1
 
 
-def test_SVM_prediction_meta_atlas():
-    SVM_prediction(query_H5AD=query,meta_atlas=True,
+def test_SVM_predict_meta_atlas():
+    SVM_predict(query_H5AD=query,meta_atlas=True,
       OutputDir=outdir_unit)
 
     assert os.path.exists(f'{outdir_unit}SVM_Pred_Labels.csv') == 1
 
 
-def test_SVMrej_prediction():
-    SVM_prediction(reference_H5AD=reference,query_H5AD=query,
-      LabelsPathTrain=labels,OutputDir=outdir_unit,rejected=True)
+def test_SVMrej_predict():
+    SVM_predict(reference_H5AD=reference,query_H5AD=query,
+      LabelsPath=labels,OutputDir=outdir_unit,rejected=True)
 
     assert os.path.exists(f'{outdir_unit}SVMrej_Pred_Labels.csv') == 1
 
 
-def test_SVM_prediction_meta_atlas():
-    SVM_prediction(reference_H5AD=reference,query_H5AD=query,
-      LabelsPathTrain=labels,OutputDir=outdir_unit,rejected=True)
+def test_SVM_predict_meta_atlas():
+    SVM_predict(reference_H5AD=reference,query_H5AD=query,
+      LabelsPath=labels,OutputDir=outdir_unit,rejected=True)
 
     assert os.path.exists(f'{outdir_unit}SVMrej_Pred_Labels.csv') == 1
 
     
 def test_SVM_import():
 
     SVM_import(query_H5AD=query,OutputDir=outdir_unit,SVM_type="SVM",replicates="time_point")
@@ -107,33 +107,33 @@
 
     SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir_unit)
     assert os.path.exists("figures/SVMrej_cnf_matrix.png") == 1
 
 ### END-TO-END
 outdir = "test_output_end_to_end/"
 
-def test_CLI_SVM_prediction():
+def test_CLI_SVM_predict():
 
-    command_to_be_executed = ['SVM_prediction',
+    command_to_be_executed = ['SVM_predict',
                               '--reference_H5AD', str(reference),
                               '--query_H5AD', str(query),
-                              '--LabelsPathTrain', str(labels),
+                              '--LabelsPath', str(labels),
                               '--OutputDir', str(outdir)]
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
     assert os.path.exists(f'{outdir}SVM_Pred_Labels.csv') == 1
 
 
-def test_CLI_SVMrej_prediction():
+def test_CLI_SVMrej_predict():
 
-    command_to_be_executed = ['SVM_prediction',
+    command_to_be_executed = ['SVM_predict',
                               '--reference_H5AD', str(reference),
                               '--query_H5AD', str(query),
-                              '--LabelsPathTrain', str(labels),
+                              '--LabelsPath', str(labels),
                               '--OutputDir', str(outdir),
                               '--rejected']
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
     assert os.path.exists(f'{outdir}SVMrej_Pred_Labels.csv') == 1
```

## Comparing `cPredictor/tests/cmaclp_test_model.py` & `cPredictor/tests/cPredictor_test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
 from scanpy import read_h5ad
 from importlib.resources import files
 
 print("Import performance function")
-from cmaclp.SVM_prediction import SVM_performance
+from cPredictor.SVM_prediction import SVM_performance
 os.environ["GIT_PYTHON_REFRESH"] = "quiet"
 import git
 
 reference = "data/cma_meta_atlas.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir = "test_output/"
-cPredictor_version = "0.1.2"
+cPredictor_version = "0.1.3"
 
 metrics = SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir)
 
 print("Setup tokens")
 # Set environments and passwords
 DAGSHUB_USER_NAME = 'Arts-of-coding'
 DAGSHUB_TOKEN =  os.environ['DH_key']
```

## Comparing `cPredictor-0.1.2.dist-info/LICENSE` & `cPredictor-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cPredictor-0.1.2.dist-info/METADATA` & `cPredictor-0.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cPredictor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cell command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools (<=57.5.0)
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

## Comparing `cPredictor-0.1.2.dist-info/RECORD` & `cPredictor-0.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-cPredictor/SVM_prediction.py,sha256=pnK-WHcbc7_gib-RQocufgjPpbPtJXelyZTHOx6s1wg,31531
-cPredictor/__init__.py,sha256=YPHM-qcVu0H_X7nlaZivyO9VYONeFVX_G9jF4GMVWhY,357
-cPredictor/tests/SVM_prediction_test.py,sha256=Vz_vAk0mkE5ld2QFsvXbk2JR7pYiAPX9_VQIZlRjjwo,6379
+cPredictor/SVM_prediction.py,sha256=ELe7jNHNEMfxIqNIYh68DrUBz1DkUJJSGKYzq3kYCF0,31485
+cPredictor/__init__.py,sha256=PjBteb1KRYocvJh79pgVH6z1tLyXbW6SEeiAlEbpgos,354
+cPredictor/tests/SVM_prediction_test.py,sha256=Jhog2SlFpTe1maaXKpPyZxEo0kwXVyhjd42Kk1W8btY,6315
 cPredictor/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cPredictor/tests/cmaclp_test_model.py,sha256=uxxur0vWjxqZAb9mb6NnDv4MTWaoi1cy7I5w5CnHBAA,2347
-cPredictor-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cPredictor-0.1.2.dist-info/METADATA,sha256=hUktb95pwevN9o0decv8aO6MNlws3K3jpvHA39ytJHM,1666
-cPredictor-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cPredictor-0.1.2.dist-info/entry_points.txt,sha256=SiNbGVA5macxTuliLj3umFAxaKJ0si_i3oc_AMsccRk,230
-cPredictor-0.1.2.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
-cPredictor-0.1.2.dist-info/RECORD,,
+cPredictor/tests/cPredictor_test_model.py,sha256=kQswXDldAYX0qZdjkDfghWd2VPrzzmV4yDDQI2YXYek,2351
+cPredictor-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cPredictor-0.1.3.dist-info/METADATA,sha256=bcg9_BzrdOmU2GZ22U9E-wDHmvVseu3NNU7Dyk8AL8k,1666
+cPredictor-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cPredictor-0.1.3.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
+cPredictor-0.1.3.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
+cPredictor-0.1.3.dist-info/RECORD,,
```

