# Comparing `tmp/drive_ibd-2.0.8.tar.gz` & `tmp/drive_ibd-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.0.8.tar", max compression
+gzip compressed data, was "drive_ibd-2.0.9.tar", max compression
```

## Comparing `drive_ibd-2.0.8.tar` & `drive_ibd-2.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.8/README.md
--rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.0.8/drive/__init__.py
--rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.8/drive/cluster/__init__.py
--rw-r--r--   0        0        0    17957 2023-07-03 15:03:19.205767 drive_ibd-2.0.8/drive/cluster/cluster.py
--rw-r--r--   0        0        0    10198 2023-07-03 15:01:39.900312 drive_ibd-2.0.8/drive/drive.py
--rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.8/drive/factory/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-30 15:43:04.548543 drive_ibd-2.0.8/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.8/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.8/drive/filters/__init__.py
--rw-r--r--   0        0        0    17195 2023-07-03 15:01:54.507938 drive_ibd-2.0.8/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.8/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.8/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.8/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.8/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.8/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.8/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.8/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.8/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.8/drive/log/logger.py
--rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.8/drive/models/__init__.py
--rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.8/drive/models/choices.py
--rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.8/drive/models/data_container.py
--rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.8/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.8/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.8/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.8/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4370 2023-07-03 15:02:21.451248 drive_ibd-2.0.8/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.8/drive/plugins/pvalues.py
--rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.8/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.8/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2277 2023-07-03 15:04:54.879313 drive_ibd-2.0.8/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.8/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     9203 2023-07-03 15:05:10.730906 drive_ibd-2.0.8/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.8/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2136 2023-07-03 15:05:19.198688 drive_ibd-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 drive_ibd-2.0.8/setup.py
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-07-03 15:40:21.545293 drive_ibd-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.0.9/drive/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.9/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    17952 2023-07-03 15:08:07.874354 drive_ibd-2.0.9/drive/cluster/cluster.py
+-rw-r--r--   0        0        0    10199 2023-07-03 15:08:07.638361 drive_ibd-2.0.9/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.9/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-30 15:43:04.548543 drive_ibd-2.0.9/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.9/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.9/drive/filters/__init__.py
+-rw-r--r--   0        0        0    17195 2023-07-03 15:08:08.606336 drive_ibd-2.0.9/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.9/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.9/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.9/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.9/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.9/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.9/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.9/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.9/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.9/drive/log/logger.py
+-rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.9/drive/models/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.9/drive/models/choices.py
+-rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.9/drive/models/data_container.py
+-rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.9/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.9/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.9/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.9/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4370 2023-07-03 15:02:21.451248 drive_ibd-2.0.9/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    10102 2023-07-06 13:55:30.401780 drive_ibd-2.0.9/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.9/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.9/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2263 2023-07-03 15:08:00.474545 drive_ibd-2.0.9/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.9/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     9303 2023-07-03 15:09:53.823629 drive_ibd-2.0.9/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.9/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2137 2023-07-06 13:56:48.547834 drive_ibd-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 drive_ibd-2.0.9/setup.py
+-rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 drive_ibd-2.0.9/PKG-INFO
```

### Comparing `drive_ibd-2.0.8/drive/cluster/cluster.py` & `drive_ibd-2.0.9/drive/cluster/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import itertools
 import logging
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Set, Tuple
 
 import igraph as ig
+from pandas import DataFrame
+
 from drive.log import CustomLogger
 from drive.models import Filter, Network, Network_Interface
-from pandas import DataFrame
 
 # creating a logger
 logger: logging.Logger = CustomLogger.get_logger(__name__)
 
 # Create a generic variable that can represents the class from the
 
 
@@ -85,15 +86,15 @@
         logger.verbose(random_walk_clusters.summary())
 
         return random_walk_clusters
 
     def filter_cluster_size(
         self, random_walk_clusters_sizes: ig.VertexClustering
     ) -> List[int]:
-        """Method to filter networks that are smaller than the min_cluster_size from 
+        """Method to filter networks that are smaller than the min_cluster_size from
         the analysis
 
         Parameters
         ----------
         random_walk_clusters_sizes : List[int]
             size of each cluster from the random walk results
 
