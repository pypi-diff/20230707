# Comparing `tmp/hdict-0.230412.3.tar.gz` & `tmp/hdict-1.230706.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdict-0.230412.3.tar", max compression
+gzip compressed data, was "hdict-1.230706.1.tar", max compression
```

## Comparing `hdict-0.230412.3.tar` & `hdict-1.230706.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-0.230412.3/LICENSE
--rw-r--r--   0        0        0     7698 2023-04-12 21:37:38.769733 hdict-0.230412.3/README.md
--rw-r--r--   0        0        0     1369 2023-04-12 21:37:42.425790 hdict-0.230412.3/pyproject.toml
--rw-r--r--   0        0        0    15593 2023-04-10 02:17:58.720650 hdict-0.230412.3/src/hdict/__init__.py
--rw-r--r--   0        0        0      223 2023-04-08 04:05:25.273250 hdict-0.230412.3/src/hdict/abs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230412.3/src/hdict/content/__init__.py
--rw-r--r--   0        0        0      755 2023-04-08 19:59:38.981761 hdict-0.230412.3/src/hdict/content/argument/__init__.py
--rw-r--r--   0        0        0    13865 2023-04-12 20:17:41.450684 hdict-0.230412.3/src/hdict/content/argument/apply.py
--rw-r--r--   0        0        0     3121 2023-04-09 21:56:47.979809 hdict-0.230412.3/src/hdict/content/argument/aux_apply.py
--rw-r--r--   0        0        0     1483 2023-04-10 01:15:22.584449 hdict-0.230412.3/src/hdict/content/argument/default.py
--rw-r--r--   0        0        0     1318 2023-04-08 19:30:32.031213 hdict-0.230412.3/src/hdict/content/argument/entry.py
--rw-r--r--   0        0        0     2162 2023-04-08 04:05:25.273250 hdict-0.230412.3/src/hdict/content/argument/field.py
--rw-r--r--   0        0        0     2328 2023-04-08 04:05:25.273250 hdict-0.230412.3/src/hdict/content/argument/sample.py
--rw-r--r--   0        0        0     3855 2023-01-29 20:20:35.027416 hdict-0.230412.3/src/hdict/content/aux_value.py
--rw-r--r--   0        0        0     2011 2023-04-12 03:04:01.496598 hdict-0.230412.3/src/hdict/content/entry/__init__.py
--rw-r--r--   0        0        0     1965 2023-04-12 20:17:41.358683 hdict-0.230412.3/src/hdict/content/entry/aux_closure.py
--rw-r--r--   0        0        0     1346 2023-04-12 20:17:41.358683 hdict-0.230412.3/src/hdict/content/entry/cached.py
--rw-r--r--   0        0        0     4337 2023-04-12 20:17:41.418684 hdict-0.230412.3/src/hdict/content/entry/closure.py
--rw-r--r--   0        0        0     2836 2023-04-12 20:17:41.342683 hdict-0.230412.3/src/hdict/content/entry/subvalue.py
--rw-r--r--   0        0        0      541 2023-04-12 20:17:41.322682 hdict-0.230412.3/src/hdict/content/entry/wrapper.py
--rw-r--r--   0        0        0     2254 2023-04-09 16:29:46.578822 hdict-0.230412.3/src/hdict/content/value.py
--rw-r--r--   0        0        0        0 2023-04-09 16:23:36.171526 hdict-0.230412.3/src/hdict/data/__init__.py
--rw-r--r--   0        0        0    10419 2023-04-12 20:17:41.442684 hdict-0.230412.3/src/hdict/data/aux_frozendict.py
--rw-r--r--   0        0        0     2211 2023-04-12 20:12:17.393861 hdict-0.230412.3/src/hdict/data/empty_.py
--rw-r--r--   0        0        0    20295 2023-04-12 20:17:41.534686 hdict-0.230412.3/src/hdict/data/frozenhdict.py
--rw-r--r--   0        0        0    25386 2023-04-12 19:38:21.121053 hdict-0.230412.3/src/hdict/data/hdict_.py
--rw-r--r--   0        0        0        0 2023-03-19 02:22:28.761130 hdict-0.230412.3/src/hdict/dataset/__init__.py
--rw-r--r--   0        0        0     6523 2023-04-12 20:17:41.354683 hdict-0.230412.3/src/hdict/dataset/dataset.py
--rw-r--r--   0        0        0     4273 2023-04-12 20:17:41.334683 hdict-0.230412.3/src/hdict/dataset/pandas_handling.py
--rw-r--r--   0        0        0        0 2023-04-09 16:15:22.403037 hdict-0.230412.3/src/hdict/expression/__init__.py
--rw-r--r--   0        0        0     3543 2023-04-12 20:17:41.362683 hdict-0.230412.3/src/hdict/expression/expr.py
--rw-r--r--   0        0        0        0 2023-04-09 16:21:52.487456 hdict-0.230412.3/src/hdict/expression/step/__init__.py
--rw-r--r--   0        0        0     2280 2023-04-10 01:05:51.172495 hdict-0.230412.3/src/hdict/expression/step/applyout.py
--rw-r--r--   0        0        0     2529 2023-04-09 16:42:55.111337 hdict-0.230412.3/src/hdict/expression/step/cache.py
--rw-r--r--   0        0        0      395 2023-04-12 20:17:41.330683 hdict-0.230412.3/src/hdict/expression/step/edict.py
--rw-r--r--   0        0        0     2198 2023-04-12 20:17:41.370683 hdict-0.230412.3/src/hdict/expression/step/step.py
--rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230412.3/src/hdict/persistence/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-09 01:26:32.621571 hdict-0.230412.3/src/hdict/persistence/stored.py
--rw-r--r--   0        0        0        0 2023-04-09 16:30:09.274848 hdict-0.230412.3/src/hdict/text/__init__.py
--rw-r--r--   0        0        0     7455 2023-04-12 19:38:03.344816 hdict-0.230412.3/src/hdict/text/customjson.py
--rw-r--r--   0        0        0     9234 1970-01-01 00:00:00.000000 hdict-0.230412.3/setup.py
--rw-r--r--   0        0        0     8742 1970-01-01 00:00:00.000000 hdict-0.230412.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-1.230706.1/LICENSE
+-rw-r--r--   0        0        0     7696 2023-07-06 23:25:53.275010 hdict-1.230706.1/README.md
+-rw-r--r--   0        0        0     1385 2023-07-06 23:26:54.439029 hdict-1.230706.1/pyproject.toml
+-rw-r--r--   0        0        0    15595 2023-07-06 23:14:52.886751 hdict-1.230706.1/src/hdict/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/abs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/__init__.py
+-rw-r--r--   0        0        0      755 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/__init__.py
+-rw-r--r--   0        0        0    14478 2023-07-06 23:19:47.382880 hdict-1.230706.1/src/hdict/content/argument/apply.py
+-rw-r--r--   0        0        0     3242 2023-07-06 22:11:28.034640 hdict-1.230706.1/src/hdict/content/argument/aux_apply.py
+-rw-r--r--   0        0        0     1483 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/default.py
+-rw-r--r--   0        0        0     1318 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/entry.py
+-rw-r--r--   0        0        0     2162 2023-07-06 23:15:22.758765 hdict-1.230706.1/src/hdict/content/argument/field.py
+-rw-r--r--   0        0        0     2330 2023-07-06 22:17:01.298525 hdict-1.230706.1/src/hdict/content/argument/sample.py
+-rw-r--r--   0        0        0     3967 2023-07-06 22:34:49.954302 hdict-1.230706.1/src/hdict/content/aux_value.py
+-rw-r--r--   0        0        0     2011 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/__init__.py
+-rw-r--r--   0        0        0     1965 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/aux_closure.py
+-rw-r--r--   0        0        0     1346 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/cached.py
+-rw-r--r--   0        0        0     4378 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/closure.py
+-rw-r--r--   0        0        0     2835 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/subvalue.py
+-rw-r--r--   0        0        0      541 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/wrapper.py
+-rw-r--r--   0        0        0     2254 2023-07-06 22:53:17.646321 hdict-1.230706.1/src/hdict/content/value.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/data/__init__.py
+-rw-r--r--   0        0        0    10149 2023-07-06 23:16:22.646793 hdict-1.230706.1/src/hdict/data/aux_frozendict.py
+-rw-r--r--   0        0        0     2211 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/data/empty_.py
+-rw-r--r--   0        0        0    21144 2023-07-06 23:19:47.554880 hdict-1.230706.1/src/hdict/data/frozenhdict.py
+-rw-r--r--   0        0        0    24195 2023-07-06 23:20:34.062898 hdict-1.230706.1/src/hdict/data/hdict_.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/dataset/__init__.py
+-rw-r--r--   0        0        0     8333 2023-07-06 23:23:02.878954 hdict-1.230706.1/src/hdict/dataset/dataset.py
+-rw-r--r--   0        0        0     4465 2023-07-06 23:23:48.782970 hdict-1.230706.1/src/hdict/dataset/pandas_handling.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/__init__.py
+-rw-r--r--   0        0        0     3543 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/expr.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-06 23:24:29.266983 hdict-1.230706.1/src/hdict/expression/step/applyout.py
+-rw-r--r--   0        0        0     2529 2023-07-06 23:19:24.594871 hdict-1.230706.1/src/hdict/expression/step/cache.py
+-rw-r--r--   0        0        0      395 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/edict.py
+-rw-r--r--   0        0        0     2198 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/step.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/persistence/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/persistence/stored.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/text/__init__.py
+-rw-r--r--   0        0        0     7525 2023-07-06 23:19:47.262880 hdict-1.230706.1/src/hdict/text/customjson.py
+-rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 hdict-1.230706.1/setup.py
+-rw-r--r--   0        0        0     8740 1970-01-01 00:00:00.000000 hdict-1.230706.1/PKG-INFO
```

### Comparing `hdict-0.230412.3/LICENSE` & `hdict-1.230706.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/README.md` & `hdict-1.230706.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ![test](https://github.com/davips/hdict/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
 <a href="https://pypi.org/project/hdict">
 <img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.10...-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
 [![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ![test](https://github.com/davips/hdict/workflows/test/badge.svg) [![codecov]
 (https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://
 codecov.io/gh/davips/hdict) [pypi] ![Python version](https://img.shields.io/
-badge/python-3.10...-blue.svg) [![license: GPL v3](https://img.shields.io/
-badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  [![arXiv]
+badge/python-3.10+-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
+License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  [![arXiv]
 (https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)]
 (https://arxiv.org/abs/2109.06028) [![API documentation](https://
 img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/
 hdict) [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)]
 (https://hosh.page) [![Downloads](https://static.pepy.tech/badge/hdict)](https:
 //pepy.tech/project/hdict) # hdict { A _unique_ data structure } [Website]
 (https://hosh.page) | [Latest Release](https://pypi.org/project/hdict) |
```

### Comparing `hdict-0.230412.3/pyproject.toml` & `hdict-1.230706.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "hdict"
-version = "0.230412.3"
+version = "1.230706.1"
 description = "A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others."
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPLv3"
-readme = 'README.md'
+readme = "README.md"
 packages = [
     { include = "hdict", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-hosh = "^2.230205.2"
+hosh = "^3.230705.2"
 indexed = "^1.3.0"  # indexed dict
 lange = "^1.230203.2"
 
 # Optional dependencies.
 pandas = { version = "^2.0.0", optional = true }
 shelchemy = { version = "^0.220906.3", optional = true }
 safeserializer = { version = "^0.230202.1", optional = true }
 lz4 = { version = "^4.3.2", optional = true }
 scikit-learn = { version = "^1.2.2", optional = true }
 liac-arff = { version = "^2.5.0", optional = true }
 
 [tool.poetry.extras]    #[tool.poetry.group.extras.dependencies]
-full = ["pandas", "shelchemy", "safeserializer", "lz4", "scikit-learn", "liac-arff"]
+full = ["pandas", "shelchemy", "safeserializer", "lz4", "scikit-learn", "liac-arff", "testfixtures"]
 
 [tool.poetry.group.dev.dependencies]
 autoreadme = "^0.2102.20"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 black = "^22.6.0"
 pdoc3 = "^0.10.0"
```

### Comparing `hdict-0.230412.3/src/hdict/__init__.py` & `hdict-1.230706.1/src/hdict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -118,77 +118,77 @@
         ww2: λ(9 y=r2)→1,
         zzzz: λ(9 13),
         f: "CustomClass()",
         zzz1: λ(11 33)→0,
         www1: λ(11 33)→1,
         zzz2: λ(r1 44)→0,
         www2: λ(r1 44)→1,
-        _id: DCHyNhF2j6CaptG.6gb9UL9RVIMztgnnbVI5MHxh,
+        _id: i5wtTs5qggivS-y5TNuhnM5jwokjF132M7jF.49a,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             alpha: A1RyW.GoA3q9-iCbCvWyWClExm1J3wI.ok6UA3Nk,
             beta: WM5TbiaJ1gLqKRSFiY3VkZEu1PwQcaAokBKBPrWg,
             gamma: yb-HU.jSxd496XfId1J..MkX7xfUPJOL1-07hHdt,
-            p1: ggJAsAHfZm2fiI0HmIbBhyZMNP9z06QJEfO24Xx2,
-            q1: YMfRygkG8EoBSwIFWwbZfEyHcQ8dlDnKo1.gOijC,
-            pq: Zm4nTmd2OIE5Ij9NJjU4DqG.hgqMlJbs1hNjSdRE,
-            p2: -RZv1aQW198-uu1wAFsRzS5CalP8THUWSHUgTy6q,
-            q2: wPuaLzMJX-wU-b6-z4A7n1hnDi-woaKQq745qo0E,
-            z1: 8dPQ2blIctM6p7mByuoL0EnTlg5no0TxEJtoACbt,
-            w1: JbWdguqn24m9-XathFYdhhMRBDvWFQVktmxj7gWL,
-            z2: 8dPQ2blIctM6p7mByuoL0EnTlg5no0TxEJtoACbt,
-            w2: JbWdguqn24m9-XathFYdhhMRBDvWFQVktmxj7gWL,
-            r1: Y3AxJytRz1Pnf8Q1bjC2jWUs3oTzAALXYkwlH1GI,
-            r2: JdDJ6LPyvJ2xnbPUwBFKDIt8k-udb4czb8PjX8dh,
-            r3: 015TXOnn-Z6AfT1ajcNN4brMD6c8YsRn73kA7RPh,
-            ra1: 8dPQ2blIctM6p7mByuoL0EnTlg5no0TxEJtoACbt,
-            rb1: JbWdguqn24m9-XathFYdhhMRBDvWFQVktmxj7gWL,
-            ra2: 8dPQ2blIctM6p7mByuoL0EnTlg5no0TxEJtoACbt,
-            rb2: JbWdguqn24m9-XathFYdhhMRBDvWFQVktmxj7gWL,
-            zz1: mQUu0IxSblJEAplB0yVRVN-rY6bv06spvVH8krlt,
-            ww1: 7J8PIEG1QPZMBDimMibqHaJPFg6pHG8mQGvDM9Pf,
-            zz2: sHib6xdxGc8tQ6CzacEANreEUZH.sjkZhIa6ZJRc,
-            ww2: FO-4MA-2R.Hp40Fa1cOnY70x.vFfraTBMvYDCTa7,
-            zzzz: GCskxsxNUipp-aSntVX1tASXmXbTqCEJ46YonXVu,
+            p1: Qs0J0I.AhR.brQjpYwUJqDNLk-zKd7FmG0g7gdd1,
+            q1: VOAVwyrrdC7eIsjnVkqdpsqUfhprKzKriATFEOQI,
+            pq: KtTWRcFQRKVgTJabGMgY-HAQWJ1TZGnOYw7NU.1K,
+            p2: qb0H0MqNit0rLwk6CsC4Q2bxpCmBQ581eoGI39sr,
+            q2: Sjsl-.MJJ3SK2.INLAJ-0R5BwlfG.tccIpxPFRtB,
+            z1: w8obIVknqdoKk.hDUN8TE2M-KiFh-yCCXtxNdrJ4,
+            w1: T0hCevYdBG6vWZ3R5Nba.jXacMTFFUW5OjOX4yAO,
+            z2: w8obIVknqdoKk.hDUN8TE2M-KiFh-yCCXtxNdrJ4,
+            w2: T0hCevYdBG6vWZ3R5Nba.jXacMTFFUW5OjOX4yAO,
+            r1: FO3NXIQIi7TBFw1FqLRJYo13EA.uu4Y-L17Fmx0z,
+            r2: HorxHsNCdpkm270yeTZ-vREjjFXWIYC99ALidDVU,
+            r3: bWc33lXvXHIJXix5Jw2.Nhw0EIsv3TuAa7t8Ix5q,
+            ra1: w8obIVknqdoKk.hDUN8TE2M-KiFh-yCCXtxNdrJ4,
+            rb1: T0hCevYdBG6vWZ3R5Nba.jXacMTFFUW5OjOX4yAO,
+            ra2: w8obIVknqdoKk.hDUN8TE2M-KiFh-yCCXtxNdrJ4,
+            rb2: T0hCevYdBG6vWZ3R5Nba.jXacMTFFUW5OjOX4yAO,
+            zz1: FB6W9j12qWZ34fUwyrBETzFuAXRB-xn7O1PGhr2j,
+            ww1: IhchjkRfjLXpnsC6zl-TFugIQrnUIdB7Wsgpnely,
+            zz2: LE5ohPby7q4dNu3qhqgucRcCt.pd87O.CyKWloqe,
+            ww2: -RBf-UiccAG3sTH0UFC6C.YFmYcpTRA.0PFP6Oun,
+            zzzz: Irbj-xVP8rEIPoylOTNmiuJ-lGdx0dpzIPgq-169,
             f: Some.arbitrary.identifier.with.length.40,
-            zzz1: Oq-jsn9xtOoG1PvtuUo99Ha-nhgow1Wwbje4TdSd,
-            www1: lUCDq9mlpw-qZEx6DRlM5BSq.xj-mOtv.L38Yuti,
-            zzz2: ivhVbLM3q-CE9M4.MFf29k3FDj8fU.8GMfZZwKh3,
-            www2: fFEl3XJdY9-tX.iVWY2FevFv5SS85e.FDrjZm2NN
+            zzz1: TBw0fUZZo1WlI9uczNuF0w4vC06u6YvzJyNPVEi1,
+            www1: WqqXpIpMwinaXxYNqRjj4qttDcKXN.gcGjARpOSh,
+            zzz2: .mJim0y-LMUYZi01GN8MTPkHj79JtFdREf7g40ug,
+            www2: jwtsaf1IZMG6sWqprXZnc.n-ilyfncwhL3Qr.-Md
         }
     }
     >>> d["p1"]
     243
     >>> from hdict import value
     >>> d.evaluate()
     >>> d = hdict(x=2)
     >>> g = lambda x, y: [x + y, x / y]
     >>> d["z"] = apply(f, 2, y=3)
     >>> d["w", "v"] = apply(f, field("x"), y=33)
     >>> d["f"] = f
-    >>> d = d >> apply(field("f"), field("x"), y=default(3), nonexistent_parameter=7)("w3", "v3") # TODO: nonexistent parameter should raise an exception
+    >>> d = d >> apply(field("f"), field("x"), y=default(3), nonexistent_parameter=7)("w3", "v3") # todo: : nonexistent parameter should raise an exception
     >>> d >>= apply(field("f"), field("x"), y=default(3))("w", "v")
     >>> d["w2", "v2"] = apply(field("f"), field("x"), y=default(3))
     >>> d >>= {"z": apply(f, field("x"), y=3), ("w", "v"): apply(g, y=7)}
     >>> d >>= apply(f, field("x"), y=3)("z9") * apply(g, y=7)("w9", "v9")
     >>> pp = apply(f, field("x"), y=3)("z") >> apply(g, y=7)("w", "v")
     >>> d >>= {"x": 3} >> pp >> apply(g, y=7)("w", "v")
     >>> from hdict import _
     >>> a1 = apply(f, y=_[1, 2, 4, ..., 128])
     >>> a2 = apply(f, _[0, 3, 6, ..., 9], y=_[0, 3, 6, ..., 9])
     >>> ppp = hdict() >> a2.sample()("k", "t")
     >>> ppp.show(colored=False)
     {
         k: λ(9 9)→0,
         t: λ(9 9)→1,
-        _id: eeMrAInYUG2lzUrGqgY0vSZd4KpYpc5vu.bV9bbP,
+        _id: dK-iumb4L5nkFVT9LCkdk3daQtuC.ORk6JwWMhnt,
         _ids: {
-            k: UgmJcTz6qQgNFiwe.S40EC69Ab6drWQ5JCw8ON3q,
-            t: MCyEzFX.viNxTiRwTio0j7dA9LDf-TwFRNKA0JhY
+            k: rHTgwW.w2SsbcvBlSnWWddLH4vgyXlM1Fhxqr48f,
+            t: IldA8m-uSN9lJcE4TBtjTcY-sSiA33mzxQ2k-wpN
         }
     }
     >>> ppp.k
     387420489
     >>> a1("z")
     z=λ(x y=~[1 2 .*. 128])
     >>> a2(w="a", v="b")
@@ -203,25 +203,25 @@
     >>> sampled = app.sample(0).c
     >>> sampled
     c=λ(9 b=default(4))
     >>> r = hdict() >> sampled
     >>> r.show(colored=False)
     {
         c: λ(9 b=4),
-        _id: -3fKdfaAaTp.4XwUm1FzlzM81PYZSgsIZEuRRCD4,
+        _id: Bbe5mzn0oCuHZ.Y84-jaEnh3jcrgD8av6IZezKEG,
         _ids: {
-            c: Ht.fDdFk9WOHzT27dOKLvaoHY0YB7Nx.Q2MNXTzJ
+            c: 6EehD7OoZe2REI.1YsVLKxSF4hJoYxfOZJLbF.Aj
         }
     }
     >>> r.evaluated.show(colored=False)
     {
         c: 5,
-        _id: -3fKdfaAaTp.4XwUm1FzlzM81PYZSgsIZEuRRCD4,
+        _id: Bbe5mzn0oCuHZ.Y84-jaEnh3jcrgD8av6IZezKEG,
         _ids: {
-            c: Ht.fDdFk9WOHzT27dOKLvaoHY0YB7Nx.Q2MNXTzJ
+            c: 6EehD7OoZe2REI.1YsVLKxSF4hJoYxfOZJLbF.Aj
         }
     }
     >>> from random import Random
     >>> rnd = Random(0)
     >>> p1 = p.sample(rnd)
     >>> d["w"]
     10
@@ -234,35 +234,35 @@
     >>> p = apply(f, y=_[1, 2, 4, ..., 128])("z") >> apply(f, y=_[0, 3, 6, ..., 9])(w="a", v="b")
     >>> d.show(colored=False)
     {
         w: 6,
         z: λ(x=w 3)→z,
         ww: λ(4 7)→0,
         v: λ(4 7)→1,
-        _id: Hu.P9nMRy97xUe7prRc3k-Uwvz2p5emCpSyVSdIC,
+        _id: x4TxaVuAymsh97Yr.15Oc1ekllvlpECk091124RM,
         _ids: {
             w: CZ7Jm5fQMZ3fZJ3kAVOi0FYK-exFqPqgoYLsGxGl,
-            z: 3eItvrVzHQPDEYbQRbksBHiCaQbe2Ia2m7Z2P1lw,
-            ww: VdHav0HHdJC6gfOF8Fqw7AFX9IYQyrIUOZc8G.Pp,
-            v: KtYqDG5UPyrYEv-5V5RaUQasieAwAjF1bYf3Tvyy
+            z: No1nN40OXnJ.zOyAvoxwCjyD06cUDiXTZQh4q8xa,
+            ww: qZepp.wpXCOYQrwnVIwoZ4kR9pIuMGDQpvRevv80,
+            v: wxkjBSP54cKEfxKE1Zte-2dDll3G9Nd-yDh3CLas
         }
     }
     >>> d = hdict(x=3) >> p.sample(rnd)
     >>> d.show(colored=False)
     {
         x: 3,
         z: λ(x 16),
         w: λ(x 9)→a,
         v: λ(x 9)→b,
-        _id: OIVFm0IdYK3jtOApTVCwdLTVXXNGarxDkUCwB0Iv,
+        _id: 22b-e.CtRGVSoMkektNzHYSVZTouhL2jAHLyPd4Q,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
-            z: -F83hM-wE8ykmcEM1XvuG.XBpo7rzkuHfNKzTVMz,
-            w: G7CpHeVpUD5KfNpJmRaMC2Rt4rTeQjIuAeGuZXSa,
-            v: glVBFsjtDi7RrpvqrV.5vh.dp.RgASp25V-qlClj
+            z: 64cxw0HmJ0fydH7By6i0HrbuwA759XexTu3Bu0Zd,
+            w: p1Z5umNo12DHCZtKbh2EClW6TZxv.M447HlALWhv,
+            v: HbYbR1RjPdU4jixjW7xSxslRpYx9W6Oiay7maK6F
         }
     }
     >>> d1 = hdict(x=52, y=13)
     >>> d2 = hdict(x=value(52, hosh="1234567890123456789012345678901234567890"))
     >>> d1.show(colored=False)
     {
         x: 52,
@@ -371,33 +371,33 @@
     }
     >>> d >>= apply(lambda a: a)("x")
     >>> d.show(colored=False)
     {
         a: 5,
         y: 28,
         x: λ(a),
-        _id: q5J7ZUr3gs0bKrG4AxVEY2q0-XH3Suvw5X8-j6do,
+        _id: qI8rmiUzMTSO1pMkCeQJpHTAOw4xuooFqM41iIiY,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
-            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR
+            x: sxkIk6E9l8oScCyoGDlzrqJ9QgpIpl5PCBvHlERp
         }
     }
-    >>> {"_id": "q5J7ZUr3gs0bKrG4AxVEY2q0-XH3Suvw5X8-j6do"} == d
+    >>> {"_id": "qI8rmiUzMTSO1pMkCeQJpHTAOw4xuooFqM41iIiY"} == d
     True
     >>> d.show(colored=False)
     {
         a: 5,
         y: 28,
         x: λ(a),
-        _id: q5J7ZUr3gs0bKrG4AxVEY2q0-XH3Suvw5X8-j6do,
+        _id: qI8rmiUzMTSO1pMkCeQJpHTAOw4xuooFqM41iIiY,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
-            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR
+            x: sxkIk6E9l8oScCyoGDlzrqJ9QgpIpl5PCBvHlERp
         }
     }
     >>> def f():
     ...     print("busy")
     ...     return 23
     >>> storage = {}
     >>> d >>= apply(f).o >> cache(storage, "x", "y")
@@ -405,49 +405,49 @@
     28
     >>> d.show(colored=False)
     {
         a: 5,
         y: 28,
         x: ↑↓ cached at `dict`·,
         o: λ(),
-        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _id: 4FdTqXVIMKldUnZgrrp315c78KHD9yu7T.Nr5zGv,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
-            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
-            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+            x: sxkIk6E9l8oScCyoGDlzrqJ9QgpIpl5PCBvHlERp,
+            o: Re1o0YXNebYNezPrVv2dOrFxtgLQutD-b-SHFRbo
         }
     }
     >>> d.evaluated.show(colored=False)
     busy
     {
         a: 5,
         y: 28,
         x: 5,
         o: 23,
-        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _id: 4FdTqXVIMKldUnZgrrp315c78KHD9yu7T.Nr5zGv,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
-            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
-            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+            x: sxkIk6E9l8oScCyoGDlzrqJ9QgpIpl5PCBvHlERp,
+            o: Re1o0YXNebYNezPrVv2dOrFxtgLQutD-b-SHFRbo
         }
     }
     >>> d.evaluated.show(colored=False)
     {
         a: 5,
         y: 28,
         x: 5,
         o: 23,
-        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _id: 4FdTqXVIMKldUnZgrrp315c78KHD9yu7T.Nr5zGv,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
-            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
-            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+            x: sxkIk6E9l8oScCyoGDlzrqJ9QgpIpl5PCBvHlERp,
+            o: Re1o0YXNebYNezPrVv2dOrFxtgLQutD-b-SHFRbo
         }
     }
     """
 
 
 class Empty(Empty_):
     """
```

### Comparing `hdict-0.230412.3/src/hdict/content/argument/__init__.py` & `hdict-1.230706.1/src/hdict/content/argument/__init__.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/argument/apply.py` & `hdict-1.230706.1/src/hdict/content/argument/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,32 @@
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 from __future__ import annotations
 
-from inspect import isfunction
+from inspect import isfunction, isbuiltin, isclass
 from inspect import signature
 from itertools import chain
 from random import Random
 
 from hosh import Hosh
 
 from hdict.content.argument import AbsBaseArgument, AbsArgument
 from hdict.content.argument.field import field
 from hdict.text.customjson import truncate
 from hdict.content.aux_value import f2hosh
 
 
+def getattr_(__o: object, name: str, __default=None):
+    return getattr(__o, name, __default)
+
+
+# todo hide unneeded attrs to avoid poluting namespace for output field
 class apply(AbsBaseArgument):
     """
     Function application
 
     Single output application is defined by attribute: 'apply(f).my_output_field'.
     Multioutput application is defined by a call: 'apply(f)("output_field1", "output_field2")'.
 
@@ -87,36 +92,36 @@
     {'a': 3, 'b': 4, 'c': 5, 'd': default(2), 'e': default(13)}
     >>> apply(f,3,4,5,6).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': default(13)}
     >>> apply(f,3,4,5,6,7).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': 7}
     >>> apply(f,d=5).requirements
     {'a': field(a), 'b': field(b), 'c': default(1), 'd': 5, 'e': default(13)}
-    >>> f = lambda a,b, *contentarg, c=1,d=2,e=13, **kwargs: 0
+    >>> f = lambda a,b, *arg, c=1,d=2,e=13, **kwargs: 0
     >>> apply(f,3,4,5,6,7,8).requirements
-    {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': 7, _5: 8}
+    {'a': 3, 'b': 4, arg_2: 5, arg_3: 6, arg_4: 7, arg_5: 8, 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> apply(f,x=3,e=4,d=5,c=6,b=7,a=8).requirements
     {'a': 8, 'b': 7, 'c': 6, 'd': 5, 'e': 4, 'x': 3}
     >>> apply(f,3,c=77,x=5).requirements
     {'a': 3, 'b': field(b), 'c': 77, 'd': default(2), 'e': default(13), 'x': 5}
     >>> apply(f,b=77,x=5).requirements
     {'a': field(a), 'b': 77, 'c': default(1), 'd': default(2), 'e': default(13), 'x': 5}
     >>> from hdict.content.argument.entry import entry
     >>> a = apply(lambda x: x.value * 7, x=entry("x"))
     >>> c = {"x": 3, "y": entry("x")} >> a.r
     >>> c.show(colored=False)
     {
         x: 3,
         y: ·3,
         r: λ(·x),
-        _id: drMRkK24R01dlyw0ye-Rx8Gzac7zxmZUS.toA1gi,
+        _id: bh0bgTZI.2f-WteZFpIrsMxJvZYUBydOfF3wFLV.,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
-            r: .PtYLSxMYqVXNTh-mnqsQygl4goFXoRrXCtQrTYP
+            r: NoAit6.-dyFNiCZnoRAhY5zbJ0hc6u5lkQzYwBCx
         }
     }
     >>> b = a.x.sample()
     >>> b
     x=λ(·x)
     >>> d = {"x": 3} >> b
     >>> d.x
@@ -132,17 +137,17 @@
         h: {
             a: 2,
             _id: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             _ids: {
                 a: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
             }
         },
-        _id: Wjqo4.Qw7KBK6NbppnlKT2W3d5KScpptjoCcNsjj,
+        _id: V8nyMrJbhGschQAaW3ZXD6uxvVRIluFmIFIkSaZ0,
         _ids: {
-            x: .PtYLSxMYqVXNTh-mnqsQygl4goFXoRrXCtQrTYP,
+            x: NoAit6.-dyFNiCZnoRAhY5zbJ0hc6u5lkQzYwBCx,
             h: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd
         }
     }
     >>> a = apply(lambda x: x.value * 7).x
     >>> d >>= a
     >>> d.show(colored=False)
     {
@@ -150,17 +155,17 @@
         h: {
             a: 2,
             _id: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             _ids: {
                 a: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
             }
         },
-        _id: 5fUCSwb7D633jeGv.xMb006XT8Ulr18os.KxyeTH,
+        _id: okwLxwrcv9.FCsOTgCrB0ZG0yBArMbEaeqXNIGa7,
         _ids: {
-            x: -89UidPh6BgYdYYTx4nxewuDpdilgWzm4O6adFwc,
+            x: H8Tgrs3lS78y7Nqm0Qaaks8JLygevb49SEOpn5QD,
             h: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd
         }
     }
     >>> a = apply(lambda x: x.value * 7, entry("x")).x
     >>> d >>= a
     >>> d.show(colored=False)
     {
@@ -168,17 +173,17 @@
         h: {
             a: 2,
             _id: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             _ids: {
                 a: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
             }
         },
-        _id: pEhqOs9sPjot-eiGgJbKQ5j7aTL1MySiBaoTj0r4,
+        _id: ZAozaV7y5Z1cjwzR9XoiBggegMtt9VC-Leafzaod,
         _ids: {
-            x: mmdYysfo0-rbXPLWBaqHKdxGkR9xwyihdlfv-q4B,
+            x: Hqq4pKtqmIAejPzyjEf6BixYtzWYVU2Znp1TdB1K,
             h: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd
         }
     }
     >>> d >>= {"b" : 2, "c": entry("b")}
     >>> d.show(colored=False)
     {
         x: λ(λ(x=21)),
@@ -187,26 +192,26 @@
             _id: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             _ids: {
                 a: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
             }
         },
         b: 2,
         c: ·2,
-        _id: WoI36oD8iHnd81y0q-VTpbFoN2rhdAbRGOk1yBK5,
+        _id: 9bTAxQR8bR-XsqVTjc7sLgCvTXoJCWXwRS6pNLHe,
         _ids: {
-            x: mmdYysfo0-rbXPLWBaqHKdxGkR9xwyihdlfv-q4B,
+            x: Hqq4pKtqmIAejPzyjEf6BixYtzWYVU2Znp1TdB1K,
             h: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             b: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29,
             c: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
         }
     }
     >>> d >>= {"b" : (2, 3), ("a1", "b1"): [0, 1]}
     >>> d >>= {("a2", "b2"): _.b}
     >>> d >>= {("a3", "b3"): entry("b")}
-    >>> d.show(colored=False)  # TODO: improve output for subvalues (and backtracking in general for pointer-like entries)
+    >>> d.show(colored=False)  # todo: : improve output for subvalues (and backtracking in general for pointer-like entries)
     {
         x: λ(λ(x=21)),
         h: {
             a: 2,
             _id: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             _ids: {
                 a: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29
@@ -219,17 +224,17 @@
         c: ·2,
         a1: 0,
         b1: 1,
         a2: "(2, 3)→0",
         b2: "(2, 3)→1",
         a3: ·(2, 3)→0,
         b3: ·(2, 3)→1,
-        _id: jY2TGGf9ZSvPk7k3Mu4bgeJJXZ45Gwwye.wPVBgX,
+        _id: gf.QcPTyypNvMcSEMveLdLVC2T218MgepHPb9Md4,
         _ids: {
-            x: mmdYysfo0-rbXPLWBaqHKdxGkR9xwyihdlfv-q4B,
+            x: Hqq4pKtqmIAejPzyjEf6BixYtzWYVU2Znp1TdB1K,
             h: GfMhwM5bo6OzIpngAf8Ruro6.QgOv2kb0nbj0mgd,
             b: -a.WUGANQp6aVgbRCtUljlgs12HNtJ-dJOAgSZWk,
             c: k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29,
             a1: M7HyZUgSF.ZSmBEMFcDkiZBQz00wU9pGF3DoRiDu,
             b1: DYu5bfVvb6FOhBCWNsss4wsEWHZYTbKnsVgoWFvl,
             a2: GfnITQ6RdDtm4F-F0UuU8fOJX1DZIBZG5RWBM8wm,
             b2: QznFPbiCaMRZKUoFhdLxMKYQf3ujIe1zDl9G5Rq-,
@@ -251,31 +256,37 @@
         if isinstance(appliable, apply):  # "clone" mode
             self.fhosh = fhosh or appliable.fhosh
             self.fargs, self.fkwargs = appliable.fargs.copy(), appliable.fkwargs.copy()
             self.isfield = appliable.isfield
             self._sampleable = appliable.sampleable if _sampleable is None else _sampleable
             self.appliable = appliable.appliable
         elif isinstance(appliable, field):
-            # TODO: o que era isso mesmo?::  "function will be provided by hdict"-mode constrains 'applied_args'
+            # todo: : o que era isso mesmo?::  "function will be provided by hdict"-mode constrains 'applied_args'
             self.fhosh = fhosh
             self.fargs, self.fkwargs = handle_args(None, applied_args, applied_kwargs)
             self.isfield = True
             self._sampleable = _sampleable
         elif callable(appliable):
-            if not isfunction(appliable):  # "not function" means "custom callable"
+            if not (
+                isfunction(appliable) or isbuiltin(appliable) or isclass(appliable)
+            ):  # "not function" means "custom callable"; `builtin_function_or_method` is not a function and does not allow signature extraction.
                 if not hasattr(appliable, "__call__"):  # pragma: no cover
                     raise Exception(f"Cannot infer method to apply non custom callable type '{type(appliable).__name__}'.")
                 if not hasattr(appliable, "hosh"):  # pragma: no cover
                     raise Exception(f"Missing 'hosh' attribute while applying custom callable class '{type(appliable).__name__}'")
                 # noinspection PyUnresolvedReferences
                 sig = signature(appliable.__call__)
                 # noinspection PyUnresolvedReferences
                 self.fhosh = fhosh or appliable.hosh
             else:
                 self.fhosh = f2hosh(appliable) if fhosh is None else fhosh
+                s = str(appliable)
+                if s.startswith("<built-in function"):
+                    if s.endswith("getattr>"):
+                        self.appliable = appliable = getattr_
                 sig = signature(appliable)
 
             # Separate positional parameters from named parameters looking at 'f' signature.
             self.fargs, self.fkwargs = handle_args(sig, applied_args, applied_kwargs)
             self._sampleable = _sampleable
         else:  # pragma: no cover
             raise Exception(f"Cannot apply type '{type(appliable).__name__}'.")
```

### Comparing `hdict-0.230412.3/src/hdict/content/argument/aux_apply.py` & `hdict-1.230706.1/src/hdict/content/argument/aux_apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,29 @@
     {'a': 'a', 'b': 'b'}
     """
 
     def __repr__(self):
         return repr(dict(self.items()))
 
 
-class Arg:
+class Arg(str):
     def __init__(self, position: int):
         self.position = position
 
     def __hash__(self):
         return hash(self.position)
 
     def __lt__(self, other):
-        return f"~{self.position}" < other
+        return f"~{self.position}" < str(other)
+
+    def __ge__(self, other):
+        return f"~{self.position}" >= str(other)
 
     def __repr__(self):
-        return f"_{self.position}"
+        return f"arg_{self.position}"
 
 
 def handle_args(signature, applied_args, applied_kwargs):
     from hdict.content.argument.field import field
     from hdict.content.value import value
 
     # Separate positional from named parameters of 'f'.
@@ -69,25 +72,25 @@
         if i < len(fargs):
             # noinspection PyUnresolvedReferences
             used.add(key := fargs.keys()[i])
             fargs[key] = wrap(applied_arg)
         else:
             if i >= len(params):
                 if not hasargs:  # pragma: no cover
-                    raise Exception("Too many arguments to apply. No '*contentarg' detected for 'f'.")
+                    raise Exception("Too many arguments to apply. No '*arg' detected for 'f'.")
                 name = Arg(i)  # REMINDER: this is just a unique hash for the nameless argument
             else:
-                name = params[i]
+                name = Arg(i) if hasargs and i >= len(fargs) else params[i]
                 if name in fkwargs:
                     del fkwargs[name]
             fargs[name] = wrap(applied_arg)
 
     for applied_kwarg, v in applied_kwargs.items():
         if applied_kwarg in used:  # pragma: no cover
-            raise Exception(f"Parameter '{applied_kwarg}' cannot appear in both 'contentarg' and 'kwargs' of 'apply()'.")
+            raise Exception(f"Parameter '{applied_kwarg}' cannot appear in both 'arg' and 'kwargs' of 'apply()'.")
         if applied_kwarg in fargs:
             fargs[applied_kwarg] = wrap(v)
         elif applied_kwarg in fkwargs or haskwargs:
             fkwargs[applied_kwarg] = wrap(v)
         else:  # pragma: no cover
             raise Exception(f"Parameter '{applied_kwarg}' is not present in 'f' signature nor '**kwargs' was detected for 'f'.")
```

### Comparing `hdict-0.230412.3/src/hdict/content/argument/default.py` & `hdict-1.230706.1/src/hdict/content/argument/default.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/argument/entry.py` & `hdict-1.230706.1/src/hdict/content/argument/entry.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/argument/field.py` & `hdict-1.230706.1/src/hdict/content/argument/field.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     }
     >>> d >>= {"x": 3, "y": 5} >> apply(lambda x, y: x + y).z
     >>> d.show(colored=False)
     {
         x: 3,
         y: 5,
         z: λ(x y),
-        _id: P0R5Ra1aPrsql5iYJsmYG56.0oCFvqPQIMv3Qe7b,
+        _id: ..SSoOQF.FYZDUevP1CGj0DJVc.M8cgimN70yI3C,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: Q1ypbWuXlEf9MeJNT1wyFcA8V0.DvHEFOeCidBrZ
+            z: 3j029VhuvENAnBK6JLRGl8ePpsQybm57sXKfX2oo
         }
     }
     >>> d >>= {"x": 3, "y": 5} >> apply(lambda x, y: x + y).x
     >>> d.x
     8
     >>> d["x"] = apply(lambda x, y: x + y)
     >>> d.x
