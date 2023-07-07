# Comparing `tmp/linex2-1.1.8.tar.gz` & `tmp/linex2-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linex2-1.1.8.tar", last modified: Tue Jan  3 11:04:37 2023, max compression
+gzip compressed data, was "linex2-1.1.9.tar", last modified: Thu Jan 19 13:25:53 2023, max compression
```

## Comparing `linex2-1.1.8.tar` & `linex2-1.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-03 12:06:01.503933 linex2-1.1.8/
--rwxrwxrwx   0 trose     (1000) trose     (1000)    34640 2022-10-25 11:28:53.000000 linex2-1.1.8/LICENSE.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)     3383 2023-01-03 12:06:01.503933 linex2-1.1.8/PKG-INFO
--rwxrwxrwx   0 trose     (1000) trose     (1000)     2408 2023-01-03 11:52:25.000000 linex2-1.1.8/README.md
-drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-03 12:06:00.132360 linex2-1.1.8/linex2/
--rwxrwxrwx   0 trose     (1000) trose     (1000)    17378 2022-11-02 09:39:57.000000 linex2-1.1.8/linex2/GenerateLipidNetwork.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)   120333 2023-01-03 11:55:13.000000 linex2-1.1.8/linex2/LipidNetwork.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     1415 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/__init__.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    38713 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/_network_analysis.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    13882 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/_network_compute_statistics.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     6834 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/_network_lipid_utils.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    21951 2023-01-03 11:55:13.000000 linex2-1.1.8/linex2/_network_lipidome_summary.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     2974 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/colour_helper.py
-drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-03 12:06:01.173011 linex2-1.1.8/linex2/data/
--rwxrwxrwx   0 trose     (1000) trose     (1000)  1358929 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/Reactome_ConnectionOfReactionsToMolecule_all.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   220411 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/Reactome_Others_all_unique.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   713888 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/Reactome_ReactionDetailsEnzyme_all.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   287418 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/Reactome_reactions_for_curation.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   612917 2022-12-06 14:39:21.000000 linex2-1.1.8/linex2/data/Rhea_ConnectionOfReactionsToMolecule_all.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   810451 2022-12-06 14:48:47.000000 linex2-1.1.8/linex2/data/Rhea_GeneName_mapping.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   243660 2022-12-06 15:03:14.000000 linex2-1.1.8/linex2/data/Rhea_Others_all_unique.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)      503 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/Rhea_ReactionDetailsEnzyme.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)   600409 2022-12-06 14:41:56.000000 linex2-1.1.8/linex2/data/Rhea_reactions_for_curation.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)        0 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/__init__.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)      740 2022-10-25 11:28:53.000000 linex2-1.1.8/linex2/data/citing_data.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)      760 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/data/default_fatty_acids.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)     9824 2022-12-06 15:27:18.000000 linex2-1.1.8/linex2/data/standard_lipid_classes.csv
--rwxrwxrwx   0 trose     (1000) trose     (1000)    12890 2022-11-25 12:39:42.000000 linex2-1.1.8/linex2/edgelist.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     2384 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/exceptions.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    17406 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/libAP_nx.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    24235 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/lipid.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     1229 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/load_data.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     4790 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/misc.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    16507 2022-11-22 13:41:48.000000 linex2-1.1.8/linex2/parser.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     8654 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/reaction.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    36782 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/reaction_evaluation.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)      322 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/reaction_types.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    11564 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/reference.py
-drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-03 12:06:01.456867 linex2-1.1.8/linex2/templates/
--rwxrwxrwx   0 trose     (1000) trose     (1000)        0 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/templates/__init__.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     2468 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/templates/lipid_colours.json
--rwxrwxrwx   0 trose     (1000) trose     (1000)    32525 2022-10-26 08:50:43.000000 linex2-1.1.8/linex2/templates/vis_dynamic.html
--rwxrwxrwx   0 trose     (1000) trose     (1000)    12479 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/templates/vis_main.html
--rwxrwxrwx   0 trose     (1000) trose     (1000)    26109 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/tmp_dirty_functions.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    34799 2023-01-03 11:55:13.000000 linex2-1.1.8/linex2/utils.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)     5786 2022-12-06 14:56:34.000000 linex2-1.1.8/linex2/validation.py
--rwxrwxrwx   0 trose     (1000) trose     (1000)    45371 2022-10-25 11:28:54.000000 linex2-1.1.8/linex2/vis_utils.py
-drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-03 12:06:00.386370 linex2-1.1.8/linex2.egg-info/
--rwxrwxrwx   0 trose     (1000) trose     (1000)     3383 2023-01-03 12:05:57.000000 linex2-1.1.8/linex2.egg-info/PKG-INFO
--rwxrwxrwx   0 trose     (1000) trose     (1000)     1437 2023-01-03 12:05:58.000000 linex2-1.1.8/linex2.egg-info/SOURCES.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)        1 2023-01-03 12:05:57.000000 linex2-1.1.8/linex2.egg-info/dependency_links.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)        1 2022-10-25 11:28:55.000000 linex2-1.1.8/linex2.egg-info/not-zip-safe
--rwxrwxrwx   0 trose     (1000) trose     (1000)       74 2023-01-03 12:05:57.000000 linex2-1.1.8/linex2.egg-info/requires.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)        7 2023-01-03 12:05:57.000000 linex2-1.1.8/linex2.egg-info/top_level.txt
--rwxrwxrwx   0 trose     (1000) trose     (1000)       78 2023-01-03 12:06:01.520855 linex2-1.1.8/setup.cfg
--rwxrwxrwx   0 trose     (1000) trose     (1000)     1709 2023-01-03 11:56:27.000000 linex2-1.1.8/setup.py
+drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-19 13:25:53.658869 linex2-1.1.9/
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    34640 2022-10-25 11:28:53.000000 linex2-1.1.9/LICENSE.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     3383 2023-01-19 13:25:53.658964 linex2-1.1.9/PKG-INFO
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     2408 2023-01-03 11:52:25.000000 linex2-1.1.9/README.md
+drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-19 13:25:51.958929 linex2-1.1.9/linex2/
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    17378 2022-11-02 09:39:57.000000 linex2-1.1.9/linex2/GenerateLipidNetwork.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   120333 2023-01-03 11:55:13.000000 linex2-1.1.9/linex2/LipidNetwork.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     1415 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/__init__.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    38713 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/_network_analysis.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    13882 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/_network_compute_statistics.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     6834 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/_network_lipid_utils.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    21951 2023-01-03 11:55:13.000000 linex2-1.1.9/linex2/_network_lipidome_summary.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     2974 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/colour_helper.py
+drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-19 13:25:53.190437 linex2-1.1.9/linex2/data/
+-rwxrwxrwx   0 trose     (1000) trose     (1000)  1358929 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/Reactome_ConnectionOfReactionsToMolecule_all.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   220411 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/Reactome_Others_all_unique.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   713888 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/Reactome_ReactionDetailsEnzyme_all.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   287418 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/Reactome_reactions_for_curation.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   612917 2022-12-06 14:39:21.000000 linex2-1.1.9/linex2/data/Rhea_ConnectionOfReactionsToMolecule_all.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   810451 2022-12-06 14:48:47.000000 linex2-1.1.9/linex2/data/Rhea_GeneName_mapping.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   243660 2022-12-06 15:03:14.000000 linex2-1.1.9/linex2/data/Rhea_Others_all_unique.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)      503 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/Rhea_ReactionDetailsEnzyme.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)   600409 2022-12-06 14:41:56.000000 linex2-1.1.9/linex2/data/Rhea_reactions_for_curation.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)        0 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/__init__.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)      740 2022-10-25 11:28:53.000000 linex2-1.1.9/linex2/data/citing_data.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)      760 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/data/default_fatty_acids.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     9844 2023-01-17 10:44:51.000000 linex2-1.1.9/linex2/data/standard_lipid_classes.csv
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    12890 2022-11-25 12:39:42.000000 linex2-1.1.9/linex2/edgelist.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     2384 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/exceptions.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    17406 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/libAP_nx.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    24235 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/lipid.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     1229 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/load_data.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     4790 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/misc.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    16507 2022-11-22 13:41:48.000000 linex2-1.1.9/linex2/parser.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     8654 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/reaction.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    36782 2023-01-17 13:10:05.000000 linex2-1.1.9/linex2/reaction_evaluation.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)      322 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/reaction_types.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    11564 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/reference.py
+drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-19 13:25:53.579288 linex2-1.1.9/linex2/templates/
+-rwxrwxrwx   0 trose     (1000) trose     (1000)        0 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/templates/__init__.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     2468 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/templates/lipid_colours.json
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    32525 2022-10-26 08:50:43.000000 linex2-1.1.9/linex2/templates/vis_dynamic.html
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    12479 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/templates/vis_main.html
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    26109 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/tmp_dirty_functions.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    34799 2023-01-03 11:55:13.000000 linex2-1.1.9/linex2/utils.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     5786 2022-12-06 14:56:34.000000 linex2-1.1.9/linex2/validation.py
+-rwxrwxrwx   0 trose     (1000) trose     (1000)    45371 2022-10-25 11:28:54.000000 linex2-1.1.9/linex2/vis_utils.py
+drwxrwxrwx   0 trose     (1000) trose     (1000)        0 2023-01-19 13:25:52.174320 linex2-1.1.9/linex2.egg-info/
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     3383 2023-01-19 13:25:49.000000 linex2-1.1.9/linex2.egg-info/PKG-INFO
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     1437 2023-01-19 13:25:50.000000 linex2-1.1.9/linex2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)        1 2023-01-19 13:25:49.000000 linex2-1.1.9/linex2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)        1 2022-10-25 11:28:55.000000 linex2-1.1.9/linex2.egg-info/not-zip-safe
+-rwxrwxrwx   0 trose     (1000) trose     (1000)       74 2023-01-19 13:25:49.000000 linex2-1.1.9/linex2.egg-info/requires.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)        7 2023-01-19 13:25:49.000000 linex2-1.1.9/linex2.egg-info/top_level.txt
+-rwxrwxrwx   0 trose     (1000) trose     (1000)       78 2023-01-19 13:25:53.668724 linex2-1.1.9/setup.cfg
+-rwxrwxrwx   0 trose     (1000) trose     (1000)     1709 2023-01-19 13:19:07.000000 linex2-1.1.9/setup.py
```

### Comparing `linex2-1.1.8/LICENSE.txt` & `linex2-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/PKG-INFO` & `linex2-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linex2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Lipid Network Explorer 2 (LINEX2) package. Python backend to the LINEX web-app
 Home-page: https://exbio.wzw.tum.de/linex/
 Author: Tim Daniel Rose, Nikolai Koehler, Olga Lazareva, Josch Konstantin Pauling
 Author-email: tim.rose@tum.de, nikolai.koehler@tum.de
 License: AGPLv3
 Project-URL: Source, https://gitlab.lrz.de/lipitum-projects/linex2_package
 Project-URL: Publication, https://doi.org/10.1093/bib/bbac572