@@ -229,15 +230,15 @@
     ) -> Tuple[List[str], Set[str]]:
         """remap the haplotype integer ids back to the haplotype
         strings for the output file
 
         Parameters
         ----------
         members : List[int]
-            list of integers that represent the name of each vertex in the network 
+            list of integers that represent the name of each vertex in the network
             corresponding the the graph
 
         Returns
         -------
         Tuple[List[str], List[str]]
             returns a list of haplotype id strings in the network. These
             strings include the phase number. Also returns a list of ids
@@ -309,15 +310,15 @@
             # added to the final_clst list
             if (
                 self.check_times < self.max_rechecks
                 and true_pos_ratio < self.minimum_connected_thres
                 and len(member_list) > self.max_network_size
                 and self.recluster
             ):
-                # We can put all of this information into a network class. Here the 
+                # We can put all of this information into a network class. Here the
                 # member list will still be in integers
                 network = Network(
                     clst_name,
                     true_pos_count,
                     true_pos_ratio,
                     false_neg_list,
                     false_neg_count,
@@ -353,16 +354,16 @@
         """Method that will redo the clustering, if the
         networks were too large or did not show a high degree
         of connectedness
 
         Parameters
         ----------
         network : Network_InterFace
-            object that represents each cluster. These objects have information 
-            about the cluster id, number and ratio of edges, true_positive_percent, 
+            object that represents each cluster. These objects have information
+            about the cluster id, number and ratio of edges, true_positive_percent,
             false_negative_edges, false_negative_count
 
         ibd_pd : pd.DataFrame
             DataFrame that has information about the edges that a pair shares
         """
         # pulling the id from the original cluster
         original_id = network.clst_id
@@ -452,15 +453,15 @@
     filter_obj : Filter
         Filter object that has two attributes: ibd_pd and ibd_vs. These
         attributes are two dataframes that have information about the
         edges and information about the vertices.
 
     cluster_obj : ClusterHandler
         Object that contains information about how the random walk
-        needs to be performed. It will use the construct networks and return those 
+        needs to be performed. It will use the construct networks and return those
         values in a list.
 
     min_network_size : int
         threshold so we can filter networks that are >= the threshold
 
         Returns
     """
```

### Comparing `drive_ibd-2.0.8/drive/drive.py` & `drive_ibd-2.0.9/drive/drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import re
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
-import drive.factory as factory
 import typer
+
+import drive.factory as factory
 from drive.cluster import ClusterHandler, cluster
 from drive.filters import IbdFilter
 from drive.log import CustomLogger
 from drive.models import Data, FormatTypes, Genes, OverlapOptions, create_indices
 from drive.utilities.callbacks import check_input_exists, check_json_path
 from drive.utilities.parser import PhenotypeFileParser, load_phenotype_descriptions
```

### Comparing `drive_ibd-2.0.8/drive/factory/factory.py` & `drive_ibd-2.0.9/drive/factory/factory.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/factory/loader.py` & `drive_ibd-2.0.9/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/filters/filter.py` & `drive_ibd-2.0.9/drive/filters/filter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Callable, Dict, Iterator, List, Optional, TypeVar
 
+from pandas import DataFrame, concat, read_csv
+
 from drive.log import CustomLogger
 from drive.models import FileIndices, Genes, OverlapOptions
-from pandas import DataFrame, concat, read_csv
 
 logger = CustomLogger.get_logger(__name__)
 
 # we are going to create two exception class for the vertex
 
 T = TypeVar("T", bound="IbdFilter")
 
@@ -382,15 +383,14 @@
             are greater than or equal to the threshold.
 
         cohort_ids : List[str]
             Lists of ids that make up the cohort. The ibd_file
             will be filtered to only this list.
         """
         for chunk in self.ibd_file:
-
             cohort_restricted_chunk = self._filter_for_cohort(chunk, cohort_ids)
 
             if cohort_restricted_chunk.empty:
                 continue
 
             size_filtered_chunk = self.filter(cohort_restricted_chunk, min_centimorgan)
```

### Comparing `drive_ibd-2.0.8/drive/log/README.md` & `drive_ibd-2.0.9/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.0.9/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.0.9/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/log/logger.py` & `drive_ibd-2.0.9/drive/log/logger.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/models/data_container.py` & `drive_ibd-2.0.9/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/models/generate_indices.py` & `drive_ibd-2.0.9/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/models/networks.py` & `drive_ibd-2.0.9/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/models/types.py` & `drive_ibd-2.0.9/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/plugins/network_writer.py` & `drive_ibd-2.0.9/drive/plugins/network_writer.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/plugins/pvalues.py` & `drive_ibd-2.0.9/drive/plugins/pvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
-from factory import factory_register
-from log import CustomLogger
-from models import Data_Interface, Network_Interface
+from drive.factory import factory_register
+from drive.log import CustomLogger
+from drive.models import Data_Interface, Network_Interface
 from numpy import float64
 from scipy.stats import binomtest
 
 logger = CustomLogger.get_logger(__name__)
 
 
 @dataclass
```

### Comparing `drive_ibd-2.0.8/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.0.9/drive/utilities/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/drive/utilities/load_phenotypes.py` & `drive_ibd-2.0.9/drive/utilities/load_phenotypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,64 +2,64 @@
 
 from pandas import DataFrame, Series
 
 
 def _identify_carriers_indx(
     carriers_series: Series, return_dict: Dict[str, List[str]]
 ) -> None:
-    """Function that will insert the key, value pair of the phenotype and the carriers 
+    """Function that will insert the key, value pair of the phenotype and the carriers
     into the dictionary
     Parameters
     ----------
     carriers_series : pd.Series
         row of dataframe that is used in the apply function in
         the generate_carrier_list function
 
     return_dict : dict[str, list[str]]
-        dictionary where the phecodes will be the keys and the values will be a list of 
+        dictionary where the phecodes will be the keys and the values will be a list of
         indices indicating which grids are carriers
     """
 
     return_dict[carriers_series.name] = carriers_series[
         carriers_series == 1
     ].index.tolist()
 
 
 def _identify_carriers_indx(
     carriers_series: Series, return_dict: Dict[str, List[str]]
 ) -> None:
