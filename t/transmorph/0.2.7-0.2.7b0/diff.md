# Comparing `tmp/transmorph-0.2.7.tar.gz` & `tmp/transmorph-0.2.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmorph-0.2.7.tar", last modified: Mon Jun 26 09:02:02 2023, max compression
+gzip compressed data, was "transmorph-0.2.7b0.tar", last modified: Fri Jul  7 08:12:47 2023, max compression
```

## Comparing `transmorph-0.2.7.tar` & `transmorph-0.2.7b0.tar`

### file list

```diff
@@ -1,130 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.381046 transmorph-0.2.7/
--rw-rw-rw-   0        0        0     1093 2022-10-10 09:12:24.000000 transmorph-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       90 2022-10-19 13:47:49.000000 transmorph-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4858 2023-06-26 09:02:02.381046 transmorph-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4344 2022-11-18 09:22:14.000000 transmorph-0.2.7/README.md
--rw-rw-rw-   0        0        0      102 2022-10-10 09:12:24.000000 transmorph-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       76 2023-06-26 09:02:02.382046 transmorph-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-06-26 08:44:08.000000 transmorph-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.255350 transmorph-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.278304 transmorph-0.2.7/src/transmorph/
--rw-rw-rw-   0        0        0      841 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/__init__.py
--rw-rw-rw-   0        0        0     1543 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_logging.py
--rw-rw-rw-   0        0        0     2845 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_profiling.py
--rw-rw-rw-   0        0        0     6536 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.307603 transmorph-0.2.7/src/transmorph/datasets/
--rw-rw-rw-   0        0        0      741 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.308603 transmorph-0.2.7/src/transmorph/datasets/data/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.330608 transmorph-0.2.7/src/transmorph/datasets/data/spirals/
--rw-rw-rw-   0        0        0    33609 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA.csv
--rw-rw-rw-   0        0        0    11258 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA_labels.csv
--rw-rw-rw-   0        0        0    51240 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB.csv
--rw-rw-rw-   0        0        0    17238 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB_labels.csv
--rw-rw-rw-   0        0        0     5866 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/databank_api.py
--rw-rw-rw-   0        0        0     2957 2022-11-28 15:56:35.000000 transmorph-0.2.7/src/transmorph/datasets/datasets.json
--rw-rw-rw-   0        0        0    18148 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/datasets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.331608 transmorph-0.2.7/src/transmorph/engine/
--rw-rw-rw-   0        0        0       75 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.332600 transmorph-0.2.7/src/transmorph/engine/checking/
--rw-rw-rw-   0        0        0      203 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/checking/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.334609 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1660 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/lisi.py
--rw-rw-rw-   0        0        0     2321 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/neighborentropy.py
--rw-rw-rw-   0        0        0     1704 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/checking.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.335609 transmorph-0.2.7/src/transmorph/engine/evaluators/
--rw-rw-rw-   0        0        0      303 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/evaluators/__init__.py
--rw-rw-rw-   0        0        0     1846 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/evaluators/matching_evaluators.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.340297 transmorph-0.2.7/src/transmorph/engine/layers/
--rw-rw-rw-   0        0        0      468 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/__init__.py
--rw-rw-rw-   0        0        0     4468 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layer.py
--rw-rw-rw-   0        0        0     7936 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/layers/layerchecking.py
--rw-rw-rw-   0        0        0     2002 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layerinput.py
--rw-rw-rw-   0        0        0     5835 2022-10-20 15:53:39.000000 transmorph-0.2.7/src/transmorph/engine/layers/layermatching.py
--rw-rw-rw-   0        0        0     2760 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/layers/layermerging.py
--rw-rw-rw-   0        0        0     1527 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/engine/layers/layeroutput.py
--rw-rw-rw-   0        0        0     2054 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layertransformation.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.341308 transmorph-0.2.7/src/transmorph/engine/matching/
--rw-rw-rw-   0        0        0      505 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.346309 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/__init__.py
--rw-rw-rw-   0        0        0     3897 2022-11-10 14:04:53.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/bknn.py
--rw-rw-rw-   0        0        0     1923 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/combinematching.py
--rw-rw-rw-   0        0        0     5095 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/fusedgw.py
--rw-rw-rw-   0        0        0     5640 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/gw.py
--rw-rw-rw-   0        0        0     1455 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/labels.py
--rw-rw-rw-   0        0        0     5816 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/mnn.py
--rw-rw-rw-   0        0        0    10156 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/ot.py
--rw-rw-rw-   0        0        0     2398 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.348320 transmorph-0.2.7/src/transmorph/engine/merging/
--rw-rw-rw-   0        0        0      318 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.350320 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/barycenter.py
--rw-rw-rw-   0        0        0     8716 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/graphembedding.py
--rw-rw-rw-   0        0        0     5301 2022-11-26 11:46:46.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/linearcorrection.py
--rw-rw-rw-   0        0        0     2690 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/merging.py
--rw-rw-rw-   0        0        0    11038 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/engine/model.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.351321 transmorph-0.2.7/src/transmorph/engine/subsampling/
--rw-rw-rw-   0        0        0      228 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.353321 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/__init__.py
--rw-rw-rw-   0        0        0      699 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/keepall.py
--rw-rw-rw-   0        0        0     1957 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/vertexcover.py
--rw-rw-rw-   0        0        0     1905 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/subsampling.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.362031 transmorph-0.2.7/src/transmorph/engine/traits/
--rw-rw-rw-   0        0        0     1223 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/traits/__init__.py
--rw-rw-rw-   0        0        0     2050 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/cancatchchecking.py
--rw-rw-rw-   0        0        0     2060 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/canlog.py
--rw-rw-rw-   0        0        0     3809 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/traits/containstransformations.py
--rw-rw-rw-   0        0        0     3988 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/hasmetadata.py
--rw-rw-rw-   0        0        0     1336 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/isprofilable.py
--rw-rw-rw-   0        0        0     3642 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/isrepresentable.py
--rw-rw-rw-   0        0        0     9772 2022-10-20 15:49:57.000000 transmorph-0.2.7/src/transmorph/engine/traits/issubsamplable.py
--rw-rw-rw-   0        0        0     4956 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usescommonfeatures.py
--rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesmatching.py
--rw-rw-rw-   0        0        0     4034 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesmetric.py
--rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesreference.py
--rw-rw-rw-   0        0        0     2219 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usessamplelabels.py
--rw-rw-rw-   0        0        0     1474 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.363042 transmorph-0.2.7/src/transmorph/engine/transforming/
--rw-rw-rw-   0        0        0      516 2022-12-09 09:35:34.000000 transmorph-0.2.7/src/transmorph/engine/transforming/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.367043 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/__init__.py
--rw-rw-rw-   0        0        0     1729 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/commonfeatures.py
--rw-rw-rw-   0        0        0     1948 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/ica.py
--rw-rw-rw-   0        0        0     3184 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pca.py
--rw-rw-rw-   0        0        0     3150 2022-11-10 09:45:55.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pooling.py
--rw-rw-rw-   0        0        0     1155 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/standardize.py
--rw-rw-rw-   0        0        0     4046 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/transformation.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.370043 transmorph-0.2.7/src/transmorph/models/
--rw-rw-rw-   0        0        0      297 2022-12-09 09:39:17.000000 transmorph-0.2.7/src/transmorph/models/__init__.py
--rw-rw-rw-   0        0        0     6411 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/embedmnn.py
--rw-rw-rw-   0        0        0     2687 2022-12-09 09:31:47.000000 transmorph-0.2.7/src/transmorph/models/harmony.py
--rw-rw-rw-   0        0        0     6564 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/mnncorrection.py
--rw-rw-rw-   0        0        0     3075 2022-12-09 09:31:40.000000 transmorph-0.2.7/src/transmorph/models/scvi_vae.py
--rw-rw-rw-   0        0        0     7768 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/transportcorrection.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.373044 transmorph-0.2.7/src/transmorph/stats/
--rw-rw-rw-   0        0        0      376 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/__init__.py
--rw-rw-rw-   0        0        0     2035 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/entropy.py
--rw-rw-rw-   0        0        0     4118 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/stats/integration.py
--rw-rw-rw-   0        0        0     3854 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/lisi.py
--rw-rw-rw-   0        0        0     7658 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/stats/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.381046 transmorph-0.2.7/src/transmorph/utils/
--rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/__init__.py
--rw-rw-rw-   0        0        0    14929 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/anndata_manager.py
--rw-rw-rw-   0        0        0     3842 2022-11-02 15:25:44.000000 transmorph-0.2.7/src/transmorph/utils/dimred.py
--rw-rw-rw-   0        0        0      220 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/utils/file.py
--rw-rw-rw-   0        0        0     2353 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/geometry.py
--rw-rw-rw-   0        0        0    23531 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/graph.py
--rw-rw-rw-   0        0        0     5464 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/infer.py
--rw-rw-rw-   0        0        0     4791 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/matrix.py
--rw-rw-rw-   0        0        0     1766 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/utils/misc.py
--rw-rw-rw-   0        0        0    19910 2022-11-30 09:32:06.000000 transmorph-0.2.7/src/transmorph/utils/plotting.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.292307 transmorph-0.2.7/src/transmorph.egg-info/
--rw-rw-rw-   0        0        0     4858 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.059746 transmorph-0.2.7b0/
+-rw-rw-rw-   0        0        0     1093 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/LICENSE
+-rw-rw-rw-   0        0        0       90 2022-10-19 13:47:49.000000 transmorph-0.2.7b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4958 2023-07-07 08:12:47.059746 transmorph-0.2.7b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4442 2023-06-26 09:10:13.000000 transmorph-0.2.7b0/README.md
+-rw-rw-rw-   0        0        0      102 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2023-07-07 08:12:47.060746 transmorph-0.2.7b0/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-07-07 08:12:35.000000 transmorph-0.2.7b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:46.906651 transmorph-0.2.7b0/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:46.927651 transmorph-0.2.7b0/src/transmorph/
+-rw-rw-rw-   0        0        0      841 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/__init__.py
+-rw-rw-rw-   0        0        0     1543 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/_logging.py
+-rw-rw-rw-   0        0        0     2845 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/_profiling.py
+-rw-rw-rw-   0        0        0     6536 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:46.975915 transmorph-0.2.7b0/src/transmorph/datasets/
+-rw-rw-rw-   0        0        0      741 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:46.976915 transmorph-0.2.7b0/src/transmorph/datasets/data/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/datasets/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.005842 transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/
+-rw-rw-rw-   0        0        0    33609 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralA.csv
+-rw-rw-rw-   0        0        0    11258 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralA_labels.csv
+-rw-rw-rw-   0        0        0    51240 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralB.csv
+-rw-rw-rw-   0        0        0    17238 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralB_labels.csv
+-rw-rw-rw-   0        0        0     5866 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/datasets/databank_api.py
+-rw-rw-rw-   0        0        0     2957 2022-11-28 15:56:35.000000 transmorph-0.2.7b0/src/transmorph/datasets/datasets.json
+-rw-rw-rw-   0        0        0    18148 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/datasets/datasets.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.006853 transmorph-0.2.7b0/src/transmorph/engine/
+-rw-rw-rw-   0        0        0       75 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.007853 transmorph-0.2.7b0/src/transmorph/engine/checking/
+-rw-rw-rw-   0        0        0      203 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/checking/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.009853 transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1660 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/lisi.py
+-rw-rw-rw-   0        0        0     2321 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/neighborentropy.py
+-rw-rw-rw-   0        0        0     1704 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/checking/checking.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.011366 transmorph-0.2.7b0/src/transmorph/engine/evaluators/
+-rw-rw-rw-   0        0        0      303 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/evaluators/__init__.py
+-rw-rw-rw-   0        0        0     1846 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/evaluators/matching_evaluators.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.016460 transmorph-0.2.7b0/src/transmorph/engine/layers/
+-rw-rw-rw-   0        0        0      468 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/__init__.py
+-rw-rw-rw-   0        0        0     4468 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layer.py
+-rw-rw-rw-   0        0        0     7936 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layerchecking.py
+-rw-rw-rw-   0        0        0     2002 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layerinput.py
+-rw-rw-rw-   0        0        0     5835 2022-10-20 15:53:39.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layermatching.py
+-rw-rw-rw-   0        0        0     2760 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layermerging.py
+-rw-rw-rw-   0        0        0     1527 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layeroutput.py
+-rw-rw-rw-   0        0        0     2054 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/layers/layertransformation.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.018460 transmorph-0.2.7b0/src/transmorph/engine/matching/
+-rw-rw-rw-   0        0        0      505 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.023136 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3897 2022-11-10 14:04:53.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/bknn.py
+-rw-rw-rw-   0        0        0     1923 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/combinematching.py
+-rw-rw-rw-   0        0        0     5095 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/fusedgw.py
+-rw-rw-rw-   0        0        0     5640 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/gw.py
+-rw-rw-rw-   0        0        0     1455 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/labels.py
+-rw-rw-rw-   0        0        0     5816 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/mnn.py
+-rw-rw-rw-   0        0        0    10156 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/ot.py
+-rw-rw-rw-   0        0        0     2398 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/matching/matching.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.024148 transmorph-0.2.7b0/src/transmorph/engine/merging/
+-rw-rw-rw-   0        0        0      318 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.026148 transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/barycenter.py
+-rw-rw-rw-   0        0        0     8716 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/graphembedding.py
+-rw-rw-rw-   0        0        0     5301 2022-11-26 11:46:46.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/linearcorrection.py
+-rw-rw-rw-   0        0        0     2690 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/merging/merging.py
+-rw-rw-rw-   0        0        0    11038 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/engine/model.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.027148 transmorph-0.2.7b0/src/transmorph/engine/subsampling/
+-rw-rw-rw-   0        0        0      228 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/subsampling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.029149 transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      699 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/keepall.py
+-rw-rw-rw-   0        0        0     1957 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/vertexcover.py
+-rw-rw-rw-   0        0        0     1905 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/subsampling/subsampling.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.039686 transmorph-0.2.7b0/src/transmorph/engine/traits/
+-rw-rw-rw-   0        0        0     1223 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/__init__.py
+-rw-rw-rw-   0        0        0     2050 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/cancatchchecking.py
+-rw-rw-rw-   0        0        0     2060 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/canlog.py
+-rw-rw-rw-   0        0        0     3809 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/containstransformations.py
+-rw-rw-rw-   0        0        0     3988 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/hasmetadata.py
+-rw-rw-rw-   0        0        0     1336 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/isprofilable.py
+-rw-rw-rw-   0        0        0     3642 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/isrepresentable.py
+-rw-rw-rw-   0        0        0     9772 2022-10-20 15:49:57.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/issubsamplable.py
+-rw-rw-rw-   0        0        0     4956 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/usescommonfeatures.py
+-rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/usesmatching.py
+-rw-rw-rw-   0        0        0     4034 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/usesmetric.py
+-rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/usesreference.py
+-rw-rw-rw-   0        0        0     2219 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/usessamplelabels.py
+-rw-rw-rw-   0        0        0     1474 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/traits/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.040686 transmorph-0.2.7b0/src/transmorph/engine/transforming/
+-rw-rw-rw-   0        0        0      516 2022-12-09 09:35:34.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.044210 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1729 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/commonfeatures.py
+-rw-rw-rw-   0        0        0     1948 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/ica.py
+-rw-rw-rw-   0        0        0     3184 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/pca.py
+-rw-rw-rw-   0        0        0     3150 2022-11-10 09:45:55.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/pooling.py
+-rw-rw-rw-   0        0        0     1155 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/standardize.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.046212 transmorph-0.2.7b0/src/transmorph/engine/transforming/external/
+-rw-rw-rw-   0        0        0        0 2023-07-07 08:08:09.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/external/__init__.py
+-rw-rw-rw-   0        0        0     1879 2022-11-26 17:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/external/harmony.py
+-rw-rw-rw-   0        0        0     3181 2022-12-09 09:46:14.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/external/scvi_vae.py
+-rw-rw-rw-   0        0        0     4046 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/engine/transforming/transformation.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.049212 transmorph-0.2.7b0/src/transmorph/models/
+-rw-rw-rw-   0        0        0      297 2022-12-09 09:39:17.000000 transmorph-0.2.7b0/src/transmorph/models/__init__.py
+-rw-rw-rw-   0        0        0     6411 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/models/embedmnn.py
+-rw-rw-rw-   0        0        0     2687 2022-12-09 09:31:47.000000 transmorph-0.2.7b0/src/transmorph/models/harmony.py
+-rw-rw-rw-   0        0        0     6564 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/models/mnncorrection.py
+-rw-rw-rw-   0        0        0     3075 2022-12-09 09:31:40.000000 transmorph-0.2.7b0/src/transmorph/models/scvi_vae.py
+-rw-rw-rw-   0        0        0     7768 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/models/transportcorrection.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.051725 transmorph-0.2.7b0/src/transmorph/stats/
+-rw-rw-rw-   0        0        0      376 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/stats/__init__.py
+-rw-rw-rw-   0        0        0     2035 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/stats/entropy.py
+-rw-rw-rw-   0        0        0     4118 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/stats/integration.py
+-rw-rw-rw-   0        0        0     3854 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/stats/lisi.py
+-rw-rw-rw-   0        0        0     7658 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/stats/matching.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:47.058754 transmorph-0.2.7b0/src/transmorph/utils/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/utils/__init__.py
+-rw-rw-rw-   0        0        0    14929 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/utils/anndata_manager.py
+-rw-rw-rw-   0        0        0     3842 2022-11-02 15:25:44.000000 transmorph-0.2.7b0/src/transmorph/utils/dimred.py
+-rw-rw-rw-   0        0        0      220 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/utils/file.py
+-rw-rw-rw-   0        0        0     2353 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/utils/geometry.py
+-rw-rw-rw-   0        0        0    23531 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/utils/graph.py
+-rw-rw-rw-   0        0        0     5464 2022-11-18 09:21:05.000000 transmorph-0.2.7b0/src/transmorph/utils/infer.py
+-rw-rw-rw-   0        0        0     4791 2022-10-10 09:12:24.000000 transmorph-0.2.7b0/src/transmorph/utils/matrix.py
+-rw-rw-rw-   0        0        0     1766 2022-10-19 13:47:50.000000 transmorph-0.2.7b0/src/transmorph/utils/misc.py
+-rw-rw-rw-   0        0        0    19910 2022-11-30 09:32:06.000000 transmorph-0.2.7b0/src/transmorph/utils/plotting.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:12:46.941493 transmorph-0.2.7b0/src/transmorph.egg-info/
+-rw-rw-rw-   0        0        0     4958 2023-07-07 08:12:46.000000 transmorph-0.2.7b0/src/transmorph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4571 2023-07-07 08:12:46.000000 transmorph-0.2.7b0/src/transmorph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:12:46.000000 transmorph-0.2.7b0/src/transmorph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-07-07 08:12:46.000000 transmorph-0.2.7b0/src/transmorph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 08:12:46.000000 transmorph-0.2.7b0/src/transmorph.egg-info/top_level.txt
```

### Comparing `transmorph-0.2.7/LICENSE` & `transmorph-0.2.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/PKG-INFO` & `transmorph-0.2.7b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmorph
-Version: 0.2.7
+Version: 0.2.7b0
 Summary: A unifying data integration framework.
 Home-page: https://github.com/Risitop/transmorph
 Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
 Author-email: aziz.fouche@curie.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,16 @@
 # [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
 
 [![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
 [![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
 [![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+[![DOI](https://zenodo.org/badge/333111705.svg)](https://zenodo.org/badge/latestdoi/333111705)
+
 
 **transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
 
 <img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
 
 Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality.
```

### Comparing `transmorph-0.2.7/README.md` & `transmorph-0.2.7b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
 
 [![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
 [![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
 [![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+[![DOI](https://zenodo.org/badge/333111705.svg)](https://zenodo.org/badge/latestdoi/333111705)
+
 
 **transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
 
 <img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
 
 Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality.
```

### Comparing `transmorph-0.2.7/setup.py` & `transmorph-0.2.7b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="transmorph",
-    version="0.2.7",
+    version="0.2.7b",
     author="Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)",
     author_email="aziz.fouche@curie.fr",
     description="A unifying data integration framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Risitop/transmorph",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `transmorph-0.2.7/src/transmorph/__init__.py` & `transmorph-0.2.7b0/src/transmorph/__init__.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/_logging.py` & `transmorph-0.2.7b0/src/transmorph/_logging.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/_profiling.py` & `transmorph-0.2.7b0/src/transmorph/_profiling.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/_settings.py` & `transmorph-0.2.7b0/src/transmorph/_settings.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/__init__.py` & `transmorph-0.2.7b0/src/transmorph/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA.csv` & `transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralA.csv`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA_labels.csv` & `transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralA_labels.csv`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB.csv` & `transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralB.csv`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB_labels.csv` & `transmorph-0.2.7b0/src/transmorph/datasets/data/spirals/spiralB_labels.csv`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/databank_api.py` & `transmorph-0.2.7b0/src/transmorph/datasets/databank_api.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/datasets.json` & `transmorph-0.2.7b0/src/transmorph/datasets/datasets.json`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/datasets/datasets.py` & `transmorph-0.2.7b0/src/transmorph/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/checking/algorithms/lisi.py` & `transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/lisi.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/checking/algorithms/neighborentropy.py` & `transmorph-0.2.7b0/src/transmorph/engine/checking/algorithms/neighborentropy.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/checking/checking.py` & `transmorph-0.2.7b0/src/transmorph/engine/checking/checking.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/evaluators/matching_evaluators.py` & `transmorph-0.2.7b0/src/transmorph/engine/evaluators/matching_evaluators.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layer.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layer.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layerchecking.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layerchecking.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layerinput.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layerinput.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layermatching.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layermatching.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layermerging.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layermerging.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layeroutput.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layeroutput.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/layers/layertransformation.py` & `transmorph-0.2.7b0/src/transmorph/engine/layers/layertransformation.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/bknn.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/bknn.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/combinematching.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/combinematching.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/fusedgw.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/fusedgw.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/gw.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/gw.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/labels.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/labels.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/mnn.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/mnn.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/ot.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/algorithms/ot.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/matching/matching.py` & `transmorph-0.2.7b0/src/transmorph/engine/matching/matching.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/merging/algorithms/barycenter.py` & `transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/barycenter.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/merging/algorithms/graphembedding.py` & `transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/graphembedding.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/merging/algorithms/linearcorrection.py` & `transmorph-0.2.7b0/src/transmorph/engine/merging/algorithms/linearcorrection.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/merging/merging.py` & `transmorph-0.2.7b0/src/transmorph/engine/merging/merging.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/model.py` & `transmorph-0.2.7b0/src/transmorph/engine/model.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/keepall.py` & `transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/keepall.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/vertexcover.py` & `transmorph-0.2.7b0/src/transmorph/engine/subsampling/algorithms/vertexcover.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/subsampling/subsampling.py` & `transmorph-0.2.7b0/src/transmorph/engine/subsampling/subsampling.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/__init__.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/cancatchchecking.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/cancatchchecking.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/canlog.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/canlog.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/containstransformations.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/containstransformations.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/hasmetadata.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/hasmetadata.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/isprofilable.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/isprofilable.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/isrepresentable.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/isrepresentable.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/issubsamplable.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/issubsamplable.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/usescommonfeatures.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/usescommonfeatures.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/usesmatching.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/usesmatching.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/usesmetric.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/usesmetric.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/usesreference.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/usesreference.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/usessamplelabels.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/usessamplelabels.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/traits/utils.py` & `transmorph-0.2.7b0/src/transmorph/engine/traits/utils.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/__init__.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/__init__.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/commonfeatures.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/commonfeatures.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/ica.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/ica.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pca.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/pca.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pooling.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/pooling.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/standardize.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/algorithms/standardize.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/engine/transforming/transformation.py` & `transmorph-0.2.7b0/src/transmorph/engine/transforming/transformation.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/models/embedmnn.py` & `transmorph-0.2.7b0/src/transmorph/models/embedmnn.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/models/harmony.py` & `transmorph-0.2.7b0/src/transmorph/models/harmony.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/models/mnncorrection.py` & `transmorph-0.2.7b0/src/transmorph/models/mnncorrection.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/models/scvi_vae.py` & `transmorph-0.2.7b0/src/transmorph/models/scvi_vae.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/models/transportcorrection.py` & `transmorph-0.2.7b0/src/transmorph/models/transportcorrection.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/stats/entropy.py` & `transmorph-0.2.7b0/src/transmorph/stats/entropy.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/stats/integration.py` & `transmorph-0.2.7b0/src/transmorph/stats/integration.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/stats/lisi.py` & `transmorph-0.2.7b0/src/transmorph/stats/lisi.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/stats/matching.py` & `transmorph-0.2.7b0/src/transmorph/stats/matching.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/anndata_manager.py` & `transmorph-0.2.7b0/src/transmorph/utils/anndata_manager.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/dimred.py` & `transmorph-0.2.7b0/src/transmorph/utils/dimred.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/geometry.py` & `transmorph-0.2.7b0/src/transmorph/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/graph.py` & `transmorph-0.2.7b0/src/transmorph/utils/graph.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/infer.py` & `transmorph-0.2.7b0/src/transmorph/utils/infer.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/matrix.py` & `transmorph-0.2.7b0/src/transmorph/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/misc.py` & `transmorph-0.2.7b0/src/transmorph/utils/misc.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph/utils/plotting.py` & `transmorph-0.2.7b0/src/transmorph/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `transmorph-0.2.7/src/transmorph.egg-info/PKG-INFO` & `transmorph-0.2.7b0/src/transmorph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmorph
-Version: 0.2.7
+Version: 0.2.7b0
 Summary: A unifying data integration framework.
 Home-page: https://github.com/Risitop/transmorph
 Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
 Author-email: aziz.fouche@curie.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,16 @@
 # [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
 
 [![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
 [![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
 [![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+[![DOI](https://zenodo.org/badge/333111705.svg)](https://zenodo.org/badge/latestdoi/333111705)
+
 
 **transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
 
 <img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
 
 Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality.
```

### Comparing `transmorph-0.2.7/src/transmorph.egg-info/SOURCES.txt` & `transmorph-0.2.7b0/src/transmorph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 src/transmorph/engine/transforming/transformation.py
 src/transmorph/engine/transforming/algorithms/__init__.py
 src/transmorph/engine/transforming/algorithms/commonfeatures.py
 src/transmorph/engine/transforming/algorithms/ica.py
 src/transmorph/engine/transforming/algorithms/pca.py
 src/transmorph/engine/transforming/algorithms/pooling.py
 src/transmorph/engine/transforming/algorithms/standardize.py
+src/transmorph/engine/transforming/external/__init__.py
+src/transmorph/engine/transforming/external/harmony.py
+src/transmorph/engine/transforming/external/scvi_vae.py
 src/transmorph/models/__init__.py
 src/transmorph/models/embedmnn.py
 src/transmorph/models/harmony.py
 src/transmorph/models/mnncorrection.py
 src/transmorph/models/scvi_vae.py
 src/transmorph/models/transportcorrection.py
 src/transmorph/stats/__init__.py
```

