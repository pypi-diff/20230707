# Comparing `tmp/celescope-1.8.1.tar.gz` & `tmp/celescope-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celescope-1.8.1.tar", last modified: Wed Mar 23 09:40:36 2022, max compression
+gzip compressed data, was "dist/celescope-1.9.0.tar", last modified: Fri Apr  1 09:26:13 2022, max compression
```

## Comparing `celescope-1.8.1.tar` & `celescope-1.9.0.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8325 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope.egg-info/dependency_links.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      109 2022-03-23 09:40:19.000000 celescope-1.8.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/rna/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2409 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6986 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna/star.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      565 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna/multi_rna.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      322 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2979 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna/mkref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/sweetseq/
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/sweetseq/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/sweetseq/multi_sweetseq.py
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/sweetseq/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/sweetseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/tag/
--rwxr-xr-x   0 runner    (1001) docker     (121)    11917 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/count_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/seurat_hashtag.R
--rw-r--r--   0 runner    (1001) docker     (121)     7682 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/split_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2222 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/multi_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7901 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/mapping_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1505 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/analysis_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      121 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/snp/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7566 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/analysis_snp.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/vcfR.R
--rwxr-xr-x   0 runner    (1001) docker     (121)     3814 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/variant_calling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      238 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/mkref.py
--rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/filter_snp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4012 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/snp/multi_snp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/hla/
--rwxr-xr-x   0 runner    (1001) docker     (121)      163 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/hla/multi_hla.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5897 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/hla/mapping_hla.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       98 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/hla/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1506 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/celescope.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/capture_virus/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/analysis_virus.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/count_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/multi_capture_virus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/filter_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      258 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      962 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_virus/mkref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/img/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4423 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/img/img1.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    28408 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/img/logo2.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/rna/
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna/star.html
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna/analysis.html
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna/count.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      646 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/sweetseq/
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/sweetseq/analysis.html
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/sweetseq/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/tag/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tag/analysis_tag.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      551 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tag/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/snp/
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/snp/analysis_snp.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      987 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/snp/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/trust_vdj/
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/trust_vdj/assemble_summary.html
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/trust_vdj/res_sum_summary.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/hla/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3667 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/hla/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/capture_virus/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/capture_virus/analysis_virus.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      844 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/capture_virus/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/help_info.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/utils/table_script/
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/table_script/dynaseq.html
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/table_script/rna.html
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/table_script/vdj.html
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/table_script/snp.html
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/start.html
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/end.html
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/table_dict.html
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/step.html
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/analysis.html
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/col2_metrics.html
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/preprocessing.html
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/head.html
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/utils/col1_metrics.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/citeseq/
--rw-r--r--   0 runner    (1001) docker     (121)     5634 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/citeseq/analysis_cite.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      228 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/citeseq/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/vdj/
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/vdj/count_vdj.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      519 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/vdj/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/capture_rna/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6930 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/capture_rna/count_capture_rna_summary.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     4021 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/capture_rna/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/rna_virus/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5719 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna_virus/analysis_rna_virus_summary.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     4001 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/rna_virus/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/mut/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3547 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/mut/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/tcr_fl/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1133 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tcr_fl/mapping_tag_summary.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     1311 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tcr_fl/count_tag_summary.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     3545 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tcr_fl/base.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     5634 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/tcr_fl/analysis_tag_summary.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/fusion/
--rwxr-xr-x   0 runner    (1001) docker     (121)      852 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/fusion/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/common/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5925 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/common/img1.html
--rwxr-xr-x   0 runner    (1001) docker     (121)    37927 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/common/logo.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/html/dynaseq/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/dynaseq/substitution.html
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/dynaseq/replace_tsne.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     1134 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/dynaseq/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/html/dynaseq/replacement.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/js/
--rwxr-xr-x   0 runner    (1001) docker     (121)   101939 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/jszip.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    81906 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/jquery.dataTables.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     1954 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/buttons.print.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)   447570 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/jquery.dataTables.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    25883 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/buttons.flash.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    86927 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/jquery.min.3.3.1.js
--rwxr-xr-x   0 runner    (1001) docker     (121)  3478132 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/plotly-1.58.4.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    23849 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/buttons.html5.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    17534 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/dataTables.buttons.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     3821 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/dataTables.jqueryui.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)  2812789 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/plotly-latest.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    86927 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/jquery.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    37045 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/css/
--rwxr-xr-x   0 runner    (1001) docker     (121)    15800 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/jquery.dataTables.css
--rwxr-xr-x   0 runner    (1001) docker     (121)   121200 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/bootstrap.min.css
--rwxr-xr-x   0 runner    (1001) docker     (121)     9160 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/buttons.dataTables.min.css
--rwxr-xr-x   0 runner    (1001) docker     (121)    38034 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/jquery-ui-git.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.eot
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.ttf
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.woff
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello.css
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello-codes.css
--rw-r--r--   0 runner    (1001) docker     (121)    13830 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello-embedded.css
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello-ie7.css
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/animation.css
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello-ie7-codes.css
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/fontello-323401c3/config.json
--rwxr-xr-x   0 runner    (1001) docker     (121)    37625 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/jquery-ui.css
--rwxr-xr-x   0 runner    (1001) docker     (121)    14476 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/templates/css/dataTables.jqueryui.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/citeseq/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1098 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/citeseq/analysis_cite.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1401 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/citeseq/multi_citeseq.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2495 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/citeseq/count_cite.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1393 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/citeseq/analysis_cite.R
--rwxr-xr-x   0 runner    (1001) docker     (121)      168 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/citeseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/tools/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2320 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/tools/cellranger3/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6632 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/sgt.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17305 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10291 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/cell_calling_3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11148 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cellranger3/get_plot_elements.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1579 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/sample.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2589 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/merge_table.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18609 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5957 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/target_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7940 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5054 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/star_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11570 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/analysis_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     6607 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/plotly_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4811 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/featureCounts.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19297 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/count.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/tools/capture/
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/capture/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/capture/count_bam.py
--rw-r--r--   0 runner    (1001) docker     (121)     9043 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/capture/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4978 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/capture/threshold.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      657 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3742 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/mkref.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7487 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/cutadapt.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1965 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7313 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/step.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14854 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/multi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24317 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/tools/barcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/vdj/
--rwxr-xr-x   0 runner    (1001) docker     (121)      179 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/vdj/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16676 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/vdj/count_vdj.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1369 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/vdj/multi_vdj.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7963 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/vdj/mapping_vdj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/snp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/snp/panel/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/snp/panel/lung_1.bed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/Clindex/
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/Clindex/tag_barcode.fasta
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/Clindex/tag_linker.fasta
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/HLA/
--rwxr-xr-x   0 runner    (1001) docker     (121)  4228813 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/HLA/hla_reference_rna.fasta
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/rRNA/
--rwxr-xr-x   0 runner    (1001) docker     (121)    43669 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/rRNA/human_ribo.fasta
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.1/bclist
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.1/linker_withC
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.2.1/
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.2.1/bclist
--rwxr-xr-x   0 runner    (1001) docker     (121)      136 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.2.1/linker_4types
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.1/bclist
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.1/linker_withC
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV3.0.1/bclist
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV3.0.1/linker_4types
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.0/bclist
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.1.0/linker
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.0/bclist
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/data/chemistry/scopeV2.0.0/linker
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/capture_rna/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1032 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_rna/multi_capture_rna.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4493 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_rna/count_capture_rna.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      241 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/capture_rna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/rna_virus/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1724 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna_virus/analysis_rna_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2228 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna_virus/count_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      948 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna_virus/star_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1611 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna_virus/multi_rna_virus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      240 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/rna_virus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1690 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/fusion/
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/analysis_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2111 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/multi_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      706 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/star_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      657 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/plot_fusion.R
--rwxr-xr-x   0 runner    (1001) docker     (121)     2655 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/count_fusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/filter_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      143 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1294 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/fusion/mkref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/dynaseq/
--rwxr-xr-x   0 runner    (1001) docker     (121)    10006 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11893 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/replacement.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1753 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/Generate_T_C_matrix.R
--rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/replace_tsne.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      472 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7814 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/substitution.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2674 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/dynaseq/multi_dynaseq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/celescope/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-03-23 09:40:19.000000 celescope-1.8.1/celescope/scripts/gene_umi_summary.R
--rwxr-xr-x   0 runner    (1001) docker     (121)     1081 2022-03-23 09:40:19.000000 celescope-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)      745 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1517 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/test_multi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/tests/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/tests/unittests/snp/
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/unittests/snp/test_snp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/unittests/snp/test_variant_calling.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/unittests/snp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-23 09:40:19.000000 celescope-1.8.1/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 09:40:36.000000 celescope-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-03-23 09:40:36.000000 celescope-1.8.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)      630 2022-03-23 09:40:19.000000 celescope-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:36.000000 celescope-1.8.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-03-23 09:40:19.000000 celescope-1.8.1/scripts/extract_read.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-03-23 09:40:19.000000 celescope-1.8.1/scripts/add_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2553 2022-03-23 09:40:19.000000 celescope-1.8.1/scripts/release_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     6693 2022-03-23 09:40:19.000000 celescope-1.8.1/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 09:40:19.000000 celescope-1.8.1/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8331 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope.egg-info/dependency_links.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      109 2022-04-01 09:25:56.000000 celescope-1.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/rna/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2514 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6986 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna/star.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      591 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna/multi_rna.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      322 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2979 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna/mkref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/sweetseq/
+-rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/sweetseq/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/sweetseq/multi_sweetseq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/sweetseq/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/sweetseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/tag/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11917 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/count_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/seurat_hashtag.R
+-rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/split_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2222 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/multi_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7901 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/mapping_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1505 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/analysis_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      121 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/snp/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7566 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/analysis_snp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/vcfR.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3814 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/variant_calling.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      238 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/mkref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/filter_snp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4012 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/snp/multi_snp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/hla/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      163 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/hla/multi_hla.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5897 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/hla/mapping_hla.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)       98 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/hla/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1506 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/celescope.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/capture_virus/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/analysis_virus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/count_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/multi_capture_virus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/filter_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      258 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      962 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_virus/mkref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/img/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4423 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/img/img1.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    28408 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/img/logo2.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/rna/
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna/star.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna/count.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      646 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/sweetseq/
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/sweetseq/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/sweetseq/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/tag/
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tag/analysis_tag.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      551 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tag/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/snp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/snp/analysis_snp.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      987 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/snp/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/trust_vdj/
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/trust_vdj/assemble_summary.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/trust_vdj/res_sum_summary.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/hla/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3667 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/hla/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/capture_virus/
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/capture_virus/analysis_virus.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      844 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/capture_virus/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/help_info.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/utils/table_script/
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/table_script/dynaseq.html
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/table_script/rna.html
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/table_script/vdj.html
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/table_script/snp.html
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/start.html
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/end.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/table_dict.html
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/step.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/col2_metrics.html
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/preprocessing.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/head.html
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/utils/col1_metrics.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/citeseq/
+-rw-r--r--   0 runner    (1001) docker     (121)     5634 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/citeseq/analysis_cite.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      228 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/citeseq/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/vdj/
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/vdj/count_vdj.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      519 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/vdj/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/capture_rna/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6930 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/capture_rna/count_capture_rna_summary.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4021 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/capture_rna/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/rna_virus/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5719 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna_virus/analysis_rna_virus_summary.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4001 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/rna_virus/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/mut/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3547 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/mut/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/tcr_fl/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1133 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tcr_fl/mapping_tag_summary.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1311 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tcr_fl/count_tag_summary.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3545 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tcr_fl/base.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5634 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/tcr_fl/analysis_tag_summary.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/fusion/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      852 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/fusion/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/common/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5925 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/common/img1.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)    37927 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/common/logo.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/html/dynaseq/
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/dynaseq/substitution.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/dynaseq/replace_tsne.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1134 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/dynaseq/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/html/dynaseq/replacement.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/js/
+-rwxr-xr-x   0 runner    (1001) docker     (121)   101939 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/jszip.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    81906 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/jquery.dataTables.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1954 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/buttons.print.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)   447570 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/jquery.dataTables.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    25883 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/buttons.flash.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    86927 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/jquery.min.3.3.1.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)  3478132 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/plotly-1.58.4.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23849 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/buttons.html5.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17534 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/dataTables.buttons.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3821 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/dataTables.jqueryui.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)  2812789 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/plotly-latest.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    86927 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/jquery.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    37045 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/css/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15800 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/jquery.dataTables.css
+-rwxr-xr-x   0 runner    (1001) docker     (121)   121200 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/bootstrap.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9160 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/buttons.dataTables.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (121)    38034 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/jquery-ui-git.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.eot
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.woff
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello.css
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello-codes.css
+-rw-r--r--   0 runner    (1001) docker     (121)    13830 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello-embedded.css
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello-ie7.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/animation.css
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello-ie7-codes.css
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/fontello-323401c3/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)    37625 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/jquery-ui.css
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14476 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/templates/css/dataTables.jqueryui.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/citeseq/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1098 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/citeseq/analysis_cite.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1401 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/citeseq/multi_citeseq.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2495 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/citeseq/count_cite.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1393 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/citeseq/analysis_cite.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)      168 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/citeseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2320 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/report.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2066 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/sample.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2589 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/merge_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19746 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/
+-rw-r--r--   0 runner    (1001) docker     (121)     6632 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/sgt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17363 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10289 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/cell_calling_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11148 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/emptydrop_cr/get_plot_elements.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5957 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/target_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7940 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5059 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/star_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11886 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/analysis_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6607 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/plotly_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4842 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/featureCounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19389 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/count.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/tools/capture/
+-rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/capture/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/capture/count_bam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9043 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/capture/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5020 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/capture/threshold.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      657 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3742 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/mkref.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7487 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/cutadapt.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1965 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7743 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/step.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14904 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/multi.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    24317 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/tools/barcode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/vdj/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      179 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/vdj/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16676 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/vdj/count_vdj.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1369 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/vdj/multi_vdj.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7963 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/vdj/mapping_vdj.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/snp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/snp/panel/
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/snp/panel/lung_1.bed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/Clindex/
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/Clindex/tag_barcode.fasta
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/Clindex/tag_linker.fasta
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/HLA/
+-rwxr-xr-x   0 runner    (1001) docker     (121)  4228813 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/HLA/hla_reference_rna.fasta
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/rRNA/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    43669 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/rRNA/human_ribo.fasta
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.1/bclist
+-rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.1/linker_withC
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.2.1/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.2.1/bclist
+-rwxr-xr-x   0 runner    (1001) docker     (121)      136 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.2.1/linker_4types
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.1/bclist
+-rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.1/linker_withC
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV3.0.1/bclist
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV3.0.1/linker_4types
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.0/bclist
+-rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.1.0/linker
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      960 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.0/bclist
+-rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/data/chemistry/scopeV2.0.0/linker
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/capture_rna/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1032 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_rna/multi_capture_rna.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4493 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_rna/count_capture_rna.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      241 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/capture_rna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/rna_virus/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1724 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna_virus/analysis_rna_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2228 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna_virus/count_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      948 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna_virus/star_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1611 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna_virus/multi_rna_virus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      240 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/rna_virus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1970 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/fusion/
+-rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/analysis_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2111 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/multi_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      706 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/star_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      657 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/plot_fusion.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2655 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/count_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/filter_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      143 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1294 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/fusion/mkref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/dynaseq/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10006 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11893 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/replacement.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1753 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/Generate_T_C_matrix.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/replace_tsne.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      472 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7814 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/substitution.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2674 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/dynaseq/multi_dynaseq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/celescope/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-01 09:25:56.000000 celescope-1.9.0/celescope/scripts/gene_umi_summary.R
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1081 2022-04-01 09:25:56.000000 celescope-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      745 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1517 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/test_multi.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/tests/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/tests/unittests/snp/
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/unittests/snp/test_snp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/unittests/snp/test_variant_calling.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/unittests/snp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-01 09:25:56.000000 celescope-1.9.0/tests/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-01 09:26:13.000000 celescope-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-04-01 09:26:13.000000 celescope-1.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)      630 2022-04-01 09:25:56.000000 celescope-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 09:26:13.000000 celescope-1.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-04-01 09:25:56.000000 celescope-1.9.0/scripts/extract_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-04-01 09:25:56.000000 celescope-1.9.0/scripts/add_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2553 2022-04-01 09:25:56.000000 celescope-1.9.0/scripts/release_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6693 2022-04-01 09:25:56.000000 celescope-1.9.0/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 09:25:56.000000 celescope-1.9.0/scripts/__init__.py
```

### Comparing `celescope-1.8.1/celescope.egg-info/PKG-INFO` & `celescope-1.9.0/celescope.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celescope
-Version: 1.8.1
+Version: 1.9.0
 Summary: Single Cell Analysis Pipelines
 Home-page: https://github.com/singleron-RD/CeleScope
 Author: zhouyiqi
 Author-email: zhouyiqi@singleronbio.com
 License: UNKNOWN
 Description: 
         # Introduction