-    """Function that will insert the key, value pair of the phenotype and the carriers 
+    """Function that will insert the key, value pair of the phenotype and the carriers
     into the dictionary
 
     Parameters
     ----------
     carriers_series : pd.Series
         row of dataframe that is used in the apply function in
         the generate_carrier_list function
 
     return_dict : dict[str, list[str]]
-        dictionary where the phecodes will be the keys and the values will be a list of 
+        dictionary where the phecodes will be the keys and the values will be a list of
         indices indicating which grids are carriers
     """
 
     return_dict[carriers_series.name] = carriers_series[
         carriers_series == "NA"
     ].index.tolist()
 
 
 def generate_carrier_dict(carriers_matrix: DataFrame) -> Dict[str, List[str]]:
-    """Function that will take the carriers_pheno_matrix and generate a dictionary that 
+    """Function that will take the carriers_pheno_matrix and generate a dictionary that
     has the list of indices for each carrier
 
     Parameters
     ----------
     carriers_matrix : pd.DataFrame
-        dataframe where the columns are the phecodes and have 0's or 1's for whether or 
+        dataframe where the columns are the phecodes and have 0's or 1's for whether or
         not they have the phecodes
-        
+
     Returns
     -------
     Tuple[dict[str, list[str]], dict[str, List[str]]
         dictionary where the keys are phecodes and the values are list of integers
     """
     return_dict = {}
```

### Comparing `drive_ibd-2.0.8/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.0.9/drive/utilities/parser/case_file_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 logger: Logger = CustomLogger.get_logger(__name__)
 
 # creating a type annotation for the PhenotypeFileParser class
 T = TypeVar("T", bound="PhenotypeFileParser")
 
 
 class PhenotypeFileParser:
-    """Parser used to read in the phenotype file. This will allow use to account for different delimiters in files as well as catch errors."""
+    """Parser used to read in the phenotype file. This will allow use to account for
+    different delimiters in files as well as catch errors."""
 
     def __init__(self, filepath: Union[Path, str]) -> None:
         """Initialize the PhenotypeFileParser class.
 
         Parameters
         ----------
         filepath : Path | str
@@ -38,15 +39,16 @@
         # the input file
         if not filepath.exists():
             raise FileNotFoundError(f"The file {filepath} was not found")
         else:
             self.file: Path = filepath
 
     def __enter__(self) -> T:
-        """Open the input file. Method determines the appropriate file type and open the file. Method is called automatically by the context manager.
+        """Open the input file. Method determines the appropriate file type and open
+        the file. Method is called automatically by the context manager.
 
         Raises
         ------
         OSError
             Raised if the program encounters an OSError while opening the file
         """
         suffix = self.file.suffix
