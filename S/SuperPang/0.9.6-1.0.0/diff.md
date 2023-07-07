# Comparing `tmp/SuperPang-0.9.6.tar.gz` & `tmp/SuperPang-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SuperPang-0.9.6.tar", last modified: Wed Mar  1 16:05:03 2023, max compression
+gzip compressed data, was "SuperPang-1.0.0.tar", last modified: Fri Jul  7 12:04:53 2023, max compression
```

## Comparing `SuperPang-0.9.6.tar` & `SuperPang-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,46 @@
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.224918 SuperPang-0.9.6/
--rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-0.9.6/LICENSE
--rw-r--r--   0 fer       (1000) fer       (1000)       56 2022-07-05 08:50:08.000000 SuperPang-0.9.6/MANIFEST.in
--rw-rw-r--   0 fer       (1000) fer       (1000)     5918 2023-03-01 16:05:03.224918 SuperPang-0.9.6/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)     5233 2023-03-01 14:42:34.000000 SuperPang-0.9.6/README.md
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.216918 SuperPang-0.9.6/SuperPang/
--rw-r--r--   0 fer       (1000) fer       (1000)        6 2023-03-01 16:02:32.000000 SuperPang-0.9.6/SuperPang/VERSION
--rw-r--r--   0 fer       (1000) fer       (1000)        0 2022-07-05 08:50:08.000000 SuperPang-0.9.6/SuperPang/__init__.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.216918 SuperPang-0.9.6/SuperPang/lib/
--rw-rw-r--   0 fer       (1000) fer       (1000)    52207 2023-03-01 14:42:34.000000 SuperPang-0.9.6/SuperPang/lib/Assembler.py
--rw-rw-r--   0 fer       (1000) fer       (1000)   945424 2023-03-01 16:05:02.000000 SuperPang-0.9.6/SuperPang/lib/Compressor.c
--rw-r--r--   0 fer       (1000) fer       (1000)        0 2022-07-05 08:50:08.000000 SuperPang-0.9.6/SuperPang/lib/__init__.py
--rw-rw-r--   0 fer       (1000) fer       (1000)     2893 2023-03-01 14:42:34.000000 SuperPang-0.9.6/SuperPang/lib/utils.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.216918 SuperPang-0.9.6/SuperPang/scripts/
--rwxrwxr-x   0 fer       (1000) fer       (1000)    15151 2023-03-01 14:42:34.000000 SuperPang-0.9.6/SuperPang/scripts/SuperPang.py
--rwxr-xr-x   0 fer       (1000) fer       (1000)    11347 2023-03-01 15:56:48.000000 SuperPang-0.9.6/SuperPang/scripts/condense-edges.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)    14903 2023-03-01 14:42:34.000000 SuperPang-0.9.6/SuperPang/scripts/homogenize.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)      947 2023-03-01 15:46:40.000000 SuperPang-0.9.6/SuperPang/scripts/test-SuperPang.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.224918 SuperPang-0.9.6/SuperPang/test_data/
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2430301 2022-07-05 08:50:01.000000 SuperPang-0.9.6/SuperPang/test_data/2636415981.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2266131 2022-07-05 08:49:59.000000 SuperPang-0.9.6/SuperPang/test_data/2636416036.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2274047 2022-07-05 08:50:00.000000 SuperPang-0.9.6/SuperPang/test_data/2636416061.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2402610 2022-07-05 08:49:59.000000 SuperPang-0.9.6/SuperPang/test_data/2636416062.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2207567 2022-07-05 08:50:00.000000 SuperPang-0.9.6/SuperPang/test_data/2639762512.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2184834 2022-07-05 08:50:01.000000 SuperPang-0.9.6/SuperPang/test_data/2639762514.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2317227 2022-07-05 08:50:02.000000 SuperPang-0.9.6/SuperPang/test_data/2639762515.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2202772 2022-07-05 08:50:01.000000 SuperPang-0.9.6/SuperPang/test_data/2639762516.fna
--rwxr-xr-x   0 fer       (1000) fer       (1000)  2210266 2022-07-05 08:50:00.000000 SuperPang-0.9.6/SuperPang/test_data/2844342787.fna
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-03-01 16:05:03.216918 SuperPang-0.9.6/SuperPang.egg-info/
--rw-rw-r--   0 fer       (1000) fer       (1000)     5918 2023-03-01 16:05:02.000000 SuperPang-0.9.6/SuperPang.egg-info/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)      795 2023-03-01 16:05:03.000000 SuperPang-0.9.6/SuperPang.egg-info/SOURCES.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-03-01 16:05:02.000000 SuperPang-0.9.6/SuperPang.egg-info/dependency_links.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       29 2023-03-01 16:05:03.000000 SuperPang-0.9.6/SuperPang.egg-info/requires.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       10 2023-03-01 16:05:03.000000 SuperPang-0.9.6/SuperPang.egg-info/top_level.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-03-01 16:05:03.224918 SuperPang-0.9.6/setup.cfg
--rw-r--r--   0 fer       (1000) fer       (1000)     3088 2022-07-05 08:50:09.000000 SuperPang-0.9.6/setup.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.480357 SuperPang-1.0.0/
+-rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-1.0.0/LICENSE
+-rw-rw-r--   0 fer       (1000) fer       (1000)       31 2023-07-07 12:04:12.000000 SuperPang-1.0.0/MANIFEST.in
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8249 2023-07-07 12:04:53.480357 SuperPang-1.0.0/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5728 2023-07-06 10:10:07.000000 SuperPang-1.0.0/README.md
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1759 2023-07-06 15:20:02.000000 SuperPang-1.0.0/pyproject.toml
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-07 12:04:53.480357 SuperPang-1.0.0/setup.cfg
+-rw-r--r--   0 fer       (1000) fer       (1000)      711 2023-07-07 12:04:45.000000 SuperPang-1.0.0/setup.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.468357 SuperPang-1.0.0/src/
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.468357 SuperPang-1.0.0/src/SuperPang.egg-info/
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8249 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1165 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/SOURCES.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/dependency_links.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)      172 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/entry_points.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/requires.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       10 2023-07-07 12:04:53.000000 SuperPang-1.0.0/src/SuperPang.egg-info/top_level.txt
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.468357 SuperPang-1.0.0/src/superpang/
+-rw-r--r--   0 fer       (1000) fer       (1000)        6 2023-06-30 13:37:17.000000 SuperPang-1.0.0/src/superpang/VERSION
+-rw-r--r--   0 fer       (1000) fer       (1000)        0 2022-07-05 08:50:08.000000 SuperPang-1.0.0/src/superpang/__init__.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.472357 SuperPang-1.0.0/src/superpang/lib/
+-rw-rw-r--   0 fer       (1000) fer       (1000)    54444 2023-07-06 15:08:18.000000 SuperPang-1.0.0/src/superpang/lib/Assembler.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)   953595 2023-07-07 12:04:51.000000 SuperPang-1.0.0/src/superpang/lib/Compressor.c
+-rw-r--r--   0 fer       (1000) fer       (1000)     3466 2023-07-03 13:34:07.000000 SuperPang-1.0.0/src/superpang/lib/Compressor.pyx
+-rw-r--r--   0 fer       (1000) fer       (1000)        0 2022-07-05 08:50:08.000000 SuperPang-1.0.0/src/superpang/lib/__init__.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)   888467 2023-07-07 12:04:52.000000 SuperPang-1.0.0/src/superpang/lib/cutils.c
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5151 2023-07-05 08:15:32.000000 SuperPang-1.0.0/src/superpang/lib/cutils.pyx
+-rw-rw-r--   0 fer       (1000) fer       (1000)     3038 2023-07-05 13:03:35.000000 SuperPang-1.0.0/src/superpang/lib/utils.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)   931708 2023-07-07 12:04:52.000000 SuperPang-1.0.0/src/superpang/lib/vtools.c
+-rw-rw-r--   0 fer       (1000) fer       (1000)     2920 2023-07-05 13:13:48.000000 SuperPang-1.0.0/src/superpang/lib/vtools.pyx
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.472357 SuperPang-1.0.0/src/superpang/scripts/
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    16805 2023-07-07 10:32:36.000000 SuperPang-1.0.0/src/superpang/scripts/SuperPang.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-06 15:12:40.000000 SuperPang-1.0.0/src/superpang/scripts/__init__.py
+-rwxr-xr-x   0 fer       (1000) fer       (1000)    11347 2023-07-06 15:12:20.000000 SuperPang-1.0.0/src/superpang/scripts/condense-edges.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    16715 2023-07-06 15:11:29.000000 SuperPang-1.0.0/src/superpang/scripts/homogenize.py
+-rwxr-xr-x   0 fer       (1000) fer       (1000)     1568 2023-07-06 15:40:01.000000 SuperPang-1.0.0/src/superpang/scripts/test-SuperPang.py
+-rwxr-xr-x   0 fer       (1000) fer       (1000)     1568 2023-07-06 15:40:01.000000 SuperPang-1.0.0/src/superpang/scripts/test_SuperPang.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-07 12:04:53.476357 SuperPang-1.0.0/src/superpang/test_data/
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2430301 2022-07-05 08:50:01.000000 SuperPang-1.0.0/src/superpang/test_data/2636415981.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2266131 2022-07-05 08:49:59.000000 SuperPang-1.0.0/src/superpang/test_data/2636416036.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2274047 2022-07-05 08:50:00.000000 SuperPang-1.0.0/src/superpang/test_data/2636416061.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2402610 2022-07-05 08:49:59.000000 SuperPang-1.0.0/src/superpang/test_data/2636416062.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2207567 2022-07-05 08:50:00.000000 SuperPang-1.0.0/src/superpang/test_data/2639762512.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2184834 2022-07-05 08:50:01.000000 SuperPang-1.0.0/src/superpang/test_data/2639762514.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2317227 2022-07-05 08:50:02.000000 SuperPang-1.0.0/src/superpang/test_data/2639762515.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2202772 2022-07-05 08:50:01.000000 SuperPang-1.0.0/src/superpang/test_data/2639762516.fna
+-rwxr-xr-x   0 fer       (1000) fer       (1000)  2210266 2022-07-05 08:50:00.000000 SuperPang-1.0.0/src/superpang/test_data/2844342787.fna
```

### Comparing `SuperPang-0.9.6/LICENSE` & `SuperPang-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/PKG-INFO` & `SuperPang-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: SuperPang
-Version: 0.9.6
-Summary: Non-redundant pangenome assemblies from multiple genomes or bins
-Home-page: https://github.com/fpusan/SuperPang
-Author: Fernando Puente-Sánchez
-Author-email: fernando.puente.sanchez@slu.se
-License: BSD
-Keywords: bioinformatics assembly metagenomics microbial-genomics genomics
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SuperPang: non-redundant pangenome assemblies from multiple genomes or bins
 
-**Check our preprint:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://www.biorxiv.org/content/10.1101/2022.03.25.485477v1.full) _bioRxiv_ (2022) DOI: 10.1101/2022.03.25.485477
+**Check our paper:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://onlinelibrary.wiley.com/doi/full/10.1111/1755-0998.13826) _Molecular Ecology Resources_ (2023) DOI: 10.1111/1755-0998.13826
+_... but note that performance is now better (3x less memory usage, 20% faster execution time) than when we first benchmarked Superpang.
 
 ## Installation
