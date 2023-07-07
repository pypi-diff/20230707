# Comparing `tmp/seismic-rna-0.1.1.tar.gz` & `tmp/seismic-rna-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.1.1.tar", last modified: Thu Jul  6 01:29:40 2023, max compression
+gzip compressed data, was "seismic-rna-0.1.2.tar", last modified: Fri Jul  7 00:57:40 2023, max compression
```

## Comparing `seismic-rna-0.1.1.tar` & `seismic-rna-0.1.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.569640 seismic-rna-0.1.1/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.1/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-06 01:29:40.568861 seismic-rna-0.1.1/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1268 2023-07-06 00:54:05.000000 seismic-rna-0.1.1/README.md
--rw-r--r--   0 mfa        (503) staff       (20)      997 2023-07-06 00:52:32.000000 seismic-rna-0.1.1/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-06 01:29:40.569757 seismic-rna-0.1.1/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.469309 seismic-rna-0.1.1/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.482473 seismic-rna-0.1.1/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     3013 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      153 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-06 01:29:40.000000 seismic-rna-0.1.1/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.484731 seismic-rna-0.1.1/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      201 2023-06-29 18:12:04.000000 seismic-rna-0.1.1/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.489835 seismic-rna-0.1.1/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.1/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.1/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.495106 seismic-rna-0.1.1/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.525226 seismic-rna-0.1.1/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.1/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    17933 2023-06-29 19:57:56.000000 seismic-rna-0.1.1/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    24046 2023-07-05 20:58:22.000000 seismic-rna-0.1.1/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.1/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)    14191 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/files_sanity.py
--rw-r--r--   0 mfa        (503) staff       (20)     7851 2023-06-29 19:57:01.000000 seismic-rna-0.1.1/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2867 2023-06-29 17:37:52.000000 seismic-rna-0.1.1/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.1/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.1/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23506 2023-06-29 20:01:50.000000 seismic-rna-0.1.1/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.1/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.1/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29463 2023-06-29 19:57:29.000000 seismic-rna-0.1.1/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.1/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.1/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.1/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.1/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.1/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.1/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.1/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.528536 seismic-rna-0.1.1/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.537203 seismic-rna-0.1.1/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.1/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.1/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.543180 seismic-rna-0.1.1/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/graph/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     9744 2023-06-30 04:08:02.000000 seismic-rna-0.1.1/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.547460 seismic-rna-0.1.1/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4083 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    13982 2023-06-29 19:40:06.000000 seismic-rna-0.1.1/src/seismicrna/mask/write.py
--rw-r--r--   0 mfa        (503) staff       (20)       47 2023-07-06 00:52:00.000000 seismic-rna-0.1.1/src/seismicrna/meta.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.555786 seismic-rna-0.1.1/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.1/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.1/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.1/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.558176 seismic-rna-0.1.1/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.1/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.1/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.565120 seismic-rna-0.1.1/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-06 01:29:40.568019 seismic-rna-0.1.1/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.1/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.1/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.517778 seismic-rna-0.1.2/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.2/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-07 00:57:40.517277 seismic-rna-0.1.2/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1268 2023-07-06 00:54:05.000000 seismic-rna-0.1.2/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)      997 2023-07-07 00:56:15.000000 seismic-rna-0.1.2/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-07 00:57:40.517926 seismic-rna-0.1.2/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.416199 seismic-rna-0.1.2/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.427486 seismic-rna-0.1.2/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3013 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      153 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.429591 seismic-rna-0.1.2/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      201 2023-06-29 18:12:04.000000 seismic-rna-0.1.2/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.434126 seismic-rna-0.1.2/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.2/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.2/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.440368 seismic-rna-0.1.2/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.471892 seismic-rna-0.1.2/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.2/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18415 2023-07-07 00:40:09.000000 seismic-rna-0.1.2/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    24043 2023-07-06 23:44:48.000000 seismic-rna-0.1.2/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.2/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14191 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/files_sanity.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7851 2023-06-29 19:57:01.000000 seismic-rna-0.1.2/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2867 2023-06-29 17:37:52.000000 seismic-rna-0.1.2/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.2/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.2/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.1.2/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.2/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.2/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29463 2023-06-29 19:57:29.000000 seismic-rna-0.1.2/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.2/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.2/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.2/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.2/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.2/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.2/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.2/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.475172 seismic-rna-0.1.2/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.485826 seismic-rna-0.1.2/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.2/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.2/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.494134 seismic-rna-0.1.2/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9744 2023-06-30 04:08:02.000000 seismic-rna-0.1.2/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.498861 seismic-rna-0.1.2/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4083 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-07-06 23:44:35.000000 seismic-rna-0.1.2/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.1.2/src/seismicrna/mask/write.py
+-rw-r--r--   0 mfa        (503) staff       (20)       47 2023-07-07 00:56:58.000000 seismic-rna-0.1.2/src/seismicrna/meta.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.507569 seismic-rna-0.1.2/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.2/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.2/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.2/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.510081 seismic-rna-0.1.2/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.2/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.2/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.514991 seismic-rna-0.1.2/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.516620 seismic-rna-0.1.2/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.2/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.1.1/LICENSE` & `seismic-rna-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/PKG-INFO` & `seismic-rna-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.1
+Version: 0.1.2
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.1.1/README.md` & `seismic-rna-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/pyproject.toml` & `seismic-rna-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
```

### Comparing `seismic-rna-0.1.1/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.1.2/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.1
+Version: 0.1.2
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.1.1/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.1.2/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.1.2/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/align/fqutil.py` & `seismic-rna-0.1.2/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/align/main.py` & `seismic-rna-0.1.2/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/align/strandedness.py` & `seismic-rna-0.1.2/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/compare.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/compare.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/em.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/krun.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/load.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/main.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/report.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/cluster/write.py` & `seismic-rna-0.1.2/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/bitcall.py` & `seismic-rna-0.1.2/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/bitvect.py` & `seismic-rna-0.1.2/src/seismicrna/core/bitvect.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,17 @@
         return self.n_affi_per_pos / self.n_info_per_pos
 
     @property
     def f_affi_per_read(self):
         """ Fraction of affirmative bits for each read. """
         return self.n_affi_per_read / self.n_info_per_read
 
