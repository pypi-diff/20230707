# Comparing `tmp/cazomevolve-0.1.4.tar.gz` & `tmp/cazomevolve-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.1.4.tar", last modified: Fri Jul  7 15:20:43 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.5.tar", last modified: Fri Jul  7 15:57:59 2023, max compression
```

## Comparing `cazomevolve-0.1.4.tar` & `cazomevolve-0.1.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.361043 cazomevolve-0.1.4/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:20:43.361043 cazomevolve-0.1.4/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    38355 2023-07-07 10:26:14.000000 cazomevolve-0.1.4/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.341042 cazomevolve-0.1.4/cazomevolve/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-07-07 15:19:45.000000 cazomevolve-0.1.4/cazomevolve/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.345043 cazomevolve-0.1.4/cazomevolve/cazome/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.345043 cazomevolve-0.1.4/cazomevolve/cazome/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7022 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.345043 cazomevolve-0.1.4/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4889 2023-07-06 19:20:47.000000 cazomevolve-0.1.4/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.349043 cazomevolve-0.1.4/cazomevolve/cazome/explore/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/cazy_classes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/cazy_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/cooccurring_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/identify_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/ie_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17620 2023-07-07 13:58:46.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/pca.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/plot.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.4/cazomevolve/cazome/explore/taxonomies.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.349043 cazomevolve-0.1.4/cazomevolve/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/genomes/__init__.py
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11300 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.353042 cazomevolve-0.1.4/cazomevolve/scripts/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.353042 cazomevolve-0.1.4/cazomevolve/scripts/bash/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/scripts/bash/build_cazy_db.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2401 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/scripts/bash/download_acc_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2078 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/scripts/build_cazy_db.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/cazomevolve_script.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3135 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/scripts/download_acc_genomes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/get_fam_seqs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/run_fam_blast.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/run_fam_diamond.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.341042 cazomevolve-0.1.4/cazomevolve/scripts/tree/
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.353042 cazomevolve-0.1.4/cazomevolve/scripts/tree/ani/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/ani/build_anim_tree.R
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/ani/run_anim.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.353042 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/align_scos.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/backtranslate.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/concatenate_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/extract_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/find_orthologues.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.357043 cazomevolve-0.1.4/cazomevolve/seq_diversity/
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/seq_diversity/get_fam_seqs.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/seq_diversity/run_blastp.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.357043 cazomevolve-0.1.4/cazomevolve/taxs/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/taxs/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11322 2023-07-07 09:52:01.000000 cazomevolve-0.1.4/cazomevolve/taxs/add_taxs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/taxs/ncbi.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.357043 cazomevolve-0.1.4/cazomevolve/utilities/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/utilities/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.361043 cazomevolve-0.1.4/cazomevolve/utilities/parsers/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1529 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4914 2023-07-07 09:52:22.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/add_taxs_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2260 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/build_cazy_db_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3133 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/common_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6316 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6780 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/download_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3477 2023-02-07 13:59:17.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/extract_prot_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4021 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_cazy_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3480 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_dbcan_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2899 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3724 2023-07-06 15:09:54.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4343 2023-07-07 09:49:30.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/parse_cmd.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2257 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/run_blast_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2372 2023-06-06 17:06:20.000000 cazomevolve-0.1.4/cazomevolve/utilities/parsers/run_diamond_parser.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:20:43.345043 cazomevolve-0.1.4/cazomevolve.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2767 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-07-07 15:20:43.000000 cazomevolve-0.1.4/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-07-07 15:20:43.361043 cazomevolve-0.1.4/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4138 2023-07-07 15:19:30.000000 cazomevolve-0.1.4/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    38355 2023-07-07 10:26:14.000000 cazomevolve-0.1.5/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-07-07 15:57:06.000000 cazomevolve-0.1.5/cazomevolve/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7022 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4889 2023-07-06 19:20:47.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.450540 cazomevolve-0.1.5/cazomevolve/cazome/explore/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/identify_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/ie_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17620 2023-07-07 13:58:46.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/pca.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/plot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/taxonomies.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.450540 cazomevolve-0.1.5/cazomevolve/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11300 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/bash/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/bash/build_cazy_db.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2401 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/bash/download_acc_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2078 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3135 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.442540 cazomevolve-0.1.5/cazomevolve/scripts/tree/
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/seq_diversity/
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/taxs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11322 2023-07-07 15:56:51.000000 cazomevolve-0.1.5/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/utilities/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/cazomevolve/utilities/parsers/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1529 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4914 2023-07-07 09:52:22.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/add_taxs_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2260 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/build_cazy_db_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3133 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/common_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6316 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6780 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/download_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3477 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/extract_prot_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4021 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_cazy_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3480 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_dbcan_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2899 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3724 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4343 2023-07-07 09:49:30.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/parse_cmd.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2257 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_blast_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2372 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_diamond_parser.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2767 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-07-07 15:57:59.466540 cazomevolve-0.1.5/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4138 2023-07-07 15:57:02.000000 cazomevolve-0.1.5/setup.py
```

### Comparing `cazomevolve-0.1.4/LICENSE` & `cazomevolve-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/PKG-INFO` & `cazomevolve-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.4
+Version: 0.1.5
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
```

### Comparing `cazomevolve-0.1.4/README.md` & `cazomevolve-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/__init__.py` & `cazomevolve-0.1.5/cazomevolve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __citation__ = "???"
 
 
 def closing_message(job, args):
     """Write closing messsage to terminal
```

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.5/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.5/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.5/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/cazome_sizes.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazome_sizes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/cazy_classes.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/cazy_families.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/cooccurring_families.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/cooccurring_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/identify_families.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/identify_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/ie_cazymes.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/ie_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/parse_data.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/parse_data.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/pca.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/pca.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/plot.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/plot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/cazome/explore/taxonomies.py` & `cazomevolve-0.1.5/cazomevolve/cazome/explore/taxonomies.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.5/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.5/cazomevolve/genomes/download_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/__init__.py` & `cazomevolve-0.1.5/cazomevolve/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/bash/build_cazy_db.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/bash/build_cazy_db.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/bash/download_acc_genomes.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/bash/download_acc_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/build_cazy_db.py` & `cazomevolve-0.1.5/cazomevolve/scripts/build_cazy_db.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/cazomevolve_script.py` & `cazomevolve-0.1.5/cazomevolve/scripts/cazomevolve_script.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/download_acc_genomes.py` & `cazomevolve-0.1.5/cazomevolve/scripts/download_acc_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/get_fam_seqs.py` & `cazomevolve-0.1.5/cazomevolve/scripts/get_fam_seqs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/run_fam_blast.py` & `cazomevolve-0.1.5/cazomevolve/scripts/run_fam_blast.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/run_fam_diamond.py` & `cazomevolve-0.1.5/cazomevolve/scripts/run_fam_diamond.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/ani/build_anim_tree.R` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/build_anim_tree.R`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/ani/run_anim.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/run_anim.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/align_scos.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/align_scos.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/annotate_genomes.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/annotate_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/backtranslate.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/backtranslate.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/concatenate_cds.py` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/concatenate_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/extract_cds.py` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/extract_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/find_orthologues.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/find_orthologues.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh` & `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.5/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.5/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.5/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/taxs/__init__.py` & `cazomevolve-0.1.5/cazomevolve/taxs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/taxs/add_taxs.py` & `cazomevolve-0.1.5/cazomevolve/taxs/add_taxs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from saintBioutils.utilities.logger import config_logger
 from tqdm import tqdm
 
 from cazomevolve.taxs.ncbi import add_ncbi_taxs
 from cazomevolve import closing_message
 
 
-def main(argv: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
+def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     if logger is None:
         config_logger(args)
     logger = logging.getLogger(__name__)
 
     Entrez.email = args.email
 
     if (args.FGP_FILE is None) and (args.FG_FILE is None):
```

### Comparing `cazomevolve-0.1.4/cazomevolve/taxs/ncbi.py` & `cazomevolve-0.1.5/cazomevolve/taxs/ncbi.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/__init__.py` & `cazomevolve-0.1.5/cazomevolve/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/__init__.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/add_taxs_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/add_taxs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/build_cazy_db_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/build_cazy_db_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/common_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/common_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/download_genomes_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/download_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/extract_prot_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/extract_prot_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_cazy_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_cazy_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_dbcan_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/get_fam_seqs_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_fam_seqs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/invoke_dbcan_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/invoke_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/parse_cmd.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/parse_cmd.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/run_blast_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_blast_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve/utilities/parsers/run_diamond_parser.py` & `cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_diamond_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.5/cazomevolve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.4
+Version: 0.1.5
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
```

### Comparing `cazomevolve-0.1.4/cazomevolve.egg-info/SOURCES.txt` & `cazomevolve-0.1.5/cazomevolve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.4/setup.py` & `cazomevolve-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazomevolve",
-    version="0.1.4",
+    version="0.1.5",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A bioinforamtic package for investigating the evolution of CAZomes"
```