-Requires [graph-tool](https://graph-tool.skewed.de/), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
+Requires [graph-tool](https://graph-tool.skewed.de/), [speedict](https://github.com/Congyuwang/RocksDict), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
 ```
 # Install into a new conda environment
 conda create -n SuperPang -c conda-forge -c bioconda -c fpusan superpang
 # Check that it works for you!
 conda activate SuperPang
 test-SuperPang.py
 ```
@@ -53,24 +36,28 @@
 * *-l/--minlen*: Scaffold length cutoff. Default `0` (no cutoff).
 * *-c/--mincov*: Scaffold coverage cutoff. Default `0` (no cutoff).
 * *-b/--bubble-identity-threshold*: Minimum identity (matches / length) required to remove a bubble in the sequence graph. Default `0.95`.
 * *-a/--genome-assignment-threshold*. Fraction of shared kmers required to assign a contig to an input genome (0 means a single shared kmer is enough). Default `0.5`.
 * *-x/--default-completeness*: Default genome completeness to assume if a CheckM output is not provided with *--checkm*. Default `70`.
 * *-t/--threads*: Number of processors to use. Default `1`.
 * *-o/--output*: Output directory. Default `output`.
+* *-d/--temp-dir*: Directory for temp files. Default `tmp`.
 * *--assume-complete*: Assume that the input genomes are complete (*--genome-assignment-threshold 0.95*, *--default-completeness 99*).
+* *--lowmem*: Use disk storages instead of memory when possible, reduces memory usage at the cost of execution time.
 * *--minimap2-path*: Path to the minimap2 executable. Default `minimap2`.
 * *--keep-intermediate*: Keep intermediate files.
+* *--keep-temporary*: Keep temporary files.
 * *--verbose-mOTUpan*: Print out mOTUpan logs.
+* *--debug*: Run additional sanity checks (increases execution time).
 
 ## Output
 * `assembly.fasta`: contigs.
 * `assembly.info`: core/auxiliary and path information for each contig.
 * `NBPs.fasta`: non-branching paths.
 * `NBPs.core.fasta`: non-branching paths deemed to belong to the core genome of the species by [mOTUpan](https://www.biorxiv.org/content/10.1101/2021.06.25.449606v1).
 * `NBPs.accessory.fasta`: non-branching paths deemed to belong to the accessory genome of the species.
 * `graph.fastg`: assembly graph in a format compatible with [bandage](https://rrwick.github.io/Bandage/).
 * `NBP2origins.tsv`: tab-separated file with the non-branching path IDs, a comma-separated list of the input sequences in which that NBP was deemed present, a comma-separated list of the input genomes in which that NBP was deemed present, and the number of input genomes in which that NBP was deemed present.
 * `params.tsv`: parameters used in the run.
 
 ## About
-*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantsbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
+*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
```

### Comparing `SuperPang-0.9.6/README.md` & `SuperPang-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,61 @@
+Metadata-Version: 2.1
+Name: SuperPang
+Version: 1.0.0
+Summary: Non-redundant pangenome assemblies from multiple genomes or bins
+Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2021, Fernando Puente-Sánchez
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/fpusan/SuperPang
+Project-URL: Bug Tracker, https://github.com/fpusan/SuperPang/issues
+Keywords: bioinformatics,assembly,metagenomics,microbial-genomics,genomics
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SuperPang: non-redundant pangenome assemblies from multiple genomes or bins
 
-**Check our preprint:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://www.biorxiv.org/content/10.1101/2022.03.25.485477v1.full) _bioRxiv_ (2022) DOI: 10.1101/2022.03.25.485477
+**Check our paper:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://onlinelibrary.wiley.com/doi/full/10.1111/1755-0998.13826) _Molecular Ecology Resources_ (2023) DOI: 10.1111/1755-0998.13826
+_... but note that performance is now better (3x less memory usage, 20% faster execution time) than when we first benchmarked Superpang.
 
 ## Installation
-Requires [graph-tool](https://graph-tool.skewed.de/), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
+Requires [graph-tool](https://graph-tool.skewed.de/), [speedict](https://github.com/Congyuwang/RocksDict), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
 ```
 # Install into a new conda environment
 conda create -n SuperPang -c conda-forge -c bioconda -c fpusan superpang
 # Check that it works for you!
 conda activate SuperPang
 test-SuperPang.py
 ```
@@ -35,24 +83,28 @@
 * *-l/--minlen*: Scaffold length cutoff. Default `0` (no cutoff).
 * *-c/--mincov*: Scaffold coverage cutoff. Default `0` (no cutoff).
 * *-b/--bubble-identity-threshold*: Minimum identity (matches / length) required to remove a bubble in the sequence graph. Default `0.95`.
 * *-a/--genome-assignment-threshold*. Fraction of shared kmers required to assign a contig to an input genome (0 means a single shared kmer is enough). Default `0.5`.
 * *-x/--default-completeness*: Default genome completeness to assume if a CheckM output is not provided with *--checkm*. Default `70`.
 * *-t/--threads*: Number of processors to use. Default `1`.
 * *-o/--output*: Output directory. Default `output`.
+* *-d/--temp-dir*: Directory for temp files. Default `tmp`.
 * *--assume-complete*: Assume that the input genomes are complete (*--genome-assignment-threshold 0.95*, *--default-completeness 99*).
+* *--lowmem*: Use disk storages instead of memory when possible, reduces memory usage at the cost of execution time.
 * *--minimap2-path*: Path to the minimap2 executable. Default `minimap2`.
 * *--keep-intermediate*: Keep intermediate files.
+* *--keep-temporary*: Keep temporary files.
 * *--verbose-mOTUpan*: Print out mOTUpan logs.
+* *--debug*: Run additional sanity checks (increases execution time).
 
 ## Output
 * `assembly.fasta`: contigs.
 * `assembly.info`: core/auxiliary and path information for each contig.
 * `NBPs.fasta`: non-branching paths.
 * `NBPs.core.fasta`: non-branching paths deemed to belong to the core genome of the species by [mOTUpan](https://www.biorxiv.org/content/10.1101/2021.06.25.449606v1).
 * `NBPs.accessory.fasta`: non-branching paths deemed to belong to the accessory genome of the species.
 * `graph.fastg`: assembly graph in a format compatible with [bandage](https://rrwick.github.io/Bandage/).
 * `NBP2origins.tsv`: tab-separated file with the non-branching path IDs, a comma-separated list of the input sequences in which that NBP was deemed present, a comma-separated list of the input genomes in which that NBP was deemed present, and the number of input genomes in which that NBP was deemed present.
 * `params.tsv`: parameters used in the run.
 
 ## About
-*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantsbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
+*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
```

### Comparing `SuperPang-0.9.6/SuperPang/lib/Assembler.py` & `SuperPang-1.0.0/src/superpang/lib/Assembler.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from itertools import combinations
 from multiprocessing import Pool
 from multiprocessing.managers import SharedMemoryManager
 from functools import partial
 
 import numpy as np
 
-from SuperPang.lib.utils import read_fasta, write_fasta, reverse_complement, print_time
-from SuperPang.lib.Compressor import Compressor
+from superpang.lib.utils import read_fasta, write_fasta, print_time
+from superpang.lib.cutils import reverse_complement
+from superpang.lib.vtools import compress_vertices, vertex_overlap, isInSeqPath
+from superpang.lib.Compressor import Compressor
 
 import graph_tool as gt
 from graph_tool.all import Graph
 
 from mappy import Aligner
-
+from speedict import Rdict, Options, SliceTransform, PlainTableFactoryOptions
 
 ### see if we can put NBPG.clear_filters() inside the set filters method, instead of having a lot of them throughout the code
 
 class Assembler:
 
     ### MULTIPROCESS METHODS
     # In order to save memory minimize serialization/deserialization overheads when multiprocessing we will pass the
@@ -65,165 +67,205 @@
                 res = pool.map(fun, range(len(iterable)))
         cls.clear_multiprocessing_globals()
         return res
     ###############################
 
 
 
-    ##    @profile
-    def __init__(self, fasta, ksize, threads):
+##    @profile
+    def __init__(self, fasta, ksize, threads, diskdb = None, debug = False):
         """
         Build a De-Bruijn Graph from an input fasta file
         """
 
         self.ksize        = ksize
         self.includedSeqs = 0
-        self.hash2vertex  = {}
-        self.vertex2hash  = {}
-        self.seqPaths     = {} # name: pathSet
+        self.seqPaths     = {} # name: compressedVertices
         self.seqLimits    = set()
 
         ### Read input sequences
-        print_time(f'Reading sequences')
+        print_time('Reading sequences')
         self.seqDict = read_fasta(fasta, ambigs = 'as_Ns', Ns = 'split')
         nNs = len({name.split('_Nsplit_')[0] for name in self.seqDict})
+        self.ref2name = list(self.seqDict)
+        max_kmers = sum(len(seq) - self.ksize + 1 for seq in self.seqDict.values())
+        max_kmers = max_kmers if max_kmers < 1000000000 else 1000000000
 
+        print_time('Allocating resources')
         ### Kmer hashing related parameters
         self.compressor = Compressor(self.ksize)
         clength = self.ksize // 4 + self.ksize % 4                # the length of a hash
         maxseqlength = max(len(s) for s in self.seqDict.values()) # length of the largest input sequence
         maxnkmers = maxseqlength-self.ksize+1                     # number of kmers in the largest input sequence
 
-        ### Get kmers from sequences and create DBG
+
+        ### Set up kmer storage
+        self.vertex2coords = np.empty(shape = (max_kmers, 2), dtype = np.uint32)
+        if diskdb:
+            opts = Options()
+            opts.increase_parallelism(threads)
+            opts.set_max_background_jobs(threads)
+            opts.set_prefix_extractor(SliceTransform.create_max_len_prefix(8))
+            opts.set_plain_table_factory(PlainTableFactoryOptions())
+            hash2vertex = Rdict(path = diskdb, options = opts)
+        else:
+            hash2vertex = {}
+
+        ### Set up edge storage
+        maxint    = np.iinfo(np.uint32).max
+        edges     = np.empty(shape = (max_kmers, 2), dtype = np.uint32)
+        edges[:]  = maxint
+
+        ### Go for the eyes, boo!
         print_time(f'Creating DBG from {len(self.seqDict)} sequences ({nNs} originals)')
-        edges = set()
-        totalSize = sum(len(seq) for seq in self.seqDict.values())
-        elapsedSize = 0
-        lastSize = 0
+        includedSeqs   = 0
+        self.seqLimits = set()
+        totalSize      = sum(len(seq) for seq in self.seqDict.values())
+        elapsedSize    = 0
+        lastSize       = 0
+        nVertices      = np.uint32(0)
+        one            = np.uint32(1) # This way increasing the nVertices counter may be slightly faster
+        nEdges         = 0
 
         with SharedMemoryManager() as smm:
             # seqMem and rcSeqMem are two shared mem buffers that will hold the fwd and rev sequences
             #    they are pre-allocated using the size of the largest sequence, for each sequence we will
             #    store/recover the correct amount of bytes according to its length
             # hashMem and revhashMem are two continuous shared mem buffers that will hold all the hashes concatenated
             #    they are pre-allocated using the number of kmers in the largest sequence multiplied by the hash size
             #    to store/recover a particular hash we can just use the right slice of the mem buffer, since hash size is constant
 
             seqMem     = smm.SharedMemory(size=maxseqlength)
             rcSeqMem   = smm.SharedMemory(size=maxseqlength)
             hashMem    = smm.SharedMemory(size=clength*maxnkmers)
-            revhashMem = smm.SharedMemory(size=clength*maxnkmers)
-            self.set_multiprocessing_globals(seqMem, rcSeqMem, hashMem, revhashMem, self.ksize, clength, self.compressor)
+            self.set_multiprocessing_globals(seqMem, rcSeqMem, hashMem, self.ksize, clength, self.compressor)
 
             with Pool(threads) as pool:
-            
-                for name, seq in self.seqDict.items():
-                    elapsedSize += len(seq)
+ 
+                for ref, (name, seq) in enumerate(self.seqDict.items()):
                     if len(seq) <= self.ksize:
+                        elapsedSize += len(seq)
                         continue
                     else:
-                        self.includedSeqs += 1
+                        includedSeqs += 1
                         rcSeq = reverse_complement(seq)
                         seq, rcSeq = seq.encode(), rcSeq.encode()
                         nkmers = len(seq)-self.ksize+1
+                        elapsedSize += len(seq) - nkmers
 
                         seqMem.buf  [:len(seq)  ] = seq
                         rcSeqMem.buf[:len(rcSeq)] = rcSeq
 
                         seq2hashes_ = partial(self.seq2hashes, seqlength=len(seq)) # we can't pass seqlength as a global when forking
                                                                                    #  since it changes for every sequence
                         pool.map(seq2hashes_, range(nkmers))
 
                         # Retrieve the kmer hashes from the memory buffers
                         # Note the use of a generator expression so that all the hashes are not residing in memory at the same time
                         #  ... so we can't close the pool until we finish going through such generator expression!
-                        hashes = (hashMem.buf[i*clength:(i+1)*clength].tobytes() for i in range(nkmers))
-                        revhashes = (revhashMem.buf[i*clength:(i+1)*clength].tobytes() for i in range(nkmers))
-                        
+                        hashes    = (hashMem.buf[i*clength:(i+1)*clength].tobytes() for i in range(nkmers))
                         # Populate the DBG
-                        sp = []
-                        prev = -1 # store the previous vertex here so we can build (prev, v) edge tuples
-                        for h, rh in zip(hashes, revhashes):
-                            if h not in self.hash2vertex and rh not in self.hash2vertex:
-                                v = len(self.hash2vertex)
-                                self.hash2vertex[h] = v
-                                self.vertex2hash[v] = h
-                            elif h in self.hash2vertex:
-                                v = self.hash2vertex[h]
-                            elif rh in self.hash2vertex:
-                                v = self.hash2vertex[rh]
+                        sp = np.empty(nkmers, dtype = np.uint32)
+                        past_first, prev_v, prev_new = False, -1, False # store the previous vertex here so we can build (prev, v) edge tuples
+                        
+                        for idx, h in enumerate(hashes):               
+                            if h in hash2vertex:
+                                newVertex = False
+                                v = hash2vertex[h]
                             else:
-                                raise('wtf')
-                            sp.append(v)
-                            if prev >=0:
-                                edges.add( (prev, v) )
-                                edges.add( (v, prev) )
-                            prev = v
-                                
-                        self.seqPaths[name] = set(sp)
-                        self.seqLimits.add( sp[0]  )
-                        self.seqLimits.add( sp[-1] )
-                                                
-                        if elapsedSize - lastSize > totalSize/100:
-                            print_time(f'\t{round(100*elapsedSize/totalSize, 2)}% bases added, {self.includedSeqs} sequences, {len(self.hash2vertex)} vertices, {len(edges)} edges         ', end = '\r')
-                            lastSize = elapsedSize
-
+                                newVertex = True
+                                v = nVertices
+                                hash2vertex[h] = v
+                                self.vertex2coords[v] = (ref, idx)
+                                nVertices += one
+
+                            sp[idx] = v
+                            
+                            if past_first and (newVertex or prev_new):
+                                edges[nEdges] = prev_v, v
+                                nEdges += 1
+                                prev = v
+
+                            prev_v, prev_new, past_first = v, newVertex, True
+                            if idx == 0:
+                                self.seqLimits.add(v)
+                            if idx == nkmers - 1:
+                                self.seqLimits.add(v)
+
+                            elapsedSize += 1
+                            
+                            if elapsedSize - lastSize > totalSize/100:
+                                print_time(f'\t{round(100*elapsedSize/totalSize, 2)}% bases processed, {includedSeqs} sequences, {nVertices} vertices, {nEdges} edges         ', end = '\r')
+                                lastSize = elapsedSize
+                        self.seqPaths[name] = compress_vertices(sp)
+
+
+        ### Populate DBG and cleanup
+        del seqMem, rcSeqMem, hashMem
+        if diskdb:
+            hash2vertex.close()
+            Rdict.destroy(diskdb, opts)
+        del hash2vertex
         self.clear_multiprocessing_globals()
-        self.DBG = Graph()
-        self.DBG.add_edge_list(edges)
-        self.DBG.ep.efilt = self.DBG.new_edge_property('bool')
-        print_time(f'\t100% bases added, {self.includedSeqs} sequences, {self.DBG.num_vertices()} vertices, {self.DBG.num_edges()} edges         ')
+
+        if debug:
+            for edge in edges[:nEdges]:
+                if maxint in edge:
+                    assert False
         
+        self.DBG = Graph(directed = False)
+        self.DBG.add_edge_list(edges[:nEdges])
+        del edges
+        self.DBG.vp.comp  = self.DBG.new_vertex_property('int16_t')
+        self.DBG.ep.efilt = self.DBG.new_edge_property('bool')
+        print_time(f'\t100% bases processed, {includedSeqs} sequences, {self.DBG.num_vertices()} vertices, {self.DBG.num_edges()} edges         ')
+
 
 ##    @profile
-    def run(self, minlen, mincov, bubble_identity_threshold, genome_assignment_threshold, max_threads):
+    def run(self, minlen, mincov, bubble_identity_threshold, genome_assignment_threshold, max_threads, debug = False):
         """
         Create contigs from a De-Bruijn Graph
         """
 
         Contig = namedtuple('Contig', ['scaffold', 'i', 'seq', 'tseq', 'cov', 'origins', 'successors'])
         contigs = {}
         addedPaths = set()
 
         ### Identify connected components
         print_time('Identifying connected components')
-        vertex2comp = {v: c for v, c in enumerate(gt.topology.label_components(self.DBG, directed = False)[0])}
-        comp2vertices = defaultdict(set)
+        self.DBG.vp.comp = gt.topology.label_components(self.DBG, directed = False)[0]
+        nComps = self.DBG.vp.comp.get_array().max() + 1
         currentScaffold = 0
-        for v, c in vertex2comp.items():
-            comp2vertices[c].add(v)
 
         ### Process connected components
-        for c, vs in comp2vertices.items():
+        for c in range(nComps):
 
-            if False: # DEBUG CODE: Skip unwanted components
+            if False: # _debug CODE: Skip unwanted components
                 TGT_COMP = 2
                 if c + 1 != TGT_COMP:
                     continue
-            
-            print_time(f'Working on comp {c+1}/{len(comp2vertices)}, {len(vs)} vertices')
+            vs = np.where(self.DBG.vp.comp.get_array() == np.int16(c))[0]
+            print_time(f'Working on comp {c+1}/{nComps}, {len(vs)} vertices')
 
             # The overhead of opening a multiprocessing pool increases with resident memory, even if we do nothing inside it
             #  so I don't think this is due to COW being triggered, just something the way fork and/or python multiprocessing pool works
             #  This becomes a problem when I have lots of small components in an otherwise large project, as I pay a large overhead several
             #  times per component. So instead we will use one thread for small-ish components.
             threads = max_threads if len(vs) > 150000 else 1
-            
+
             # Get the seqPaths that appear in this DBG component
             #  just check that the first vertex in the seqPath belongs to this component
-            seqPathsThisComp = {name: sp for name, sp in self.seqPaths.items() if iter(sp).__next__() in vs}
-
+            seqPathsThisComp = {name: sp for name, sp in self.seqPaths.items() if sp[0][0] in vs}
             ### Reconstruct non-branching paths
             print_time('\tCollecting non-branching paths')
             NBPs = []
             inits = set()
             badEdges = set()
-            inits = {v for v, isInit in zip(list(vs), self.multimap(self.is_NBP_init, threads, list(vs), self.DBG, self.seqLimits,
-                                                                    self.vertex2hash, self.compressor)) if isInit}
-
+            inits = {v for v, isInit in zip(vs, self.multimap(self.is_NBP_init, threads, vs, self.DBG, self.seqLimits,
+                                                                     self.vertex2coords, self.ref2name, self.seqDict, self.ksize)) if isInit}
 
             # Break cycle if required
             isCycle = False
             ignoreEdge = set()
             if not inits:
                 #is this a cycle?
                 if min([len(set(self.DBG.get_out_neighbors(v))) for v in vs]) == 2: # no sources or sinks
@@ -247,18 +289,18 @@
             for j, ini in enumerate(inits):
                 for n in set(self.DBG.get_out_neighbors(ini)):
                     p = [ini, n]
                     last = ini
                     while True:
                         if p[-1] in inits:
                             break
-                        s = set(self.DBG.get_out_neighbors(p[-1])) - {last, p[-1]} #p[-1] to avoid stopping at self loops
+                        s = [x for x in self.DBG.get_out_neighbors(p[-1]) if x != last and x != p[-1]][0] #p[-1] to avoid stopping at self loops
                         last = p[-1]
-                        s = s.pop()
-                        p.append(s)
+                        p.append(s) # before we casted to np.uint32, but it doesn't seem to make a big difference memory wise and takes a bit.
+                        #p.append(np.uint32(s))
                     p = tuple(p)
                     NBPs.append(p)
 
             if isCycle: # make them circular by adding the first vertex also in the end so there's an overlap
                 assert len(NBPs) == 2
                 NBPs = [NBP+(NBP[0],) for NBP in NBPs]
 
@@ -270,15 +312,15 @@
             print_time(f'\tBuilding sequence graph out of {len(NBPs)} non-branching paths')
 
             # Remove NBPs with terminally duplicated vertices
             # Those broke our code once. we had three nvs with NBPs (0,0,1,2) (0,1,2) and (2,1,0) under the same pset (see below)
             NBPs = [p for p in NBPs if p[0] != p[1] and p[-1] != p[-2]]
 
             # Translate NBPs into sequences
-            NBP2seq = dict(zip(NBPs, self.multimap(self.reconstruct_sequence, threads, NBPs, self.vertex2hash, self.compressor)))
+            NBP2seq = dict(zip(NBPs, self.multimap(self.reconstruct_sequence, threads, NBPs, self.vertex2coords, self.ref2name, self.seqDict, self.ksize)))
 
             # Collect prefixes-suffixes for locating potential overlaps
             start2NBPs = defaultdict(set) # first k nucleotides
             sStart = {}
             sEnd = {}
             for p, seq in NBP2seq.items():
                 start, end = seq[:self.ksize], seq[-self.ksize:]
@@ -294,37 +336,37 @@
                 assert p not in NBP2vertex
                 NBP2vertex[p] = int(NBPG.add_vertex())
             for p1 in NBPs:
                 for p2 in start2NBPs[sEnd[p1]]:
                     NBPG.add_edge(NBP2vertex[p1], NBP2vertex[p2])
                            
             vertex2NBP = {v: p for p,v in NBP2vertex.items()}
-
-
+                
             ### Write component's input sequences, DBG and NBPG
             if False:
                 oris = {ori for oris in self.multimap(self.get_vertex2origins, threads, list(vs), seqPathsThisComp, single_thread_threshold = 10000) for ori in oris}
                 with open(f'comp_{c+1}.fasta', 'w') as outfile:
                     for ori in oris:
                         outfile.write(f'>{ori}\n{self.seqDict[ori]}\n')
                 self.DBG.vp.vfilt = self.DBG.new_vertex_property('bool')
-                self.set_vertex_filter(self.DBG, vs)
+                self.set_vertex_filter(self.DBG, set(vs))
                 DBG2 = Graph(self.DBG, prune = True)
                 print(f'DBG: {DBG2.num_vertices()} vertices, {DBG2.num_edges()} edges')
                 DBG2.save(f'comp_{c+1}.DBG.graphml')
                 print(f'NBPG: {NBPG.num_vertices()} vertices, {NBPG.num_edges()} edges')
                 NBPG.save(f'comp_{c+1}.NBPG.graphml')
+            del vs
 
 
             ### Extract forward component
             def get_psets(nvs):
                 """Get a dict with a frozenset of vertices as keys, and the two complementary non-branching paths sharing those vertices as values"""
                 psets = defaultdict(list)
                 for nv in nvs:
-                    pset = frozenset(vertex2NBP[nv])
+                    pset = hash(frozenset(vertex2NBP[nv]))
                     psets[pset].append(nv)
                 for nvs_ in psets.values():
                     assert len(nvs_) == 2
                 return psets
 
 
             print_time('\tExtracting forward component')
@@ -341,40 +383,40 @@
             rcComps = {}
             for nc1, nc2 in combinations(comp2nvs,2):
                 v1 = {v for nv in comp2nvs[nc1] for v in vertex2NBP[nv]}
                 v2 = {v for nv in comp2nvs[nc2] for v in vertex2NBP[nv]}
                 if v1 == v2:
                     rcComps[nc1] = nc2
                     rcComps[nc2] = nc1
-
+                del v1, v2
+            
             # Count how many times each Non-Branching Path is in the same orientation as the input sequences
             nv2rightOrientation = defaultdict(int)
             added = set()
             for nc1, nc2 in rcComps.items(): # For now we only do it for the components with a clear RC
                 if nc1 in added:
                     continue
                 # Find reverse complement Non-Branching Paths
                 psets = get_psets(comp2nvs[nc1] | comp2nvs[nc2])
                 assert len(psets) == len(comp2nvs[nc1]) == len(comp2nvs[nc1]) # each sequence path should have a reverse complement equivalent (same vertices in the kmer graph, reverse order)
                 # Count
                 names = list(seqPathsThisComp.keys())
                 stt = threads if len(psets) > threads else 1000000000
                 for spGS in dict(zip(names, self.multimap(self.get_seqPaths_NBPs, threads, names, seqPathsThisComp, psets, NBP2seq, vertex2NBP, self.seqDict, single_thread_threshold = stt))):
                     for nv in spGS:
-                        nv2rightOrientation[nv] += 1            
+                        nv2rightOrientation[nv] += 1
             
 
             # If we didn't find a RC for all components this means that in some case fwd and rev are joined in the same component
             noRC = {nc for nc in comp2nvs if nc not in rcComps} 
             for nc in noRC: # for each of those evil components...
 
                 # Find reverse complement Non-Branching Paths
-                psets = get_psets(comp2nvs[nc])               
+                psets = get_psets(comp2nvs[nc])             
                 assert len(psets) == len(comp2nvs[nc]) / 2 # each sequence path should have a reverse complement equivalent (same vertices in the kmer graph, reverse order)
-                
                 nv2rc = {}
                 for nv1, nv2 in psets.values():
                     nv2rc[nv1] = nv2
                     nv2rc[nv2] = nv1
                 self.set_vertex_filter(NBPG, comp2nvs[nc])
                 assert {int(nv) for nv in NBPG.vertices()} == comp2nvs[nc] # did we alter nv indices when filtering?
                 assert(len(set(gt.topology.label_components(NBPG, directed = False)[0]))) == 1 # check that this is only one component
@@ -394,20 +436,16 @@
                         nv2rightOrientation[nv] += 1
                         addedNodes.update( (nv, nv2rc[nv]) )
                     
                 # Add nodes in the sequence graph that weren't fully contained in an original sequence
                 for nv in comp2nvs[nc] - addedNodes:
                     fakeName = hash( (len(seqPaths_NBPs), nv) )
                     seqPaths_NBPs[fakeName] = {nv} | set(NBPG.get_all_neighbors(nv)) # add its neighbors so that it'll overlap with the real sequences in at least one nv
-                
-                seqPaths_NBPs_rev = {name: {nv2rc[nv] for nv in nvs} for name, nvs in seqPaths_NBPs.items()}
-
-                x = {nv for nvs in seqPaths_NBPs.values() for nv in nvs}
-                y = {nv2rc[nv] for nv in x}
 
+                seqPaths_NBPs_rev = {name: {nv2rc[nv] for nv in nvs} for name, nvs in seqPaths_NBPs.items()}
                 
                 # Separate fwd and rev
                 nvs1 = set()
                 refSeqNames = sorted(seqPaths_NBPs, key = lambda name: len(seqPaths_NBPs[name]), reverse = True) # sort by decreasing number of nodes in the NBPG
 
                 addedNames = {refSeqNames[0]}
                 nvs1.update(seqPaths_NBPs[refSeqNames[0]]) # start from the longest seq
@@ -431,16 +469,14 @@
                     addedNames.add(best_name)
                     best_nvs = {nv for nv in best_nvs if nv2rc[nv] not in nvs1} # don't add reverse complements at this stage
                                                                                 # some are really there and needed to keep everything into a single component
                                                                                 # some will be duplications (e.g. because one of the input genomes has an inverted region)
                     nvs1.update(best_nvs)
 
                 nvs2 = {nv2rc[nv] for nv in nvs1}
-                v1 = {v for nv in nvs1 for v in vertex2NBP[nv]}
-                v2 = {v for nv in nvs2 for v in vertex2NBP[nv]}
 
                 assert (nvs1 | nvs2) == comp2nvs[nc]
 
                 # Identify subcomponents in nv1
                 NBPG.clear_filters()
                 self.set_vertex_filter(NBPG, nvs1)
                 subcomps1 = defaultdict(set)
@@ -451,18 +487,16 @@
                 self.set_vertex_filter(NBPG, nvs2)
                 subcomps2 = defaultdict(set)
                 for nv,c in zip(NBPG.vertices(), gt.topology.label_components(NBPG, directed = False)[0]):
                     subcomps2[c].add(nv)
                 NBPG.clear_filters()
                 # Identify RC components
                 assert len(subcomps1) == len(subcomps2)
-                
-                subcomp2vertex1 = {snc1: {v for nv in snvs1 for v in vertex2NBP[nv]} for snc1, snvs1 in subcomps1.items()} # so we don't have to compute this inside the loop
-                subcomp2vertex2 = {snc2: {v for nv in snvs2 for v in vertex2NBP[nv]} for snc2, snvs2 in subcomps2.items()}
 
+                
                 # Try to merge into one fwd and one rev subcomp
                 # In some cases the fwd and rev sequences can be actually be present in the same genome
                 # So we identify the largest fwd subcomponent, throw in the rest of components in fwd and rev, and hope that they become connected when everything is together
                 largestSubcomp = list(sorted(subcomps1, key = lambda snc: len(subcomps1[snc]), reverse = True))[0]
                 combined = subcomps1[largestSubcomp]
                 for snc in subcomps1:
                     if snc != largestSubcomp:
@@ -493,21 +527,24 @@
                 subcomps1_corrected = {c: nvs for c, nvs in subcomps1_corrected.items() if c not in bad1}
                 subcomps2_corrected = {c: nvs for c, nvs in subcomps2_corrected.items() if c not in bad2}
 
                 # Keep going
                 subcomps1 = subcomps1_corrected
                 subcomps2 = subcomps2_corrected
 
-                subcomp2vertex1 = {snc1: {v for nv in snv1 for v in vertex2NBP[nv]} for snc1, snv1 in subcomps1.items()} # so we don't have to compute this inside the loop
-                subcomp2vertex2 = {snc2: {v for nv in snv2 for v in vertex2NBP[nv]} for snc2, snv2 in subcomps2.items()}   
 
                 # Assertions
-                v1 = set.union(*list(subcomp2vertex1.values()))
-                v2 = set.union(*list(subcomp2vertex2.values()))
-                assert v1 == v2
+                if debug:
+                    subcomp2vertex1 = {snc1: {v for nv in snv1 for v in vertex2NBP[nv]} for snc1, snv1 in subcomps1.items()}
+                    subcomp2vertex2 = {snc2: {v for nv in snv2 for v in vertex2NBP[nv]} for snc2, snv2 in subcomps2.items()}
+                    v1 = set.union(*list(subcomp2vertex1.values()))
+                    v2 = set.union(*list(subcomp2vertex2.values()))
+                    assert v1 == v2
+                    del subcomp2vertex1, subcomp2vertex2
+
 
                 for snvs1, snvs2 in combinations(subcomps1.values(), 2):
                     assert not snvs1 & snvs2 # if they are not RC they should not share any paths
                 for snvs1, snvs2 in combinations(subcomps2.values(), 2):
                     assert not snvs1 & snvs2 # if they are not RC they should not share any paths
 
                 
@@ -519,30 +556,31 @@
                     for nc2, nvs in comp2nvs.items(): # they should not share any paths with other components in the sequence graph either
                         if nc2 != nc:
                             assert not nvs & snv2
 
                 NBPG.clear_filters()                
 
                 first = True
-                for snc1, snv1 in subcomps1.items():
-                    v1 = subcomp2vertex1[snc1]
-                    for snc2, snv2 in subcomps2.items():
-                        v2 = subcomp2vertex2[snc2]
+                for snv1 in subcomps1.values():
+                    v1 = sorted([v for nv in snv1 for v in vertex2NBP[nv]]) # list instead of set to reduce memory usage
+                    for snv2 in subcomps2.values():                         #  but ofc it sucks
+                        v2 = sorted([v for nv in snv2 for v in vertex2NBP[nv]])
                         if v1 == v2:
                             i1 = nc if first else len(comp2nvs) # recycle the previous component index for nc1
                             comp2nvs[i1] = snv1
                             first = False
                             i2 = len(comp2nvs)
                             comp2nvs[i2] = snv2
                             rcComps[i1] = i2
                             rcComps[i2] = i1
                             break
                     else: # assert that all our subcomponents have RC components
                         assert False
-                
+
+                del v1, v2
                 NBPG.clear_filters()
 
             assert len(rcComps) == len(comp2nvs) # all our components have a rc component, splitting was successful
 
             # For each pair of RC component, we select the component with the most Non-Branching paths in the same orientation as the input sequences
             compS2paths = {}
             for nc1, nc2 in rcComps.items():
@@ -555,28 +593,32 @@
                 compS2paths[currentScaffold] =  {vertex2NBP[nv] for nv in comp2nvs[fwd]}
                 added.add(nc1)
                 added.add(nc2)
                 currentScaffold += 1
                 
 
             # Check that we included all the input vertices
-            assert vs == {v for p in NBPs for v in p}
+            if debug:
+                vs = {np.uint32(v) for v, c_ in enumerate(self.DBG.vp.comp) if c_ == c}
+                assert set(vs) == {v for p in NBPs for v in p}
             # Check that no paths appear in two different scaffolds
             for cs1, cs2 in combinations(compS2paths, 2):
                 assert not compS2paths[cs1] & compS2paths[cs2]
 
 
             ### Process each scaffold in the sequence graph
             for scaffold, NBPs in compS2paths.items():
                 # Test that the scaffolds are really connected
                 NBPG.clear_filters() # NEVER FORGET!!!
                 self.set_vertex_filter(NBPG, {NBP2vertex[p] for p in NBPs})
                 msg = f'\tScaffold {scaffold}, {NBPG.num_vertices()} NBP vertices, {NBPG.num_edges()} NBP edges'
                 print_time(msg, end = '\r')
-                assert len(set(gt.topology.label_components(NBPG, directed = False)[0])) == 1
+
+                if debug:
+                    assert len(set(gt.topology.label_components(NBPG, directed = False)[0])) == 1
 
                 # Compute scaffold length and skip if too short
                 scaffoldLen = 0
                 for p in NBPs:
                     seq = NBP2seq[p]
                     if NBPG.get_out_neighbors(NBP2vertex[p]).shape[0]:
                         seq = seq[:-self.ksize] # trim the overlap unless this is a terminal node
@@ -598,15 +640,17 @@
                 
                 print_time(msg, end='\r')
                 
                 # Identify and flatten bubbles
                 sortBy = 'length'         # can be 'length' or 'cov'.
                 bubble_paths_all = list() # length had slighly higher assembly completeness when I tested it, and is faster
                 bubble_paths     = set()
-                bubble_vertex2origins = defaultdict(set) # Keep track of the new ones here, the originals are calculated on the fly to save memory
+                bubble_vertex2origins = defaultdict(list) # Keep track of the new ones here,
+                                                          #  the originals are calculated on the fly to save memory
+                                                          #  use list instead of set to save memory
                 if bubble_identity_threshold and bubble_identity_threshold < 1:
                     path_limits = defaultdict(list)
                     for p in NBPs:
                         path_limits[(p[0], p[-1])].append(p)
                     for (start, end), ps in path_limits.items():
                         if len(ps) > 1: # more than one path with similar start and end
                             bubble_paths_all.extend(ps)
@@ -620,48 +664,47 @@
                                 ps = sorted(ps, key = lambda x: len(x), reverse = True)
                             elif sortBy == 'cov':
                                 ps = sorted(ps, key = lambda x: path2cov[x], reverse = True)
                             else:
                                 assert False
                             p1 = ps[0] # the longest / most covered one
                             s1 = NBP2seq[p1][self.ksize:-self.ksize] # remove the first and last kmer
-                            ref = Aligner(seq = s1, n_threads = 1)
+                            ref = Aligner(seq = s1, preset = 'sr', n_threads = 1)
                             newOris = set()
                             for p2 in ps[1:]:
                                 s2 = NBP2seq[p2][self.ksize:-self.ksize]
                                 al = list(ref.map(s2)) 
                                 if not al:
                                     continue
                                 mlen = sum(a.mlen for a in al)
                                 if mlen/len(s2) >= bubble_identity_threshold: # note that s2 might be smaller than s1 if sorting by cov, so I should correct this
                                     bubble_paths.add(p2)  
                                     m1 += 1
                                     newOris.update( {ori for v2 in p2 for ori in self.vertex2origins(v2, seqPathsThisComp)} )
                             for v1 in p1:
-                                bubble_vertex2origins[v1].update(newOris) # count vertices in p1 as appearing in all of the origins in the bubble paths that we just discarded
-                                    
+                                bubble_vertex2origins[v1].extend(newOris) # count vertices in p1 as appearing in all of the origins in the bubble paths that we just discarded
+                           
                     NBPs = [p for p in NBPs if p not in bubble_paths]
                     msg += f', removed {m1} bubbles'
                     print_time(msg, end = '\r')
                     NBPG.clear_filters()
                     self.set_vertex_filter(NBPG, {NBP2vertex[p] for p in NBPs})
 
                 
 
                 # Join contiguous non-branching paths (can happen after solving the fwd component and popping bubbles
-                predecessors = defaultdict(set)
-                successors = defaultdict(set)
+                predecessors = defaultdict(list)
+                successors = defaultdict(list)
                 for p1 in NBPs:
                     for nv2 in NBPG.get_out_neighbors(NBP2vertex[p1]):
                         if vertex2NBP[nv2] not in bubble_paths:
-                            successors[p1].add(vertex2NBP[nv2])
+                            successors[p1].append(vertex2NBP[nv2])
                     for nv2 in NBPG.get_in_neighbors(NBP2vertex[p1]):
                         if vertex2NBP[nv2] not in bubble_paths:
-                            predecessors[p1].add(vertex2NBP[nv2])
-
+                            predecessors[p1].append(vertex2NBP[nv2])
                 
                 extenders = {p for p in NBPs if len(successors[p]) <= 1 and (successors[p] or predecessors[p])}
                 extenders = extenders | {p for p in NBPs if len(predecessors[p]) == 1} ### added later, consider removing this line if we start failing assertions
                 joinStarters =  {p for p in extenders if len(predecessors[p]) != 1 or len(successors[list(predecessors[p])[0]]) > 1}
 
                 if not joinStarters: # Is this a cycle
                     if min(len(ps) for ps in predecessors.values()) == 1: # This does not cover the case in which there is a cycle but also a linear component
@@ -674,36 +717,36 @@
                 newPaths = []
                 
                 visited = set()
                 for start in joinStarters:
                     new_path = start
                     end = start
                     succs = successors[start]
-                    succ = list(succs)[0] if succs else None
+                    succ = succs[0] if succs else None
                     extended = False
                     while succ in joinExtenders:
                         extended = True
                         visited.add(succ)
                         new_path += succ[1:]
                         end = succ
                         succs = successors[succ]
-                        succ = list(succs)[0] if succs else None
+                        succ = succs[0] if succs else None
                     NBPs.append(new_path)
                     if extended:
                         sStart[new_path] = sStart[start]
                         sEnd[new_path] = sEnd[end]
                         newPaths.append(new_path)
                         predecessors[new_path] = predecessors[start]
                         for pred in predecessors[new_path]:
-                            successors[pred].add(new_path)
+                            successors[pred].append(new_path)
                         successors[new_path] = successors[end]
                         for succ in successors[new_path]:
-                            predecessors[succ].add(new_path)
+                            predecessors[succ].append(new_path)
 
-                NBP2seq.update(dict(zip(newPaths, self.multimap(self.reconstruct_sequence, threads, newPaths, self.vertex2hash, self.compressor))))
+                NBP2seq.update(dict(zip(newPaths, self.multimap(self.reconstruct_sequence, threads, newPaths, self.vertex2coords, self.ref2name, self.seqDict, self.ksize))))
                         
 
                 assert visited == joinExtenders
 
                 # Update scaffold graph
                 pathSet = set(NBPs)
                 for p, preds in predecessors.items():
@@ -752,17 +795,18 @@
                     if p not in keep_right:
                         tp = tp[:-1]
                     if p in trim_left:
                         tp = tp[1:]
                     assert tp
                     trimmedPaths.append(tp)
 
-                vs = {v for p in NBPs for v in p}
-                vst = {v for p in trimmedPaths for v in p}
-                assert vs == vst
+                if debug:
+                    vs = {v for p in NBPs for v in p}
+                    vst = {v for p in trimmedPaths for v in p}
+                    assert vs == vst
                 
                 trimmedSeqs = []
                 for p in NBPs:
                     tseq = NBP2seq[p]
                     if p not in keep_right:
                         tseq = tseq[:-self.ksize]
                     if p in trim_left:
@@ -775,15 +819,16 @@
                 path2id  = {p: (scaffold, i) for i, p in enumerate(NBPs)}
                 ori2covs = self.multimap(self.get_ori2cov, threads, trimmedPaths, seqPathsThisComp, bubble_vertex2origins)
                 # Using trimmedPaths/trimmedSeqs: don't take into account overlaps with other paths for mean cov calculation and origin reporting
                 
                 foundOris = set()
 
                 for p, ori2cov, tseq in zip(NBPs, ori2covs, trimmedSeqs):
-                    assert p not in addedPaths
+                    if debug:
+                        assert p not in addedPaths
                     id_ = path2id[p]
                     # Even for complete genomes, we can have non-branching paths that belong to the core but don't have full coverage in some sequences
                     # This can happen if there are missing bases at the beginning or end of some of the input sequences (contigs in the original assemblies)
                     # So there is no branching, but some are missing
                     avgcov = sum(ori2cov.values())
                     goodOris = {ori for ori, cov in ori2cov.items() if cov >= genome_assignment_threshold}
                     goodOris.add( list(sorted(ori2cov, key = lambda ori: ori2cov[ori], reverse = True))[0] ) # add at least the origin with the highest cov
@@ -792,15 +837,17 @@
                     contigs[id_] = Contig(scaffold   = id_[0],
                                           i          = id_[1],
                                           seq        = NBP2seq[p],
                                           tseq       = tseq,
                                           cov        = avgcov,
                                           origins    = goodOris,
                                           successors = [path2id[succ] for succ in successors[p]])
-                    addedPaths.add(p)
+                    
+                    if debug:
+                        addedPaths.add(p)
 
                 msg += ', done'
                 print_time(msg)
 
         ### Finished!
         return contigs
 
@@ -817,23 +864,25 @@
         NBPG.set_vertex_filter(NBPG.vp.vfilt)
 
 
     @classmethod
     def seq2hashes(cls, i, seqlength):
         """
         Obtain sequence hashes for the kmers of a forward and a reverse sequence
-        Stores results in two shared memory buffers
+        Stores results in a shared memory buffer
         """
         # hashMem and revhashMem are two continuous shared mem buffers that will hold all the hashes concatenated
         # for each index, we just read/write from/to the proper slices, since hash size is constant
-        seqMem, rcSeqMem, hashMem, revhashMem, ksize, clength, compressor = cls.get_multiprocessing_globals()
+        seqMem, rcSeqMem, hashMem, ksize, clength, compressor = cls.get_multiprocessing_globals()
         seq, rcSeq = seqMem.buf[:seqlength], rcSeqMem.buf[:seqlength]
         ri = len(rcSeq) - i - ksize
-        hashMem.buf[i*clength:(i+1)*clength] = compressor.compress(seq[i:i+ksize])
-        revhashMem.buf[i*clength:(i+1)*clength] = compressor.compress(rcSeq[ri:ri+ksize])
+        h  = compressor.compress(seq[i:i+ksize])
+        rh = compressor.compress(rcSeq[ri:ri+ksize])
+        h = h if h >= rh else rh
+        hashMem.buf[i*clength:(i+1)*clength] = h
 
 
     @classmethod
     def is_NBP_init(cls, i):
         """
         Check if a given vertex of a DBG will be a non-branching path init
         This will happen if
@@ -844,15 +893,15 @@
               last kmer
             - So original sequences were kA->kB, kC->kB (where kA,kB,kC are kmers)
             - But due to how we build our DBG, the DBG ends up being A=B=C (where = denotes a
                bidirectional link)
             - But a sequence can not really be reconstructed for the paths A->B->C or C->B->A
             - So we mark B as an init even if it looks like an extender in the DBG
         """
-        vs, DBG, seqLimits, vertex2hash, compressor = cls.get_multiprocessing_globals()
+        vs, DBG, seqLimits, vertex2coords, ref2name, seqDict, ksize = cls.get_multiprocessing_globals()
         v = vs[i]
         succs = set(DBG.get_out_neighbors(v)) - {v} # - {v} to avoid self loops being init points
         isInit = False
         if len(succs) != 2: 
             isInit = True
         elif v in seqLimits:
             # We are reconstructing the sequence for the edges B->A and B->C
@@ -860,85 +909,87 @@
             #  so A,C are successors of B
             # Normally when reconstructing B->A and B->C, the valid kmer for B would be in forward
             #  orientation in one case, and in reverse complement orientation in the other,
             #  so len(kmers) == 2
             # However if the node is a fake extender, the valid kmer for B will be the same in
             #  B->A and B->C
             kmers = set()
-            k1x = cls.vertex2kmer(v, vertex2hash, compressor)
+            k1x = cls.vertex2kmer(v, vertex2coords, ref2name, seqDict, ksize)
             for s in succs:
                 for k1 in (k1x, reverse_complement(k1x)):
-                    ext = cls.extendKmer(k1,s,vertex2hash, compressor)
+                    ext = cls.extendKmer(k1, s, vertex2coords, ref2name, seqDict, ksize)
                     if ext:
                         kmers.add(k1)
             if len(kmers) == 1:
                 isInit = True
         return isInit
 
 
     @classmethod
     def reconstruct_sequence(cls, i):
         """
         Reconstruct a nucleotide sequence for a De-Bruijn Graph path
         """
-        NBPs, vertex2hash, compressor = cls.get_multiprocessing_globals()
+        NBPs, vertex2coords, ref2name, seqDict, ksize = cls.get_multiprocessing_globals()
         path = NBPs[i]
         kmers = []
         # Each vertex corresponds to two kmers (fwd and rev)
         # Which kmers give us a meaningful sequence?
         # We are reading this in a given direction (from path[0] to path[-1])
         # For the starting kmer (in position 0), pick the one that overlaps with any of the two kmers in position 1
-        kmers = cls.edge2kmer(path[0], path[1], vertex2hash, compressor)
+        kmers = cls.edge2kmer(path[0], path[1],  vertex2coords, ref2name, seqDict, ksize)
         
         # Then just keep advancing in the path, for each vertex pick the kmer that overlaps with the previously-picked kmer
         for v in path[2:]:
-            kmers.append(cls.extendKmer(kmers[-1], v, vertex2hash, compressor, force = True))
+            kmers.append(cls.extendKmer(kmers[-1], v, vertex2coords, ref2name, seqDict, ksize, force = True))
             
         assert len(kmers) == len(path) # We can remove this assertion, since edge2kmer and extendKmer(force=True)
                                        #  have internal assertions
         
         return cls.seq_from_kmers(kmers)
 
 
     @classmethod
-    def vertex2kmer(cls, v, vertex2hash, compressor):
+    def vertex2kmer(cls, v, vertex2coords, ref2name, seqDict, ksize):
         """
         Return the kmer corresponding to a given vertex in the De-Bruijn Graph
         """
-        return compressor.decompress(vertex2hash[v])
+        ref, idx = vertex2coords[v]
+        name = ref2name[ref]
+        return seqDict[name][ idx : (idx + ksize) ]
 
 
     @classmethod
-    def edge2kmer(cls, v1, v2, vertex2hash, compressor):
+    def edge2kmer(cls, v1, v2,  vertex2coords, ref2name, seqDict, ksize):
         """
         Return the kmers corresponding to a given edge in the De-Bruijn Graph
         """
         # Each vertex corresponds to two kmers (fwd and rev)
         # Which kmers give us a meaningful sequence?
         # We are reading this in a given direction (from path[0] to path[-1])
         # For the starting kmer (in position 0), pick the one that overlaps with any of the two kmers in position 1
         kmers = []
-        k1x = cls.vertex2kmer(v1, vertex2hash, compressor)
+        k1x = cls.vertex2kmer(v1, vertex2coords, ref2name, seqDict, ksize)
         for k1 in (k1x, reverse_complement(k1x)):
-            k2 = cls.extendKmer(k1, v2, vertex2hash, compressor)
+            k2 = cls.extendKmer(k1, v2,  vertex2coords, ref2name, seqDict, ksize)
             if k2:
                 kmers.extend([k1, k2])
         
         assert len(kmers) == 2
         return kmers
 
 
     @classmethod
-    def extendKmer(cls, k1, v2, vertex2hash, compressor, force = False):
+    def extendKmer(cls, k1, v2, vertex2coords, ref2name, seqDict, ksize, force = False):
         """
         Return the kmer that extends a given first kmer k1, where k1 is a 
          kmer coming from a vertex v1, and v1,v2 is an edge in the De-Bruijn Graph
         """
         kmers = []
-        k2x = cls.vertex2kmer(v2, vertex2hash, compressor)
+        k2x = cls.vertex2kmer(v2, vertex2coords, ref2name, seqDict, ksize)
         for k2 in (k2x, reverse_complement(k2x)):
             if k2[:-1] == k1[1:]:
                 kmers.append(k2)
         if force:
             assert len(kmers) == 1
         else:
             assert len(kmers) <= 1 # can be 0 if k1 is in the wrong orientation
@@ -952,27 +1003,30 @@
         """
         fullseq = [kmers[0]]
         extra = [kmer[-1] for kmer in kmers[1:]]
         fullseq.extend(extra)
         return ''.join(fullseq)
 
     
-
     @classmethod
+##    @profile
     def get_seqPaths_NBPs(cls, i):
         """
         Return the vertices in the Sequence Graph that are contained in a given input sequence in its original orientation
         """
         names, seqPaths, psets, NBP2seq, vertex2NBP, seqDict = cls.get_multiprocessing_globals()
         name = names[i]
-        path = seqPaths[name]     
+        seqPath = seqPaths[name]     
         
         spGS = set()
         for pset, (nv1, nv2) in psets.items():
-            if pset.issubset(path):
+            NBP = vertex2NBP[nv1]
+            cNBP = compress_vertices(np.array(NBP, dtype=np.uint32))
+            refLen = len(NBP) if NBP[0] != NBP[-1] else len(NBP) - 1 # A NBP will only have duplicated vertices if it is circular
+            if vertex_overlap(cNBP, seqPaths[name]) == refLen: # the pset is a subset of the seqPath.
                 for nv in (nv1, nv2):
                     if NBP2seq[vertex2NBP[nv]] in seqDict[name]: # check the string to make sure that we only add nodes from the same orientation
                         spGS.add(nv)
                         break
         return spGS
 
 
@@ -991,43 +1045,34 @@
     @classmethod
     def get_ori2cov(cls, i):
         """
         For a given path in the De-Bruijn Graph, calculate the fraction of its vertices that are contained in each input sequence
         """
         NBPs, seqPaths, bubble_vertex2origins = cls.get_multiprocessing_globals()
         path = NBPs[i]
-
-##        # Pre-screen the seqPaths before the big analysis
-##        # This may save time? It saved 1 second (over 20) for the test dataset...
-##        if len(path) > 10:
-##            pset = {v for i, v in enumerate(path) if not i % 20} | {path[-1]}
-##        else:
-##            pset = {path[0], path[len(path)//2], path[-1]}
-##        candidates = {name: sp for name, sp in seqPaths.items() if pset & sp}
-##        seqPaths = candidates
         
         ori2cov = defaultdict(int)
         for v in path:
-            for ori in cls.vertex2origins(v, seqPaths) | bubble_vertex2origins[v]: # note how I'm also getting origins not really associated to this path
-                ori2cov[ori] += 1                                               # but to bubbles that were originally in this path before we popped them
+            for ori in cls.vertex2origins(v, seqPaths) | set(bubble_vertex2origins[v]): # note how I'm also getting origins not really associated to this path
+                ori2cov[ori] += 1                                                       # but to bubbles that were originally in this path before we popped them
         return {ori: cov/len(path) for ori, cov in ori2cov.items()}
 
 
     @classmethod
     def get_vertex2origins(cls, i):
         vertices, seqPaths = cls.get_multiprocessing_globals()
         return cls.vertex2origins(vertices[i], seqPaths)
         
 
     @classmethod
     def vertex2origins(cls, v, seqPaths):
         """
         Return the names of the input sequences that contain a given vertex in the De-Bruijn Graph
         """
-        return {name for name in seqPaths if v in seqPaths[name]}
+        return {name for name in seqPaths if isInSeqPath(v, seqPaths[name])}
 
 
 
     @classmethod
     def get_vertex2originslen(cls, i):
         """
         Return the number of input sequences that contain a given vertex in the De-Bruijn Graph
```

### Comparing `SuperPang-0.9.6/SuperPang/lib/Compressor.c` & `SuperPang-1.0.0/src/superpang/lib/Compressor.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
-        "name": "SuperPang.lib.Compressor",
+        "name": "superpang.lib.Compressor",
         "sources": [
-            "SuperPang/lib/Compressor.pyx"
+            "src/superpang/lib/Compressor.pyx"
         ]
     },
-    "module_name": "SuperPang.lib.Compressor"
+    "module_name": "superpang.lib.Compressor"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,14 +58,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -86,29 +87,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -141,18 +147,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -164,15 +216,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -203,15 +255,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -326,17 +378,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -406,14 +455,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -513,35 +567,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -699,16 +753,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__SuperPang__lib__Compressor
-#define __PYX_HAVE_API__SuperPang__lib__Compressor
+#define __PYX_HAVE__superpang__lib__Compressor
+#define __PYX_HAVE_API__superpang__lib__Compressor
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
@@ -946,15 +1000,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "SuperPang/lib/Compressor.pyx",
+  "src/superpang/lib/Compressor.pyx",
   "stringsource",
   "array.pxd",
   "__init__.pxd",
   "type.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
@@ -968,51 +1022,47 @@
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* Atomics.proto */
 #include <pythread.h>
 #ifndef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 1
 #endif
+#define __PYX_CYTHON_ATOMICS_ENABLED() CYTHON_ATOMICS
 #define __pyx_atomic_int_type int
-#if CYTHON_ATOMICS && __GNUC__ >= 4 && (__GNUC_MINOR__ > 1 ||\
-                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL >= 2)) &&\
-                    !defined(__i386__)
-    #define __pyx_atomic_incr_aligned(value, lock) __sync_fetch_and_add(value, 1)
-    #define __pyx_atomic_decr_aligned(value, lock) __sync_fetch_and_sub(value, 1)
+#if CYTHON_ATOMICS && (__GNUC__ >= 5 || (__GNUC__ == 4 &&\
+                    (__GNUC_MINOR__ > 1 ||\
+                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL__ >= 2))))
+    #define __pyx_atomic_incr_aligned(value) __sync_fetch_and_add(value, 1)
+    #define __pyx_atomic_decr_aligned(value) __sync_fetch_and_sub(value, 1)
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
-#elif CYTHON_ATOMICS && defined(_MSC_VER) && 0
-    #include <Windows.h>
+#elif CYTHON_ATOMICS && defined(_MSC_VER) && CYTHON_COMPILING_IN_NOGIL
+    #include <intrin.h>
     #undef __pyx_atomic_int_type
-    #define __pyx_atomic_int_type LONG
-    #define __pyx_atomic_incr_aligned(value, lock) InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) InterlockedDecrement(value)
+    #define __pyx_atomic_int_type long
+    #pragma intrinsic (_InterlockedExchangeAdd)
+    #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
+    #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
-#elif CYTHON_ATOMICS && (defined(__ICC) || defined(__INTEL_COMPILER)) && 0
-    #define __pyx_atomic_incr_aligned(value, lock) _InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) _InterlockedDecrement(value)
-    #ifdef __PYX_DEBUG_ATOMICS
-        #warning "Using Intel atomics"
-    #endif
 #else
     #undef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 0
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Not using atomics"
     #endif
 #endif
 typedef volatile __pyx_atomic_int_type __pyx_atomic_int;
 #if CYTHON_ATOMICS
     #define __pyx_add_acquisition_count(memview)\
-             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview))
     #define __pyx_sub_acquisition_count(memview)\