-    def _check_duplicate_reads(self):
-        """ Verify that no read name occurs more than once. """
-        if self.reads.has_duplicates:
-            dups = self.reads[self.reads.duplicated(keep="first")]
-            raise DuplicateIndexError(f"Duplicate read names: {dups}")
+    @abstractmethod
+    def _drop_duplicate_reads(self, *args):
+        """ Drop any read with a duplicate name. """
 
 
 class BitMatrix(BitVectorBase, ABC):
     """ Bit vectors represented with two explicit boolean matrices of
     informative and affirmative bits. """
 
     @property
@@ -240,28 +238,42 @@
 
     @property
     def n_affi_per_read(self):
         """ Number of affirmative bits for each read. """
         return pd.Series(np.count_nonzero(self.affi, axis=1),
                          index=self.reads)
 
+    def _drop(self, drop: pd.Index):
+        """ Drop the reads in `drop`; return the number dropped. """
+        if drop.size > 0:
+            logger.debug(f"Dropping {drop} from {self}")
+            self.info.drop(index=drop, inplace=True)
+            self.affi.drop(index=drop, inplace=True)
+        return drop.size
+
+    def _drop_duplicate_reads(self):
+        dups = self.reads[self.reads.duplicated(keep="first")]
+        if self._drop(dups):
+            logger.warning(f"{self} got duplicate read names: {dups.to_list()}")
+        return dups
+
 
 class BitBatch(BitMatrix):
     """ One batch of bit vectors. """
 
     def __init__(self, section: Section,
                  info: pd.DataFrame, affi: pd.DataFrame,
                  mask: dict[str, Callable[[BitBatch], pd.Index]] | None = None):
         super().__init__(section)
         # Initialize the reads.
         self._info = info
         self._affi = affi
         # Validate the reads.
         self._check_indexes()