```

### Comparing `hdict-0.230412.3/src/hdict/content/argument/sample.py` & `hdict-1.230706.1/src/hdict/content/argument/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     [2 -4 8]
     """
 
     sampleable = True
 
     def __init__(self, *values: list[int | float], rnd: int | Random = 0, maxdigits=28):
         self.rnd = rnd
-        # TODO: accept list of non numeric types (categoric)?
+        # todo: : accept list of non numeric types (categoric)?
         prog = list2progression(values, maxdigits=maxdigits)
         if prog.n.is_infinite():  # pragma: no cover
             raise Exception(f"Cannot sample from an infinite list: {prog}")
         self.values = prog
 
     def sample(self, rnd: int | Random = None):
         if rnd is None:
```

### Comparing `hdict-0.230412.3/src/hdict/content/aux_value.py` & `hdict-1.230706.1/src/hdict/content/aux_value.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
 import dis
 import re
 from collections import OrderedDict
-from inspect import signature
+from inspect import signature, isbuiltin, isclass
 from pickle import dumps
 
 from hosh import Hosh, ø
 
 
 def v2hosh(value: object) -> Hosh:
     """
@@ -47,19 +47,19 @@
     My-custom-identifier-arbitrarily-defined
     """
     if hasattr(value, "hosh"):
         return value.hosh
     else:
         try:
             if callable(value):
-                value = f2hosh(value)
+                return f2hosh(value)
             # REMINDER: pickle is the fastest serialization
             return Hosh(dumps(value, protocol=5))
         except TypeError as e:  # pragma: no cover
-            raise Exception(f"Cannot pickle. Pickling is needed to hosh idict values ({value}): {e}")
+            raise Exception(f"Cannot pickle. Pickling is needed to hosh hdict values ({value}): {e}")
 
 
 def f2hosh(function: callable):
     """
     Convert a function to a hosh object.
 
     Adopt pickle(bytecode) for hoshfication because it is faster than other serializations of bytecode.