-            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview))
 #else
     #define __pyx_add_acquisition_count(memview)\
             __pyx_add_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
             __pyx_sub_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
 #endif
 
@@ -1061,211 +1111,193 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":716
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":720
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
-/* "SuperPang/lib/Compressor.pyx":10
+/* "superpang/lib/Compressor.pyx":10
  * cimport numpy as np
  * DTYPE = np.uint8
  * ctypedef np.uint8_t DTYPE_t             # <<<<<<<<<<<<<<
  * 
  * cdef class Compressor:
  */
-typedef __pyx_t_5numpy_uint8_t __pyx_t_9SuperPang_3lib_10Compressor_DTYPE_t;
+typedef __pyx_t_5numpy_uint8_t __pyx_t_9superpang_3lib_10Compressor_DTYPE_t;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
@@ -1288,74 +1320,74 @@
 
 
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
-struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor;
+struct __pyx_obj_9superpang_3lib_10Compressor_Compressor;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "SuperPang/lib/Compressor.pyx":12
+/* "superpang/lib/Compressor.pyx":12
  * ctypedef np.uint8_t DTYPE_t
  * 
  * cdef class Compressor:             # <<<<<<<<<<<<<<
  *     """
  *     Hash a nucleotide sequence into a compressed form
  */
-struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor {
+struct __pyx_obj_9superpang_3lib_10Compressor_Compressor {
   PyObject_HEAD
-  struct __pyx_vtabstruct_9SuperPang_3lib_10Compressor_Compressor *__pyx_vtab;
+  struct __pyx_vtabstruct_9superpang_3lib_10Compressor_Compressor *__pyx_vtab;
   Py_ssize_t ksize;
   Py_ssize_t com;
   Py_ssize_t rem;
   Py_ssize_t clength;
 };
 
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 struct __pyx_array_obj {
@@ -1372,28 +1404,28 @@
   PyObject *_format;
   void (*callback_free_data)(void *);
   int free_data;
   int dtype_is_object;
 };
 
 
-/* "View.MemoryView":279
+/* "View.MemoryView":280
  * 
  * @cname('__pyx_MemviewEnum')
  * cdef class Enum(object):             # <<<<<<<<<<<<<<
  *     cdef object name
  *     def __init__(self, name):
  */
 struct __pyx_MemviewEnum_obj {
   PyObject_HEAD
   PyObject *name;
 };
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 struct __pyx_memoryview_obj {
@@ -1408,15 +1440,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1425,44 +1457,44 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "SuperPang/lib/Compressor.pyx":12
+/* "superpang/lib/Compressor.pyx":12
  * ctypedef np.uint8_t DTYPE_t
  * 
  * cdef class Compressor:             # <<<<<<<<<<<<<<
  *     """
  *     Hash a nucleotide sequence into a compressed form
  */
 
-struct __pyx_vtabstruct_9SuperPang_3lib_10Compressor_Compressor {
-  int (*change_base)(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *, int, int, int);
+struct __pyx_vtabstruct_9superpang_3lib_10Compressor_Compressor {
+  int (*change_base)(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *, int, int, int);
 };
-static struct __pyx_vtabstruct_9SuperPang_3lib_10Compressor_Compressor *__pyx_vtabptr_9SuperPang_3lib_10Compressor_Compressor;
-static CYTHON_INLINE int __pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *, int, int, int);
+static struct __pyx_vtabstruct_9superpang_3lib_10Compressor_Compressor *__pyx_vtabptr_9superpang_3lib_10Compressor_Compressor;
+static CYTHON_INLINE int __pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *, int, int, int);
 
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 
 struct __pyx_vtabstruct_array {
   PyObject *(*get_memview)(struct __pyx_array_obj *);
 };
 static struct __pyx_vtabstruct_array *__pyx_vtabptr_array;
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 
@@ -1474,15 +1506,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -1747,26 +1779,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1787,14 +1819,19 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1977,14 +2014,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
@@ -2004,22 +2058,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -2349,15 +2411,15 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static CYTHON_INLINE int __pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base(CYTHON_UNUSED struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, int __pyx_v_num, int __pyx_v_base0, int __pyx_v_base1); /* proto*/
+static CYTHON_INLINE int __pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base(CYTHON_UNUSED struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, int __pyx_v_num, int __pyx_v_base0, int __pyx_v_base1); /* proto*/
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
 static PyObject *__pyx_memoryview_is_slice(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assignment(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_dst, PyObject *__pyx_v_src); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assign_scalar(struct __pyx_memoryview_obj *__pyx_v_self, struct __pyx_memoryview_obj *__pyx_v_dst, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_setitem_indexed(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_convert_item_to_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
@@ -2407,28 +2469,28 @@
 static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
 static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
-/* Module declarations from 'SuperPang.lib.Compressor' */
-static PyTypeObject *__pyx_ptype_9SuperPang_3lib_10Compressor_Compressor = 0;
+/* Module declarations from 'superpang.lib.Compressor' */
+static PyTypeObject *__pyx_ptype_9superpang_3lib_10Compressor_Compressor = 0;
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static PyObject *__pyx_f_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *, PyObject *); /*proto*/
+static PyObject *__pyx_f_9superpang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *, PyObject *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -2455,19 +2517,19 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_unsigned_char__const__ = { "const unsigned char", NULL, sizeof(unsigned char const ), { 0 }, 0, IS_UNSIGNED(unsigned char const ) ? 'U' : 'I', IS_UNSIGNED(unsigned char const ), 0 };
-#define __Pyx_MODULE_NAME "SuperPang.lib.Compressor"
-extern int __pyx_module_is_main_SuperPang__lib__Compressor;
-int __pyx_module_is_main_SuperPang__lib__Compressor = 0;
+#define __Pyx_MODULE_NAME "superpang.lib.Compressor"
+extern int __pyx_module_is_main_superpang__lib__Compressor;
+int __pyx_module_is_main_superpang__lib__Compressor = 0;
 
-/* Implementation of 'SuperPang.lib.Compressor' */
+/* Implementation of 'superpang.lib.Compressor' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_chr;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_TypeError;
@@ -2553,15 +2615,15 @@
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_pyx_unpickle_Compressor[] = "__pyx_unpickle_Compressor";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
-static const char __pyx_k_SuperPang_lib_Compressor[] = "SuperPang.lib.Compressor";
+static const char __pyx_k_superpang_lib_Compressor[] = "superpang.lib.Compressor";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
@@ -2601,15 +2663,14 @@
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_n_s_SuperPang_lib_Compressor;
 static PyObject *__pyx_n_u_T;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
@@ -2672,28 +2733,29 @@
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
+static PyObject *__pyx_n_s_superpang_lib_Compressor;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_tounicode;
 static PyObject *__pyx_n_u_u;
 static PyObject *__pyx_n_s_uint8;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
-static int __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor___init__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v_ksize); /* proto */
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_2compress(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_seq); /* proto */
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_4decompress(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_cseq); /* proto */
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_6__reduce_cython__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_8__setstate_cython__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_9superpang_3lib_10Compressor_10Compressor___init__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v_ksize); /* proto */
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_2compress(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_seq); /* proto */
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_4decompress(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_cseq); /* proto */
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_6__reduce_cython__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_8__setstate_cython__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor___pyx_unpickle_Compressor(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -2730,15 +2792,15 @@
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_9SuperPang_3lib_10Compressor_Compressor(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9superpang_3lib_10Compressor_Compressor(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_98135457;
@@ -2777,25 +2839,25 @@
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_codeobj__24;
 static PyObject *__pyx_codeobj__31;
 /* Late includes */
 
-/* "SuperPang/lib/Compressor.pyx":25
+/* "superpang/lib/Compressor.pyx":25
  *     cdef Py_ssize_t clength
  * 
  *     def __init__(self, ksize):             # <<<<<<<<<<<<<<
  *         self.ksize = ksize
  *         self.com = self.ksize // 4
  */
 
 /* Python wrapper */
-static int __pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_9superpang_3lib_10Compressor_10Compressor_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_9superpang_3lib_10Compressor_10Compressor_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_ksize = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
@@ -2827,129 +2889,129 @@
     }
     __pyx_v_ksize = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor___init__(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_ksize);
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor_10Compressor___init__(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_ksize);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor___init__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v_ksize) {
+static int __pyx_pf_9superpang_3lib_10Compressor_10Compressor___init__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v_ksize) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "SuperPang/lib/Compressor.pyx":26
+  /* "superpang/lib/Compressor.pyx":26
  * 
  *     def __init__(self, ksize):
  *         self.ksize = ksize             # <<<<<<<<<<<<<<
  *         self.com = self.ksize // 4
  *         self.rem = self.ksize % 4
  */
   __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_ksize); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_v_self->ksize = __pyx_t_1;
 
-  /* "SuperPang/lib/Compressor.pyx":27
+  /* "superpang/lib/Compressor.pyx":27
  *     def __init__(self, ksize):
  *         self.ksize = ksize
  *         self.com = self.ksize // 4             # <<<<<<<<<<<<<<
  *         self.rem = self.ksize % 4
  *         self.clength = self.com + self.rem
  */
   __pyx_v_self->com = (__pyx_v_self->ksize / 4);
 
-  /* "SuperPang/lib/Compressor.pyx":28
+  /* "superpang/lib/Compressor.pyx":28
  *         self.ksize = ksize
  *         self.com = self.ksize // 4
  *         self.rem = self.ksize % 4             # <<<<<<<<<<<<<<
  *         self.clength = self.com + self.rem
  * 
  */
   __pyx_v_self->rem = (__pyx_v_self->ksize % 4);
 
-  /* "SuperPang/lib/Compressor.pyx":29
+  /* "superpang/lib/Compressor.pyx":29
  *         self.com = self.ksize // 4
  *         self.rem = self.ksize % 4
  *         self.clength = self.com + self.rem             # <<<<<<<<<<<<<<
  * 
  *     def compress(self, const unsigned char [:] seq):
  */
   __pyx_v_self->clength = (__pyx_v_self->com + __pyx_v_self->rem);
 
-  /* "SuperPang/lib/Compressor.pyx":25
+  /* "superpang/lib/Compressor.pyx":25
  *     cdef Py_ssize_t clength
  * 
  *     def __init__(self, ksize):             # <<<<<<<<<<<<<<
  *         self.ksize = ksize
  *         self.com = self.ksize // 4
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SuperPang/lib/Compressor.pyx":31
+/* "superpang/lib/Compressor.pyx":31
  *         self.clength = self.com + self.rem
  * 
  *     def compress(self, const unsigned char [:] seq):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef const unsigned char [:] tetra
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_3compress(PyObject *__pyx_v_self, PyObject *__pyx_arg_seq); /*proto*/
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_3compress(PyObject *__pyx_v_self, PyObject *__pyx_arg_seq) {
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_3compress(PyObject *__pyx_v_self, PyObject *__pyx_arg_seq); /*proto*/
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_3compress(PyObject *__pyx_v_self, PyObject *__pyx_arg_seq) {
   __Pyx_memviewslice __pyx_v_seq = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compress (wrapper)", 0);
   assert(__pyx_arg_seq); {
     __pyx_v_seq = __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_char__const__(__pyx_arg_seq, 0); if (unlikely(!__pyx_v_seq.memview)) __PYX_ERR(0, 31, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_2compress(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_seq);
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor_10Compressor_2compress(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_seq);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_2compress(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_seq) {
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_2compress(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_seq) {
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   __Pyx_memviewslice __pyx_v_tetra = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __pyx_t_9SuperPang_3lib_10Compressor_DTYPE_t __pyx_v_cseq[0x3E8];
+  __pyx_t_9superpang_3lib_10Compressor_DTYPE_t __pyx_v_cseq[0x3E8];
   int __pyx_v_ctetra;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   __Pyx_memviewslice __pyx_t_4 = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -2959,27 +3021,27 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compress", 0);
 
-  /* "SuperPang/lib/Compressor.pyx":36
+  /* "superpang/lib/Compressor.pyx":36
  *         cdef DTYPE_t [1000] cseq
  *         cdef int ctetra
  *         for i in range(self.com):             # <<<<<<<<<<<<<<
  *             # Each tetranucleotide is stored as an 8-bit binary
  *             # A: 00, C: 01, G: 10, T: 11
  */
   __pyx_t_1 = __pyx_v_self->com;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "SuperPang/lib/Compressor.pyx":39
+    /* "superpang/lib/Compressor.pyx":39
  *             # Each tetranucleotide is stored as an 8-bit binary
  *             # A: 00, C: 01, G: 10, T: 11
  *             tetra = seq[i*4:(i*4)+4]             # <<<<<<<<<<<<<<
  *             ctetra = 0
  *             for j in range(3,-1,-1):
  */
     __pyx_t_4.data = __pyx_v_seq.data;
@@ -3004,250 +3066,250 @@
 }
 
 __PYX_XDEC_MEMVIEW(&__pyx_v_tetra, 1);
     __pyx_v_tetra = __pyx_t_4;
     __pyx_t_4.memview = NULL;
     __pyx_t_4.data = NULL;
 
-    /* "SuperPang/lib/Compressor.pyx":40
+    /* "superpang/lib/Compressor.pyx":40
  *             # A: 00, C: 01, G: 10, T: 11
  *             tetra = seq[i*4:(i*4)+4]
  *             ctetra = 0             # <<<<<<<<<<<<<<
  *             for j in range(3,-1,-1):
  *                 if tetra[3-j] == b'A':
  */
     __pyx_v_ctetra = 0;
 
-    /* "SuperPang/lib/Compressor.pyx":41
+    /* "superpang/lib/Compressor.pyx":41
  *             tetra = seq[i*4:(i*4)+4]
  *             ctetra = 0
  *             for j in range(3,-1,-1):             # <<<<<<<<<<<<<<
  *                 if tetra[3-j] == b'A':
  *                     pass
  */
     for (__pyx_t_6 = 3; __pyx_t_6 > -1L; __pyx_t_6-=1) {
       __pyx_v_j = __pyx_t_6;
 
-      /* "SuperPang/lib/Compressor.pyx":42
+      /* "superpang/lib/Compressor.pyx":42
  *             ctetra = 0
  *             for j in range(3,-1,-1):
  *                 if tetra[3-j] == b'A':             # <<<<<<<<<<<<<<
  *                     pass
  *                 elif tetra[3-j] == b'C':
  */
       __pyx_t_7 = (3 - __pyx_v_j);
       __pyx_t_8 = (((*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_tetra.data + __pyx_t_7 * __pyx_v_tetra.strides[0]) ))) == 'A') != 0);
       if (__pyx_t_8) {
         goto __pyx_L7;
       }
 
-      /* "SuperPang/lib/Compressor.pyx":44
+      /* "superpang/lib/Compressor.pyx":44
  *                 if tetra[3-j] == b'A':
  *                     pass
  *                 elif tetra[3-j] == b'C':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**(2*j)
  *                 elif tetra[3-j] == b'G':
  */
       __pyx_t_7 = (3 - __pyx_v_j);
       __pyx_t_8 = (((*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_tetra.data + __pyx_t_7 * __pyx_v_tetra.strides[0]) ))) == 'C') != 0);
       if (__pyx_t_8) {
 
-        /* "SuperPang/lib/Compressor.pyx":45
+        /* "superpang/lib/Compressor.pyx":45
  *                     pass
  *                 elif tetra[3-j] == b'C':
  *                     ctetra += 10**(2*j)             # <<<<<<<<<<<<<<
  *                 elif tetra[3-j] == b'G':
  *                     ctetra += 10**((2*j)+1)
  */
         __pyx_v_ctetra = (__pyx_v_ctetra + __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j)));
 
-        /* "SuperPang/lib/Compressor.pyx":44
+        /* "superpang/lib/Compressor.pyx":44
  *                 if tetra[3-j] == b'A':
  *                     pass
  *                 elif tetra[3-j] == b'C':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**(2*j)
  *                 elif tetra[3-j] == b'G':
  */
         goto __pyx_L7;
       }
 