-        self._check_duplicate_reads()
+        self._drop_duplicate_reads()
         # Mask the reads.
         self._masked = Counter(self._mask(mask or dict()))
 
     def _check_indexes(self):
         """ Verify that the read names and positions in info and muts
         are consistent with each other and with the section. """
         logger.debug(f"Checking indexes of {self}")
@@ -284,25 +296,22 @@
         return self._info
 
     @property
     def affi(self):
         """ DataFrame of affirmative bits. """
         return self._affi
 
+    def drop_reads(self, drop: pd.Index):
+        """ Drop the reads in `drop`; return the number dropped. """
+        return self._drop(drop)
+
     @property
     def nmasked(self):
         return self._masked
 
-    def _drop(self, drop: pd.Index):
-        """ Drop the reads in `drop`; return the number dropped. """
-        logger.debug(f"Dropping {drop} from {self}")
-        self._info.drop(index=drop, inplace=True)
-        self._affi.drop(index=drop, inplace=True)
-        return drop.size
-
     def _mask(self, masks: dict[str, Callable[[BitBatch], np.ndarray]]):
         """ Drop reads selected by any of the masks, which should be
         boolean NumPy arrays. """
         logger.debug(f"Masking {self} with {masks}")
         return {name: self._drop(self.reads[mask(self)])
                 for name, mask in masks.items()}
 
@@ -355,14 +364,16 @@
             logger.debug(f"Add batch {self.nbatches + 1} ({batch}) to {self}")
             # Confirm that the sections from which the batch derives
             # matches the section from which the accumulator derives.
             if batch.section != self.section:
                 raise InconsistentSectionError(
                     f"Sections of the batch ({batch.section}) and accumulator "
                     f"({self.section}) do not match")
+            # Drop any reads whose names match reads that already exist.
+            self._drop_duplicate_reads(batch)
             # Update the counts of the numbers of reads masked.
             self._masked += batch.nmasked
             logger.debug(f"Current masked counts for {self}: {self.nmasked}")
             # Add the counts of informative and affirmative bits.
             self._count_info_affi(batch)
             # Increment the number of batches given.
             self._nbatches += 1
@@ -381,14 +392,21 @@
         return self._masked
 
     @property
     def nbatches(self):
         """ Number of batches given to the accumulator. """
         return self._nbatches
 
+    def _drop_duplicate_reads(self, batch: BitBatch):
+        dups = batch.reads.intersection(self.reads)
+        if batch.drop_reads(dups):
+            logger.warning(f"{self} got read(s) in {batch} with name(s) seen "
+                           f"in a previous batch: {dups.to_list()}")
+        return dups
+
 
 class BitMonolith(BitAccum, BitMatrix):
     """ Accumulates batches of bit vectors into one monolithic unit. """
 
     def __init__(self, section: Section, batches: Iterable[BitBatch]):
         # Initialize lists of each batch's total and affirmative bits.
         self._info: list[pd.DataFrame] | pd.DataFrame = list()
@@ -398,16 +416,14 @@
             # Merge the informative and affirmative bits to DataFrames.
             self._info = pd.concat(self._info, axis=0)
             self._affi = pd.concat(self._affi, axis=0)
         else:
             # No batches were given.
             self._info = self._empty_accum()
             self._affi = self._empty_accum()
-        # Check for duplicate read names among all batches.
-        self._check_duplicate_reads()
 
     def _empty_accum(self):
         """ Empty DataFrame whose columns are the section indexes. """
         return pd.DataFrame(index=[], columns=self.section.unmasked,
                             dtype=int)
 
     def _count_info_affi(self, batch: BitBatch):
@@ -435,16 +451,14 @@
     def __init__(self, section: Section, batches: Iterable[BitBatch]):
         # Initialize the counts of informative and affirmative bits.
         self._info_per_pos = self._init_per_pos(section)
         self._affi_per_pos = self._init_per_pos(section)
         self._info_per_read: list[pd.Series] = list()
         self._affi_per_read: list[pd.Series] = list()
         super().__init__(section, batches)
-        # Check for duplicate read names among all batches.
-        self._check_duplicate_reads()
 
     def _init_per_pos(self, section: Section):
         """ Initialize a count of 0 for each position. """
         return pd.Series(0, index=section.unmasked)
 
     def _empty_accum(self):
         return pd.Series([], dtype=int)