@@ -69,14 +69,16 @@
     vD8.I-NU3x5hzmj-m1EJgeAIE-.H.HGnWxqvZng0
     >>> fun.hosh = ø * "My-custom-identifier-arbitrarily-defined"
     >>> print(f2hosh(fun))
     My-custom-identifier-arbitrarily-defined
     """
     if hasattr(function, "hosh"):
         return function.hosh
+    if isbuiltin(function) or isclass(function):
+        return Hosh(str(function).encode())
     fields_and_params = signature(function).parameters.values()
     fields_and_params = {v.name: None if v.default is v.empty else v.default for v in fields_and_params}
 
     # Remove line numbers.
     groups = [l for l in dis.Bytecode(function).dis().split("\n\n") if l]
     clean_lines = [fields_and_params]
```

### Comparing `hdict-0.230412.3/src/hdict/content/entry/__init__.py` & `hdict-1.230706.1/src/hdict/content/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/entry/aux_closure.py` & `hdict-1.230706.1/src/hdict/content/entry/aux_closure.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/entry/cached.py` & `hdict-1.230706.1/src/hdict/content/entry/cached.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/entry/closure.py` & `hdict-1.230706.1/src/hdict/content/entry/closure.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         from hdict.data.aux_frozendict import handle_item
 
         self.application = application
         self.out = out
         self.torepr = {}
         hosh = ø
         arg = None
-        fargs, fkwargs, discarded_defaults = {}, {}, set()
-        sorted_fargs = zip(map(str, application.fargs), application.fargs.items())
-        for idx, tup in sorted(chain(sorted_fargs, application.fkwargs.items())):  # We sort by keys for a deterministic hosh.
+        fargs, fkwargs, discarded_defaults = application.fargs.copy(), {}, set()  # We copy fargs to keep args order.
+        sortable_fargs = zip(map(str, fargs), fargs.items())
+        for idx, tup in sorted(chain(sortable_fargs, application.fkwargs.items())):  # We sort by keys for a deterministic hosh.
             if isinstance(tup, tuple):
                 key, val = tup
                 arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr)
                 fargs[key] = arg
             else:
                 key, val = idx, tup
                 arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr)
@@ -60,15 +60,15 @@
         self.hosh = hosh
         self.discarded_defaults = discarded_defaults
 
     @property
     def value(self):
         if isinstance(self._value, Unevaluated):
             self._value = self.f()
-            # del self.application  # TODO: delete clasure.application inside each subvalue?
+            # del self.application  # todo: : delete clasure.application inside each subvalue?
         return self._value
 
     def __repr__(self, out=None):
         from hdict import value
         from hdict import field
         from hdict.content.entry.wrapper import Wrapper
```

### Comparing `hdict-0.230412.3/src/hdict/content/entry/subvalue.py` & `hdict-1.230706.1/src/hdict/content/entry/subvalue.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     index: int
     n: int
     source: str = None
 
     # target: str = None
 
     def __post_init__(self):
-        self.hosh = self.parent.hosh[self.index : self.n]
+        self.hosh = self.parent.hosh[self.index, self.n]
 
     @property
     def value(self):
         from hdict.content.entry import Unevaluated
 
         if isinstance(self._value, Unevaluated):
             value = self.parent.value
```

### Comparing `hdict-0.230412.3/src/hdict/content/entry/wrapper.py` & `hdict-1.230706.1/src/hdict/content/entry/wrapper.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/content/value.py` & `hdict-1.230706.1/src/hdict/content/value.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/data/aux_frozendict.py` & `hdict-1.230706.1/src/hdict/data/aux_frozendict.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 
 
 def handle_items(*datas: [Dict[str, object]], previous: [Dict[str, AbsEntry]]):
     result = previous.copy()
     result__mirror_fields = {}
     for key, item in chain(*(data.items() for data in datas)):
         entry = handle_item(key, item, result)
-        if isinstance(key, str) and key.endswith("_") and isinstance(entry, value):
-            result__mirror_fields[f"{key[:-1]}"] = value(entry.hdict, entry.hosh)
+        if isinstance(key, str) and key.endswith("_"):
+            if isinstance(entry, value):
+                result__mirror_fields[f"{key[:-1]}"] = value(entry.hdict, entry.hdict.hosh)
+            else:
+                raise Exception(f"lazy mirror?")  # todo:
         if isinstance(entry, dict):
             result.update(entry)
         else:
             result[key] = entry
     result.update(result__mirror_fields)
     return result
 
@@ -63,24 +66,28 @@
         case ApplyOut():  # pragma: no cover
             raise Exception("Cannot assign output through both apply and dict-key: '>> {out: apply(...)(out)}'.")
         case AbsAny():  # pragma: no cover
             raise Exception(f"Cannot handle instance of type '{type(item).__name__}'.")
         case _ if str(type(item)) == "<class 'pandas.core.frame.DataFrame'>":
             from hdict.dataset.pandas_handling import explode_df
 
-            res = explode_df(item)
+            # todo: check if this is the best default way of handling DFs.
+            df = item.copy(deep=False)
+            d = explode_df(df)
+            df.__dict__["ashdict"] = d
+            res = value(df, hosh=d.hosh.rev, hdict=d)
         case _:
             res = value(item)
 
     if isinstance(key, tuple):
         return handle_multioutput(key, res, previous)
     elif not isinstance(key, str):  # pragma: no cover
         raise Exception(f"Invalid type for input field specification: {type(key).__name__}")
-    elif key.startswith("_"):  # pragma: no cover
-        raise Exception(f"Field names cannot start with '_': {key}")
+    # elif key.startswith("_"):  # pragma: no cover     # reminder: _* allowed here due to parameter name in getattr(__o)
+    #     raise Exception(f"Field names cannot start with '_': {key}")
 
     return res
 
 
 def handle_identity(data):
     hosh = ø
     ids, later = {}, {}
@@ -89,17 +96,21 @@
         if k.startswith("_"):  # pragma: no cover
             raise Exception("Custom metafields are not allowed:", k)
             # self.mhosh += self.data[k].hosh * k.encode()                # self.mids[k] = self.data[k].hosh.id
         elif k.endswith("_"):
             # mirrorfield, e.g.: 'df_' is a mirror/derived from 'df'
             later[k] = v.id
         else:
-            hosh += v.hosh * k.encode()
-            # PAPER REMINDER: state in the paper that hash(identifier) must be different from hash(value), for any identifier and value. E.g.: hash(X) != hash("X")    #   Here the difference always happen because values are pickled, while identifiers are just encoded().
             ids[k] = v.hosh.id
+        hosh += v.hosh * k.encode()
+        # todo:  PAPER REMINDER: state in the paper that identifiers are not strings. they are a special type that never appears as a value.
+        #   I.e., hash(identifier) must be different from hash(value), for all identifiers and values.
+        #   E.g.: hash(field name X) != hash(string "X")
+        #   In this impementation, the difference is always* true because values are always pickled (they are never hashed as strings), while identifiers are just str.encoded().
+        #   * → probabilistically
     ids.update(later)
     return hosh, ids
 
 
 def handle_multioutput(field_names: tuple, entry: AbsEntry | apply, previous):
     """Fields and hoshes are assigned to each output according to the alphabetical order of the original keys.
 
