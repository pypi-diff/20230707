# Comparing `tmp/sequana_variant_calling-1.0.0.tar.gz` & `tmp/sequana_variant_calling-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_variant_calling-1.0.0.tar", last modified: Wed May 24 07:44:23 2023, max compression
+gzip compressed data, was "dist/sequana_variant_calling-1.0.1.tar", last modified: Fri Jul  7 11:41:43 2023, max compression
```

## Comparing `sequana_variant_calling-1.0.0.tar` & `sequana_variant_calling-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6926 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    90725 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/dag.png
--rw-r--r--   0 runner    (1001) docker     (122)     5336 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     5543 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/multiqc_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    19086 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/variant_calling.rules
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-24 07:44:23.000000 sequana_variant_calling-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-24 07:44:16.000000 sequana_variant_calling-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9766 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7078 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    90725 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5336 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5951 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    19168 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/variant_calling.rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9766 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-07 11:41:43.000000 sequana_variant_calling-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-07 11:41:39.000000 sequana_variant_calling-1.0.1/setup.py
```

### Comparing `sequana_variant_calling-1.0.0/PKG-INFO` & `sequana_variant_calling-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_variant_calling
-Version: 1.0.0
+Version: 1.0.1
 Summary: A variant calling pipeline to analyse sequencing Illumina data
 Home-page: http://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -136,14 +136,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ======================================================================
         Version   Description
         ========= ======================================================================
+        1.0.1     * automatically fill the bwa index algorithm and fix bwa_index rule to 
+                    use the options in the config file (not the harcoded one)
         1.0.0     * use last warppers and graphviz apptainer
         0.12.0    * set all apptainers containers and add vcf to bcf conversions
                   * Update rule sambamba to use latest wrappers
         0.11.0    * Add singularity containers
         0.10.0    * fully integrated sequana wrappers and simplification of HTML reports
         0.9.10    * Uses new sequana_pipetools and wrappers
         0.9.5     * fix typo in the onsuccess and update sequana requirements to use
```

### Comparing `sequana_variant_calling-1.0.0/README.rst` & `sequana_variant_calling-1.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,16 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ======================================================================
 Version   Description
 ========= ======================================================================
+1.0.1     * automatically fill the bwa index algorithm and fix bwa_index rule to 
+            use the options in the config file (not the harcoded one)
 1.0.0     * use last warppers and graphviz apptainer
 0.12.0    * set all apptainers containers and add vcf to bcf conversions
           * Update rule sambamba to use latest wrappers
 0.11.0    * Add singularity containers
 0.10.0    * fully integrated sequana wrappers and simplification of HTML reports
 0.9.10    * Uses new sequana_pipetools and wrappers
 0.9.5     * fix typo in the onsuccess and update sequana requirements to use
```

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/config.yaml` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/dag.png` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/logo.png` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/main.py` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,19 +59,19 @@
         pipeline_group.add_argument(
             "--annotation-file",
             dest="annotation",
             default=None,
             help="The annotation for snpeff"
         )
         pipeline_group.add_argument("--threads", dest="threads", default=4, type=int)
-        pipeline_group.add_argument("--do-coverage", dest="do_coverage", 
-            action="store_true", 
+        pipeline_group.add_argument("--do-coverage", dest="do_coverage",
+            action="store_true",
             help="perform the coverage analysis using sequana_coverage")
-        pipeline_group.add_argument("--do-joint-calling", dest="do_joint_calling", 
-            action="store_true", 
+        pipeline_group.add_argument("--do-joint-calling", dest="do_joint_calling",
+            action="store_true",
             help="do the joint calling analysise")
 
         pipeline_group.add_argument("-o", "--circular", action="store_true")
         pipeline_group.add_argument("--freebayes-ploidy", type=int, default=1)
 
         pipeline_group.add_argument("--create-bigwig", action="store_true",
             help="create the bigwig files from the BAM files" )
@@ -132,20 +132,32 @@
             cfg.snpeff.do = False
             cfg['sequana_coverage']['genbank_file'] = ""
 
         cfg['sequana_coverage']['do'] = options.do_coverage
         cfg['sequana_coverage']["circular"] = options.circular
         cfg['joint_freebayes']['do'] = options.do_joint_calling
         cfg['bwa_mem']['threads'] = options.threads
+
+
         cfg['freebayes']['ploidy'] = options.freebayes_ploidy
 
         cfg.reference_file = os.path.abspath(options.reference)
         manager.exists(cfg.reference_file)
 
-        # coverage
+        # Given the reference, let us compute its length and st the index algorithm
+        from sequana import FastA
+        f = FastA(options.reference)
+        N = f.get_stats()['total_length']
+
+        # seems to be a hardcoded values in bwa according to the documentation
+        if N >= 2000000000:
+            cfg['bwa_mem']['index_algorithm'] = "bwtsw"
+        else:
+            cfg['bwa_mem']['index_algorithm'] = "is"
+
 
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
     if options.run:
```

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/multiqc_config.yaml` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/schema.yaml` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/sequana_pipelines/variant_calling/variant_calling.rules` & `sequana_variant_calling-1.0.1/sequana_pipelines/variant_calling/variant_calling.rules`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
             reference=new_reference
         output:
             bwa_bwt=new_reference + ".bwt",
             fai=new_reference + ".fai"
         log:
             "reference/build.log"
         params:
-            options="",
-            index_algorithm="is"
+            options=config['bwa_mem'].get('index_options', ""),
+            index_algorithm=config['bwa_mem'].get('index_algorithm', "is")
         container:
             config['apptainers']['sequana_tools']
         threads: 2
         wrapper:
             f"{sequana_wrapper_branch}/wrappers/bwa/build"
 
     # ========================================================= bwa mapping
```

### Comparing `sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/PKG-INFO` & `sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-variant-calling
-Version: 1.0.0
+Version: 1.0.1
 Summary: A variant calling pipeline to analyse sequencing Illumina data
 Home-page: http://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -136,14 +136,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ======================================================================
         Version   Description
         ========= ======================================================================
+        1.0.1     * automatically fill the bwa index algorithm and fix bwa_index rule to 
+                    use the options in the config file (not the harcoded one)
         1.0.0     * use last warppers and graphviz apptainer
         0.12.0    * set all apptainers containers and add vcf to bcf conversions
                   * Update rule sambamba to use latest wrappers
         0.11.0    * Add singularity containers
         0.10.0    * fully integrated sequana wrappers and simplification of HTML reports
         0.9.10    * Uses new sequana_pipetools and wrappers
         0.9.5     * fix typo in the onsuccess and update sequana requirements to use
```

### Comparing `sequana_variant_calling-1.0.0/sequana_variant_calling.egg-info/SOURCES.txt` & `sequana_variant_calling-1.0.1/sequana_variant_calling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_variant_calling-1.0.0/setup.py` & `sequana_variant_calling-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
 _MAJOR               = 1
 _MINOR               = 0
-_MICRO               = 0
+_MICRO               = 1
 
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
```