-      /* "SuperPang/lib/Compressor.pyx":46
+      /* "superpang/lib/Compressor.pyx":46
  *                 elif tetra[3-j] == b'C':
  *                     ctetra += 10**(2*j)
  *                 elif tetra[3-j] == b'G':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**((2*j)+1)
  *                 elif tetra[3-j] == b'T':
  */
       __pyx_t_7 = (3 - __pyx_v_j);
       __pyx_t_8 = (((*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_tetra.data + __pyx_t_7 * __pyx_v_tetra.strides[0]) ))) == 'G') != 0);
       if (__pyx_t_8) {
 
-        /* "SuperPang/lib/Compressor.pyx":47
+        /* "superpang/lib/Compressor.pyx":47
  *                     ctetra += 10**(2*j)
  *                 elif tetra[3-j] == b'G':
  *                     ctetra += 10**((2*j)+1)             # <<<<<<<<<<<<<<
  *                 elif tetra[3-j] == b'T':
  *                     ctetra += 10**((2*j)+1)
  */
         __pyx_v_ctetra = (__pyx_v_ctetra + __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1)));
 
-        /* "SuperPang/lib/Compressor.pyx":46
+        /* "superpang/lib/Compressor.pyx":46
  *                 elif tetra[3-j] == b'C':
  *                     ctetra += 10**(2*j)
  *                 elif tetra[3-j] == b'G':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**((2*j)+1)
  *                 elif tetra[3-j] == b'T':
  */
         goto __pyx_L7;
       }
 
-      /* "SuperPang/lib/Compressor.pyx":48
+      /* "superpang/lib/Compressor.pyx":48
  *                 elif tetra[3-j] == b'G':
  *                     ctetra += 10**((2*j)+1)
  *                 elif tetra[3-j] == b'T':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**((2*j)+1)
  *                     ctetra += 10**(2*j)
  */
       __pyx_t_7 = (3 - __pyx_v_j);
       __pyx_t_8 = (((*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_tetra.data + __pyx_t_7 * __pyx_v_tetra.strides[0]) ))) == 'T') != 0);
       if (__pyx_t_8) {
 
-        /* "SuperPang/lib/Compressor.pyx":49
+        /* "superpang/lib/Compressor.pyx":49
  *                     ctetra += 10**((2*j)+1)
  *                 elif tetra[3-j] == b'T':
  *                     ctetra += 10**((2*j)+1)             # <<<<<<<<<<<<<<
  *                     ctetra += 10**(2*j)
  *             # Transform the 8-bit into a 1-byte decimal
  */
         __pyx_v_ctetra = (__pyx_v_ctetra + __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1)));
 
-        /* "SuperPang/lib/Compressor.pyx":50
+        /* "superpang/lib/Compressor.pyx":50
  *                 elif tetra[3-j] == b'T':
  *                     ctetra += 10**((2*j)+1)
  *                     ctetra += 10**(2*j)             # <<<<<<<<<<<<<<
  *             # Transform the 8-bit into a 1-byte decimal
  *             cseq[i] = self.change_base(ctetra, 2, 10)
  */
         __pyx_v_ctetra = (__pyx_v_ctetra + __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j)));
 
-        /* "SuperPang/lib/Compressor.pyx":48
+        /* "superpang/lib/Compressor.pyx":48
  *                 elif tetra[3-j] == b'G':
  *                     ctetra += 10**((2*j)+1)
  *                 elif tetra[3-j] == b'T':             # <<<<<<<<<<<<<<
  *                     ctetra += 10**((2*j)+1)
  *                     ctetra += 10**(2*j)
  */
       }
       __pyx_L7:;
     }
 
-    /* "SuperPang/lib/Compressor.pyx":52
+    /* "superpang/lib/Compressor.pyx":52
  *                     ctetra += 10**(2*j)
  *             # Transform the 8-bit into a 1-byte decimal
  *             cseq[i] = self.change_base(ctetra, 2, 10)             # <<<<<<<<<<<<<<
  *         # For the remainder, just store each base as a byte
  *         for i in range(self.rem):
  */
-    (__pyx_v_cseq[__pyx_v_i]) = __pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base(__pyx_v_self, __pyx_v_ctetra, 2, 10);
+    (__pyx_v_cseq[__pyx_v_i]) = __pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base(__pyx_v_self, __pyx_v_ctetra, 2, 10);
   }
 
-  /* "SuperPang/lib/Compressor.pyx":54
+  /* "superpang/lib/Compressor.pyx":54
  *             cseq[i] = self.change_base(ctetra, 2, 10)
  *         # For the remainder, just store each base as a byte
  *         for i in range(self.rem):             # <<<<<<<<<<<<<<
  *             cseq[self.com+i] = seq[4*self.com+i] # this directly casts the char into into DTYPE_t
  * 
  */
   __pyx_t_1 = __pyx_v_self->rem;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "SuperPang/lib/Compressor.pyx":55
+    /* "superpang/lib/Compressor.pyx":55
  *         # For the remainder, just store each base as a byte
  *         for i in range(self.rem):
  *             cseq[self.com+i] = seq[4*self.com+i] # this directly casts the char into into DTYPE_t             # <<<<<<<<<<<<<<
  * 
  *         return cseq[0:self.clength]
  */
     __pyx_t_7 = ((4 * __pyx_v_self->com) + __pyx_v_i);
     (__pyx_v_cseq[(__pyx_v_self->com + __pyx_v_i)]) = (*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_seq.data + __pyx_t_7 * __pyx_v_seq.strides[0]) )));
   }
 
-  /* "SuperPang/lib/Compressor.pyx":57
+  /* "superpang/lib/Compressor.pyx":57
  *             cseq[self.com+i] = seq[4*self.com+i] # this directly casts the char into into DTYPE_t
  * 
  *         return cseq[0:self.clength]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_9 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_cseq) + 0, __pyx_v_self->clength - 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_r = __pyx_t_9;
   __pyx_t_9 = 0;
   goto __pyx_L0;
 
-  /* "SuperPang/lib/Compressor.pyx":31
+  /* "superpang/lib/Compressor.pyx":31
  *         self.clength = self.com + self.rem
  * 
  *     def compress(self, const unsigned char [:] seq):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef const unsigned char [:] tetra
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_seq, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_tetra, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SuperPang/lib/Compressor.pyx":60
+/* "superpang/lib/Compressor.pyx":60
  * 
  * 
  *     def decompress(self, const unsigned char[:] cseq):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef int dec
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_5decompress(PyObject *__pyx_v_self, PyObject *__pyx_arg_cseq); /*proto*/
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_5decompress(PyObject *__pyx_v_self, PyObject *__pyx_arg_cseq) {
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_5decompress(PyObject *__pyx_v_self, PyObject *__pyx_arg_cseq); /*proto*/
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_5decompress(PyObject *__pyx_v_self, PyObject *__pyx_arg_cseq) {
   __Pyx_memviewslice __pyx_v_cseq = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("decompress (wrapper)", 0);
   assert(__pyx_arg_cseq); {
     __pyx_v_cseq = __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_char__const__(__pyx_arg_cseq, 0); if (unlikely(!__pyx_v_cseq.memview)) __PYX_ERR(0, 60, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_4decompress(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_cseq);
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor_10Compressor_4decompress(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v_self), __pyx_v_cseq);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_4decompress(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_cseq) {
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_4decompress(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, __Pyx_memviewslice __pyx_v_cseq) {
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   int __pyx_v_dec;
   int __pyx_v_ctetra;
   arrayobject *__pyx_v_seq = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3262,15 +3324,15 @@
   Py_ssize_t __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decompress", 0);
 
-  /* "SuperPang/lib/Compressor.pyx":64
+  /* "superpang/lib/Compressor.pyx":64
  *         cdef int dec
  *         cdef int ctetra
  *         seq = array('u', '0'*self.ksize)             # <<<<<<<<<<<<<<
  *         for i in range(self.com):
  *             dec = cseq[i]
  */
   __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->ksize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
@@ -3288,186 +3350,186 @@
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_seq = ((arrayobject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "SuperPang/lib/Compressor.pyx":65
+  /* "superpang/lib/Compressor.pyx":65
  *         cdef int ctetra
  *         seq = array('u', '0'*self.ksize)
  *         for i in range(self.com):             # <<<<<<<<<<<<<<
  *             dec = cseq[i]
  *             # Get the 8-bit binary from the decimal byte
  */
   __pyx_t_3 = __pyx_v_self->com;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "SuperPang/lib/Compressor.pyx":66
+    /* "superpang/lib/Compressor.pyx":66
  *         seq = array('u', '0'*self.ksize)
  *         for i in range(self.com):
  *             dec = cseq[i]             # <<<<<<<<<<<<<<
  *             # Get the 8-bit binary from the decimal byte
  *             ctetra = self.change_base(dec, 10, 2)
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_v_dec = (*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_cseq.data + __pyx_t_6 * __pyx_v_cseq.strides[0]) )));
 
-    /* "SuperPang/lib/Compressor.pyx":68
+    /* "superpang/lib/Compressor.pyx":68
  *             dec = cseq[i]
  *             # Get the 8-bit binary from the decimal byte
  *             ctetra = self.change_base(dec, 10, 2)             # <<<<<<<<<<<<<<
  *             # Reconstruc the tetranucleotide
  *             for j in range(3,-1,-1):
  */
-    __pyx_v_ctetra = __pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base(__pyx_v_self, __pyx_v_dec, 10, 2);
+    __pyx_v_ctetra = __pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base(__pyx_v_self, __pyx_v_dec, 10, 2);
 
-    /* "SuperPang/lib/Compressor.pyx":70
+    /* "superpang/lib/Compressor.pyx":70
  *             ctetra = self.change_base(dec, 10, 2)
  *             # Reconstruc the tetranucleotide
  *             for j in range(3,-1,-1):             # <<<<<<<<<<<<<<
  *                 if ctetra // 10**((2*j)+1):
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
  */
     for (__pyx_t_7 = 3; __pyx_t_7 > -1L; __pyx_t_7-=1) {
       __pyx_v_j = __pyx_t_7;
 
-      /* "SuperPang/lib/Compressor.pyx":71
+      /* "superpang/lib/Compressor.pyx":71
  *             # Reconstruc the tetranucleotide
  *             for j in range(3,-1,-1):
  *                 if ctetra // 10**((2*j)+1):             # <<<<<<<<<<<<<<
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'T'
  */
       __pyx_t_8 = ((__pyx_v_ctetra / __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1))) != 0);
       if (__pyx_t_8) {
 
-        /* "SuperPang/lib/Compressor.pyx":72
+        /* "superpang/lib/Compressor.pyx":72
  *             for j in range(3,-1,-1):
  *                 if ctetra // 10**((2*j)+1):
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):             # <<<<<<<<<<<<<<
  *                         seq[(i*4)+(3-j)] = 'T'
  *                         ctetra -= 10**((2*j)+1)
  */
         __pyx_t_8 = (((__pyx_v_ctetra - __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1))) / __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j))) != 0);
         if (__pyx_t_8) {
 
-          /* "SuperPang/lib/Compressor.pyx":73
+          /* "superpang/lib/Compressor.pyx":73
  *                 if ctetra // 10**((2*j)+1):
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'T'             # <<<<<<<<<<<<<<
  *                         ctetra -= 10**((2*j)+1)
  *                         ctetra -= 10**(2*j)
  */
           __pyx_t_9 = ((__pyx_v_i * 4) + (3 - __pyx_v_j));
           if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_seq), __pyx_t_9, __pyx_n_u_T, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 73, __pyx_L1_error)
 
-          /* "SuperPang/lib/Compressor.pyx":74
+          /* "superpang/lib/Compressor.pyx":74
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'T'
  *                         ctetra -= 10**((2*j)+1)             # <<<<<<<<<<<<<<
  *                         ctetra -= 10**(2*j)
  *                     else:
  */
           __pyx_v_ctetra = (__pyx_v_ctetra - __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1)));
 
-          /* "SuperPang/lib/Compressor.pyx":75
+          /* "superpang/lib/Compressor.pyx":75
  *                         seq[(i*4)+(3-j)] = 'T'
  *                         ctetra -= 10**((2*j)+1)
  *                         ctetra -= 10**(2*j)             # <<<<<<<<<<<<<<
  *                     else:
  *                         seq[(i*4)+(3-j)] = 'G'
  */
           __pyx_v_ctetra = (__pyx_v_ctetra - __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j)));
 
-          /* "SuperPang/lib/Compressor.pyx":72
+          /* "superpang/lib/Compressor.pyx":72
  *             for j in range(3,-1,-1):
  *                 if ctetra // 10**((2*j)+1):
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):             # <<<<<<<<<<<<<<
  *                         seq[(i*4)+(3-j)] = 'T'
  *                         ctetra -= 10**((2*j)+1)
  */
           goto __pyx_L8;
         }
 
-        /* "SuperPang/lib/Compressor.pyx":77
+        /* "superpang/lib/Compressor.pyx":77
  *                         ctetra -= 10**(2*j)
  *                     else:
  *                         seq[(i*4)+(3-j)] = 'G'             # <<<<<<<<<<<<<<
  *                         ctetra -= 10**((2*j)+1)
  *                 else:
  */
         /*else*/ {
           __pyx_t_9 = ((__pyx_v_i * 4) + (3 - __pyx_v_j));
           if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_seq), __pyx_t_9, __pyx_n_u_G, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
 
-          /* "SuperPang/lib/Compressor.pyx":78
+          /* "superpang/lib/Compressor.pyx":78
  *                     else:
  *                         seq[(i*4)+(3-j)] = 'G'
  *                         ctetra -= 10**((2*j)+1)             # <<<<<<<<<<<<<<
  *                 else:
  *                     if ctetra // 10**((2*j)):
  */
           __pyx_v_ctetra = (__pyx_v_ctetra - __Pyx_pow_Py_ssize_t(10, ((2 * __pyx_v_j) + 1)));
         }
         __pyx_L8:;
 
-        /* "SuperPang/lib/Compressor.pyx":71
+        /* "superpang/lib/Compressor.pyx":71
  *             # Reconstruc the tetranucleotide
  *             for j in range(3,-1,-1):
  *                 if ctetra // 10**((2*j)+1):             # <<<<<<<<<<<<<<
  *                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'T'
  */
         goto __pyx_L7;
       }
 
-      /* "SuperPang/lib/Compressor.pyx":80
+      /* "superpang/lib/Compressor.pyx":80
  *                         ctetra -= 10**((2*j)+1)
  *                 else:
  *                     if ctetra // 10**((2*j)):             # <<<<<<<<<<<<<<
  *                         seq[(i*4)+(3-j)] = 'C'
  *                         ctetra -= 10**(2*j)
  */
       /*else*/ {
         __pyx_t_8 = ((__pyx_v_ctetra / __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j))) != 0);
         if (__pyx_t_8) {
 
-          /* "SuperPang/lib/Compressor.pyx":81
+          /* "superpang/lib/Compressor.pyx":81
  *                 else:
  *                     if ctetra // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'C'             # <<<<<<<<<<<<<<
  *                         ctetra -= 10**(2*j)
  *                     else:
  */
           __pyx_t_9 = ((__pyx_v_i * 4) + (3 - __pyx_v_j));
           if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_seq), __pyx_t_9, __pyx_n_u_C, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 81, __pyx_L1_error)
 
-          /* "SuperPang/lib/Compressor.pyx":82
+          /* "superpang/lib/Compressor.pyx":82
  *                     if ctetra // 10**((2*j)):
  *                         seq[(i*4)+(3-j)] = 'C'
  *                         ctetra -= 10**(2*j)             # <<<<<<<<<<<<<<
  *                     else:
  *                         seq[(i*4)+(3-j)] = 'A'
  */
           __pyx_v_ctetra = (__pyx_v_ctetra - __Pyx_pow_Py_ssize_t(10, (2 * __pyx_v_j)));
 
-          /* "SuperPang/lib/Compressor.pyx":80
+          /* "superpang/lib/Compressor.pyx":80
  *                         ctetra -= 10**((2*j)+1)
  *                 else:
  *                     if ctetra // 10**((2*j)):             # <<<<<<<<<<<<<<
  *                         seq[(i*4)+(3-j)] = 'C'
  *                         ctetra -= 10**(2*j)
  */
           goto __pyx_L9;
         }
 