@@ -128,16 +139,17 @@
             for field_name, (_, val) in zip(field_names, sorted(dct.items())):
                 data[field_name] = handle_item(field_name, val, previous)
         case AbsEntry() | apply():
             keys = []  # For repr().
             parent = Closure(entry, previous, keys) if isinstance(entry, apply) else entry
             n = len(field_names)
             for key, i, source in loop_field_names(field_names):
-                keys.append(key)
-                data[key] = SubValue(parent, i, n, source)
+                if key is not None:
+                    keys.append(key)
+                    data[key] = SubValue(parent, i, n, source)
         case _:  # pragma: no cover
             raise Exception(f"Cannot handle multioutput for key '{field_names}' and type '{type(entry).__name__}'.")
     return data
 
 
 def loop_field_names(field_names):
     if all(isinstance(x, tuple) for x in field_names):
@@ -174,39 +186,39 @@
     >>> from hdict import hdict
     >>> df = hdict(index=[1,2], X=[3,4], y=[5,6]).asdf
     >>> handle_format("Xy", ["X", "y"], df, True).show(colored=False)
     {
         X: "‹{'X': {1: 3, 2: 4}}›",
         y: "‹[0 1]›",
         name: true,
-        _id: Qbcv80d7nEuKex05ecsNrCyQ4d7OI1XsgTWgcCcd,
+        _id: ekKHL1k.UmrpmE3dyQs4T1-kZTt4YNYxm4ptPcNc,
         _ids: {
-            X: oPj-WdtESlEAiUDqGQOUXR-4uwVNfYDl98o042.P,
+            X: UJPgtENMhTLAyrjuPQFGJZDQ2i94vIFqflScHEzP,
             y: cm5S71YBRAlVWV5Yn9pXHzsacyZuEH4ZFDNAw9nu,
             name: oK8X-7eG1Qp1WH7v6fokBDrQPdngKn.h86tlEnx4
         }
     }
     >>> handle_format("df", ["X", "y"], df, True).show(colored=False)
     {
         df: "‹{'X': {1: 3, 2: 4}, 'y': {1: 5, 2: 6}}›",
         name: true,
-        _id: Y8dS5prSxAflQwA0RvutZ.EMDRcyzeZAZCAAuWtT,
+        _id: h3NlgeKfkuO9mCm2Z3N0dlL-Ad-6tjvQWwGXkuXX,
         _ids: {
-            df: taqqcce8-I2nyIyk8LCm4iec0SVkrnbE6FjEvpiS,
+            df: BrLdigqE7urdheEOU6p1l0-jSKPVksJT3zp.lZLW,
             name: oK8X-7eG1Qp1WH7v6fokBDrQPdngKn.h86tlEnx4
         }
     }
     >>> handle_format("Xy", None, df, True).show(colored=False)
     {
         X: "‹{'X': {1: 3, 2: 4}}›",
         y: "‹[0 1]›",
         name: true,
-        _id: Qbcv80d7nEuKex05ecsNrCyQ4d7OI1XsgTWgcCcd,
+        _id: ekKHL1k.UmrpmE3dyQs4T1-kZTt4YNYxm4ptPcNc,
         _ids: {
-            X: oPj-WdtESlEAiUDqGQOUXR-4uwVNfYDl98o042.P,
+            X: UJPgtENMhTLAyrjuPQFGJZDQ2i94vIFqflScHEzP,
             y: cm5S71YBRAlVWV5Yn9pXHzsacyZuEH4ZFDNAw9nu,
             name: oK8X-7eG1Qp1WH7v6fokBDrQPdngKn.h86tlEnx4
         }
     }
     """
     if fields and not isinstance(fields, list):  # pragma: no cover
         raise Exception(f"`fields` must be a list.")
@@ -227,27 +239,7 @@
         d = frozenhdict({fields[0]: dic["X"], fields[1]: dic["y"]})
     else:  # pragma: no cover
         raise Exception(f"Unknown {format=}.")
 
     if name:
         d >>= {"name": name}
     return d
-
-
-# TODO:  fix apply() for *args
-#
-"""
-            f = lambda *args: args[0].asdf
-            return apply(f, field(k), fhosh=ø).enclosure(data, k)
-
-        return apply(f, field(k), fhosh=ø).enclosure(data, k)
-      File "/home/davi/git/hdict/src/hdict/content/argument/apply.py", line 311, in enclosure
-        return Closure(self, data, [key])
-      File "/home/davi/git/hdict/src/hdict/content/entry/closure.py", line 29, in __init__
-        arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr)
-      File "/home/davi/git/hdict/src/hdict/content/entry/aux_closure.py", line 30, in handle_arg
-        arg = handle_item(str(key), data[name], data)  # key passed for no purpose here AFAIR
-      File "/home/davi/git/hdict/src/hdict/data/aux_frozendict.py", line 76, in handle_item
-        raise Exception(f"Field names cannot start with '_': {key}")
-    Exception: Field names cannot start with '_': _0
-
-"""
```

### Comparing `hdict-0.230412.3/src/hdict/data/empty_.py` & `hdict-1.230706.1/src/hdict/data/empty_.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/data/frozenhdict.py` & `hdict-1.230706.1/src/hdict/data/frozenhdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,79 +72,86 @@
     >>> d = {"v": 7} * d
     >>> d.solve().show(colored=False)
     {
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
-        _id: -a24f2g4z-c-tPEss6G8WEd7h8zMopCCsCdQowjL,
+        _id: 0qFPOnULZigyiXU9Jv.1D.XSTIYHZ24UCT00DMHF,
         _ids: {
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
+            z: 2-wfv1b9RyFHB2kdba3EBCy6Do5L-mMPJjT-nfPa
         }
     }
     >>> d = _ >> d
     >>> d.show(colored=False)
     {
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
-        _id: -a24f2g4z-c-tPEss6G8WEd7h8zMopCCsCdQowjL,
+        _id: 0qFPOnULZigyiXU9Jv.1D.XSTIYHZ24UCT00DMHF,
         _ids: {
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
+            z: 2-wfv1b9RyFHB2kdba3EBCy6Do5L-mMPJjT-nfPa
         }
     }
     >>> d = {"a": 5} >> d
     >>> d.show(colored=False)
     {
         a: 5,
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
-        _id: ELQZugqdug6eCOLZSPaimnGqgmhRjJoDLD8cOlYR,
+        _id: jZrJ2CiVUA9OqW.G7dwb3KoaTWGMUmSUVUXn0CkM,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
+            z: 2-wfv1b9RyFHB2kdba3EBCy6Do5L-mMPJjT-nfPa
         }
     }
     >>> from hdict.content.entry import AbsEntry, Unevaluated
     >>> from hdict import frozenhdict
     """
 
     _evaluated = None
     _asdict, _asdicts, _asdicts_noid = None, None, None