```

### Comparing `celescope-1.8.1/celescope.egg-info/SOURCES.txt` & `celescope-1.9.0/celescope.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -188,20 +188,20 @@
 celescope/tools/target_metrics.py
 celescope/tools/utils.py
 celescope/tools/capture/__init__.py
 celescope/tools/capture/analysis.py
 celescope/tools/capture/count_bam.py
 celescope/tools/capture/filter.py
 celescope/tools/capture/threshold.py
-celescope/tools/cellranger3/__init__.py
-celescope/tools/cellranger3/cell_calling_3.py
-celescope/tools/cellranger3/get_plot_elements.py
-celescope/tools/cellranger3/sgt.py
-celescope/tools/cellranger3/stats.py
-celescope/tools/cellranger3/wrapper.py
+celescope/tools/emptydrop_cr/__init__.py
+celescope/tools/emptydrop_cr/cell_calling_3.py
+celescope/tools/emptydrop_cr/get_plot_elements.py
+celescope/tools/emptydrop_cr/sgt.py
+celescope/tools/emptydrop_cr/stats.py
+celescope/tools/emptydrop_cr/wrapper.py
 celescope/vdj/__init__.py
 celescope/vdj/count_vdj.py
 celescope/vdj/mapping_vdj.py
 celescope/vdj/multi_vdj.py
 scripts/__init__.py
 scripts/add_tag.py
 scripts/extract_read.py