@@ -55,26 +57,27 @@
             if suffix == ".gz":
                 file = gzip.open(self.file, "rt")
             else:
                 file = open(self.file, "r", encoding="utf-8")
         except OSError as e:
             logger.critical(e)
             logger.critical(
-                f"Encountered the following error while trying to open the file: {self.file}"
+                f"Encountered the following error while trying to open the file: {self.file}"  # noqa: E501
             )
             raise OSError(
-                f"Encountered the following error while trying to open the file: {self.file}"
+                f"Encountered the following error while trying to open the file: {self.file}"  # noqa: E501
             )
 
         self.opened_file = file
 
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
-        """Close the resource when it is not longer being used. Used by the context manager."""
+        """Close the resource when it is not longer being used. Used by the context
+        manager."""
         self.opened_file.close()
 
     @staticmethod
     def _check_separator(line: str) -> str:
         """Determine what the separator for the file should be.
 
         Parameters
@@ -99,15 +102,15 @@
             return ","
         elif len(line.split("\t")) > 1:
             return "\t"
         elif len(line.split("|")) > 1:
             return "|"
         else:
             raise ValueError(
-                "The was no appropriate separator found for the file. Currently DRIVE supports: ',' or '\t' or '|'"
+                "The was no appropriate separator found for the file. Currently DRIVE supports: ',' or '\t' or '|'"  # noqa: E501
             )
 
     def _determine_status(
         self,
         line: list[str],
         phenotype_dict: Dict[str, Dict[str, Set[str]]],
         phenotype_indx: Dict[int, str],
@@ -145,15 +148,15 @@
                 phenotype_dict[phenotype_mapping]["controls"].add(grid_id)
             # we are going to excluded on values na, n/a, -1, -1.
             # 0, "", " " to try to catch different values
             elif value.lower() in ["na", "n/a", "-1", "-1.0", " ", ""]:
                 phenotype_dict[phenotype_mapping]["excluded"].add(grid_id)
             else:
                 logger.warning(
-                    f"The status for individual, {grid_id}, was not recognized. The status found in the file was {value} for phenotype {phenotype_mapping}. This individual will be added to the exclusion list but it is recommended that the user checks to ensure that this is not a typo in the phenotype file."
+                    f"The status for individual, {grid_id}, was not recognized. The status found in the file was {value} for phenotype {phenotype_mapping}. This individual will be added to the exclusion list but it is recommended that the user checks to ensure that this is not a typo in the phenotype file."  # noqa: E501
                 )
                 phenotype_dict[phenotype_mapping]["excluded"].append(grid_id)
 
     def _create_phenotype_dictionary(
         self,
         header_line: str,
     ) -> Tuple[Dict[str, Dict[str, Set[str]]], Dict[int, str], str]:
@@ -178,17 +181,18 @@
         """
 
         # determining what the appropriate separator should be
         separator = PhenotypeFileParser._check_separator(header_line)
 
         logger.debug(f"Identified the separator, {separator}, in the file: {self.file}")
 
-        # raise an error if there is no header line, otherwise determine all the phenotypes
-        if not "grid" in header_line.lower() and not "grids" in header_line.lower():
-            error_msg = "Expected the first line of the phenotype file to have a header line with a column called grid or grids."
+        # raise an error if there is no header line, otherwise determine all the
+        # phenotypes
+        if "grid" not in header_line.lower() and "grids" not in header_line.lower():
+            error_msg = "Expected the first line of the phenotype file to have a header line with a column called grid or grids."  # noqa: E501
 
             logger.critical(error_msg)
 
             raise ValueError(error_msg)
         else:
             split_line_phenotypes = header_line.strip("\n").split(separator)[1:]
```

### Comparing `drive_ibd-2.0.8/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.0.9/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.8/pyproject.toml` & `drive_ibd-2.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drive-ibd"
-version = "2.0.8"
+version = "2.0.9"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://belowlab.github.io/drive/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
@@ -57,14 +57,15 @@
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "2.0.2"
 tag_format = "$version"
 update_changelog_on_bump = true
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 markers = [
     "integtest: marks test as integration test (deselected with '-m \"not integration\"')",
```

### Comparing `drive_ibd-2.0.8/setup.py` & `drive_ibd-2.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:app']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
-    'long_description': '# DRIVE:\n\nThis repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://belowlab.github.io/drive/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.',
+    'long_description': '[![Documentation Status](https://readthedocs.org/projects/drive-ibd/badge/?version=latest)](https://drive-ibd.readthedocs.io/en/latest/?badge=latest)\n\n# DRIVE:\n\nThis repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://drive-ibd.readthedocs.io/en/latest/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.\n\n',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://belowlab.github.io/drive/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `drive_ibd-2.0.8/PKG-INFO` & `drive_ibd-2.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.0.8
+Version: 2.0.9
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://belowlab.github.io/drive/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
@@ -22,22 +22,26 @@
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/belowlab/drive
 Description-Content-Type: text/markdown
 
+[![Documentation Status](https://readthedocs.org/projects/drive-ibd/badge/?version=latest)](https://drive-ibd.readthedocs.io/en/latest/?badge=latest)
+
 # DRIVE:
 
-This repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://belowlab.github.io/drive/)
+This repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://drive-ibd.readthedocs.io/en/latest/)
 
 ## Installing DRIVE:
 DRIVE is available on PYPI and can easily be installed using the following command:
 
 ```bash
 pip install drive-ibd
 ```
 
 If the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.
 
 ### Reporting issues:
 If you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.
+
+
```

