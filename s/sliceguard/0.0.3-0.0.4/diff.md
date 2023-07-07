# Comparing `tmp/sliceguard-0.0.3.tar.gz` & `tmp/sliceguard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.3.tar", last modified: Wed Jul  5 07:51:23 2023, max compression
+gzip compressed data, was "sliceguard-0.0.4.tar", last modified: Fri Jul  7 08:13:34 2023, max compression
```

## Comparing `sliceguard-0.0.3.tar` & `sliceguard-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:51:23.476410 sliceguard-0.0.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.3/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      945 2023-07-05 07:51:23.476410 sliceguard-0.0.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      289 2023-07-05 07:44:42.000000 sliceguard-0.0.3/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2023-07-05 07:44:02.000000 sliceguard-0.0.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-05 07:51:23.476410 sliceguard-0.0.3/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:51:23.476410 sliceguard-0.0.3/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 07:45:16.000000 sliceguard-0.0.3/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5828 2023-07-04 14:10:22.000000 sliceguard-0.0.3/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-07-04 14:10:22.000000 sliceguard-0.0.3/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-04 14:10:22.000000 sliceguard-0.0.3/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7851 2023-07-04 14:10:22.000000 sliceguard-0.0.3/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-04 14:10:22.000000 sliceguard-0.0.3/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:51:23.476410 sliceguard-0.0.3/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      945 2023-07-05 07:51:23.000000 sliceguard-0.0.3/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-05 07:51:23.000000 sliceguard-0.0.3/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-05 07:51:23.000000 sliceguard-0.0.3/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      232 2023-07-05 07:51:23.000000 sliceguard-0.0.3/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-05 07:51:23.000000 sliceguard-0.0.3/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:51:23.476410 sliceguard-0.0.3/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4464 2023-07-05 07:46:11.000000 sliceguard-0.0.3/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.4/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2844 2023-07-07 08:13:34.066984 sliceguard-0.0.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2188 2023-07-07 08:09:57.000000 sliceguard-0.0.4/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-07 08:11:41.000000 sliceguard-0.0.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 08:13:34.066984 sliceguard-0.0.4/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.4/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9222 2023-07-07 08:09:57.000000 sliceguard-0.0.4/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-05 08:28:25.000000 sliceguard-0.0.4/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2844 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-07 08:13:34.000000 sliceguard-0.0.4/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 08:13:34.066984 sliceguard-0.0.4/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4644 2023-07-07 08:09:57.000000 sliceguard-0.0.4/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.3/LICENSE` & `sliceguard-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.3/pyproject.toml` & `sliceguard-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -22,15 +22,16 @@
   "umap-learn >= 0.5.3",
   "transformers >= 4.30.2",
   "torch >= 2.0.1",
   "torchaudio >= 2.0.2",
   "sentence-transformers >= 2.2.1",
   "tqdm >= 4.65.0",
   "Pillow >= 9.5.0",
-  "renumics-spotlight >= 1.3.0rc1",
+  "renumics-spotlight >= 1.3.0rc2",
+  "plotly >= 5.15.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Renumics/sliceguard"
 "Bug Tracker" = "https://github.com/Renumics/sliceguard/issues"
 
 [tool.setuptools]
```

### Comparing `sliceguard-0.0.3/sliceguard/detection.py` & `sliceguard-0.0.4/sliceguard/detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,29 @@
     :param df: The dataframe containing ground-truth and predictions.
     :param y: The name of the ground-truth column.
     :param y_pred: The name of the predictions column.
     :param metric: The metric function.
 
     """
     # Identify hierarchical clustering with h-nne
+    # As h-nne fails for less than 2 dimenions introduce dummy dimension in this case
+    num_features = encoded_data.shape[1]
+    if num_features <= 1:
+        encoded_data = np.concatenate(
+            (encoded_data, np.zeros((encoded_data.shape[0], 1))), axis=1
+        )
+
     hnne = HNNE(
         metric="euclidean"
     )  # TODO Probably explore different settings for hnne. Default of metric is cosine. To determine if this is better choice!
     projection = hnne.fit_transform(encoded_data)
+    partitions = hnne.hierarchy_parameters.partitions
+
     partitions = np.flip(
-        hnne.hierarchy_parameters.partitions, axis=1
+        partitions, axis=1
     )  # reverse the order of the hierarchy levels, go from coarse to fine
     partition_sizes = hnne.hierarchy_parameters.partition_sizes
     partition_levels = len(partition_sizes)
 
     clustering_cols = [f"clustering_{i}" for i in range(partition_levels)]
     clustering_df = pd.DataFrame(
         data=partitions, columns=clustering_cols, index=df.index
@@ -77,15 +86,15 @@
     computed hierarchical clustering.
     :param mfs: List of fairlearn MetricFrames computed on different cluster levels.
     :param clustering_df: The dataframe containing the previously created hierarchical clustering.
     :param clustering_cols: List of columns in clustering_df that correspond to different hierarchy levels.
     :param min_drop: Minimum drop that has to be present so the cluster is marked as problematic.
     :param min_support: Minimum number of samples in one cluster so that it is marked as issue.
     :param metric_mode: Optimization goal for the metric. Can be "min" or "max".
-    
+
     """
     # Determine the hierarchy levels that most likely capture real problems
     # TODO: Determine if these values should be chosen adaptively, potentially differing on every level
     group_dfs = []
 
     if min_drop is None:
         min_drop = 0.1 * mfs[0].overall.values[0]