```

### Comparing `celescope-1.8.1/celescope.egg-info/entry_points.txt` & `celescope-1.9.0/celescope.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna/analysis.py` & `celescope-1.9.0/celescope/rna/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,21 +32,22 @@
         super().__init__(args, display_title)
 
         self.display_title = display_title
         self._table_id = 'marker_genes'
 
     def run(self):
 
-        scanpy_wrapper = analysis_wrapper.Scanpy_wrapper(self.args, display_title=self.display_title)
-        scanpy_wrapper.run()
+        with analysis_wrapper.Scanpy_wrapper(self.args, display_title=self.display_title) as scanpy_wrapper:
+            scanpy_wrapper.run()
+            df_tsne, df_marker = scanpy_wrapper.get_df()
+            self.set_metric_list(metric_list=scanpy_wrapper.get_metric_list())
 
-        report_runner = analysis_wrapper.Report_runner(self.args, display_title=self.display_title)
-        report_runner.add_marker_help()
+        with analysis_wrapper.Report_runner(self.args, display_title=self.display_title) as report_runner:
+            report_runner.add_marker_help()
 
-        df_tsne, df_marker = scanpy_wrapper.get_df()
 
         tsne_cluster = Tsne_plot(df_tsne, 'cluster').get_plotly_div()
         self.add_data(tsne_cluster=tsne_cluster)
 
         tsne_gene = Tsne_plot(df_tsne, 'Gene_Counts', discrete=False).get_plotly_div()
         self.add_data(tsne_gene=tsne_gene)
```

### Comparing `celescope-1.8.1/celescope/rna/star.py` & `celescope-1.9.0/celescope/rna/star.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna/mkref.py` & `celescope-1.9.0/celescope/rna/mkref.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/sweetseq/analysis.py` & `celescope-1.9.0/celescope/sweetseq/analysis.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/sweetseq/multi_sweetseq.py` & `celescope-1.9.0/celescope/sweetseq/multi_sweetseq.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/sweetseq/mapping.py` & `celescope-1.9.0/celescope/sweetseq/mapping.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tag/count_tag.py` & `celescope-1.9.0/celescope/tag/count_tag.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tag/seurat_hashtag.R` & `celescope-1.9.0/celescope/tag/seurat_hashtag.R`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tag/split_tag.py` & `celescope-1.9.0/celescope/tag/split_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pysam
 import pandas as pd
 
 from celescope.tools import utils
 from celescope.tools.step import Step, s_common
 from celescope.tools.__init__ import FILTERED_MATRIX_DIR_SUFFIX
 from celescope.__init__ import HELP_DICT
-from celescope.tools.cellranger3.wrapper import Cell_calling, read_raw_matrix
+from celescope.tools.emptydrop_cr.wrapper import Cell_calling, read_raw_matrix
 
 
 def get_clonotypes_table(df):
     chains = sorted(set(df['chain'].tolist()))
     res = pd.DataFrame(columns=['barcode'])
     for c in chains:
         df_c = df[df['chain'] == c][['barcode', 'aaSeqCDR3', 'nSeqCDR3']]
```

