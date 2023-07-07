# Comparing `tmp/loreme-0.1.7.tar.gz` & `tmp/loreme-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.7.tar", last modified: Fri Jul  7 01:29:47 2023, max compression
+gzip compressed data, was "loreme-0.1.8.tar", last modified: Fri Jul  7 02:06:05 2023, max compression
```

## Comparing `loreme-0.1.7.tar` & `loreme-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.795215 loreme-0.1.7/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.7/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 01:29:47.794772 loreme-0.1.7/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.7/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.776263 loreme-0.1.7/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-06 22:23:39.000000 loreme-0.1.7/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-07 01:29:47.795323 loreme-0.1.7/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.767820 loreme-0.1.7/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.794245 loreme-0.1.7/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.7/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.7/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.7/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37399 2023-07-06 23:58:13.000000 loreme-0.1.7/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.7/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.7/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2507 2023-07-07 01:20:59.000000 loreme-0.1.7/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-06 22:23:47.000000 loreme-0.1.7/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.551694 loreme-0.1.8/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.8/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 02:06:05.551141 loreme-0.1.8/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.8/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.525699 loreme-0.1.8/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-07 01:45:52.000000 loreme-0.1.8/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-07 02:06:05.551855 loreme-0.1.8/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.518293 loreme-0.1.8/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.550028 loreme-0.1.8/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.8/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.8/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.8/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37399 2023-07-06 23:58:13.000000 loreme-0.1.8/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.8/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.8/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2563 2023-07-07 02:04:48.000000 loreme-0.1.8/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-07 01:45:55.000000 loreme-0.1.8/src/loreme/version.py
```

### Comparing `loreme-0.1.7/LICENSE` & `loreme-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/PKG-INFO` & `loreme-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.7
+Version: 0.1.8
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.7/README.md` & `loreme-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/loreme.egg-info/PKG-INFO` & `loreme-0.1.8/loreme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.7
+Version: 0.1.8
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.7/loreme.egg-info/SOURCES.txt` & `loreme-0.1.8/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/__init__.py` & `loreme-0.1.8/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/check_gpu_availability.py` & `loreme-0.1.8/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/dorado.py` & `loreme-0.1.8/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/download.py` & `loreme-0.1.8/src/loreme/download.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/env.py` & `loreme-0.1.8/src/loreme/env.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/export_bedgraph.py` & `loreme-0.1.8/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/gene_body_methylation.py` & `loreme-0.1.8/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/intersect.py` & `loreme-0.1.8/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/loreme.py` & `loreme-0.1.8/src/loreme/loreme.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/mean.py` & `loreme-0.1.8/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/merge.py` & `loreme-0.1.8/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/methylation_hist.py` & `loreme-0.1.8/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/parse_gff.py` & `loreme-0.1.8/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/pbcpg.py` & `loreme-0.1.8/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/plot.py` & `loreme-0.1.8/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/plot_bedtools.py` & `loreme-0.1.8/src/loreme/plot_bedtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     chromosomes
         iterable of chromosomes to include in results, or None to include
         all chromosomes
 
     Yield
     -----
     tuple
+        
     """
 
     if chromosomes is not None:
         chromosomes = set(chromosomes)
     for i in bedtool:
         n_fields = len(i.fields)
         if n_fields == 16:
@@ -48,21 +49,26 @@
     scale : float
         ratio of chromosome size to mean chromosome size
     shift : float
         x-axis shift of this chromosome, for plots showing multiple chromosomes
         consecutively
     smooth : bool
         if True, draw a smoother plot
+
+    Yield
+    -----
+    tuple
+        
     """
 
     for bt, g in zip(bedtools, groups):
         for i in bt:
             n_fields = len(i.fields)
             if n_fields == 16:
-                _, _, _, _, _, _, _, _, _, meth_col, _, start, end, strand, _, _ = i.fields
+                _, _, pos, _, _, _, _, _, _, meth_col, _, start, end, strand, index, group = i.fields
                 meth = meth_col.split()[1]
             elif n_fields == 15:
-                _, _, pos, meth, _, _, _, _, _, _, start, end, strand, index, _, group = i.fields+[g]
+                _, _, pos, meth, _, _, _, _, _, _, start, end, strand, index, group = i.fields+[g]
             else:
                 raise RuntimeError('Invalid methylation BED file')
             yield (round((int(pos)-int(start) if strand == '+' else int(end)-int(pos))
          / (int(end)-int(start)), 2-smooth)*scale + shift, float(meth), group, index)
```

### Comparing `loreme-0.1.7/src/loreme/plot_genes.py` & `loreme-0.1.8/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/plot_repeats.py` & `loreme-0.1.8/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.7/src/loreme/promoter_methylation.py` & `loreme-0.1.8/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

