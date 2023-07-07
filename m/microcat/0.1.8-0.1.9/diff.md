# Comparing `tmp/microcat-0.1.8.tar.gz` & `tmp/microcat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.8.tar", last modified: Thu Jul  6 07:49:20 2023, max compression
+gzip compressed data, was "microcat-0.1.9.tar", last modified: Fri Jul  7 07:53:38 2023, max compression
```

## Comparing `microcat-0.1.8.tar` & `microcat-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.302207 microcat-0.1.8/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-06 07:49:20.302207 microcat-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-06 07:49:18.000000 microcat-0.1.8/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.1.8/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-19 01:50:35.000000 microcat-0.1.8/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.8/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    34429 2023-07-06 07:45:55.000000 microcat-0.1.8/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.1.8/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.8/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.8/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.8/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.1.8/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.1.8/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.8/microcat/envs/trimming.yaml
--rwxr-xr-x   0 root         (0) root         (0)     5102 2023-07-06 06:34:24.000000 microcat-0.1.8/microcat/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.294207 microcat-0.1.8/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat/profiles/lsf/
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.8/microcat/profiles/lsf/CookieCutter.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/OSLayer.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/lsf_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/lsf_config.py
--rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/lsf_jobscript.sh
--rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/lsf_submit.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/profiles/lsf/memory_units.py
--rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.1.8/microcat/rich_agrpase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.8/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.8/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.1.8/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.8/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    74506 2023-07-06 06:41:05.000000 microcat-0.1.8/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.8/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.302207 microcat-0.1.8/microcat/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.8/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.1.8/microcat/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.1.8/microcat/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.8/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.1.8/microcat/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1214 2023-06-23 14:00:52.000000 microcat-0.1.8/microcat/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.1.8/microcat/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.8/microcat/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.8/microcat/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.1.8/microcat/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.1.8/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.1.8/microcat/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.8/microcat/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     1973 2023-06-24 01:45:21.000000 microcat-0.1.8/microcat/scripts/split_Starsolo_BAM_by_RG.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.302207 microcat-0.1.8/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.8/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1928 2023-06-24 02:40:05.000000 microcat-0.1.8/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)     8723 2023-07-02 16:16:54.000000 microcat-0.1.8/microcat/snakefiles/scRNA_wf_test.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.8/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:49:20.298207 microcat-0.1.8/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1810 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 07:49:20.000000 microcat-0.1.8/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 07:49:20.302207 microcat-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.673895 microcat-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-07 07:53:38.673895 microcat-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.669895 microcat-0.1.9/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-07 07:53:37.000000 microcat-0.1.9/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.1.9/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.669895 microcat-0.1.9/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-19 01:50:35.000000 microcat-0.1.9/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.9/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    34429 2023-07-06 07:45:55.000000 microcat-0.1.9/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.669895 microcat-0.1.9/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.1.9/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.9/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.9/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.9/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.9/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.1.9/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.1.9/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.9/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5102 2023-07-07 07:36:43.000000 microcat-0.1.9/microcat/prepare.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.1.9/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.669895 microcat-0.1.9/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.9/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.9/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.1.9/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.9/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    74506 2023-07-06 06:41:05.000000 microcat-0.1.9/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.9/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.673895 microcat-0.1.9/microcat/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.9/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.1.9/microcat/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.1.9/microcat/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.9/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.1.9/microcat/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-06-23 14:00:52.000000 microcat-0.1.9/microcat/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.9/microcat/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.1.9/microcat/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.9/microcat/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.9/microcat/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.1.9/microcat/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.1.9/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.1.9/microcat/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.9/microcat/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2023-06-24 01:45:21.000000 microcat-0.1.9/microcat/scripts/split_Starsolo_BAM_by_RG.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.673895 microcat-0.1.9/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.9/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-06-24 02:40:05.000000 microcat-0.1.9/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     8723 2023-07-02 16:16:54.000000 microcat-0.1.9/microcat/snakefiles/scRNA_wf_test.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.9/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:53:38.669895 microcat-0.1.9/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 07:53:38.000000 microcat-0.1.9/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 07:53:38.673895 microcat-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.9/setup.py
```

### Comparing `microcat-0.1.8/LICENSE` & `microcat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/PKG-INFO` & `microcat-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.8
+Version: 0.1.9
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.8/microcat/__init__.py` & `microcat-0.1.9/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/config/config.yaml` & `microcat-0.1.9/microcat/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/configer.py` & `microcat-0.1.9/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/corer.py` & `microcat-0.1.9/microcat/corer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/prepare.py` & `microcat-0.1.9/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rich_agrpase.py` & `microcat-0.1.9/microcat/rich_agrpase.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rules/ERCC.smk` & `microcat-0.1.9/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rules/build.smk` & `microcat-0.1.9/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rules/classfier.smk` & `microcat-0.1.9/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rules/database.smk` & `microcat-0.1.9/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/rules/host.smk` & `microcat-0.1.9/microcat/rules/host.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/sample.py` & `microcat-0.1.9/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/INVADEseq.py` & `microcat-0.1.9/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.1.9/microcat/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/create_hdf5.py` & `microcat-0.1.9/microcat/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/extract_kraken_reads.py` & `microcat-0.1.9/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/extract_microbiome_output.R` & `microcat-0.1.9/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/generate_PE_manifest_file.py` & `microcat-0.1.9/microcat/scripts/generate_PE_manifest_file.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/get_ncbi_domains.py` & `microcat-0.1.9/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/krak2_output_denosing.R` & `microcat-0.1.9/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/kraken2mpa.py` & `microcat-0.1.9/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/kraken2sc.py` & `microcat-0.1.9/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/microcat_bam_handle.Rmd` & `microcat-0.1.9/microcat/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/sample_denosing.R` & `microcat-0.1.9/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/sckmer_unpaired.R` & `microcat-0.1.9/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.1.9/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.1.9/microcat/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.1.9/microcat/snakefiles/scRNA_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat/snakefiles/scRNA_wf_test.smk` & `microcat-0.1.9/microcat/snakefiles/scRNA_wf_test.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.8/microcat.egg-info/PKG-INFO` & `microcat-0.1.9/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.8
+Version: 0.1.9
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.8/microcat.egg-info/SOURCES.txt` & `microcat-0.1.9/microcat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,14 @@
 microcat/envs/kmer_qc.yaml
 microcat/envs/kraken2.yaml
 microcat/envs/krakenuniq.yaml
 microcat/envs/metaphlan.yaml
 microcat/envs/pathseq.yaml
 microcat/envs/star.yaml
 microcat/envs/trimming.yaml
-microcat/profiles/lsf/CookieCutter.py
-microcat/profiles/lsf/OSLayer.py
-microcat/profiles/lsf/config.yaml
-microcat/profiles/lsf/lsf_cancel.py
-microcat/profiles/lsf/lsf_config.py
-microcat/profiles/lsf/lsf_jobscript.sh
-microcat/profiles/lsf/lsf_status.py
-microcat/profiles/lsf/lsf_submit.py
-microcat/profiles/lsf/memory_units.py
 microcat/rules/ERCC.smk
 microcat/rules/build.smk
 microcat/rules/classfier.smk
 microcat/rules/database.smk
 microcat/rules/host.smk
 microcat/scripts/INVADEseq.py
 microcat/scripts/add_tags_to_PathSeq_bam.py
```

### Comparing `microcat-0.1.8/setup.py` & `microcat-0.1.9/setup.py`

 * *Files identical despite different names*