### Comparing `celescope-1.8.1/celescope/tag/multi_tag.py` & `celescope-1.9.0/celescope/tag/multi_tag.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tag/mapping_tag.py` & `celescope-1.9.0/celescope/tag/mapping_tag.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tag/analysis_tag.py` & `celescope-1.9.0/celescope/tag/analysis_tag.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/snp/analysis_snp.py` & `celescope-1.9.0/celescope/snp/analysis_snp.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/snp/variant_calling.py` & `celescope-1.9.0/celescope/snp/variant_calling.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/snp/mkref.py` & `celescope-1.9.0/celescope/snp/mkref.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/snp/filter_snp.py` & `celescope-1.9.0/celescope/snp/filter_snp.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/snp/multi_snp.py` & `celescope-1.9.0/celescope/snp/multi_snp.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/hla/mapping_hla.py` & `celescope-1.9.0/celescope/hla/mapping_hla.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/celescope.py` & `celescope-1.9.0/celescope/celescope.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/capture_virus/multi_capture_virus.py` & `celescope-1.9.0/celescope/capture_virus/multi_capture_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/capture_virus/filter_virus.py` & `celescope-1.9.0/celescope/capture_virus/filter_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/capture_virus/mkref.py` & `celescope-1.9.0/celescope/capture_virus/mkref.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/img/img1.png` & `celescope-1.9.0/celescope/templates/img/img1.png`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/img/logo2.png` & `celescope-1.9.0/celescope/templates/img/logo2.png`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna/star.html` & `celescope-1.9.0/celescope/templates/html/rna/star.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna/analysis.html` & `celescope-1.9.0/celescope/templates/html/rna/analysis.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna/count.html` & `celescope-1.9.0/celescope/templates/html/rna/count.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna/base.html` & `celescope-1.9.0/celescope/templates/html/rna/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/sweetseq/analysis.html` & `celescope-1.9.0/celescope/templates/html/sweetseq/analysis.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tag/analysis_tag.html` & `celescope-1.9.0/celescope/templates/html/tag/analysis_tag.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tag/base.html` & `celescope-1.9.0/celescope/templates/html/tag/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/snp/analysis_snp.html` & `celescope-1.9.0/celescope/templates/html/snp/analysis_snp.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/snp/base.html` & `celescope-1.9.0/celescope/templates/html/snp/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/trust_vdj/assemble_summary.html` & `celescope-1.9.0/celescope/templates/html/trust_vdj/assemble_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/trust_vdj/res_sum_summary.html` & `celescope-1.9.0/celescope/templates/html/trust_vdj/res_sum_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/hla/base.html` & `celescope-1.9.0/celescope/templates/html/hla/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/capture_virus/analysis_virus.html` & `celescope-1.9.0/celescope/templates/html/capture_virus/analysis_virus.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/capture_virus/base.html` & `celescope-1.9.0/celescope/templates/html/capture_virus/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/table_script/dynaseq.html` & `celescope-1.9.0/celescope/templates/html/utils/table_script/dynaseq.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/table_script/rna.html` & `celescope-1.9.0/celescope/templates/html/utils/table_script/rna.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/table_dict.html` & `celescope-1.9.0/celescope/templates/html/utils/table_dict.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/analysis.html` & `celescope-1.9.0/celescope/templates/html/utils/analysis.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/col2_metrics.html` & `celescope-1.9.0/celescope/templates/html/utils/col2_metrics.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/utils/head.html` & `celescope-1.9.0/celescope/templates/html/utils/head.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/citeseq/analysis_cite.html` & `celescope-1.9.0/celescope/templates/html/citeseq/analysis_cite.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/vdj/count_vdj.html` & `celescope-1.9.0/celescope/templates/html/vdj/count_vdj.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/vdj/base.html` & `celescope-1.9.0/celescope/templates/html/vdj/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/capture_rna/count_capture_rna_summary.html` & `celescope-1.9.0/celescope/templates/html/capture_rna/count_capture_rna_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/capture_rna/base.html` & `celescope-1.9.0/celescope/templates/html/capture_rna/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna_virus/analysis_rna_virus_summary.html` & `celescope-1.9.0/celescope/templates/html/rna_virus/analysis_rna_virus_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/rna_virus/base.html` & `celescope-1.9.0/celescope/templates/html/rna_virus/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/mut/base.html` & `celescope-1.9.0/celescope/templates/html/mut/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tcr_fl/mapping_tag_summary.html` & `celescope-1.9.0/celescope/templates/html/tcr_fl/mapping_tag_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tcr_fl/count_tag_summary.html` & `celescope-1.9.0/celescope/templates/html/tcr_fl/count_tag_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tcr_fl/base.html` & `celescope-1.9.0/celescope/templates/html/tcr_fl/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/tcr_fl/analysis_tag_summary.html` & `celescope-1.9.0/celescope/templates/html/tcr_fl/analysis_tag_summary.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/fusion/base.html` & `celescope-1.9.0/celescope/templates/html/fusion/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/common/img1.html` & `celescope-1.9.0/celescope/templates/html/common/img1.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/common/logo.html` & `celescope-1.9.0/celescope/templates/html/common/logo.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/dynaseq/substitution.html` & `celescope-1.9.0/celescope/templates/html/dynaseq/substitution.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/dynaseq/replace_tsne.html` & `celescope-1.9.0/celescope/templates/html/dynaseq/replace_tsne.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/html/dynaseq/base.html` & `celescope-1.9.0/celescope/templates/html/dynaseq/base.html`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/jszip.min.js` & `celescope-1.9.0/celescope/templates/js/jszip.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/jquery.dataTables.min.js` & `celescope-1.9.0/celescope/templates/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/buttons.print.min.js` & `celescope-1.9.0/celescope/templates/js/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/jquery.dataTables.js` & `celescope-1.9.0/celescope/templates/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/buttons.flash.min.js` & `celescope-1.9.0/celescope/templates/js/buttons.flash.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/jquery.min.3.3.1.js` & `celescope-1.9.0/celescope/templates/js/jquery.min.3.3.1.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/plotly-1.58.4.min.js` & `celescope-1.9.0/celescope/templates/js/plotly-1.58.4.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/buttons.html5.min.js` & `celescope-1.9.0/celescope/templates/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/dataTables.buttons.min.js` & `celescope-1.9.0/celescope/templates/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/dataTables.jqueryui.min.js` & `celescope-1.9.0/celescope/templates/js/dataTables.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/plotly-latest.min.js` & `celescope-1.9.0/celescope/templates/js/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/jquery.min.js` & `celescope-1.9.0/celescope/templates/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/js/bootstrap.min.js` & `celescope-1.9.0/celescope/templates/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/jquery.dataTables.css` & `celescope-1.9.0/celescope/templates/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/bootstrap.min.css` & `celescope-1.9.0/celescope/templates/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/buttons.dataTables.min.css` & `celescope-1.9.0/celescope/templates/css/buttons.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/jquery-ui-git.css` & `celescope-1.9.0/celescope/templates/css/jquery-ui-git.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.woff2` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.woff2`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.eot` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.ttf` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.svg` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/font/fontello.woff` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello.css` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/fontello-embedded.css` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/fontello-embedded.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/fontello-323401c3/css/animation.css` & `celescope-1.9.0/celescope/templates/css/fontello-323401c3/css/animation.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/jquery-ui.css` & `celescope-1.9.0/celescope/templates/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/templates/css/dataTables.jqueryui.min.css` & `celescope-1.9.0/celescope/templates/css/dataTables.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/citeseq/analysis_cite.py` & `celescope-1.9.0/celescope/citeseq/analysis_cite.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/citeseq/multi_citeseq.py` & `celescope-1.9.0/celescope/citeseq/multi_citeseq.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/citeseq/count_cite.py` & `celescope-1.9.0/celescope/citeseq/count_cite.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/citeseq/analysis_cite.R` & `celescope-1.9.0/celescope/citeseq/analysis_cite.R`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/report.py` & `celescope-1.9.0/celescope/tools/report.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/cellranger3/sgt.py` & `celescope-1.9.0/celescope/tools/emptydrop_cr/sgt.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/cellranger3/stats.py` & `celescope-1.9.0/celescope/tools/emptydrop_cr/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,31 +148,31 @@
 #     return float(recovered_cells) * cr_constants.FILTER_BARCODES_MAX_RECOVERED_CELLS_MULTIPLE # 6
     return float(recovered_cells) * 6
 
 
 def init_barcode_filter_result():
     return {
         'filtered_bcs': 0,
-        'filtered_bcs_lb': 0,
-        'filtered_bcs_ub': 0,
-        'max_filtered_bcs': 0,
+        #'filtered_bcs_lb': 0,
+        #'filtered_bcs_ub': 0,
+        #'max_filtered_bcs': 0,
         'filtered_bcs_var': 0,
-        'filtered_bcs_cv': 0,
+        #'filtered_bcs_cv': 0,
     }
 
 
 def summarize_bootstrapped_top_n(top_n_boot):
     top_n_bcs_mean = np.mean(top_n_boot)
-    top_n_bcs_sd = np.std(top_n_boot)
+    #top_n_bcs_sd = np.std(top_n_boot)
     top_n_bcs_var = np.var(top_n_boot)
     result = {}
     result['filtered_bcs_var'] = top_n_bcs_var