```

### Comparing `linex2-1.1.8/README.md` & `linex2-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/GenerateLipidNetwork.py` & `linex2-1.1.9/linex2/GenerateLipidNetwork.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/LipidNetwork.py` & `linex2-1.1.9/linex2/LipidNetwork.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/__init__.py` & `linex2-1.1.9/linex2/__init__.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/_network_analysis.py` & `linex2-1.1.9/linex2/_network_analysis.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/_network_compute_statistics.py` & `linex2-1.1.9/linex2/_network_compute_statistics.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/_network_lipid_utils.py` & `linex2-1.1.9/linex2/_network_lipid_utils.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/_network_lipidome_summary.py` & `linex2-1.1.9/linex2/_network_lipidome_summary.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/colour_helper.py` & `linex2-1.1.9/linex2/colour_helper.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Reactome_ConnectionOfReactionsToMolecule_all.csv` & `linex2-1.1.9/linex2/data/Reactome_ConnectionOfReactionsToMolecule_all.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Reactome_Others_all_unique.csv` & `linex2-1.1.9/linex2/data/Reactome_Others_all_unique.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Reactome_ReactionDetailsEnzyme_all.csv` & `linex2-1.1.9/linex2/data/Reactome_ReactionDetailsEnzyme_all.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Reactome_reactions_for_curation.csv` & `linex2-1.1.9/linex2/data/Reactome_reactions_for_curation.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Rhea_ConnectionOfReactionsToMolecule_all.csv` & `linex2-1.1.9/linex2/data/Rhea_ConnectionOfReactionsToMolecule_all.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Rhea_GeneName_mapping.csv` & `linex2-1.1.9/linex2/data/Rhea_GeneName_mapping.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Rhea_Others_all_unique.csv` & `linex2-1.1.9/linex2/data/Rhea_Others_all_unique.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/Rhea_reactions_for_curation.csv` & `linex2-1.1.9/linex2/data/Rhea_reactions_for_curation.csv`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/citing_data.txt` & `linex2-1.1.9/linex2/data/citing_data.txt`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/default_fatty_acids.txt` & `linex2-1.1.9/linex2/data/default_fatty_acids.txt`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/data/standard_lipid_classes.csv` & `linex2-1.1.9/linex2/data/standard_lipid_classes.csv`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 Glycerophospholipids,Phosphatidylserine,56,PS,,PS 36:2,PS 18:1-18:1,PS,2,2,0,1,0,
 Glycerophospholipids,Plasmanylphosphatidylethanolamine,58b,PE O-a,,PE O-a 36:2,PE O-18:1a/18:1,PE,2,2,1,1,0,
 Glycerophospholipids,Plasmenylphosphatidylethanolamine,58c,PE O-p,,PE O-p 36:2,PE O-18:1p/18:1,PE,2,2,1,1,0,
 Prenol lipids,Dolichol,59,Dol-,,Dol-80,,Dol-,,,0,0,,isoprene
 Prenol lipids,Dolichol phosphate,60,DolP-,,DolP-80,,DolP-,,,0,0,,isoprene
 Prenol lipids,Dolichol phosphate hexose,61,DolPHex-,,DolPHex-80,,DolPHex-,,,0,0,,isoprene
 Sphingolipids,Ceramide phosphate,62,CerP,,CerP 36:1;2,,P ,2,2,0,1,1,sphingoid