```

### Comparing `sliceguard-0.0.3/sliceguard/embedding_utils.py` & `sliceguard-0.0.4/sliceguard/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.3/sliceguard/explanation.py` & `sliceguard-0.0.4/sliceguard/explanation.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.3/sliceguard/sliceguard.py` & `sliceguard-0.0.4/sliceguard/sliceguard.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from typing import List, Literal, Dict, Callable
 
 import pandas as pd
 import numpy as np
+import plotly.express as px
 
 from renumics import spotlight
 from renumics.spotlight.analysis.typing import DataIssue
+from renumics.spotlight import layout
 
 from .utils import infer_feature_types, encode_normalize_features
 from .detection import generate_metric_frames, detect_issues
 from .explanation import explain_clusters
 
 
 class SliceGuard:
     """
     The main class for detecting issues in your data
     """
 
-    def generate_summary_report(
-        data, raw_data, precomputed_embeddings, features, metadata
-    ):
-        """
-        Generate a report on biases, potential underrepresented populations, problematic features, hidden stratification etc.
-        """
-        raise RuntimeError("This functionality has not been implemented yet.")
-
     # TODO: Introduce control features to account for expected variations
     def find_issues(
         self,
         data: pd.DataFrame,
         features: List[str],
         y: str,
         y_pred: str,
@@ -83,14 +77,18 @@
         (
             mfs,
             clustering_df,
             clustering_cols,
             clustering_metric_cols,
         ) = generate_metric_frames(encoded_data, df, y, y_pred, metric)
 
+        if len(mfs) > 0:
+            overall_metric = mfs[0].overall.values[0]
+            print(f"The overall metric value is {overall_metric}")
+
         group_dfs = detect_issues(
             mfs, clustering_df, clustering_cols, min_drop, min_support, metric_mode
         )
 
         num_issues = np.sum([group_df["issue"].sum() for group_df in group_dfs])
 
         print(f"Identified {num_issues} problematic slices.")
@@ -120,14 +118,16 @@
         # This is done to help understanding of the problem reason
         # First stage this will be only importance values!
         issue_df = explain_clusters(
             features, feature_types, issue_df, df, prereduced_embeddings
         )
 
         self._issue_df = issue_df
+        self._clustering_df = clustering_df
+        self._clustering_cols = clustering_cols
         self._metric_mode = metric_mode
         self._df = df
         self.embeddings = raw_embeddings
 
         return issue_df
 
     def report(self, spotlight_dtype: Dict[str, spotlight.dtypes.base.DType] = {}):
@@ -173,8 +173,43 @@
         if self._metric_mode == "min":
             data_issue_order = data_issue_order[::-1]
 
         spotlight.show(
             df,
             dtype=spotlight_dtype,
             issues=np.array(data_issues)[data_issue_order].tolist(),
+            layout=layout.layout(
+                [
+                    [layout.table()],
+                    [layout.similaritymap()],
+                    [layout.histogram()],
+                ],
+                [[layout.widgets.Inspector()], [layout.widgets.Issues()]],
+            ),
         )
+
+    def _plot_clustering_overview(self):
+        """
+        Debugging method to get an overview on the last clustering structure.
+        """
+        # for i in range(len(self._clustering_cols)):
+        # cur_clustering_cols = self._clustering_cols[:i+1]
+        cur_clustering_cols = self._clustering_cols
+        plotting_df = pd.concat((self._clustering_df, self._issue_df), axis=1)
+        plotting_df["is_issue"] = plotting_df["issue"] != -1
+        plotting_df["issue_metric_str"] = plotting_df["issue_metric"].apply(
+            lambda x: "{0:.2f}".format(x)
+            if (isinstance(x, float) or isinstance(x, np.floating)) and not np.isnan(x)
+            else ""
+        )
+        fig = px.treemap(
+            plotting_df,
+            path=cur_clustering_cols,
+            color="is_issue",
+            color_discrete_map={"(?)": "lightgrey", True: "gold", False: "darkblue"},
+            custom_data="issue_metric_str",
+        )
+        fig.data[0].texttemplate = "%{customdata[0]}"
+        fig.data[0].textinfo = "none"
+        # fig.write_image(f"clustering_{i}.png", scale=4)
+
+        fig.show()
```

### Comparing `sliceguard-0.0.3/sliceguard/utils.py` & `sliceguard-0.0.4/sliceguard/utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.3/tests/test_sliceguard.py` & `sliceguard-0.0.4/tests/test_sliceguard.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,35 @@
 import shutil
 from pathlib import Path
 from urllib.parse import urlparse
 
 from sklearn.metrics import accuracy_score
 import requests
 import pandas as pd
+import matplotlib.pyplot as plt
 import numpy as np
 from jiwer import wer
 import datasets
-from renumics import spotlight
-from renumics.spotlight import Embedding, Image, Audio
+from renumics.spotlight import Image, Audio
 
 from sliceguard import SliceGuard
 
 
 def wer_metric(y_true, y_pred):
     return np.mean([wer(s_y, s_pred) for s_y, s_pred in zip(y_true, y_pred)])
 
 
 def test_sliceguard_text():
     df = pd.read_json("tests/predictions.json")
+
+    # df = df.drop(
+    #     columns=["up_votes", "down_votes", "locale", "segment", "variant", "audio"]
+    # )
+    # df.sample(500).to_json("example_data.json", orient="records")
+
     df = df[df["accent"] != ""]
     df = df[df["age"] != ""]
     df = df[df["gender"] != ""]
 
     df["audio"] = "tests/" + df["audio"]
 
     sg = SliceGuard()
@@ -46,25 +52,25 @@
                 "fifties",
                 "sixties",
                 "seventies",
                 "eighties",
                 "nineties",
             ]
         },