-#     result['filtered_bcs_cv'] = tk_stats.robust_divide(top_n_bcs_sd, top_n_bcs_mean)
-    result['filtered_bcs_lb'] = round(sp_stats.norm.ppf(0.025, top_n_bcs_mean, top_n_bcs_sd))
-    result['filtered_bcs_ub'] = round(sp_stats.norm.ppf(0.975, top_n_bcs_mean, top_n_bcs_sd))
+    # comment these two lines out to avoid `ValueError: cannot convert float NaN to integer` when analyze data with low number of barcode
+    #result['filtered_bcs_lb'] = round(sp_stats.norm.ppf(0.025, top_n_bcs_mean, top_n_bcs_sd))
+    #result['filtered_bcs_ub'] = round(sp_stats.norm.ppf(0.975, top_n_bcs_mean, top_n_bcs_sd))
     result['filtered_bcs'] = int(round(top_n_bcs_mean))
     return result
 
 
 def find_within_ordmag(x, baseline_idx):
     x_ascending = np.sort(x)
     baseline = x_ascending[-baseline_idx]
```

### Comparing `celescope-1.8.1/celescope/tools/cellranger3/wrapper.py` & `celescope-1.9.0/celescope/tools/emptydrop_cr/wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-cellranger3 cell-calling on raw matrix
+emptydrop_cr cell-calling on raw matrix
 """
 
 import os
 import sys
 
 import numpy as np
 import pandas as pd
 import scipy.io
 
 from celescope.tools.__init__ import (BARCODE_FILE_NAME, FEATURE_FILE_NAME,
                                       MATRIX_FILE_NAME)
-from celescope.tools.cellranger3.cell_calling_3 import find_nonambient_barcodes
+from celescope.tools.emptydrop_cr.cell_calling_3 import find_nonambient_barcodes
 from celescope.tools import utils
 
 
 EXPECTED_CELL_NUM = 3000
 
 
 @utils.add_log
@@ -23,15 +23,15 @@
 
     raw_mat_path = os.path.join(all_matrix_10X_dir, MATRIX_FILE_NAME[0])
     raw_mat = scipy.io.mmread(raw_mat_path)  # scipy.sparse.coo.coo_matrix
 
     raw_features_path = os.path.join(all_matrix_10X_dir, FEATURE_FILE_NAME[0])
 
     raw_barcodes_path = os.path.join(all_matrix_10X_dir, BARCODE_FILE_NAME[0])
-    raw_barcodes_df = pd.read_csv(raw_barcodes_path, sep='\t', error_bad_lines=False, names=['barcode'])
+    raw_barcodes_df = pd.read_csv(raw_barcodes_path, sep='\t', on_bad_lines='skip', names=['barcode'])
     raw_barcodes = np.array(raw_barcodes_df['barcode'].tolist())
 
     return raw_mat, raw_features_path, raw_barcodes
 
 
 @utils.add_log
 def cell_calling(raw_mat, expected_cell_num):
```

### Comparing `celescope-1.8.1/celescope/tools/cellranger3/cell_calling_3.py` & `celescope-1.9.0/celescope/tools/emptydrop_cr/cell_calling_3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from collections import namedtuple
 
 import numpy as np
 import numpy.ma as ma
 import pandas as pd
 import scipy.io
 
-import celescope.tools.cellranger3.sgt as cr_sgt  # # modified sgt.py
-import celescope.tools.cellranger3.stats as cr_stats  # # modified stats.py
+import celescope.tools.emptydrop_cr.sgt as cr_sgt  # # modified sgt.py
+import celescope.tools.emptydrop_cr.stats as cr_stats  # # modified stats.py
 from celescope.tools.__init__ import (BARCODE_FILE_NAME, FEATURE_FILE_NAME,
                                       MATRIX_FILE_NAME)
 
 # Set random seed
 random.seed(0)
 np.random.seed(0)
 
@@ -223,21 +223,21 @@
 
 def cell_calling_3(all_matrix_10X_dir, expected_cell_num):
 
     raw_mat_path = os.path.join(all_matrix_10X_dir, MATRIX_FILE_NAME[0])
     raw_mat = scipy.io.mmread(raw_mat_path)  # scipy.sparse.coo.coo_matrix
 
     raw_features_path = os.path.join(all_matrix_10X_dir, FEATURE_FILE_NAME[0])
-    raw_features_df = pd.read_csv(raw_features_path, sep='\t', error_bad_lines=False, names=['id', 'name', 'type'])
+    raw_features_df = pd.read_csv(raw_features_path, sep='\t', on_bad_lines='skip', names=['id', 'name', 'type'])
     raw_features_df['id'].tolist()
     raw_features_df['name'].tolist()
     raw_features_df['type'].tolist()
 
     raw_barcodes_path = os.path.join(all_matrix_10X_dir, BARCODE_FILE_NAME[0])
-    raw_barcodes_df = pd.read_csv(raw_barcodes_path, sep='\t', error_bad_lines=False, names=['barcode'])
+    raw_barcodes_df = pd.read_csv(raw_barcodes_path, sep='\t', on_bad_lines='skip', names=['barcode'])
     raw_barcodes = np.array(raw_barcodes_df['barcode'].tolist())
 
     # Run cell calling
     filtered_bc_indices, round_1_filtered_metrics, _non_ambient_barcode_result = find_nonambient_barcodes(
         raw_mat=raw_mat, recovered_cells=expected_cell_num)
 
     cell_bc = raw_barcodes[filtered_bc_indices]
```

### Comparing `celescope-1.8.1/celescope/tools/cellranger3/get_plot_elements.py` & `celescope-1.9.0/celescope/tools/emptydrop_cr/get_plot_elements.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/sample.py` & `celescope-1.9.0/celescope/tools/sample.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 from celescope.tools import utils
 from celescope.__init__ import __VERSION__
 from celescope.tools.__init__ import __PATTERN_DICT__
 from celescope.tools.barcode import Chemistry
 from celescope.tools.step import Step, s_common
 
 
+def add_kit_version(chemistry):
+    kit_dict = {
+        '1': 'no longer in use',
+        '2': 'kit V1',
+        '3': 'kit V2',
+    }
+    if chemistry.startswith('scopeV'):
+        s = chemistry.replace('scopeV', '')
+        chem_version = s[0]
+        kit = kit_dict[chem_version]
+        chemistry = f'{chemistry} ({kit})'
+    
+    return chemistry
+
 class Sample(Step):
     def __init__(self, args):
         Step.__init__(self, args)
         self.assay_description = utils.get_assay_text(self.assay)
         self.version = __VERSION__
         self.chemistry = args.chemistry
 
@@ -31,15 +45,16 @@
         self.add_metric(
             name='Assay',
             value=self.assay_description,
         )
         self.add_metric(
             name='Chemistry',
             value=chemistry,
-            help_info='Chemistry of the input fastqs',
+            display=add_kit_version(chemistry),
+            help_info='For more information, see <a href="https://github.com/singleron-RD/CeleScope/blob/master/docs/chemistry.md">here</a>',
         )
         self.add_metric(
             name='Software Version',
             value=self.version,
         )
```

### Comparing `celescope-1.8.1/celescope/tools/merge_table.py` & `celescope-1.9.0/celescope/tools/merge_table.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/utils.py` & `celescope-1.9.0/celescope/tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import importlib
 import logging
 import os
 import re
 import resource
 import subprocess
 import time
+import unittest
 from collections import Counter, defaultdict
 from datetime import timedelta
 from functools import wraps
 
 import pandas as pd
 import pysam
 
@@ -88,17 +89,19 @@
     else:
         file_obj = open(file_name, *args, **kwargs)
     return file_obj
 
 
 class Gtf_dict(dict):
     '''
-
     key: gene_id
     value: gene_name
+    If the key does not exist, return key. This is to avoid the error:
+        The gtf file contains one exon lines with a gene_id, but do not contain a gene line with the same gene_id. FeatureCounts 
+        work correctly under this condition, but the gene_id will not appear in the Gtf_dict.
     '''
 
     def __init__(self, gtf_file):
         super().__init__()
         self.gtf_file = gtf_file
         self.load_gtf()
 
@@ -106,14 +109,15 @@
     @add_log
     def load_gtf(self):
         """
         get gene_id:gene_name from gtf file
             - one gene_name with multiple gene_id: "_{count}" will be added to gene_name.
             - one gene_id with multiple gene_name: error.
             - duplicated (gene_name, gene_id): ignore duplicated records and print a warning.