-Sphingolipids,Dihexosylceramide,63,Hex2Cer,LacCer ,Hex2Cer 36:2;2,Hex2Cer 18:1;2/18:1,Hex2,2,2,0,1,1,sphingoid
+Sphingolipids,Dihexosylceramide,63,Hex2Cer,LacCer /LacCer,Hex2Cer 36:2;2,Hex2Cer 18:1;2/18:1,Hex2,2,2,0,1,1,sphingoid
 Sphingolipids,Ethanolaminephosphoceramide ,64,EPC,PE-Cer,EPC 36:1;2,,EP,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GA1,,GA1,,,,GA1,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GD1,65,GD1,,GD1 36:2;2,,GD1,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GD2,66,GD2,,GD2 36:2;2,,GD2,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GD3,67,GD3,,GD3 36:2;2,,GD3,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GM1,68,GM1,,GM1 36:2;2,,GM1,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GM2,69,GM2,,GM2 36:2;2,,GM2,2,2,0,1,1,sphingoid
@@ -87,18 +87,18 @@
 Sphingolipids,Ganglioside GT1,71,GT1,,GT1 36:2;2,,GT1,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GT2,72,GT2,,GT2 36:2;2,,GT2,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GT3,73,GT3,,GT3 36:2;2,,GT3,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GQ3,73,GQ3,,GQ3 36:2;2,,GQ3,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GQ2,,GQ2,,,,GQ2,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GQ1,,GQ1,,,,GQ1,2,2,0,1,1,sphingoid
 Sphingolipids,Ganglioside GP3/2/1,73,GP3/2/1,,GP3 36:2;2,,GP3,2,2,0,1,1,sphingoid