-        /* "SuperPang/lib/Compressor.pyx":84
+        /* "superpang/lib/Compressor.pyx":84
  *                         ctetra -= 10**(2*j)
  *                     else:
  *                         seq[(i*4)+(3-j)] = 'A'             # <<<<<<<<<<<<<<
  * 
  *         # For the remainder, just transform the byte into a character
  */
         /*else*/ {
@@ -3476,37 +3538,37 @@
         }
         __pyx_L9:;
       }
       __pyx_L7:;
     }
   }
 
-  /* "SuperPang/lib/Compressor.pyx":87
+  /* "superpang/lib/Compressor.pyx":87
  * 
  *         # For the remainder, just transform the byte into a character
  *         for i in range(self.rem):             # <<<<<<<<<<<<<<
  *             dec = cseq[self.com+i]
  *             seq[4*self.com+i] = chr(dec)
  */
   __pyx_t_3 = __pyx_v_self->rem;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "SuperPang/lib/Compressor.pyx":88
+    /* "superpang/lib/Compressor.pyx":88
  *         # For the remainder, just transform the byte into a character
  *         for i in range(self.rem):
  *             dec = cseq[self.com+i]             # <<<<<<<<<<<<<<
  *             seq[4*self.com+i] = chr(dec)
  * 
  */
     __pyx_t_6 = (__pyx_v_self->com + __pyx_v_i);
     __pyx_v_dec = (*((unsigned char const  *) ( /* dim=0 */ (__pyx_v_cseq.data + __pyx_t_6 * __pyx_v_cseq.strides[0]) )));
 
-    /* "SuperPang/lib/Compressor.pyx":89
+    /* "superpang/lib/Compressor.pyx":89
  *         for i in range(self.rem):
  *             dec = cseq[self.com+i]
  *             seq[4*self.com+i] = chr(dec)             # <<<<<<<<<<<<<<
  * 
  *         return seq.tounicode()
  */
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_dec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
@@ -3515,15 +3577,15 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = ((4 * __pyx_v_self->com) + __pyx_v_i);
     if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_seq), __pyx_t_7, __pyx_t_1, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "SuperPang/lib/Compressor.pyx":91
+  /* "superpang/lib/Compressor.pyx":91
  *             seq[4*self.com+i] = chr(dec)
  * 
  *         return seq.tounicode()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3544,119 +3606,119 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "SuperPang/lib/Compressor.pyx":60
+  /* "superpang/lib/Compressor.pyx":60
  * 
  * 
  *     def decompress(self, const unsigned char[:] cseq):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef int dec
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_cseq, 1);
   __Pyx_XDECREF((PyObject *)__pyx_v_seq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SuperPang/lib/Compressor.pyx":94
+/* "superpang/lib/Compressor.pyx":94
  * 
  * 
  *     cdef inline int change_base(self, int num, int base0, int base1):             # <<<<<<<<<<<<<<
  *         # This expects 8-bit binary numbers and decimals no larger than 255!
  *         cdef Py_ssize_t i
  */
 