+            - no gene_name: gene_id will be used as gene_name.
 
         Returns:
             {gene_id: gene_name} dict
         """
 
         gene_id_pattern = re.compile(r'gene_id "(\S+)";')
         gene_name_pattern = re.compile(r'gene_name "(\S+)"')
@@ -610,8 +614,25 @@
         rec_dict['GT'] = [s['GT'] for s in rec.samples.values()][0]
         rec_dict['GT'] = [str(item) for item in rec_dict['GT']]
         rec_dict['GT'] = '/'.join(rec_dict['GT'])
         '''
 
         df = df.append(pd.Series(rec_dict), ignore_index=True)
     vcf.close()
-    return df
+    return df
+
+
+class Test_utils(unittest.TestCase):
+    def test_gtf_dict(self):
+        import tempfile
+        fp = tempfile.NamedTemporaryFile(suffix='.gtf')
+        fp.write(b'1\tprocessed_transcript\tgene\t11869\t14409\t.\t+\t.\tgene_id "gene_id_with_gene_name"; gene_name "gene_name";\n')
+        fp.write(b'1\tprocessed_transcript\tgene\t11869\t14409\t.\t+\t.\tgene_id "gene_id_without_gene_name"; \n')
+        fp.seek(0)
+        gtf_dict = Gtf_dict(fp.name)
+        self.assertEqual(gtf_dict['gene_id_with_gene_name'], 'gene_name')
+        self.assertEqual(gtf_dict['gene_id_without_gene_name'], 'gene_id_without_gene_name')
+        self.assertEqual(gtf_dict['gene_id_not_exist'], 'gene_id_not_exist')
+        fp.close()
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `celescope-1.8.1/celescope/tools/target_metrics.py` & `celescope-1.9.0/celescope/tools/target_metrics.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/consensus.py` & `celescope-1.9.0/celescope/tools/consensus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/star_mixin.py` & `celescope-1.9.0/celescope/tools/star_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         default=0
     )
     parser.add_argument(
         '--out_unmapped',
         help='Output unmapped reads.',
         action='store_true'
     )
-    parser.add_argument('--STAR_param', help='Other STAR parameters.', default="")
+    parser.add_argument('--STAR_param', help=HELP_DICT['additional_param'], default="")
     parser.add_argument(
         '--outFilterMultimapNmax',
         help='Default `1`. How many places are allowed to match a read at most.',
         default=1
     )
     parser.add_argument(
         '--starMem',
```

### Comparing `celescope-1.8.1/celescope/tools/analysis_wrapper.py` & `celescope-1.9.0/celescope/tools/analysis_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import pandas as pd
 
 from celescope.tools import utils
 from celescope.__init__ import HELP_DICT
 from celescope.rna.mkref import Mkref_rna
 from celescope.tools.step import Step, s_common
 
-
+# markers adjust p_value
+PVAL_CUTOFF = 0.05
+# scanpy mitochonrial variable name
 MITO_VAR = 'mito'
 NORMALIZED_LAYER = 'normalised'
-
 RESOLUTION = 1.2
 N_PCS = 25
-PVAL_CUTOFF = 0.05
+MITO_GENE_PERCENT_LIST = [5, 10, 15, 20, 50]
 
 
 def read_tsne(tsne_file):
     df = pd.read_csv(tsne_file, sep='\t')
     # compatible with old version
     if 'Unnamed: 0' in df.columns:
         df.rename(columns={'Unnamed: 0': 'barcode'}, inplace=True)
@@ -87,29 +88,28 @@
             use_raw=False,
             log1p=False, 
             inplace=True
         )
 
     @utils.add_log
     def write_mito_stats(self):
- 
-        #stat.txt
-        total_cell = len(self.adata.obs)
-        percent_list = [5,10,15,20,50]
-        mito_dict = {
-            key: sum(self.adata.obs[f'pct_counts_{MITO_VAR}'] > key) / total_cell             
-            for key in percent_list
-        }
 
-        for percent in percent_list:
+        mt_pct_var = f'pct_counts_{MITO_VAR}'
+        total_cell_number = self.adata.n_obs
+
+        for mito_gene_percent in MITO_GENE_PERCENT_LIST:
+            cell_number = sum(self.adata.obs[mt_pct_var] > mito_gene_percent)
+            fraction = round(cell_number / total_cell_number * 100, 2)
             self.add_metric(
-                name=f'Fraction of cells have mito gene percent>{percent}%',
-                value=round(mito_dict[percent], 2),
+                name=f'Fraction of cells have mito gene percent>{mito_gene_percent}%',
+                value=f'{fraction}%',
+                show=False,
             )
 
+
     @utils.add_log
     def normalize(self):
         """
         sc.pp.normalize_per_cell() and sc.pp.log1p()
         """
 
         sc.pp.normalize_total(
@@ -249,15 +249,15 @@
             partition_type=None,
             neighbors_key=None,
             obsp=None,
             copy=False
         )
 
     @utils.add_log
-    def cluster(self):
+    def find_marker_genes(self):
         """
         Wrapper function for sc.tl.rank_genes_groups
         """
         sc.tl.rank_genes_groups(
             self.adata,
             "cluster",
             reference='rest',
@@ -265,27 +265,31 @@
             method="wilcoxon",
             use_raw=False,
             layer=NORMALIZED_LAYER
         )
 
     @utils.add_log
     def write_markers(self):
+        '''
+        write only p_val_adj < PVAL_CUTOFF to avoid too many markers
+        '''
         df_markers = sc.get.rank_genes_groups_df(self.adata, group=None, pval_cutoff=PVAL_CUTOFF)
         df_markers = df_markers[df_markers['logfoldchanges'].notna()]
         markers_name_dict = {
             'group':'cluster',
             'names':'gene',
             'logfoldchanges':'avg_log2FC',
             'pvals':'p_val',
             'pvals_adj':'p_val_adj',
             'pct_nz_group':'pct.1',
             'pct_nz_reference':'pct.2'
          }
         df_markers = df_markers.rename(markers_name_dict,axis='columns')
         df_markers['cluster'] = df_markers['cluster'].map(lambda x : int(x)+1)
+        df_markers = df_markers.loc[df_markers['p_val_adj'] < PVAL_CUTOFF, ]
         df_markers.to_csv(self.df_marker_file, index=None, sep='\t')
 
     @utils.add_log
     def write_tsne(self):
         df_tsne = self.adata.obsm.to_df()[['X_tsne1','X_tsne2']]
         df_tsne['cluster']=self.adata.obs.cluster
         df_tsne['Gene_Counts']=self.adata.obs.n_genes_by_counts
@@ -308,16 +312,15 @@
         self.hvg()
         self.scale()
         self.pca()
         self.neighbors()
         self.tsne()
         self.umap()
         self.leiden()
-        self.cluster()
-
+        self.find_marker_genes()
 
         self.write_markers()
         self.write_tsne()
         self.write_h5ad()
 
 
     def get_df(self):
```

### Comparing `celescope-1.8.1/celescope/tools/plotly_plot.py` & `celescope-1.9.0/celescope/tools/plotly_plot.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/featureCounts.py` & `celescope-1.9.0/celescope/tools/featureCounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import os
 import re
 
 from celescope.rna.mkref import Mkref_rna
 from celescope.tools.step import Step, s_common
 from celescope.tools import utils
+from celescope.__init__ import HELP_DICT
 
 
 class FeatureCounts(Step):
     """
     ## Features
     - Assigning uniquely mapped reads to genomic features with FeatureCounts.
     ## Output