+    _hoshes = None
 
     # noinspection PyMissingConstructor
     def __init__(self, /, _dictionary=None, _previous=None, **kwargs):
         from hdict.content.entry import AbsEntry
         from hdict.data.aux_frozendict import handle_identity
         from hdict.data.aux_frozendict import handle_items
 
         if _previous is None:
             _previous = {}
 
-        # TODO: check if _dictionary keys is 'str'; regex to check if k is an identifier;
+        # todo: : check if _dictionary keys is 'str'; regex to check if k is an identifier;
         data = _dictionary or {}
         # REMINDER: Inside data, the only 'dict' entries are "_id" and "_ids", the rest are AbsEntry objects.
         self.data: dict[str, AbsEntry | str | dict[str, str]]
         self.data = handle_items(data, kwargs, previous=_previous)
         self.hosh, self.ids = handle_identity(self.data)
         self.id = self.hosh.id
         self.raw = self.data
 
+    @property
+    def hoshes(self):
+        if self._hoshes is None:
+            self._hoshes = {k: v.hosh for k, v in self.data.items()}
+        return self._hoshes
+
     def __rmul__(self, left):
         from hdict import frozenhdict
         from hdict.expression.step.edict import EDict
         from hdict.expression.expr import Expr
 
         from hdict import hdict
 
@@ -202,15 +209,14 @@
                 dct = {k: Cached(self.ids[k], storage, self.raw[k]) for k in fields}
             case dict():
                 dct = other
             case Expr():
                 return Expr(self, other).solve()
             case _:  # pragma: no cover
                 return NotImplemented
-
         return frozenhdict(dct, _previous=self.data)
 
     def __getitem__(self, item):  # pragma: no cover
         return self.data[item].value
 
     def __getattr__(self, item):  # pragma: no cover
         if item in self.data:
@@ -361,15 +367,15 @@
         return dic, hoshes
 
     def astext(self, colored=True, key_quotes=False):
         r"""Textual representation of a frozenidict object"""
         dicts, hoshes = self.asdicts_hoshes_noneval
         txt = json.dumps(dicts, indent=4, ensure_ascii=False, cls=CustomJSONEncoder)
 
-        # Put colors after json, to avoid escaping ansi codes.  TODO: check how HTML behaves here
+        # Put colors after json, to avoid escaping ansi codes.  todo: check how HTML behaves here
         for h in hoshes:
             txt = txt.replace(f'"{h.id}"', repr(h)) if colored else txt.replace(f'"{h.id}"', h.id)
 
         # Remove quotes.
         txt = re.sub(r'(": )"(λ.+?)"(?=,\n)', '": \\2', txt)  # Closure
         txt = re.sub(r'(": )"(·.+?)"(?=,\n)', '": \\2', txt)  # Wrapper
         txt = re.sub(r'(": )"(↑↓ cached at `.+?·)"(?=,\n)', '": \\2', txt)  # cache
@@ -425,20 +431,26 @@
         from hdict.content.entry.cached import kindid
         from hdict.persistence.stored import Stored
 
         data = {self.id: self.ids}
         for field, fid in self.ids.items():
             value = self[field]
             if field.endswith("_"):
-                # TODO check existence of the counterpart
+                raise Exception(f"Not implemented for mirror fields")
+                # todo:  confirm existence of the counterpart
                 data[kindid(fid)] = str(type(value))
             elif isinstance(value, frozenhdict):
                 value.save(storage)
             else:
                 data[fid] = Stored(value)
+        # todo:  check if frozenhdict is being stored by mistake
+        # todo:  attribute/method as subfield:
+        #       apply(f, _.df.x)            SubField(name="df", attribute="x")
+        #       apply(_.df.drop, "col1")    SubField(name="df", attribute="drop")
+        #
         storage.update(data)
 
     @staticmethod
     def load(id, storage: dict, lazy=True) -> Union["frozenhdict", None]:
         """
         Fetch an entire frozenidict
         """
@@ -468,14 +480,17 @@
 
         if ishdict:
             ids = obj
             data = {}
             mirrored = set()
             for field, fid in ids.items():
                 if field.endswith("_"):
+                    # TODO:  2023-06-23
+                    #  -
+                    raise Exception(f"Not implemented for mirror fields")
                     mirrored.add(field[:-1])
                     continue
                 if lazy:
                     data[field] = Cached(fid, storage)
                 else:
                     obj = frozenhdict.fetch(fid, storage, lazy=False, ishdict=False)
                     if obj is None:  # pragma: no cover
@@ -498,21 +513,21 @@
         from pandas import DataFrame
 
         data = dict(self)
         index = data.pop("index")
         return DataFrame(data, index=index)
 
     @staticmethod
-    def fromfile(name, fields=None, format="df", named=None):
+    def fromfile(name, fields=None, format="df", named=None, hide_types=True):
         r"""
         Input format is defined by file extension: .arff, .csv
         """
         from hdict.data.aux_frozendict import handle_format
 
-        df, name = file2df(name)
+        df, name = file2df(name, hide_types)
         return handle_format(format, fields, df, named and name)
 
     @staticmethod
     def fromtext(text: str, fields=None, format="df", named=None):
         r"""
         Input format is defined by file extension: .arff, .csv
         """
@@ -566,7 +581,13 @@
 
     def __iter__(self):
         for k in self.data:
             yield k
 
     def __hash__(self):
         return hash(self.hosh)
+
+    # def __reduce__(self):
+    # dic = self.data.copy()
+    # del dic["_id"]
+    # del dic["_ids"]
+    # return self.__class__, (dic,)
```

### Comparing `hdict-0.230412.3/src/hdict/data/hdict_.py` & `hdict-1.230706.1/src/hdict/data/hdict_.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import TypeVar, Union
 
 from hdict.data.frozenhdict import frozenhdict
 
 VT = TypeVar("VT")
 
 
-# TODO: finish all '*' combinations and check all '>>' to see when to generate hdict and when to generate Expr.
+# todo: : finish all '*' combinations and check all '>>' to see when to generate hdict and when to generate Expr.
 
 
 class hdict_(dict[str, VT]):
     """
     This class was created only due to slowness of IDE created by excessive doctests in the main file.
 
     >>> from hdict import _, apply
@@ -42,30 +42,30 @@
         _ids: {}
     } » {} » {}⦒
     >>> d = {"x": 3, "f": lambda x: x+1} >> e >> apply(_.f, _.x).x
     >>> d.show(colored=False)  # doctest:+ELLIPSIS
     {
         x: λ(3),
         f: "<function <lambda> at 0x...>",
-        _id: KLOoEeCH2RuCEsOqTVVWLH1JR69eozXUF0xgvVJM,
+        _id: KxAogdPlPbTXATJzW7E8C.4j.82ZIDrVpTbVRxiZ,
         _ids: {
-            x: k0mNmg8iUh4smoL5cs9Xf5HqZY6O6CLHwTFU.UVa,
-            f: LwPloQfKaEYl7z9kNJqrw46sQMASaNgCtBmICRp7
+            x: KeU-dCTjUgnSYGRNrrMMr4i.hg64Dkkfb3c14eh3,
+            f: p-nM7oHlOFr6iHSF9ZISWXc9zqi017c3zcvcV8Dr
         }
     }
     >>> d.x
     4
     >>> d.show(colored=False)  # doctest:+ELLIPSIS
     {
         x: 4,
         f: "<function <lambda> at 0x...>",
-        _id: KLOoEeCH2RuCEsOqTVVWLH1JR69eozXUF0xgvVJM,
+        _id: KxAogdPlPbTXATJzW7E8C.4j.82ZIDrVpTbVRxiZ,
         _ids: {
-            x: k0mNmg8iUh4smoL5cs9Xf5HqZY6O6CLHwTFU.UVa,
-            f: LwPloQfKaEYl7z9kNJqrw46sQMASaNgCtBmICRp7
+            x: KeU-dCTjUgnSYGRNrrMMr4i.hg64Dkkfb3c14eh3,
+            f: p-nM7oHlOFr6iHSF9ZISWXc9zqi017c3zcvcV8Dr
         }
     }
     >>> str({"a": 2} * d)  # doctest:+ELLIPSIS
     '⦑{a: 2} » {x: 4, f: "<function <lambda> at 0x...>"}⦒'
     """
 
     # noinspection PyMissingConstructor
@@ -111,34 +111,34 @@
     def evaluate(self):
         """
         >>> from hdict import apply, hdict
         >>> d = hdict(x=apply(apply(lambda: 2)))
         >>> d.show(colored=False)
         {
             x: λ(),
-            _id: GJC7Qc4lmfpP32nUEG6UAe2fL35KL1wDnubPFgJS,
+            _id: YwRX7paX43aafhz-Jndo9HYnvyMSOtPEbRDjgQ3r,
             _ids: {
-                x: uOjLdXgq4zFpx0Hw7Ofsj1PiXt64oSuLOFpWtD2B
+                x: J746LLRT3gd5glC2ZiaHBgHegmewpiOMC4Sq4bp9
             }
         }
         >>> d.evaluate()
         >>> d.show(colored=False)
         {
             x: 2,
-            _id: GJC7Qc4lmfpP32nUEG6UAe2fL35KL1wDnubPFgJS,
+            _id: YwRX7paX43aafhz-Jndo9HYnvyMSOtPEbRDjgQ3r,
             _ids: {
-                x: uOjLdXgq4zFpx0Hw7Ofsj1PiXt64oSuLOFpWtD2B
+                x: J746LLRT3gd5glC2ZiaHBgHegmewpiOMC4Sq4bp9
             }
         }
         >>> d.evaluated.show(colored=False)
         {
             x: 2,
-            _id: GJC7Qc4lmfpP32nUEG6UAe2fL35KL1wDnubPFgJS,
+            _id: YwRX7paX43aafhz-Jndo9HYnvyMSOtPEbRDjgQ3r,
             _ids: {
-                x: uOjLdXgq4zFpx0Hw7Ofsj1PiXt64oSuLOFpWtD2B
+                x: J746LLRT3gd5glC2ZiaHBgHegmewpiOMC4Sq4bp9
             }
         }
         """
         self.frozen.evaluate()
 
     @property
     def hosh(self):
@@ -307,38 +307,38 @@
                 z: 9,
                 _id: izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM,
                 _ids: {
                     z: GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj
                 }
             },
             w: λ(x y),
-            _id: s3aPQRspwLR81It8zlXsD3Da1Gg76DGSDe841d0b,
+            _id: Jf8QtLAszezNdiqblJCXMuoXocCWZ90QwrxY90Zu,
             _ids: {
                 x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
                 y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
                 z: izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM,
-                w: vo3qMHk3Ef-O065cO-sb4MLHq69x6bKSU694sREJ
+                w: NjWbIhEnN3s8E-w61pptxBuiYmqQ2D3QNX2ZAEB1
             }
         }
         >>> d.save(storage)
         >>> storage
-        {'izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM': {'z': 'GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj'}, 'GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj': Stored(content=9), 's3aPQRspwLR81It8zlXsD3Da1Gg76DGSDe841d0b': {'x': 'KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr', 'y': 'eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf', 'z': 'izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM', 'w': 'vo3qMHk3Ef-O065cO-sb4MLHq69x6bKSU694sREJ'}, 'KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr': Stored(content=3), 'eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf': Stored(content=7), 'vo3qMHk3Ef-O065cO-sb4MLHq69x6bKSU694sREJ': Stored(content=0.42857142857142855)}
+        {'izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM': {'z': 'GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj'}, 'GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj': Stored(content=9), 'Jf8QtLAszezNdiqblJCXMuoXocCWZ90QwrxY90Zu': {'x': 'KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr', 'y': 'eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf', 'z': 'izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM', 'w': 'NjWbIhEnN3s8E-w61pptxBuiYmqQ2D3QNX2ZAEB1'}, 'KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr': Stored(content=3), 'eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf': Stored(content=7), 'NjWbIhEnN3s8E-w61pptxBuiYmqQ2D3QNX2ZAEB1': Stored(content=0.42857142857142855)}
         >>> e = hdict.load(d.id, storage)
         >>> e.show(colored=False)
         {
             x: ↑↓ cached at `dict`·,
             y: ↑↓ cached at `dict`·,
             z: ↑↓ cached at `dict`·,
             w: ↑↓ cached at `dict`·,
-            _id: s3aPQRspwLR81It8zlXsD3Da1Gg76DGSDe841d0b,
+            _id: Jf8QtLAszezNdiqblJCXMuoXocCWZ90QwrxY90Zu,
             _ids: {
                 x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
                 y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
                 z: izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM,
-                w: vo3qMHk3Ef-O065cO-sb4MLHq69x6bKSU694sREJ
+                w: NjWbIhEnN3s8E-w61pptxBuiYmqQ2D3QNX2ZAEB1
             }
         }
         >>> d.w
         0.42857142857142855
         >>> e.w
         0.42857142857142855
         >>> e.evaluate()