-static CYTHON_INLINE int __pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base(CYTHON_UNUSED struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, int __pyx_v_num, int __pyx_v_base0, int __pyx_v_base1) {
+static CYTHON_INLINE int __pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base(CYTHON_UNUSED struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, int __pyx_v_num, int __pyx_v_base0, int __pyx_v_base1) {
   Py_ssize_t __pyx_v_i;
   int __pyx_v_res;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("change_base", 0);
 
-  /* "SuperPang/lib/Compressor.pyx":97
+  /* "superpang/lib/Compressor.pyx":97
  *         # This expects 8-bit binary numbers and decimals no larger than 255!
  *         cdef Py_ssize_t i
  *         cdef int res = 0             # <<<<<<<<<<<<<<
  *         for i in range(7,-1,-1):
  *             if num // base1**i:
  */
   __pyx_v_res = 0;
 
-  /* "SuperPang/lib/Compressor.pyx":98
+  /* "superpang/lib/Compressor.pyx":98
  *         cdef Py_ssize_t i
  *         cdef int res = 0
  *         for i in range(7,-1,-1):             # <<<<<<<<<<<<<<
  *             if num // base1**i:
  *                 num -= base1**i
  */
   for (__pyx_t_1 = 7; __pyx_t_1 > -1L; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "SuperPang/lib/Compressor.pyx":99
+    /* "superpang/lib/Compressor.pyx":99
  *         cdef int res = 0
  *         for i in range(7,-1,-1):
  *             if num // base1**i:             # <<<<<<<<<<<<<<
  *                 num -= base1**i
  *                 res += base0**i
  */
     __pyx_t_2 = ((__pyx_v_num / __Pyx_pow_Py_ssize_t(((Py_ssize_t)__pyx_v_base1), __pyx_v_i)) != 0);
     if (__pyx_t_2) {
 
-      /* "SuperPang/lib/Compressor.pyx":100
+      /* "superpang/lib/Compressor.pyx":100
  *         for i in range(7,-1,-1):
  *             if num // base1**i:
  *                 num -= base1**i             # <<<<<<<<<<<<<<
  *                 res += base0**i
  *         return res
  */
       __pyx_v_num = (__pyx_v_num - __Pyx_pow_Py_ssize_t(((Py_ssize_t)__pyx_v_base1), __pyx_v_i));
 
-      /* "SuperPang/lib/Compressor.pyx":101
+      /* "superpang/lib/Compressor.pyx":101
  *             if num // base1**i:
  *                 num -= base1**i
  *                 res += base0**i             # <<<<<<<<<<<<<<
  *         return res
  */
       __pyx_v_res = (__pyx_v_res + __Pyx_pow_Py_ssize_t(((Py_ssize_t)__pyx_v_base0), __pyx_v_i));
 
-      /* "SuperPang/lib/Compressor.pyx":99
+      /* "superpang/lib/Compressor.pyx":99
  *         cdef int res = 0
  *         for i in range(7,-1,-1):
  *             if num // base1**i:             # <<<<<<<<<<<<<<
  *                 num -= base1**i
  *                 res += base0**i
  */
     }
   }
 
-  /* "SuperPang/lib/Compressor.pyx":102
+  /* "superpang/lib/Compressor.pyx":102
  *                 num -= base1**i
  *                 res += base0**i
  *         return res             # <<<<<<<<<<<<<<
  */
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
 
-  /* "SuperPang/lib/Compressor.pyx":94
+  /* "superpang/lib/Compressor.pyx":94
  * 
  * 
  *     cdef inline int change_base(self, int num, int base0, int base1):             # <<<<<<<<<<<<<<
  *         # This expects 8-bit binary numbers and decimals no larger than 255!
  *         cdef Py_ssize_t i
  */
 
@@ -3669,27 +3731,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_7__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_6__reduce_cython__(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor_10Compressor_6__reduce_cython__(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_6__reduce_cython__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self) {
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_6__reduce_cython__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -3906,15 +3968,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -3924,42 +3986,42 @@
  *     else:
  *         return __pyx_unpickle_Compressor, (type(self), 0x708d54a, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Compressor__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_10Compressor_9__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_8__setstate_cython__(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor_10Compressor_8__setstate_cython__(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor_10Compressor_8__setstate_cython__(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor_10Compressor_8__setstate_cython__(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Compressor, (type(self), 0x708d54a, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Compressor__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9superpang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Compressor, (type(self), 0x708d54a, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -3967,32 +4029,32 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.Compressor.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.Compressor.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_Compressor(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_1__pyx_unpickle_Compressor(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9SuperPang_3lib_10Compressor_1__pyx_unpickle_Compressor = {"__pyx_unpickle_Compressor", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9SuperPang_3lib_10Compressor_1__pyx_unpickle_Compressor, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9SuperPang_3lib_10Compressor_1__pyx_unpickle_Compressor(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_1__pyx_unpickle_Compressor(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9superpang_3lib_10Compressor_1__pyx_unpickle_Compressor = {"__pyx_unpickle_Compressor", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9superpang_3lib_10Compressor_1__pyx_unpickle_Compressor, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9superpang_3lib_10Compressor_1__pyx_unpickle_Compressor(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4046,26 +4108,26 @@
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Compressor", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.__pyx_unpickle_Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.__pyx_unpickle_Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_9superpang_3lib_10Compressor___pyx_unpickle_Compressor(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9superpang_3lib_10Compressor___pyx_unpickle_Compressor(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -4158,15 +4220,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x708d54a, 0xcae9114, 0x5d96da1) = (clength, com, ksize, rem))" % __pyx_checksum)
  *     __pyx_result = Compressor.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Compressor__set_state(<Compressor> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9SuperPang_3lib_10Compressor_Compressor), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9superpang_3lib_10Compressor_Compressor), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
@@ -4196,16 +4258,16 @@
     /* "(tree fragment)":9
  *     __pyx_result = Compressor.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Compressor__set_state(<Compressor> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Compressor__set_state(Compressor __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_f_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_9superpang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x708d54a, 0xcae9114, 0x5d96da1) = (clength, com, ksize, rem))" % __pyx_checksum)
  *     __pyx_result = Compressor.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -4234,15 +4296,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.__pyx_unpickle_Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.__pyx_unpickle_Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -4252,15 +4314,15 @@
  *         __pyx_unpickle_Compressor__set_state(<Compressor> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Compressor__set_state(Compressor __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.clength = __pyx_state[0]; __pyx_result.com = __pyx_state[1]; __pyx_result.ksize = __pyx_state[2]; __pyx_result.rem = __pyx_state[3]
  *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_9SuperPang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_9superpang_3lib_10Compressor___pyx_unpickle_Compressor__set_state(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
@@ -4376,15 +4438,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("SuperPang.lib.Compressor.__pyx_unpickle_Compressor__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("superpang.lib.Compressor.__pyx_unpickle_Compressor__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5036,15 +5098,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5053,29 +5115,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5086,15 +5148,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5103,29 +5165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5136,15 +5198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5153,29 +5215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5186,15 +5248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5203,29 +5265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5236,15 +5298,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5253,29 +5315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5286,212 +5348,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(3, 927, __pyx_L1_error)
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5507,15 +5577,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5523,84 +5593,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 939, __pyx_L3_error)
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 945, __pyx_L5_except_error)
+      __PYX_ERR(3, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5615,15 +5685,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5639,15 +5709,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5655,84 +5725,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 945, __pyx_L3_error)
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 951, __pyx_L5_except_error)
+      __PYX_ERR(3, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5747,15 +5817,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5771,15 +5841,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5787,84 +5857,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 951, __pyx_L3_error)
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(3, 957, __pyx_L5_except_error)
+      __PYX_ERR(3, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5879,189 +5949,189 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":122
+/* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -6105,21 +6175,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_itemsize)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(1, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(1, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(1, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(1, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -6127,15 +6197,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allocate_buffer);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 122, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 123, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -6143,46 +6213,46 @@
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_shape = ((PyObject*)values[0]);
-    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 122, __pyx_L3_error)
+    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 123, __pyx_L3_error)
     __pyx_v_format = values[2];
     __pyx_v_mode = values[3];
     if (values[4]) {
-      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 123, __pyx_L3_error)
+      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 124, __pyx_L3_error)
     } else {
 
-      /* "View.MemoryView":123
+      /* "View.MemoryView":124
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 123, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.array.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(1, 122, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(1, 123, __pyx_L1_error)
   if (unlikely(((PyObject *)__pyx_v_format) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(1, 122, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(1, 123, __pyx_L1_error)
   }
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(((struct __pyx_array_obj *)__pyx_v_self), __pyx_v_shape, __pyx_v_itemsize, __pyx_v_format, __pyx_v_mode, __pyx_v_allocate_buffer);
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -6216,579 +6286,579 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_format);
 
-  /* "View.MemoryView":129
+  /* "View.MemoryView":130
  *         cdef PyObject **p
  * 
  *         self.ndim = <int> len(shape)             # <<<<<<<<<<<<<<
  *         self.itemsize = itemsize
  * 
  */
   if (unlikely(__pyx_v_shape == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(1, 129, __pyx_L1_error)
+    __PYX_ERR(1, 130, __pyx_L1_error)
   }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 129, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 130, __pyx_L1_error)
   __pyx_v_self->ndim = ((int)__pyx_t_1);
 
-  /* "View.MemoryView":130
+  /* "View.MemoryView":131
  * 
  *         self.ndim = <int> len(shape)
  *         self.itemsize = itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not self.ndim:
  */
   __pyx_v_self->itemsize = __pyx_v_itemsize;
 
-  /* "View.MemoryView":132
+  /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_self->ndim != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":133
+    /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 133, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 133, __pyx_L1_error)
+    __PYX_ERR(1, 134, __pyx_L1_error)
 
-    /* "View.MemoryView":132
+    /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":135
+  /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   __pyx_t_2 = ((__pyx_v_itemsize <= 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":136
+    /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 136, __pyx_L1_error)
+    __PYX_ERR(1, 137, __pyx_L1_error)
 
-    /* "View.MemoryView":135
+    /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":138
+  /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_format); 
   __pyx_t_4 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":139
+    /* "View.MemoryView":140
  * 
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')             # <<<<<<<<<<<<<<
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 139, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_n_s_ASCII) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_ASCII);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 139, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_format, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":138
+    /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   }
 
-  /* "View.MemoryView":140
+  /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 140, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":141
+  /* "View.MemoryView":142
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format             # <<<<<<<<<<<<<<
  * 
  * 
  */
   if (unlikely(__pyx_v_self->_format == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 141, __pyx_L1_error)
+    __PYX_ERR(1, 142, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 142, __pyx_L1_error)
   __pyx_v_self->format = __pyx_t_7;
 
-  /* "View.MemoryView":144
+  /* "View.MemoryView":145
  * 
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)             # <<<<<<<<<<<<<<
  *         self._strides = self._shape + self.ndim
  * 
  */
   __pyx_v_self->_shape = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * __pyx_v_self->ndim) * 2)));
 
-  /* "View.MemoryView":145
+  /* "View.MemoryView":146
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)
  *         self._strides = self._shape + self.ndim             # <<<<<<<<<<<<<<
  * 
  *         if not self._shape:
  */
   __pyx_v_self->_strides = (__pyx_v_self->_shape + __pyx_v_self->ndim);
 
-  /* "View.MemoryView":147
+  /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   __pyx_t_4 = ((!(__pyx_v_self->_shape != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "View.MemoryView":148
+    /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 148, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 148, __pyx_L1_error)
+    __PYX_ERR(1, 149, __pyx_L1_error)
 
-    /* "View.MemoryView":147
+    /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   }
 
-  /* "View.MemoryView":151
+  /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   __pyx_t_8 = 0;
   __pyx_t_3 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(1, 151, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(1, 152, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 151, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 151, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 152, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_8;
     __pyx_t_8 = (__pyx_t_8 + 1);
 
-    /* "View.MemoryView":152
+    /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     __pyx_t_4 = ((__pyx_v_dim <= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":153
+      /* "View.MemoryView":154
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))             # <<<<<<<<<<<<<<
  *             self._shape[idx] = dim
  * 
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 153, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 153, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 153, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 153, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 153, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(1, 153, __pyx_L1_error)
+      __PYX_ERR(1, 154, __pyx_L1_error)
 
-      /* "View.MemoryView":152
+      /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     }
 
-    /* "View.MemoryView":154
+    /* "View.MemoryView":155
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim             # <<<<<<<<<<<<<<
  * 
  *         cdef char order
  */
     (__pyx_v_self->_shape[__pyx_v_idx]) = __pyx_v_dim;
 
-    /* "View.MemoryView":151
+    /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":157
+  /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 157, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 158, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":158
+    /* "View.MemoryView":159
  *         cdef char order
  *         if mode == 'fortran':
  *             order = b'F'             # <<<<<<<<<<<<<<
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  */
     __pyx_v_order = 'F';
 
-    /* "View.MemoryView":159
+    /* "View.MemoryView":160
  *         if mode == 'fortran':
  *             order = b'F'
  *             self.mode = u'fortran'             # <<<<<<<<<<<<<<
  *         elif mode == 'c':
  *             order = b'C'
  */
     __Pyx_INCREF(__pyx_n_u_fortran);
     __Pyx_GIVEREF(__pyx_n_u_fortran);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_fortran;
 
-    /* "View.MemoryView":157
+    /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":160
+  /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 160, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 161, __pyx_L1_error)
   if (likely(__pyx_t_4)) {
 
-    /* "View.MemoryView":161
+    /* "View.MemoryView":162
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  *             order = b'C'             # <<<<<<<<<<<<<<
  *             self.mode = u'c'
  *         else:
  */
     __pyx_v_order = 'C';
 
-    /* "View.MemoryView":162
+    /* "View.MemoryView":163
  *         elif mode == 'c':
  *             order = b'C'
  *             self.mode = u'c'             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  */
     __Pyx_INCREF(__pyx_n_u_c);
     __Pyx_GIVEREF(__pyx_n_u_c);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_c;
 
-    /* "View.MemoryView":160
+    /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":164
+  /* "View.MemoryView":165
  *             self.mode = u'c'
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)             # <<<<<<<<<<<<<<
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 164, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 164, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_10, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __PYX_ERR(1, 164, __pyx_L1_error)
+    __PYX_ERR(1, 165, __pyx_L1_error)
   }
   __pyx_L10:;
 
-  /* "View.MemoryView":166
+  /* "View.MemoryView":167
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,             # <<<<<<<<<<<<<<
  *                                              itemsize, self.ndim, order)
  * 
  */
   __pyx_v_self->len = __pyx_fill_contig_strides_array(__pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_itemsize, __pyx_v_self->ndim, __pyx_v_order);
 
-  /* "View.MemoryView":169
+  /* "View.MemoryView":170
  *                                              itemsize, self.ndim, order)
  * 
  *         self.free_data = allocate_buffer             # <<<<<<<<<<<<<<
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:
  */
   __pyx_v_self->free_data = __pyx_v_allocate_buffer;
 
-  /* "View.MemoryView":170
+  /* "View.MemoryView":171
  * 
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'             # <<<<<<<<<<<<<<
  *         if allocate_buffer:
  * 
  */
-  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 170, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_self->dtype_is_object = __pyx_t_4;
 
-  /* "View.MemoryView":171
+  /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = (__pyx_v_allocate_buffer != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":174
+    /* "View.MemoryView":175
  * 
  * 
  *             self.data = <char *>malloc(self.len)             # <<<<<<<<<<<<<<
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")
  */
     __pyx_v_self->data = ((char *)malloc(__pyx_v_self->len));
 
-    /* "View.MemoryView":175
+    /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     __pyx_t_4 = ((!(__pyx_v_self->data != 0)) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":176
+      /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 176, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(1, 176, __pyx_L1_error)
+      __PYX_ERR(1, 177, __pyx_L1_error)
 
-      /* "View.MemoryView":175
+      /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     }
 
-    /* "View.MemoryView":178
+    /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     __pyx_t_4 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":179
+      /* "View.MemoryView":180
  * 
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data             # <<<<<<<<<<<<<<
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  */
       __pyx_v_p = ((PyObject **)__pyx_v_self->data);
 
-      /* "View.MemoryView":180
+      /* "View.MemoryView":181
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):             # <<<<<<<<<<<<<<
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)
  */
       if (unlikely(__pyx_v_itemsize == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-        __PYX_ERR(1, 180, __pyx_L1_error)
+        __PYX_ERR(1, 181, __pyx_L1_error)
       }
       else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_self->len))) {
         PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-        __PYX_ERR(1, 180, __pyx_L1_error)
+        __PYX_ERR(1, 181, __pyx_L1_error)
       }
       __pyx_t_1 = (__pyx_v_self->len / __pyx_v_itemsize);
       __pyx_t_9 = __pyx_t_1;
       for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_9; __pyx_t_11+=1) {
         __pyx_v_i = __pyx_t_11;
 
-        /* "View.MemoryView":181
+        /* "View.MemoryView":182
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None             # <<<<<<<<<<<<<<
  *                     Py_INCREF(Py_None)
  * 
  */
         (__pyx_v_p[__pyx_v_i]) = Py_None;
 
-        /* "View.MemoryView":182
+        /* "View.MemoryView":183
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
         Py_INCREF(Py_None);
       }
 
-      /* "View.MemoryView":178
+      /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     }
 
-    /* "View.MemoryView":171
+    /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -6804,15 +6874,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_format);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":185
+/* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -6847,249 +6917,249 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":186
+  /* "View.MemoryView":187
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1             # <<<<<<<<<<<<<<
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
   __pyx_v_bufmode = -1;
 
-  /* "View.MemoryView":187
+  /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 187, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 188, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":188
+    /* "View.MemoryView":189
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
     __pyx_v_bufmode = (PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":187
+    /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":189
+  /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 189, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 190, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":190
+    /* "View.MemoryView":191
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  */
     __pyx_v_bufmode = (PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":189
+    /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":191
+  /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   __pyx_t_1 = ((!((__pyx_v_flags & __pyx_v_bufmode) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":192
+    /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 192, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 192, __pyx_L1_error)
+    __PYX_ERR(1, 193, __pyx_L1_error)
 
-    /* "View.MemoryView":191
+    /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   }
 
-  /* "View.MemoryView":193
+  /* "View.MemoryView":194
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data             # <<<<<<<<<<<<<<
  *         info.len = self.len
  *         info.ndim = self.ndim
  */
   __pyx_t_4 = __pyx_v_self->data;
   __pyx_v_info->buf = __pyx_t_4;
 
-  /* "View.MemoryView":194
+  /* "View.MemoryView":195
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  *         info.len = self.len             # <<<<<<<<<<<<<<
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  */
   __pyx_t_5 = __pyx_v_self->len;
   __pyx_v_info->len = __pyx_t_5;
 
-  /* "View.MemoryView":195
+  /* "View.MemoryView":196
  *         info.buf = self.data
  *         info.len = self.len
  *         info.ndim = self.ndim             # <<<<<<<<<<<<<<
  *         info.shape = self._shape
  *         info.strides = self._strides
  */
   __pyx_t_6 = __pyx_v_self->ndim;
   __pyx_v_info->ndim = __pyx_t_6;
 
-  /* "View.MemoryView":196
+  /* "View.MemoryView":197
  *         info.len = self.len
  *         info.ndim = self.ndim
  *         info.shape = self._shape             # <<<<<<<<<<<<<<
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  */
   __pyx_t_7 = __pyx_v_self->_shape;
   __pyx_v_info->shape = __pyx_t_7;
 
-  /* "View.MemoryView":197
+  /* "View.MemoryView":198
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  *         info.strides = self._strides             # <<<<<<<<<<<<<<
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  */
   __pyx_t_7 = __pyx_v_self->_strides;
   __pyx_v_info->strides = __pyx_t_7;
 
-  /* "View.MemoryView":198
+  /* "View.MemoryView":199
  *         info.shape = self._shape
  *         info.strides = self._strides
  *         info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *         info.itemsize = self.itemsize
  *         info.readonly = 0
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "View.MemoryView":199
+  /* "View.MemoryView":200
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize             # <<<<<<<<<<<<<<
  *         info.readonly = 0
  * 
  */
   __pyx_t_5 = __pyx_v_self->itemsize;
   __pyx_v_info->itemsize = __pyx_t_5;
 
-  /* "View.MemoryView":200
+  /* "View.MemoryView":201
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  *         info.readonly = 0             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   __pyx_v_info->readonly = 0;
 
-  /* "View.MemoryView":202
+  /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":203
+    /* "View.MemoryView":204
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_4 = __pyx_v_self->format;
     __pyx_v_info->format = __pyx_t_4;
 
-    /* "View.MemoryView":202
+    /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
     goto __pyx_L5;
   }
 
-  /* "View.MemoryView":205
+  /* "View.MemoryView":206
  *             info.format = self.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.obj = self
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L5:;
 
-  /* "View.MemoryView":207
+  /* "View.MemoryView":208
  *             info.format = NULL
  * 
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":185
+  /* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -7111,15 +7181,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":211
+/* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
@@ -7135,122 +7205,122 @@
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":212
+  /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
   __pyx_t_1 = ((__pyx_v_self->callback_free_data != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":213
+    /* "View.MemoryView":214
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)             # <<<<<<<<<<<<<<
  *         elif self.free_data:
  *             if self.dtype_is_object:
  */
     __pyx_v_self->callback_free_data(__pyx_v_self->data);
 
-    /* "View.MemoryView":212
+    /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":214
+  /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   __pyx_t_1 = (__pyx_v_self->free_data != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":215
+    /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":216
+      /* "View.MemoryView":217
  *         elif self.free_data:
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,             # <<<<<<<<<<<<<<
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_self->data, __pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_self->ndim, 0);
 
-      /* "View.MemoryView":215
+      /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     }
 
-    /* "View.MemoryView":218
+    /* "View.MemoryView":219
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  *             free(self.data)             # <<<<<<<<<<<<<<
  *         PyObject_Free(self._shape)
  * 
  */
     free(__pyx_v_self->data);
 
-    /* "View.MemoryView":214
+    /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":219
+  /* "View.MemoryView":220
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  *         PyObject_Free(self._shape)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   PyObject_Free(__pyx_v_self->_shape);
 
-  /* "View.MemoryView":211
+  /* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":222
+/* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -7272,29 +7342,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":223
+  /* "View.MemoryView":224
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 223, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":222
+  /* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -7305,15 +7375,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":226
+/* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -7325,54 +7395,54 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_memview", 0);
 
-  /* "View.MemoryView":227
+  /* "View.MemoryView":228
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  */
   __pyx_v_flags = ((PyBUF_ANY_CONTIGUOUS | PyBUF_FORMAT) | PyBUF_WRITABLE);
 
-  /* "View.MemoryView":228
+  /* "View.MemoryView":229
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":226
+  /* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -7385,15 +7455,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":230
+/* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
@@ -7411,39 +7481,39 @@
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":231
+  /* "View.MemoryView":232
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
  */
   __pyx_r = (__pyx_v_self->_shape[0]);
   goto __pyx_L0;
 
-  /* "View.MemoryView":230
+  /* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":233
+/* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -7466,32 +7536,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
 
-  /* "View.MemoryView":234
+  /* "View.MemoryView":235
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 234, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 234, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":233
+  /* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -7503,15 +7573,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":236
+/* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -7534,32 +7604,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":237
+  /* "View.MemoryView":238
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 237, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 237, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":236
+  /* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -7571,15 +7641,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":239
+/* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -7601,27 +7671,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
-  /* "View.MemoryView":240
+  /* "View.MemoryView":241
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(1, 240, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(1, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":239
+  /* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -7746,15 +7816,15 @@
   __Pyx_AddTraceback("View.MemoryView.array.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":244
+/* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -7768,145 +7838,145 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_cwrapper", 0);
 
-  /* "View.MemoryView":248
+  /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_buf == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":249
+    /* "View.MemoryView":250
  * 
  *     if buf == NULL:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))             # <<<<<<<<<<<<<<
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":248
+    /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":251
+  /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
   /*else*/ {
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":252
+    /* "View.MemoryView":253
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)             # <<<<<<<<<<<<<<
  *         result.data = buf
  * 
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 252, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(1, 252, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(1, 253, __pyx_L1_error)
 
-    /* "View.MemoryView":251
+    /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "View.MemoryView":253
+    /* "View.MemoryView":254
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)
  *         result.data = buf             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_v_result->data = __pyx_v_buf;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":255
+  /* "View.MemoryView":256
  *         result.data = buf
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":244
+  /* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -7921,15 +7991,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":281
+/* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
@@ -7958,26 +8028,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 281, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 282, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 281, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 282, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.Enum.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v_name);
 
@@ -7987,42 +8057,42 @@
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "View.MemoryView":282
+  /* "View.MemoryView":283
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
  */
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_v_name;
 
-  /* "View.MemoryView":281
+  /* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":283
+/* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -8040,27 +8110,27 @@
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":284
+  /* "View.MemoryView":285
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "View.MemoryView":283
+  /* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -8335,15 +8405,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -8360,98 +8430,98 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":298
+/* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
 static void *__pyx_align_pointer(void *__pyx_v_memory, size_t __pyx_v_alignment) {
   Py_intptr_t __pyx_v_aligned_p;
   size_t __pyx_v_offset;
   void *__pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":300
+  /* "View.MemoryView":301
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory             # <<<<<<<<<<<<<<
  *     cdef size_t offset
  * 
  */
   __pyx_v_aligned_p = ((Py_intptr_t)__pyx_v_memory);
 
-  /* "View.MemoryView":304
+  /* "View.MemoryView":305
  * 
  *     with cython.cdivision(True):
  *         offset = aligned_p % alignment             # <<<<<<<<<<<<<<
  * 
  *     if offset > 0:
  */
   __pyx_v_offset = (__pyx_v_aligned_p % __pyx_v_alignment);
 
-  /* "View.MemoryView":306
+  /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   __pyx_t_1 = ((__pyx_v_offset > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":307
+    /* "View.MemoryView":308
  * 
  *     if offset > 0:
  *         aligned_p += alignment - offset             # <<<<<<<<<<<<<<
  * 
  *     return <void *> aligned_p
  */
     __pyx_v_aligned_p = (__pyx_v_aligned_p + (__pyx_v_alignment - __pyx_v_offset));
 
-    /* "View.MemoryView":306
+    /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   }
 
-  /* "View.MemoryView":309
+  /* "View.MemoryView":310
  *         aligned_p += alignment - offset
  * 
  *     return <void *> aligned_p             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((void *)__pyx_v_aligned_p);
   goto __pyx_L0;
 
-  /* "View.MemoryView":298
+  /* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":345
+/* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -8488,47 +8558,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(1, 345, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(1, 346, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype_is_object);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 345, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 346, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_obj = values[0];
-    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 345, __pyx_L3_error)
+    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 346, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 345, __pyx_L3_error)
+      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 346, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 345, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 346, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_obj, __pyx_v_flags, __pyx_v_dtype_is_object);
 
@@ -8545,37 +8615,37 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "View.MemoryView":346
+  /* "View.MemoryView":347
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  */
   __Pyx_INCREF(__pyx_v_obj);
   __Pyx_GIVEREF(__pyx_v_obj);
   __Pyx_GOTREF(__pyx_v_self->obj);
   __Pyx_DECREF(__pyx_v_self->obj);
   __pyx_v_self->obj = __pyx_v_obj;
 
-  /* "View.MemoryView":347
+  /* "View.MemoryView":348
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj
  *         self.flags = flags             # <<<<<<<<<<<<<<
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  */
   __pyx_v_self->flags = __pyx_v_flags;
 
-  /* "View.MemoryView":348
+  /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   __pyx_t_2 = (((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))) == ((PyObject *)__pyx_memoryview_type));
@@ -8587,231 +8657,250 @@
   }
   __pyx_t_3 = (__pyx_v_obj != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":349
+    /* "View.MemoryView":350
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)             # <<<<<<<<<<<<<<
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  */
-    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 349, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 350, __pyx_L1_error)
 
-    /* "View.MemoryView":350
+    /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     __pyx_t_1 = ((((PyObject *)__pyx_v_self->view.obj) == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":351
+      /* "View.MemoryView":352
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None             # <<<<<<<<<<<<<<
  *                 Py_INCREF(Py_None)
  * 
  */
       ((Py_buffer *)(&__pyx_v_self->view))->obj = Py_None;
 
-      /* "View.MemoryView":352
+      /* "View.MemoryView":353
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
- *         global __pyx_memoryview_thread_locks_used
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
  */
       Py_INCREF(Py_None);
 
-      /* "View.MemoryView":350
+      /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     }
 
-    /* "View.MemoryView":348
+    /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   }
 
   /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
  * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
-  __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+  __pyx_t_1 = ((!(__PYX_CYTHON_ATOMICS_ENABLED() != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":356
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- */
-    __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
-
     /* "View.MemoryView":357
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
-    __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
+    __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+    if (__pyx_t_1) {
 
-    /* "View.MemoryView":355
- * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+      /* "View.MemoryView":358
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
+ *                 __pyx_memoryview_thread_locks_used += 1
+ *             if self.lock is NULL:
  */
-  }
+      __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
 
-  /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
+      /* "View.MemoryView":359
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
  *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
  */
-  __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-  if (__pyx_t_1) {
+      __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
 
-    /* "View.MemoryView":359
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
- *             if self.lock is NULL:
- *                 raise MemoryError
+      /* "View.MemoryView":357
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
-    __pyx_v_self->lock = PyThread_allocate_lock();
+    }
 
     /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-    if (unlikely(__pyx_t_1)) {
+    if (__pyx_t_1) {
 
       /* "View.MemoryView":361
- *             self.lock = PyThread_allocate_lock()
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:
- *                 raise MemoryError             # <<<<<<<<<<<<<<
+ *                 self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
+ *                 if self.lock is NULL:
+ *                     raise MemoryError
+ */
+      __pyx_v_self->lock = PyThread_allocate_lock();
+
+      /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
+      if (unlikely(__pyx_t_1)) {
+
+        /* "View.MemoryView":363
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
+ *                     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-      PyErr_NoMemory(); __PYX_ERR(1, 361, __pyx_L1_error)
+        PyErr_NoMemory(); __PYX_ERR(1, 363, __pyx_L1_error)
+
+        /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      }
 
       /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     }
 
-    /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
- *             if self.lock is NULL:
+    /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
+ * 
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
   }
 
-  /* "View.MemoryView":363
- *                 raise MemoryError
+  /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":364
+    /* "View.MemoryView":366
  * 
  *         if flags & PyBUF_FORMAT:
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')             # <<<<<<<<<<<<<<
  *         else:
  *             self.dtype_is_object = dtype_is_object
  */
     __pyx_t_2 = (((__pyx_v_self->view.format[0]) == 'O') != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L11_bool_binop_done;
+      goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_self->view.format[1]) == '\x00') != 0);
     __pyx_t_1 = __pyx_t_2;
-    __pyx_L11_bool_binop_done:;
+    __pyx_L12_bool_binop_done:;
     __pyx_v_self->dtype_is_object = __pyx_t_1;
 
-    /* "View.MemoryView":363
- *                 raise MemoryError
+    /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
-    goto __pyx_L10;
+    goto __pyx_L11;
   }
 
-  /* "View.MemoryView":366
+  /* "View.MemoryView":368
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  *             self.dtype_is_object = dtype_is_object             # <<<<<<<<<<<<<<
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  */
   /*else*/ {
     __pyx_v_self->dtype_is_object = __pyx_v_dtype_is_object;
   }
-  __pyx_L10:;
+  __pyx_L11:;
 
-  /* "View.MemoryView":368
+  /* "View.MemoryView":370
  *             self.dtype_is_object = dtype_is_object
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(             # <<<<<<<<<<<<<<
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL
  */
   __pyx_v_self->acquisition_count_aligned_p = ((__pyx_atomic_int *)__pyx_align_pointer(((void *)(&(__pyx_v_self->acquisition_count[0]))), (sizeof(__pyx_atomic_int))));
 
-  /* "View.MemoryView":370
+  /* "View.MemoryView":372
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(memoryview self):
  */
   __pyx_v_self->typeinfo = NULL;
 
-  /* "View.MemoryView":345
+  /* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -8822,15 +8911,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":372
+/* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
@@ -8853,215 +8942,215 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
   PyThread_type_lock __pyx_t_7;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":373
+  /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":374
+    /* "View.MemoryView":376
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
-    /* "View.MemoryView":373
+    /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":375
+  /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":377
+    /* "View.MemoryView":379
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
  *             Py_DECREF(Py_None)
  * 
  */
     ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
 
-    /* "View.MemoryView":378
+    /* "View.MemoryView":380
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
     Py_DECREF(Py_None);
 
-    /* "View.MemoryView":375
+    /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":385
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":387
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":390
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":389
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":391
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":393
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
 
-  /* "View.MemoryView":372
+  /* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -9079,107 +9168,107 @@
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":397
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 399, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 397, __pyx_L1_error)
+          else __PYX_ERR(1, 399, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":400
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 398, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 400, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 400, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":402
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -9191,15 +9280,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -9229,143 +9318,143 @@
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":407
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":409
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 407, __pyx_L1_error)
+      __PYX_ERR(1, 409, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 409, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 412, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":413
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":415
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 415, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":416
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -9380,15 +9469,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -9416,182 +9505,182 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 418, __pyx_L1_error)
+    __PYX_ERR(1, 420, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":422
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 420, __pyx_L1_error)
+      __PYX_ERR(1, 422, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 422, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 422, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 424, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":425
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 424, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 426, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":427
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":429
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 429, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":431
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -9608,15 +9697,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -9634,26 +9723,26 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -9661,59 +9750,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":437
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 435, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 437, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -9722,30 +9811,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":438
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 438, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":439
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -9754,15 +9843,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -9775,36 +9864,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":441
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -9818,15 +9907,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -9842,60 +9931,60 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 445, __pyx_L1_error)
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 445, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":448
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 446, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 446, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 448, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 448, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":449
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 445, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -9908,15 +9997,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -9941,204 +10030,204 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":453
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":458
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 456, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 458, __pyx_L1_error)
   __pyx_v_dst_slice = __pyx_t_1;
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
   __pyx_t_2 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":461
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     __pyx_t_2 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":463
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(1, 461, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(1, 463, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":464
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":466
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":468
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
     __pyx_t_2 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":470
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":472
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 470, __pyx_L6_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 472, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     __pyx_t_2 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":477
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 475, __pyx_L6_error)
+      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 477, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":478
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":481
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -10177,15 +10266,15 @@
       __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_6;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -10198,15 +10287,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -10217,36 +10306,36 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":484
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 484, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":485
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 483, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -10259,15 +10348,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10289,39 +10378,39 @@
   size_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":490
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":493
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 491, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -10329,24 +10418,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":495
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -10355,94 +10444,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":500
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 500, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":501
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -10453,52 +10542,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":496
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 496, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 496, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -10510,15 +10599,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10536,15 +10625,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10570,88 +10659,88 @@
   char *__pyx_t_13;
   char *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":506
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":512
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":514
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -10660,102 +10749,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(1, 514, __pyx_L1_error)
+    __PYX_ERR(1, 516, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10775,15 +10864,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -10818,15 +10907,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -10836,268 +10925,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 520, __pyx_L1_error)
+    __PYX_ERR(1, 522, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":525
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":527
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":530
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":532
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":535
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":537
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":540
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":542
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":544
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":545
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":546
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":547
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":548
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":549
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -11119,15 +11208,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -11151,49 +11240,49 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 556, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":557
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 555, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 557, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":558
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -11205,15 +11294,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -11231,42 +11320,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -11293,41 +11382,41 @@
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":566
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 566, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -11339,15 +11428,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -11375,73 +11464,73 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 570, __pyx_L1_error)
+    __PYX_ERR(1, 572, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":574
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 574, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -11453,15 +11542,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -11489,77 +11578,77 @@
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__15, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__15, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":581
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 581, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 581, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -11571,15 +11660,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -11601,29 +11690,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":585
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -11634,15 +11723,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -11664,29 +11753,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":589
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -11697,15 +11786,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -11729,35 +11818,35 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":593
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -11770,15 +11859,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -11807,98 +11896,98 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":598
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":600
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 600, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":601
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 599, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 601, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":603
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":605
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -11911,15 +12000,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -11938,68 +12027,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":609
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":611
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -12023,64 +12112,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":615
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -12093,15 +12182,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -12124,43 +12213,43 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":618
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -12172,15 +12261,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12205,39 +12294,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 622, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 624, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 623, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12248,15 +12337,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12281,39 +12370,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":630
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 628, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(1, 630, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":631
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 629, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12324,15 +12413,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -12357,57 +12446,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":635
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":637
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":638
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 638, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":643
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -12418,15 +12507,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -12452,57 +12541,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":647
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":649
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":650
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 648, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 650, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":655
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -12626,15 +12715,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -12646,64 +12735,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":661
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":662
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -12717,54 +12806,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":666
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -12790,243 +12879,243 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":674
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 674, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":676
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":678
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 676, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":679
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":680
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 681, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 679, __pyx_L1_error)
+          else __PYX_ERR(1, 681, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__18);
             __Pyx_GIVEREF(__pyx_slice__18);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__18);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":685
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":687
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__18); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__18); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -13038,40 +13127,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":691
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(1, 689, __pyx_L1_error)
+        __PYX_ERR(1, 691, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":693
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -13082,120 +13171,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":694
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 694, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":696
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 694, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 696, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":698
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__18);
         __Pyx_GIVEREF(__pyx_slice__18);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__18);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":700
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -13213,15 +13302,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -13235,60 +13324,60 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":703
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(1, 703, __pyx_L1_error)
+      __PYX_ERR(1, 705, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -13301,15 +13390,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -13345,529 +13434,529 @@
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":713
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":720
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":724
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 722, __pyx_L1_error)
+      __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":727
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 725, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 727, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":728
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":730
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":731
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":737
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":738
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":743
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":744
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 748, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 746, __pyx_L1_error)
+          else __PYX_ERR(1, 748, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":753
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 751, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 753, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":750
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 748, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 750, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":757
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":758
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":759
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":760
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":762
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 762, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 762, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":763
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 763, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 763, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 763, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":764
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 764, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 764, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 764, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":766
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 766, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":767
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 765, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 767, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":768
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 768, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":770
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 768, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 770, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":776
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":780
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 778, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 780, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":781
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 779, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 781, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 777, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 779, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":785
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 782, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 782, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 784, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -13881,15 +13970,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -13900,95 +13989,95 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":832
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":834
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":837
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -13999,15 +14088,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -14017,639 +14106,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":840
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 840, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":845
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":847
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":850
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":852
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":855
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":857
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":861
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":863
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":865
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":868
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":870
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":873
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":877
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":880
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":883
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":886
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":887
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":888
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":892
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":894
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":899
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":901
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":902
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 899, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 901, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":904
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":906
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -14665,15 +14754,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -14690,280 +14779,280 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":914
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":915
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":919
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 919, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 919, __pyx_L1_error)
     }
     __pyx_v_shape = (__pyx_v_view->len / __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":920
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":922
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":923
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":925
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":928
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":930
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 928, __pyx_L1_error)
+      __PYX_ERR(1, 930, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":933
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 931, __pyx_L1_error)
+    __PYX_ERR(1, 933, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":935
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":937
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":939
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -14974,15 +15063,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -15002,90 +15091,90 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":946
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":948
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":949
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":953
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = (__pyx_v_ndim / 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":954
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":955
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":956
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -15095,44 +15184,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":959
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 959, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":961
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -15148,15 +15237,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -15171,36 +15260,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":979
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -15210,64 +15299,64 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":983
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 983, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":985
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -15278,15 +15367,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -15297,58 +15386,58 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":989
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 987, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 989, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":991
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 991, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -15361,15 +15450,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -15387,27 +15476,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":995
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -15527,15 +15616,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -15555,351 +15644,351 @@
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1010
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1015
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1017
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1018
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1020
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1018, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1020, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1021
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1023
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1024
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1025
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1026
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1027
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1030
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1032
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1034
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1035
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1038
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1039
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1041
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1042
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1044
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1045
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1045, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1046
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1046, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1048
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1049
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1051
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -15913,15 +16002,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -15933,79 +16022,79 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1055
+  /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1058
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1056, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1058, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1059
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
+    /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1061
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1062
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -16016,15 +16105,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -16037,120 +16126,120 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1069
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1070
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1071
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1073
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1074
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1076
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1077
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1078
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1079
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -16160,38 +16249,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1085
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1086
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1086, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -16202,15 +16291,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -16225,99 +16314,99 @@
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1097
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1098
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1100
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1101
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1103
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1105
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1101, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -16328,81 +16417,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1113
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1115
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -16412,187 +16501,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1123
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1124
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1126
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1128
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1129
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1131
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1133
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1134
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1137
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1139
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -16605,61 +16694,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1149
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1150
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1151
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1152
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -16671,195 +16760,195 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1156
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1157
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1159
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1160
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1161
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1162
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1164
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1165
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1169
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1170
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1175
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
@@ -16868,70 +16957,70 @@
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
 
-  /* "View.MemoryView":1179
+  /* "View.MemoryView":1181
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for shape in src.shape[:ndim]:
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1181
+  /* "View.MemoryView":1183
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  * 
  *     for shape in src.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         size *= shape
  * 
  */
   __pyx_t_3 = (__pyx_v_src->shape + __pyx_v_ndim);
   for (__pyx_t_4 = __pyx_v_src->shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_shape = (__pyx_t_2[0]);
 
-    /* "View.MemoryView":1182
+    /* "View.MemoryView":1184
  * 
  *     for shape in src.shape[:ndim]:
  *         size *= shape             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size * __pyx_v_shape);
   }
 
-  /* "View.MemoryView":1184
+  /* "View.MemoryView":1186
  *         size *= shape
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1187
+/* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -16939,121 +17028,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1196
+  /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1199
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1198
+      /* "View.MemoryView":1200
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1201
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1196
+    /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1201
+  /* "View.MemoryView":1203
  *             stride *= shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1202
+      /* "View.MemoryView":1204
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1205
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1205
+  /* "View.MemoryView":1207
  *             stride *= shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1187
+  /* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1208
+/* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -17069,222 +17158,222 @@
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1219
+  /* "View.MemoryView":1221
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1222
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1222
+  /* "View.MemoryView":1224
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1226
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1224, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1226, __pyx_L1_error)
 
-    /* "View.MemoryView":1223
+    /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1227
+  /* "View.MemoryView":1229
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1230
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1231
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1230
+    /* "View.MemoryView":1232
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1233
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1233
+  /* "View.MemoryView":1235
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1237
+  /* "View.MemoryView":1239
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1238
+    /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1241
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1238
+      /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1241
+  /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1244
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1241
+    /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1244
+  /* "View.MemoryView":1246
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1246
+  /* "View.MemoryView":1248
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1208
+  /* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -17300,15 +17389,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1251
+/* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -17323,57 +17412,57 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1256
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1253
+  /* "View.MemoryView":1255
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1253, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1253, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(1, 1253, __pyx_L1_error)
+  __PYX_ERR(1, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1251
+  /* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -17388,15 +17477,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1257
+/* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -17412,26 +17501,26 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1260
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -17441,22 +17530,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 1258, __pyx_L1_error)
+  __PYX_ERR(1, 1260, __pyx_L1_error)
 
-  /* "View.MemoryView":1257
+  /* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -17472,15 +17561,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1261
+/* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -17497,32 +17586,32 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1265
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1263, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -17530,43 +17619,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1263, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 1263, __pyx_L1_error)
+    __PYX_ERR(1, 1265, __pyx_L1_error)
 
-    /* "View.MemoryView":1262
+    /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1265
+  /* "View.MemoryView":1267
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(1, 1265, __pyx_L1_error)
+    __PYX_ERR(1, 1267, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1261
+  /* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -17582,15 +17671,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1268
+/* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -17612,119 +17701,119 @@
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1276
+  /* "View.MemoryView":1278
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1279
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1279
+  /* "View.MemoryView":1281
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1282
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1283
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1284
+  /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1287
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1284
+    /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1286
+  /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1289
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1289
+  /* "View.MemoryView":1291
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -17732,420 +17821,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1291
+  /* "View.MemoryView":1293
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1292
+    /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1296
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1297
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1293
+        /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1297
+      /* "View.MemoryView":1299
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1297, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1299, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1292
+      /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1299
+    /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1302
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1300, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1302, __pyx_L1_error)
 
-      /* "View.MemoryView":1299
+      /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1302
+  /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1304
+    /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1307
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1304
+      /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1307
+    /* "View.MemoryView":1309
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1307, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1309, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1310
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1302
+    /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1310
+  /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1313
+    /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1316
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1313
+      /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1315
+    /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1318
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1318
+    /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1320
+      /* "View.MemoryView":1322
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1323
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1324
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1325
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1326
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1318
+      /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1310
+    /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1326
+  /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1329
+    /* "View.MemoryView":1331
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1329, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1331, __pyx_L1_error)
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1332
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1330, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1332, __pyx_L1_error)
 
-    /* "View.MemoryView":1326
+    /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1332
+  /* "View.MemoryView":1334
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1335
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1336
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1336
+  /* "View.MemoryView":1338
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1339
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1268
+  /* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -18161,217 +18250,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1340
+/* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1344
+  /* "View.MemoryView":1346
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1346
+  /* "View.MemoryView":1348
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1347
+    /* "View.MemoryView":1349
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1350
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1351
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1351
+  /* "View.MemoryView":1353
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1352
+    /* "View.MemoryView":1354
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1355
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1356
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1340
+  /* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1362
+/* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1366
+  /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1369
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1366
+    /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1362
+  /* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1371
+/* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1374
+  /* "View.MemoryView":1376
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1371
+  /* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1377
+/* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -18380,178 +18469,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1381
+  /* "View.MemoryView":1383
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1382
+    /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1386
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1383
+        /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1386
+      /* "View.MemoryView":1388
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1382
+      /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1388
+    /* "View.MemoryView":1390
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1389
+      /* "View.MemoryView":1391
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1391
+    /* "View.MemoryView":1393
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1377
+  /* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1397
+/* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1400
+  /* "View.MemoryView":1402
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1403
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1403
+  /* "View.MemoryView":1405
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1397
+  /* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1407
+/* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -18560,118 +18649,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1411
+  /* "View.MemoryView":1413
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1414
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1414
+  /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1417
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1416
+      /* "View.MemoryView":1418
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1419
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1414
+    /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1419
+  /* "View.MemoryView":1421
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1420
+      /* "View.MemoryView":1422
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1422
+      /* "View.MemoryView":1424
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1407
+  /* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -18895,15 +18984,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -19074,53 +19163,53 @@
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_9SuperPang_3lib_10Compressor_Compressor __pyx_vtable_9SuperPang_3lib_10Compressor_Compressor;
+static struct __pyx_vtabstruct_9superpang_3lib_10Compressor_Compressor __pyx_vtable_9superpang_3lib_10Compressor_Compressor;
 
-static PyObject *__pyx_tp_new_9SuperPang_3lib_10Compressor_Compressor(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *p;
+static PyObject *__pyx_tp_new_9superpang_3lib_10Compressor_Compressor(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *)o);
-  p->__pyx_vtab = __pyx_vtabptr_9SuperPang_3lib_10Compressor_Compressor;
+  p = ((struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *)o);
+  p->__pyx_vtab = __pyx_vtabptr_9superpang_3lib_10Compressor_Compressor;
   return o;
 }
 
-static void __pyx_tp_dealloc_9SuperPang_3lib_10Compressor_Compressor(PyObject *o) {
+static void __pyx_tp_dealloc_9superpang_3lib_10Compressor_Compressor(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_9SuperPang_3lib_10Compressor_Compressor[] = {
-  {"compress", (PyCFunction)__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_3compress, METH_O, 0},
-  {"decompress", (PyCFunction)__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_5decompress, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_7__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_9__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_9superpang_3lib_10Compressor_Compressor[] = {
+  {"compress", (PyCFunction)__pyx_pw_9superpang_3lib_10Compressor_10Compressor_3compress, METH_O, 0},
+  {"decompress", (PyCFunction)__pyx_pw_9superpang_3lib_10Compressor_10Compressor_5decompress, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9superpang_3lib_10Compressor_10Compressor_7__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9superpang_3lib_10Compressor_10Compressor_9__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_9SuperPang_3lib_10Compressor_Compressor = {
+static PyTypeObject __pyx_type_9superpang_3lib_10Compressor_Compressor = {
   PyVarObject_HEAD_INIT(0, 0)
-  "SuperPang.lib.Compressor.Compressor", /*tp_name*/
-  sizeof(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor), /*tp_basicsize*/
+  "superpang.lib.Compressor.Compressor", /*tp_name*/
+  sizeof(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_9SuperPang_3lib_10Compressor_Compressor, /*tp_dealloc*/
+  __pyx_tp_dealloc_9superpang_3lib_10Compressor_Compressor, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -19145,25 +19234,25 @@
   "\n    Hash a nucleotide sequence into a compressed form\n    Each tetranucleotide will be stored as a single byte\n    When the sequence length is not divisible by 4, each\n     remaining base will be stored as a byte\n    ", /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_9SuperPang_3lib_10Compressor_Compressor, /*tp_methods*/
+  __pyx_methods_9superpang_3lib_10Compressor_Compressor, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
-  __pyx_pw_9SuperPang_3lib_10Compressor_10Compressor_1__init__, /*tp_init*/
+  __pyx_pw_9superpang_3lib_10Compressor_10Compressor_1__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_9SuperPang_3lib_10Compressor_Compressor, /*tp_new*/
+  __pyx_tp_new_9superpang_3lib_10Compressor_Compressor, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -19174,15 +19263,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -19203,15 +19292,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -19301,15 +19390,15 @@
   #endif
   __pyx_array_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_array = {
   PyVarObject_HEAD_INIT(0, 0)
-  "SuperPang.lib.Compressor.array", /*tp_name*/
+  "superpang.lib.Compressor.array", /*tp_name*/
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_array, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19366,15 +19455,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -19388,15 +19477,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -19423,15 +19512,15 @@
   {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
-  "SuperPang.lib.Compressor.Enum", /*tp_name*/
+  "superpang.lib.Compressor.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19488,15 +19577,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -19519,15 +19608,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19687,15 +19776,15 @@
   #endif
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_memoryview = {
   PyVarObject_HEAD_INIT(0, 0)
-  "SuperPang.lib.Compressor.memoryview", /*tp_name*/
+  "superpang.lib.Compressor.memoryview", /*tp_name*/
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19752,15 +19841,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -19772,15 +19861,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19828,15 +19917,15 @@
 static struct PyGetSetDef __pyx_getsets__memoryviewslice[] = {
   {(char *)"base", __pyx_getprop___pyx_memoryviewslice_base, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
   PyVarObject_HEAD_INIT(0, 0)
-  "SuperPang.lib.Compressor._memoryviewslice", /*tp_name*/
+  "superpang.lib.Compressor._memoryviewslice", /*tp_name*/
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19901,15 +19990,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -19979,15 +20068,14 @@
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_n_s_SuperPang_lib_Compressor, __pyx_k_SuperPang_lib_Compressor, sizeof(__pyx_k_SuperPang_lib_Compressor), 0, 0, 1, 1},
   {&__pyx_n_u_T, __pyx_k_T, sizeof(__pyx_k_T), 0, 1, 0, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
@@ -20050,35 +20138,36 @@
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
+  {&__pyx_n_s_superpang_lib_Compressor, __pyx_k_superpang_lib_Compressor, sizeof(__pyx_k_superpang_lib_Compressor), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_tounicode, __pyx_k_tounicode, sizeof(__pyx_k_tounicode), 0, 0, 1, 1},
   {&__pyx_n_u_u, __pyx_k_u, sizeof(__pyx_k_u), 0, 1, 0, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 36, __pyx_L1_error)
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 89, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 109, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 945, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 133, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(3, 941, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 134, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -20091,88 +20180,88 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x708d54a, 0xcae9114, 0x5d96da1) = (clength, com, ksize, rem))" % __pyx_checksum)
  */
   __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_118019402, __pyx_int_212766996, __pyx_int_98135457); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(3, 945, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(3, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../miniconda3/envs/SuperPang/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-8deoat1_/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 951, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "View.MemoryView":133
+  /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 133, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "View.MemoryView":136
+  /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "View.MemoryView":148
+  /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "View.MemoryView":176
+  /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "View.MemoryView":192
+  /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 192, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20187,66 +20276,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 418, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 495, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 520, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 570, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__15 = PyTuple_New(1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_New(1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__15, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":2
@@ -20264,33 +20353,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "View.MemoryView":682
+  /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__18 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__18)) __PYX_ERR(1, 682, __pyx_L1_error)
+  __pyx_slice__18 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__18)) __PYX_ERR(1, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__18);
   __Pyx_GIVEREF(__pyx_slice__18);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 703, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 705, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20318,66 +20407,66 @@
  *     cdef object __pyx_result
  */
   __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Compressor, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -20390,15 +20479,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_98135457 = PyInt_FromLong(98135457L); if (unlikely(!__pyx_int_98135457)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_118019402 = PyInt_FromLong(118019402L); if (unlikely(!__pyx_int_118019402)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20449,77 +20543,77 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_9SuperPang_3lib_10Compressor_Compressor = &__pyx_vtable_9SuperPang_3lib_10Compressor_Compressor;
-  __pyx_vtable_9SuperPang_3lib_10Compressor_Compressor.change_base = (int (*)(struct __pyx_obj_9SuperPang_3lib_10Compressor_Compressor *, int, int, int))__pyx_f_9SuperPang_3lib_10Compressor_10Compressor_change_base;
-  if (PyType_Ready(&__pyx_type_9SuperPang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_vtabptr_9superpang_3lib_10Compressor_Compressor = &__pyx_vtable_9superpang_3lib_10Compressor_Compressor;
+  __pyx_vtable_9superpang_3lib_10Compressor_Compressor.change_base = (int (*)(struct __pyx_obj_9superpang_3lib_10Compressor_Compressor *, int, int, int))__pyx_f_9superpang_3lib_10Compressor_10Compressor_change_base;
+  if (PyType_Ready(&__pyx_type_9superpang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_9SuperPang_3lib_10Compressor_Compressor.tp_print = 0;
+  __pyx_type_9superpang_3lib_10Compressor_Compressor.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9SuperPang_3lib_10Compressor_Compressor.tp_dictoffset && __pyx_type_9SuperPang_3lib_10Compressor_Compressor.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_9SuperPang_3lib_10Compressor_Compressor.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9superpang_3lib_10Compressor_Compressor.tp_dictoffset && __pyx_type_9superpang_3lib_10Compressor_Compressor.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_9superpang_3lib_10Compressor_Compressor.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_9SuperPang_3lib_10Compressor_Compressor.tp_dict, __pyx_vtabptr_9SuperPang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Compressor, (PyObject *)&__pyx_type_9SuperPang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9SuperPang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_ptype_9SuperPang_3lib_10Compressor_Compressor = &__pyx_type_9SuperPang_3lib_10Compressor_Compressor;
+  if (__Pyx_SetVtable(__pyx_type_9superpang_3lib_10Compressor_Compressor.tp_dict, __pyx_vtabptr_9superpang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Compressor, (PyObject *)&__pyx_type_9superpang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9superpang_3lib_10Compressor_Compressor) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_ptype_9superpang_3lib_10Compressor_Compressor = &__pyx_type_9superpang_3lib_10Compressor_Compressor;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
-  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
-  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
-  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
-  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 331, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(1, 331, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 331, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 967, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 967, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 967, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -20530,60 +20624,43 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_36(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20769,28 +20846,28 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_SuperPang__lib__Compressor) {
+  if (__pyx_module_is_main_superpang__lib__Compressor) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "SuperPang.lib.Compressor")) {
-      if (unlikely(PyDict_SetItemString(modules, "SuperPang.lib.Compressor", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "superpang.lib.Compressor")) {
+      if (unlikely(PyDict_SetItemString(modules, "superpang.lib.Compressor", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20803,27 +20880,27 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "SuperPang/lib/Compressor.pyx":7
+  /* "superpang/lib/Compressor.pyx":7
  * 
  * from cpython.array cimport array
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * DTYPE = np.uint8
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "SuperPang/lib/Compressor.pyx":9
+  /* "superpang/lib/Compressor.pyx":9
  * import numpy as np
  * cimport numpy as np
  * DTYPE = np.uint8             # <<<<<<<<<<<<<<
  * ctypedef np.uint8_t DTYPE_t
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
@@ -20835,122 +20912,122 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Compressor(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_9SuperPang_3lib_10Compressor_1__pyx_unpickle_Compressor, NULL, __pyx_n_s_SuperPang_lib_Compressor); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_9superpang_3lib_10Compressor_1__pyx_unpickle_Compressor, NULL, __pyx_n_s_superpang_lib_Compressor); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Compressor, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "SuperPang/lib/Compressor.pyx":1
+  /* "superpang/lib/Compressor.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * #cython: boundscheck=False
  * #cython: wraparound=False
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":209
+  /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 209, __pyx_L1_error)
+  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 209, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_array_type);
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":316
+  /* "View.MemoryView":317
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
  */
   __pyx_memoryview_thread_locks_used = 0;
 
-  /* "View.MemoryView":317
+  /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
   __pyx_t_3[0] = PyThread_allocate_lock();
@@ -20959,37 +21036,37 @@
   __pyx_t_3[3] = PyThread_allocate_lock();
   __pyx_t_3[4] = PyThread_allocate_lock();
   __pyx_t_3[5] = PyThread_allocate_lock();
   __pyx_t_3[6] = PyThread_allocate_lock();
   __pyx_t_3[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_3, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 997, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -21011,19 +21088,19 @@
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init SuperPang.lib.Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init superpang.lib.Compressor", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init SuperPang.lib.Compressor");
+    PyErr_SetString(PyExc_ImportError, "init superpang.lib.Compressor");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -21272,15 +21349,15 @@
 }
 #ifndef Py_NO_RETURN
 #define Py_NO_RETURN
 #endif
 static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
     va_list vargs;
     char msg[200];
-#ifdef HAVE_STDARG_PROTOTYPES
+#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
     va_start(vargs, fmt);
 #else
     va_start(vargs);
 #endif
     vsnprintf(msg, 200, fmt, vargs);
     va_end(vargs);
     Py_FatalError(msg);
@@ -21627,15 +21704,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -22024,28 +22101,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22064,14 +22141,54 @@
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -22454,15 +22571,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -23003,61 +23120,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -23065,15 +23200,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -24323,15 +24458,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -24477,15 +24612,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -24629,15 +24764,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24901,15 +25036,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25097,15 +25232,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `SuperPang-0.9.6/SuperPang/lib/utils.py` & `SuperPang-1.0.0/src/superpang/lib/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from datetime import datetime
 import resource
 
 
-def read_fasta(fasta, ambigs = 'ignore', Ns = 'ignore'):
+def read_fasta(fasta, ambigs = 'ignore', Ns = 'ignore', split_name = True):
     assert Ns in ('ignore', 'split')
     assert ambigs in ('ignore', 'as_Ns')
-    ambig2N = {ord(a): ord('N') for a in ('R', 'Y', 'K', 'M', 'S', 'W', 'B', 'D', 'H', 'V')} # ord bc str.translate wants ascii codes
-    allowedChars = {'A', 'C', 'T', 'G', 'N'}
     seqDict = {}
     for seq in open(fasta).read().strip().lstrip('>').split('>'):
         name, seq = seq.split('\n',1)
+        if split_name:
+            name = name.split(' ')[0]
         seq = seq.upper().replace('\n','').replace('.','').replace('-','').replace('U','A')
         if ambigs == 'as_Ns': # just translate the
-            seq = seq.translate(ambig2N)
-            assert set(seq).issubset(allowedChars)
+            seq = fix_Ns(seq)
         s = 0
         if name in seqDict:
             raise Exception(f'Sequence "{name}" is duplicated in your input file')
         if Ns == 'ignore':
             seqDict[name] = seq
         else:
             if 'N' not in seq:
@@ -27,30 +26,43 @@
                 for seq in seq.split('N'):
                     if seq:
                         seqDict[f'{name}_Nsplit_{i}'] = seq
                         i += 1
     return seqDict
 
 
-def read_fastq(fastq):
+def read_fastq(fastq, ambigs = 'ignore'):
+    assert ambigs in ('ignore', 'as_Ns')
     seqDict = {}
     with open(fastq) as infile:
         while True:
             name = infile.readline().strip().lstrip('@')
             seq = infile.readline().strip()
+            if ambigs == 'as_Ns':
+                seq = fix_Ns(seq)
             sep = infile.readline().strip()
             qual = infile.readline().strip()
             if not name:
                 break
             if name in seqDict:
                 raise Exception(f'Sequence "{name}" is duplicated in your input file')
             seqDict[name] = seq
     return seqDict
 
 
+ambig2N = {ord(a): ord('N') for a in ('R', 'Y', 'K', 'M', 'S', 'W', 'B', 'D', 'H', 'V')} # ord bc str.translate wants ascii codes
+allowedChars = {'A', 'C', 'T', 'G', 'N'}
+def fix_Ns(seq):
+    seq = seq.translate(ambig2N)
+    if not set(seq).issubset(allowedChars):
+        badChars = set(seq) - allowedChars
+        raise ValueError(f'Illegal chars in seq "{name}": {badChars}')
+    return seq
+
+
 def write_fasta(seqDict, fasta):
     with open(fasta, 'w') as outfile:
         for name, seq in seqDict.items():
             outfile.write(f'>{name}\n{seq}\n')
         
 
 
@@ -64,21 +76,20 @@
 def fasta2fastq(fasta, fastq):
     write_fastq(read_fasta(fasta), fastq)
 
 
 def fastq2fasta(fastq, fasta):
     write_fasta(read_fastq(fastq), fasta)
 
+base_for = 'ACGTN'
+base_rev = 'TGCAN'
+comp_tab = str.maketrans(base_for, base_rev)
 
 def reverse_complement(seq):
-    complementarity_matrix = {'A':'T', 'C':'G', 'T':'A', 'G':'C', 'N':'N', 
-                              'W':'W', 'S':'S', 'R':'Y', 'Y':'R', 'M':'K', 
-                              'K':'M', 'B':'V', 'V':'B', 'D':'H', 'H':'D',
-                              '-':'-', '.':'.'}
-    return ''.join([complementarity_matrix[b] for b in seq[::-1]])
+    return seq.translate(comp_tab)[::-1]
 
 
 
 def print_time(msg, end = None):
     dt = datetime.now().strftime('%d/%m/%Y %H:%M:%S')
     mem = round(resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024)
     print(f'{dt}\t{mem}MB\t{msg}', end = end)
```

### Comparing `SuperPang-0.9.6/SuperPang/scripts/SuperPang.py` & `SuperPang-1.0.0/src/superpang/scripts/SuperPang.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 #!/usr/bin/env python3
 
 import sys
 from os.path import dirname, realpath
-from os import mkdir
-path = dirname(realpath(sys.argv[0]))
-sys.path.remove(path)
+from os import mkdir, remove
+from shutil import rmtree, copy
+path = dirname(realpath(__file__))
+if path in sys.path:
+    sys.path.remove(path)
 sys.path.insert(0, realpath(path + '/../..'))
 
 try:
     import graph_tool
 except ModuleNotFoundError:
     print('\nCan\'t import the graph_tool python module! Make sure it\'s available in your environment\n')
     sys.exit(1)
 
 
-from SuperPang.lib.Assembler import Assembler
-from SuperPang.lib.utils import read_fasta, write_fasta, print_time
+from superpang.lib.Assembler import Assembler
+from superpang.lib.utils import read_fasta, write_fasta, print_time
 from mOTUlizer.classes.mOTU import mOTU
 from mOTUlizer.utils import parse_checkm
 
 from uuid import uuid4
 from inspect import getfile
 from hashlib import sha1
 from collections import defaultdict
 from subprocess import call, DEVNULL
+from glob import glob
 from argparse import ArgumentParser
 
 libpath = dirname(realpath(getfile(Assembler)))
 
 with open(libpath + '/../VERSION') as infile:
     VERSION = infile.read().strip()
-CITATION = 'Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson. Exploring intra-species diversity through non-redundant pangenome assemblies. bioRxiv (2022) DOI: 10.1101/2022.03.25.485477'
+CITATION = 'Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. Exploring intra-species diversity through non-redundant pangenome assemblies. Molecular Ecology Resources (2023) DOI: 10.1111/1755-0998.13826'
 
+class ControlledExit(Exception):
+    pass
 
-def main(args):
+
+def main(args, uuid):
 
     ### Welcome message
     print()
     print(f'This is SuperPang version {VERSION}')
     print()
     print('If using in publications or products please cite:')
     print()
     print(CITATION)
     print()
+    if(args.debug):
+        print('Running in debug mode. Execution speed will be slower...')
+        print()
     print()
 
 
     ### File names
-    uuid = uuid4().hex[:7]
-    input_combined       = f'/tmp/{uuid}.combined.fasta'
-    input_minimap2       = f'/tmp/{uuid}.pre.minimap2.fasta'
+    temp_prefix          = f'{args.temp_dir}/{uuid}'
+    corrected_dir        = args.output_dir + '/corrected_input'
+    prelim_dir           = args.output_dir + '/preliminary'
+    temp_saved_dir       = args.output_dir + '/temp'
+    input_combined       = f'{temp_prefix}.combined.fasta'
+    input_minimap2       = f'{temp_prefix}.pre.minimap2.fasta'
+    diskdb               = f'{temp_prefix}.diskdb' if args.lowmem else None
     params               = args.output_dir + '/params.tsv'
-    outputPre_kept       = args.output_dir + '/preliminary/prelim.fasta'
-    outputPre2origs_kept = args.output_dir + '/preliminary/prelim2origins.tsv'
-    name2bin_kept        = args.output_dir + '/preliminary/orig2bin.tsv'
+    outputPre_kept       = prelim_dir      + '/prelim.fasta'
+    outputPre2origs_kept = prelim_dir      + '/prelim2origins.tsv'
+    name2bin_kept        = prelim_dir      + '/orig2bin.tsv'
     outputNodes          = args.output_dir + '/NBPs.fasta'
     outputCore           = args.output_dir + '/NBPs.core.fasta'
     outputAux            = args.output_dir + '/NBPs.accessory.fasta'
     outputNode2origs     = args.output_dir + '/NBP2origins.tsv'
     outputEdges          = args.output_dir + '/graph.fastg'
     outputName           = args.output_dir + '/assembly'
 
@@ -75,37 +88,44 @@
     except OSError as e:
         if e.errno != 17:
             raise
         elif args.force_overwrite:
             pass
         else:
             print(f'\nThe directory {args.output_dir} already contains results. Add --force-overwrite to ignore this message.\n')
-            exit(1)
+            raise ControlledExit
+    try:
+        rmtree(corrected_dir)
+    except:
+        pass
+    try:
+        rmtree(prelim_dir)
+    except:
+        pass
+    try:
+        rmtree(temp_saved_dir)
+    except:
+        pass
     if args.keep_intermediate:
-        try:
-            mkdir(args.output_dir + '/corrected_input')
-        except OSError as e:
-            if e.errno != 17:
-                raise
-        try:
-            mkdir(args.output_dir + '/preliminary')
-        except OSError as e:
-            if e.errno != 17:
-                raise
+        mkdir(corrected_dir)
+        mkdir(prelim_dir)
+    if args.keep_temporary:
+        mkdir(temp_saved_dir)
 
 
     ### Log params
     with open(params, 'w') as outfile:
         outfile.write(f'version\t{VERSION}\n'    )
         outfile.write(f'main_sha1\t{main_sha1}\n')
         outfile.write(f'homo_sha1\t{homo_sha1}\n')
         outfile.write(f'asse_sha1\t{asse_sha1}\n')
         outfile.write(f'cond_sha1\t{cond_sha1}\n')
         for arg in vars(args):
             outfile.write(f'{arg}\t{getattr(args, arg)}\n')
+        outfile.write(f'uuid\t{uuid}\n')
 
 
     ### Load sequences
     name2bin = {}
     seqDict = {}
     genomes = open(args.fasta[0]).read().strip().split('\n') if len(args.fasta) == 1 else args.fasta
     for f in genomes:
@@ -118,63 +138,68 @@
             name2bin[name] = bin_
     write_fasta(seqDict, input_combined)
     if args.keep_intermediate:
         with open(name2bin_kept, 'w') as outfile:
             for name, bin_ in name2bin.items():
                 outfile.write(f'{name}\t{bin_}\n')
 
+
     ### Ensure the checkm file is available and properly formatted, and parse it
     if not args.checkm:
         completeness = {bin_: args.default_completeness for bin_ in set(name2bin.values())}
     elif args.checkm.endswith('.tsv'):
         completeness = {bin_: float(completeness) for bin_, completeness in (line.strip().split('\t') for line in open(args.checkm))}
     else:
         completeness = {bin_: vals['Completeness'] for bin_, vals in parse_checkm(args.checkm).items()}
     missing_bins = set(name2bin.values()) - set(completeness)
     if missing_bins:
         print('\nThe following bins are missing from your CheckM/completeness file:\n')
         for bin_ in missing_bins:
             print(bin_)
         print('\nNote that SuperPang expect bin names in the CheckM/completeness file to NOT contain the file extension\n')
-        sys.exit(1)
+        raise ControlledExit()
 
     
     ### Correct input sequences with minimap2
     correct = args.identity_threshold and args.identity_threshold < 1
     if correct:
         # Check for minimap2
         try:
-            call([args.minimap2_path, '-h'], stdout=DEVNULL, stdin=DEVNULL)
+            call([args.minimap2_path, '-h'], stdout=DEVNULL, stderr=DEVNULL)
         except FileNotFoundError:
             print('\nCan\'t find minimap2. Make sure that it is present in your system and that the --minimap2-path is pointing to the executable\n')
-            sys.exit(1)
+            raise ControlledExit
         # Do stuff
         for i in range(1): # support for multiple calls to homogenize, but apparently it made no big difference
             if i:
                 input_combined = input_minimap2
                 input_minimap2 = f'{input_minimap2}.{i}'
-            
-            ecode = call([path + '/' + 'homogenize.py', '-f', input_combined, '-o', input_minimap2, '-i', str(args.identity_threshold), '-m', str(args.mismatch_size_threshold),
+
+            command = [sys.executable, path + '/' + 'homogenize.py', '-f', input_combined, '-o', input_minimap2, '-i', str(args.identity_threshold), '-m', str(args.mismatch_size_threshold),
                           '-g', str(args.indel_size_threshold), '-r', str(args.correction_repeats), '-n', str(args.correction_repeats_min), '-t', str(args.threads),
-                          '--minimap2-path', args.minimap2_path, '--silent'])
+                          '--minimap2-path', args.minimap2_path, '--silent']
+            if args.debug:
+                command.append('--debug')
+            ecode = call(command)
+
             if ecode:
                 print('\nThere was an error running homogenize.py. Please open an issue\n')
-                sys,exit(1)
+                raise ControlledExit
                 
         if args.keep_intermediate:
-            outfiles = {bin_: open(f'{args.output_dir}/corrected_input/{bin_}.fasta', 'w') for bin_ in set(name2bin.values())}
+            outfiles = {bin_: open(f'{corrected_dir}/{bin_}.fasta', 'w') for bin_ in set(name2bin.values())}
             for name, seq in read_fasta(input_minimap2).items():
                 outfiles[name2bin[name]].write(f'>{name}\n{seq}\n')
             for of in outfiles.values():
                 of.close()
     else:
-        input_minimap2 = input_combined           
+        input_minimap2 = input_combined          
 
     ### Assemble
-    contigs = Assembler(input_minimap2, args.ksize, args.threads).run(args.minlen, args.mincov, args.bubble_identity_threshold, args.genome_assignment_threshold, args.threads)
+    contigs = Assembler(input_minimap2, args.ksize, args.threads, diskdb, args.debug).run(args.minlen, args.mincov, args.bubble_identity_threshold, args.genome_assignment_threshold, args.threads, args.debug)
     if args.keep_intermediate:
         prelim = {}
         with open(outputPre2origs_kept, 'w') as outfile:
             for id_, contig in contigs.items():
                 origs = ','.join(contig.origins)
                 prelimName = f'PRELIM_Sc{contig.scaffold}-{contig.i}_length_{len(contig.seq)}_cov_{round(contig.cov,2)};'
                 outfile.write(f'{prelimName}\t{origs}\n')
@@ -248,23 +273,23 @@
             bins = [name2bin[name] for name in contig.origins]
             lbins = len(set(bins))
             bins  = ','.join(bins)
             outfile.write(f'{nodeNames[id_]}\t{origs}\t{bins}\t{lbins}/{len(completeness)}\n')
 
     ### Condense edges
     print_time('Reconstructing contigs')
-    ecode = call([path + '/' + 'condense-edges.py', outputEdges, outputName, str(args.ksize)])
+    ecode = call([sys.executable, path + '/' + 'condense-edges.py', outputEdges, outputName, str(args.ksize)])
     if ecode:
         print('\nThere was an error running condense-edges.py. Please open an issue\n')
-        sys,exit(1)
+        raise ControlledExit
 
-    ### Cleanup
-    call(['rm', input_combined])
-    if correct:
-        call(['rm', input_minimap2])
+    if args.keep_temporary:
+        for f in glob(f'{temp_prefix}*'):
+            copy(f, temp_saved_dir)
+    
     print_time('Finished')
 
 
 def parse_args():
     parser = ArgumentParser(description='Create a consensus pangenome assembly from a set of bins/genomes from the same mOTU/species')
     parser.add_argument('-f', '--fasta', type = str, nargs='+', required = True,
                         help = 'Input fasta files with the sequences for each bin/genome, or a single file containing the path to one input fasta file per line')
@@ -292,30 +317,48 @@
                         help = 'Fraction of shared kmers required to assign a contig to an input genome')
     parser.add_argument('-x', '--default-completeness', type = float, default = 70,
                         help = 'Default genome completeness to assume if a CheckM output is not provided')
     parser.add_argument('-t', '--threads', type = int, default = 1,
                         help = 'Number of processors to use')
     parser.add_argument('-o', '--output-dir', type = str, default = 'output',
                         help = 'Output directory')
+    parser.add_argument('-d', '--temp-dir', type = str, default = '/tmp/',
+                        help = 'Temp directory')
     parser.add_argument('--assume-complete', action='store_true',
                         help = 'Assume that the input genomes are complete (--genome-assignment-threshold 0.95 --default-completeness 99)')
+    parser.add_argument('--lowmem', action='store_true',
+                        help = 'Use disk storages instead of memory when possible, reduces memory usage at the cost of execution time')
     parser.add_argument('--minimap2-path', type = str, default = 'minimap2',
                         help = 'Path to the minimap2 executable')
     parser.add_argument('--keep-intermediate', action='store_true',
                         help = 'Keep intermediate files')
+    parser.add_argument('--keep-temporary', action='store_true',
+                        help = 'Keep temporary files')
     parser.add_argument('--verbose-mOTUpan', action='store_true',
                         help = 'Print out mOTUpan logs')
     parser.add_argument('--force-overwrite', action='store_true',
                         help='Write results even if the output directory already exists')
+    parser.add_argument('--debug', action='store_true',
+                        help = 'Run additional sanity checks (increases execution time)')
     args = parser.parse_args()
     if args.assume_complete:
         args.checkm = None
         args.genome_assignment_threshold = 0.95
         args.default_completeness = 99
     return args
 
 
-if __name__ == '__main__':
-    main(parse_args())
+def cli():
+    args        = parse_args()
+    uuid        = uuid4().hex[:7]
+    temp_prefix = f'{args.temp_dir}/{uuid}'
+    try:
+        main(args, uuid)
+    except ControlledExit:
+        sys.exit(1)
+    finally:
+        if not args.keep_temporary:
+            call(['rm', '-r'] + glob(f'{temp_prefix}*'), stdout=DEVNULL, stderr=DEVNULL)
 
-    
-    
+ 
+if __name__ == '__main__':
+    cli()
```

### Comparing `SuperPang-0.9.6/SuperPang/scripts/condense-edges.py` & `SuperPang-1.0.0/src/superpang/scripts/condense-edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from os.path import dirname, realpath
 path = dirname(realpath(sys.argv[0]))
 sys.path.remove(path)
 sys.path.insert(0, realpath(path + '/../..'))
 
-from SuperPang.lib.utils import read_fasta, write_fasta
+from superpang.lib.utils import read_fasta, write_fasta
 
 from collections import defaultdict
 
 import graph_tool as gt
 from graph_tool.all import Graph
 
 def main():
```

### Comparing `SuperPang-0.9.6/SuperPang/scripts/homogenize.py` & `SuperPang-1.0.0/src/superpang/scripts/homogenize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 
 import sys
 from os.path import dirname, realpath
-path = dirname(realpath(sys.argv[0]))
-sys.path.remove(path)
+path = dirname(realpath(__file__))
+if path in sys.path:
+    sys.path.remove(path)
 sys.path.insert(0, realpath(path + '/../..'))
 
-from SuperPang.lib.utils import read_fastq, write_fastq, fasta2fastq, fastq2fasta, reverse_complement, print_time
+from superpang.lib.utils import read_fastq, write_fastq, fasta2fastq, fastq2fasta, print_time
+from superpang.lib.cutils import parse_cigar, correct_query, reverse_complement
 
 from argparse import ArgumentParser
 
 from collections import defaultdict
 from subprocess import call, DEVNULL
 import re
 
 
+
 def main(args):
 
     assert args.fasta != args.output
     prefix = args.output.rsplit('.', 1)[0].split('/')[-1]
     current1 = '/tmp/' + prefix + '.current1.fastq'
     current2 = '/tmp/' + prefix + '.current2.fastq'
     fasta2fastq(args.fasta, current1)
@@ -54,19 +57,19 @@
             break
         if rounds == args.correction_repeats:
             break
         prev_tries = current_tries
 
     fastq2fasta(current1, args.output)
 
-
+#@profile
 def iterate(args, rounds, prefix, infastq, outfastq, corrected_previously, correction_tries, identity_threshold, mismatch_size_threshold, indel_size_threshold):
 
     seqOrderOriginal = []
-    seqs = read_fastq(infastq)
+    seqs = read_fastq(infastq, ambigs = 'as_Ns')
     seqOrderOriginal = list(seqs.keys()) # trust that dict remembers insertion order
     sortedSeqs = list(sorted(seqs, key = lambda a: len(seqs[a]), reverse = True))
     lexi = list(sorted((f'{i}' for i in range(len(sortedSeqs))), reverse = True))
     ori2minimap = {name: lexi[i] for i, name in enumerate(sortedSeqs)} # with "--dual=no" minimap2 will skip query-target pairs wherein the query name
     minimap2ori = {mm: name for name, mm in ori2minimap.items()}       #  is lexicographically greater than the target name.
 
     mLen = 0
@@ -139,131 +142,150 @@
                 continue
             if query in corrected_previously and target in corrected_previously[query]:
                 continue
 
             queryLen, queryStart, queryEnd, targetLen, targetStart, targetEnd, matches, alignLen, qual = map(int, [queryLen, queryStart, queryEnd, targetLen, targetStart, targetEnd, matches, alignLen, qual])
                 
             isRC = isRC == '-'
-            cigar = cigar.replace('cg:Z:','')
-            cigar = re.split('(\d+)',cigar)[1:]
-            cigar = [(int(cigar[i]), cigar[i+1]) for i in range(0, len(cigar), 2)]
-            idlen = sum([L for L, op in cigar if op in {'=', 'X'}])
+            cigar = cigar[5:] #ignore leading cg:Z:
 
-            if len(cigar) == 1 and cigar[0][1] == '=':
+            cigLengths, cigOps, idlen, iden = parse_cigar(cigar)
+            if args.debug:
+                cigLengthsPy, cigOpsPy, idlenPy, idenPy = parse_cigar_py(cigar)
+                try:
+                    assert list(cigLengths) == cigLengthsPy
+                    assert list(cigOps) == cigOpsPy
+                    assert idlen == idlenPy
+                    assert round(iden, 2)  == round(idenPy, 2) or abs(1 - iden/idenPy) < 0.01
+                except:
+                    print(list(cigLengths)[1:10], cigLengthsPy[1:10])
+                    print(list(cigOps)[1:10], cigOpsPy[1:10])
+                    print(idlen, idlenPy)
+                    print(sum([L for L, op in zip(cigLengths, cigOps) if op == 61]), sum([L for L, op in zip(cigLengthsPy, cigOpsPy) if op == 61]))
+                    print(round(iden, 6), round(idenPy, 6))
+                    raise
+            
+            if cigLengths.size == 1 and chr(cigOps[0]) == '=':
                 continue # perfect match, ignore
-
-            if sum([L for L, op in cigar if op == '=']) / idlen < identity_threshold:
+            
+            if iden < identity_threshold:
                 continue # too many mismatches, ignore (indels are not counted here)
 
-##            if sum([L for L, op in cigar if op == '=']) / alignLen < identity_threshold:
-##                continue # too mamy mismatches and indels
-
             assert targetLen >= queryLen
 
-            overlaps[target][query].append( ( queryStart, queryEnd, targetStart, targetEnd, cigar, isRC, matches, idlen, alignLen) )
+            overlaps[target][query].append( ( queryStart, queryEnd, targetStart, targetEnd, cigLengths, cigOps, isRC, matches, idlen, alignLen) )
         
         # query is the sequence we want to correct, target is the template
         # before we were using target0 and query0, but the code should work even if we kept using query and target as variable names
         for target in targets:
             if target in corrected_thisround or target in correctedSeqs:
                 continue
             for query, ols in overlaps[target].items():
                 # Check whether we can make this correction
                 if query in correctedSeqs or query in corrected_thisround:
                     continue
                 if query in corrected_previously:
                     assert target not in corrected_previously[query]
 
-                #print(ori2minimap[target], ori2minimap[query], len(ols)) ####################
                 # Ensure that the different regions to correct do not overlap
                 fullCorrection = True
                 ols = sorted(ols, key = lambda x: x[0]) # sort by query start
                 lastEnd = -1
                 goodOls = []
-                for queryStart, queryEnd, targetStart, targetEnd, cigar, isRC, matches, idlen, alignLen in ols:
+                for queryStart, queryEnd, targetStart, targetEnd, cigLengths, cigOps, isRC, matches, idlen, alignLen in ols:
                     if queryStart > lastEnd:
-                        goodOls.append( (queryStart, queryEnd, targetStart, targetEnd, cigar, isRC, matches, idlen, alignLen) )
+                        goodOls.append( (queryStart, queryEnd, targetStart, targetEnd, cigLengths, cigOps, isRC, matches, idlen, alignLen) )
                         lastEnd = queryEnd
                     else:
                         fullCorrection = False
 
                 # Double-check
                 lastEnd = -1
-                for queryStart, queryEnd, targetStart, targetEnd, cigar, isRC, matches, idlen, alignLen in goodOls:
+                for queryStart, queryEnd, targetStart, targetEnd, cigLengths, cigOps, isRC, matches, idlen, alignLen in goodOls:
                     assert queryStart > lastEnd
                     lastEnd = queryEnd
         
                     mLen += matches
                     iLen += idlen
                     oLen += alignLen
 
                 # Correct
                 try:
                     correctedSeq = []
                     lastEnd = 0
-                    for  queryStart, queryEnd, targetStart, targetEnd, cigar, isRC, matches, idlen, alignLen in goodOls:
+                    for  queryStart, queryEnd, targetStart, targetEnd, cigLengths, cigOps, isRC, matches, idlen, alignLen in goodOls:
                         correctedSeq.append(seqs[query][lastEnd:queryStart])
                         correctedSeq.append( correct_query(seqs[query], queryStart, queryEnd, seqs[target], targetStart, targetEnd,
-                                                           cigar = cigar, isRC = isRC, mismatch_size_threshold = mismatch_size_threshold, indel_size_threshold = indel_size_threshold)
+                                                           cigLengths = cigLengths, cigOps = cigOps, isRC = isRC,
+                                                           mismatch_size_threshold = mismatch_size_threshold,
+                                                           indel_size_threshold = indel_size_threshold)
                                            )
+                        if args.debug:
+                            assert correctedSeq[-1] == correct_query_py(seqs[query], queryStart, queryEnd, seqs[target], targetStart, targetEnd,
+                                                                        cigLengths = cigLengths, cigOps = cigOps, isRC = isRC,
+                                                                        mismatch_size_threshold = mismatch_size_threshold,
+                                                                        indel_size_threshold = indel_size_threshold)
                         lastEnd = queryEnd
                     correctedSeq.append( seqs[query][lastEnd:-1] )
 
                     correctedSeqs[query] = ''.join(correctedSeq)
                     if fullCorrection or correction_tries[(query, target)] == 5:
                         # we'll try to achieve full correction in 5 rounds, otherwise we'll consider it as corrected so we can use it as a template
                         corrected_thisround[query] = {target}
                     else:
                         correction_tries[(query, target)] += 1
 
-                except AssertionError: # we failed some assertion in correct_query. I checked a case and it was actually because the alignment/CIGAR string generated by minimap2 was wrong
+                except ValueError: # we failed some assertion in correct_query. I checked a case and it was actually because the alignment/CIGAR string generated by minimap2 was wrong
                     nErrors += 1        # so we just ignore this correction completely
 
 
+
     for header in seqs:
         if header not in correctedSeqs:
             correctedSeqs[header] = seqs[header]
 
     with open(outfastq, 'w') as outfile:
         for header in seqOrderOriginal:
             seq = correctedSeqs[header]
             quals = 'I'*len(seq)
             outfile.write(f'@{header}\n{seq}\n+\n{quals}\n')
 
     print_time(' '*40, end = '\r')
-    
+ 
     return mLen, iLen, oLen, corrected_thisround, nErrors
 
 
-
-def switch_cigar(cigar): # unused
-    newCigar = []
-    for L, op in cigar:
-        if op == 'D':
-            op = 'I'
-        elif op == 'I':
-            op = 'D'
-        newCigar.append( (L, op) )
-    return newCigar
+def parse_cigar_py(cigar):
+    cigar   = re.split('(\d+)',cigar)[1:]
+    Larray  = [int(cigar[i])   for i in range(0, len(cigar), 2)]
+    oparray = [ord(cigar[i+1]) for i in range(0, len(cigar), 2)]
+    mlen    = sum([L for L, op in zip(Larray, oparray) if op == 61]) # '='
+    idlen   = sum([L for L, op in zip(Larray, oparray) if op == 61 or op == 88]) # '=' or 'X'
+    iden    = mlen/idlen if idlen else 0
+    return Larray, oparray, idlen, iden
 
 
-def correct_query(query, queryStart, queryEnd, target, targetStart, targetEnd, cigar, isRC = False, mismatch_size_threshold = 10, indel_size_threshold = 100):
+#@profile
+def correct_query_py(query, queryStart, queryEnd, target, targetStart, targetEnd, cigLengths, cigOps, isRC = False, mismatch_size_threshold = 10, indel_size_threshold = 100):
     ops = {'=', 'X', 'I', 'D'}
+    ngOps = {'=', 'X'}
     query = query if not isRC else reverse_complement(query)
     queryPos = queryStart if not isRC else len(query) - queryEnd
     targetPos = targetStart
     correction = []
         
-    for i, (L, op) in enumerate(cigar):
-        assert op in ops
-        if op == '=' or op == 'X':
+    for i, (L, op) in enumerate(zip(cigLengths, cigOps)):
+        op = chr(op)
+##        assert op in ops
+        if op in ngOps: #op == '=' or op == 'X':
             queryFrag = query[queryPos:queryPos+L]
             newFrag = target[targetPos:targetPos+L]
             if op == '=':
-                assert newFrag == queryFrag
+                if newFrag != queryFrag:
+                    raise ValueError
 ##                try:
 ##                    assert newFrag == queryFrag
 ##                except:
 ##                    print('ERROR!')
 ##                    print(i, L, op, isRC)
 ##                    print('>NEWFRAG')
 ##                    print(newFrag)
@@ -320,13 +342,19 @@
                         help = 'Output name')
     parser.add_argument('-t', '--threads', type = int, default = 1,
                         help = 'Number of processors to use')
     parser.add_argument('--minimap2-path', type = str, default = 'minimap2',
                         help = 'Path to the minimap2 executable')
     parser.add_argument('--silent', action = 'store_true',
                         help = 'Ignore stderr from minimus2')
+    parser.add_argument('--debug', action = 'store_true',
+                        help = 'Run additional sanity checks (increases execution time)') 
 
     return parser.parse_args()
 
-                
-if __name__ == '__main__':
+
+def cli():
     main(parse_args())
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `SuperPang-0.9.6/SuperPang/scripts/test-SuperPang.py` & `SuperPang-1.0.0/src/superpang/scripts/test-SuperPang.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 #!/usr/bin/env python3
 
 MINIMAP2_PATH = 'minimap2'
 
 import sys
 from os.path import dirname, realpath
 from os import mkdir
-path = dirname(realpath(sys.argv[0]))
-sys.path.remove(path)
+path = dirname(realpath(__file__))
+if path in sys.path:
+    sys.path.remove(path)
 sys.path.insert(0, realpath(path + '/../..'))
 superpath = path + '/' + 'SuperPang.py'
 
-import SuperPang
+import superpang
 from inspect import getfile
-data_path = getfile(SuperPang)
+data_path = getfile(superpang)
 output_path = '/tmp/SuperPang_test_output'
 datapath = dirname(realpath(data_path)) + '/' + 'test_data'
 
 from subprocess import call
 from glob import glob
 
-print(f'\nAssuming that minimap2 can be found in the following path "{MINIMAP2_PATH}". Otherwise edit the MINIMAP2_PATH variable in this script\n')
+def main():
+    print(f'\nAssuming that minimap2 can be found in the following path "{MINIMAP2_PATH}". Otherwise edit the MINIMAP2_PATH variable in this script\n')
 
-ecode = call([superpath,'-f'] + glob(f'{datapath}/*fna') + ['--assume-complete', '-t', '12', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH, '--keep-intermediate'])
+    if len(sys.argv) > 1 and sys.argv[1] == 'fast':
+        files = [f'{datapath}/2636415981.fna', f'{datapath}/2636416036.fna']
+        iden = '-i1'
+    elif len(sys.argv) > 1 and sys.argv[1] == 'fasth':
+        files = [f'{datapath}/2636415981.fna', f'{datapath}/2636416036.fna']
+        iden = '-i0.95'
+    else:
+       files = glob(f'{datapath}/*fna')
+       iden = '-i0.95'
+
+    args = [sys.executable, superpath,'-f'] + files + ['--assume-complete',
+            iden, '-t12', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH,
+            '--keep-temporary', '--keep-intermediate', '--debug']
+    argss = ' '.join(args)
+    print(f'Running SuperPang with command "{argss}"')
+    ecode = call(args)
 
-if not ecode:
-    print(f'\n\nAll went well, I hope! Test results should be present in {output_path}\n')
+    if not ecode:
+        print(f'\n\nAll went well, I hope! Test results should be present in {output_path}\n')
 
+
+if __name__ == '__main__':
+    main()
```

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2636415981.fna` & `SuperPang-1.0.0/src/superpang/test_data/2636415981.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2636416036.fna` & `SuperPang-1.0.0/src/superpang/test_data/2636416036.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2636416061.fna` & `SuperPang-1.0.0/src/superpang/test_data/2636416061.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2636416062.fna` & `SuperPang-1.0.0/src/superpang/test_data/2636416062.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2639762512.fna` & `SuperPang-1.0.0/src/superpang/test_data/2639762512.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2639762514.fna` & `SuperPang-1.0.0/src/superpang/test_data/2639762514.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2639762515.fna` & `SuperPang-1.0.0/src/superpang/test_data/2639762515.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2639762516.fna` & `SuperPang-1.0.0/src/superpang/test_data/2639762516.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang/test_data/2844342787.fna` & `SuperPang-1.0.0/src/superpang/test_data/2844342787.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-0.9.6/SuperPang.egg-info/PKG-INFO` & `SuperPang-1.0.0/src/SuperPang.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,61 @@
 Metadata-Version: 2.1
 Name: SuperPang
-Version: 0.9.6
+Version: 1.0.0
 Summary: Non-redundant pangenome assemblies from multiple genomes or bins
-Home-page: https://github.com/fpusan/SuperPang
-Author: Fernando Puente-Sánchez
-Author-email: fernando.puente.sanchez@slu.se
-License: BSD
-Keywords: bioinformatics assembly metagenomics microbial-genomics genomics
+Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2021, Fernando Puente-Sánchez
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/fpusan/SuperPang
+Project-URL: Bug Tracker, https://github.com/fpusan/SuperPang/issues
+Keywords: bioinformatics,assembly,metagenomics,microbial-genomics,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SuperPang: non-redundant pangenome assemblies from multiple genomes or bins
 
-**Check our preprint:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://www.biorxiv.org/content/10.1101/2022.03.25.485477v1.full) _bioRxiv_ (2022) DOI: 10.1101/2022.03.25.485477
+**Check our paper:** Puente-Sánchez F, Hoetzinger M, Buck M and Bertilsson S. [Exploring intra-species diversity through non-redundant pangenome assemblies](https://onlinelibrary.wiley.com/doi/full/10.1111/1755-0998.13826) _Molecular Ecology Resources_ (2023) DOI: 10.1111/1755-0998.13826
+_... but note that performance is now better (3x less memory usage, 20% faster execution time) than when we first benchmarked Superpang.
 
 ## Installation
-Requires [graph-tool](https://graph-tool.skewed.de/), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
+Requires [graph-tool](https://graph-tool.skewed.de/), [speedict](https://github.com/Congyuwang/RocksDict), [mOTUlizer v0.2.4](https://github.com/moritzbuck/mOTUlizer), [minimap2](https://github.com/lh3/minimap2) and [mappy](https://pypi.org/project/mappy/). The easiest way to get it running is using conda.
 ```
 # Install into a new conda environment
 conda create -n SuperPang -c conda-forge -c bioconda -c fpusan superpang
 # Check that it works for you!
 conda activate SuperPang
 test-SuperPang.py
 ```
@@ -53,24 +83,28 @@
 * *-l/--minlen*: Scaffold length cutoff. Default `0` (no cutoff).
 * *-c/--mincov*: Scaffold coverage cutoff. Default `0` (no cutoff).
 * *-b/--bubble-identity-threshold*: Minimum identity (matches / length) required to remove a bubble in the sequence graph. Default `0.95`.
 * *-a/--genome-assignment-threshold*. Fraction of shared kmers required to assign a contig to an input genome (0 means a single shared kmer is enough). Default `0.5`.
 * *-x/--default-completeness*: Default genome completeness to assume if a CheckM output is not provided with *--checkm*. Default `70`.
 * *-t/--threads*: Number of processors to use. Default `1`.
 * *-o/--output*: Output directory. Default `output`.
+* *-d/--temp-dir*: Directory for temp files. Default `tmp`.
 * *--assume-complete*: Assume that the input genomes are complete (*--genome-assignment-threshold 0.95*, *--default-completeness 99*).
+* *--lowmem*: Use disk storages instead of memory when possible, reduces memory usage at the cost of execution time.
 * *--minimap2-path*: Path to the minimap2 executable. Default `minimap2`.
 * *--keep-intermediate*: Keep intermediate files.
+* *--keep-temporary*: Keep temporary files.
 * *--verbose-mOTUpan*: Print out mOTUpan logs.
+* *--debug*: Run additional sanity checks (increases execution time).
 
 ## Output
 * `assembly.fasta`: contigs.
 * `assembly.info`: core/auxiliary and path information for each contig.
 * `NBPs.fasta`: non-branching paths.
 * `NBPs.core.fasta`: non-branching paths deemed to belong to the core genome of the species by [mOTUpan](https://www.biorxiv.org/content/10.1101/2021.06.25.449606v1).
 * `NBPs.accessory.fasta`: non-branching paths deemed to belong to the accessory genome of the species.
 * `graph.fastg`: assembly graph in a format compatible with [bandage](https://rrwick.github.io/Bandage/).
 * `NBP2origins.tsv`: tab-separated file with the non-branching path IDs, a comma-separated list of the input sequences in which that NBP was deemed present, a comma-separated list of the input genomes in which that NBP was deemed present, and the number of input genomes in which that NBP was deemed present.
 * `params.tsv`: parameters used in the run.
 
 ## About
-*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantsbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
+*SuperPang* is developed by Fernando Puente-Sánchez (Sveriges lantbruksuniversitet). Feel free to open an issue or reach out for support [fernando.puente.sanchez@slu.se](mailto:fernando.puente.sanchez@slu.se).
```

