# Comparing `tmp/badgers-0.0.1.tar.gz` & `tmp/badgers-0.0.2.tar.gz`

## Comparing `badgers-0.0.1.tar` & `badgers-0.0.2.tar`

### file list

```diff
@@ -1,58 +1,61 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 badgers-0.0.1/.editorconfig
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 badgers-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 badgers-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 badgers-0.0.1/requirements_dev.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 badgers-0.0.1/tox.ini
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 badgers-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 badgers-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/core/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/core/base.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/core/decorators.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/core/pipeline.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/core/utils.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/geolocated_data/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/graph/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/graph/missingness.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/image/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/__init__.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/drift.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/imbalance.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/missingness.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/noise.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/tabular_data/outliers.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/text/__init__.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/text/typos.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/time_series/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/time_series/noise.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 badgers-0.0.1/badgers/generators/time_series/outliers.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/about.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/changelog.md
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/getting-started.md
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/index.md
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/resources.md
--rw-r--r--   0        0        0   176777 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/tutorials/Imbalance-Tabular-Data.ipynb
--rw-r--r--   0        0        0   140551 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/tutorials/Missingness-Tabular-Data.ipynb
--rw-r--r--   0        0        0    41538 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/tutorials/Noise-Tabular-Data.ipynb
--rw-r--r--   0        0        0   338286 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/tutorials/Outliers-Tabular-Data.ipynb
--rw-r--r--   0        0        0    64936 2020-02-02 00:00:00.000000 badgers-0.0.1/docs/tutorials/Pipeline-Tabular-Data.ipynb
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/core/__init__.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/core/test_pipelines.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/__init__.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/test_drift.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/test_imbalance.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/test_missingness.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/test_noise.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/tabular_data/test_outliers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/text/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 badgers-0.0.1/tests/generators/text/test_typos.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 badgers-0.0.1/.gitignore
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 badgers-0.0.1/LICENSE
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 badgers-0.0.1/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 badgers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 badgers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 badgers-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 badgers-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 badgers-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 badgers-0.0.2/requirements_dev.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 badgers-0.0.2/tox.ini
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 badgers-0.0.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 badgers-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 badgers-0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/core/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/core/base.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/core/decorators.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/core/pipeline.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/core/utils.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/geolocated_data/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/graph/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/graph/missingness.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/image/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/__init__.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/drift.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/imbalance.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/missingness.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/noise.py
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/tabular_data/outliers.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/text/__init__.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/text/typos.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/time_series/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/time_series/noise.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 badgers-0.0.2/badgers/generators/time_series/outliers.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/about.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/changelog.md
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/getting-started.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/index.md
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/resources.md
+-rw-r--r--   0        0        0   176777 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/tutorials/Imbalance-Tabular-Data.ipynb
+-rw-r--r--   0        0        0   140551 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/tutorials/Missingness-Tabular-Data.ipynb
+-rw-r--r--   0        0        0    70508 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/tutorials/Noise-Tabular-Data.ipynb
+-rw-r--r--   0        0        0   338286 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/tutorials/Outliers-Tabular-Data.ipynb
+-rw-r--r--   0        0        0    64936 2020-02-02 00:00:00.000000 badgers-0.0.2/docs/tutorials/Pipeline-Tabular-Data.ipynb
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/core/__init__.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/core/test_pipelines.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/__init__.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/test_drift.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/test_imbalance.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/test_missingness.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/test_noise.py
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/tabular_data/test_outliers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/text/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/text/test_typos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/time_series/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 badgers-0.0.2/tests/generators/time_series/test_outliers.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 badgers-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 badgers-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 badgers-0.0.2/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 badgers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 badgers-0.0.2/PKG-INFO
```

### Comparing `badgers-0.0.1/CONTRIBUTING.md` & `badgers-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/mkdocs.yml` & `badgers-0.0.2/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 site_name: Badgers Documentation
 site_url: https://github.com/Fraunhofer-IESE/badgers
