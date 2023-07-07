# Comparing `tmp/loreme-0.1.6.tar.gz` & `tmp/loreme-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.6.tar", last modified: Mon Jul  3 21:34:03 2023, max compression
+gzip compressed data, was "loreme-0.1.7.tar", last modified: Fri Jul  7 01:29:47 2023, max compression
```

## Comparing `loreme-0.1.6.tar` & `loreme-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.979321 loreme-0.1.6/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.6/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-03 21:34:03.976913 loreme-0.1.6/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.6/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.938737 loreme-0.1.6/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-03 21:32:31.000000 loreme-0.1.6/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-03 21:34:03.979622 loreme-0.1.6/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.927199 loreme-0.1.6/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.975839 loreme-0.1.6/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.6/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.6/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.6/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37390 2023-06-26 22:03:44.000000 loreme-0.1.6/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.6/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.6/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2483 2023-06-14 05:33:30.000000 loreme-0.1.6/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-03 21:32:29.000000 loreme-0.1.6/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.795215 loreme-0.1.7/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.7/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 01:29:47.794772 loreme-0.1.7/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.7/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.776263 loreme-0.1.7/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-07 01:29:47.000000 loreme-0.1.7/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-06 22:23:39.000000 loreme-0.1.7/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-07 01:29:47.795323 loreme-0.1.7/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.767820 loreme-0.1.7/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 01:29:47.794245 loreme-0.1.7/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.7/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.7/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.7/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37399 2023-07-06 23:58:13.000000 loreme-0.1.7/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.7/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.7/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2507 2023-07-07 01:20:59.000000 loreme-0.1.7/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.7/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-06 22:23:47.000000 loreme-0.1.7/src/loreme/version.py
```

### Comparing `loreme-0.1.6/LICENSE` & `loreme-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/PKG-INFO` & `loreme-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.6
+Version: 0.1.7
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.6/README.md` & `loreme-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/loreme.egg-info/PKG-INFO` & `loreme-0.1.7/loreme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.6
+Version: 0.1.7
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.6/loreme.egg-info/SOURCES.txt` & `loreme-0.1.7/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/pyproject.toml` & `loreme-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.6" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.7" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.6/src/loreme/__init__.py` & `loreme-0.1.7/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/check_gpu_availability.py` & `loreme-0.1.7/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/dorado.py` & `loreme-0.1.7/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/download.py` & `loreme-0.1.7/src/loreme/download.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/env.py` & `loreme-0.1.7/src/loreme/env.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/export_bedgraph.py` & `loreme-0.1.7/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/gene_body_methylation.py` & `loreme-0.1.7/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/intersect.py` & `loreme-0.1.7/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/loreme.py` & `loreme-0.1.7/src/loreme/loreme.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
     parser_promoter.add_argument('--chromosomes', metavar='<X>', nargs='+',
         help='chromosomes to include')
     parser_promoter.add_argument('--cytosines', action='store_true',
         help='output a column with number of cytosines in each promoter')
     parser_promoter.add_argument('--coverage', action='store_true',
         help='output a column of coverage for each promoter')
     parser_promoter.add_argument('--min-coverage', metavar='<int>',
-        type=int, default=1, help='minimum coverage to include promoter [1)')
+        type=int, default=1, help='minimum coverage to include promoter (default: 1)')
     parser_promoter.add_argument('--bins', action='store_true',
         help='output a column binning promoters by discrete methylation level')
     parser_promoter.add_argument('--levels', metavar='<Level>',
         nargs='+', default=['Min', 'Low', 'Mid', 'High', 'Max'],
         help='discrete methylation levels')
     parser_promoter.add_argument('--hist', metavar='<file.{pdf,png,svg}>',
         help='generate histogram of methylation levels')
```

### Comparing `loreme-0.1.6/src/loreme/mean.py` & `loreme-0.1.7/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/merge.py` & `loreme-0.1.7/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/methylation_hist.py` & `loreme-0.1.7/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/parse_gff.py` & `loreme-0.1.7/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/pbcpg.py` & `loreme-0.1.7/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/plot.py` & `loreme-0.1.7/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/plot_bedtools.py` & `loreme-0.1.7/src/loreme/plot_bedtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
 
     if chromosomes is not None:
         chromosomes = set(chromosomes)
     for i in bedtool:
         n_fields = len(i.fields)
         if n_fields == 16:
-            chrom, _, _, _, _, _, _, _, _, coverage, meth_col, _, start, end, strand, gene, _ = i.fields
+            chrom, _, _, _, coverage, _, _, _, _, meth_col, _, start, end, strand, gene, _ = i.fields
             meth = meth_col.split()[1]
         elif n_fields == 15:
             chrom, _, _, meth, _, coverage, _, _, _, _, start, end, strand, gene, _ = i.fields
         else:
             raise RuntimeError('Invalid methylation BED file')
         if (chromosomes is None) or (chrom in chromosomes):
             yield chrom, int(start), int(end), gene, strand, 1, int(coverage), float(meth)
@@ -53,15 +53,16 @@
     smooth : bool
         if True, draw a smoother plot
     """
 
     for bt, g in zip(bedtools, groups):
         for i in bt:
             n_fields = len(i.fields)
-            if n_fields == 17:
-                _, _, pos, _, _, _, _, _, _, _, meth, _, start, end, strand, index, _, group = i.fields+[g]
+            if n_fields == 16:
+                _, _, _, _, _, _, _, _, _, meth_col, _, start, end, strand, _, _ = i.fields
+                meth = meth_col.split()[1]
             elif n_fields == 15:
                 _, _, pos, meth, _, _, _, _, _, _, start, end, strand, index, _, group = i.fields+[g]
             else:
                 raise RuntimeError('Invalid methylation BED file')
             yield (round((int(pos)-int(start) if strand == '+' else int(end)-int(pos))
          / (int(end)-int(start)), 2-smooth)*scale + shift, float(meth), group, index)
```

### Comparing `loreme-0.1.6/src/loreme/plot_genes.py` & `loreme-0.1.7/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/plot_repeats.py` & `loreme-0.1.7/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.6/src/loreme/promoter_methylation.py` & `loreme-0.1.7/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

