# Comparing `tmp/cazomevolve-0.1.0.tar.gz` & `tmp/cazomevolve-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.1.0.tar", last modified: Wed Jun  7 08:51:12 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.2.tar", last modified: Fri Jul  7 09:42:33 2023, max compression
```

## Comparing `cazomevolve-0.1.0.tar` & `cazomevolve-0.1.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    31182 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    30417 2023-06-07 08:48:37.000000 cazomevolve-0.1.0/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.631525 cazomevolve-0.1.0/cazomevolve/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/build_db.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6916 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4375 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/cazome/explore/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_classes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cooccurring_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/identify_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/ie_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17003 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/pca.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/plot.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/taxonomies.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/genomes/__init__.py
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2382 2023-06-07 08:39:51.000000 cazomevolve-0.1.0/cazomevolve/genomes/download_acc_genomes.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11257 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/scripts/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1713 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/build_cazy_db.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/cazomevolve_script.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3130 2023-06-07 08:41:03.000000 cazomevolve-0.1.0/cazomevolve/scripts/download_acc_genomes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/get_fam_seqs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/run_fam_blast.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/run_fam_diamond.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.631525 cazomevolve-0.1.0/cazomevolve/scripts/tree/
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/build_anim_tree.R
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/run_anim.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/align_scos.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/backtranslate.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/concatenate_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/extract_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/find_orthologues.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/seq_diversity/
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/get_fam_seqs.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/run_blastp.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/taxs/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11563 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/add_taxs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/ncbi.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    31182 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2015 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4127 2023-06-07 08:50:54.000000 cazomevolve-0.1.0/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.169781 cazomevolve-0.1.2/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.2/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    33713 2023-07-07 09:42:33.165781 cazomevolve-0.1.2/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    32948 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.137781 cazomevolve-0.1.2/cazomevolve/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-07-07 09:41:29.000000 cazomevolve-0.1.2/cazomevolve/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.141781 cazomevolve-0.1.2/cazomevolve/cazome/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.2/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.141781 cazomevolve-0.1.2/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.2/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7022 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.145781 cazomevolve-0.1.2/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.2/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4889 2023-07-06 19:20:47.000000 cazomevolve-0.1.2/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.153781 cazomevolve-0.1.2/cazomevolve/cazome/explore/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/identify_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/ie_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17529 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/pca.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/plot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.2/cazomevolve/cazome/explore/taxonomies.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.153781 cazomevolve-0.1.2/cazomevolve/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.2/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11300 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.157781 cazomevolve-0.1.2/cazomevolve/scripts/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.157781 cazomevolve-0.1.2/cazomevolve/scripts/bash/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/scripts/bash/build_cazy_db.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2401 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/scripts/bash/download_acc_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2078 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3135 2023-07-06 15:09:54.000000 cazomevolve-0.1.2/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.133781 cazomevolve-0.1.2/cazomevolve/scripts/tree/
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.157781 cazomevolve-0.1.2/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.161781 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.165781 cazomevolve-0.1.2/cazomevolve/seq_diversity/
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.165781 cazomevolve-0.1.2/cazomevolve/taxs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11563 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.2/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 09:42:33.141781 cazomevolve-0.1.2/cazomevolve.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    33713 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2026 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-07-07 09:42:33.000000 cazomevolve-0.1.2/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-07-07 09:42:33.169781 cazomevolve-0.1.2/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4138 2023-07-07 09:41:21.000000 cazomevolve-0.1.2/setup.py
```

### Comparing `cazomevolve-0.1.0/LICENSE` & `cazomevolve-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/PKG-INFO` & `cazomevolve-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.0
+Version: 0.1.2
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
@@ -20,18 +20,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
-[![Funding](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
-[![PhD licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/PhD_Project_Scripts/blob/master/LICENSE)
+[![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
+[![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
+[![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
+[![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
 
 Use `cazomevolve` to explore:
 
 **CAZome sizes:**
 * Compare the number of CAZymes and CAZy families
@@ -89,14 +91,36 @@
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
 3. [Installation](#installation)
+4. [Requirements](#requirements)
+5. [Explore sequence diversity in CAZy families](#explore-sequence-diversity-in-cazy-families)
+  * [Construct a local CAZyme database](#construct-a-local-cazyme-database)
+  * [Get sequences](#get-protein-sequences)
+  * [Run all-versus-all analysis](#run-all-versus-all-analysis)
+  * [Visualise sequence diversity](#visualise-the-sequence-diversity)
+6. [Annotate the CAZome](#annotate-the-cazome)
+  * [Download genomes](#download-genomes)
+    * [Use genomic accessions](#genomic-accession)
+    * [Using taxonomies](#taxa)
+  * [Annotate](#annotate-cazomes)
+    * [Local CAZyme database](#build-a-local-cazyme-database-using-cazy-webscraper)
+    * [CAZy annotations](#retrieve-cazy-annotations)
+    * [dbCAN annotations](#invoke-dbcan)
+      * [Invoke dbCAN](#invoke-dbcan)
+      * [Get annotations](#retrieve-dbcan-annotations)
+7. [Explore the CAZome](#explore-the-cazome-composition)
+8. [Networks of co-evolving CAZymes](#identify-networkds-of-co-evolving-cazy-families)
+  * [Multi-gene phylogenetic tree reconstruction](#maximum-likelihood-multi-gene-tree)
+  * [ANI distance-based tree](#a-distanced-based-approach)
+  * [Networks of co-evolving CAZymes](#find-networks-of-co-evolving-cazy-families)
+9. [CAZome dendrograms](#build-dendrograms-based-upon-cazome-composition)
 
 ## Installation
 
 ### PyPi
 
 The easiest way to install `cazomeolve` is via PyPi
 
@@ -175,24 +199,24 @@
 * [`Orthofinder`](https://github.com/davidemms/OrthoFinder)
 * [`Prodigal`](https://github.com/hyattpd/Prodigal)
 * [`RaxML-ng`](https://github.com/amkozlov/raxml-ng)
 * [`T-coffee`](https://tcoffee.crg.eu/)
 
 <p>&nbsp;</p>
 
-# Method
+# Explore sequence diversity in CAZy families
 
 ## Construct a local CAZyme database
 
 Download all CAZyme records from CAZy, and compile the records into a local SQLite3 database using `cazy_webscraper`:
 ```bash
 cazy_webscraper <user-email-address> -o <desired-path-for-db>
 ```
 
-## Explore sequence diversity in CAZy families
+## Get protein sequences
 
 Presuming a local CAZyme database has already been generated using `cazy_webscraper`:
 
 1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which takes 4 positional arguments:
 
 * email address
 * path to a local cazyme db
@@ -261,50 +285,71 @@
 
 The genomes to be download can be specified by [A] their genomic accessions, or [B] by specifying a taxa of interest (using a taxa of any level).
 
 ### [A] Genomic accessions
 
 If you have a list of genomic version accessions in a plain text file, `cazomevolve` can use the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
 
-Using the `download_acc_genomes` subcommand, which takes 4 positional arguments and 1 optional argument:
+Using the `download_acc_genomes` subcommand, which takes 5 positional arguments:
 
 **Positional arguments:**
-1. Path to file containing list of accessions (with a unique genome accession per row)
-2. Path to output directory (will be created by `cazevolve_download_acc_genomes`)
-3. File options - a comma-separated list, e.g. "fasta,assembly-report": Choose from: ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
-4. Download Refseq ('refseq') or GenBank ('genbank') assemblies
+* `accessions` - Path to file listing the accessions, with a unique genome accession per row
+* `outdir` - Output directory to write out the genomes to
+* `file_opts`- File options - the file foramts to download the genomic assemblies in. Chose from:
+  * genbank
+  * **fasta**
+  * rm
+  * features 
+  * gff
+  * **protein**
+  * genpept
+  * wgs
+  * cdsfasta
+  * rnafna
+* `database` - NCBI database - the database to retrieve the assemblies from, GenBank or RefSeq: `refseq` or `genbank`
+
+To download the protein sequences of all annotated protein sequences, download the  assembles in `protein` format.  
+
+If you are going to annotate the genomes, download the genomes in `fasta` (genomic sequence) formate.  
 
 **Optional arguments:**
-1. Assembly level. Default 'all'. Comma separated list. Choose from: ['all', 'complete', 'chromosome', 'scaffold', 'contig']
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force`           Force file over writting (default: False)
+* `-n`, `--nodelete`        enable/disable deletion of exisiting files (default: False)
 
-**Downloads the genomes in `.fna` and `faa` format.**
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ### [B] Taxa
 
 To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the subcommand `download_genomes`, which takes 4 arguments:
 
-1. User email address (required by NCBI)
-2. The terms of interest. Comma-separated list, e.g. 'Pectobacterium,Dickeya'
-3. The file formats to download the genomic assemblies in. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]"
-4. Path to an output directory (this will be built by `cazomevolve`).
-
-By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
-
-**Optional flags:**
-
-``--assembly_levels``, ``-A`` - Restrict the dataset to genomic assemblies of a specific assembly level(s). Space separated list, e.g. 'complete chromosome'. Choices: ['all', 'complete', 'chromosome', 'scaffold', 'contig']. Default 'all'.
+**Positional arguments:**
+* email - User email address
+* output_dir - Path to directory to write out genomic assemblies
+* terms - Terms to search NCBI. Comma-separated listed, e.g, 'Pectobacterium,Dickeya'. To include spaces in terms, encapsulate the all terms in quotation marks, e.g. 'Pectobacterium wasabiae'
+* file format: {genomic,protein}- Space-separated list of file formats to dowload. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]
+* NCBI database: {genbank,refseq} - Choose which NCBI db to get genomes from: refseq or genbank
 
-``--genbank``, ``-G`` - Retrieve GenBank not RefSeq data. By default ``cazomevolve`` downloads RefSeq assemblies. Add this flag to the command to download GenBank assemblies instead.
+**Optional arguments:**
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force` - Force file over writting (default: False)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-l`, `--log` - path to write out log file
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+* `--timeout` - time in seconds before connection times out (default: 30)
 
-``-f``, ``--force`` - Force file over writting (default: False)
-``-l - log file name, --log log file name
-                        Defines log file name and/or path (default: None)
-``-n``, ``--nodelete`` - enable/disable deletion of exisiting files (default: False)
-``--timeout`` TIMEOUT - time in seconds before connection times out (default: 30)
-``-v``, ``--verbose`` - Set logger level to 'INFO' (default: False)
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ## Annotate CAZomes
 
 To retrieve the most comprehensive annotation of the CAZome, we recommend using the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
 
 > Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard; cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets, BioRxiv, 3 December 2022, https://doi.org/10.1101/2022.12.02.518825
 
@@ -314,20 +359,21 @@
 
 To include 'canonical' CAZy family classifications from CAZy, download all data from the CAZy database and compile the data into a local CAZyme database using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al., 2022).
 
 > cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets
 Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard
 bioRxiv 2022.12.02.518825; doi: https://doi.org/10.1101/2022.12.02.518825
 
-The `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
+Use the `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
 ```bash
 cazomevolve build_cazy_db \
   <email> \
-  <desired db path>
+  <desired path for db FILE>
 ```
+Note the path needs to point to the target FILE path not DIR path. `cazy_webscraper` will build all necessary parent directories.
 
 Or you can use `cazy_webscraper` directly
 ```bash
 cazy_webscraper \
     <email> \
     -o <db file output path>
 ```
@@ -378,26 +424,29 @@
 _`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM._
 
 `dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using the `cazomveolve`, subcommand `run_dbcan` command.
 
 ```bash
 cazomevolve run_dbcan \
     <path to dir containing FASTA files> \
-    <path to output directory> 
+    <path to output directory> \
+    <dbcan major version number, 2, 3 or 4>
 ```
 
+``cazomevolve`` will which ever version of dbCAN is installed, but the commands and arguments between dbCAN version 2, 3 and 4 are different, so ``cazomevolve`` must be told which version to of dbCAN to communicate with.
+
 The ouput directory will be created by `run_dbcan`. 
 
 Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
 
 Optional args:
 ```bash
 options:
   -h, --help            show this help message and exit
-  -V2--version_2        Use dbCAN version 2 NOT 3/4 (default: False)
+  --cpu CPU             Number of CPU cores to use. Default all available cores (default: all avilable cores)
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
@@ -433,17 +482,15 @@
 ```bash
 options:
   -h, --help            show this help message and exit
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
-  --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
-  -v2, --version_2      Parse the data from dbCAN version 2 (default: False, parse data from dbCAN version 3)
 ```
 
 # Explore the CAZome composition
 
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
```

### Comparing `cazomevolve-0.1.0/README.md` & `cazomevolve-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
-[![Funding](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
-[![PhD licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/PhD_Project_Scripts/blob/master/LICENSE)
+[![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
+[![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
+[![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
+[![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
 
 Use `cazomevolve` to explore:
 
 **CAZome sizes:**
 * Compare the number of CAZymes and CAZy families
@@ -67,14 +69,36 @@
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
 3. [Installation](#installation)
+4. [Requirements](#requirements)
+5. [Explore sequence diversity in CAZy families](#explore-sequence-diversity-in-cazy-families)
+  * [Construct a local CAZyme database](#construct-a-local-cazyme-database)
+  * [Get sequences](#get-protein-sequences)
+  * [Run all-versus-all analysis](#run-all-versus-all-analysis)
+  * [Visualise sequence diversity](#visualise-the-sequence-diversity)
+6. [Annotate the CAZome](#annotate-the-cazome)
+  * [Download genomes](#download-genomes)
+    * [Use genomic accessions](#genomic-accession)
+    * [Using taxonomies](#taxa)
+  * [Annotate](#annotate-cazomes)
+    * [Local CAZyme database](#build-a-local-cazyme-database-using-cazy-webscraper)
+    * [CAZy annotations](#retrieve-cazy-annotations)
+    * [dbCAN annotations](#invoke-dbcan)
+      * [Invoke dbCAN](#invoke-dbcan)
+      * [Get annotations](#retrieve-dbcan-annotations)
+7. [Explore the CAZome](#explore-the-cazome-composition)
+8. [Networks of co-evolving CAZymes](#identify-networkds-of-co-evolving-cazy-families)
+  * [Multi-gene phylogenetic tree reconstruction](#maximum-likelihood-multi-gene-tree)
+  * [ANI distance-based tree](#a-distanced-based-approach)
+  * [Networks of co-evolving CAZymes](#find-networks-of-co-evolving-cazy-families)
+9. [CAZome dendrograms](#build-dendrograms-based-upon-cazome-composition)
 
 ## Installation
 
 ### PyPi
 
 The easiest way to install `cazomeolve` is via PyPi
 
@@ -153,24 +177,24 @@
 * [`Orthofinder`](https://github.com/davidemms/OrthoFinder)
 * [`Prodigal`](https://github.com/hyattpd/Prodigal)
 * [`RaxML-ng`](https://github.com/amkozlov/raxml-ng)
 * [`T-coffee`](https://tcoffee.crg.eu/)
 
 <p>&nbsp;</p>
 
-# Method
+# Explore sequence diversity in CAZy families
 
 ## Construct a local CAZyme database
 
 Download all CAZyme records from CAZy, and compile the records into a local SQLite3 database using `cazy_webscraper`:
 ```bash
 cazy_webscraper <user-email-address> -o <desired-path-for-db>
 ```
 
-## Explore sequence diversity in CAZy families
+## Get protein sequences
 
 Presuming a local CAZyme database has already been generated using `cazy_webscraper`:
 
 1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which takes 4 positional arguments:
 
 * email address
 * path to a local cazyme db
@@ -239,50 +263,71 @@
 
 The genomes to be download can be specified by [A] their genomic accessions, or [B] by specifying a taxa of interest (using a taxa of any level).
 
 ### [A] Genomic accessions
 
 If you have a list of genomic version accessions in a plain text file, `cazomevolve` can use the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
 
-Using the `download_acc_genomes` subcommand, which takes 4 positional arguments and 1 optional argument:
+Using the `download_acc_genomes` subcommand, which takes 5 positional arguments:
 
 **Positional arguments:**
-1. Path to file containing list of accessions (with a unique genome accession per row)
-2. Path to output directory (will be created by `cazevolve_download_acc_genomes`)
-3. File options - a comma-separated list, e.g. "fasta,assembly-report": Choose from: ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
-4. Download Refseq ('refseq') or GenBank ('genbank') assemblies
+* `accessions` - Path to file listing the accessions, with a unique genome accession per row
+* `outdir` - Output directory to write out the genomes to
+* `file_opts`- File options - the file foramts to download the genomic assemblies in. Chose from:
+  * genbank
+  * **fasta**
+  * rm
+  * features 
+  * gff
+  * **protein**
+  * genpept
+  * wgs
+  * cdsfasta
+  * rnafna
+* `database` - NCBI database - the database to retrieve the assemblies from, GenBank or RefSeq: `refseq` or `genbank`
+
+To download the protein sequences of all annotated protein sequences, download the  assembles in `protein` format.  
+
+If you are going to annotate the genomes, download the genomes in `fasta` (genomic sequence) formate.  
 
 **Optional arguments:**
-1. Assembly level. Default 'all'. Comma separated list. Choose from: ['all', 'complete', 'chromosome', 'scaffold', 'contig']
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force`           Force file over writting (default: False)
+* `-n`, `--nodelete`        enable/disable deletion of exisiting files (default: False)
 
-**Downloads the genomes in `.fna` and `faa` format.**
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ### [B] Taxa
 
 To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the subcommand `download_genomes`, which takes 4 arguments:
 
-1. User email address (required by NCBI)
-2. The terms of interest. Comma-separated list, e.g. 'Pectobacterium,Dickeya'
-3. The file formats to download the genomic assemblies in. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]"
-4. Path to an output directory (this will be built by `cazomevolve`).
-
-By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
-
-**Optional flags:**
-
-``--assembly_levels``, ``-A`` - Restrict the dataset to genomic assemblies of a specific assembly level(s). Space separated list, e.g. 'complete chromosome'. Choices: ['all', 'complete', 'chromosome', 'scaffold', 'contig']. Default 'all'.
+**Positional arguments:**
+* email - User email address
+* output_dir - Path to directory to write out genomic assemblies
+* terms - Terms to search NCBI. Comma-separated listed, e.g, 'Pectobacterium,Dickeya'. To include spaces in terms, encapsulate the all terms in quotation marks, e.g. 'Pectobacterium wasabiae'
+* file format: {genomic,protein}- Space-separated list of file formats to dowload. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]
+* NCBI database: {genbank,refseq} - Choose which NCBI db to get genomes from: refseq or genbank
 
-``--genbank``, ``-G`` - Retrieve GenBank not RefSeq data. By default ``cazomevolve`` downloads RefSeq assemblies. Add this flag to the command to download GenBank assemblies instead.
+**Optional arguments:**
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force` - Force file over writting (default: False)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-l`, `--log` - path to write out log file
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+* `--timeout` - time in seconds before connection times out (default: 30)
 
-``-f``, ``--force`` - Force file over writting (default: False)
-``-l - log file name, --log log file name
-                        Defines log file name and/or path (default: None)
-``-n``, ``--nodelete`` - enable/disable deletion of exisiting files (default: False)
-``--timeout`` TIMEOUT - time in seconds before connection times out (default: 30)
-``-v``, ``--verbose`` - Set logger level to 'INFO' (default: False)
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ## Annotate CAZomes
 
 To retrieve the most comprehensive annotation of the CAZome, we recommend using the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
 
 > Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard; cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets, BioRxiv, 3 December 2022, https://doi.org/10.1101/2022.12.02.518825
 
@@ -292,20 +337,21 @@
 
 To include 'canonical' CAZy family classifications from CAZy, download all data from the CAZy database and compile the data into a local CAZyme database using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al., 2022).
 
 > cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets
 Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard
 bioRxiv 2022.12.02.518825; doi: https://doi.org/10.1101/2022.12.02.518825
 
-The `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
+Use the `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
 ```bash
 cazomevolve build_cazy_db \
   <email> \
-  <desired db path>
+  <desired path for db FILE>
 ```
+Note the path needs to point to the target FILE path not DIR path. `cazy_webscraper` will build all necessary parent directories.
 
 Or you can use `cazy_webscraper` directly
 ```bash
 cazy_webscraper \
     <email> \
     -o <db file output path>
 ```
@@ -356,26 +402,29 @@
 _`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM._
 
 `dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using the `cazomveolve`, subcommand `run_dbcan` command.
 
 ```bash
 cazomevolve run_dbcan \
     <path to dir containing FASTA files> \
-    <path to output directory> 
+    <path to output directory> \
+    <dbcan major version number, 2, 3 or 4>
 ```
 
+``cazomevolve`` will which ever version of dbCAN is installed, but the commands and arguments between dbCAN version 2, 3 and 4 are different, so ``cazomevolve`` must be told which version to of dbCAN to communicate with.
+
 The ouput directory will be created by `run_dbcan`. 
 
 Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
 
 Optional args:
 ```bash
 options:
   -h, --help            show this help message and exit
-  -V2--version_2        Use dbCAN version 2 NOT 3/4 (default: False)
+  --cpu CPU             Number of CPU cores to use. Default all available cores (default: all avilable cores)
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
@@ -411,17 +460,15 @@
 ```bash
 options:
   -h, --help            show this help message and exit
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
-  --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
-  -v2, --version_2      Parse the data from dbCAN version 2 (default: False, parse data from dbCAN version 3)
 ```
 
 # Explore the CAZome composition
 
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
```

### Comparing `cazomevolve-0.1.0/cazomevolve/__init__.py` & `cazomevolve-0.1.2/cazomevolve/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 
 __citation__ = "???"
 
 
 def closing_message(job, args):
     """Write closing messsage to terminal
```

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.2/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.2/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/cazy/build_db.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/bash/build_cazy_db.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.2/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
     if str(args.fam_genome_protein_list.parent) != ".":
         if str(args.fam_genome_list.parent) == str(args.fam_genome_protein_list.parent):
             make_output_directory(args.fam_genome_protein_list.parent, True, True)
         else:
             make_output_directory(args.fam_genome_protein_list.parent, args.force, args.nodelete)
 
+    logger = logging.getLogger(__name__)
+
     # connect to the local CAZyme db
     connection = get_db_connection(args.database, args.sql_echo, False)
 
     # retrieve path to protein FASTA files
     fasta_files_paths = get_file_paths(args.input_dir, suffixes=['.fasta', '.faa'])
 
     if len(fasta_files_paths) == 0:
@@ -158,15 +160,15 @@
             with Session(bind=connection) as session:
                 fam_query = session.query(Genbank, CazyFamily).\
                     join(CazyFamily, Genbank.families).\
                     filter(Genbank.genbank_accession == prot_acc).\
                     all()
 
                 for result in fam_query:
-                    fam = result[1].family
+                    fam = result[1].family.split("_")[0]  # make sure to remove subfamily classification
                     fam_genome_data += f"{fam}\t{genomic_accession}\n"
                     fam_genome_protein_data += f"{fam}\t{genomic_accession}\t{prot_acc}\n"
 
         # write out data
         with open(args.fam_genome_list, "a") as fh:
             fh.write(fam_genome_data)
```

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.2/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.2/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.2/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files 24% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             try:
                 genomic_accession = re.findall(r"GCA_\d+\.\d{1,5}", fasta_path.name)[0]
             except IndexError:
                 logger.warning(
                     f"Could not retrieve genomic accession from\n{fasta_path}\n"
                     "Skipping FASTA file"
                 )
-                return
+                continue
         
         output_dir = args.output_dir / genomic_accession
 
         if output_dir.exists():
             print(f"Already parsed {genomic_accession}\nSKIIIP")
             continue
 
@@ -95,42 +95,60 @@
     :param args: cmd-line args parser
 
     Return nothing
     """
     # make the output directory
     make_output_directory(out_dir, True, False)
 
-    if args.version_2:
+    if args.dbcan_version == 2:
         # create list of args to invoke run_dbCAN
         dbcan_args = [
             "run_dbcan.py",
             str(input_path),
             "protein",
             "--out_dir",
             str(out_dir),
         ]
 
-    else:
+    elif args.dbcan_version == 3:
         # create list of args to invoke run_dbCAN
         dbcan_args = [
             "run_dbcan",
             str(input_path),
             "protein",
             "--out_dir",
             str(out_dir),
             "--stp_cpu",
-            "8",
+            str(args.cpu),
             "--tf_cpu",
-            "8",
+            str(args.cpu),
             "--eCAMI_jobs",
-            "8",
+            str(args.cpu),
+            "--hmm_cpu",
+            str(args.cpu),
+            "--dia_cpu",
+            str(args.cpu),
+        ]
+
+    else:
+        # create list of args to invoke run_dbCAN
+        dbcan_args = [
+            "run_dbcan",
+            str(input_path),
+            "protein",
+            "--out_dir",
+            str(out_dir),
+            "--stp_cpu",
+            str(args.cpu),
+            "--tf_cpu",
+            str(args.cpu),
             "--hmm_cpu",
-            "8",
+            str(args.cpu),
             "--dia_cpu",
-            "8",
+            str(args.cpu),
         ]
 
     with open(f"{out_dir}/dbcan.log", "w+") as fh:
         process = subprocess.run(dbcan_args, text=True, capture_output=True)
 
     return
```

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/cazome_sizes.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/cazome_sizes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_classes.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/cazy_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_families.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/cazy_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/cooccurring_families.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/cooccurring_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/identify_families.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/identify_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/ie_cazymes.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/ie_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/parse_data.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/parse_data.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/pca.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
     figsize=None, 
     xlim=None,
     ylim=None,
     dpi=300,
     loc='upper left',
     marker_size=100,
     markers=True,
+    ax=None,
 ):
     """Project genomes onto the PCs
     
     :param pca: sklearn PCA object
     :param X_scaled: obj from scaling data
     :param fam_df: df of cazy family freqs
     :param first_pc: int, number of the first PC
@@ -185,14 +186,15 @@
     :param xlim: tuple, limits of the x axis
     :param ylim: tuple, limits of the y axis
     :param dpi: int, dpi to write out figure
     :param loc: str, location of key
     :param marker_size: int, scale of markers
     :param markers: dict, pass dict to map each level style to a marker 
         defined in matplotlib
+    :param ax: axis - used to combining multiple scatter plots into a multiplot
     
     Return plot
     """
     grouping = f"{group_by[0].upper()}{group_by[1:]}"
     X_pca = pca.transform(X_scaled)
     
     if figsize is not None:
@@ -216,41 +218,44 @@
                     data=fam_df,
                     hue=group_by,
                     s=marker_size,
                     hue_order=hue_order,
                     style=style,
                     style_order=style_order,
                     markers=markers,
+                    ax=ax,
                 )
                 
             else:
                 print('Not applying style order')
                 # use default style order
                 g = sns.scatterplot(
                     x=X_pca[:,first_pc-1],
                     y=X_pca[:, second_pc-1],
                     data=fam_df,
                     hue=group_by,
                     s=marker_size,
                     hue_order=hue_order,
                     style=style,
                     markers=markers,
+                    ax=ax,
                 )                
             
         else:
             print('Not applying style')
             # hue order only
             g = sns.scatterplot(
                 x=X_pca[:,first_pc-1],
                 y=X_pca[:, second_pc-1],
                 data=fam_df,
                 hue=group_by,
                 s=marker_size,
                 hue_order=hue_order,
                 markers=markers,
+                ax=ax,
             )  
         
     else:  # using default hue order - i.e. order data is presented in df
         print('Not applying hue order')
         
         if style is not None:  # use different markers for catagroies in provided col
             print('Applying style')
@@ -263,40 +268,43 @@
                     y=X_pca[:, second_pc-1],
                     data=fam_df,
                     hue=group_by,
                     s=marker_size,
                     style=style,
                     style_order=style_order,
                     markers=markers,
+                    ax=ax,
                 )
                 
             else:
                 print('Not applying style order')
                 # use default style order
                 g = sns.scatterplot(
                     x=X_pca[:,first_pc-1],
                     y=X_pca[:, second_pc-1],
                     data=fam_df,
                     hue=group_by,
                     s=marker_size,
                     style=style,
                     markers=markers,
+                    ax=ax,
                 )
         
         else:
             print('Not Applying style')
             # no options specified
             # do not apply style
             g = sns.scatterplot(
                 x=X_pca[:,first_pc-1],
                 y=X_pca[:, second_pc-1],
                 data=fam_df,
                 hue=group_by,
                 s=marker_size,
                 markers=markers,
+                ax=ax,
             )
     
     if xlim is not None:
         g.set(xlim=xlim);
     if ylim is not None:
         g.set(ylim=ylim);
     
@@ -328,14 +336,15 @@
     threshold=0.7,
     font_scale=1.15,
     font_size=12,
     dpi=300,
     fig_size=(16,16),
     file_path=None,
     marker_size=100,
+    ax=None,
 ):
     """Build loadings plot
     
     :param pca: sklearn pca object
     :param fam_df: cazy family frequncy df
     :param first_pc: int, number of the first PC, e.g. PC1 == 1
     :param second_pc: int, number of the second PC e.g. PC2 == 2
@@ -344,14 +353,15 @@
         Only families with a value greater than the threshold
         will be annotated
     :param font_scale: scale font
     :param font_size: font size of family labels
     :param fig_size: tuple (width, height) of final plot
     :param file_path: str, path to write out a figure.
         If None, no figure is saved
+    :param ax: axis, used to define axis in multiple plot to place figure
     
     Return nothing"""
     sns.set(font_scale=font_scale)
 
     # calculate loading = variables x loadings, returns an array
     loadings = pca.components_.T * np.sqrt(pca.explained_variance_)
     # get labels of variables, i.e. cazy families
@@ -387,17 +397,32 @@
         else:
             cazy_class.append('CBM')
 
     loadings_df['cazy_class'] = cazy_class
 
     plt.figure(figsize=fig_size)
     if style:
-        g = sns.scatterplot(x=loadings_x, y=loadings_y, data=loadings_df, hue=cazy_class, s=marker_size, style=cazy_class);
+        g = sns.scatterplot(
+            x=loadings_x,
+            y=loadings_y,
+            data=loadings_df,
+            hue=cazy_class,
+            s=marker_size,
+            style=cazy_class,
+            ax=ax,
+        );
     else:
-        g = sns.scatterplot(x=loadings_x, y=loadings_y, data=loadings_df, hue=cazy_class, s=marker_size);
+        g = sns.scatterplot(
+            x=loadings_x,
+            y=loadings_y,
+            data=loadings_df,
+            hue=cazy_class,
+            s=marker_size,
+            ax=ax,
+        );
     g.axhline(0, linestyle='--', color='grey', linewidth=1.25);
     g.axvline(0, linestyle='--', color='grey', linewidth=1.25);
     g.set(xlim=(-1,1),ylim=(-1,1));
     plt.ylabel(f"PC{second_pc}") 
     plt.xlabel(f"PC{first_pc}")
 
     texts = [
```

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/plot.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/plot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/cazome/explore/taxonomies.py` & `cazomevolve-0.1.2/cazomevolve/cazome/explore/taxonomies.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.2/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/genomes/download_acc_genomes.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/bash/download_acc_genomes.sh`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # $2 output directory to write out the genomes to
 # $3 file options - A comma-separated list of formats is also possible. For example: "fasta,assembly-report". Choose from:
 # ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
 # $4 refseq or genbank
 # $5 assembly level, default all, ['all', 'complete', 'chromosome', 'scaffold', 'contig']
 
 echo "Running ncbi-genome-download"
-echo "Citation: Blin et al. (2017) ncbi-genome-download, Follow link (ctrl + click)"
+echo "Citation: Blin et al. (2017) ncbi-genome-download, https://github.com/kblin/ncbi-genome-download"
 
 ncbi-genome-download \
     all \
     --section $4 \
     --formats $3 \
     --assembly-levels $5 \
     --assembly-accessions $1 \
```

### Comparing `cazomevolve-0.1.0/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.2/cazomevolve/genomes/download_genomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 """Retrieve all genomic assembly accessions descendent from a taxonomy node"""
 
 
 import logging
 import re
 import time
 
+from pathlib import Path
 from typing import List, Optional
 
 from socket import timeout
 from Bio import Entrez
 from saintBioutils.utilities.file_io import make_output_directory
 from tqdm import tqdm
 from urllib.request import urlopen
@@ -173,15 +174,15 @@
             existing_v = existing_accession[(existing_accession.find(".")) + 1 : ]
 
             if accession_v > existing_v:
                 accession_data = accession_data.pop(existing_v)
                 accession_data[accession_number_v] = batch_result['DocumentSummarySet']['DocumentSummary'][index]['AssemblyName']
 
     for accession in tqdm(accession_data, desc=f"Downloading genomes for {term}"):
-        for file_type in ((args.file_types).split(",")):
+        for file_type in args.file_types:
             download_file(
                 accession_number=accession,
                 assembly_name=accession_data[accession],
                 file_type=file_type,
                 args=args,
             )
     return
@@ -221,28 +222,28 @@
         )
         return
 
     return record
 
 
 def download_file(
-    accession_number, assembly_name, file_type, args, url_prefix="ftp://ftp.ncbi.nlm.nih.gov/genomes/all"
+    accession_number, assembly_name, file_type, args, url_prefix="https://ftp.ncbi.nlm.nih.gov/genomes/all"
 ):
     """Download file.
 
     :param accession_number: str, accession number of genome
     :param assembly_name: str, name of assembly
     :param file_type: str, denotes in logger file type downloaded [accepted = 'protein.faa', 'genomic.fna']
     param args: parser arguments
 
     Return nothing.
     """
     logger = logging.getLogger(__name__)
 
-    if args.genbank:   # retrieve GenBank not RefSeq
+    if args.database == 'genbank':   # retrieve GenBank not RefSeq
         gbk_accession = accession_number.replace("GCF_", "GCA_")
     else:  # retrieve RefSeq not GenBank
         gbk_accession = accession_number.replace("GCA_", "GCF_")
 
     file_name = f"{gbk_accession}_{assembly_name}.{file_type}"
     file_name = file_name.replace(" ","_")
     output_path = args.output_dir / file_name
@@ -250,15 +251,15 @@
 
     if output_path.exists():
         logger.warning(f"Output file {output_path} exists, not downloading")
         return
     if unzipped_path.exists():
         logger.warning(f"Output file {unzipped_path} exists, not downloading")
         return
-    
+
     escape_characters = re.compile(r"[\s/,#\(\)]")
     escape_name = re.sub(escape_characters, "_", assembly_name)
 
     filestem = "_".join([gbk_accession, escape_name])
 
     url_parts = tuple(filestem.split("_", 2))
     # separate identifying numbers from version number, and split up into groups of 3 digits
@@ -269,15 +270,15 @@
     genbank_url = f"{url_prefix}/{url_parts[0]}/{sub_directories}/{filestem}/{filestem}_{file_type}.gz"
 
     # try URL connection
     try:
         response = urlopen(genbank_url, timeout=args.timeout)
     except (HTTPError, URLError, timeout) as e:
         logger.error(
-            f"Failed to download {file_type} for {accession_number}", exc_info=1,
+            f"Failed to download {file_type} for {accession_number}\nURL: {genbank_url}", exc_info=1,
         )
         return
     file_size = int(response.info().get("Content-length"))
     bsize = 1_048_576
     try:
         with open(output_path, "wb") as out_handle:
             # Using leave=False as this will be an internally-nested progress bar
```

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/__init__.py` & `cazomevolve-0.1.2/cazomevolve/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/build_cazy_db.py` & `cazomevolve-0.1.2/cazomevolve/taxs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# (c) University of St Andrews 2020-2021
-# (c) University of Strathclyde 2020-2021
+# (c) University of St Andrews 2022
+# (c) University of Strathclyde 2022
+# (c) James Hutton Institute 2022
 # Author:
 # Emma E. M. Hobbs
 
 # Contact
 # eemh1@st-andrews.ac.uk
 
 # Emma E. M. Hobbs,
@@ -32,22 +33,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Retrieving protein seqs for fams of interest"""
-
-
-import argparse
-import subprocess
-
-def main(args: argparse.Namespace) -> int:
-    theproc = subprocess.Popen([
-        "./cazome/cazy/build_db.sh",
-        args.email,
-        args.db,
-    ], shell=True)
-    theproc.communicate()
-
-    return 0
+"""Module for adding taxonomic classifications to tab delimited lists"""
```

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/cazomevolve_script.py` & `cazomevolve-0.1.2/cazomevolve/scripts/cazomevolve_script.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/download_acc_genomes.py` & `cazomevolve-0.1.2/cazomevolve/scripts/download_acc_genomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 # $5 assembly level, default all, ['all', 'complete', 'chromosome', 'scaffold', 'contig']
 
 
 def main(args: argparse.Namespace) -> int:
     if str(Path(args.outdir).parent) != ".":
         make_output_directory(Path(args.outdir), args.force, args.nodelete)
 
-    cazevolve_path = abspath(getsourcefile(lambda:0).replace("scripts/download_acc_genomes.py","genomes/download_acc_genomes.sh"))
+    cazevolve_path = abspath(getsourcefile(lambda:0).replace("scripts/download_acc_genomes.py","scripts/bash/download_acc_genomes.sh"))
 
     cmd = [
             cazevolve_path,
             args.accessions,
             args.outdir,
             args.file_opts,
             args.database,
```

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/get_fam_seqs.py` & `cazomevolve-0.1.2/cazomevolve/scripts/get_fam_seqs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/run_fam_blast.py` & `cazomevolve-0.1.2/cazomevolve/scripts/run_fam_blast.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/run_fam_diamond.py` & `cazomevolve-0.1.2/cazomevolve/scripts/run_fam_diamond.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/build_anim_tree.R` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/ani/build_anim_tree.R`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/run_anim.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/ani/run_anim.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/align_scos.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/align_scos.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/annotate_genomes.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/annotate_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/backtranslate.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/backtranslate.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/concatenate_cds.py` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/concatenate_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/extract_cds.py` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/extract_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/find_orthologues.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/find_orthologues.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh` & `cazomevolve-0.1.2/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.2/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.2/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.2/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/taxs/__init__.py` & `cazomevolve-0.1.2/cazomevolve/scripts/build_cazy_db.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# (c) University of St Andrews 2022
-# (c) University of Strathclyde 2022
-# (c) James Hutton Institute 2022
+# (c) University of St Andrews 2020-2021
+# (c) University of Strathclyde 2020-2021
 # Author:
 # Emma E. M. Hobbs
 
 # Contact
 # eemh1@st-andrews.ac.uk
 
 # Emma E. M. Hobbs,
@@ -33,8 +32,41 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Module for adding taxonomic classifications to tab delimited lists"""
+"""Retrieving protein seqs for fams of interest"""
+
+
+import argparse
+import sys
+import subprocess
+import os
+
+from inspect import getsourcefile
+from os.path import abspath
+from pathlib import Path
+
+
+def main(args: argparse.Namespace) -> int:
+
+    cazevolve_path = abspath(getsourcefile(lambda:0).replace("scripts/build_cazy_db.py","scripts/bash/build_cazy_db.sh"))
+
+    cmd = [
+        cazevolve_path,
+        args.email,
+        args.db,
+        ]
+    txt = ' '.join(["build_db.sh"]+cmd[1:])
+
+    print(f"Running command: {txt}")
+
+    theproc = subprocess.Popen([
+        "bash",
+        cazevolve_path,
+        args.email,
+        args.db,
+    ])
+
+    return 0
```

### Comparing `cazomevolve-0.1.0/cazomevolve/taxs/add_taxs.py` & `cazomevolve-0.1.2/cazomevolve/taxs/add_taxs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve/taxs/ncbi.py` & `cazomevolve-0.1.2/cazomevolve/taxs/ncbi.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.0/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.2/cazomevolve.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.0
+Version: 0.1.2
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
@@ -20,18 +20,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
-[![Funding](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
-[![PhD licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/PhD_Project_Scripts/blob/master/LICENSE)
+[![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
+[![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
+[![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
+[![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
 
 Use `cazomevolve` to explore:
 
 **CAZome sizes:**
 * Compare the number of CAZymes and CAZy families
@@ -89,14 +91,36 @@
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
 3. [Installation](#installation)
+4. [Requirements](#requirements)
+5. [Explore sequence diversity in CAZy families](#explore-sequence-diversity-in-cazy-families)
+  * [Construct a local CAZyme database](#construct-a-local-cazyme-database)
+  * [Get sequences](#get-protein-sequences)
+  * [Run all-versus-all analysis](#run-all-versus-all-analysis)
+  * [Visualise sequence diversity](#visualise-the-sequence-diversity)
+6. [Annotate the CAZome](#annotate-the-cazome)
+  * [Download genomes](#download-genomes)
+    * [Use genomic accessions](#genomic-accession)
+    * [Using taxonomies](#taxa)
+  * [Annotate](#annotate-cazomes)
+    * [Local CAZyme database](#build-a-local-cazyme-database-using-cazy-webscraper)
+    * [CAZy annotations](#retrieve-cazy-annotations)
+    * [dbCAN annotations](#invoke-dbcan)
+      * [Invoke dbCAN](#invoke-dbcan)
+      * [Get annotations](#retrieve-dbcan-annotations)
+7. [Explore the CAZome](#explore-the-cazome-composition)
+8. [Networks of co-evolving CAZymes](#identify-networkds-of-co-evolving-cazy-families)
+  * [Multi-gene phylogenetic tree reconstruction](#maximum-likelihood-multi-gene-tree)
+  * [ANI distance-based tree](#a-distanced-based-approach)
+  * [Networks of co-evolving CAZymes](#find-networks-of-co-evolving-cazy-families)
+9. [CAZome dendrograms](#build-dendrograms-based-upon-cazome-composition)
 
 ## Installation
 
 ### PyPi
 
 The easiest way to install `cazomeolve` is via PyPi
 
@@ -175,24 +199,24 @@
 * [`Orthofinder`](https://github.com/davidemms/OrthoFinder)
 * [`Prodigal`](https://github.com/hyattpd/Prodigal)
 * [`RaxML-ng`](https://github.com/amkozlov/raxml-ng)
 * [`T-coffee`](https://tcoffee.crg.eu/)
 
 <p>&nbsp;</p>
 
-# Method
+# Explore sequence diversity in CAZy families
 
 ## Construct a local CAZyme database
 
 Download all CAZyme records from CAZy, and compile the records into a local SQLite3 database using `cazy_webscraper`:
 ```bash
 cazy_webscraper <user-email-address> -o <desired-path-for-db>
 ```
 
-## Explore sequence diversity in CAZy families
+## Get protein sequences
 
 Presuming a local CAZyme database has already been generated using `cazy_webscraper`:
 
 1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which takes 4 positional arguments:
 
 * email address
 * path to a local cazyme db
@@ -261,50 +285,71 @@
 
 The genomes to be download can be specified by [A] their genomic accessions, or [B] by specifying a taxa of interest (using a taxa of any level).
 
 ### [A] Genomic accessions
 
 If you have a list of genomic version accessions in a plain text file, `cazomevolve` can use the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
 
-Using the `download_acc_genomes` subcommand, which takes 4 positional arguments and 1 optional argument:
+Using the `download_acc_genomes` subcommand, which takes 5 positional arguments:
 
 **Positional arguments:**
-1. Path to file containing list of accessions (with a unique genome accession per row)
-2. Path to output directory (will be created by `cazevolve_download_acc_genomes`)
-3. File options - a comma-separated list, e.g. "fasta,assembly-report": Choose from: ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
-4. Download Refseq ('refseq') or GenBank ('genbank') assemblies
+* `accessions` - Path to file listing the accessions, with a unique genome accession per row
+* `outdir` - Output directory to write out the genomes to
+* `file_opts`- File options - the file foramts to download the genomic assemblies in. Chose from:
+  * genbank
+  * **fasta**
+  * rm
+  * features 
+  * gff
+  * **protein**
+  * genpept
+  * wgs
+  * cdsfasta
+  * rnafna
+* `database` - NCBI database - the database to retrieve the assemblies from, GenBank or RefSeq: `refseq` or `genbank`
+
+To download the protein sequences of all annotated protein sequences, download the  assembles in `protein` format.  
+
+If you are going to annotate the genomes, download the genomes in `fasta` (genomic sequence) formate.  
 
 **Optional arguments:**
-1. Assembly level. Default 'all'. Comma separated list. Choose from: ['all', 'complete', 'chromosome', 'scaffold', 'contig']
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force`           Force file over writting (default: False)
+* `-n`, `--nodelete`        enable/disable deletion of exisiting files (default: False)
 
-**Downloads the genomes in `.fna` and `faa` format.**
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ### [B] Taxa
 
 To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the subcommand `download_genomes`, which takes 4 arguments:
 
-1. User email address (required by NCBI)
-2. The terms of interest. Comma-separated list, e.g. 'Pectobacterium,Dickeya'
-3. The file formats to download the genomic assemblies in. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]"
-4. Path to an output directory (this will be built by `cazomevolve`).
-
-By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
-
-**Optional flags:**
-
-``--assembly_levels``, ``-A`` - Restrict the dataset to genomic assemblies of a specific assembly level(s). Space separated list, e.g. 'complete chromosome'. Choices: ['all', 'complete', 'chromosome', 'scaffold', 'contig']. Default 'all'.
+**Positional arguments:**
+* email - User email address
+* output_dir - Path to directory to write out genomic assemblies
+* terms - Terms to search NCBI. Comma-separated listed, e.g, 'Pectobacterium,Dickeya'. To include spaces in terms, encapsulate the all terms in quotation marks, e.g. 'Pectobacterium wasabiae'
+* file format: {genomic,protein}- Space-separated list of file formats to dowload. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]
+* NCBI database: {genbank,refseq} - Choose which NCBI db to get genomes from: refseq or genbank
 
-``--genbank``, ``-G`` - Retrieve GenBank not RefSeq data. By default ``cazomevolve`` downloads RefSeq assemblies. Add this flag to the command to download GenBank assemblies instead.
+**Optional arguments:**
+* `-A`, `--assembly_levels` - limit the download to assemblies with the assembly status provided. A space-separate lists of assembly levels. Can provide multiple levels: Accepted levels:
+  * complete
+  * chromosome
+  * scaffold
+  * contig 
+* `-f`, `--force` - Force file over writting (default: False)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-l`, `--log` - path to write out log file
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+* `--timeout` - time in seconds before connection times out (default: 30)
 
-``-f``, ``--force`` - Force file over writting (default: False)
-``-l - log file name, --log log file name
-                        Defines log file name and/or path (default: None)
-``-n``, ``--nodelete`` - enable/disable deletion of exisiting files (default: False)
-``--timeout`` TIMEOUT - time in seconds before connection times out (default: 30)
-``-v``, ``--verbose`` - Set logger level to 'INFO' (default: False)
+By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
 ## Annotate CAZomes
 
 To retrieve the most comprehensive annotation of the CAZome, we recommend using the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
 
 > Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard; cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets, BioRxiv, 3 December 2022, https://doi.org/10.1101/2022.12.02.518825
 
@@ -314,20 +359,21 @@
 
 To include 'canonical' CAZy family classifications from CAZy, download all data from the CAZy database and compile the data into a local CAZyme database using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al., 2022).
 
 > cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets
 Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard
 bioRxiv 2022.12.02.518825; doi: https://doi.org/10.1101/2022.12.02.518825
 
-The `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
+Use the `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
 ```bash
 cazomevolve build_cazy_db \
   <email> \
-  <desired db path>
+  <desired path for db FILE>
 ```
+Note the path needs to point to the target FILE path not DIR path. `cazy_webscraper` will build all necessary parent directories.
 
 Or you can use `cazy_webscraper` directly
 ```bash
 cazy_webscraper \
     <email> \
     -o <db file output path>
 ```
@@ -378,26 +424,29 @@
 _`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM._
 
 `dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using the `cazomveolve`, subcommand `run_dbcan` command.
 
 ```bash
 cazomevolve run_dbcan \
     <path to dir containing FASTA files> \
-    <path to output directory> 
+    <path to output directory> \
+    <dbcan major version number, 2, 3 or 4>
 ```
 
+``cazomevolve`` will which ever version of dbCAN is installed, but the commands and arguments between dbCAN version 2, 3 and 4 are different, so ``cazomevolve`` must be told which version to of dbCAN to communicate with.
+
 The ouput directory will be created by `run_dbcan`. 
 
 Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
 
 Optional args:
 ```bash
 options:
   -h, --help            show this help message and exit
-  -V2--version_2        Use dbCAN version 2 NOT 3/4 (default: False)
+  --cpu CPU             Number of CPU cores to use. Default all available cores (default: all avilable cores)
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
@@ -433,17 +482,15 @@
 ```bash
 options:
   -h, --help            show this help message and exit
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
-  --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
-  -v2, --version_2      Parse the data from dbCAN version 2 (default: False, parse data from dbCAN version 3)
 ```
 
 # Explore the CAZome composition
 
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
```

### Comparing `cazomevolve-0.1.0/cazomevolve.egg-info/SOURCES.txt` & `cazomevolve-0.1.2/cazomevolve.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 cazomevolve.egg-info/SOURCES.txt
 cazomevolve.egg-info/dependency_links.txt
 cazomevolve.egg-info/entry_points.txt
 cazomevolve.egg-info/requires.txt
 cazomevolve.egg-info/top_level.txt
 cazomevolve/cazome/__init__.py
 cazomevolve/cazome/cazy/__init__.py
-cazomevolve/cazome/cazy/build_db.sh
 cazomevolve/cazome/cazy/get_cazy_cazymes.py
 cazomevolve/cazome/dbcan/__init__.py
 cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
 cazomevolve/cazome/dbcan/invoke_dbcan.py
 cazomevolve/cazome/explore/__init__.py
 cazomevolve/cazome/explore/cazome_sizes.py
 cazomevolve/cazome/explore/cazy_classes.py
@@ -23,23 +22,24 @@
 cazomevolve/cazome/explore/identify_families.py
 cazomevolve/cazome/explore/ie_cazymes.py
 cazomevolve/cazome/explore/parse_data.py
 cazomevolve/cazome/explore/pca.py
 cazomevolve/cazome/explore/plot.py
 cazomevolve/cazome/explore/taxonomies.py
 cazomevolve/genomes/__init__.py
-cazomevolve/genomes/download_acc_genomes.sh
 cazomevolve/genomes/download_genomes.py
 cazomevolve/scripts/__init__.py
 cazomevolve/scripts/build_cazy_db.py
 cazomevolve/scripts/cazomevolve_script.py
 cazomevolve/scripts/download_acc_genomes.py
 cazomevolve/scripts/get_fam_seqs.py
 cazomevolve/scripts/run_fam_blast.py
 cazomevolve/scripts/run_fam_diamond.py
+cazomevolve/scripts/bash/build_cazy_db.sh
+cazomevolve/scripts/bash/download_acc_genomes.sh
 cazomevolve/scripts/tree/ani/build_anim_tree.R
 cazomevolve/scripts/tree/ani/run_anim.sh
 cazomevolve/scripts/tree/phylo/align_scos.sh
 cazomevolve/scripts/tree/phylo/annotate_genomes.sh
 cazomevolve/scripts/tree/phylo/backtranslate.sh
 cazomevolve/scripts/tree/phylo/concatenate_cds.py
 cazomevolve/scripts/tree/phylo/extract_cds.py
```

### Comparing `cazomevolve-0.1.0/setup.py` & `cazomevolve-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazomevolve",
-    version="0.1.0",
+    version="0.1.2",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A bioinforamtic package for investigating the evolution of CAZomes"
@@ -70,19 +70,19 @@
     platforms="Posix, MacOS X",
     entry_points={
         "console_scripts": [
             "cazomevolve = cazomevolve.scripts.cazomevolve_script:main",
         ]
     },
     scripts=[
-        'cazomevolve/genomes/download_acc_genomes.sh',
+        'cazomevolve/scripts/bash/download_acc_genomes.sh',
         'cazomevolve/seq_diversity/get_fam_seqs.sh',
         'cazomevolve/seq_diversity/run_blastp.sh',
         'cazomevolve/seq_diversity/run_diamond.sh',
-        'cazomevolve/cazome/cazy/build_db.sh',
+        'cazomevolve/scripts/bash/build_cazy_db.sh',
         'cazomevolve/scripts/tree/phylo/align_scos.sh',
         'cazomevolve/scripts/tree/phylo/annotate_genomes.sh',
         'cazomevolve/scripts/tree/phylo/backtranslate.sh',
         'cazomevolve/scripts/tree/phylo/concatenate_cds.py',
         'cazomevolve/scripts/tree/phylo/extract_cds.py',
         'cazomevolve/scripts/tree/phylo/find_orthologues.sh',
         'cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh',
```

