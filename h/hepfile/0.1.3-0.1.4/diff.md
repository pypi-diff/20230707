# Comparing `tmp/hepfile-0.1.3.tar.gz` & `tmp/hepfile-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepfile-0.1.3.tar", last modified: Mon May 30 04:47:04 2022, max compression
+gzip compressed data, was "hepfile-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hepfile-0.1.3.tar` & `hepfile-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,14 @@
--rw-r--r--   0        0        0       36 2022-05-16 17:26:26.189677 hepfile-0.1.3/.flake8
--rw-r--r--   0        0        0      799 2021-07-09 20:45:06.521441 hepfile-0.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0     2176 2021-08-19 04:58:17.822927 hepfile-0.1.3/.gitignore
--rw-r--r--   0        0        0      432 2022-05-16 17:26:26.189677 hepfile-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       72 2022-05-30 04:43:44.315543 hepfile-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0      168 2021-08-19 05:14:50.927987 hepfile-0.1.3/DEV_NOTES.md
--rw-r--r--   0        0        0    11389 2021-07-16 15:24:43.780248 hepfile-0.1.3/LICENSE
--rw-r--r--   0        0        0     1874 2021-07-30 16:33:15.704666 hepfile-0.1.3/README.md
--rw-r--r--   0        0        0      633 2021-06-21 06:53:42.014253 hepfile-0.1.3/docs/Makefile
--rw-r--r--   0        0        0       21 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/citations.rst
--rw-r--r--   0        0        0     2390 2022-05-30 04:42:59.153484 hepfile-0.1.3/docs/conf.py
--rw-r--r--   0        0        0      324 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/contributors.rst
--rw-r--r--   0        0        0      353 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/examples.rst
--rw-r--r--   0        0        0     1709 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/examples/write_HEP.rst
--rw-r--r--   0        0        0     8064 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/fundamentals.rst
--rw-r--r--   0        0        0      443 2021-07-30 16:33:15.704666 hepfile-0.1.3/docs/hepfile.rst
--rw-r--r--   0        0        0    98663 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/images/household_example_spreadsheet_00.png
--rw-r--r--   0        0        0    82135 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/images/household_example_spreadsheet_01.png
--rw-r--r--   0        0        0    71228 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/images/household_example_spreadsheet_02.png
--rw-r--r--   0        0        0      306 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/index.rst
--rw-r--r--   0        0        0     1559 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/introduction.rst
--rw-r--r--   0        0        0      759 2021-06-21 06:53:42.014253 hepfile-0.1.3/docs/make.bat
--rw-r--r--   0        0        0       64 2021-07-16 15:24:43.780248 hepfile-0.1.3/docs/requirements.txt
--rw-r--r--   0        0        0      885 2021-07-30 16:33:15.708667 hepfile-0.1.3/docs/schema.rst
--rw-r--r--   0        0        0     8324 2021-08-11 23:53:04.271971 hepfile-0.1.3/docs/usage.rst
--rw-r--r--   0        0        0      428 2021-08-19 06:36:54.924372 hepfile-0.1.3/examples/awkward_example.py
--rw-r--r--   0        0        0     1867 2022-01-29 06:05:15.963831 hepfile-0.1.3/examples/csvreader.py
--rw-r--r--   0        0        0     3144 2022-01-29 06:05:15.963831 hepfile-0.1.3/examples/csvreader_long.py
--rw-r--r--   0        0        0     2842 2021-08-15 04:08:48.488131 hepfile-0.1.3/examples/cylindrical_example.py
--rw-r--r--   0        0        0     2871 2021-08-15 04:08:36.863838 hepfile-0.1.3/examples/matrix_example.py
--rw-r--r--   0        0        0     1196 2022-05-30 04:28:05.042347 hepfile-0.1.3/examples/read_hepfile.py
--rw-r--r--   0        0        0      767 2021-08-15 04:09:22.360987 hepfile-0.1.3/examples/read_many_hepfile.py
--rw-r--r--   0        0        0      204 2022-05-16 17:30:58.635378 hepfile-0.1.3/examples/sandbox_testing.py
--rw-r--r--   0        0        0      493 2021-07-22 20:42:44.132997 hepfile-0.1.3/examples/sheet1.csv
--rw-r--r--   0        0        0      302 2021-07-22 20:42:44.132997 hepfile-0.1.3/examples/sheet2.csv
--rw-r--r--   0        0        0      224 2021-07-22 20:42:44.132997 hepfile-0.1.3/examples/sheet3.csv
--rw-r--r--   0        0        0     3223 2022-01-29 06:05:15.963831 hepfile-0.1.3/examples/write_large_file_to_hepfile.py
--rw-r--r--   0        0        0     1569 2022-05-16 17:33:55.535040 hepfile-0.1.3/examples/write_to_hepfile.py
--rw-r--r--   0        0        0     1922 2022-01-29 06:05:15.963831 hepfile-0.1.3/examples/write_to_hepfile_FOR_PROFILING.py
--rw-r--r--   0        0        0     3113 2021-07-30 16:33:15.708667 hepfile-0.1.3/paper/paper.bib
--rw-r--r--   0        0        0     2731 2021-07-30 16:33:15.708667 hepfile-0.1.3/paper/paper.md
--rw-r--r--   0        0        0     1797 2022-05-30 04:46:46.212055 hepfile-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      336 2022-05-30 04:46:52.821527 hepfile-0.1.3/src/hepfile/__init__.py
--rw-r--r--   0        0        0     2071 2022-01-29 06:05:12.891754 hepfile-0.1.3/src/hepfile/awkward_tools.py
--rw-r--r--   0        0        0        0 2021-06-21 06:53:42.014253 hepfile-0.1.3/src/hepfile/py.typed
--rw-r--r--   0        0        0    15912 2022-05-30 04:31:17.461202 hepfile-0.1.3/src/hepfile/read.py
--rw-r--r--   0        0        0    22486 2022-05-16 17:41:58.189931 hepfile-0.1.3/src/hepfile/write.py
--rw-r--r--   0        0        0       67 2021-06-21 20:42:04.913937 hepfile-0.1.3/tests/test_package.py
--rw-r--r--   0        0        0     3921 2022-01-29 06:05:15.963831 hepfile-0.1.3/tests/test_read.py
--rw-r--r--   0        0        0     7368 2021-08-15 04:06:09.356172 hepfile-0.1.3/tests/test_write.py
--rw-r--r--   0        0        0     1345 2021-08-15 04:06:14.596300 hepfile-0.1.3/tests/write_file_for_unit_tests.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 hepfile-0.1.3/setup.py
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 hepfile-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2975 2023-07-07 14:08:15.978160 hepfile-0.1.4/README.md
+-rw-r--r--   0        0        0     1782 2023-07-07 14:08:15.986160 hepfile-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/_version.py
+-rw-r--r--   0        0        0     7823 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/awkward_tools.py
+-rw-r--r--   0        0        0      402 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/constants.py
+-rw-r--r--   0        0        0     1757 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/csv_tools.py
+-rw-r--r--   0        0        0     8405 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/df_tools.py
+-rw-r--r--   0        0        0     6843 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/dict_tools.py
+-rw-r--r--   0        0        0     1452 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/errors.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/py.typed
+-rw-r--r--   0        0        0    21124 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/read.py
+-rw-r--r--   0        0        0    28546 2023-07-07 14:08:15.990160 hepfile-0.1.4/src/hepfile/write.py
+-rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 hepfile-0.1.4/PKG-INFO
```

### Comparing `hepfile-0.1.3/pyproject.toml` & `hepfile-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,56 +17,58 @@
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Development Status :: 1 - Planning",
 ]
 
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 
 requires = [
   "numpy >=1.13.3",
+  "pandas",
   "h5py",
-  "awkward >= 1.4",
-  "typing; python_version<'3.5'",
+  "awkward >= 2.1.2",
   "pre-commit",
+  "jupyter",
+  "mistune"
 ]
 
 [tool.flit.metadata.requires-extra]
 test = [
     "pytest >=6",
 ]
 dev = [
   "pytest >=6",
 ]
 docs = [
   "Sphinx >=3.0.0",
   "myst_parser>=0.13",
+  "nbsphinx>=0.9.1",
   "sphinx-book-theme>=0.0.33",
   "sphinx_copybutton",
 ]
 awkward = [
   "awkward >= 1.4",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra -Wd"
 testpaths = ["tests"]
 
 
 [tool.mypy]
 files = "src"
-python_version = "3.6"
+python_version = "3.9"
 warn_unused_configs = true
 
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
```

### Comparing `hepfile-0.1.3/src/hepfile/read.py` & `hepfile-0.1.4/src/hepfile/read.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,328 +1,399 @@
+"""
+Functions to assist in reading and accessing information in hepfiles.
+"""
+
+from __future__ import annotations
+
+import warnings
 import h5py as h5
 import numpy as np
+import pandas as pd
+from . import constants
+from .errors import RangeSubsetError, InputError, MetadataNotFound, HeaderNotFound
+from .awkward_tools import hepfile_to_awkward
+from .df_tools import hepfile_to_df
 
-################################################################################
-def load(filename=None, verbose=False, desired_datasets=None, subset=None):
 
-    '''
+################################################################################
+def load(
+    filename: str,
+    verbose: bool = False,
+    desired_groups: list[str] = None,
+    subset: int = None,
+    return_type: str = "dictionary",
+) -> tuple[dict, dict]:
+    """
     Reads all, or a subset of the data, from the HDF5 file to fill a data dictionary.
     Returns an empty dictionary to be filled later with data from individual buckets.
 
     Args:
-	**filename** (string): Name of the input file
-	
-	**verbose** (boolean): True if debug output is required
+        filename (string): Name of the input file
 
-	**desired_datasets** (list): Datasets to be read from input file, THIS IS REALLY
-    STRING MATCHING SO THE USER COULD PASS IN A GROUP NAME. IS THIS RIGHT?
+        verbose (boolean): True if debug output is required
 
-	**subset** (int): Number of buckets to be read from input file
+        desired_groups (list): Groups to be read from input file,
+
+        subset (int): Number of buckets to be read from input file
+
+        return_type (str): Type to return. Options are 'dictionary', 'awkward', and 'pandas'.
+                           Default is 'dictionary'.
 
     Returns:
-	**data** (dict): Selected data from HDF5 file
-	
-	**bucket** (dict): An empty bucket dictionary to be filled by data from select buckets
-
-    '''
-
-    # Open the HDF5 file
-    infile = None
-    if filename != None:
-        infile = h5.File(filename, "r+")
-    else:
-        print("No filename passed in! Can't open file.\n")
-        return None,None
-
-    # Create the initial data and bucket dictionary to hold the data
-    data = {}
-    bucket = {}
-
-    # We'll fill the data dictionary with some extra fields, though we won't
-    # need them all for the bucket
-    data["_MAP_DATASETS_TO_COUNTERS_"] = {}
-    data["_MAP_DATASETS_TO_INDEX_"] = {}
-    data["_LIST_OF_COUNTERS_"] = []
-    data["_LIST_OF_DATASETS_"] = []
-
-    # Get the number of buckets.
-    # In HEP (High Energy Physics), this would be the number of events
-    data["_NUMBER_OF_BUCKETS_"] = infile.attrs["_NUMBER_OF_BUCKETS_"]
-
-    # We might only read in a subset of the data though!
-    if subset is not None:
-        if type(subset) is tuple:
-            subset = list(subset)
-
-        if type(subset) is int:
-            print("Single subset value of {subset} being interpreted as a high range")
-            print(f"subset being set to a range of (0,{subset})\n")
-            subset = [0, subset]
-
-        # If the user has specified `subset` incorrectly, then let's return
-        # an empty data and bucket
-        if subset[1]-subset[0]<=0:
-            print("The range in subset is either 0 or negative!")
-            print(f"{subset[1]} - {subset[0]} = {subset[1] - subset[0]}")
-            print("Returning an empty data and bucket dictionary!\n")
-            return data,bucket
-
-        # Make sure the user is not asking for something bigger than the file!
-        nbuckets = data["_NUMBER_OF_BUCKETS_"]
-
-        if subset[0] > nbuckets:
-            print("Range for subset starts greater than number of buckets in file!")
-            print(f"{subset[0]} > {nbuckets}")
-            print(f"I'm not sure how to handle this so the file will not be opened.")
-            print(f"Returning None,None")
-            infile.close()
-            return None,None
-
-        if subset[1] > nbuckets:
-            print("Range for subset is greater than number of buckets in file!")
-            print(f"{subset[1]} > {nbuckets}")
-            print(f"High range of subset will be set to {nbuckets}\n")
-            subset[1] = nbuckets
-
-        data["_NUMBER_OF_BUCKETS_"] = subset[1] - subset[0]
-        nbuckets = data["_NUMBER_OF_BUCKETS_"]
-
-        print("Will read in a subset of the file!")
-        print(f"From bucket {subset[0]} (inclusive) through bucket {subset[1]-1} (inclusive)")
-        print(f"Bucket {subset[1]} is not read in")
-        print(f"Reading in {nbuckets} buckets\n")
-
-    ############################################################################
-    # Get the datasets and counters
-    ############################################################################
-    dc = infile["_MAP_DATASETS_TO_COUNTERS_"]
-    for vals in dc:
+        data (dict): Selected data from HDF5 file
 
-        if verbose:
-            print(f"Map datasets to counters: {vals}")
+        bucket (dict): An empty bucket dictionary to be filled by data from select buckets
+
+    """
 
-        # The decode is there because vals were stored as numpy.bytes
-        counter = vals[1].decode()
-        index = f"{counter}_INDEX"
-        data["_MAP_DATASETS_TO_COUNTERS_"][vals[0].decode()] = counter
-        data["_MAP_DATASETS_TO_INDEX_"][vals[0].decode()] = index
-        data["_LIST_OF_COUNTERS_"].append(vals[1].decode())
-        data["_LIST_OF_DATASETS_"].append(vals[0].decode())
-        data["_LIST_OF_DATASETS_"].append(vals[1].decode())  # Get the counters as well
-
-    # We may have added some counters and datasets multiple times.
-    # So just to be sure, only keep the unique values
-    data["_LIST_OF_COUNTERS_"] = np.unique(data["_LIST_OF_COUNTERS_"]).tolist()
-    data["_LIST_OF_DATASETS_"] = np.unique(data["_LIST_OF_DATASETS_"]).tolist()
-    ############################################################################
-
-    ############################################################################
-    # Pull out the SINGLETON datasets
-    ############################################################################
-    sg = infile["_SINGLETONSGROUPFORSTORAGE_"][0]  # This is a numpy array of strings
-    decoded_string = sg[1].decode()
-
-    vals = decoded_string.split("__:__")
-    vals.remove("COUNTER")
-
-    data["_SINGLETONS_GROUP_"] = vals
-    ############################################################################
-
-    ############################################################################
-    # Get the list of datasets and groups
-    ############################################################################
-    all_datasets = data["_LIST_OF_DATASETS_"]
-
-    if verbose:
-        print(f"all_datasets: {all_datasets}")
-    ############################################################################
-
-    ############################################################################
-    # Only keep select data from file, if we have specified desired_datasets
-    ############################################################################
-    if desired_datasets is not None:
-        if type(desired_datasets) != list:
-            desired_datasets = list(desired_datasets)
-
-        # Count backwards because we'll be removing stuff as we go.
-        i = len(all_datasets) - 1
-        while i >= 0:
-            entry = all_datasets[i]
-
-            is_dropped = True
-            # This is looking to see if the string is anywhere in the name
-            # of the dataset
-            for desdat in desired_datasets:
-                if desdat in entry:
-                    is_dropped = False
-                    break
-
-            if is_dropped == True:
-                print(f"Not reading out {entry} from the file....")
-                all_datasets.remove(entry)
+    if return_type not in {"dictionary", "awkward", "pandas"}:
+        raise InputError("return_type must be dictionary, awkward, or pandas")
 
-            i -= 1
+    with h5.File(filename, "r+") as infile:
+        # Create the initial data and bucket dictionary to hold the data
+        data = {}
+        bucket = {}
+
+        # We'll fill the data dictionary with some extra fields, though we won't
+        # need them all for the bucket
+        data["_MAP_DATASETS_TO_COUNTERS_"] = {}
+        data["_MAP_DATASETS_TO_INDEX_"] = {}
+        data["_LIST_OF_COUNTERS_"] = []
+        data["_LIST_OF_DATASETS_"] = []
+        data["_META_"] = {}
+
+        # Get the number of buckets.
+        # In HEP (High Energy Physics), this would be the number of events
+        data["_NUMBER_OF_BUCKETS_"] = infile.attrs["_NUMBER_OF_BUCKETS_"]
+
+        # We might only read in a subset of the data though!
+        if subset is not None:
+            if isinstance(subset, tuple):
+                subset = list(subset)
+
+            if isinstance(subset, int):
+                print(
+                    "Single subset value of {subset} being interpreted as a high range"
+                )
+                print(f"subset being set to a range of (0,{subset})\n")
+                subset = [0, subset]
+
+            # If the user has specified `subset` incorrectly, then let's return
+            # an empty data and bucket
+            if subset[1] - subset[0] <= 0:
+                raise RangeSubsetError(
+                    f"The range in subset is either 0 or negative! \
+                    {subset[1]} - {subset[0]} = {subset[1] - subset[0]}"
+                )
+
+            # Make sure the user is not asking for something bigger than the file!
+            nbuckets = data["_NUMBER_OF_BUCKETS_"]
+
+            if subset[0] > nbuckets:
+                raise RangeSubsetError(
+                    f"Range for subset starts greater than number of buckets \
+                    in file! {subset[0]} > {nbuckets}"
+                )
+
+            if subset[1] > nbuckets:
+                warnings.warn(
+                    f"Range for subset is greater than number of buckets in \
+                    file!\n{subset[1]} > {nbuckets}\nHigh range of subset will \
+                    be set to {nbuckets}\n"
+                )
+                subset[1] = nbuckets
+
+            data["_NUMBER_OF_BUCKETS_"] = subset[1] - subset[0]
+            nbuckets = data["_NUMBER_OF_BUCKETS_"]
+
+            print("Will read in a subset of the file!")
+            print(
+                f"From bucket {subset[0]} (inclusive) through bucket {subset[1]-1} (inclusive)"
+            )
+            print(f"Bucket {subset[1]} is not read in")
+            print(f"Reading in {nbuckets} buckets\n")
+
+        ############################################################################
+        # Get the datasets and counters
+        ############################################################################
+        allvalues = infile["_MAP_DATASETS_TO_COUNTERS_"]
+        for vals in allvalues:
+            if verbose:
+                print(f"Map datasets to counters: {vals}")
+
+            # The decode is there because vals were stored as numpy.bytes
+            counter = vals[1].decode()
+            index = f"{counter}_INDEX"
+            data["_MAP_DATASETS_TO_COUNTERS_"][vals[0].decode()] = counter
+            data["_MAP_DATASETS_TO_INDEX_"][vals[0].decode()] = index
+            data["_LIST_OF_COUNTERS_"].append(vals[1].decode())
+            data["_LIST_OF_DATASETS_"].append(vals[0].decode())
+            data["_LIST_OF_DATASETS_"].append(
+                vals[1].decode()
+            )  # Get the counters as well
+
+        # We may have added some counters and datasets multiple times.
+        # So just to be sure, only keep the unique values
+        data["_LIST_OF_COUNTERS_"] = np.unique(data["_LIST_OF_COUNTERS_"]).tolist()
+        data["_LIST_OF_DATASETS_"] = np.unique(data["_LIST_OF_DATASETS_"]).tolist()
+        ############################################################################
+
+        ############################################################################
+        # Pull out the SINGLETON datasets
+        ############################################################################
+        # This is a numpy array of strings
+        singletons_group = infile["_SINGLETONSGROUPFORSTORAGE_"][0]
+        decoded_string = singletons_group[1].decode()
+
+        vals = decoded_string.split("__:__")
+        vals.remove("COUNTER")
+
+        data["_SINGLETONS_GROUP_"] = vals
+        ############################################################################
+
+        ############################################################################
+        # Get the list of datasets and groups
+        ############################################################################
+        all_datasets = data["_LIST_OF_DATASETS_"]
 
         if verbose:
-            print(f"After only selecting certain datasets ----- ")
             print(f"all_datasets: {all_datasets}")
-    ###########################################################################
+        ############################################################################
 
-    # We might need the counter for SINGLETONS so let's pull it out
-    data["_SINGLETONS_GROUP_/COUNTER"] = infile["_SINGLETONS_GROUP_"]['COUNTER']
+        ############################################################################
+        # Only keep select data from file, if we have specified desired_groups
+        ############################################################################
+        if desired_groups is not None:
+            if not isinstance(desired_groups, list):
+                desired_groups = list(desired_groups)
+
+            # Count backwards because we'll be removing stuff as we go.
+            i = len(all_datasets) - 1
+            while i >= 0:
+                entry = all_datasets[i]
+
+                is_dropped = True
+                # This is looking to see if the string is anywhere in the name
+                # of the dataset
+                for desdat in desired_groups:
+                    if desdat in entry:
+                        is_dropped = False
+                        break
+
+                if is_dropped is True:
+                    print(f"Not reading out {entry} from the file....")
+                    all_datasets.remove(entry)
+
+                i -= 1
+
+            if verbose:
+                print("After only selecting certain datasets ----- ")
+                print(f"all_datasets: {all_datasets}")
+        ###########################################################################
 
-    if verbose == True:
-        print("\nDatasets and counters:")
-        print(data["_MAP_DATASETS_TO_COUNTERS_"])
-        print("\nList of counters:")
-        print(data["_LIST_OF_COUNTERS_"])
-        print("\n_SINGLETONS_GROUP_/COUNTER:")
-        print(data["_SINGLETONS_GROUP_/COUNTER"])
-        print("\n")
-
-    ############################################################################
-    # Pull out the counters and build the indices
-    ############################################################################
-    print("Building the indices...\n")
-
-    if verbose:
-        print("data.keys()")
-        print(data.keys())
-        print("\n")
-
-    # We will need to keep track of the indices in the entire file
-    # This way, if the user specifies a subset of the data, we have the full 
-    # indices already calculated
-    full_file_indices = {}
+        # We might need the counter for SINGLETONS so let's pull it out
+        data["_SINGLETONS_GROUP_/COUNTER"] = infile["_SINGLETONS_GROUP_"]["COUNTER"]
 
-    for counter_name in data["_LIST_OF_COUNTERS_"]:
+        if verbose:
+            print("\nDatasets and counters:")
+            print(data["_MAP_DATASETS_TO_COUNTERS_"])
+            print("\nList of counters:")
+            print(data["_LIST_OF_COUNTERS_"])
+            print("\n_SINGLETONS_GROUP_/COUNTER:")
+            print(data["_SINGLETONS_GROUP_/COUNTER"])
+            print("\n")
+
+        ############################################################################
+        # Pull out the counters and build the indices
+        ############################################################################
+        print("Building the indices...\n")
 
         if verbose:
-            print(f"counter name: ------------ {counter_name}\n")
+            print("data.keys()")
+            print(data.keys())
+            print("\n")
+
+        # We will need to keep track of the indices in the entire file
+        # This way, if the user specifies a subset of the data, we have the full
+        # indices already calculated
+        full_file_indices = {}
+
+        for counter_name in data["_LIST_OF_COUNTERS_"]:
+            if verbose:
+                print(f"counter name: ------------ {counter_name}\n")
+
+            full_file_counters = infile[counter_name]
+            full_file_index = calculate_index_from_counters(full_file_counters)
+
+            if verbose:
+                print(f"full file counters: {full_file_counters}\n")
+                print(f"full file index: {full_file_index}\n")
+
+            # If we passed in subset, grab that slice of the data from the file
+            if subset is not None and subset[1] <= subset[0]:
+                raise RangeSubsetError(
+                    f"Unable to read anything in! High range of {subset[1]} is \
+                    less than or equal to low range of {subset[0]}"
+                )
 
-        full_file_counters = infile[counter_name]
-        full_file_index = calculate_index_from_counters(full_file_counters)
+            if subset is not None:
+                # We tack on +1 to the high range of subset when we pull out the counters
+                # and index because we want to get all of the entries for the last entry.
+                data[counter_name] = infile[counter_name][subset[0] : subset[1] + 1]
+                index = full_file_index[subset[0] : subset[1] + 1]
+            else:
+                data[counter_name] = infile[counter_name][:]
+                index = full_file_index
 
-        if verbose:
-            print(f"full file counters: {full_file_counters}\n")
-            print(f"full file index: {full_file_index}\n")
+            subset_index = index
+            # If the file is *not* empty....
+            # Just to make sure the "local" index of the data dictionary starts at 0
+            if len(index) > 0:
+                subset_index = index - index[0]
+
+            index_name = f"{counter_name}_INDEX"
 
-        # If we passed in subset, grab that slice of the data from the file
-        if subset is not None and subset[1] <= subset[0]:
-            print("Will not be reading anything in!")
-            print(f"High range of {subset[1]} is less than or equal to low range of {subset[0]}")
-            print("Returning None,None...")
-            return None,None
-
-        elif subset is not None:
-            # We tack on +1 to the high range of subset when we pull out the counters
-            # and index because we want to get all of the entries for the last entry.
-            data[counter_name] = infile[counter_name][subset[0] : subset[1]+1]
-            index = full_file_index[subset[0] : subset[1]+1]
-        else:
-            data[counter_name] = infile[counter_name][:]
-            index = full_file_index
-
-        subset_index = index
-        # If the file is *not* empty....
-        # Just to make sure the "local" index of the data dictionary starts at 0
-        if len(index)>0:
-            subset_index = index - index[0]
-
-        index_name = "%s_INDEX" % (counter_name)
-
-        data[index_name] = subset_index
-        full_file_indices[index_name] = index
-
-    print("Built the indices!")
-
-    if verbose:
-        print("full_file_index: ")
-        print(f"{full_file_indices}\n")
-
-    # Loop over the all_datasets we want and pull out the data.
-    for name in all_datasets:
-
-        # If this is a counter, we're going to have to grab the indices
-        # differently than for a "normal" dataset
-        IS_COUNTER = True
-        index_name = None
-        if name not in data["_LIST_OF_COUNTERS_"]:
-            index_name = data["_MAP_DATASETS_TO_INDEX_"][name]
-            IS_COUNTER = False # We will use different indices for the counters
-
-        if verbose == True:
-            print(f"------ {name}")
-            print(f"index_name: {index_name}\n")
+            data[index_name] = subset_index
+            full_file_indices[index_name] = index
 
-        dataset = infile[name]
+        print("Built the indices!")
 
         if verbose:
-            print(f"dataset type: {type(dataset)}")
-        
-        # This will ignore the groups
-        if type(dataset) == h5.Dataset:
-            dataset_name = name
+            print("full_file_index: ")
+            print(f"{full_file_indices}\n")
 
-            if subset is not None:
-                if IS_COUNTER:
-                    # If this is a counter, then the subset indices
-                    # map on to the same locations for any counters
-                    lo = subset[0]
-                    hi = subset[1]
+        # Loop over the all_datasets we want and pull out the data.
+        for name in all_datasets:
+            # If this is a counter, we're going to have to grab the indices
+            # differently than for a "normal" dataset
+            is_counter = True
+            index_name = None
+            if name not in data["_LIST_OF_COUNTERS_"]:
+                index_name = data["_MAP_DATASETS_TO_INDEX_"][name]
+                is_counter = False  # We will use different indices for the counters
+
+            if verbose:
+                print(f"------ {name}")
+                print(f"index_name: {index_name}\n")
+
+            dataset = infile[name]
+
+            if verbose:
+                print(f"dataset type: {type(dataset)}")
+
+            # This will ignore the groups
+            if isinstance(dataset, h5.Dataset):
+                dataset_name = name
+
+                if subset is not None:
+                    if is_counter:
+                        # If this is a counter, then the subset indices
+                        # map on to the same locations for any counters
+                        lo = subset[0]
+                        hi = subset[1]
+                    else:
+                        lo = full_file_indices[index_name][0]
+                        hi = full_file_indices[index_name][-1]
+                    if verbose:
+                        print(f"dataset name/lo/hi: {dataset_name},{lo},{hi}\n")
+                    data[dataset_name] = dataset[lo:hi]
                 else:
-                    lo = full_file_indices[index_name][0]
-                    hi = full_file_indices[index_name][-1]
+                    data[dataset_name] = dataset[:]
+
+                bucket[dataset_name] = None  # This will be filled for individual bucket
                 if verbose:
-                    print(f"dataset name/lo/hi: {dataset_name},{lo},{hi}\n")
-                data[dataset_name] = dataset[lo : hi]
-            else:
-                data[dataset_name] = dataset[:]
+                    print(dataset)
 
-            bucket[dataset_name] = None  # This will be filled for individual bucket
-            if verbose == True:
-                print(dataset)
+            # write the metadata for that group to data if it exists
+            if name not in constants.protected_names and "meta" in dataset.attrs.keys():
+                data["_META_"][name] = dataset.attrs["meta"]
 
-    infile.close()
     print("Data is read in and input file is closed.")
 
+    # edit data so it matches the format of the data dict that was saved to the file
+    # this makes it so that data can be directly passed to write_to_file
+    # 1) add back in _GROUP_
+    datasets = np.array(data["_LIST_OF_DATASETS_"])
+
+    allgroups = np.array([d.split("/")[0] for d in datasets])
+
+    singletons_group = set(data["_SINGLETONS_GROUP_"])
+    groups = {}
+
+    groups["_SINGLETONS_GROUP_"] = data["_SINGLETONS_GROUP_"]  # copy over the data
+    for key in np.unique(allgroups):
+        if key in singletons_group:
+            continue
+        if key in constants.protected_names:
+            continue
+
+        where_groups = np.where((key == allgroups) * (key != datasets))[0]
+        groups[key] = [dataset.split("/")[-1] for dataset in datasets[where_groups]]
+
+    data["_GROUPS_"] = groups
+
+    # 2) add back in _MAP_DATASETS_TO_DATA_TYPES
+    dtypes = {}
+    for key in data["_LIST_OF_DATASETS_"]:
+        if key not in data:
+            continue
+
+        if isinstance(data[key], list):
+            data[key] = np.array(data[key])
+
+        dtypes[key] = data[key].dtype
+
+    data["_MAP_DATASETS_TO_DATA_TYPES_"] = dtypes
+
+    # 3) add _PROTECTED_NAMES_
+    data["_PROTECTED_NAMES_"] = constants.protected_names
+
+    if return_type == "awkward":
+        return hepfile_to_awkward(data), bucket
+
+    if return_type == "pandas":
+        return hepfile_to_df(data), bucket
+
     return data, bucket
 
 
 ################################################################################
 
-################################################################################
-def calculate_index_from_counters(counters):
 
+################################################################################
+def calculate_index_from_counters(counters: int) -> int:
+    """
+    Calculates an index array from the counters
+    """
     index = np.add.accumulate(counters) - counters
 
     return index
 
-################################################################################
 
 ################################################################################
-def unpack(bucket, data, n=0):
 
-    """ Fills the bucket dictionary with selected rows from the data dictionary.
+
+################################################################################
+def unpack(bucket: dict, data: dict, n: int = 0):
+    """Fills the bucket dictionary with selected rows from the data dictionary.
 
     Args:
 
-	**bucket** (dict): bucket dictionary to be filled
+        bucket (dict): bucket dictionary to be filled
 
-	**data** (dict): Data dictionary used to fill the bucket dictionary
+        data (dict): Data dictionary used to fill the bucket dictionary
 
-    **n** (integer): 0 by default. Which entry should be pulled out of the data
+        n (integer): 0 by default. Which entry should be pulled out of the data
                      dictionary and inserted into the bucket dictionary.
 
     """
 
     keys = bucket.keys()
 
     for key in keys:
-
         # if "num" in key:
         # IS THERE A WAY THAT THIS COULD BE FASTER?
         # print(data['_LIST_OF_COUNTERS_'],key)
         if key in data["_LIST_OF_COUNTERS_"] or key in data["_SINGLETONS_GROUP_"]:
             bucket[key] = data[key][n]
 
         elif "INDEX" not in key:  # and 'Jets' in key:
@@ -334,103 +405,131 @@
 
             if len(data[numkey]) > 0:
                 nobjs = data[numkey][n]
                 bucket[key] = data[key][index : index + nobjs]
 
 
 ################################################################################
-def get_nbuckets_in_file(filename):
+def get_nbuckets_in_file(filename: str) -> int:
+    """Get the number of buckets in the file."""
 
-    """ Get the number of buckets in the file.
+    # f = h5.File(filename, "r+")
+    # a = f.attrs
 
-    """
+    if not isinstance(filename, str):
+        raise InputError("Expecting the input filename to be a string!")
 
-    #f = h5.File(filename, "r+")
-    #a = f.attrs
+    with h5.File(filename, "r+") as infile:
+        attr = infile.attrs
+        if "_NUMBER_OF_BUCKETS_" not in attr:
+            raise AttributeError(
+                'File does not contain the attribute, "_NUMBER_OF_BUCKETS_"'
+            )
 
-    if type(filename) is not str:
-        print(f"Expecting a string for the filename!")
-        return None
+        num_buckets = attr.get("_NUMBER_OF_BUCKETS_")
+        return num_buckets
 
-    with h5.File(filename, "r+") as f:
-        a = f.attrs
 
-        if a.__contains__("_NUMBER_OF_BUCKETS_"):
-            _NUMBER_OF_BUCKETS_ = a.get("_NUMBER_OF_BUCKETS_")
-            f.close()
-            return _NUMBER_OF_BUCKETS_
-        else:
-            print('\nFile does not contain the attribute, "_NUMBER_OF_BUCKETS_"\n')
-            f.close()
-            return None
-
-################################################################################
-def get_nbuckets_in_data(data):
-
-    """ Get the number of buckets in the data dictionary.
-        
-        This is useful in case you've only pulled out subsets of the data
+################################################################################
+def get_nbuckets_in_data(data: dict) -> int:
+    """Get the number of buckets in the data dictionary.
+
+    This is useful in case you've only pulled out subsets of the data
 
     """
 
-    if type(data) is not dict:
-        print(f"{data} is not a dictionary!\n")
-        return None
+    if not isinstance(data, dict):
+        raise InputError(f"{data} is not a dictionary!\n")
 
-    if "_NUMBER_OF_BUCKETS_" in list(data.keys()):
-        _NUMBER_OF_BUCKETS_ = data["_NUMBER_OF_BUCKETS_"]
-        return _NUMBER_OF_BUCKETS_
-    else:
-        print('\ndata dictionary does not contain the key, "_NUMBER_OF_BUCKETS_"\n')
-        return None
+    if "_NUMBER_OF_BUCKETS_" not in list(data.keys()):
+        raise AttributeError(
+            '\ndata dictionary does not contain the key, "_NUMBER_OF_BUCKETS_"\n'
+        )
+    num_buckets = data["_NUMBER_OF_BUCKETS_"]
+    return num_buckets
 
 
 ################################################################################
-def get_file_metadata(filename):
+def get_file_metadata(filename: str) -> dict:
+    """Get the file metadata and return it as a dictionary"""
 
-    """ Get the file metadata and return it as a dictionary
+    with h5.File(filename, "r+") as infile:
+        attrs = infile.attrs
 
-    """
+        if len(attrs) < 1:
+            raise MetadataNotFound(
+                f"No metadata in file {filename}! File has no attributes.\n"
+            )
 
-    f = h5.File(filename, "r+")
+        metadata = {}
+        for key in attrs:
+            metadata[key] = attrs[key]
 
-    a = f.attrs
+    return metadata
 
-    if len(a) < 1:
-        print(f"No metadata in file {filename}!")
-        print(f"File has no attributes.\n")
-        f.close()
-        return None
 
-    metadata = {}
+################################################################################
 
-    for key in a.keys():
-        metadata[key] = a[key]
 
-    f.close()
+################################################################################
+def get_file_header(filename: str, return_type: str = "dict") -> dict:
+    """Get the file header and return it as a dictionary or dataframe
 
-    return metadata
+    Args:
+    filename(string): HDF5 file to open and read the header information
 
+    return_type(string): If 'dict' return the header information as a dictionary.
+                         If 'df' or 'dataframe', return the information as a
+                         pandas dataframe.
 
-################################################################################
+    """
 
-################################################################################
-def print_file_metadata(filename):
+    if return_type is not None and return_type not in ["dict", "df", "dataframe"]:
+        print("'return_type' must be 'dict', 'df', or 'dataframe'")
+        print("Not returning any header information")
+        return None
 
-    """ Pretty print the file metadata 
+    with h5.File(filename, "r+") as infile:
+        if "_HEADER_" not in infile:
+            raise HeaderNotFound(
+                f"No header data in file {filename}! File has no _HEADER_ group.\n"
+            )
 
-    """
+        header_group = infile["_HEADER_"]
 
-    metadata = get_file_metadata(filename)
+        header = {}
+        for key in header_group:
+            # Let's decode the binary strings to make it easier on the user.
+            values = header_group[key][:]
+            temp = []
+            for val in values:
+                temp.append(val[0].decode())
 
-    if metadata is None:
-        return None
+            # Convert it to numpy array as that may be more expected for the user.
+            header[key] = np.array(temp)
+
+        if return_type in ("dataframe", "df"):
+            header = pd.DataFrame.from_dict(header)
+
+    return header
+
+
+################################################################################
+################################################################################
+def print_file_metadata(filename: str):
+    """Pretty print the file metadata"""
 
     output = ""
 
+    try:
+        metadata = get_file_metadata(filename)
+    except MetadataNotFound:
+        print(f"No Metadata in {filename}!")
+        return output
+
     keys = list(metadata.keys())
 
     first_keys_to_print = ["date", "_NUMBER_OF_BUCKETS_"]
 
     keys_already_printed = []
 
     # Print the basics first
@@ -461,7 +560,34 @@
 
     print(output)
 
     return output
 
 
 ################################################################################
+
+
+def print_file_header(filename: str) -> str:
+    """
+    Pretty print the file header
+
+    Args:
+        filename (str): filename to retrieve the header from.
+
+    Returns:
+        String representation of the header information, if it exists.
+    """
+
+    hdr = get_file_header(filename, return_type="dict")
+
+    return_str = f"{'#':#>64}\n"
+    return_str += f"###{' ':>22}Hepfile Header{' ':>22}###\n"
+    return_str += f"{'#':#>64}\n"
+    return_str += f"{'#':#>64}\n"
+
+    for key in hdr.keys():
+        return_str += f"{key}:"
+        for val in hdr[key]:
+            return_str += f"\t\t\t{val}\n"
+
+    print(return_str)
+    return return_str
```

### Comparing `hepfile-0.1.3/src/hepfile/write.py` & `hepfile-0.1.4/src/hepfile/write.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,621 +1,813 @@
-import numpy as np
-import h5py as h5
+"""
+Functions to assist in writing a hepfile "from scratch"
+"""
+
+from __future__ import annotations
+
 import datetime
 import sys
+import warnings
+
+import numpy as np
+import awkward as ak
+import h5py as h5
+
 import hepfile
+from . import constants
+from .errors import InputError, DatasetSizeDiscrepancy, MissingSingletonValue
 
 
 ################################################################################
-def initialize():
-    """ Creates an empty data dictionary
+def initialize() -> dict:
+    """Creates an empty data dictionary
 
     Returns:
 
-        **data** (dict): An empty data dictionary
+        data (dict): An empty data dictionary
 
     """
 
     data = {}
     data["_GROUPS_"] = {}
     data["_MAP_DATASETS_TO_COUNTERS_"] = {}
     data["_LIST_OF_COUNTERS_"] = []
 
     # For singleton entries, variables with only one entry per bucket.
     data["_GROUPS_"]["_SINGLETONS_GROUP_"] = ["COUNTER"]
-    data["_MAP_DATASETS_TO_COUNTERS_"]["_SINGLETONS_GROUP_"] = "_SINGLETONS_GROUP_/COUNTER"
+    data["_MAP_DATASETS_TO_COUNTERS_"][
+        "_SINGLETONS_GROUP_"
+    ] = "_SINGLETONS_GROUP_/COUNTER"
     data["_LIST_OF_COUNTERS_"].append("_SINGLETONS_GROUP_/COUNTER")
 
     data["_SINGLETONS_GROUP_/COUNTER"] = []
     data["_MAP_DATASETS_TO_DATA_TYPES_"] = {}
     data["_MAP_DATASETS_TO_DATA_TYPES_"]["_SINGLETONS_GROUP_/COUNTER"] = int
 
-    data["_PROTECTED_NAMES_"] = ["_PROTCTED_NAMES_",
-                                 "_GROUPS_",
-                                 "_MAP_DATASETS_TO_COUNTERS_",
-                                 "_MAP_DATASETS_TO_DATA_TYPES_"
-                                 "_LIST_OF_COUNTERS_",
-                                 "_SINGLETONS_GROUP_/COUNTER",
-                                 ]
+    data["_META_"] = {}
 
     return data
 
 
 ################################################################################
-def clear_bucket(bucket):
-    """ Clears the data from the bucket dictionary - should the name of the function change?
+def clear_bucket(bucket: dict) -> None:
+    """Clears the data from the bucket dictionary - should the name of the function change?
 
     Args:
-        **bucket** (dict): The dictionary to be cleared. This is designed to clear the data from
-                      the lists in the **bucket** dictionary, but theoretically, it would
-                      clear out the lists from any dictionary. 
+        bucket (dict): The dictionary to be cleared. This is designed to clear the data from
+                      the lists in the bucket dictionary, but theoretically, it would
+                      clear out the lists from any dictionary.
 
     """
 
     for key in bucket.keys():
-
-        if key == '_LIST_OF_COUNTERS_':
+        if key == "_LIST_OF_COUNTERS_":
             continue
 
-        if type(bucket[key]) == list:
+        if isinstance(bucket[key], list):
             bucket[key].clear()
-        elif type(bucket[key]) == int:
-            if key in bucket['_LIST_OF_COUNTERS_']:
+        elif isinstance(bucket[key], int):
+            if key in bucket["_LIST_OF_COUNTERS_"]:
                 bucket[key] = 0
             else:
                 bucket[key] = -999
-        elif type(bucket[key]) == float:
+        elif isinstance(bucket[key], float):
             bucket[key] = -999.0
-        elif type(bucket[key]) == str:
+        elif isinstance(bucket[key], str):
             bucket[key] = "-999"
 
 
 ################################################################################
 # Create a single bucket (dictionary) that will eventually be used to fill
 # the overall dataset
 ################################################################################
-def create_single_bucket(data):
-    """ Creates an bucket dictionary that will be used to collect data and then
+def create_single_bucket(data: dict) -> dict:
+    """Creates an bucket dictionary that will be used to collect data and then
     packed into the the master data dictionary.
 
     Args:
-        **data** (dict): Data dictionary that will hold all the data from the bucket.
+        data (dict): Data dictionary that will hold all the data from the bucket.
 
     Returns:
-        **bucket** (dict): The new bucket dictionary with keys and no bucket information
+        bucket (dict): The new bucket dictionary with keys and no bucket information
 
     """
 
-    bucket = {}
-
-    for k in data.keys():
-        if k in data["_LIST_OF_COUNTERS_"]:
-            bucket[k] = 0
-        else:
-            bucket[k] = data[k].copy()
+    bucket = {k: data[k].copy() for k in data.keys()}
+    for k in bucket["_LIST_OF_COUNTERS_"]:
+        bucket[k] = 0
 
     return bucket
 
 
 ################################################################################
 # This adds a group in the dictionary, similar to
 # a la CreateBranch in ROOT
 ################################################################################
-def create_group(data, group_name, counter=None):
-    """ Adds a group in the dictionary
+def create_group(
+    data: dict,
+    group_name: str,
+    counter: str = None,
+    verbose=False,
+    ignore_protected=False,
+):
+    """Adds a group in the dictionary
 
     Args:
-        **data** (dict): Dictionary to which the group will be added
+        data (dict): Dictionary to which the group will be added
 
-        **group_name** (string): Name of the group to be added
+        group_name (string): Name of the group to be added
 
-        **counter** (string): Name of the counter key. None by default
+        counter (string): Name of the counter key. None by default
 
     """
+    # check that group_name isn't in protected_names
+    if not ignore_protected and group_name in constants.protected_names:
+        raise InputError(
+            f"{group_name} is protected, please choose a different group name!"
+        )
 
     # Check for slashes in the group name. We can't have them.
-    if group_name.find('/')>=0:
-        new_group_name = group_name.replace('/','-')
+    if "/" in group_name:
+        new_group_name = group_name.replace("/", "-")
         print("----------------------------------------------------")
-        print(f"Slashes / are not allowed in group names")
+        print("Slashes / are not allowed in group names")
         print(f"Replacing / with - in group name {group_name}")
         print(f"The new name will be {new_group_name}")
         print("----------------------------------------------------")
-        group_name = new_group_name 
+        group_name = new_group_name
 
     # Change name of variable, just to keep code more understandable
     counter_name = counter
 
     # Create a counter_name if the user has not specified one
     if counter_name is None:
         print("----------------------------------------------------")
-        print(
-            f"There is no counter to go with group \033[1m{group_name}\033[0m")
+        print(f"There is no counter to go with group \033[1m{group_name}\033[0m")
         print("Are you sure that's what you want?")
         counter_name = f"N_{group_name}"
         print(f"Creating a counter called \033[1m{counter_name}\033[0m")
         print("-----------------------------------------------------")
 
     # Check for slashes in the counter name. We can't have them.
-    if counter_name.find('/')>=0:
-        new_counter_name = counter_name.replace('/','-')
+    if "/" in counter_name:
+        new_counter_name = counter_name.replace("/", "-")
         print("----------------------------------------------------")
-        print(f"Slashes / are not allowed in counter names")
+        print("Slashes / are not allowed in counter names")
         print(f"Replacing / with - in counter name {counter_name}")
         print(f"The new name will be {new_counter_name}")
         print("----------------------------------------------------")
-        counter_name = new_counter_name 
+        counter_name = new_counter_name
 
     keys = data.keys()
 
     # Then put the group and any datasets in there next.
     keyfound = False
-    for k in keys:
-        if group_name == k:
-            print(f"\033[1m{group_name}\033[0m is already in the dictionary!")
-            keyfound = True
-            break
-
-    if keyfound == False:
+    if group_name in keys:
+        print(f"\033[1m{group_name}\033[0m is already in the dictionary!")
+        keyfound = True
 
+    if not keyfound:
         data["_GROUPS_"][group_name] = []
-        print(f"Adding group \033[1m{group_name}\033[0m")
+        if verbose:
+            print(f"Adding group \033[1m{group_name}\033[0m")
 
         data["_GROUPS_"][group_name].append(counter_name)
         full_counter_name = f"{group_name}/{counter_name}"
 
         data["_MAP_DATASETS_TO_COUNTERS_"][group_name] = full_counter_name
         data["_MAP_DATASETS_TO_DATA_TYPES_"][full_counter_name] = int
 
         if full_counter_name not in data["_LIST_OF_COUNTERS_"]:
             data["_LIST_OF_COUNTERS_"].append(full_counter_name)
 
         data[full_counter_name] = []
-        print(f"Adding a counter for \033[1m{group_name}\033[0m as \033[1m{counter_name}\033[0m")
+        if verbose:
+            print(
+                f"Adding a counter for \033[1m{group_name}\033[0m as \033[1m{counter_name}\033[0m"
+            )
 
     return 0
 
+
 ################################################################################
 
+
 ################################################################################
 # This adds a dataset to the dictionary, similar to
 # a la CreateBranch in ROOT
 #
 # This can also add a dataset that is not associate with a group
 ################################################################################
-def create_dataset(data, datasets, group=None, dtype=float):
-    """ Adds a dataset to a group in a dictionary. If the group does not exist, it will be created.
+def create_dataset(
+    data: dict,
+    datasets: list,
+    group: str = None,
+    dtype: type = float,
+    verbose=False,
+    ignore_protected=False,
+):
+    """Adds a dataset to a group in a dictionary. If the group does not exist, it will be created.
 
     Args:
-        **data** (dict): Dictionary that contains the group
+        data (dict): Dictionary that contains the group
 
-        **datasets** (list): Dataset to be added to the group (This doesn't have to be a list)
+        datasets (list): Dataset to be added to the group (This doesn't have to be a list)
 
-        **group** (string): Name of group the dataset will be added to.  None by default
+        group (string): Name of group the dataset will be added to.  None by default
 
-        **dtype** (type): The data type. None by default - I don't think this is every used 
+        dtype (type): The data type. None by default - I don't think this is every used
 
     Returns:
-        **-1**: If the group is None
-
+        -1: If the group is None
 
     """
 
-    if type(datasets) != list:
+    if not isinstance(datasets, list):
         datasets = [datasets]
 
-    # Check for slashes in the group name. We can't have them.
-    for i in range(len(datasets)):
-        tempname = datasets[i]
-        if tempname.find('/')>=0:
-            new_dataset_name = tempname.replace('/','-')
+    # Check for slashes in the dataset name. We can't have them.
+    for i, tempname in enumerate(datasets):
+        # check that tempname isn't in protected_names
+        if not ignore_protected and tempname in constants.protected_names:
+            raise InputError(
+                f"{tempname} is protected, please choose a different dataset name!"
+            )
+
+        if "/" in tempname:
+            new_dataset_name = tempname.replace("/", "-")
             print("----------------------------------------------------")
-            print(f"Slashes / are not allowed in dataset names")
+            print("Slashes / are not allowed in dataset names")
             print(f"Replacing / with - in dataset name {tempname}")
             print(f"The new name will be {new_dataset_name}")
             print("----------------------------------------------------")
-            datasets[i] = new_dataset_name 
+            datasets[i] = new_dataset_name
 
     keys = data.keys()
 
     # These will be entries for the SINGLETON_GROUP, if there is no group passed in
     if group is None:
-
         for dataset in datasets:
             keyfound = False
-            for k in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
-                if dataset == k:
-                    print(f"\033[1m{dataset}\033[0m is already in the dictionary!")
-                    keyfound = True
-            if keyfound == False:
-                print(f"Adding dataset \033[1m{dataset}\033[0m to the dictionary as a SINGLETON.")
+
+            if dataset in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
+                print(f"\033[1m{dataset}\033[0m is already in the dictionary!")
+                keyfound = True
+
+            if not keyfound:
+                if verbose:
+                    print(
+                        f"Adding dataset \033[1m{dataset}\033[0m to the dictionary as a SINGLETON."
+                    )
                 data["_GROUPS_"]["_SINGLETONS_GROUP_"].append(dataset)
                 data[dataset] = []
-                data["_MAP_DATASETS_TO_COUNTERS_"][dataset] = "_SINGLETONS_GROUP_/COUNTER"
+                data["_MAP_DATASETS_TO_COUNTERS_"][
+                    dataset
+                ] = "_SINGLETONS_GROUP_/COUNTER"
 
                 data["_MAP_DATASETS_TO_DATA_TYPES_"][dataset] = dtype
 
         return 0
 
     # Put the counter in the dictionary first.
-    keyfound = False
-    for k in data["_GROUPS_"]:
-        if group == k:
-            keyfound = True
+    keyfound = group in data["_GROUPS_"]
 
     # NEED TO FIX THIS PART SO THAT IT FINDS THE RIGHT COUNTER FROM THE GROUP
-    if keyfound == False:
-        print(f"Your group, \033[1m{group}\033[0m is not in the dictionary yet!")
+    if not keyfound:
         counter = f"N_{group}"
-        print(f"Adding it, along with a counter of \033[1m{counter}\033[0m")
+        warnings.warn(
+            f"Your group, \033[1m{group}\033[0m is not in the dictionary yet! \
+            Adding it, along with a counter of \033[1m{counter}\033[0m"
+        )
         create_group(data, group, counter=counter)
 
-    # Then put the datasets into the group in there next.
-    if type(datasets) != list:
-        datasets = [datasets]
-
     for dataset in datasets:
         keyfound = False
-        name = "%s/%s" % (group, dataset)
-        for k in keys:
-            if name == k:
-                print(f"\033[1m{name}\033[0m is already in the dictionary!")
-                keyfound = True
-        if keyfound == False:
-            print(f"Adding dataset \033[1m{dataset}\033[0m to the dictionary under group \033[1m{group}\033[0m.")
+        name = f"{group}/{dataset}"
+
+        # check that tempname isn't in protected_names
+        if not ignore_protected and name in constants.protected_names:
+            raise InputError(
+                f"{name} is protected, please choose a different dataset or group name!"
+            )
+
+        if name in keys:
+            warnings.warn(
+                f"\033[1m{name}\033[0m is already in the dictionary! Skipping!!!"
+            )
+            keyfound = True
+
+        if not keyfound:
+            if verbose:
+                print(
+                    f"Adding dataset \033[1m{dataset}\033[0m to the dictionary \
+                    under group \033[1m{group}\033[0m."
+                )
             data[name] = []
             data["_GROUPS_"][group].append(dataset)
 
             # Add a counter for this dataset for the group with which it is associated.
             counter = data["_MAP_DATASETS_TO_COUNTERS_"][group]
             # counter_name = "%s/%s" % (group,counter)
             data["_MAP_DATASETS_TO_COUNTERS_"][name] = counter
 
             data["_MAP_DATASETS_TO_DATA_TYPES_"][name] = dtype
 
     return 0
 
 
+###############################################################################
+def add_meta(data: dict, name: str, meta_data: list):
+    """
+    Create metadata for a group (or singleton) and add it to data
+
+    Args:
+        data (dict): a data object returned by hf.initialize()
+        name (str): name of either a group, singleton, or dataset the metadata corresponds to.
+                    if passing a dataset name, make sure it is the full path (group/dataset)!
+        meta_data (list): list of metadata to write to that group/dataset/singleton
+    """
+
+    if name in data["_META_"].keys():
+        warnings.warn(
+            f"This name {name} already has metadata in the hepfile data, skipping!"
+        )
+        return
+
+    data["_META_"][name] = meta_data  # empty list for metadata
+
+
 ################################################################################
-def pack(data, bucket, AUTO_SET_COUNTER=True, EMPTY_OUT_BUCKET=True, STRICT_CHECKING=False, verbose=False):
-    """ Takes the data from an bucket and packs it into the data dictionary, 
-    intelligently, so that it can be stored and extracted efficiently. 
+def pack(
+    data: dict,
+    bucket: dict,
+    AUTO_SET_COUNTER: bool = True,
+    EMPTY_OUT_BUCKET: bool = True,
+    STRICT_CHECKING: bool = False,
+    verbose: bool = False,
+):
+    """Takes the data from an bucket and packs it into the data dictionary,
+    intelligently, so that it can be stored and extracted efficiently.
     (This is analagous to the ROOT TTree::Fill() member function).
 
     Args:
-        **data** (dict): Data dictionary to hold the entire dataset EDIT.
+        data (dict): Data dictionary to hold the entire dataset EDIT.
 
-        **bucket** (dict): bucket to be packed into data.
+        bucket (dict): bucket to be packed into data.
 
-        **EMPTY_OUT_BUCKET** (bool): If this is `True` then empty out the `bucket`
-                                container in preparation for the next iteration. We used to ask the users to do
-                                this "by hand" but now do it automatically by default. We allow the user to 
-                                not do this, if they are running some sort of debugging. 
+        EMPTY_OUT_BUCKET (bool): If this is `True` then empty out the `bucket`
+                                container in preparation for the next iteration.
+                                We used to ask the users to do this "by hand" but
+                                now do it automatically by default. We allow the user to
+                                not do this, if they are running some sort of debugging.
 
     """
 
     # Calculate the number of entries for each group and set the
     # value of that counter
     # This is all done in bucket
     if AUTO_SET_COUNTER:
-        for group in data['_GROUPS_']:
-
+        for group in data["_GROUPS_"]:
             if verbose:
                 print(f"group: {group}")
 
-            datasets = data['_GROUPS_'][group]
-            counter = data['_MAP_DATASETS_TO_COUNTERS_'][group]
-            if counter == '_SINGLETONS_GROUP_/COUNTER':
+            datasets = data["_GROUPS_"][group]
+            counter = data["_MAP_DATASETS_TO_COUNTERS_"][group]
+            if counter == "_SINGLETONS_GROUP_/COUNTER":
                 continue
 
             # Here we will calculate the values for the counters, based
             # on the size of the datasets
             counter_value = None
 
             # Loop over the datasets
-            for d in datasets:
-                full_dataset_name = group + "/" + d
+            for dset in datasets:
+                full_dataset_name = group + "/" + dset
                 # Skip any counters
                 if counter == full_dataset_name:
                     continue
-                else:
-                    # Grab the size of the first dataset
-                    temp_counter_value = len(bucket[full_dataset_name])
 
-                    # If we're not STRICT_CHECKING, then use that value for the
-                    # counter and break the loop over the datasets, moving on
-                    # to the next group.
-                    if STRICT_CHECKING is False:
-                        bucket[counter] = temp_counter_value
-                        break
-                    # Otherwise, we'll check that *all* the datasets have the same
-                    # length.
-                    else:
-                        if counter_value is None:
-                            counter_value = temp_counter_value
-                            bucket[counter] = temp_counter_value
-                        elif counter_value != temp_counter_value:
-                            # In this case, we found two groups of different length!
-                            # Print this to help the user identify their error
-                            print(
-                                f"Oh no!!!! Two datasets in group {group} have different sizes!")
-                            for tempd in datasets:
-                                temp_full_dataset_name = group + "/" + tempd
-                                # Don't worry about the dataset
-                                if counter == temp_full_dataset_name:
-                                    continue
-                                print(
-                                    f"{tempd}: {len(bucket[temp_full_dataset_name])}")
+                # Grab the size of the first dataset
+                temp_counter_value = len(bucket[full_dataset_name])
 
-                            # Return a value for the external program to catch.
-                            return -1
+                # If we're not STRICT_CHECKING, then use that value for the
+                # counter and break the loop over the datasets, moving on
+                # to the next group.
+                if STRICT_CHECKING is False:
+                    bucket[counter] = temp_counter_value
+                    break
+                # Otherwise, we'll check that *all* the datasets have the same
+                # length.
+                if counter_value is None:
+                    counter_value = temp_counter_value
+                    bucket[counter] = temp_counter_value
+                elif counter_value != temp_counter_value:
+                    # In this case, we found two groups of different length!
+                    # Print this to help the user identify their error
+                    err = ""
+                    for tempd in datasets:
+                        temp_full_dataset_name = group + "/" + tempd
+                        # Don't worry about the dataset
+                        if counter == temp_full_dataset_name:
+                            continue
+                        err += f"{tempd}: {len(bucket[temp_full_dataset_name])}\n"
+
+                    # Raise an exception for the external program to catch.
+                    raise DatasetSizeDiscrepancy(
+                        f"Oh no!!!! Two datasets in group {group} have different sizes! {err}"
+                    )
 
     # Then pack the bucket into the data
     keys = list(bucket.keys())
 
     for key in keys:
-
-        if (
-            key == "_MAP_DATASETS_TO_COUNTERS_"
-            or key == "_GROUPS_"
-            or key == "_LIST_OF_COUNTERS_"
-            or key == "_MAP_DATASETS_TO_DATA_TYPES_"
-        ):
+        if key in {
+            "_MAP_DATASETS_TO_COUNTERS_",
+            "_GROUPS_",
+            "_LIST_OF_COUNTERS_",
+            "_MAP_DATASETS_TO_DATA_TYPES_",
+            "_META_",
+            "_PROTECTED_NAMES_",
+        }:
             continue
 
         # The singletons will only have 1 entry per bucket
         if key == "_SINGLETONS_GROUP_/COUNTER":
             data[key].append(1)
             continue
 
-        if type(bucket[key]) == list:
+        if isinstance(bucket[key], (list, np.ndarray)):
             value = bucket[key]
+            if isinstance(value, np.ndarray):
+                value = value.tolist()
             if len(value) > 0:
                 data[key] += value
         else:
             # This is for counters and SINGLETONS
             if key in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
-                if bucket[key] == None:
-                    print(f"\n\033[1m{key}\033[0m is part of the SINGLETON group and is expected to have a value for each bucket.")
-                    print("However it is None...exiting.\n")
-                    exit()
+                if bucket[key] is None:
+                    raise MissingSingletonValue(
+                        f"\n\033[1m{key}\033[0m is part of the SINGLETON group \
+                        and is expected to have a value for each bucket. However it is None!"
+                    )
+
                 # Append the single value from the singletons
-                else:
-                    data[key].append(bucket[key])
+                data[key].append(bucket[key])
             # Append the values to the counters
             else:
                 data[key].append(bucket[key])
 
     # Clear out the bucket after it's been packed if that's what we want
     if EMPTY_OUT_BUCKET:
         clear_bucket(bucket)
 
     return 0
 
+
 ################################################################################
 
 
-def convert_list_and_key_to_string_data(datalist, key):
-    """ Converts data dictionary to a string
+def _convert_list_and_key_to_string_data(datalist: list[any], key: str) -> str:
+    """Converts data dictionary to a string
 
     Args:
-        **datalist** (list): A list to be saved as a string.
+        datalist (list): A list to be saved as a string.
 
     Returns:
-        **key** (string): We will assume that this will be unpacked as a dictionary,
+        key (string): We will assume that this will be unpacked as a dictionary,
                       and this will be the key for the list in that dictionary.
-
+        length (int): length of the dataset (needed for writing strings to h5 files)
     """
-
-    a = np.string_(key)
+    stra = np.string_(key)
 
     mydataset = []
-    b = np.string_("")
+    strb = np.string_("")
     nvals = len(datalist)
     for i, val in enumerate(datalist):
-        b += np.string_(val)
+        strb += np.string_(val)
         if i < nvals - 1:
-            b += np.string_("__:__")
-    mydataset.append([a, b])
+            strb += np.string_("__:__")
+    mydataset.append([stra, strb])
 
-    return mydataset
+    return mydataset, len(strb)
 
 
 ################################################################################
 
+
 ################################################################################
-def convert_dict_to_string_data(dictionary):
-    """ Converts data dictionary to a string
+def _convert_dict_to_string_data(dictionary: dict) -> str:
+    """Converts data dictionary to a string
 
     Args:
-        **dictionary** (dict): Dictionary to be converted to a string
+        dictionary (dict): Dictionary to be converted to a string
 
     Returns:
-        **mydataset** (string): String representation of the dataset
+        mydataset (string): String representation of the dataset
 
     """
 
-    keys = dictionary.keys()
+    mydataset = []
+    longest_str_length = 0
+    for key in dictionary:
+        astr = np.string_(key)
+        longest_str_length = max(len(astr), longest_str_length)
 
-    nkeys = len(keys)
+        bstr = np.string_(dictionary[key])
+        longest_str_length = max(len(bstr), longest_str_length)
 
-    mydataset = []
-    for i, key in enumerate(keys):
-        a = np.string_(key)
-        b = np.string_(dictionary[key])
-        mydataset.append([a, b])
+        mydataset.append([astr, bstr])
 
-    return mydataset
+    return mydataset, longest_str_length
 
 
 ################################################################################
 # This function writes default attributes and metadata to a file.
 ################################################################################
-def write_file_metadata(filename, mydict={}, write_default_values=True, append=True):
-    """ Writes file metadata in the attributes of an HDF5 file
+def write_file_metadata(
+    filename: str,
+    mydict: dict = None,
+    write_default_values: bool = True,
+    append: bool = True,
+) -> h5.File:
+    """Writes file metadata in the attributes of an HDF5 file
 
     Args:
-    **filename** (string): Name of output file
+    filename (string): Name of output file
 
-    **mydict** (dictionary): Metadata desired by user
+    mydict (dictionary): Metadata desired by user
 
-    **write_default_values** (boolean): True if user wants to write/update the 
-                                        default metadata: date, hepfile version, 
-                                        h5py version, numpy version, and Python 
+    write_default_values (boolean): True if user wants to write/update the
+                                        default metadata: date, hepfile version,
+                                        h5py version, numpy version, and Python
                                         version, false if otherwise.
 
-    **append** (boolean): True if user wants to keep older metadata, false otherwise.
+    append (boolean): True if user wants to keep older metadata, false otherwise.
 
     Returns:
-    **hdoutfile** (HDF5): File with new metadata
+    hdoutfile (HDF5): File with new metadata
 
     """
 
-    hdoutfile = h5.File(filename, "a")
+    with h5.File(filename, "a") as hdoutfile:
+        # hdoutfile = h5.File(filename, "a")
+
+        non_metadata = ["_NUMBER_OF_BUCKETS_"]
+
+        if not append:
+            for key in hdoutfile.attrs:
+                if key not in non_metadata:
+                    del hdoutfile.attrs[key]
+
+        if write_default_values:
+            hdoutfile.attrs["date"] = datetime.datetime.now().isoformat(sep=" ")
+            hdoutfile.attrs["hepfile_version"] = hepfile.__version__
+            hdoutfile.attrs["numpy_version"] = np.__version__
+            hdoutfile.attrs["h5py_version"] = h5.__version__
+            hdoutfile.attrs["awkward_version"] = ak.__version__
+            hdoutfile.attrs["python_version"] = sys.version
+
+        if mydict is not None:
+            for key in mydict:
+                hdoutfile.attrs[key] = mydict[key]
+
+    print("Metadata added")
+    return hdoutfile
+
 
-    non_metadata = ["_NUMBER_OF_BUCKETS_"]
+################################################################################
+# This function writes a set of user-defined header information to the
+# hepfile
+################################################################################
+def write_file_header(filename: str, mydict: dict) -> h5.File:
+    """
+    Writes header data to a protected group in an HDF5 file.
 
-    if not append:
-        for key in hdoutfile.attr.keys():
-            if key not in non_metadata:
-                del hdoutfile.attrs[key]
+    If there is already header information, it is overwritten
+    by this function.
 
-    if write_default_values:
-        hdoutfile.attrs["date"] = datetime.datetime.now().isoformat(sep=" ")
-        hdoutfile.attrs["hepfile_version"] = hepfile.__version__
-        hdoutfile.attrs["numpy_version"] = np.__version__
-        hdoutfile.attrs["h5py_version"] = h5.__version__
-        hdoutfile.attrs["python_version"] = sys.version
+    Args:
+        filename (string): Name of file to write to (file should already exist
+                           and the group will be appended to it.)
 
-    for key in mydict:
-        hdoutfile.attrs[key] = mydict[key]
+        mydict (dictionary): Header data passed in by user
 
+    Returns:
+        hdoutfile (HDF5): Returns the file with new metadata
+
+    """
+
+    if len(mydict.keys()) == 0:
+        raise InputError("Please provide header data to write to the header!")
+
+    with h5.File(filename, "a") as hdoutfile:
+        # We are going to write *all* the values as strings. The user can
+        # change the type upon reading, if they so choose.
+        dtype = h5.string_dtype(encoding="utf-8")
+
+        # If the _HEADER_ group exists, delete it.
+        header_group = None
+        if "_HEADER_" in hdoutfile:
+            del hdoutfile["_HEADER_"]
+
+        header_group = hdoutfile.create_group("_HEADER_")
+
+        for key in mydict.keys():
+            values = mydict[key]
+
+            # check that values can be converted to a np.array
+            try:
+                values = np.array(values)
+            except Exception as err:
+                raise InputError(
+                    "Unable to convert header data to a numpy array!"
+                ) from err
+
+            # If value is just a str, int, or float, make it an array
+            if isinstance(values, (str, float, int)):
+                values = values.astype(str)
+
+            # When we pass in the values, we need to do it as a list (NOT SURE WHY?)
+            header_group.create_dataset(
+                key, (len(values), 1), dtype=dtype, data=values.tolist()
+            )
+
+    # DO WE WANT TO DO THIS HERE?
     hdoutfile.close()
-    print("Metadata added")
+
+    print("Header data added")
     return hdoutfile
 
 
 ################################################################################
 
 ################################################################################
+
+
+################################################################################
 def write_to_file(
-    filename, data, comp_type=None, comp_opts=None, force_single_precision=True,  verbose=False
-):
-    """ Writes the selected data to an HDF5 file
+    filename: str,
+    data: dict,
+    comp_type: str = None,
+    comp_opts: list = None,
+    force_single_precision: bool = True,
+    verbose: bool = False,
+) -> h5.File:
+    """Writes the selected data to an HDF5 file
 
     Args:
-        **filename** (string): Name of output file
+        filename (string): Name of output file
 
-        **data** (dictionary): Data to be written into output file
+        data (dictionary): Data to be written into output file
 
-        **comp_type** (string): Type of compression
+        comp_type (string): Type of compression
 
-        **force_single_precision** (boolean): True if data should be written in single precision
+        force_single_precision (boolean): True if data should be written in single precision
 
     Returns:
-        **hdoutfile** (HDF5): File to which the data has been written 
+        hdoutfile (HDF5): File to which the data has been written
 
     """
 
-    hdoutfile = h5.File(filename, "w")
+    # hdoutfile = h5.File(filename, "w")
 
-    _GROUPS_ = data["_GROUPS_"].keys()
+    with h5.File(filename, "w") as hdoutfile:
+        groups = data["_GROUPS_"].keys()
 
-    # Convert this to a 2xN array for writing to the hdf5 file.
-    # This gives us one small list of informtion if we need to pull out
-    # small chunks of data
-    mydataset = convert_dict_to_string_data(data["_MAP_DATASETS_TO_COUNTERS_"])
-    dset = hdoutfile.create_dataset(
-        "_MAP_DATASETS_TO_COUNTERS_",
-        data=mydataset,
-        dtype="S256",
-        compression=comp_type,
-        compression_opts=comp_opts,
-    )
-
-    # Convert this to a 2xN array for writing to the hdf5 file.
-    # This has the _GROUPS_ and the datasets in them.
-    mydataset = convert_list_and_key_to_string_data(
-        data["_GROUPS_"]["_SINGLETONS_GROUP_"], "_SINGLETONSGROUPFORSTORAGE_"
-    )
-    dset = hdoutfile.create_dataset(
-        "_SINGLETONSGROUPFORSTORAGE_",
-        data=mydataset,
-        dtype="S256",
-        compression=comp_type,
-        compression_opts=comp_opts,
-    )
-
-    for group in _GROUPS_:
-
-        hdoutfile.create_group(group)
-        hdoutfile[group].attrs["counter"] = np.string_(
-            data["_MAP_DATASETS_TO_COUNTERS_"][group]
+        # Convert this to a 2xN array for writing to the hdf5 file.
+        # This gives us one small list of informtion if we need to pull out
+        # small chunks of data
+        mydataset, length = _convert_dict_to_string_data(
+            data["_MAP_DATASETS_TO_COUNTERS_"]
+        )
+        hdoutfile.create_dataset(
+            "_MAP_DATASETS_TO_COUNTERS_",
+            data=mydataset,
+            dtype=f"S{length}",
+            compression=comp_type,
+            compression_opts=comp_opts,
         )
 
-        datasets = data["_GROUPS_"][group]
+        # Convert this to a 2xN array for writing to the hdf5 file.
+        # This has the _GROUPS_ and the datasets in them.
+        mydataset, length = _convert_list_and_key_to_string_data(
+            data["_GROUPS_"]["_SINGLETONS_GROUP_"], "_SINGLETONSGROUPFORSTORAGE_"
+        )
 
-        for dataset in datasets:
+        hdoutfile.create_dataset(
+            "_SINGLETONSGROUPFORSTORAGE_",
+            data=mydataset,
+            dtype=f"S{length}",
+            compression=comp_type,
+            compression_opts=comp_opts,
+        )
 
-            name = None
-            if group == "_SINGLETONS_GROUP_" and dataset is not "COUNTER":
-                name = dataset
-            else:
-                name = "%s/%s" % (group, dataset)
+        for group in groups:
+            hdoutfile.create_group(group)
+            hdoutfile[group].attrs["counter"] = np.string_(
+                data["_MAP_DATASETS_TO_COUNTERS_"][group]
+            )
+
+            if group in data["_META_"].keys():
+                hdoutfile[group].attrs["meta"] = np.string_(data["_META_"][group])
+
+            datasets = data["_GROUPS_"][group]
+
+            for dataset in datasets:
+                name = None
+                if group == "_SINGLETONS_GROUP_" and dataset != "COUNTER":
+                    name = dataset
+                else:
+                    name = f"{group}/{dataset}"
 
-            x = data[name]
+                if verbose is True:
+                    print(f"Writing {name} to file")
 
-            dataset_dtype = data['_MAP_DATASETS_TO_DATA_TYPES_'][name]
+                x = data[name]
 
-            if type(x) == list:
-                x = np.array(x)
+                dataset_dtype = data["_MAP_DATASETS_TO_DATA_TYPES_"][name]
 
-            # Do single precision only, unless specified
-            if force_single_precision == True:
-                if x.dtype == np.float64:
-                    x = x.astype(np.float32)
-                    dataset_dtype = np.float32
+                if isinstance(x, list):
+                    if verbose is True:
+                        print("\tConverting list to array...")
+                    x = np.array(x)
+
+                # Do single precision only, unless specified
+                if force_single_precision:
+                    # different type calls depending on input datastructure
+                    if isinstance(x, np.ndarray):
+                        dtype = x.dtype
+                    elif isinstance(x, (ak.Array, ak.Record)):
+                        dtype = x.type
+                    else:
+                        dtype = None
+                        warnings.warn(
+                            "Not a proper data type to convert to single precision, skipping!"
+                        )
+
+                    if dtype == np.float64:
+                        if verbose is True:
+                            print("\tConverting array to single precision...")
+                        x = x.astype(np.float32)
+                        dataset_dtype = np.float32
+
+                if dataset_dtype is not str:
+                    if verbose is True:
+                        print("\tWriting to file...")
+                    hdoutfile.create_dataset(
+                        name,
+                        data=x,
+                        compression=comp_type,
+                        compression_opts=comp_opts,
+                        dtype=dataset_dtype,
+                    )
+                else:
+                    # For writing strings, we need to make sure our strings are ascii
+                    # and not Unicode
+                    #
+                    # See my question on StackOverflow and the super-helpful response!
+                    #
+                    # https://stackoverflow.com/questions/68500454/can-i-use-h5py-to-write-strings-to-an-hdf5-file-in-one-line-rather-than-looping
+                    dataset_dtype = h5.special_dtype(vlen=str)
+                    longest_word = len(max(x, key=len))
+                    arr = np.array(x, dtype="S" + str(longest_word))
+                    hdoutfile.create_dataset(
+                        name,
+                        data=arr,
+                        dtype=dataset_dtype,
+                        compression=comp_type,
+                        compression_opts=comp_opts,
+                    )
+
+                # write the dataset metadata if there is some
+                if name in data["_META_"]:
+                    hdoutfile[name].attrs["meta"] = np.string_(data["_META_"][name])
+
+                if verbose:
+                    print(f"Writing to file {name} as type {str(dataset_dtype)}")
+
+        # Get the number of buckets
+        counters = data["_LIST_OF_COUNTERS_"]
+        num_buckets = -1
+        prevcounter = None
+        for i, countername in enumerate(counters):
+            ncounter = len(data[countername])
+
+            if verbose:
+                print(f"{countername:<32s} has {ncounter:<12d} entries")
 
-            if dataset_dtype is not str:
-                hdoutfile.create_dataset(
-                    name, data=x, compression=comp_type, compression_opts=comp_opts, dtype=dataset_dtype
+            if i > 0 and ncounter != num_buckets:
+                warnings.warn(
+                    f"{countername} and {prevcounter} have differing numbers of entries!"
                 )
-            else:
-                # For writing strings, we need to make sure our strings are ascii and not Unicode
-                #
-                # See my question on StackOverflow and the super-helpful response!
-                #
-                # https://stackoverflow.com/questions/68500454/can-i-use-h5py-to-write-strings-to-an-hdf5-file-in-one-line-rather-than-looping
-                dataset_dtype = h5.special_dtype(vlen=str)
-                longest_word = len(max(x, key=len))
-                arr = np.array(x, dtype='S'+str(longest_word))
-                hdoutfile.create_dataset(
-                    name, data=arr, dtype=dataset_dtype,  compression=comp_type, compression_opts=comp_opts)
-
-            if (verbose):
-                print(f"Writing to file {name} as type {str(dataset_dtype)}")
-
-    # Get the number of buckets
-    counters = data["_LIST_OF_COUNTERS_"]
-    _NUMBER_OF_BUCKETS_ = -1
-    prevcounter = None
-    for i, countername in enumerate(counters):
-        ncounter = len(data[countername])
-        #print("%-32s has %-12d entries" % (countername, ncounter))
-        print(f"{countername:<32s} has {ncounter:<12d} entries")
-        if i > 0 and ncounter != _NUMBER_OF_BUCKETS_:
-            print("-------- WARNING -----------")
-            print(f"{countername} and {prevcounter} have differing numbers of entries!")
-            print("-------- WARNING -----------")
-            # SHOULD WE EXIT ON THIS?
+                # SHOULD WE EXIT ON THIS?
 
-        if _NUMBER_OF_BUCKETS_ < ncounter:
-            _NUMBER_OF_BUCKETS_ = ncounter
+            num_buckets = max(num_buckets, ncounter)
 
-        prevcounter = countername
+            prevcounter = countername
 
-    hdoutfile.attrs["_NUMBER_OF_BUCKETS_"] = _NUMBER_OF_BUCKETS_
-    hdoutfile.close()
+        hdoutfile.attrs["_NUMBER_OF_BUCKETS_"] = num_buckets
+        # hdoutfile.close()
 
     write_file_metadata(filename)
 
     return hdoutfile
```