-Sphingolipids,Hexosylceramide,74,HexCer,GlcCer,HexCer 36:2;2,HexCer 18:1;2/18:1,Hex,2,2,0,1,1,sphingoid
+Sphingolipids,Hexosylceramide,74,HexCer,GlcCer/GalCer,HexCer 36:2;2,HexCer 18:1;2/18:1,Hex,2,2,0,1,1,sphingoid
 Sphingolipids,Lysoinositolphosphoceramide,75,LIPC,,LIPC 18:1;2,,IP,2,1,0,1,1,sphingoid
 Sphingolipids,Lysomonohexosylceramide,76,LHexCer,,LHexCer 18:1;2,,Hex,2,1,0,1,1,sphingoid
-Sphingolipids,Inositolphosphoceramide,77,IPC,,IPC 36:1;2,IPC 18:0;3/26:0;1,IP,2,2,0,1,1,sphingoid
+Sphingolipids,Inositolphosphoceramide,77,IPC,PI-Cer,IPC 36:1;2,IPC 18:0;3/26:0;1,IP,2,2,0,1,1,sphingoid
 Sphingolipids,Long-chain base,78,LCB,,LCB 18:1;2,,,2,1,0,1,1,sphingoid
 Sphingolipids,Long-chain base phosphate,79,LCBP,SBP,LCBP 18:1;2,,P,2,1,0,1,1,sphingoid
 Sphingolipids,Lysosphingomyelin,80,LSM,,LSM 18:1;2,LSM 18:1;2,PC,2,1,0,1,1,sphingoid
 Sphingolipids,Mannosyldiinositolphosphoceramide,81,M(IP)2C,,M(IP)2C 36:2;2,M(IP)2C 18:0;3/26:0;1,M(IP)2,2,2,0,1,1,sphingoid
 Sphingolipids,Mannosylinositolphosphoceramide,82,MIPC,,MIPC 36:2;2,MIPC 18:0;3/26:0;1,MIP,2,2,0,1,1,sphingoid
 Sphingolipids,Sphingomyelin,83,SM,,SM 36:2;2,SM 18:1;2/18:1,PC,2,2,0,1,1,sphingoid
 Sphingolipids,Sulfatide,84,SHexCer,Sulfatide,SHexCer 36:2;2,SHexCer 18:1;2/18:1,SHex,2,2,0,1,1,sphingoid
