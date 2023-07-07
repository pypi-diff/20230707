# Comparing `tmp/iCount-Mini-2.0.3.tar.gz` & `tmp/iCount-Mini-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iCount-Mini-2.0.3.tar", last modified: Wed Jun  2 11:07:40 2021, max compression
+gzip compressed data, was "iCount-Mini-3.0.0.tar", last modified: Fri Jul  7 07:14:36 2023, max compression
```

## Comparing `iCount-Mini-2.0.3.tar` & `iCount-Mini-3.0.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.310101 iCount-Mini-2.0.3/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     9787 2021-05-19 09:10:16.000000 iCount-Mini-2.0.3/.pylintrc
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     7715 2021-05-19 09:10:16.000000 iCount-Mini-2.0.3/CLA
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2181 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/Dockerfile
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1580 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/Dockerfile_test
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1145 2021-06-01 11:14:23.000000 iCount-Mini-2.0.3/LICENSE
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      600 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/MANIFEST.in
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2838 2021-06-02 11:07:40.310350 iCount-Mini-2.0.3/PKG-INFO
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1964 2021-06-02 11:03:41.000000 iCount-Mini-2.0.3/README.md
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.250155 iCount-Mini-2.0.3/docs/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3267 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/Makefile
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      559 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/changelog.sh
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      200 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/pack_testupload.sh
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.262939 iCount-Mini-2.0.3/docs/source/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1302 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/cite.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     5836 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/docs/source/conf.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    10629 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/contributing.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      520 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/faq.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      240 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/index.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3071 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/installation.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       78 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/license.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       86 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/ref.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       99 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/ref_CLI.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    39639 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/ref_CLI.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      565 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/ref_python.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       55 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/revisions.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    12384 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/tutorial.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       92 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/source/versions.rst
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      230 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/docs/testdownload_install.sh
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.268116 iCount-Mini-2.0.3/iCount/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      836 2021-06-02 11:06:52.000000 iCount-Mini-2.0.3/iCount/__about__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2281 2021-06-01 16:00:33.000000 iCount-Mini-2.0.3/iCount/__init__.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.273622 iCount-Mini-2.0.3/iCount/analysis/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      636 2021-06-01 15:34:24.000000 iCount-Mini-2.0.3/iCount/analysis/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4092 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/analysis/annotate.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      346 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/analysis/group.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    40612 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/analysis/kmers.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4252 2021-06-01 15:34:24.000000 iCount-Mini-2.0.3/iCount/analysis/peaks.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    10205 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/analysis/rnamaps.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    22815 2021-06-01 15:34:24.000000 iCount-Mini-2.0.3/iCount/analysis/sigxls.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     5385 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/analysis/summary.py
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    18221 2021-06-01 15:34:24.000000 iCount-Mini-2.0.3/iCount/cli.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    11127 2021-05-19 09:50:35.000000 iCount-Mini-2.0.3/iCount/demultiplex.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.276611 iCount-Mini-2.0.3/iCount/examples/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1709 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/examples/__init__.py
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3310 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/examples/hnRNPC.sh
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3348 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/examples/hnRNPC_reduced.sh
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1962 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/examples/tutorial.sh
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.278319 iCount-Mini-2.0.3/iCount/externals/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      324 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/externals/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2941 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/externals/cutadapt.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     7465 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/externals/star.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.281195 iCount-Mini-2.0.3/iCount/files/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3781 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/files/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3591 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/files/bed.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3183 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/files/bedgraph.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      762 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/files/fasta.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3221 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/files/fastq.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.283521 iCount-Mini-2.0.3/iCount/genomes/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     5143 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/genomes/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    10859 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/genomes/ensembl.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     7089 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/genomes/gencode.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    40515 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/genomes/segment.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     6994 2021-05-19 09:50:35.000000 iCount-Mini-2.0.3/iCount/logger.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.286128 iCount-Mini-2.0.3/iCount/mapping/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      377 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/mapping/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      925 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/mapping/filters.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      197 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/mapping/indexstar.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      218 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/mapping/mapstar.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    22429 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/mapping/xlsites.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1558 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/iCount/metrics.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.287992 iCount-Mini-2.0.3/iCount/plotting/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      158 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/plotting/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2195 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/plotting/plot_combined.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     5427 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/plotting/plot_rnaheatmap.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4451 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/plotting/plot_rnamap.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.301389 iCount-Mini-2.0.3/iCount/tests/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       20 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/__init__.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.306005 iCount-Mini-2.0.3/iCount/tests/functional/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      367 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/__init__.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     9158 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/gtf_variations.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    29055 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3308 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/pipeline_examples.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      278 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/segments_count.out.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4366 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/functional/segments_count.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     6912 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_annotate.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2696 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_bed.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    16192 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_cli.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2580 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_clusters.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1081 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_data.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    14672 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_demultiplex.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     6815 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_e2e.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1012 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_examples.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4604 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_externals.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     9046 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_files.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    10194 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_genomes.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     4109 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_peaks.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     3652 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_plotting.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     9680 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_rnamaps.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    42560 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_segment.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     6056 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_summary.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    14112 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/test_xlsites.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)    11519 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/iCount/tests/utils.py
-drwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        0 2021-06-02 11:07:40.309663 iCount-Mini-2.0.3/iCount_Mini.egg-info/
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2838 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/PKG-INFO
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2561 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/SOURCES.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        1 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/dependency_links.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)       49 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/entry_points.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      266 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/requires.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)        7 2021-06-02 11:07:40.000000 iCount-Mini-2.0.3/iCount_Mini.egg-info/top_level.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      111 2021-05-19 09:10:17.000000 iCount-Mini-2.0.3/requirements-rtd.txt
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)      242 2021-06-02 11:07:40.311202 iCount-Mini-2.0.3/setup.cfg
--rwxr-xr-x   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     2546 2021-06-01 15:25:39.000000 iCount-Mini-2.0.3/setup.py
--rw-r--r--   0 jonesm5  (73768299) THECRICK\Domain Users (1934034978)     1108 2021-05-19 09:49:54.000000 iCount-Mini-2.0.3/tox.ini
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.134516 iCount-Mini-3.0.0/
+-rw-r--r--   0 capitac    (501) staff       (20)     9787 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/.pylintrc
+-rw-r--r--   0 capitac    (501) staff       (20)     7715 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/CLA
+-rw-r--r--   0 capitac    (501) staff       (20)     2181 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/Dockerfile
+-rw-r--r--   0 capitac    (501) staff       (20)     1580 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/Dockerfile_test
+-rw-r--r--   0 capitac    (501) staff       (20)     1145 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/LICENSE
+-rw-r--r--   0 capitac    (501) staff       (20)      600 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/MANIFEST.in
+-rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-07 07:14:36.134648 iCount-Mini-3.0.0/PKG-INFO
+-rw-r--r--   0 capitac    (501) staff       (20)     2484 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/README.md
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.890162 iCount-Mini-3.0.0/docs/
+-rw-r--r--   0 capitac    (501) staff       (20)     3267 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/Makefile
+-rwxr-xr-x   0 capitac    (501) staff       (20)      559 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/changelog.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)      200 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/pack_testupload.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.953925 iCount-Mini-3.0.0/docs/source/
+-rw-r--r--   0 capitac    (501) staff       (20)     1302 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/cite.rst
+-rw-r--r--   0 capitac    (501) staff       (20)     5836 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/conf.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10629 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/contributing.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      520 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/faq.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      240 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/index.rst
+-rw-r--r--   0 capitac    (501) staff       (20)     3071 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/installation.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       78 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/license.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       86 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       99 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref_CLI.rst
+-rw-r--r--   0 capitac    (501) staff       (20)    39672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/docs/source/ref_CLI.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      565 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/ref_python.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       55 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/revisions.rst
+-rw-r--r--   0 capitac    (501) staff       (20)    12384 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/tutorial.rst
+-rw-r--r--   0 capitac    (501) staff       (20)       92 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/source/versions.rst
+-rw-r--r--   0 capitac    (501) staff       (20)      230 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/docs/testdownload_install.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.969457 iCount-Mini-3.0.0/iCount/
+-rw-r--r--   0 capitac    (501) staff       (20)      836 2023-07-07 07:08:15.000000 iCount-Mini-3.0.0/iCount/__about__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2281 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/__init__.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:35.993350 iCount-Mini-3.0.0/iCount/analysis/
+-rw-r--r--   0 capitac    (501) staff       (20)      638 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/analysis/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4092 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/annotate.py
+-rw-r--r--   0 capitac    (501) staff       (20)      346 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/group.py
+-rw-r--r--   0 capitac    (501) staff       (20)    40612 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/kmers.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10210 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/analysis/metagene.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4252 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/peaks.py
+-rw-r--r--   0 capitac    (501) staff       (20)    22815 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/sigxls.py
+-rw-r--r--   0 capitac    (501) staff       (20)     5385 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/analysis/summary.py
+-rwxr-xr-x   0 capitac    (501) staff       (20)    18226 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/cli.py
+-rw-r--r--   0 capitac    (501) staff       (20)    11127 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/demultiplex.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.014030 iCount-Mini-3.0.0/iCount/examples/
+-rw-r--r--   0 capitac    (501) staff       (20)     1709 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/__init__.py
+-rwxr-xr-x   0 capitac    (501) staff       (20)     3310 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/hnRNPC.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)     3348 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/hnRNPC_reduced.sh
+-rwxr-xr-x   0 capitac    (501) staff       (20)     1962 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/examples/tutorial.sh
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.025751 iCount-Mini-3.0.0/iCount/externals/
+-rw-r--r--   0 capitac    (501) staff       (20)      324 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2941 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/cutadapt.py
+-rw-r--r--   0 capitac    (501) staff       (20)     7465 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/externals/star.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.038664 iCount-Mini-3.0.0/iCount/files/
+-rw-r--r--   0 capitac    (501) staff       (20)     3781 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3591 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/bed.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3183 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/bedgraph.py
+-rw-r--r--   0 capitac    (501) staff       (20)      762 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/fasta.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3221 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/files/fastq.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.049187 iCount-Mini-3.0.0/iCount/genomes/
+-rw-r--r--   0 capitac    (501) staff       (20)     5143 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10859 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/ensembl.py
+-rw-r--r--   0 capitac    (501) staff       (20)     7089 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/genomes/gencode.py
+-rw-r--r--   0 capitac    (501) staff       (20)    40516 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/genomes/segment.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6994 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/logger.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.058885 iCount-Mini-3.0.0/iCount/mapping/
+-rw-r--r--   0 capitac    (501) staff       (20)      377 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)      925 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/filters.py
+-rw-r--r--   0 capitac    (501) staff       (20)      197 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/indexstar.py
+-rw-r--r--   0 capitac    (501) staff       (20)      218 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/mapstar.py
+-rw-r--r--   0 capitac    (501) staff       (20)    22429 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/mapping/xlsites.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1558 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/metrics.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.067181 iCount-Mini-3.0.0/iCount/plotting/
+-rw-r--r--   0 capitac    (501) staff       (20)      160 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2204 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_combined.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4460 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_metagene.py
+-rw-r--r--   0 capitac    (501) staff       (20)     5435 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/plotting/plot_rnaheatmap.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.112433 iCount-Mini-3.0.0/iCount/tests/
+-rw-r--r--   0 capitac    (501) staff       (20)       20 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/__init__.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.126426 iCount-Mini-3.0.0/iCount/tests/functional/
+-rw-r--r--   0 capitac    (501) staff       (20)      367 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/__init__.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9158 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/gtf_variations.py
+-rw-r--r--   0 capitac    (501) staff       (20)    29055 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt
+-rw-r--r--   0 capitac    (501) staff       (20)     3308 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.py
+-rw-r--r--   0 capitac    (501) staff       (20)      278 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/segments_count.out.txt
+-rw-r--r--   0 capitac    (501) staff       (20)     4366 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/functional/segments_count.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6912 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_annotate.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2696 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_bed.py
+-rw-r--r--   0 capitac    (501) staff       (20)    16194 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_cli.py
+-rw-r--r--   0 capitac    (501) staff       (20)     2580 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_clusters.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1081 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_data.py
+-rw-r--r--   0 capitac    (501) staff       (20)    14672 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_demultiplex.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6817 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_e2e.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1012 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_examples.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4604 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_externals.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9046 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_files.py
+-rw-r--r--   0 capitac    (501) staff       (20)    10194 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_genomes.py
+-rw-r--r--   0 capitac    (501) staff       (20)     4109 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_peaks.py
+-rw-r--r--   0 capitac    (501) staff       (20)     3672 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_plotting.py
+-rw-r--r--   0 capitac    (501) staff       (20)     9700 2023-05-17 05:53:23.000000 iCount-Mini-3.0.0/iCount/tests/test_rnamaps.py
+-rw-r--r--   0 capitac    (501) staff       (20)    42560 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_segment.py
+-rw-r--r--   0 capitac    (501) staff       (20)     6056 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_summary.py
+-rw-r--r--   0 capitac    (501) staff       (20)    14112 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/test_xlsites.py
+-rw-r--r--   0 capitac    (501) staff       (20)    11519 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/iCount/tests/utils.py
+drwxr-xr-x   0 capitac    (501) staff       (20)        0 2023-07-07 07:14:36.134316 iCount-Mini-3.0.0/iCount_Mini.egg-info/
+-rw-r--r--   0 capitac    (501) staff       (20)     3338 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/PKG-INFO
+-rw-r--r--   0 capitac    (501) staff       (20)     2564 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/SOURCES.txt
+-rw-r--r--   0 capitac    (501) staff       (20)        1 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/dependency_links.txt
+-rw-r--r--   0 capitac    (501) staff       (20)       48 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/entry_points.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      266 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/requires.txt
+-rw-r--r--   0 capitac    (501) staff       (20)        7 2023-07-07 07:14:35.000000 iCount-Mini-3.0.0/iCount_Mini.egg-info/top_level.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      111 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/requirements-rtd.txt
+-rw-r--r--   0 capitac    (501) staff       (20)      242 2023-07-07 07:14:36.136873 iCount-Mini-3.0.0/setup.cfg
+-rwxr-xr-x   0 capitac    (501) staff       (20)     2546 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/setup.py
+-rw-r--r--   0 capitac    (501) staff       (20)     1108 2023-05-15 06:53:41.000000 iCount-Mini-3.0.0/tox.ini
```

### Comparing `iCount-Mini-2.0.3/.pylintrc` & `iCount-Mini-3.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/CLA` & `iCount-Mini-3.0.0/CLA`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/Dockerfile` & `iCount-Mini-3.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/Dockerfile_test` & `iCount-Mini-3.0.0/Dockerfile_test`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/LICENSE` & `iCount-Mini-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/MANIFEST.in` & `iCount-Mini-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/PKG-INFO` & `iCount-Mini-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: iCount-Mini
-Version: 2.0.3
+Version: 3.0.0
 Summary: Computational pipeline for analysis of iCLIP data
 Home-page: https://github.com/ulelab/iCount-Mini
 Author: Ule Group, The Francis Crick Institute, London
 Author-email: jernej.ule@crick.ac.uk
 License: MIT
 Keywords: iCLIP protein-RNA
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -23,25 +22,32 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # iCount-Mini
 
 This is a fork of iCount maintained by members of [Jernej Ule's](http://ulelab.info) group, focussing on the peak calling features of iCount.
 
+Run commands using:
+`iCount-Mini <command>`
+
+**Note on small differences of terminology between iCount-Mini and iCount**
++ In iCount-Mini, sigxls = iCount peaks and iCount-Mini peaks = iCount clusters. This is to bring the terminology more in line with the rest of the field.
++ In iCount-Mini RNA-maps have been renamed to 'metagene', to distinguish these plots which include only CLIP data from other RNA-maps which group crosslinks into categories dependent on orthogonal data, such as alternatively spliced exons.
+
 # iCount: protein-RNA interaction analysis
 
 iCount is a Python module and associated command-line interface (CLI), which provides all the commands needed to process iCLIP data on protein-RNA interactions and generate:
  
 + demultiplexed and adapter-trimmed FASTQ files
 + BAM files with mapped iCLIP reads
 + identified protein-RNA cross-linked sites, saved to BED files
 + statistically significant cross-linked sites, saved to BED files
 + peaks of significant cross-linked sites, saved to BED files
 + grouping of individual replicate experiments
-+ RNAmap generation showing the positional distribution of cross-linked sites relative to genomic landmarks
++ metagene generation showing the positional distribution of cross-linked sites relative to genomic landmarks
 + kmer enrichment analysis
 
 You may start with the [tutorial](http://icount.readthedocs.io/en/latest/tutorial.html) or dive into the 
 [documentation](http://icount.readthedocs.io/en/latest/index.html).
 
 ## iCount-Mini Authors
 
@@ -58,9 +64,7 @@
 
 To install a development version of iCount-Mini, use this command.
 It's recommended to do this within a Python virtual environment.
 
 ```bash
 pip install --upgrade -r requirements-rtd.txt -e .
 ```
-
-
```

### Comparing `iCount-Mini-2.0.3/README.md` & `iCount-Mini-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # iCount-Mini
 
 This is a fork of iCount maintained by members of [Jernej Ule's](http://ulelab.info) group, focussing on the peak calling features of iCount.
 
+Run commands using:
+`iCount-Mini <command>`
+
+**Note on small differences of terminology between iCount-Mini and iCount**
++ In iCount-Mini, sigxls = iCount peaks and iCount-Mini peaks = iCount clusters. This is to bring the terminology more in line with the rest of the field.
++ In iCount-Mini RNA-maps have been renamed to 'metagene', to distinguish these plots which include only CLIP data from other RNA-maps which group crosslinks into categories dependent on orthogonal data, such as alternatively spliced exons.
+
 # iCount: protein-RNA interaction analysis
 
 iCount is a Python module and associated command-line interface (CLI), which provides all the commands needed to process iCLIP data on protein-RNA interactions and generate:
  
 + demultiplexed and adapter-trimmed FASTQ files
 + BAM files with mapped iCLIP reads
 + identified protein-RNA cross-linked sites, saved to BED files
 + statistically significant cross-linked sites, saved to BED files
 + peaks of significant cross-linked sites, saved to BED files
 + grouping of individual replicate experiments
-+ RNAmap generation showing the positional distribution of cross-linked sites relative to genomic landmarks
++ metagene generation showing the positional distribution of cross-linked sites relative to genomic landmarks
 + kmer enrichment analysis
 
 You may start with the [tutorial](http://icount.readthedocs.io/en/latest/tutorial.html) or dive into the 
 [documentation](http://icount.readthedocs.io/en/latest/index.html).
 
 ## iCount-Mini Authors
```

### Comparing `iCount-Mini-2.0.3/docs/Makefile` & `iCount-Mini-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/changelog.sh` & `iCount-Mini-3.0.0/docs/changelog.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/cite.rst` & `iCount-Mini-3.0.0/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/conf.py` & `iCount-Mini-3.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/contributing.rst` & `iCount-Mini-3.0.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/faq.rst` & `iCount-Mini-3.0.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/installation.rst` & `iCount-Mini-3.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/ref_CLI.txt` & `iCount-Mini-3.0.0/docs/source/ref_CLI.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     segment      Parse annotation file into internal iCount structure - segmentation.
     demultiplex  Split FASTQ file into separate files, one for each sample barcode.
     cutadapt     Remove adapter sequences from reads in FASTQ file.
     indexstar    Generate STAR genome index.
     mapstar      Map reads to genome with STAR.
     xlsites      Quantity cross-link events and determine their positions.
     annotate     Annotate each cross link site with types of regions that intersect with it.
-    clusters     Merge adjacent peaks into clusters and sum cross-links within clusters.
+    peaks        Merge adjacent sigxls into peaks and sum cross-links within peaks.
     group        Merge multiple BED files with crosslinks into one.
-    peaks        Find positions with high density of cross-linked sites.
-    rnamaps      Distribution of cross-links relative to genomic landmarks.
+    sigxls       Find positions with high density of cross-linked sites.
+    metagene     Distribution of cross-links relative to genomic landmarks.
     summary      Report proportion of cross-link events/sites on each region type.
     examples     Provide a set of example bash scripts.
     man          Print help for all commands.
     args         Print arguments form all CLI commands.
 
 
 releases
@@ -624,36 +624,36 @@
                         Report analysis progress (default: False)
   -S , --stdout_log     Threshold value (0-50) for logging to stdout. If 0, logging to stdout if turned OFF.
   -F , --file_log       Threshold value (0-50) for logging to file. If 0, logging to file if turned OFF.
   -P , --file_logpath   Path to log file.
   -M , --results_file   File into which to store Metrics.
 
 
-rnamaps
+metagene
 =======
 
-usage: iCount rnamaps [-h] [--implicit_handling] [-mis] [--mapq_th]
+usage: iCount metagene [-h] [--implicit_handling] [-mis] [--mapq_th]
                       [--holesize_th] [-S] [-F] [-P] [-M]
                       bam segmentation out_file strange cross_transcript
 
 Distribution of cross-links relative to genomic landmarks.
 
-What is an RNA-map?
+What is a metagene?
 ^^^^^^^^^^^^^^^^^^^
 
 Imagine the following situation (on positive strand)::
 
     |---intron1---||---exon2---||---intron2---||---exon3---|
                               x|-----R1-----|
 
 Situation is simple: a read perfectly maps to reference genome. First cross-link
 (nucletide before the start of read R1) is located 2 nucleotides before
 landmark of type 'exon-intron'. By examining all cross-links(reads) that are
 located in vicinity of landmarks one can obtain the distribution of
-cross-link-to-landmark distances. Such distibution is called an RNA map.
+cross-link-to-landmark distances. Such distibution is called a metagene.
 
 Of course, situation gets complicated. Real-world-situation more likely looks
 like this::
 
     |--------transcript1-------|
     |-ncRNA-||-intron-||-ncRNA-|
             |------------------transcript2-----------------|
@@ -665,51 +665,51 @@
              x|R2.1->          <--R2.2-|
                                 x|-R3-|
 
 All sort of situations can arise:
 
     * read can intersect with multiple genes/transcripts/segments
       simultaneously, which means that one read is relevant for different types
-      of RNA maps.
+      of metagene.
     * if whole read is mapped to one segment (as is read R3 on transcript2),
-      then it is impossible to tell the type of RNA map it belongs to: is it
+      then it is impossible to tell the type of metagene it belongs to: is it
       CDS-intron or intron-CDS?
     * read can be mapped in multiple parts - for example when introns are
       removed before translation, first half of read will map to ``exon1`` and
       second half to ``exon2``.
     * same cross-link event can be represented by multiple reads with same
       random barcode.
     * ...
 
 The algorithm takes care for all of this, as explained below. It outputs a file,
 that looks like this::
 
-    rna_map_type    position    all     explicit
+    metagene_type    position    all     explicit
     exon-intron     42          13      14
     exon-intron     43          123     19
     exon-intron     44          56      16
     ....
     intron-CDS      23474       34      2
     intron-CDS      23475       85      65
     intron-CDS      23476       92      1
     ...
 
-Each line consits of four columns: RNA map type, position, all and explicit. RNA
+Each line consits of four columns: metagene type, position, all and explicit. RNA
 map type defines the landmark type, while position defines relative distance of
 cross-links to this landmark. All and explicit are counting number of crosslinks
-that are ``positions`` away from landmark of type RNA map type. Cross link is
-explicit, if read identifying cross-link is mapped to both parts of RNA-map. In
-upper example, R1 is explicit, since it maps to intron *and* exon. Read R3 on
-transcript2 is implicit, since one has to decide wheather it's cross-link
-belongs to ``CDS-intron`` or ``intron-CDS`` RNA map. The term *all* means
+that are ``positions`` away from landmark of type metagene type. Cross link is
+explicit, if the read identifying the cross-link is mapped to both parts of the metagene.
+In the upper example, R1 is explicit, since it maps to intron *and* exon. Read R3 
+on transcript2 is implicit, since one has to decide wheather it's cross-link
+belongs to ``CDS-intron`` or ``intron-CDS`` metagene. The term *all* means
 explicit + implicit in this context.
 
 If read is implicit (start and stop within same segment), one can choose two
 varinats of the algorithm. One option is that whole score of read is given to
-RNA-map of the *closest* landmark. Other option is to *split* score on half to
+metagene of the *closest* landmark. Other option is to *split* score on half to
 both neighbouring segments. This behaviour is controlled by parameter
 implicit_handling.
 
 There are also two cases when a read can map in a way that is not predicted by
 annotation:
 
     * For split reads, second start can fall on nucleotide that is not start of
@@ -726,54 +726,54 @@
         * for each ss_group, take annotation from reverse strand and check what
           is the situation on other side.
         * What si again the bio-contxt here - explain in docs...?
     * Test: Each cross-link should have the same cDNA count as in xlsites
       results. The final check should be: sum all scores - the result should be
       the same as for xlsites. Actually, the metrics.cross_transcript should
       also be considered:
-      assert: sum(xlsites scores) == sum(RNAmaps "all" + metrics.cross_transc)
+      assert: sum(xlsites scores) == sum(metagene "all" + metrics.cross_transc)
     * if read crosses two ore more regions from start to end, only end-type is
-      considered for RNAmap type. Should we fix this and which region type to
+      considered for metagene type. Should we fix this and which region type to
       take? Since reads are tpyically much shorted than regions, this is
       probably a rare case.
 
 -------------------------------------------------------------------------------
 
 Wishes and ideas(Jernej, Tomaz):
 
     * The whole idea is to get a feeling what is happening around landmarks
 
     * separate pre-mRNA and mRNA [this is partially done in _add_entry]
         * Life cyle of RNA: part of DNA in transcribed to RNA in nucleus. Introns
           are cut out already between this process! Really???
         * pre-mRNA contains introns, mature mRNA has no introns and goes outside
           from the nucleus.
-        * so: RNAmap exon-intron will for sure contain only pre-mRNA, but RNAmap
+        * so: metagene exon-intron will for sure contain only pre-mRNA, but metagene
           exon-exon can contain pre-mRNA and mRNA... It would be really nice to
           report on percentage of theese two categories.
         * This can be done by introducing three categories:  pre-mRNa, mRNA and
           undecided. This can be determined from results - they contain explicit /
-          implicit info and RNAmap type:
+          implicit info and metagene type:
 
-    * Intoduce three categories (colors in visualisation?) in every RNAmap type.
+    * Intoduce three categories (colors in visualisation?) in every metagene type.
       Let's take exon-intron as example:
 
         * whole read in left part - color #1 (negative coord, implicit)
         * whole read in right part - color #2 (positive coord, implicit)
         * read crossing junction - color #3 (explicit)
 
     * How to handle situation when one region in individual's sequence clearly
       differs from reference sequence but it is just some variation?
 
         * Change the reference sequence? This can be complex... Make a helper
           tool for this?
         * Provide additional data in function - which exceptions /abnormalities
           to ignore?
 
-    * Gaussian smooting of RNAmaps?
+    * Gaussian smooting of metagene?
 
     * split read - it can differ also on "first-stop", not juts second-start
         * we could have some sort of quality check when observing the variance
           of first-stop-s. THe major question is: "Do all reads for certain
           xlink event indicate the same behaviour?"
 
 positional arguments:
```

### Comparing `iCount-Mini-2.0.3/docs/source/ref_python.rst` & `iCount-Mini-3.0.0/docs/source/ref_python.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/docs/source/tutorial.rst` & `iCount-Mini-3.0.0/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/__about__.py` & `iCount-Mini-3.0.0/iCount/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #       interfere with a global variable __name__ denoting object's name.
 __title__ = 'iCount-Mini'
 __summary__ = 'Computational pipeline for analysis of iCLIP data'
 __url__ = 'https://github.com/ulelab/iCount-Mini'
 
 # Semantic versioning is used. For more information see:
 # https://packaging.python.org/en/latest/distributing/#semantic-versioning-preferred
-__version__ = '2.0.3'
+__version__ = '3.0.0'
 
 __author__ = 'Ule Group, The Francis Crick Institute, London'
 __email__ = 'jernej.ule@crick.ac.uk'
 
 __license__ = 'MIT'
 __copyright__ = '2016-2017, University of Ljubljana, Bioinformatics Laboratory'
```

### Comparing `iCount-Mini-2.0.3/iCount/__init__.py` & `iCount-Mini-3.0.0/iCount/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/analysis/__init__.py` & `iCount-Mini-3.0.0/iCount/analysis/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 .. automodule:: iCount.analysis.peaks
    :members:
 
 .. automodule:: iCount.analysis.kmers
    :members:
 
-.. automodule:: iCount.analysis.rnamaps
+.. automodule:: iCount.analysis.metagene
    :members:
 
 .. automodule:: iCount.analysis.annotate
    :members:
 
 .. automodule:: iCount.analysis.summary
    :members:
@@ -29,9 +29,9 @@
 """
 
 from . import annotate
 from . import peaks
 from . import group
 from . import kmers
 from . import sigxls
-from . import rnamaps
+from . import metagene
 from . import summary
```

### Comparing `iCount-Mini-2.0.3/iCount/analysis/annotate.py` & `iCount-Mini-3.0.0/iCount/analysis/annotate.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/analysis/kmers.py` & `iCount-Mini-3.0.0/iCount/analysis/kmers.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/analysis/peaks.py` & `iCount-Mini-3.0.0/iCount/analysis/peaks.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/analysis/rnamaps.py` & `iCount-Mini-3.0.0/iCount/analysis/metagene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """.. Line to protect from pydocstyle D205, D400.
 
-RNA maps
+Metagene
 --------
 
-Perform RNA-maps analysis.
+Perform metagene analysis.
 """
 import csv
 import logging
 import os
 
 import pandas as pd
 from pybedtools import BedTool, create_interval_from_list
@@ -186,16 +186,16 @@
     data = {}
     up_limit = -max([mtyp['upstream-size-limit'] for mtyp in MAP_TYPES.values()])
     down_limit = max([mtyp['downstream-size-limit'] for mtyp in MAP_TYPES.values()])
     header = list(range(up_limit, down_limit + 1))
 
     for basename in [file_ for file_ in os.listdir(outdir) if file_.endswith('.tsv')]:
         results_file = os.path.join(outdir, basename)
-        maptype = iCount.plotting.plot_rnamap.guess_maptype(results_file)
-        plot_data, _ = iCount.plotting.plot_rnamap.parse_results(results_file)
+        maptype = iCount.plotting.plot_metagene.guess_maptype(results_file)
+        plot_data, _ = iCount.plotting.plot_metagene.parse_results(results_file)
 
         # Make date of the same size, impute with 0 score on locations with no data.
         data[maptype] = [plot_data.get(pos, 0) for pos in header]
         assert len(header) == len(data[maptype])
 
     dframe = pd.DataFrame.from_dict(data, orient='index', columns=header)
     dframe.to_csv(fname, sep='\t')
@@ -240,15 +240,15 @@
     None
 
     """
     iCount.logger.log_inputs(LOGGER)
 
     sites_name = iCount.files.remove_extension(sites, ['.bed', '.bed.gz'])
     if outdir is None:
-        outdir = os.path.join(os.path.abspath(os.getcwd()), 'rnamaps_{}'.format(sites_name))
+        outdir = os.path.join(os.path.abspath(os.getcwd()), 'metagene_{}'.format(sites_name))
         LOGGER.info('Output directory not given, creating one at %s', outdir)
     os.makedirs(outdir, exist_ok=True)
 
     for maptype in MAP_TYPES:
         LOGGER.info('Creating landmarks for %s', maptype)
         landmarks = make_landmarks_file(regions, maptype)
         if not BedTool(landmarks).head(n=1, as_string=True):
@@ -274,12 +274,12 @@
             top_n=top_n,
             smoothing=smoothing,
             nbins=nbins,
             binsize=binsize,
             colormap=colormap,
         )
 
-    # Single file with only RNA-maps distibution plot data.
+    # Single file with only metagene distibution plot data.
     results_summarised_file = os.path.join(outdir, '{}_plot_data.tsv'.format(sites_name))
     make_results_summarised_file(outdir, results_summarised_file)
 
     LOGGER.info('Done.')
```

### Comparing `iCount-Mini-2.0.3/iCount/analysis/sigxls.py` & `iCount-Mini-3.0.0/iCount/analysis/sigxls.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/analysis/summary.py` & `iCount-Mini-3.0.0/iCount/analysis/summary.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/cli.py` & `iCount-Mini-3.0.0/iCount/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,21 +359,21 @@
     make_parser_from_function(
         iCount.analysis.peaks.run, subparsers)
     make_parser_from_function(
         iCount.analysis.group.run, subparsers, module=iCount.analysis.group)
     make_parser_from_function(
         iCount.analysis.sigxls.run, subparsers)
     make_parser_from_function(
-        iCount.analysis.rnamaps.run, subparsers)
+        iCount.analysis.metagene.run, subparsers)
     make_parser_from_function(
         iCount.analysis.summary.summary_reports, subparsers)
 
     # Plotting:
     make_parser_from_function(
-        iCount.plotting.plot_rnamap.plot_rnamap, subparsers)
+        iCount.plotting.plot_metagene.plot_metagene, subparsers)
     make_parser_from_function(
         iCount.plotting.plot_rnaheatmap.plot_rnaheatmap, subparsers)
     make_parser_from_function(
         iCount.plotting.plot_combined.plot_combined, subparsers)
 
     # File converters:
     make_parser_from_function(iCount.files.bedgraph.bed2bedgraph, subparsers)
```

### Comparing `iCount-Mini-2.0.3/iCount/demultiplex.py` & `iCount-Mini-3.0.0/iCount/demultiplex.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/examples/__init__.py` & `iCount-Mini-3.0.0/iCount/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/examples/hnRNPC.sh` & `iCount-Mini-3.0.0/iCount/examples/hnRNPC.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/examples/hnRNPC_reduced.sh` & `iCount-Mini-3.0.0/iCount/examples/hnRNPC_reduced.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/examples/tutorial.sh` & `iCount-Mini-3.0.0/iCount/examples/tutorial.sh`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/externals/cutadapt.py` & `iCount-Mini-3.0.0/iCount/externals/cutadapt.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/externals/star.py` & `iCount-Mini-3.0.0/iCount/externals/star.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/files/__init__.py` & `iCount-Mini-3.0.0/iCount/files/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/files/bed.py` & `iCount-Mini-3.0.0/iCount/files/bed.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/files/bedgraph.py` & `iCount-Mini-3.0.0/iCount/files/bedgraph.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/files/fasta.py` & `iCount-Mini-3.0.0/iCount/files/fasta.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/files/fastq.py` & `iCount-Mini-3.0.0/iCount/files/fastq.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/genomes/__init__.py` & `iCount-Mini-3.0.0/iCount/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/genomes/ensembl.py` & `iCount-Mini-3.0.0/iCount/genomes/ensembl.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/genomes/gencode.py` & `iCount-Mini-3.0.0/iCount/genomes/gencode.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/genomes/segment.py` & `iCount-Mini-3.0.0/iCount/genomes/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1055,15 +1055,15 @@
             gene_id#2: {},
             ...
         }
 
     Note that intergenic segments have multiple roles: the same intergenic
     segment has the role of gene, transcript and sub-transcript segment. This
     eases the treatment of intergenic intervals in algorithms that use this
-    function (rnamaps, xlsites, ...)
+    function (metagene, xlsites, ...)
 
     Parameters
     ----------
     seg_file : str
         Path to GTF file, produces by ``get_segments`` function.
 
     Returns
```

### Comparing `iCount-Mini-2.0.3/iCount/logger.py` & `iCount-Mini-3.0.0/iCount/logger.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/mapping/filters.py` & `iCount-Mini-3.0.0/iCount/mapping/filters.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/mapping/xlsites.py` & `iCount-Mini-3.0.0/iCount/mapping/xlsites.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/metrics.py` & `iCount-Mini-3.0.0/iCount/metrics.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/plotting/plot_combined.py` & `iCount-Mini-3.0.0/iCount/plotting/plot_combined.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """.. Line to protect from pydocstyle D205, D400.
 
-Plot combined (distribution & heatmap) RNA-map
+Plot combined (distribution & heatmap) metagene
 ----------------------------------------------
 
-Plot combined (distribution & heatmap) RNA-map.
+Plot combined (distribution & heatmap) metagene.
 """
-from . import plot_rnaheatmap, plot_rnamap
+from . import plot_rnaheatmap, plot_metagene
 
 # pylint: disable=wrong-import-order
 import matplotlib
 # Force matplotlib to not use any Xwindows backend.
 matplotlib.use('Agg')
 from matplotlib import pyplot as plt  # pylint: disable=wrong-import-position
 # pylint: enable=wrong-import-order
@@ -22,20 +22,20 @@
                   top_n=100,
                   smoothing=1,
                   nbins=50,
                   binsize=None,
                   colormap='Greys',
                   ):
     """
-    Plot combined (distribution & heatmap) RNA-map.
+    Plot combined (distribution & heatmap) metagene.
 
     Parameters
     ----------
     fname : str
-        RNA-maps result file to plot.
+        Metagene result file to plot.
     outfile : str
         Output file.
     up_limit : int
         Upstream plot limit.
     down_limit : int
         Sownstream plot limit.
     top_n : int
@@ -56,15 +56,15 @@
     """
     fig = plt.figure(figsize=(9, 16))
     gridspec = fig.add_gridspec(2, 1, height_ratios=[1, 4])
 
     distribution = fig.add_subplot(gridspec[0])
     hist = fig.add_subplot(gridspec[1])
 
-    plot_rnamap.plot_rnamap(
+    plot_metagene.plot_metagene(
         fname,
         outfile=None,
         up_limit=up_limit,
         down_limit=down_limit,
         ax=distribution,
         smoothing=smoothing,
     )
```

### Comparing `iCount-Mini-2.0.3/iCount/plotting/plot_rnaheatmap.py` & `iCount-Mini-3.0.0/iCount/plotting/plot_rnaheatmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """.. Line to protect from pydocstyle D205, D400.
 
-Plot heatmap RNA-map
+Plot heatmap Metagene
 --------------------
 
 Plot heatmap for most covered landmarks.
 """
 import csv
 
 import numpy as np
 import pandas as pd
 
-from . import plot_rnamap
+from . import plot_metagene
 
 # pylint: disable=wrong-import-order
 import matplotlib
 # Force matplotlib to not use any Xwindows backend.
 matplotlib.use('Agg')
 from matplotlib import pyplot as plt  # pylint: disable=wrong-import-position
 # pylint: enable=wrong-import-order
@@ -33,26 +33,26 @@
             position_to_bin[pos] = bin_start
 
     return position_to_bin
 
 
 def get_top_n_landmarks(fname, top_n, up_limit, down_limit):
     """Get top_n covered landmarks."""
-    df, total_cdna = plot_rnamap.parse_results_basic(fname)
+    df, total_cdna = plot_metagene.parse_results_basic(fname)
 
     # Create a "sum" column, by which one can sort most covered landmarks.
     df["Sum"] = df.sum(axis=1)
     # Sort and take only top_n covered landmarks. Take index and cast to list.
     top_n_landmarks = df.sort_values(by='Sum', ascending=False).iloc[:top_n].index.tolist()
 
     return top_n_landmarks, total_cdna
 
 
 def parse_results(fname, up_limit, down_limit, top_n, nbins=None, binsize=None):
-    """Parse RNA-maps results file."""
+    """Parse Metagene results file."""
     # Determine bins.
     if nbins is None and binsize is None:
         raise ValueError('Please define ``binsize`` or ``nbins``.')
     elif nbins and binsize:
         raise ValueError('Either ``binsize`` or ``nbins`` can be defined, but not both.')
     elif nbins:
         nbins = int(nbins)
@@ -87,15 +87,15 @@
             for pos, score in zip(header[1:], row[1:]):
                 pos, score = int(pos), int(score)
                 if up_limit <= pos <= down_limit:
                     bin_ = position_to_bin[pos]
                     data.at[landmark_name, bin_] = data.at[landmark_name, bin_] + score
 
     # Perform CPM ormalizaton
-    data = data.apply(plot_rnamap.normalize_cpm, args=(total_cdna,))
+    data = data.apply(plot_metagene.normalize_cpm, args=(total_cdna,))
 
     return data
 
 
 def plot_rnaheatmap(fname,
                     outfile=None,
                     up_limit=100,
@@ -103,20 +103,20 @@
                     top_n=100,
                     ax=None,
                     binsize=None,
                     nbins=None,
                     colormap='Greys',
                     ):
     """
-    Plot RNA-map heatmap.
+    Plot Metagene heatmap.
 
     Parameters
     ----------
     fname : str
-        RNA-maps result file to plot.
+        Metagene result file to plot.
     outfile : str
         Output file.
     up_limit : int
         Upstream plot limit.
     down_limit : int
         Sownstream plot limit.
     top_n : int
```

### Comparing `iCount-Mini-2.0.3/iCount/plotting/plot_rnamap.py` & `iCount-Mini-3.0.0/iCount/plotting/plot_metagene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """.. Line to protect from pydocstyle D205, D400.
 
-Plot distribution RNA-map
+Plot distribution Metagene
 -------------------------
 
 Plot distribution of crosslinks relative to landmark of specific type.
 """
 import os
 
 import pandas as pd
@@ -21,26 +21,26 @@
 
 def normalize_cpm(value, total):
     """Normalize by CPM."""
     return value / total * 10**6
 
 
 def parse_results_basic(fname):
-    """Parse RNA-maps results file."""
+    """Parse Metagene results file."""
     # First read total cdna info:
     with open(fname, 'rt') as handle:
         total_cdna_line = handle.readline()
         total_cdna = int(total_cdna_line.strip().split(':')[1])
 
     df = pd.read_csv(fname, delimiter='\t', header=1, index_col=0)
     return df, total_cdna
 
 
 def parse_results(fname):
-    """Parse RNA-maps results file."""
+    """Parse Metagene results file."""
     df, total_cdna = parse_results_basic(fname)
     landmark_count = len(df)
     distro = df.sum(axis=0)
 
     # Perform CPM normalization
     normalized_data = {int(pos): normalize_cpm(score, total_cdna) for pos, score in distro.to_dict().items()}
 
@@ -61,37 +61,37 @@
     """Make output filename."""
     basename = iCount.files.remove_extension(fname, ['.tsv'])
     dirname = os.path.dirname(fname)
     return os.path.join(dirname, '{}_distro.{}'.format(basename, imgfmt))
 
 
 def guess_maptype(fname):
-    """Try to get RNA maptype from filename."""
+    """Try to get metagene type from filename."""
     # Since "noncoding-gene-start" can be mistaken for "gene-start" check longest names first.
-    for mtype in sorted(iCount.analysis.rnamaps.MAP_TYPES.keys(), key=len, reverse=True):
+    for mtype in sorted(iCount.analysis.metagene.MAP_TYPES.keys(), key=len, reverse=True):
         if fname.endswith('{}.tsv'.format(mtype)):
             return mtype
 
 
-def plot_rnamap(fnames,
+def plot_metagene(fnames,
                 outfile=None,
                 up_limit=100,
                 down_limit=100,
                 ax=None,
                 ylim=None,
                 imgfmt='png',
                 smoothing=1,
                 ):
     """
-    Plot distribution RNA-map.
+    Plot distribution Metagene.
 
     Parameters
     ----------
     fnames : list_str
-        List of rnamaps result files to plot.
+        List of metagene result files to plot.
     outfile : str
         Output file.
     up_limit : int
         Upstream plot limit.
     down_limit : int
         Downstream plot limit.
     ax : str
@@ -144,13 +144,13 @@
         ax.plot(positions, smooth(scores, smoothing), label=label)
 
     ax.set_xlim((up_limit, down_limit))
     ax.set_xlabel('Position')
     if ylim:
         ax.set_ylim((0, ylim))
     ax.set_ylabel('Score [CPM]')
-    ax.set_title('RNA-map')
+    ax.set_title('Metagene')
     ax.grid(b=True, which='major', axis='both')
     ax.legend()
 
     if is_independent:
         fig.savefig(outfile)
```

### Comparing `iCount-Mini-2.0.3/iCount/tests/functional/gtf_variations.py` & `iCount-Mini-3.0.0/iCount/tests/functional/gtf_variations.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt` & `iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.hnRNPC_reduced.sh.out.txt`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/functional/pipeline_examples.py` & `iCount-Mini-3.0.0/iCount/tests/functional/pipeline_examples.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/functional/segments_count.py` & `iCount-Mini-3.0.0/iCount/tests/functional/segments_count.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_annotate.py` & `iCount-Mini-3.0.0/iCount/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_bed.py` & `iCount-Mini-3.0.0/iCount/tests/test_bed.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_cli.py` & `iCount-Mini-3.0.0/iCount/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
             '--report_progress',
             '-S', '40',  # Supress lower than ERROR messages.
         ]
 
         self.assertEqual(subprocess.call(command_basic), 0)
         self.assertEqual(subprocess.call(command_full), 0)
 
-    def test_rnamaps(self):
+    def test_metagene(self):
         regions = make_file_from_list([
             ['1', '.', 'intergenic', '1', '100', '.', '+', '.', ''],
             ['1', '.', 'intergenic', '1', '610', '.', '-', '.', ''],
             ['1', '.', 'UTR5', '101', '160', '.', '+', '.', ''],
             ['1', '.', 'intron', '161', '320', '.', '+', '.', ''],
             ['1', '.', 'CDS', '321', '380', '.', '+', '.', ''],
             ['1', '.', 'intron', '381', '540', '.', '+', '.', ''],
@@ -395,15 +395,15 @@
             ['1', '120', '121', '.', '1', '+'],
             ['1', '350', '351', '.', '1', '+'],
             ['1', '550', '551', '.', '1', '+'],
             ['1', '750', '751', '.', '1', '-'],
         ])
 
         command_basic = [
-            'iCount', 'rnamaps',
+            'iCount', 'metagene',
             cross_links,
             regions,
             '-S', '40',  # Supress lower than ERROR messages.
         ]
 
         self.assertEqual(subprocess.call(command_basic), 0)
```

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_clusters.py` & `iCount-Mini-3.0.0/iCount/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_data.py` & `iCount-Mini-3.0.0/iCount/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_demultiplex.py` & `iCount-Mini-3.0.0/iCount/tests/test_demultiplex.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_e2e.py` & `iCount-Mini-3.0.0/iCount/tests/test_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             ofile.write(seq + '\n')
             ofile.write('+' + '\n')
             ofile.write(
                 make_quality_scores(len(seq), min_chr=70, max_chr=73, rnd_seed=rseed) + '\n')
 
     def test_e2e(self):
         """
-        From raw reads and ENSEMBL annotation to rnamaps.
+        From raw reads and ENSEMBL annotation to metagene.
         """
 
         # Make segmentation & regions file
         seg = get_temp_file_name(extension='gtf')
         out_dir = get_temp_dir()
         iCount.genomes.segment.get_segments(self.gtf, seg, self.fai)
         iCount.genomes.segment.make_regions(seg, out_dir)
@@ -130,12 +130,12 @@
         pysam.index(bam)  # pylint:disable=no-member
 
         sites_single = get_temp_file_name(extension='bed.gz')
         sites_multi = get_temp_file_name(extension='bed.gz')
         skipped = get_temp_file_name(extension='bam')
         iCount.mapping.xlsites.run(bam, sites_single, sites_multi, skipped)
 
-        iCount.analysis.rnamaps.run(sites_single, regions)
+        iCount.analysis.metagene.run(sites_single, regions)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_examples.py` & `iCount-Mini-3.0.0/iCount/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_externals.py` & `iCount-Mini-3.0.0/iCount/tests/test_externals.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_files.py` & `iCount-Mini-3.0.0/iCount/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_genomes.py` & `iCount-Mini-3.0.0/iCount/tests/test_genomes.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_peaks.py` & `iCount-Mini-3.0.0/iCount/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_plotting.py` & `iCount-Mini-3.0.0/iCount/tests/test_plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring, protected-access
 import os
 import unittest
 import warnings
 
-from iCount.plotting import plot_rnamap, plot_rnaheatmap, plot_combined
+from iCount.plotting import plot_metagene, plot_rnaheatmap, plot_combined
 from iCount.tests.utils import get_temp_file_name, make_file_from_list
 
 
 def get_example_results_file():
     """Produce some thest file."""
     def zeros(size):
         """Return array of zeros of size ``size``."""
@@ -19,60 +19,60 @@
         ['chr1_+_100'] + zeros(51) + ['3', '5'] + zeros(48),
         ['chr1_+_200'] + zeros(49) + ['3', '0', '0', '1'] + zeros(48),
     ])
 
     return fname
 
 
-class TestPlotRnaMap(unittest.TestCase):
+class TestPlotMetagene(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", (ResourceWarning, ImportWarning))
 
         self.results_file = get_example_results_file()
 
     def test_normalize_cpm(self):
 
-        normalized = plot_rnamap.normalize_cpm(1, 10**6)
+        normalized = plot_metagene.normalize_cpm(1, 10**6)
         self.assertEqual(normalized, 1)
 
-        normalized = plot_rnamap.normalize_cpm(2, 10**6 * 2)
+        normalized = plot_metagene.normalize_cpm(2, 10**6 * 2)
         self.assertEqual(normalized, 1)
 
     def test_parse(self):
-        data, landmark_count = plot_rnamap.parse_results(self.results_file)
+        data, landmark_count = plot_metagene.parse_results(self.results_file)
         self.assertEqual(landmark_count, 2)
 
         expected = {
             -1: 3.0,
             1: 3.0,
             2: 6.0,
         }
         for pos, score in data.items():
             self.assertEqual(score, expected.get(pos, 0.0))
 
     def test_plot(self):
         outfile = get_temp_file_name(extension='png')
-        plot_rnamap.plot_rnamap(self.results_file, outfile)
+        plot_metagene.plot_metagene(self.results_file, outfile)
         self.assertTrue(os.path.isfile(outfile))
 
 
 class TestSmooth(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", (ResourceWarning, ImportWarning))
 
     def test_smoothe(self):
         # pylint: disable=missing-docstring, protected-access
         values = [0, 2, 0]
-        self.assertEqual(plot_rnamap.smooth(values, 1), [1, 2 / 3, 1])
+        self.assertEqual(plot_metagene.smooth(values, 1), [1, 2 / 3, 1])
 
         values = [0, 2, 4, 1, 0]
-        self.assertEqual(plot_rnamap.smooth(values, 1), [1, 2, 7 / 3, 5 / 3, 0.5])
-        self.assertEqual(plot_rnamap.smooth(values, 2), [2, 7 / 4, 7 / 5, 7 / 4, 5 / 3])
+        self.assertEqual(plot_metagene.smooth(values, 1), [1, 2, 7 / 3, 5 / 3, 0.5])
+        self.assertEqual(plot_metagene.smooth(values, 2), [2, 7 / 4, 7 / 5, 7 / 4, 5 / 3])
 
 
 class TestPlotRnaHeatMap(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", (ResourceWarning, ImportWarning))
```

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_rnamaps.py` & `iCount-Mini-3.0.0/iCount/tests/test_rnamaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 # pylint: disable=missing-docstring, protected-access
 import os
 import unittest
 import warnings
 
 from pybedtools import create_interval_from_list
 
-from iCount.analysis import rnamaps
+from iCount.analysis import metagene
 from iCount.files import remove_extension
 from iCount.tests.utils import get_temp_file_name, make_file_from_list, make_list_from_file
 
 
 class TestGetGeneName(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", (ResourceWarning, ImportWarning))
 
     def test_basic(self):
         seg_level0 = create_interval_from_list(['1', '.', 'CDS', '1', '2', '.', '+', '.', 'gene_name "G0";'])
         seg_level1 = create_interval_from_list(['1', '.', 'UTR3', '1', '2', '.', '+', '.', 'gene_name "G1";'])
         seg_level4 = create_interval_from_list(['1', '.', 'intron', '1', '2', '.', '+', '.', 'gene_name "G2";'])
 
-        self.assertEqual('G0', rnamaps.get_gene_name(seg_level0, seg_level1))
-        self.assertEqual('G0', rnamaps.get_gene_name(seg_level1, seg_level0))
-        self.assertEqual('G1', rnamaps.get_gene_name(seg_level1, seg_level4))
+        self.assertEqual('G0', metagene.get_gene_name(seg_level0, seg_level1))
+        self.assertEqual('G0', metagene.get_gene_name(seg_level1, seg_level0))
+        self.assertEqual('G1', metagene.get_gene_name(seg_level1, seg_level4))
         with self.assertRaises(ValueError):
-            self.assertEqual('B', rnamaps.get_gene_name(seg_level0, seg_level0))
+            self.assertEqual('B', metagene.get_gene_name(seg_level0, seg_level0))
 
 
 class TestMakeLandmarksFile(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", (ResourceWarning, ImportWarning))
 
     def test_basic(self):
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '150', '200', '.', '+', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '351', '.', '+', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'exon-intron')
+        fn = metagene.make_landmarks_file(regions, 'exon-intron')
         self.assertEqual(make_list_from_file(fn), [
             ['chr1', '200', '201', 'A', '.', '+'],
         ])
 
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '150', '200', '.', '-', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '351', '.', '-', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'intron-exon')
+        fn = metagene.make_landmarks_file(regions, 'intron-exon')
         self.assertEqual(make_list_from_file(fn), [
             ['chr1', '199', '200', 'A', '.', '-'],
         ])
 
     def test_limits_upstream(self):
         """Landmarks with too short upstream segment should not be used."""
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '151', '200', '.', '+', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '400', '.', '+', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'exon-intron')
+        fn = metagene.make_landmarks_file(regions, 'exon-intron')
         self.assertEqual(make_list_from_file(fn), [])
 
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '150', '200', '.', '-', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '350', '.', '-', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'intron-exon')
+        fn = metagene.make_landmarks_file(regions, 'intron-exon')
         self.assertEqual(make_list_from_file(fn), [])
 
     def test_limits_downstream(self):
         """Landmarks with too short upstream segment should not be used."""
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '150', '200', '.', '+', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '350', '.', '+', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'exon-intron')
+        fn = metagene.make_landmarks_file(regions, 'exon-intron')
         self.assertEqual(make_list_from_file(fn), [])
 
         regions = make_file_from_list([
             ['chr1', '.', 'CDS', '151', '200', '.', '-', '.', 'gene_name "A";'],
             ['chr1', '.', 'intron', '201', '351', '.', '-', '.', 'gene_name "A";'],
         ])
-        fn = rnamaps.make_landmarks_file(regions, 'intron-exon')
+        fn = metagene.make_landmarks_file(regions, 'intron-exon')
         self.assertEqual(make_list_from_file(fn), [])
 
 
 class TestComputeDistances(unittest.TestCase):
 
     def setUp(self):
         warnings.simplefilter("ignore", ResourceWarning)
@@ -96,72 +96,72 @@
             ['chr2', '10', '11', 'G3', '.', '+'],
         ])
 
     def test_basic(self):
         xlinks = make_file_from_list([
             ['chr1', '12', '13', '.', '3', '+'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 3)
         self.assertEqual(distances, {
             'chr1__+__10__G1': {2: 3},
         })
 
     def test_scores_sum(self):
         xlinks = make_file_from_list([
             ['chr1', '12', '13', '.', '3', '+'],
             ['chr1', '12', '13', '.', '1', '+'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 4)
         self.assertEqual(distances, {
             'chr1__+__10__G1': {2: 4},
         })
 
     def test_strands_not_mixed(self):
         xlinks = make_file_from_list([
             ['chr1', '12', '13', '.', '3', '+'],
             ['chr1', '12', '13', '.', '1', '-'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 4)
         self.assertEqual(distances, {
             'chr1__+__10__G1': {2: 3},
             'chr1__-__20__G2': {8: 1},
         })
 
     def test_chroms_not_mixed(self):
         xlinks = make_file_from_list([
             ['chr1', '12', '13', '.', '3', '+'],
             ['chr2', '12', '13', '.', '1', '+'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 4)
         self.assertEqual(distances, {
             'chr1__+__10__G1': {2: 3},
             'chr2__+__10__G3': {2: 1},
         })
 
     def test_size_limit(self):
         xlinks = make_file_from_list([
             ['chr1', '22', '23', '.', '3', '+'],
             ['chr2', '222', '223', '.', '1', '+'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 4)
         self.assertEqual(distances, {
             'chr1__+__20__G1': {2: 3},
         })
 
     def test_no_landmark(self):
         """Landmark is missing on this chromosome / stramd."""
         xlinks = make_file_from_list([
             ['chrX', '22', '23', '.', '3', '+'],
         ])
-        distances, total_cdna = rnamaps.compute_distances(self.landmarks, xlinks, 'exon-intron')
+        distances, total_cdna = metagene.compute_distances(self.landmarks, xlinks, 'exon-intron')
         self.assertEqual(total_cdna, 3)
         self.assertEqual(distances, {})
 
 
 class TestMakeFullResultsFile(unittest.TestCase):
 
     def setUp(self):
@@ -169,15 +169,15 @@
         self.fname = get_temp_file_name()
 
     def test_make_full_results_file(self):
         distances = {
             'chr1__+__10__G1': {2: 3},
             'chr2__+__20__G2': {-3: 3, 1: 5},
         }
-        rnamaps.make_results_raw_file(distances, self.fname, total_cdna=11, maptype='exon-intron')
+        metagene.make_results_raw_file(distances, self.fname, total_cdna=11, maptype='exon-intron')
 
         result = make_list_from_file(self.fname, fields_separator='\t')
         self.assertEqual(result[0], ['total_cdna:11'])
         self.assertEqual(result[1], ['.'] + list(map(str, range(-50, 151))))
         self.assertEqual(result[2][0], 'chr1__+__10__G1')
         self.assertEqual(result[2][45:55], ['0', '0', '0', '0', '0', '0', '0', '0', '3', '0'])
         self.assertEqual(result[3][45:55], ['0', '0', '0', '3', '0', '0', '0', '5', '0', '0'])
@@ -211,20 +211,20 @@
             ['chr1', '350', '351', '.', '1', '+'],
             ['chr1', '350', '351', '.', '1', '-'],
             ['chr1', '550', '551', '.', '1', '+'],
             ['chr1', '740', '741', '.', '1', '+'],
             ['chr1', '750', '751', '.', '1', '-'],
         ])
 
-        rnamaps.run(sites, regions, outdir=self.outdir)
+        metagene.run(sites, regions, outdir=self.outdir)
 
         self.assertTrue(os.path.isdir(self.outdir))
 
         sites_name = remove_extension(sites, ['.bed', '.bed.gz'])
-        for maptype in rnamaps.MAP_TYPES:
+        for maptype in metagene.MAP_TYPES:
             basename = os.path.join(self.outdir, '{}_{}'.format(sites_name, maptype))
             # for extension in ['.tsv', '.png', '_plot_data.txt']:
             for extension in ['.tsv', '.png']:
                 fname = basename + extension
                 self.assertTrue(os.path.isfile(fname))
                 self.assertGreater(os.path.getsize(fname), 1)
```

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_segment.py` & `iCount-Mini-3.0.0/iCount/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_summary.py` & `iCount-Mini-3.0.0/iCount/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/test_xlsites.py` & `iCount-Mini-3.0.0/iCount/tests/test_xlsites.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount/tests/utils.py` & `iCount-Mini-3.0.0/iCount/tests/utils.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/iCount_Mini.egg-info/PKG-INFO` & `iCount-Mini-3.0.0/iCount_Mini.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: iCount-Mini
-Version: 2.0.3
+Version: 3.0.0
 Summary: Computational pipeline for analysis of iCLIP data
 Home-page: https://github.com/ulelab/iCount-Mini
 Author: Ule Group, The Francis Crick Institute, London
 Author-email: jernej.ule@crick.ac.uk
 License: MIT
 Keywords: iCLIP protein-RNA
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -23,25 +22,32 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # iCount-Mini
 
 This is a fork of iCount maintained by members of [Jernej Ule's](http://ulelab.info) group, focussing on the peak calling features of iCount.
 
+Run commands using:
+`iCount-Mini <command>`
+
+**Note on small differences of terminology between iCount-Mini and iCount**
++ In iCount-Mini, sigxls = iCount peaks and iCount-Mini peaks = iCount clusters. This is to bring the terminology more in line with the rest of the field.
++ In iCount-Mini RNA-maps have been renamed to 'metagene', to distinguish these plots which include only CLIP data from other RNA-maps which group crosslinks into categories dependent on orthogonal data, such as alternatively spliced exons.
+
 # iCount: protein-RNA interaction analysis
 
 iCount is a Python module and associated command-line interface (CLI), which provides all the commands needed to process iCLIP data on protein-RNA interactions and generate:
  
 + demultiplexed and adapter-trimmed FASTQ files
 + BAM files with mapped iCLIP reads
 + identified protein-RNA cross-linked sites, saved to BED files
 + statistically significant cross-linked sites, saved to BED files
 + peaks of significant cross-linked sites, saved to BED files
 + grouping of individual replicate experiments
-+ RNAmap generation showing the positional distribution of cross-linked sites relative to genomic landmarks
++ metagene generation showing the positional distribution of cross-linked sites relative to genomic landmarks
 + kmer enrichment analysis
 
 You may start with the [tutorial](http://icount.readthedocs.io/en/latest/tutorial.html) or dive into the 
 [documentation](http://icount.readthedocs.io/en/latest/index.html).
 
 ## iCount-Mini Authors
 
@@ -58,9 +64,7 @@
 
 To install a development version of iCount-Mini, use this command.
 It's recommended to do this within a Python virtual environment.
 
 ```bash
 pip install --upgrade -r requirements-rtd.txt -e .
 ```
-
-
```

### Comparing `iCount-Mini-2.0.3/iCount_Mini.egg-info/SOURCES.txt` & `iCount-Mini-3.0.0/iCount_Mini.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 iCount/demultiplex.py
 iCount/logger.py
 iCount/metrics.py
 iCount/analysis/__init__.py
 iCount/analysis/annotate.py
 iCount/analysis/group.py
 iCount/analysis/kmers.py
+iCount/analysis/metagene.py
 iCount/analysis/peaks.py
-iCount/analysis/rnamaps.py
 iCount/analysis/sigxls.py
 iCount/analysis/summary.py
 iCount/examples/__init__.py
 iCount/examples/hnRNPC.sh
 iCount/examples/hnRNPC_reduced.sh
 iCount/examples/tutorial.sh
 iCount/externals/__init__.py
@@ -60,16 +60,16 @@
 iCount/mapping/__init__.py
 iCount/mapping/filters.py
 iCount/mapping/indexstar.py
 iCount/mapping/mapstar.py
 iCount/mapping/xlsites.py
 iCount/plotting/__init__.py
 iCount/plotting/plot_combined.py
+iCount/plotting/plot_metagene.py
 iCount/plotting/plot_rnaheatmap.py
-iCount/plotting/plot_rnamap.py
 iCount/tests/__init__.py
 iCount/tests/test_annotate.py
 iCount/tests/test_bed.py
 iCount/tests/test_cli.py
 iCount/tests/test_clusters.py
 iCount/tests/test_data.py
 iCount/tests/test_demultiplex.py
```

### Comparing `iCount-Mini-2.0.3/setup.py` & `iCount-Mini-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `iCount-Mini-2.0.3/tox.ini` & `iCount-Mini-3.0.0/tox.ini`

 * *Files identical despite different names*