@@ -346,20 +346,20 @@
         {
             x: 3,
             y: 7,
             z: {
                 z: 9
             },
             w: 0.42857142857142855,
-            _id: s3aPQRspwLR81It8zlXsD3Da1Gg76DGSDe841d0b,
+            _id: Jf8QtLAszezNdiqblJCXMuoXocCWZ90QwrxY90Zu,
             _ids: {
                 x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
                 y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
                 z: izn67XbX0tQNF6E5qkwniN2jxZg5MT6f7z5AJzPM,
-                w: vo3qMHk3Ef-O065cO-sb4MLHq69x6bKSU694sREJ
+                w: NjWbIhEnN3s8E-w61pptxBuiYmqQ2D3QNX2ZAEB1
             }
         }
         """
         self.frozen.save(storage)
 
     @staticmethod
     def fetch(id: str, storage: dict, lazy=True, ishdict=False) -> Union["hdict_", None]:
@@ -369,137 +369,109 @@
         When cache is a list, traverse it from the end (right item to the left item).
 
         >>> from hdict import hdict, cache
         >>> from testfixtures import TempDirectory
         >>> arff = "@RELATION mini\n@ATTRIBUTE attr1	REAL\n@ATTRIBUTE attr2 	REAL\n@ATTRIBUTE class 	{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1"
         >>> with TempDirectory() as tmp:  # doctest:+ELLIPSIS
         ...    tmp.write("mini.arff", arff.encode())
-        ...    d = hdict.fromfile(tmp.path + "/mini.arff", fields=["df_"])
+        ...    d = hdict.fromfile(tmp.path + "/mini.arff", fields=["df"])
         '/tmp/.../mini.arff'
         >>> d.show(colored=False)
         {
-            df_: "‹{'attr1@REAL': {0: 5.1, 1: 3.1}, 'attr2@REAL': {0: 3.5, 1: 4.5}, 'class@{0,1}': {0: '0', 1: '1'}}›",
-            df: {
-                index: "‹{0: 0, 1: 1}›",
-                "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
-                "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
-                "class@{0,1}": "‹{0: '0', 1: '1'}›",
-                _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                _ids: {
-                    index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
-                    "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
-                    "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
-                    "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
-                }
-            },
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+            df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: '0', 1: '1'}}›",
+            _id: lV4eqST0pTJL.B3GB4Njtv.P1P2aS5EcuQrjnrdX,
             _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                df_: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+                df: rq05QYjRDa4F3kJfE4P8USt4ngF.3skHvVOU5aUt
             }
         }
         >>> storage = {}
         >>> d.save(storage)
         >>> d = hdict.fetch(d.id, storage)
         >>> d.show(colored=False)
         {
             df: ↑↓ cached at `dict`·,
-            df_: λ(df=↑↓ cached at `dict`·),
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
-            _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                df_: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
-            }
-        }
-        >>> d.df_
-           attr1@REAL  attr2@REAL class@{0,1}
-        0         5.1         3.5           0
-        1         3.1         4.5           1
-        >>> d.df.show(colored=False)
-        {
-            index: "‹{0: 0, 1: 1}›",
-            "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
-            "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
-            "class@{0,1}": "‹{0: '0', 1: '1'}›",
-            _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-            _ids: {
-                index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
-                "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
-                "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
-                "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
-            }
-        }
-        >>> d = hdict.fetch(d.id, storage, lazy=False)
-        >>> d.show(colored=False)
-        {
-            df: {
-                index: "‹{0: 0, 1: 1}›",
-                "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
-                "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
-                "class@{0,1}": "‹{0: '0', 1: '1'}›",
-                _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                _ids: {
-                    index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
-                    "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
-                    "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
-                    "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
-                }
-            },
-            df_: λ({    i···),
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
-            _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                df_: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
-            }
-        }
-        >>> del d["df_"]
-        >>> d.show(colored=False)
-        {
-            df: {
-                index: "‹{0: 0, 1: 1}›",
-                "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
-                "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
-                "class@{0,1}": "‹{0: '0', 1: '1'}›",
-                _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                _ids: {
-                    index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
-                    "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
-                    "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
-                    "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
-                }
-            },
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
-            _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
-            }
-        }
-        >>> d.save(storage)
-        >>> d = hdict.fetch(d.id, storage, lazy=False)
-        >>> d.show(colored=False)
-        {
-            df: {
-                index: "‹{0: 0, 1: 1}›",
-                "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
-                "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
-                "class@{0,1}": "‹{0: '0', 1: '1'}›",
-                _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
-                _ids: {
-                    index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
-                    "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
-                    "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
-                    "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
-                }
-            },
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+            _id: lV4eqST0pTJL.B3GB4Njtv.P1P2aS5EcuQrjnrdX,
             _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+                df: rq05QYjRDa4F3kJfE4P8USt4ngF.3skHvVOU5aUt
             }
         }
-        >>> str(d)
-        '{df: {index: "‹{0: 0, 1: 1}›", attr1@REAL: "‹{0: 5.1, 1: 3.1}›", attr2@REAL: "‹{0: 3.5, 1: 4.5}›", class@{0,1}: "‹{0: \'0\', 1: \'1\'}›"}}'
+        >>> d.df
+           attr1  attr2 class
+        0    5.1    3.5     0
+        1    3.1    4.5     1
+
+        # >>> #d.df.show(colored=False)
+        # >>> d = hdict.fetch(d.id, storage, lazy=False)
+        # >>> d.show(colored=False)
+        # {
+        #     df: {
+        #         index: "‹{0: 0, 1: 1}›",
+        #         "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
+        #         "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
+        #         "class@{0,1}": "‹{0: '0', 1: '1'}›",
+        #         _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
+        #         _ids: {
+        #             index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
+        #             "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
+        #             "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
+        #             "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
+        #         }
+        #     },
+        #     df_: λ({    i···),
+        #     _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+        #     _ids: {
+        #         df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
+        #         df_: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+        #     }
+        # }
+        # >>> #del d["df_"]
+        # >>> d.show(colored=False)
+        # {
+        #     df: {
+        #         index: "‹{0: 0, 1: 1}›",
+        #         "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
+        #         "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
+        #         "class@{0,1}": "‹{0: '0', 1: '1'}›",
+        #         _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
+        #         _ids: {
+        #             index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
+        #             "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
+        #             "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
+        #             "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
+        #         }
+        #     },
+        #     _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+        #     _ids: {
+        #         df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+        #     }
+        # }
+        # >>> d.save(storage)
+        # >>> d = hdict.fetch(d.id, storage, lazy=False)
+        # >>> d.show(colored=False)
+        # {
+        #     df: {
+        #         index: "‹{0: 0, 1: 1}›",
+        #         "attr1@REAL": "‹{0: 5.1, 1: 3.1}›",
+        #         "attr2@REAL": "‹{0: 3.5, 1: 4.5}›",
+        #         "class@{0,1}": "‹{0: '0', 1: '1'}›",
+        #         _id: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J,
+        #         _ids: {
+        #             index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
+        #             "attr1@REAL": wsy0JDrZO04O0RVwr64jpawX62WmCKtddYdvZlwm,
+        #             "attr2@REAL": LvEgUazJoB1-.A3kABbskN-.iauWmWLTTo1iC51n,
+        #             "class@{0,1}": b.kJy3SrU-JQ1oeh1d.uWLO7Pqh-eW6zwK78nTY4
+        #         }
+        #     },
+        #     _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+        #     _ids: {
+        #         df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+        #     }
+        # }
+        # >>> str(d)
+        # '{df: {index: "‹{0: 0, 1: 1}›", attr1@REAL: "‹{0: 5.1, 1: 3.1}›", attr2@REAL: "‹{0: 3.5, 1: 4.5}›", class@{0,1}: "‹{0: \'0\', 1: \'1\'}›"}}'
         """
         return frozenhdict.fetch(id, storage, lazy, ishdict).unfrozen
 
     @staticmethod
     def load(id, storage: dict):
         """
         Fetch an entire hdict
@@ -527,73 +499,73 @@
                 x: 1234567890123456789012345678901234567890
             }
         }
         """
         return frozenhdict.load(id, storage).unfrozen
 
     @staticmethod
-    def fromfile(name, fields=None, format="df", named=None):
+    def fromfile(name, fields=None, format="df", named=None, hide_types=True):
         r"""
         Input format is defined by file extension: .arff, .csv
 
         >>> from hdict import hdict
         >>> from testfixtures import TempDirectory
         >>> arff = "@RELATION mini\n@ATTRIBUTE attr1	REAL\n@ATTRIBUTE attr2 	REAL\n@ATTRIBUTE class 	{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1"
         >>> with TempDirectory() as tmp:  # doctest:+ELLIPSIS
         ...    tmp.write("mini.arff", arff.encode())
         ...    d = hdict.fromfile(tmp.path + "/mini.arff")
         '/tmp/.../mini.arff'
         >>> d.show(colored=False)
         {
-            df: "‹{'attr1@REAL': {0: 5.1, 1: 3.1}, 'attr2@REAL': {0: 3.5, 1: 4.5}, 'class@{0,1}': {0: '0', 1: '1'}}›",
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+            df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: '0', 1: '1'}}›",
+            _id: lV4eqST0pTJL.B3GB4Njtv.P1P2aS5EcuQrjnrdX,
             _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+                df: rq05QYjRDa4F3kJfE4P8USt4ngF.3skHvVOU5aUt
             }
         }
         >>> csv = "attr1,attr2,class\n5.1,3.5,0\n3.1,4.5,1"
         >>> with TempDirectory() as tmp:  # doctest:+ELLIPSIS
         ...    tmp.write("mini.csv", csv.encode())
         ...    d = hdict.fromfile(tmp.path + "/mini.csv")
         '/tmp/.../mini.csv'
         >>> d.show(colored=False)
         {
             df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: 0, 1: 1}}›",
-            _id: X4CDIwtBn8BiF71hNG5JeISRQcVffsy.7UWv16IX,
+            _id: X5OQYZSPdJyyE0sSuSRbkfqVuKyd1zppSAhb6EQd,
             _ids: {
-                df: Cr4zP7wsqcNFjkkfcGvy7nV4oTh5tOeu9Zh5MQmu
+                df: SOhTT4S1x3Tfct.v4Fi7QhjacZWya06UT18MQmvM
             }
         }
         """
-        return frozenhdict.fromfile(name, fields, format, named).unfrozen
+        return frozenhdict.fromfile(name, fields, format, named, hide_types).unfrozen
 
     @staticmethod
     def fromtext(text: str, fields=None, format="df", named=None):
         r"""
         Input format is defined by file extension: .arff, .csv
 
         >>> from hdict import hdict
         >>> arff = "@RELATION mini\n@ATTRIBUTE attr1	REAL\n@ATTRIBUTE attr2 	REAL\n@ATTRIBUTE class 	{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1"
         >>> d = hdict.fromtext(arff)
         >>> d.show(colored=False)
         {
             df: "‹{'attr1@REAL': {0: 5.1, 1: 3.1}, 'attr2@REAL': {0: 3.5, 1: 4.5}, 'class@{0,1}': {0: '0', 1: '1'}}›",
-            _id: CWkreYbSmrL0DPN9OtoU4Za1dg8.Jjl.fXD6yblb,
+            _id: CukZPsWIhD.itTmQB6-7svrjNtrRJjwm2lJwNp2x,
             _ids: {
-                df: cHrG-npBDd2VEB8Foeg.7jQNZtdkTM1uhouHgW.J
+                df: sZ.7F68Bw2uV6jehdOpmzOK7-mWGXFcR3q46w8J3
             }
         }
         >>> csv = "attr1,attr2,class\n5.1,3.5,0\n3.1,4.5,1"
         >>> d = hdict.fromtext(csv)
         >>> d.show(colored=False)
         {
             df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: 0, 1: 1}}›",
-            _id: X4CDIwtBn8BiF71hNG5JeISRQcVffsy.7UWv16IX,
+            _id: X5OQYZSPdJyyE0sSuSRbkfqVuKyd1zppSAhb6EQd,
             _ids: {
-                df: Cr4zP7wsqcNFjkkfcGvy7nV4oTh5tOeu9Zh5MQmu
+                df: SOhTT4S1x3Tfct.v4Fi7QhjacZWya06UT18MQmvM
             }
         }
         """
         return frozenhdict.fromtext(text, fields, format, named).unfrozen
 
     @property
     def asdf(self):