-        min_support=10,
-        min_drop=0.08,
+        min_support=30,
+        min_drop=0.04,
     )
 
-    df["age"] = df["age"].astype("category")
-    df["gender"] = df["gender"].astype("category")
-    df["accent"] = df["accent"].astype("category")
+    # df["age"] = df["age"].astype("category")
+    # df["gender"] = df["gender"].astype("category")
+    # df["accent"] = df["accent"].astype("category")
 
-    sg.report(
-        spotlight_dtype={"audio": Audio},
-    )
+    sg.report(spotlight_dtype={"audio": Audio})
+
+    # sg._plot_clustering_overview()
 
 
 def test_sliceguard_images():
     dataset = datasets.load_dataset("olivierdehaene/xkcd", split="train")
     df = dataset.to_pandas()
     image_urls = df["image_url"]
     data_dir = Path("test_data/xkcd")
@@ -90,27 +96,26 @@
         df = df.iloc[valid_indices]
         df["image_path"] = target_paths
         df.to_json(data_dir / "metadata.json")
     df = pd.read_json(data_dir / "metadata.json")
 
     df = df[~pd.isnull(df["transcript"])]
     df = df[~pd.isnull(df["explanation"])]
-    df = df.sample(500)
 
     sg = SliceGuard()
     issue_df = sg.find_issues(
         df,
         ["image_path"],
         "explanation",
         "transcript",
         wer_metric,
         metric_mode="min",
         # feature_types={"age": "ordinal"},
         # feature_orders={"age": ["", "teens", "twenties", "thirties", "fourties", "fifties", "sixties", "seventies", "eighties", "nineties"]},
-        min_support=5,
+        min_support=10,
         min_drop=0.08,
     )
 
     sg.report(spotlight_dtype={"image_path": Image})
 
 
 def test_sliceguard_audio():
```