@@ -126,14 +127,14 @@
 
 def get_opts_featureCounts(parser, sub_program):
     parser.add_argument(
         '--gtf_type',
         help='Specify feature type in GTF annotation',
         default='exon'
     )
-    parser.add_argument('--genomeDir', help='Required. Genome directory.')
-    parser.add_argument('--featureCounts_param', help='Other featureCounts parameters', default="")
+    parser.add_argument('--genomeDir', help=HELP_DICT['genomeDir'])
+    parser.add_argument('--featureCounts_param', help=HELP_DICT['additional_param'], default="")
 
     if sub_program:
         parser.add_argument('--input', help='Required. BAM file path.', required=True)
         parser = s_common(parser)
     return parser
```

### Comparing `celescope-1.8.1/celescope/tools/count.py` & `celescope-1.9.0/celescope/tools/count.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 import numpy as np
 import pandas as pd
 import pysam
 from scipy.io import mmwrite
 from scipy.sparse import coo_matrix
 
 from celescope.tools import utils
+from celescope.__init__ import HELP_DICT
 from celescope.tools.__init__ import (BARCODE_FILE_NAME, FEATURE_FILE_NAME,
     MATRIX_FILE_NAME, FILTERED_MATRIX_DIR_SUFFIX, RAW_MATRIX_DIR_SUFFIX)
-from celescope.tools.cellranger3 import get_plot_elements
-from celescope.tools.cellranger3.cell_calling_3 import cell_calling_3
+from celescope.tools.emptydrop_cr import get_plot_elements
+from celescope.tools.emptydrop_cr.cell_calling_3 import cell_calling_3
 from celescope.tools.step import Step, s_common
 from celescope.rna.mkref import Mkref_rna
 from celescope.tools.plotly_plot import Line_plot
 
 TOOLS_DIR = os.path.dirname(__file__)
 random.seed(0)
 np.random.seed(0)
@@ -211,16 +212,16 @@
     def cell_calling(self, df_sum):
         cell_calling_method = self.cell_calling_method
 
         if (self.force_cell_num is not None) and (self.force_cell_num != 'None'):
             cell_bc, UMI_threshold = self.force_cell(df_sum)
         elif cell_calling_method == 'auto':
             cell_bc, UMI_threshold = self.auto_cell(df_sum)