+repo_url: https://github.com/Fraunhofer-IESE/badgers
+repo_name: Fraunhofer-IESE/badgers
 
 nav:
     -   Home: index.md
     -   Getting started: getting-started.md
     -   About: about.md
     -   Changes: changelog.md
     -   Tutorials:
@@ -35,8 +37,8 @@
                 python:
                     options:
                         show_source: true
                     selection:
                         docstring_style: sphinx
     - mkdocs-jupyter
 watch:
-    - ../badgers
+    - ../badgers
```

### Comparing `badgers-0.0.1/.github/workflows/python-publish.yml` & `badgers-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/.github/workflows/tests.yml` & `badgers-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/core/decorators.py` & `badgers-0.0.2/badgers/core/decorators.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/core/pipeline.py` & `badgers-0.0.2/badgers/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/core/utils.py` & `badgers-0.0.2/badgers/core/utils.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/graph/missingness.py` & `badgers-0.0.2/badgers/generators/graph/missingness.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/tabular_data/drift.py` & `badgers-0.0.2/badgers/generators/tabular_data/drift.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/tabular_data/imbalance.py` & `badgers-0.0.2/badgers/generators/tabular_data/imbalance.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/tabular_data/missingness.py` & `badgers-0.0.2/badgers/generators/tabular_data/missingness.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/tabular_data/outliers.py` & `badgers-0.0.2/badgers/generators/tabular_data/outliers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,21 @@
 
 
 class OutliersGenerator(GeneratorMixin):
     """
     Base class for transformers that add outliers to tabular data
     """
 
-    def __init__(self, random_generator=default_rng(seed=0), percentage_outliers: int = 10):
+    def __init__(self, random_generator=default_rng(seed=0), n_outliers: int = 10):
         """
         :param random_generator: A random generator
-        :param percentage_outliers: The percentage of outliers to generate
+        :param n_outliers: The number of outliers to generate
         """
-        assert 0 <= percentage_outliers <= 100
-
         self.random_generator = random_generator
-        self.percentage_outliers = percentage_outliers
+        self.n_outliers = n_outliers
 
     @abc.abstractmethod
     def generate(self, X, y=None, **params):
         pass
 
 
 class ZScoreSamplingGenerator(OutliersGenerator):
@@ -61,22 +59,19 @@
         # standardize X
         scaler = StandardScaler()
 
         # fit, transform
         scaler.fit(X)
         Xt = scaler.transform(X)
 
-        # compute number of outliers
-        n_outliers = int(Xt.shape[0] * self.percentage_outliers / 100)
-
         # generate outliers
         outliers = np.array([
             random_sign(self.random_generator, size=Xt.shape[1]) * (
                 3. + self.random_generator.exponential(size=Xt.shape[1]))
-            for _ in range(n_outliers)
+            for _ in range(self.n_outliers)
         ])
 
         # in case we only have 1 outlier, reshape the array to match sklearn convention
         if outliers.shape[0] == 1:
             outliers = outliers.reshape(1, -1)
 
         # add "outliers" as labels for outliers
@@ -112,25 +107,22 @@
         # standardize X
         scaler = StandardScaler()
 
         # fit, transform
         scaler.fit(X)
         Xt = scaler.transform(X)
 
-        # compute number of outliers
-        n_outliers = int(Xt.shape[0] * self.percentage_outliers / 100)
-
         # computing outliers
         outliers = np.array([
             random_spherical_coordinate(
                 random_generator=self.random_generator,
                 size=Xt.shape[1],
                 radius=3. + self.random_generator.exponential()
             )
-            for _ in range(n_outliers)
+            for _ in range(self.n_outliers)
         ])
 
         # in case we only have 1 outlier, reshape the array to match sklearn convention
         if outliers.shape[0] == 1:
             outliers = outliers.reshape(1, -1)
 
         # add "outliers" as labels for outliers
@@ -177,25 +169,23 @@
             raise NotImplementedError('So far this generator only supports tabular data with at most 5 columns')
         # standardize X
         scaler = StandardScaler()
         # fit, transform
         scaler.fit(X)
         Xt = scaler.transform(X)
 