```

### Comparing `linex2-1.1.8/linex2/edgelist.py` & `linex2-1.1.9/linex2/edgelist.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/exceptions.py` & `linex2-1.1.9/linex2/exceptions.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/libAP_nx.py` & `linex2-1.1.9/linex2/libAP_nx.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/lipid.py` & `linex2-1.1.9/linex2/lipid.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/load_data.py` & `linex2-1.1.9/linex2/load_data.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/misc.py` & `linex2-1.1.9/linex2/misc.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/parser.py` & `linex2-1.1.9/linex2/parser.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/reaction.py` & `linex2-1.1.9/linex2/reaction.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/reaction_evaluation.py` & `linex2-1.1.9/linex2/reaction_evaluation.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/reference.py` & `linex2-1.1.9/linex2/reference.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/templates/lipid_colours.json` & `linex2-1.1.9/linex2/templates/lipid_colours.json`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/templates/vis_dynamic.html` & `linex2-1.1.9/linex2/templates/vis_dynamic.html`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/templates/vis_main.html` & `linex2-1.1.9/linex2/templates/vis_main.html`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/tmp_dirty_functions.py` & `linex2-1.1.9/linex2/tmp_dirty_functions.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/utils.py` & `linex2-1.1.9/linex2/utils.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/validation.py` & `linex2-1.1.9/linex2/validation.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2/vis_utils.py` & `linex2-1.1.9/linex2/vis_utils.py`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/linex2.egg-info/PKG-INFO` & `linex2-1.1.9/linex2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linex2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Lipid Network Explorer 2 (LINEX2) package. Python backend to the LINEX web-app
 Home-page: https://exbio.wzw.tum.de/linex/
 Author: Tim Daniel Rose, Nikolai Koehler, Olga Lazareva, Josch Konstantin Pauling
 Author-email: tim.rose@tum.de, nikolai.koehler@tum.de
 License: AGPLv3
 Project-URL: Source, https://gitlab.lrz.de/lipitum-projects/linex2_package
 Project-URL: Publication, https://doi.org/10.1093/bib/bbac572
```

### Comparing `linex2-1.1.8/linex2.egg-info/SOURCES.txt` & `linex2-1.1.9/linex2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linex2-1.1.8/setup.py` & `linex2-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='linex2',
-    version='1.1.8',
+    version='1.1.9',
 
     description='Lipid Network Explorer 2 (LINEX2) package. Python backend to the LINEX web-app',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://exbio.wzw.tum.de/linex/',
     project_urls={  # Optional
```