```

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/cli.py` & `seismic-rna-0.1.2/src/seismicrna/core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,28 +460,26 @@
                    help="Table file.")
 
 opt_table_cols = Option(("--table-cols", "-c"),
                         default="",
                         type=str,
                         help="Output columns of these relationships")
 
-
 # RNA structure prediction
 
 opt_fold = Option(("--fold/--no-fold",),
                   type=bool,
                   default=True,
                   help="Whether to predict the RNA structure using Fold")
 
 opt_dms_quantile = Option(("--dms-quantile", "-q"),
                           type=float,
                           default=0.9,
                           help="Quantile of DMS reactivities for normalization")
 
-
 # Graphing
 
 opt_stack = Option(("--stack", "-s"),
                    default="",
                    type=str,
                    help="Draw stacked graphs of these relationships")
 
@@ -517,15 +515,14 @@
                   help="Whether to output each graph as an HTML file")
 
 opt_pdf = Option(("--pdf/--no-pdf",),
                  default=False,
                  type=bool,
                  help="Whether to output each graph as a PDF file")
 
-
 # Logging options
 opt_verbose = Option(("--verbose", "-v"),
                      count=True,
                      help="Print info or info+debug messages to stdout")
 opt_quiet = Option(("--quiet", "-q"),
                    count=True,
                    help="Suppress warnings or warnings+errors to stdout")
```

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/depend.py` & `seismic-rna-0.1.2/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/docdef.py` & `seismic-rna-0.1.2/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/docstring.py` & `seismic-rna-0.1.2/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/dump.py` & `seismic-rna-0.1.2/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/files.py` & `seismic-rna-0.1.2/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/files_sanity.py` & `seismic-rna-0.1.2/src/seismicrna/core/files_sanity.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/load.py` & `seismic-rna-0.1.2/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/logs.py` & `seismic-rna-0.1.2/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/mu.py` & `seismic-rna-0.1.2/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/mu_test.py` & `seismic-rna-0.1.2/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/parallel.py` & `seismic-rna-0.1.2/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/path.py` & `seismic-rna-0.1.2/src/seismicrna/core/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,29 +410,29 @@
 DmFastq2Seg = Segment("dm-fastq2", {REF: NameField, EXT: Fastq2Ext})
 # Alignment
 XamSeg = Segment("xam", {REF: NameField, EXT: XamExt})
 BamIndexSeg = Segment("bai", {REF: NameField, EXT: BamIndexExt})
 AlignRepSeg = Segment("align-rep", {EXT: ReportExt}, frmt="report-align{ext}")
 # Relation Vectors
 RelateBatSeg = Segment("rel-bat", {BATCH: IntField, EXT: RelVecBatExt},
-                       frmt="batch-rel-{batch}{ext}")
+                       frmt="batch-relate-{batch}{ext}")
 RelateRepSeg = Segment("rel-rep", {EXT: ReportExt}, frmt="report-relate{ext}")
 # Masking
 MaskBatSeg = Segment("mask-bat", {BATCH: IntField, EXT: MaskBatExt},
                      frmt="batch-mask-{batch}{ext}")
 MaskRepSeg = Segment("mask-rep", {EXT: ReportExt}, frmt="report-mask{ext}")
 # Clustering
 ClustTabSeg = Segment("clust-tab", {TABLE: ClustTabField,
                                     NCLUST: IntField,
                                     RUN: IntField,
                                     EXT: ClustTabExt},
                       frmt="{table}-k{k}-r{run}{ext}")
 ClustCountSeg = Segment("clust-count", {EXT: ClustCountExt}, frmt="counts{ext}")
 ClustBatSeg = Segment("clust-bat", {BATCH: IntField, EXT: ClustBatExt},
-                      frmt="batch-clust-{batch}{ext}")
+                      frmt="batch-cluster-{batch}{ext}")
 ClustRepSeg = Segment("clust-rep", {EXT: ReportExt},
                       frmt="report-cluster{ext}")
 # Mutation Tables
 MutTabSeg = Segment("mut-tab", {TABLE: CountTabField, EXT: MutTabExt})
 # RNA Structure Formats
 ConnectTableSeg = Segment("rna-ct", {STRUCT: NameField, EXT: ConnectTableExt})
 DotBracketSeg = Segment("rna-dot", {STRUCT: NameField, EXT: DotBracketExt})