-        # compute number of outliers
-        n_outliers = int(Xt.shape[0] * self.percentage_outliers / 100)
-
         # compute the histogram of the data
         hist, edges = np.histogramdd(Xt, density=False, bins=self.bins)
         # normalize
         norm_hist = hist / (np.max(hist) - np.min(hist))
         # get coordinates of the histogram where the density is low (below a certain threshold)
         hist_coords_low_density = np.where(norm_hist <= self.threshold_low_density)
         # randomly pick some coordinates in the histogram where the density is low
-        hist_coords_random = self.random_generator.choice(list(zip(*hist_coords_low_density)), n_outliers, replace=True)
+        hist_coords_random = self.random_generator.choice(list(zip(*hist_coords_low_density)), self.n_outliers,
+                                                          replace=True)
 
         # computing outliers values
         outliers = np.array([
             [
                 self.random_generator.uniform(low=edges[i][c], high=edges[i][c + 1])
                 for i, c in enumerate(h_coords)
             ]
@@ -210,16 +200,16 @@
         yt = np.array(["outliers"] * len(outliers))
 
         return scaler.inverse_transform(outliers), yt
 
 
 class LowDensitySamplingGenerator(OutliersGenerator):
 
-    def __init__(self, random_generator=default_rng(seed=0), percentage_outliers: int = 10):
-        super().__init__(random_generator=random_generator, percentage_outliers=percentage_outliers)
+    def __init__(self, random_generator=default_rng(seed=0), n_outliers: int = 10):
+        super().__init__(random_generator=random_generator, n_outliers=n_outliers)
         self.density_estimator = KernelDensity(bandwidth="scott")
 
     def generate(self, X, y=None, **params):
         """
         Generate data points belonging to low density regions.
 
         Pseudo code:
@@ -239,36 +229,34 @@
         # fit, transform
         scaler.fit(X)
         Xt = scaler.transform(X)
         # fit density estimator
         self.density_estimator = self.density_estimator.fit(Xt)
         low_density_threshold = np.percentile(self.density_estimator.score_samples(Xt), 0.1)
 
-        n_outliers = int(Xt.shape[0] * self.percentage_outliers / 100)
-
         if params.get('max_samples') is not None:
             max_samples = params['max_samples']
         else:
-            max_samples = n_outliers * 100
+            max_samples = self.n_outliers * 100
 
         outliers = np.array([
             x
             for x in self.random_generator.uniform(
                 low=np.min(Xt, axis=0),
                 high=np.max(Xt, axis=0),
                 size=(max_samples, Xt.shape[1])
             )
             if self.density_estimator.score_samples(x.reshape(1, -1)) <= low_density_threshold
         ])
 
-        if outliers.shape[0] < n_outliers:
+        if outliers.shape[0] < self.n_outliers:
             warnings.warn(
-                f'LowDensitySamplingGenerator could not generate all {n_outliers} outliers. It only generated {len(outliers)}.')
+                f'LowDensitySamplingGenerator could not generate all {self.n_outliers} outliers. It only generated {len(outliers)}.')
         else:
-            outliers = outliers[:n_outliers]
+            outliers = outliers[:self.n_outliers]
 
         # in case we only have 1 outlier, reshape the array to match sklearn convention
         if outliers.shape[0] == 1:
             outliers = outliers.reshape(1, -1)
 
         # add "outliers" as labels for outliers
         yt = np.array(["outliers"] * len(outliers))
@@ -291,18 +279,16 @@
         :param outlier_generator: The outlier transformer to be used after the dimensionality has been reduced
         """
         assert hasattr(
             decomposition_transformer,
             'inverse_transform'), \
             f'the decomposition transformer class must implement the inverse_transform function.' \
             f'\nUnfortunately the class {decomposition_transformer} does not'
-        super().__init__(
-            random_generator=outlier_generator.random_generator,
-            percentage_outliers=outlier_generator.percentage_outliers
-        )
+        super().__init__(random_generator=outlier_generator.random_generator,
+                         n_outliers=outlier_generator.n_outliers)
 
         self.decomposition_transformer = decomposition_transformer
         self.outlier_generator = outlier_generator
 
     def generate(self, X, y=None, **params):
         """
         Randomly generate outliers by first applying a dimensionality reduction technique (sklearn.decomposition)
```

### Comparing `badgers-0.0.1/badgers/generators/text/typos.py` & `badgers-0.0.2/badgers/generators/text/typos.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/badgers/generators/time_series/noise.py` & `badgers-0.0.2/badgers/generators/time_series/noise.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,35 +10,32 @@
 class NoiseGenerator(GeneratorMixin):
     """
     Base class for transformers that add noise to tabular data
     """
 
     def __init__(self, random_generator=default_rng(seed=0)):
         """
-        :param random_generator: numpy.random.Generator, default default_rng(seed=0)
-            A random generator
+        :param random_generator: A random generator
         """
         self.random_generator = random_generator
 
     @abc.abstractmethod
     def generate(self, X, y, **params) -> Tuple:
         pass
 
 
 class GaussianNoiseGenerator(NoiseGenerator):
-    def __init__(self, random_generator=default_rng(seed=0), signal_to_noise_ratio: float = 0.1):
+    def __init__(self, random_generator=default_rng(seed=0), noise_std: float = 0.1):
         """
 
-        :param random_generator: numpy.random.Generator, default default_rng(seed=0)
-            A random generator
-        :param signal_to_noise_ratio: float, default 0.1
-            The standard deviation of the noise to be added
+        :param random_generator: A random generator
+        :param noise_std: The standard deviation of the noise to be added
         """
         super().__init__(random_generator=random_generator)
-        self.signal_to_noise_ratio = signal_to_noise_ratio
+        self.noise_std = noise_std
 
     def generate(self, X, y, **params):
         """
         Add Gaussian white noise to the data.
         the data is first standardized (each column has a mean = 0 and variance = 1).
         The noise is generated from a normal distribution with standard deviation = `noise_std`.
         The noise is added to the data.
@@ -47,10 +44,10 @@
         :return:
         """
         scaler = StandardScaler()
         # fit, transform
         scaler.fit(X)
         Xt = scaler.transform(X)
         # add noise
-        Xt = Xt + self.random_generator.normal(loc=0, scale=self.signal_to_noise_ratio, size=Xt.shape)
+        Xt = Xt + self.random_generator.normal(loc=0, scale=self.noise_std, size=Xt.shape)
         # inverse pca
         return scaler.inverse_transform(Xt), y
```

### Comparing `badgers-0.0.1/badgers/generators/time_series/outliers.py` & `badgers-0.0.2/badgers/generators/time_series/outliers.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,48 +26,51 @@
 
 
 class LocalZScoreGenerator(OutliersGenerator):
     """
     Randomly generates extreme values
     """
 
-    def __init__(self, random_generator=default_rng(seed=0), percentage_extreme_values: int = 10,
+    def __init__(self, random_generator=default_rng(seed=0), n_outliers: int = 10,
                  local_window_size: int = 10):
         """
 
         :param random_generator: a random number generator
-        :param percentage_extreme_values: the percentage of extreme values to generate
+        :param n_outliers: the percentage of extreme values to generate
         :param  local_window_size: the width (number of data points) of the local window to compute local Z-Score
         """
         super().__init__(random_generator=random_generator)
-        assert 0 <= percentage_extreme_values <= 100
-        self.percentage_extreme_values = percentage_extreme_values
+        self.n_outliers = n_outliers
         self.local_window_size = local_window_size
+        self.outliers_indices_ = []
 
     def generate(self, X, y, **params):
         """
         Computes indices of extreme values using a uniform distribution.
         Computes the absolute values uniformly at random between mean(X) + 3 sigma(X) and mean(X) + 5 sigma(X).
         The sign of the extreme value is the same as the value being replaced.
 
         :param X:
         :return: the transformed array
         """
-        # compute number of extreme values per column
-        nb_extreme_values = int(X.shape[0] * self.percentage_extreme_values / 100)
+        # TODO input validation!
+        if X.ndim < 2:
+            raise ValueError(
+                "Expected 2D array. "
+                "Reshape your data either using array.reshape(-1, 1) if "
+                "your data has a single feature or array.reshape(1, -1) "
+                "if it contains a single sample."
+            )
         # generate extreme values indices and values
-        self.outliers_indices_ = dict()
-        for col in range(X.shape[1]):
-            rows = self.random_generator.choice(X.shape[0], size=nb_extreme_values, replace=False, p=None)
-            # keeping track of the outliers indices
-            self.outliers_indices_ += [(row, col) for row in rows]
-            for row in rows:
-                local_window = X[row - int(self.local_window_size / 2):row + int(self.local_window_size / 2), col]
-                local_mean = local_window.mean()
-                local_var = local_window.var()
-                value = local_mean + random_sign(self.random_generator, 1) * self.random_generator.uniform(
-                    low=3. * local_var[col], high=5 * local_mean[col]
-                )
-                # updating with new outliers
-                X[row, col] = value
+        self.outliers_indices_ = []
+
+        self.outliers_indices_ = self.random_generator.choice(X.shape[0], size=self.n_outliers, replace=False, p=None)
+        # keeping track of the outliers indices
+        for idx in self.outliers_indices_:
+            local_window = X[idx - int(self.local_window_size / 2):idx + int(self.local_window_size / 2), :]
+            local_mean = local_window.mean(axis=0)
+            local_std = local_window.std(axis=0)
+            value = local_mean + random_sign(self.random_generator, size=X.shape[1]) * (3. * local_std + self.random_generator.exponential(size=X.shape[1]))
+            # updating with new outliers
+            X[idx, :] = value
 
         return X, y
```

### Comparing `badgers-0.0.1/docs/about.md` & `badgers-0.0.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/gen_ref_pages.py` & `badgers-0.0.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/getting-started.md` & `badgers-0.0.2/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/index.md` & `badgers-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/resources.md` & `badgers-0.0.2/docs/resources.md`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/tutorials/Imbalance-Tabular-Data.ipynb` & `badgers-0.0.2/docs/tutorials/Imbalance-Tabular-Data.ipynb`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/tutorials/Missingness-Tabular-Data.ipynb` & `badgers-0.0.2/docs/tutorials/Missingness-Tabular-Data.ipynb`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/tutorials/Outliers-Tabular-Data.ipynb` & `badgers-0.0.2/docs/tutorials/Outliers-Tabular-Data.ipynb`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/docs/tutorials/Pipeline-Tabular-Data.ipynb` & `badgers-0.0.2/docs/tutorials/Pipeline-Tabular-Data.ipynb`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/core/test_pipelines.py` & `badgers-0.0.2/tests/core/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/core/test_utils.py` & `badgers-0.0.2/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/generators/tabular_data/__init__.py` & `badgers-0.0.2/tests/generators/tabular_data/__init__.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/generators/tabular_data/test_drift.py` & `badgers-0.0.2/tests/generators/tabular_data/test_drift.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/generators/tabular_data/test_imbalance.py` & `badgers-0.0.2/tests/generators/tabular_data/test_imbalance.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/generators/tabular_data/test_missingness.py` & `badgers-0.0.2/tests/generators/tabular_data/test_missingness.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/tests/generators/tabular_data/test_outliers.py` & `badgers-0.0.2/tests/generators/tabular_data/test_outliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.assertEqual(yt.shape[0], outliers.shape[0])
 
     def assert_shape_outliers(self, X, outliers, generator):
         """
         asserts that the correct number of outliers have been produced
         with the correct number of features
         """
-        self.assertEqual(outliers.shape[0], int(generator.percentage_outliers * X.shape[0] / 100))
+        self.assertEqual(outliers.shape[0], int(generator.n_outliers))
         self.assertEqual(outliers.shape[1], X.shape[1])
 
 
 class TestZScoreSamplingGenerator(TestOutliersGenerator):
     def setUp(self) -> None:
         self.rng = default_rng(0)
         self.generator = ZScoreSamplingGenerator(random_generator=self.rng, percentage_outliers=10)
@@ -99,15 +99,15 @@
                 self.assert_shape_yt(yt, outliers)
                 self.assert_shape_outliers(X, outliers, generator=self.generator)
 
 
 class TestLowDensitySamplingGenerator(TestOutliersGenerator):
     def setUp(self) -> None:
         self.rng = default_rng(0)
-        self.generator = LowDensitySamplingGenerator(random_generator=self.rng, percentage_outliers=10)
+        self.generator = LowDensitySamplingGenerator(random_generator=self.rng, n_outliers=10)
         self.input_test_data = generate_test_data_only_features(rng=self.rng)
 
     def test_generator(self):
         """
 
         """
         for input_type, (X, y) in self.input_test_data.items():
```

### Comparing `badgers-0.0.1/tests/generators/text/test_typos.py` & `badgers-0.0.2/tests/generators/text/test_typos.py`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/.gitignore` & `badgers-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/LICENSE` & `badgers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `badgers-0.0.1/README.md` & `badgers-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Badgers: bad data generators
 
 [badgers](https://github.com/Fraunhofer-IESE/badgers) is a python library for generating bad data (more precisely to augment existing data with data quality deficits such as outliers, missing values, noise, etc.). It is based upon a simple API and provides a set of generators object that can generate data quality deficits from existing data.
 
+A word of caution: badgers is still in an early development stage. Although the core structure of the package and the `generate(X,y)` signature are not expected to change, some API details (like attributes names) are likely to change.
+
+
 The full documentation is hosted here: [https://fraunhofer-iese.github.io/badgers/](https://fraunhofer-iese.github.io/badgers/).
 
 For a quick-start, you can install `badgers` with pip:
 
 ```bash
 pip install badgers
 ```
```

### Comparing `badgers-0.0.1/pyproject.toml` & `badgers-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "badgers"
-version = "0.0.1"
+version = "0.0.2"
 keywords = ["data quality", "bad data", "data science"]
 authors = [
     { name = "Julien Siebert", email = "julien.siebert@iese.fraunhofer.de" },
 ]
 maintainers = [
     { name = "Julien Siebert", email = "julien.siebert@iese.fraunhofer.de" },
 ]
```

### Comparing `badgers-0.0.1/PKG-INFO` & `badgers-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Badgers: bad data generators
 Project-URL: Homepage, https://github.com/Fraunhofer-IESE/badgers
 Project-URL: Bug Tracker, https://github.com/Fraunhofer-IESE/badgers/issues
 Author-email: Julien Siebert <julien.siebert@iese.fraunhofer.de>
 Maintainer-email: Julien Siebert <julien.siebert@iese.fraunhofer.de>
 License: BSD 3-Clause License
         
@@ -47,14 +47,17 @@
 Requires-Dist: scikit-learn
 Description-Content-Type: text/markdown
 
 # Badgers: bad data generators
 
 [badgers](https://github.com/Fraunhofer-IESE/badgers) is a python library for generating bad data (more precisely to augment existing data with data quality deficits such as outliers, missing values, noise, etc.). It is based upon a simple API and provides a set of generators object that can generate data quality deficits from existing data.
 
+A word of caution: badgers is still in an early development stage. Although the core structure of the package and the `generate(X,y)` signature are not expected to change, some API details (like attributes names) are likely to change.
+
+
 The full documentation is hosted here: [https://fraunhofer-iese.github.io/badgers/](https://fraunhofer-iese.github.io/badgers/).
 
 For a quick-start, you can install `badgers` with pip:
 
 ```bash
 pip install badgers
 ```
```