@@ -605,7 +577,14 @@
         >>> d.asdf
            x  y
         a  1  5
         b  2  6
         c  3  7
         """
         return self.frozen.asdf
+
+    @property
+    def hoshes(self):
+        return self.frozen.hoshes
+
+    # def __reduce__(self):
+    # return self.frozen.__reduce__()
```

### Comparing `hdict-0.230412.3/src/hdict/dataset/dataset.py` & `hdict-1.230706.1/src/hdict/dataset/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -114,35 +114,90 @@
             attrs.append((attr[0], attr[1]))
 
     data = list(df.values)
     result = {"attributes": attrs, "data": data, "description": description, "relation": relation}
     return result
 
 
-# def dump(df, fp):  # TODO: save arff/CSV from hdict
+# def dump(df, fp):  # todo: : save arff/CSV from hdict
 #     import arff as liacarff
 #
 #     arff = df2liac(df)
 #     liacarff.dump(arff, fp)
 #
 #
-# def dumps(df):  # TODO: output arff/CSV from hdict
+# def dumps(df):  # todo: : output arff/CSV from hdict
 #     import arff as liacarff
 #
 #     arff = df2liac(df)
 #     return liacarff.dumps(arff)
 
 
-def df2Xy(df):
-    from sklearn.preprocessing import LabelEncoder
-
-    le = LabelEncoder()
-    X_ = df.drop(df.columns[[-1]], axis=1)
-    y_ = le.fit_transform(df[df.columns[-1]])
-    return {"X": X_, "y": y_}
+def df2Xy(df, target=None):
+    r"""
+    >>> from hdict import hdict
+    >>> from hdict.dataset.dataset import df2Xy
+    >>> from testfixtures import TempDirectory
+    >>> arff = "@RELATION mini\n@ATTRIBUTE attr1	REAL\n@ATTRIBUTE attr2 	REAL\n@ATTRIBUTE class 	{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1"
+    >>> with TempDirectory() as tmp:  # doctest:+ELLIPSIS
+    ...    tmp.write("mini.arff", arff.encode())
+    ...    d = hdict.fromfile(tmp.path + "/mini.arff")
+    '/tmp/.../mini.arff'
+    >>> df2Xy(d.df)
+    {'X':    attr1  attr2
+    0    5.1    3.5
+    1    3.1    4.5, 'y': array([0, 1])}
+    >>> df2Xy(d.df, target="attr2")
+    {'X':    attr1 class
+    0    5.1     0
+    1    3.1     1, 'y': 0    3.5
+    1    4.5
+    Name: attr2, dtype: float64}
+    """
+    if target is None:
+        from sklearn.preprocessing import LabelEncoder
+
+        le = LabelEncoder()
+        X = df.drop(df.columns[[-1]], axis=1)
+        y = le.fit_transform(df[df.columns[-1]])
+    else:
+        y = df[target]
+        X = df.drop(target, axis=1)
+    return {"X": X, "y": y}
+
+
+def nom2bin(X, nomcols):
+    """
+    >>> import numpy as np
+    >>> from pandas import DataFrame as DF
+    >>> X = DF(np.array([[0, "a", 1.6], [3.2, "b", 2], [8, "c", 3]]))
+    >>> X
+         0  1    2
+    0    0  a  1.6
+    1  3.2  b    2
+    2    8  c    3
+    >>> nom2bin(X, nomcols=[1])
+         0    2  1_a  1_b  1_c
+    0    0  1.6    1    0    0
+    1  3.2    2    0    1    0
+    2    8    3    0    0    1
+    """
+    if X.__class__.__name__ in ["DataFrame", "Series"]:
+        import pandas
+
+        clabels = X.columns[nomcols]
+        return pandas.get_dummies(X, prefix=clabels, columns=clabels, dtype=int)
+    else:
+        import numpy
+        from sklearn.preprocessing import OneHotEncoder
+
+        encoder = OneHotEncoder()
+        nom = encoder.fit_transform(X.iloc[:, nomcols] if hasattr(X, "iloc") else X[:, nomcols]).toarray()
+        num = numpy.delete(X, nomcols, axis=1).astype(float)
+        return numpy.column_stack((nom, num))
 
 
 #
 #
 # def df2arff(input="df", output="arff", **kwargs):
 #     """
 #     >>> from idict import let, idict
```

### Comparing `hdict-0.230412.3/src/hdict/dataset/pandas_handling.py` & `hdict-1.230706.1/src/hdict/dataset/pandas_handling.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
-from hdict.content.value import value
 
 
-def explode_df(df) -> value:
+def explode_df(df):
     """
     >>> from pandas import DataFrame
     >>> from hdict import hdict, cache
     >>> df = DataFrame({"x": [1,2,3], "y": [5,6,7]}, index=["a", "b", "c"])
     >>> d = hdict(df_=df)
     >>> d.show(colored=False)
     {
@@ -39,18 +38,18 @@
             _id: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC,
             _ids: {
                 index: HBNoEs58wCDhsdWWisp0sjMwsWmNMXuwaGFE9UAt,
                 x: 3F.7UkfLr2tpB-FxATaRJYIpbYpg9oa1r5M31M0j,
                 y: bqYjHGDn-brebdANtxtNo4OkpOXfDwwVYejlzo4t
             }
         },
-        _id: qMP.-f8p3zIrmTuOOqBLCVurT6uIIfihnR3rZne4,
+        _id: aeZiHhtCekhlDKPjI1odXiO-beLTbpUeMO.jzWtS,
         _ids: {
             df: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC,
-            df_: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC
+            df_: Cem6iaHrGtpk5R64.TcbqxhNgRv-dmfUZwoJJGZI
         }
     }
     >>> d.df_
        x  y
     a  1  5
     b  2  6
     c  3  7
@@ -66,18 +65,18 @@
             _id: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC,
             _ids: {
                 index: HBNoEs58wCDhsdWWisp0sjMwsWmNMXuwaGFE9UAt,
                 x: 3F.7UkfLr2tpB-FxATaRJYIpbYpg9oa1r5M31M0j,
                 y: bqYjHGDn-brebdANtxtNo4OkpOXfDwwVYejlzo4t
             }
         },
-        _id: qMP.-f8p3zIrmTuOOqBLCVurT6uIIfihnR3rZne4,
+        _id: aeZiHhtCekhlDKPjI1odXiO-beLTbpUeMO.jzWtS,
         _ids: {
             df: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC,
-            df_: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC
+            df_: Cem6iaHrGtpk5R64.TcbqxhNgRv-dmfUZwoJJGZI
         }
     }
     >>> d.df.show(colored=False)
     {
         index: "‹{'a': 'a', 'b': 'b', 'c': 'c'}›",
         x: "‹{'a': 1, 'b': 2, 'c': 3}›",
         y: "‹{'a': 5, 'b': 6, 'c': 7}›",
@@ -86,35 +85,42 @@
             index: HBNoEs58wCDhsdWWisp0sjMwsWmNMXuwaGFE9UAt,
             x: 3F.7UkfLr2tpB-FxATaRJYIpbYpg9oa1r5M31M0j,
             y: bqYjHGDn-brebdANtxtNo4OkpOXfDwwVYejlzo4t
         }
     }
     """
     from hdict.data.frozenhdict import frozenhdict
-    from hdict import value
 
     dic = {"index": df.index.to_series()}
     for col in df:
         dic[str(col)] = df[col]
     d = frozenhdict(dic)
-    return value(df, d.hosh, hdict=d)  # `value.hdict` points to `d`.
+    return d
 
 
-def file2df(name):
+def file2df(filename, hide_types=True, return_name=True):
     from hdict.dataset.dataset import load
 
-    if name.endswith(".arff"):
+    if filename.endswith(".arff"):
         relation = None
-        with open(name) as f:
+        with open(filename) as f:
             for line in f:
                 if line[:9].upper() == "@RELATION":
                     relation = line[9:-1]
                     break
-        with open(name) as f:
+        with open(filename) as f:
             df = load(f)
-        return df, relation or name
-    elif name.endswith(".csv"):
+        if hide_types:
+            df.rename(columns={k: k.split("@")[0] for k in df.columns}, inplace=True)
+        if return_name:
+            return df, relation or filename
+        else:
+            return df
+    elif filename.endswith(".csv"):
         from pandas import read_csv
 
-        return read_csv(name), name
+        if return_name:
+            return read_csv(filename), filename
+        else:
+            return read_csv(filename)
     else:  # pragma: no cover
-        raise Exception(f"Unknown extension {name.split('.')[-1]}.")
+        raise Exception(f"Unknown extension {filename.split('.')[-1]}.")
```

### Comparing `hdict-0.230412.3/src/hdict/expression/expr.py` & `hdict-1.230706.1/src/hdict/expression/expr.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/expression/step/applyout.py` & `hdict-1.230706.1/src/hdict/expression/step/applyout.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     ⦑{} » a=λ(x=~[1 2 .+. 9]) » ↑↓`dict` » {s: "~[1 2 .+. 9]"}⦒
     >>> e.steps[0].steps[1].sampleable
     True
     >>> (~e).show(colored=False)
     {
         a: ↑↓ cached at `dict`·,
         s: 7,
-        _id: J2CPNGfxvEaLcJSy1sA2WAlmGyFDjXkor.DkEGpl,
+        _id: E3YKpiQXWwK1AZh9BcqI7AoamBanxAr1GAOeJudy,
         _ids: {
-            a: 8v.MUDWXtCirIrM97YgzEDDrmIAbmlWqkrhZMWPS,
+            a: ygBt7xenihJVMnjwJxN6Z1H7HYnrET04zEYTRKD3,
             s: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf
         }
     }
     """
 
     nested: apply
     out: [str | tuple[str, str]]
```

### Comparing `hdict-0.230412.3/src/hdict/expression/step/cache.py` & `hdict-1.230706.1/src/hdict/expression/step/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,45 +30,45 @@
     >>> storage = {}
     >>> d = hdict(x=3, y=5) >> apply(lambda x, y: x / y).z
     >>> d.show(colored=False)
     {
         x: 3,
         y: 5,
         z: λ(x y),
-        _id: UB8No.x9HiKWeFqpmTv1lWn0lEsTJS16lPNCojcK,
+        _id: IIh20mb2BGUx9XMCDwzTr4y7v-JaGin3eEHvx692,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: cszQVZnzMQSS3.2tdWWQL-wGCv.lO0TWqVoSNFww
+            z: GC-BMZNVRagHxgUynUadKUYA1kZ8GzcUj6OKWstQ
         }
     }
     >>> d >>= cache(storage)
     >>> d.show(colored=False)
     {
         x: 3,
         y: 5,
         z: ↑↓ cached at `dict`·,
-        _id: UB8No.x9HiKWeFqpmTv1lWn0lEsTJS16lPNCojcK,
+        _id: IIh20mb2BGUx9XMCDwzTr4y7v-JaGin3eEHvx692,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: cszQVZnzMQSS3.2tdWWQL-wGCv.lO0TWqVoSNFww
+            z: GC-BMZNVRagHxgUynUadKUYA1kZ8GzcUj6OKWstQ
         }
     }
     >>> d.evaluate()
     >>> d.show(colored=False)
     {
         x: 3,
         y: 5,
         z: 0.6,
-        _id: UB8No.x9HiKWeFqpmTv1lWn0lEsTJS16lPNCojcK,
+        _id: IIh20mb2BGUx9XMCDwzTr4y7v-JaGin3eEHvx692,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            z: cszQVZnzMQSS3.2tdWWQL-wGCv.lO0TWqVoSNFww
+            z: GC-BMZNVRagHxgUynUadKUYA1kZ8GzcUj6OKWstQ
         }
     }
     """
 
     def __init__(self, storage: dict, *fields):
         self.storage = storage
         self.fields = fields
```

### Comparing `hdict-0.230412.3/src/hdict/expression/step/step.py` & `hdict-1.230706.1/src/hdict/expression/step/step.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/persistence/stored.py` & `hdict-1.230706.1/src/hdict/persistence/stored.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230412.3/src/hdict/text/customjson.py` & `hdict-1.230706.1/src/hdict/text/customjson.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,21 +73,21 @@
             _id: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
             _ids: {
                 index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
                 0: 8ianf2LAQlxK7ZFvdOX.avsuK4L9FjUiMC7sM2Lm,
                 1: IIffH-qkWUFB.-VFd0z6BBrIpfvNuc8GPxlQYgg3
             }
         },
-        _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
+        _id: S1nTzl98Gz1FWNCx4PjWyiicvZwwm17VZ.Pk-hbr,
         _ids: {
             d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
             df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
-            df_: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
+            df_: Bzf414aFK2VBHxFEmB4pLGAsKSllj4QcNfm0QC7l
         }
     }
     >>> from numpy import array
     >>> hdict(b=b, z=9, c=(c:=array([1,2,3])), d=Series(c), dd=array([[1, 2], [3, 4]])).show(colored=False)
     {
         b: {
             d: {
@@ -107,30 +107,30 @@
                 _id: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
                 _ids: {
                     index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
                     0: 8ianf2LAQlxK7ZFvdOX.avsuK4L9FjUiMC7sM2Lm,
                     1: IIffH-qkWUFB.-VFd0z6BBrIpfvNuc8GPxlQYgg3
                 }
             },
-            _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
+            _id: S1nTzl98Gz1FWNCx4PjWyiicvZwwm17VZ.Pk-hbr,
             _ids: {
                 d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
                 y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
                 ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
                 df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
-                df_: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
+                df_: Bzf414aFK2VBHxFEmB4pLGAsKSllj4QcNfm0QC7l
             }
         },
         z: 9,
         c: "‹[1 2 3]›",
         d: "‹{0: 1, 1: 2, 2: 3}›",
         dd: "‹[[1 2] [3 4]]›",
-        _id: 75i4qCm0ZAOdRV9TWDeUNQ7GuGmWWMQ8dndlVEsm,
+        _id: Jd3NfEBIPpLs5oPz4VEXkRY38XfsvE.qp37xB7SM,
         _ids: {
-            b: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
+            b: S1nTzl98Gz1FWNCx4PjWyiicvZwwm17VZ.Pk-hbr,
             z: GuwIQCrendfKXZr5jGfrUwoP-8TWMhmLHYrja2yj,
             c: QkfVsy7ITAmoIiOFgbYpsQodBSIYshhiUm3v2r8d,
             d: 5iU-DAFL3XTLno88g056s2G12RidCKkCgLCLIwB5,
             dd: fVj30baMeet4PcN9ZY-8uMpFin89FY8h8MI4RkDd
         }
     }
     >>> hdict(s={1,3,2}, t={3,1,2}, u={2,1,3}, v={2,1,3}).show(colored=False)
@@ -159,15 +159,17 @@
             # if isinstance(obj, Idict):
             #     return obj.frozen.asdicts
             # if isinstance(obj, FrozenIdict):
             #     return obj.asdicts
             if obj is Ellipsis:
                 return "..."
             if isinstance(obj, AbsEntry) and obj.isevaluated:
-                if isinstance(obj.value, dict):
+                from hdict import hdict, frozenhdict
+
+                if isinstance(obj.value, (frozenhdict, hdict)):
                     return obj.value.asdicts_noid
                 return obj.value
             # if isinstance(obj, FunctionType):
             #     return str(obj)
             if not isinstance(obj, (dict, list, str, int, float, bytearray, bool)):
                 if type(obj).__name__ in ["DataFrame", "Series"]:
                     # ‹str()› is to avoid nested identation
```

### Comparing `hdict-0.230412.3/setup.py` & `hdict-1.230706.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,29 @@
  'hdict.persistence',
  'hdict.text']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['hosh>=2.230205.2,<3.0.0', 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0']
+['hosh>=3.230705.2,<4.0.0', 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0']
 
 extras_require = \
 {'full': ['pandas>=2.0.0,<3.0.0',
           'shelchemy>=0.220906.3,<0.220907.0',
           'safeserializer>=0.230202.1,<0.230203.0',
           'lz4>=4.3.2,<5.0.0',
           'scikit-learn>=1.2.2,<2.0.0',
           'liac-arff>=2.5.0,<3.0.0']}
 
 setup_kwargs = {
     'name': 'hdict',
-    'version': '0.230412.3',
+    'version': '1.230706.1',
     'description': 'A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.',
-    'long_description': '![test](https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n<a href="https://pypi.org/project/hdict">\n<img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.10...-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\n## Overview\nShortly, `hdict` is a data structure useful for frictionless experiments, distributed data, among others.\nIt can be more formally defined as a hosh¹-based cacheable lazy `dict` with predictable/deterministic universally unique² identifiers.\n\nThis library is stable for the most common scenarios.\nHowever, we will wait for more use in the wild before reaching the major version 1.\nSee the Section Versioning below for more information.\n\n¹ hosh: _Operable HaSH_\n\n² unique: _probabilistically guaranteed_\n\n\n\n### Context\n\n  * [hosh](https://pypi.org/project/hosh): identification engine at the core of `hdict`\n  * previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/garoupa)\n\n### The concept\n\n`hdict` is like an ordinary `dict` with `str` keys. \nEach entry, called _field_, and the `hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/hosh)).\nA `hdict` object (say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field identifiers),\naccessible through square brackets or through the shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n<details>\n<p>\n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict(x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z": 10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7, "z": 10}\n\n# All three options have the same result.\nd.show(colored=False)\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n```python3\n\nfrom hosh import setup\n\n# For better integration within the documentation, we change the color theme.\nsetup(dark_theme=False)\n\nd.show(colored=False)\n\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n\n</p>\n</details>\n\nA field contains a value or a function application.\nA field pointing to an application is only evaluated on demand, i.e., lazily.\n\n<!-- ------------------------------------------------------------------------ \nValue objects can have custom identifiers as well, if provided whithin the entry `ids`. \nOtherwise, identifiers for functions and values will be calculated through blake3 hashing of their content.\nFor functions, the bytecode is used as content.\nFor this reason, such functions should be simple, with minimal external dependencies or\nwith their import statements inside the function body.\nThis decreases the odds of using two functions with identical local code (and, therefore, identical identifiers)\nperforming different calculations.\n\ntransformation steps done through the operator `>>`, which symbolizes the ordering of the steps.\n* **value insertion** - represented by dict-like objects\n* **function application** - represented by ordinary Python functions\n\nFunctions, `hdict`s, and values have a deterministic UUID\n(called _hosh_ - **o**perable **h**a**sh**). \nIdentifiers (hoshes) for `hdict`s and values are predictable through the\nmagic available [here](https://pypi.org/project/garoupa).\nAn `hdict` is completely defined by its key-value pairs so that\nit can be converted from/to a built-in `dict`.\n\n\n------------------------------------------------------------------------  -->\n\nPlease refer to our [website](https://hosh.page) for more examples.\n\n\n## Installation\n### ...as a standalone lib\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI...\npip install --upgrade pip\npip install -U hdict\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)\npip install -U hdict[full]\n\n# ...or, install from updated source code.\npip install git+https://github.com/davips/hdict\n```\n\n### ...from source\n```bash\ngit clone https://github.com/davips/hdict\ncd hdict\npoetry install\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)  \npoetry install -E full\n```\n\n## Examples\n\nPlease refer to our [website](https://hosh.page) for examples.\n\n\n\n## Development\n### Licensing\nThe initial license choosen is GPL. Please contact the developer for other licensing needs.\n\n### Versioning\nWhile the version scheme has a meaningful calendar component (`minor=yymmdd`), it is still compatible with semantic versioning.\nFor instance, the version `0.230215.1` means `major=0`, `minor=230215`, `micro/patch=1`. Notes:\n * While `major=0`, some compatibility-breaking changes may occur.\n * From `major=1` onwards, compatibility-breaking changes increment it, and update the minor version to reflect the release date.\n * New (non breaking) features update only the minor version to reflect the release date.\n * Bug fixes (including compatibility-breaking ones) increment only the micro version.\n\n### Contributing\n#### Collaboration\nWe have ongoing research applying this tool to machine learning and clinical academic experiments.\nAlthough, the scope of application is broad as it encompasses software development in general.\nFeel free to contact us if you are interested in the project/concept or have a suggestion/interesting problem to be solved.\n\n#### Donation\nCurrently there are no established forms of donation.\nExpenses:\n  * Programming hours\n  * Support\n  * Custom features\n  * Domain name maintenance yearly costs\n\n### Acknowledgement\nThis work was based on a previous research supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0)\nuntil 2021-03-31.\n\nWe would like to thank the providers of free tools that make this project feasible:\n  * github for hosting the code repository freely\n  * Oracle for hosting the website freely\n  * Developers of Mint, XFCE, and GNU/Linux for the operating system\n  * JetBrains for Intellij IDEA Community Edition\n  * Developers of Python packages listed in our project.toml\n',
+    'long_description': '![test](https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n<a href="https://pypi.org/project/hdict">\n<img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.10+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\n## Overview\nShortly, `hdict` is a data structure useful for frictionless experiments, distributed data, among others.\nIt can be more formally defined as a hosh¹-based cacheable lazy `dict` with predictable/deterministic universally unique² identifiers.\n\nThis library is stable for the most common scenarios.\nHowever, we will wait for more use in the wild before reaching the major version 1.\nSee the Section Versioning below for more information.\n\n¹ hosh: _Operable HaSH_\n\n² unique: _probabilistically guaranteed_\n\n\n\n### Context\n\n  * [hosh](https://pypi.org/project/hosh): identification engine at the core of `hdict`\n  * previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/garoupa)\n\n### The concept\n\n`hdict` is like an ordinary `dict` with `str` keys. \nEach entry, called _field_, and the `hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/hosh)).\nA `hdict` object (say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field identifiers),\naccessible through square brackets or through the shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n<details>\n<p>\n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict(x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z": 10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7, "z": 10}\n\n# All three options have the same result.\nd.show(colored=False)\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n```python3\n\nfrom hosh import setup\n\n# For better integration within the documentation, we change the color theme.\nsetup(dark_theme=False)\n\nd.show(colored=False)\n\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n\n</p>\n</details>\n\nA field contains a value or a function application.\nA field pointing to an application is only evaluated on demand, i.e., lazily.\n\n<!-- ------------------------------------------------------------------------ \nValue objects can have custom identifiers as well, if provided whithin the entry `ids`. \nOtherwise, identifiers for functions and values will be calculated through blake3 hashing of their content.\nFor functions, the bytecode is used as content.\nFor this reason, such functions should be simple, with minimal external dependencies or\nwith their import statements inside the function body.\nThis decreases the odds of using two functions with identical local code (and, therefore, identical identifiers)\nperforming different calculations.\n\ntransformation steps done through the operator `>>`, which symbolizes the ordering of the steps.\n* **value insertion** - represented by dict-like objects\n* **function application** - represented by ordinary Python functions\n\nFunctions, `hdict`s, and values have a deterministic UUID\n(called _hosh_ - **o**perable **h**a**sh**). \nIdentifiers (hoshes) for `hdict`s and values are predictable through the\nmagic available [here](https://pypi.org/project/garoupa).\nAn `hdict` is completely defined by its key-value pairs so that\nit can be converted from/to a built-in `dict`.\n\n\n------------------------------------------------------------------------  -->\n\nPlease refer to our [website](https://hosh.page) for more examples.\n\n\n## Installation\n### ...as a standalone lib\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI...\npip install --upgrade pip\npip install -U hdict\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)\npip install -U hdict[full]\n\n# ...or, install from updated source code.\npip install git+https://github.com/davips/hdict\n```\n\n### ...from source\n```bash\ngit clone https://github.com/davips/hdict\ncd hdict\npoetry install\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)  \npoetry install -E full\n```\n\n## Examples\n\nPlease refer to our [website](https://hosh.page) for examples.\n\n\n\n## Development\n### Licensing\nThe initial license choosen is GPL. Please contact the developer for other licensing needs.\n\n### Versioning\nWhile the version scheme has a meaningful calendar component (`minor=yymmdd`), it is still compatible with semantic versioning.\nFor instance, the version `0.230215.1` means `major=0`, `minor=230215`, `micro/patch=1`. Notes:\n * While `major=0`, some compatibility-breaking changes may occur.\n * From `major=1` onwards, compatibility-breaking changes increment it, and update the minor version to reflect the release date.\n * New (non breaking) features update only the minor version to reflect the release date.\n * Bug fixes (including compatibility-breaking ones) increment only the micro version.\n\n### Contributing\n#### Collaboration\nWe have ongoing research applying this tool to machine learning and clinical academic experiments.\nAlthough, the scope of application is broad as it encompasses software development in general.\nFeel free to contact us if you are interested in the project/concept or have a suggestion/interesting problem to be solved.\n\n#### Donation\nCurrently there are no established forms of donation.\nExpenses:\n  * Programming hours\n  * Support\n  * Custom features\n  * Domain name maintenance yearly costs\n\n### Acknowledgement\nThis work was based on a previous research supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0)\nuntil 2021-03-31.\n\nWe would like to thank the providers of free tools that make this project feasible:\n  * github for hosting the code repository freely\n  * Oracle for hosting the website freely\n  * Developers of Mint, XFCE, and GNU/Linux for the operating system\n  * JetBrains for Intellij IDEA Community Edition\n  * Developers of Python packages listed in our project.toml\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hdict', 'hdict.abs', 'hdict.content',
 'hdict.content.argument', 'hdict.content.entry', 'hdict.data', 'hdict.dataset',
 'hdict.expression', 'hdict.expression.step', 'hdict.persistence', 'hdict.text']
-package_data = \ {'': ['*']} install_requires = \ ['hosh>=2.230205.2,<3.0.0',
+package_data = \ {'': ['*']} install_requires = \ ['hosh>=3.230705.2,<4.0.0',
 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0'] extras_require = \
 {'full': ['pandas>=2.0.0,<3.0.0', 'shelchemy>=0.220906.3,<0.220907.0',
 'safeserializer>=0.230202.1,<0.230203.0', 'lz4>=4.3.2,<5.0.0', 'scikit-
 learn>=1.2.2,<2.0.0', 'liac-arff>=2.5.0,<3.0.0']} setup_kwargs = { 'name':
-'hdict', 'version': '0.230412.3', 'description': 'A versatile dictionary based
+'hdict', 'version': '1.230706.1', 'description': 'A versatile dictionary based
 on a novel paradigm useful for computing, caching, experiments, distributed
 data, among others.', 'long_description': '![test](https://github.com/davips/
 hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/
 hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n\n
-[pypi]\n\n![Python version](https://img.shields.io/badge/python-3.10...-
+[pypi]\n\n![Python version](https://img.shields.io/badge/python-3.10+-
 blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-
 blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![arXiv](https://
 img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
 arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
 API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual]
 (https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://
 hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://
```

### Comparing `hdict-0.230412.3/PKG-INFO` & `hdict-1.230706.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hdict
-Version: 0.230412.3
+Version: 1.230706.1
 Summary: A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
-Requires-Dist: hosh (>=2.230205.2,<3.0.0)
+Requires-Dist: hosh (>=3.230705.2,<4.0.0)
 Requires-Dist: indexed (>=1.3.0,<2.0.0)
 Requires-Dist: lange (>=1.230203.2,<2.0.0)
 Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra == "full"
 Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full"
 Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "full"
 Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full"
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "full"
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/davips/hdict/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
 <a href="https://pypi.org/project/hdict">
 <img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.10...-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
 [![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: hdict Version: 0.230412.3 Summary: A versatile
+Metadata-Version: 2.1 Name: hdict Version: 1.230706.1 Summary: A versatile
 dictionary based on a novel paradigm useful for computing, caching,
 experiments, distributed data, among others. License: GPLv3 Author: davips
 Author-email: dpsabc@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: full Requires-Dist: hosh
-(>=2.230205.2,<3.0.0) Requires-Dist: indexed (>=1.3.0,<2.0.0) Requires-Dist:
+(>=3.230705.2,<4.0.0) Requires-Dist: indexed (>=1.3.0,<2.0.0) Requires-Dist:
 lange (>=1.230203.2,<2.0.0) Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra
 == "full" Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full" Requires-Dist:
 pandas (>=2.0.0,<3.0.0) ; extra == "full" Requires-Dist: safeserializer
 (>=0.230202.1,<0.230203.0) ; extra == "full" Requires-Dist: scikit-learn
 (>=1.2.2,<2.0.0) ; extra == "full" Requires-Dist: shelchemy
 (>=0.220906.3,<0.220907.0) ; extra == "full" Description-Content-Type: text/
 markdown ![test](https://github.com/davips/hdict/workflows/test/badge.svg) [!
 [codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)]
 (https://codecov.io/gh/davips/hdict) [pypi] ![Python version](https://
-img.shields.io/badge/python-3.10...-blue.svg) [![license: GPL v3](https://
+img.shields.io/badge/python-3.10+-blue.svg) [![license: GPL v3](https://
 img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
 3.0)  [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
 b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
 documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hdict) [![Manual](https://img.shields.io/badge/
 manual-handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
 static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict) # hdict { A
```