```

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/rel.py` & `seismic-rna-0.1.2/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/rel_test.py` & `seismic-rna-0.1.2/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/report.py` & `seismic-rna-0.1.2/src/seismicrna/core/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/rna.py` & `seismic-rna-0.1.2/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/sect.py` & `seismic-rna-0.1.2/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/sect_test.py` & `seismic-rna-0.1.2/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/seq.py` & `seismic-rna-0.1.2/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/seq_test.py` & `seismic-rna-0.1.2/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/shell.py` & `seismic-rna-0.1.2/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/sim.py` & `seismic-rna-0.1.2/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/sim_test.py` & `seismic-rna-0.1.2/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/types.py` & `seismic-rna-0.1.2/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/core/xam.py` & `seismic-rna-0.1.2/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.1.2/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/demult/main.py` & `seismic-rna-0.1.2/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/draw/main.py` & `seismic-rna-0.1.2/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.1.2/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/draw/plotter.py` & `seismic-rna-0.1.2/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/draw/study.py` & `seismic-rna-0.1.2/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/draw/util.py` & `seismic-rna-0.1.2/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/graph/base.py` & `seismic-rna-0.1.2/src/seismicrna/graph/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/graph/color.py` & `seismic-rna-0.1.2/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/graph/default.py` & `seismic-rna-0.1.2/src/seismicrna/graph/default.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/graph/hist.py` & `seismic-rna-0.1.2/src/seismicrna/graph/hist.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/graph/seq.py` & `seismic-rna-0.1.2/src/seismicrna/graph/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/main.py` & `seismic-rna-0.1.2/src/seismicrna/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/mask/load.py` & `seismic-rna-0.1.2/src/seismicrna/mask/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/mask/main.py` & `seismic-rna-0.1.2/src/seismicrna/mask/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/mask/report.py` & `seismic-rna-0.1.2/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/mask/write.py` & `seismic-rna-0.1.2/src/seismicrna/mask/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             n_reads_min_finfo=self.n_reads_min_finfo,
             n_reads_max_fmut=self.n_reads_max_fmut,
             n_reads_min_gap=self.n_reads_min_gap,
             n_reads_kept=self.n_reads_kept,
         )
 
     def __str__(self):
-        return f"Mask {self.section} with {self.bit_caller}"
+        return f"Mask {self.sample} over {self.section} with {self.bit_caller}"
 
 
 def mask_section(loader: RelateLoader,
                  section: Section,
                  count_del: bool,
                  count_ins: bool,
                  discount: Iterable[str], *,
```

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/export.py` & `seismic-rna-0.1.2/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/load.py` & `seismic-rna-0.1.2/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/main.py` & `seismic-rna-0.1.2/src/seismicrna/relate/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/relate.py` & `seismic-rna-0.1.2/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/report.py` & `seismic-rna-0.1.2/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/sam.py` & `seismic-rna-0.1.2/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.1.2/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/test.py` & `seismic-rna-0.1.2/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/relate/write.py` & `seismic-rna-0.1.2/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/struct/main.py` & `seismic-rna-0.1.2/src/seismicrna/struct/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.1.2/src/seismicrna/struct/rnastructure.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/table/base.py` & `seismic-rna-0.1.2/src/seismicrna/table/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/table/load.py` & `seismic-rna-0.1.2/src/seismicrna/table/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/table/main.py` & `seismic-rna-0.1.2/src/seismicrna/table/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/table/tabulate.py` & `seismic-rna-0.1.2/src/seismicrna/table/tabulate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/table/write.py` & `seismic-rna-0.1.2/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.1/src/seismicrna/test/main.py` & `seismic-rna-0.1.2/src/seismicrna/test/main.py`

 * *Files identical despite different names*

