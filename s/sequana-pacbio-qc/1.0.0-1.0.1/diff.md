# Comparing `tmp/sequana_pacbio_qc-1.0.0.tar.gz` & `tmp/sequana_pacbio_qc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_pacbio_qc-1.0.0.tar", last modified: Mon May 22 15:58:04 2023, max compression
+gzip compressed data, was "dist/sequana_pacbio_qc-1.0.1.tar", last modified: Fri Jul  7 13:13:08 2023, max compression
```

## Comparing `sequana_pacbio_qc-1.0.0.tar` & `sequana_pacbio_qc-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4693 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 15:58:03.000000 sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    17653 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/dag.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     4787 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5333 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14043 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      968 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-22 15:58:04.000000 sequana_pacbio_qc-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2772 2023-05-22 15:57:58.000000 sequana_pacbio_qc-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7086 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4738 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7086 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    17653 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/dag.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4787 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5333 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14063 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/pacbio_qc.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-07 13:13:08.000000 sequana_pacbio_qc-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2772 2023-07-07 13:13:01.000000 sequana_pacbio_qc-1.0.1/setup.py
```

### Comparing `sequana_pacbio_qc-1.0.0/PKG-INFO` & `sequana_pacbio_qc-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_pacbio_qc
-Version: 1.0.0
+Version: 1.0.1
 Summary: QC on various type of pacbio data
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -108,14 +108,15 @@
         
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.1     fix missing import in the summary 
         1.0.0     Uses latest wrappers and graphviz apptainers
         0.11.0    Release to use latests sequana_pipetools framework
         0.10.0    Update to use latest tools from sequana framework
         0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
                   modules (0.9.5)
         ========= ====================================================================
```

### Comparing `sequana_pacbio_qc-1.0.0/README.rst` & `sequana_pacbio_qc-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 
 Changelog
 ~~~~~~~~~
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.0.1     fix missing import in the summary 
 1.0.0     Uses latest wrappers and graphviz apptainers
 0.11.0    Release to use latests sequana_pipetools framework
 0.10.0    Update to use latest tools from sequana framework
 0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
           modules (0.9.5)
 ========= ====================================================================
```

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/PKG-INFO` & `sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-pacbio-qc
-Version: 1.0.0
+Version: 1.0.1
 Summary: QC on various type of pacbio data
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -108,14 +108,15 @@
         
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.1     fix missing import in the summary 
         1.0.0     Uses latest wrappers and graphviz apptainers
         0.11.0    Release to use latests sequana_pipetools framework
         0.10.0    Update to use latest tools from sequana framework
         0.9.0     First release of sequana_pacbio_qc using latest sequana rules and
                   modules (0.9.5)
         ========= ====================================================================
```

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pacbio_qc.egg-info/SOURCES.txt` & `sequana_pacbio_qc-1.0.1/sequana_pacbio_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/config.yaml` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/dag.png` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/main.py` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/main.py`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/multiqc_config.yaml` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/pacbio_qc.rules` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/pacbio_qc.rules`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         read_len   = "{sample}/images/hist_read_len_{sample}.png",
         GC_content = "{sample}/images/GC_content_{sample}.png",
         ZMW        = "{sample}/images/ZMW_passes_{sample}.png",
         SNR        = "{sample}/images/SNR_{sample}.png",
         GC_vs_len  = "{sample}/images/GC_vs_len_{sample}.png",
         summary    = "{sample}/sequana_summary_pacbio_qc_{sample}.json"
     run:
+        import json
         from sequana import pacbio
         import pylab
         def setname(name):
             return name
         ########## labels for plots
         short_name = input[0].replace(".bam","").split("/")[-1]
         bam_pacbio = pacbio.PacbioSubreads(input[0])
```

### Comparing `sequana_pacbio_qc-1.0.0/sequana_pipelines/pacbio_qc/schema.yaml` & `sequana_pacbio_qc-1.0.1/sequana_pipelines/pacbio_qc/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pacbio_qc-1.0.0/setup.py` & `sequana_pacbio_qc-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 _MAJOR               = 1
 _MINOR               = 0
-_MICRO               = 0
+_MICRO               = 1
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
```