-        elif cell_calling_method == 'cellranger3':
-            cell_bc, UMI_threshold = self.cellranger3_cell(df_sum)
+        elif cell_calling_method == 'EmptyDrops_CR':
+            cell_bc, UMI_threshold = self.emptydrop_cr_cell(df_sum)
         return cell_bc, UMI_threshold
 
     @utils.add_log
     def force_cell(self, df_sum):
         force_cell_num = int(self.force_cell_num)
 
         df_barcode_count = df_sum.groupby(
@@ -260,15 +261,15 @@
         threshold = int(Count.find_threshold(df_sum, idx) * 0.1)
         threshold = max(1, threshold)
         cell_bc = Count.get_cell_bc(df_sum, threshold)
 
         return cell_bc, threshold
 
     @utils.add_log
-    def cellranger3_cell(self, df_sum):
+    def emptydrop_cr_cell(self, df_sum):
         cell_bc, initial_cell_num = cell_calling_3(self.raw_matrix_dir, self.expected_cell_num)
         threshold = Count.find_threshold(df_sum, initial_cell_num)
         return cell_bc, threshold
 
     @staticmethod
     def get_df_sum(df, col='UMI'):
         def num_gt2(x):
@@ -322,15 +323,15 @@
     def get_summary(self, CB_describe, CB_total_Genes,
                     CB_reads_count, reads_mapped_to_transcriptome):
 
         estimated_cells = int(CB_describe.loc['count', 'readcount'])
         self.add_metric(
             name='Estimated Number of Cells',
             value=estimated_cells,
-            help_info='the number of barcodes considered as cell-associated'
+            help_info=f'the number of barcodes considered as cell-associated. The cell calling method used for this sample is {self.cell_calling_method}.'
         )
 
         fraction_reads_in_cells = round(float(CB_reads_count) / reads_mapped_to_transcriptome * 100, 2)
         self.add_metric(
             name='Fraction Reads in Cells',
             value=fraction_reads_in_cells,
             display=f'{fraction_reads_in_cells}%',
@@ -464,17 +465,17 @@
 
 
 def get_opts_count(parser, sub_program):
     parser.add_argument('--genomeDir', help='Required. Genome directory.')
     parser.add_argument('--expected_cell_num', help='Default `3000`. Expected cell number.', default=3000)
     parser.add_argument(
         '--cell_calling_method',
-        help='Default `auto`. Cell calling methods. Choose from `auto` and `cellranger3`',
-        choices=['auto', 'cellranger3'],
-        default='auto',
+        help=HELP_DICT['cell_calling_method'],
+        choices=['auto', 'EmptyDrops_CR'],
+        default='EmptyDrops_CR',
     )
     if sub_program:
         parser = s_common(parser)
         parser.add_argument('--bam', help='Required. BAM file from featureCounts.', required=True)
         parser.add_argument(
             '--force_cell_num',
             help='Default `None`. Force the cell number to be this number. ',
```

### Comparing `celescope-1.8.1/celescope/tools/capture/analysis.py` & `celescope-1.9.0/celescope/tools/capture/analysis.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/capture/count_bam.py` & `celescope-1.9.0/celescope/tools/capture/count_bam.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/capture/filter.py` & `celescope-1.9.0/celescope/tools/capture/filter.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/capture/threshold.py` & `celescope-1.9.0/celescope/tools/capture/threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,28 @@
         return_threshold = math.ceil(self.log_base ** self.threshold)
 
         return return_threshold
 
 
 class Auto():
     """
-    threshold = top 1% cell count / 10
+    threshold = top 1% cell count / coef
     """
-    def __init__(self, array):
+    def __init__(self, array, coef=3):
         self.array = [x for x in array if x > 0 ]
+        self.coef = coef
     
     def run(self):
         array = self.array
         if not array:
             return 1
         n_cell_1_percentile = len(array) // 100
         sorted_counts = sorted(array, reverse=True)
         count_cell_1_percentile = sorted_counts[n_cell_1_percentile]
-        threshold = int(count_cell_1_percentile / 10)
+        threshold = int(count_cell_1_percentile / self.coef)
 
         return threshold
 
 
 class Threshold():
     """
     Args:
```

### Comparing `celescope-1.8.1/celescope/tools/__init__.py` & `celescope-1.9.0/celescope/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/mkref.py` & `celescope-1.9.0/celescope/tools/mkref.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/cutadapt.py` & `celescope-1.9.0/celescope/tools/cutadapt.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/debug.py` & `celescope-1.9.0/celescope/tools/debug.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/tools/step.py` & `celescope-1.9.0/celescope/tools/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
     def add_metric(self, name, value, total=None, help_info=None, display=None, show=True):
         '''
         add metric to metric_list
         
         Args
             display: controls how to display the metric in HTML report.
+            show: whether to add to .data.json, show the metric in HTML report and stat.txt.
         '''
 
         name = cap_str_except_preposition(name)
         if help_info:
             help_info = help_info[0].upper() + help_info[1:]
             if help_info[-1] != '.':
                 help_info += '.'
@@ -121,19 +122,20 @@
                 "show": show,
             }
         )
 
     def _write_stat(self):
         with open(self.__stat_file, 'w') as writer:
             for metric in self.__metric_list:
-                name = metric['name']
-                display = metric['display']
+                if metric['show']:
+                    name = metric['name']
+                    display = metric['display']
 
-                line = f'{name}: {display}'
-                writer.write(line + '\n')
+                    line = f'{name}: {display}'
+                    writer.write(line + '\n')
 
     def _dump_content(self):
         '''dump content to json file
         '''
         for slot, path in self._path_dict.items():
             if self.__content_dict[slot]:
                 with open(path, 'w') as f:
@@ -146,15 +148,19 @@
         with io.open(report_html, 'w', encoding='utf8') as f:
             html = template.render(self.__content_dict['data'])
             f.write(html)
 
     def _add_content_data(self):
         step_summary = {}
         step_summary['display_title'] = self._display_title
-        step_summary['metric_list'] = self.__metric_list
+        metric_list = []
+        for metric in self.__metric_list:
+            if metric['show']:
+                metric_list.append(metric)
+        step_summary['metric_list'] = metric_list
         step_summary['help_content'] = self.__help_content
         self.__content_dict['data'][self._step_summary_name].update(step_summary)
 
     def _add_content_metric(self):
         metric_dict = dict()
         for metric in self.__metric_list:
             name = metric['name']
@@ -216,14 +222,20 @@
     def debug_subprocess_call(self, cmd):
         '''
         debug subprocess call
         '''
         self.debug_subprocess_call.logger.debug(cmd)
         subprocess.check_call(cmd, shell=True)
 
+    def get_metric_list(self):
+        return self.__metric_list
+
+    def set_metric_list(self, metric_list):
+        self.__metric_list = metric_list
+
     @abc.abstractmethod
     def run(self):
         sys.exit('Please implement run() method.')
 
     def __enter__(self):
         return self
```

### Comparing `celescope-1.8.1/celescope/tools/multi.py` & `celescope-1.9.0/celescope/tools/multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,28 +171,28 @@
         """
         self.args = self.parser.parse_args()
 
         if self.args.gzip:
             self.fq_suffix = ".gz"
         if self.args.steps_run != 'all':
             self.steps_run = self.args.steps_run.strip().split(',')
+        
+        if self.args.mod == 'sjm':
 
-        self.sjm_dir = f'{self.args.outdir}/sjm/'
-        self.sjm_file = f'{self.sjm_dir}/sjm.job'
+            self.sjm_dir = f'{self.args.outdir}/sjm/'
+            utils.check_mkdir(self.sjm_dir)
+            self.logdir = self.args.outdir + '/log'
+            utils.check_mkdir(self.logdir)
 
-        self.logdir = self.args.outdir + '/log'
-        self.sjm_cmd = f'log_dir {self.logdir}\n'
+            self.sjm_file = f'{self.sjm_dir}/sjm.job'
+            self.sjm_cmd = f'log_dir {self.logdir}\n'
 
         # parse_mapfile
         self.fq_dict, self.col4_dict, self.col5_dict = self.parse_mapfile(self.args.mapfile, self.col4_default)
 
-        # mk dir
-        utils.check_mkdir(self.logdir)
-        utils.check_mkdir(self.sjm_dir)
-
         for sample in self.fq_dict:
             self.outdir_dic[sample] = {}
             index = 0
             for step in self.__STEPS__:
                 step_outdir = f"{self.args.outdir}/{sample}/{index:02d}.{step}"
                 self.outdir_dic[sample].update({step: step_outdir})
                 index += 1
```

### Comparing `celescope-1.8.1/celescope/tools/barcode.py` & `celescope-1.9.0/celescope/tools/barcode.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/vdj/count_vdj.py` & `celescope-1.9.0/celescope/vdj/count_vdj.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/vdj/multi_vdj.py` & `celescope-1.9.0/celescope/vdj/multi_vdj.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/vdj/mapping_vdj.py` & `celescope-1.9.0/celescope/vdj/mapping_vdj.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/HLA/hla_reference_rna.fasta` & `celescope-1.9.0/celescope/data/HLA/hla_reference_rna.fasta`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/rRNA/human_ribo.fasta` & `celescope-1.9.0/celescope/data/rRNA/human_ribo.fasta`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV2.1.1/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV2.1.1/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV2.2.1/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV2.2.1/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV2.0.1/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV2.0.1/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV3.0.1/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV3.0.1/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV2.1.0/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV2.1.0/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/data/chemistry/scopeV2.0.0/bclist` & `celescope-1.9.0/celescope/data/chemistry/scopeV2.0.0/bclist`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/capture_rna/multi_capture_rna.py` & `celescope-1.9.0/celescope/capture_rna/multi_capture_rna.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/capture_rna/count_capture_rna.py` & `celescope-1.9.0/celescope/capture_rna/count_capture_rna.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna_virus/analysis_rna_virus.py` & `celescope-1.9.0/celescope/rna_virus/analysis_rna_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna_virus/count_virus.py` & `celescope-1.9.0/celescope/rna_virus/count_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna_virus/star_virus.py` & `celescope-1.9.0/celescope/rna_virus/star_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/rna_virus/multi_rna_virus.py` & `celescope-1.9.0/celescope/rna_virus/multi_rna_virus.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/analysis_fusion.py` & `celescope-1.9.0/celescope/fusion/analysis_fusion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/multi_fusion.py` & `celescope-1.9.0/celescope/fusion/multi_fusion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/star_fusion.py` & `celescope-1.9.0/celescope/fusion/star_fusion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/plot_fusion.R` & `celescope-1.9.0/celescope/fusion/plot_fusion.R`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/count_fusion.py` & `celescope-1.9.0/celescope/fusion/count_fusion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/filter_fusion.py` & `celescope-1.9.0/celescope/fusion/filter_fusion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/fusion/mkref.py` & `celescope-1.9.0/celescope/fusion/mkref.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/conversion.py` & `celescope-1.9.0/celescope/dynaseq/conversion.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/replacement.py` & `celescope-1.9.0/celescope/dynaseq/replacement.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/Generate_T_C_matrix.R` & `celescope-1.9.0/celescope/dynaseq/Generate_T_C_matrix.R`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/replace_tsne.py` & `celescope-1.9.0/celescope/dynaseq/replace_tsne.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/substitution.py` & `celescope-1.9.0/celescope/dynaseq/substitution.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/dynaseq/multi_dynaseq.py` & `celescope-1.9.0/celescope/dynaseq/multi_dynaseq.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/celescope/scripts/gene_umi_summary.R` & `celescope-1.9.0/celescope/scripts/gene_umi_summary.R`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/setup.py` & `celescope-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/tests/test_function.py` & `celescope-1.9.0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/tests/conftest.py` & `celescope-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/tests/test_multi.py` & `celescope-1.9.0/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/tests/unittests/snp/test_snp.py` & `celescope-1.9.0/tests/unittests/snp/test_snp.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/tests/unittests/snp/test_variant_calling.py` & `celescope-1.9.0/tests/unittests/snp/test_variant_calling.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/PKG-INFO` & `celescope-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celescope
-Version: 1.8.1
+Version: 1.9.0
 Summary: Single Cell Analysis Pipelines
 Home-page: https://github.com/singleron-RD/CeleScope
 Author: zhouyiqi
 Author-email: zhouyiqi@singleronbio.com
 License: UNKNOWN
 Description: 
         # Introduction
```

### Comparing `celescope-1.8.1/README.md` & `celescope-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/scripts/extract_read.py` & `celescope-1.9.0/scripts/extract_read.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/scripts/add_tag.py` & `celescope-1.9.0/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/scripts/release_local.py` & `celescope-1.9.0/scripts/release_local.py`

 * *Files identical despite different names*

### Comparing `celescope-1.8.1/scripts/generate_docs.py` & `celescope-1.9.0/scripts/generate_docs.py`

 * *Files identical despite different names*

