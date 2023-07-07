# Comparing `tmp/phepy-0.0.0.tar.gz` & `tmp/phepy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/phepy/phepy/dist/.tmp-q_dl10zq/phepy-0.0.0.tar", last modified: Thu May  4 15:32:24 2023, max compression
+gzip compressed data, was "/home/runner/work/phepy/phepy/dist/.tmp-7ie0xnc7/phepy-0.1.0.tar", last modified: Fri Jul  7 10:48:00 2023, max compression
```

## Comparing `phepy-0.0.0.tar` & `phepy-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:24.000000 phepy-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 15:32:04.000000 phepy-0.0.0/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 15:32:04.000000 phepy-0.0.0/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-05-04 15:32:24.000000 phepy-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-04 15:32:04.000000 phepy-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy/toys/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/toys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/toys/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/toys/haystack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-04 15:32:04.000000 phepy-0.0.0/phepy/toys/line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 15:32:24.000000 phepy-0.0.0/phepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 15:32:04.000000 phepy-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:32:24.000000 phepy-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:00.000000 phepy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 10:47:47.000000 phepy-0.1.0/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 10:47:47.000000 phepy-0.1.0/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-07 10:48:00.000000 phepy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-07 10:47:47.000000 phepy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy/toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/toys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/toys/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/toys/haystack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-07 10:47:47.000000 phepy-0.1.0/phepy/toys/line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 10:48:00.000000 phepy-0.1.0/phepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 10:47:47.000000 phepy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:48:00.000000 phepy-0.1.0/setup.cfg
```

### Comparing `phepy-0.0.0/LICENSE-APACHE` & `phepy-0.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `phepy-0.0.0/LICENSE-MIT` & `phepy-0.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `phepy-0.0.0/PKG-INFO` & `phepy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phepy
-Version: 0.0.0
+Version: 0.1.0
 Summary: Intuitive evaluation of out-of-distribution detectors using simple toy examples.
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -209,19 +209,22 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: example
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
-# phepy &emsp; [![PyPi]][pypi-url] [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![CI Status]][ci-status]
+# phepy &emsp; [![PyPi]][pypi-url]  [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![Docs]][docs-stable] [![CI Status]][ci-status]
 
 [PyPI]: https://img.shields.io/pypi/v/phepy
 [pypi-url]: https://pypi.org/project/phepy
 
+[Docs]: https://img.shields.io/pypi/v/phepy?color=blue&label=Docs
+[docs-stable]: https://juntyr.github.io/phepy/
+
 [License Apache-2.0]: https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg
 [apache-2.0]: https://opensource.org/licenses/Apache-2.0
 
 [License MIT]: https://img.shields.io/badge/License-MIT-yellow.svg
 [mit]: https://opensource.org/licenses/MIT
 
 [CI Status]: https://img.shields.io/github/actions/workflow/status/juntyr/phepy/ci.yml?branch=main&label=CI
@@ -253,15 +256,15 @@
 Next, enter the repository folder and use `pip` to install the program:
 ```bash
 cd phepy && pip install .
 ```
 
 ## Usage Example
 
-The following code snippet only provides a minimal example to get started, please refer to the [`examples`](examples) folder to find more extensive examples.
+The following code snippet only provides a minimal example to get started, please refer to the [`examples`](https://github.com/juntyr/phepy/tree/main/examples) folder to find more extensive examples.
 
 ```python
 # Import numpy, matplotlib, and sklearn
 import numpy as np
 import sklearn
 
 from matplotlib import pyplot as plt
@@ -310,15 +313,15 @@
     toys = [line, circle, haystack],
     cmap = "coolwarm", # use e.g. "viridis" to be colour-blind safe
 )
 
 plt.show()
 ```
 
-![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](examples/minimal.png)
+![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](https://raw.githubusercontent.com/juntyr/phepy/main/examples/minimal.png)
 
 In the above figure, the single row showcases the Local Outlier Factor (LOF, [^1]) method, while the three columns contain the following three test cases:
 
 * Two groups of training points are scattered along a line in the 2D feature space. The target variable only depends on the location along the line. In this example, points off the line are OOD.
 * The training points are scattered around the sine-displaced boundary of a circle, but none are inside it. The target variable only depends on the location along the boundary. Again, points off the line are OOD.
 * The training points are sampled from a 10-dimensional multivariate normal distribution, where one of the features is set to a constant. This example tests whether an OOD detection method can find a needle in a high-dimensional haystack, i.e. identify that points which do not share the constant are OOD.
 
@@ -326,21 +329,21 @@
 
 The Local Outlier Factor (LOF, [^1]) estimates the training data density around unseen data. Thus, it performs quite well on the line and circle examples where the data points are closely scattered. The LOF classifies the gap between the two groups of training inputs on the line as out-of-distribution (OOD), which may be too conservative if we assume that a machine-learning model can interpolate between the two groups. While LOF produces slightly lower confidence for the OOD inputs in the haystack, it does not clearly identify test data that do not have the constant feature seen in training as out-of-distribution.
 
 ## License
 
 Licensed under either of
 
-* Apache License, Version 2.0 ([`LICENSE-APACHE`](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
-* MIT license ([`LICENSE-MIT`](LICENSE-MIT) or http://opensource.org/licenses/MIT)
+* Apache License, Version 2.0 ([`LICENSE-APACHE`](https://github.com/juntyr/phepy/blob/main/LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
+* MIT license ([`LICENSE-MIT`](https://github.com/juntyr/phepy/blob/main/LICENSE-MIT) or http://opensource.org/licenses/MIT)
 
 at your option.
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.
 
 ## Citation
 
-Please refer to the [CITATION.cff](CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
+Please refer to the [CITATION.cff](https://github.com/juntyr/phepy/blob/main/CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
 
 [^1]: M. M. Breunig *et al*. LOF: Identifying Density-Based Local Outliers. *Proceedings of the 2000 ACM SIGMOD International Conference on Management of Data*. SIGMOD '00. Dallas, Texas, USA: Associ- ation for Computing Machinery, 2000, 93–104. Available from: [doi:10.1145/342009.335388](https://doi.org/10.1145/342009.335388).
```

### Comparing `phepy-0.0.0/README.md` & `phepy-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# phepy &emsp; [![PyPi]][pypi-url] [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![CI Status]][ci-status]
+# phepy &emsp; [![PyPi]][pypi-url]  [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![Docs]][docs-stable] [![CI Status]][ci-status]
 
 [PyPI]: https://img.shields.io/pypi/v/phepy
 [pypi-url]: https://pypi.org/project/phepy
 
+[Docs]: https://img.shields.io/pypi/v/phepy?color=blue&label=Docs
+[docs-stable]: https://juntyr.github.io/phepy/
+
 [License Apache-2.0]: https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg
 [apache-2.0]: https://opensource.org/licenses/Apache-2.0
 
 [License MIT]: https://img.shields.io/badge/License-MIT-yellow.svg
 [mit]: https://opensource.org/licenses/MIT
 
 [CI Status]: https://img.shields.io/github/actions/workflow/status/juntyr/phepy/ci.yml?branch=main&label=CI
@@ -38,15 +41,15 @@
 Next, enter the repository folder and use `pip` to install the program:
 ```bash
 cd phepy && pip install .
 ```
 
 ## Usage Example
 
-The following code snippet only provides a minimal example to get started, please refer to the [`examples`](examples) folder to find more extensive examples.
+The following code snippet only provides a minimal example to get started, please refer to the [`examples`](https://github.com/juntyr/phepy/tree/main/examples) folder to find more extensive examples.
 
 ```python
 # Import numpy, matplotlib, and sklearn
 import numpy as np
 import sklearn
 
 from matplotlib import pyplot as plt
@@ -95,15 +98,15 @@
     toys = [line, circle, haystack],
     cmap = "coolwarm", # use e.g. "viridis" to be colour-blind safe
 )
 
 plt.show()
 ```
 
-![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](examples/minimal.png)
+![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](https://raw.githubusercontent.com/juntyr/phepy/main/examples/minimal.png)
 
 In the above figure, the single row showcases the Local Outlier Factor (LOF, [^1]) method, while the three columns contain the following three test cases:
 
 * Two groups of training points are scattered along a line in the 2D feature space. The target variable only depends on the location along the line. In this example, points off the line are OOD.
 * The training points are scattered around the sine-displaced boundary of a circle, but none are inside it. The target variable only depends on the location along the boundary. Again, points off the line are OOD.
 * The training points are sampled from a 10-dimensional multivariate normal distribution, where one of the features is set to a constant. This example tests whether an OOD detection method can find a needle in a high-dimensional haystack, i.e. identify that points which do not share the constant are OOD.
 
@@ -111,21 +114,21 @@
 
 The Local Outlier Factor (LOF, [^1]) estimates the training data density around unseen data. Thus, it performs quite well on the line and circle examples where the data points are closely scattered. The LOF classifies the gap between the two groups of training inputs on the line as out-of-distribution (OOD), which may be too conservative if we assume that a machine-learning model can interpolate between the two groups. While LOF produces slightly lower confidence for the OOD inputs in the haystack, it does not clearly identify test data that do not have the constant feature seen in training as out-of-distribution.
 
 ## License
 
 Licensed under either of
 
-* Apache License, Version 2.0 ([`LICENSE-APACHE`](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
-* MIT license ([`LICENSE-MIT`](LICENSE-MIT) or http://opensource.org/licenses/MIT)
+* Apache License, Version 2.0 ([`LICENSE-APACHE`](https://github.com/juntyr/phepy/blob/main/LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
+* MIT license ([`LICENSE-MIT`](https://github.com/juntyr/phepy/blob/main/LICENSE-MIT) or http://opensource.org/licenses/MIT)
 
 at your option.
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.
 
 ## Citation
 
-Please refer to the [CITATION.cff](CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
+Please refer to the [CITATION.cff](https://github.com/juntyr/phepy/blob/main/CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
 
 [^1]: M. M. Breunig *et al*. LOF: Identifying Density-Based Local Outliers. *Proceedings of the 2000 ACM SIGMOD International Conference on Management of Data*. SIGMOD '00. Dallas, Texas, USA: Associ- ation for Computing Machinery, 2000, 93–104. Available from: [doi:10.1145/342009.335388](https://doi.org/10.1145/342009.335388).
```

### Comparing `phepy-0.0.0/phepy/detector.py` & `phepy-0.1.0/phepy/detector.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,23 @@
     def calibrate(
         self, X_valid: np.ndarray, Y_valid: np.ndarray
     ) -> OutOfDistributionScorer:
         pass
 
     @abc.abstractmethod
     def predict(self, X_test: np.ndarray) -> np.ndarray:
+        """Predict the confidence scores for several test data inputs.
+
+        Args:
+          X_test:
+            numpy array of shape `N_SAMPLES x N_FEATURES`
+
+        Returns:
+          The array confidence scores of shape `N_SAMPLES`
+        """
         pass
 
 
 class PercentileScorer(OutOfDistributionScorer):
     def __init__(
         self, detector: OutOfDistributionDetector
     ) -> PercentileScorer:
@@ -64,7 +73,26 @@
         ) / len(self.__S_valid)
 
         return (
             S_test
             if type(self.detector).low_score_is_low_confidence()
             else 1.0 - S_test
         )
+
+
+class IdentityScorer(OutOfDistributionScorer):
+    def __init__(self, detector: OutOfDistributionDetector) -> IdentityScorer:
+        super().__init__(detector)
+
+    def calibrate(
+        self, X_valid: np.ndarray, Y_valid: np.ndarray
+    ) -> IdentityScorer:
+        return self
+
+    def predict(self, X_test: np.ndarray) -> np.ndarray:
+        S_test = self.detector.predict(X_test)
+
+        return (
+            S_test
+            if type(self.detector).low_score_is_low_confidence()
+            else 1.0 - S_test
+        )
```

### Comparing `phepy-0.0.0/phepy/toys/__init__.py` & `phepy-0.1.0/phepy/toys/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,20 +31,25 @@
     def X_test(self) -> np.ndarray:
         pass
 
     @abc.abstractmethod
     def reconstruct(X: np.ndarray) -> np.ndarray:
         pass
 
+    @abc.abstractmethod
+    def is_in_distribution(X: np.ndarray) -> np.ndarray:
+        pass
+
     @property
     @abc.abstractmethod
     def aspect_ratio(self) -> float:
         pass
 
     @abc.abstractmethod
     def plot(
         self,
         conf: np.ndarray,
         ax: mpl.axes.Axes,
         cmap: Union[str, mpl.colors.Colormap],
+        with_scatter: bool = True,
     ):
         pass
```

### Comparing `phepy-0.0.0/phepy/toys/circle.py` & `phepy-0.1.0/phepy/toys/circle.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import matplotlib as mpl
 import numpy as np
 
 from . import ToyExample
 
 
 class CircleToyExample(ToyExample):
-    def __init__(self, rng: np.random.Generator) -> CircleToyExample:
-        N = 10_000 * 2
-
+    def __init__(
+        self, rng: np.random.Generator, N: int = 10_000
+    ) -> CircleToyExample:
         Y = np.sin(np.linspace(0, np.pi * 8.0, N))
 
         X1 = np.sin(np.linspace(0, np.pi * 2.0, N)) * (5 + Y)
         X2 = np.cos(np.linspace(0, np.pi * 2.0, N)) * (5 + Y)
 
         X1 += rng.normal(loc=0.0, scale=0.1, size=N)
         X2 += rng.normal(loc=0.0, scale=0.1, size=N)
@@ -56,56 +56,76 @@
 
     @property
     def X_test(self) -> np.ndarray:
         return np.copy(self.__X_test)
 
     def reconstruct(self, X: np.ndarray) -> np.ndarray:
         # Project X onto the sin-perturbed circle
-        angle = np.arctan2(X[:, 0], X[:, 1])
+        angle = _my_arctan2(X[:, 0], X[:, 1])
 
         Y = np.sin(angle * 4.0)
 
         X1 = np.sin(angle) * (5.0 + Y)
         X2 = np.cos(angle) * (5.0 + Y)
 
-        return np.stack([X1, X2], axis=1)
+        # return np.stack([X1, X2], axis=1)
+        return X1.reshape((len(X), 1)) * np.array([[1, 0]]) + X2.reshape(
+            (len(X), 1)
+        ) * np.array([[0, 1]])
+
+    def is_in_distribution(self, X: np.ndarray) -> np.ndarray:
+        # Two standard deviations off the mean -> 95.45% interval
+        return np.linalg.norm(X - self.reconstruct(X), axis=1) <= 0.2
 
     @property
     def aspect_ratio(self) -> float:
         return 1.0
 
     def plot(
         self,
         conf: np.ndarray,
         ax: mpl.axes.Axes,
         cmap: Union[str, mpl.colors.Colormap],
+        with_scatter: bool = True,
     ):
+        N_skip = len(self.X_train) // 40
+
         ax.imshow(
             conf.reshape(np.mgrid[-7.5:7.5:0.01, -7.5:7.5:0.01][0].shape).T,
             cmap=cmap,
             vmin=0.0,
             vmax=1.0,
             extent=[-7.5, 7.5, -7.5, 7.5],
             origin="lower",
             interpolation="bicubic",
             rasterized=True,
         )
 
         ax.set_xlim(-7.5, 7.5)
         ax.set_ylim(-7.5, 7.5)
 
-        ax.scatter(
-            self.X_train[::250, 0],
-            self.X_train[::250, 1],
-            c="white",
-            marker="x",
-            lw=3,
-            s=48,
-        )
-        ax.scatter(
-            self.X_train[::250, 0],
-            self.X_train[::250, 1],
-            c="black",
-            marker="x",
-        )
+        if with_scatter:
+            ax.scatter(
+                self.X_train[::N_skip, 0],
+                self.X_train[::N_skip, 1],
+                c="white",
+                marker="x",
+                lw=3,
+                s=48,
+            )
+            ax.scatter(
+                self.X_train[::N_skip, 0],
+                self.X_train[::N_skip, 1],
+                c="black",
+                marker="x",
+            )
 
         ax.axis("off")
+
+
+def _my_arctan2(x1: np.ndarray, x2: np.ndarray) -> np.ndarray:
+    a = np.arctan(x1 / x2)
+
+    a += np.pi * ((x2 < 0.0) & (x1 >= 0.0))
+    a -= np.pi * ((x2 < 0.0) & (x1 < 0.0))
+
+    return a
```

### Comparing `phepy-0.0.0/phepy/toys/haystack.py` & `phepy-0.1.0/phepy/toys/haystack.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 import matplotlib as mpl
 import numpy as np
 
 from . import ToyExample
 
 
 class HaystackToyExample(ToyExample):
-    def __init__(self, rng: np.random.Generator) -> HaystackToyExample:
-        N = 10_000 * 2
+    def __init__(
+        self, rng: np.random.Generator, N: int = 10_000
+    ) -> HaystackToyExample:
+        N *= 2
 
         n = 10
         a = 2
 
         # https://stats.stackexchange.com/a/124554
         A = np.matrix(
             [rng.normal(size=n) + rng.normal(size=1) * a for i in range(n)]
@@ -70,35 +72,41 @@
 
     def reconstruct(self, X: np.ndarray) -> np.ndarray:
         # Project X onto the line
         return X * np.array(
             [[1.0, 1.0, 1.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0]]
         ) - np.array([[0.0, 0.0, 0.0, 0.42, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]])
 
+    def is_in_distribution(self, X: np.ndarray) -> np.ndarray:
+        # Can only be ID if the constant feature value matches
+        return X[:, 3] == -0.42
+
     @property
     def aspect_ratio(self) -> float:
         return 1.0
 
     def plot(
         self,
         conf: np.ndarray,
         ax: mpl.axes.Axes,
         cmap: Union[str, mpl.colors.Colormap],
+        with_scatter: bool = True,
     ):
         ax.spines["top"].set_visible(False)
         ax.spines["right"].set_visible(False)
         ax.spines["bottom"].set_visible(False)
         ax.spines["left"].set_visible(False)
 
         ax.set_xticks([-0.42 - 0.4, -0.42, -0.42 + 0.4])
         ax.set_xticklabels([r"$-0.4 \sigma$", "const", r"$+0.4 \sigma$"])
         ax.get_yaxis().set_visible(False)
 
         ax.axvline(-0.42, c="white", lw=7, zorder=-1)
 
+        # with_scatter is ignored
         ax.scatter(self.X_test[:, 3], conf, c="white", s=6, rasterized=True)
         ax.scatter(self.X_test[:, 3], conf, c="black", s=1, rasterized=True)
 
         ax.imshow(
             [[x / 100, x / 100] for x in range(100, -1, -1)],
             cmap=cmap,
             interpolation="bicubic",
```

### Comparing `phepy-0.0.0/phepy/toys/line.py` & `phepy-0.1.0/phepy/toys/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import matplotlib as mpl
 import numpy as np
 
 from . import ToyExample
 
 
 class LineToyExample(ToyExample):
-    def __init__(self, rng: np.random.Generator) -> LineToyExample:
-        N = 10_000
-
+    def __init__(
+        self, rng: np.random.Generator, N: int = 10_000
+    ) -> LineToyExample:
         X1 = np.concatenate(
             [np.linspace(0, 4, N // 2), np.linspace(6, 10, N // 2)]
         )
         X2 = 1 + X1 * 0.5 + rng.normal(loc=0.0, scale=0.1, size=N)
         X1 += rng.normal(loc=0.0, scale=0.1, size=N)
 
         self.__X_train = np.stack([X1, X2], axis=1)
@@ -59,47 +59,55 @@
     def reconstruct(self, X: np.ndarray) -> np.ndarray:
         # Project X onto the line
         return np.array([[0.0, 1.0]]) + np.array([[1.0, 0.5]]) * (
             np.matmul((X - np.array([0.0, 1.0])), np.array([[1.0], [0.5]]))
             / np.matmul(np.array([[1.0, 0.5]]), np.array([[1.0], [0.5]]))
         )
 
+    def is_in_distribution(self, X: np.ndarray) -> np.ndarray:
+        # Two standard deviations off the mean -> 95.45% interval
+        return np.linalg.norm(X - self.reconstruct(X), axis=1) <= 0.2
+
     @property
     def aspect_ratio(self) -> float:
         return 14 / 9
 
     def plot(
         self,
         conf: np.ndarray,
         ax: mpl.axes.Axes,
         cmap: Union[str, mpl.colors.Colormap],
+        with_scatter: bool = True,
     ):
+        N_skip = len(self.X_train) // 40
+
         ax.imshow(
             conf.reshape(np.mgrid[-2:12:0.01, -1:8:0.01][0].shape).T,
             cmap=cmap,
             vmin=0.0,
             vmax=1.0,
             extent=[-2, 12, -1, 8],
             origin="lower",
             interpolation="bicubic",
             rasterized=True,
         )
 
         ax.set_xlim(-2, 12)
         ax.set_ylim(-1, 8)
 
-        ax.scatter(
-            self.X_train[::250, 0],
-            self.X_train[::250, 1],
-            c="white",
-            marker="x",
-            lw=3,
-            s=48,
-        )
-        ax.scatter(
-            self.X_train[::250, 0],
-            self.X_train[::250, 1],
-            c="black",
-            marker="x",
-        )
+        if with_scatter:
+            ax.scatter(
+                self.X_train[::N_skip, 0],
+                self.X_train[::N_skip, 1],
+                c="white",
+                marker="x",
+                lw=3,
+                s=48,
+            )
+            ax.scatter(
+                self.X_train[::N_skip, 0],
+                self.X_train[::N_skip, 1],
+                c="black",
+                marker="x",
+            )
 
         ax.axis("off")
```

### Comparing `phepy-0.0.0/phepy.egg-info/PKG-INFO` & `phepy-0.1.0/phepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phepy
-Version: 0.0.0
+Version: 0.1.0
 Summary: Intuitive evaluation of out-of-distribution detectors using simple toy examples.
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -209,19 +209,22 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: example
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
-# phepy &emsp; [![PyPi]][pypi-url] [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![CI Status]][ci-status]
+# phepy &emsp; [![PyPi]][pypi-url]  [![License Apache-2.0]][apache-2.0] [![License MIT]][mit] [![Docs]][docs-stable] [![CI Status]][ci-status]
 
 [PyPI]: https://img.shields.io/pypi/v/phepy
 [pypi-url]: https://pypi.org/project/phepy
 
+[Docs]: https://img.shields.io/pypi/v/phepy?color=blue&label=Docs
+[docs-stable]: https://juntyr.github.io/phepy/
+
 [License Apache-2.0]: https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg
 [apache-2.0]: https://opensource.org/licenses/Apache-2.0
 
 [License MIT]: https://img.shields.io/badge/License-MIT-yellow.svg
 [mit]: https://opensource.org/licenses/MIT
 
 [CI Status]: https://img.shields.io/github/actions/workflow/status/juntyr/phepy/ci.yml?branch=main&label=CI
@@ -253,15 +256,15 @@
 Next, enter the repository folder and use `pip` to install the program:
 ```bash
 cd phepy && pip install .
 ```
 
 ## Usage Example
 
-The following code snippet only provides a minimal example to get started, please refer to the [`examples`](examples) folder to find more extensive examples.
+The following code snippet only provides a minimal example to get started, please refer to the [`examples`](https://github.com/juntyr/phepy/tree/main/examples) folder to find more extensive examples.
 
 ```python
 # Import numpy, matplotlib, and sklearn
 import numpy as np
 import sklearn
 
 from matplotlib import pyplot as plt
@@ -310,15 +313,15 @@
     toys = [line, circle, haystack],
     cmap = "coolwarm", # use e.g. "viridis" to be colour-blind safe
 )
 
 plt.show()
 ```
 
-![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](examples/minimal.png)
+![By-example evaluation of Local Outlier Factor as a distance-based OOD detection method](https://raw.githubusercontent.com/juntyr/phepy/main/examples/minimal.png)
 
 In the above figure, the single row showcases the Local Outlier Factor (LOF, [^1]) method, while the three columns contain the following three test cases:
 
 * Two groups of training points are scattered along a line in the 2D feature space. The target variable only depends on the location along the line. In this example, points off the line are OOD.
 * The training points are scattered around the sine-displaced boundary of a circle, but none are inside it. The target variable only depends on the location along the boundary. Again, points off the line are OOD.
 * The training points are sampled from a 10-dimensional multivariate normal distribution, where one of the features is set to a constant. This example tests whether an OOD detection method can find a needle in a high-dimensional haystack, i.e. identify that points which do not share the constant are OOD.
 
@@ -326,21 +329,21 @@
 
 The Local Outlier Factor (LOF, [^1]) estimates the training data density around unseen data. Thus, it performs quite well on the line and circle examples where the data points are closely scattered. The LOF classifies the gap between the two groups of training inputs on the line as out-of-distribution (OOD), which may be too conservative if we assume that a machine-learning model can interpolate between the two groups. While LOF produces slightly lower confidence for the OOD inputs in the haystack, it does not clearly identify test data that do not have the constant feature seen in training as out-of-distribution.
 
 ## License
 
 Licensed under either of
 
-* Apache License, Version 2.0 ([`LICENSE-APACHE`](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
-* MIT license ([`LICENSE-MIT`](LICENSE-MIT) or http://opensource.org/licenses/MIT)
+* Apache License, Version 2.0 ([`LICENSE-APACHE`](https://github.com/juntyr/phepy/blob/main/LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
+* MIT license ([`LICENSE-MIT`](https://github.com/juntyr/phepy/blob/main/LICENSE-MIT) or http://opensource.org/licenses/MIT)
 
 at your option.
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.
 
 ## Citation
 
-Please refer to the [CITATION.cff](CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
+Please refer to the [CITATION.cff](https://github.com/juntyr/phepy/blob/main/CITATION.cff) file and refer to https://citation-file-format.github.io to extract the citation in a format of your choice.
 
 [^1]: M. M. Breunig *et al*. LOF: Identifying Density-Based Local Outliers. *Proceedings of the 2000 ACM SIGMOD International Conference on Management of Data*. SIGMOD '00. Dallas, Texas, USA: Associ- ation for Computing Machinery, 2000, 93–104. Available from: [doi:10.1145/342009.335388](https://doi.org/10.1145/342009.335388).
```

### Comparing `phepy-0.0.0/pyproject.toml` & `phepy-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phepy"
-version = "0.0.0"
+version = "0.1.0"
 requires-python = ">=3.7"
 description = "Intuitive evaluation of out-of-distribution detectors using simple toy examples."
 readme = "README.md"
 license = { file = "LICENSE-APACHE" }
 authors = [
     { name = "Juniper Tyree", email = "juniper.tyree@helsinki.fi" }
 ]
@@ -47,8 +47,8 @@
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"CITATION.cff" = ['^version: {version}', "^commit: '{version}'", 'https://pypi.org/project/phepy/{version}/', 'https://github.com/juntyr/phepy/releases/tag/{version}', "date-released: 'YYYY-0M-0D'"]
+"CITATION.cff" = ['^version: {version}', "^commit: 'v{version}'", 'https://pypi.org/project/phepy/{version}/', 'https://github.com/juntyr/phepy/releases/tag/v{version}', "date-released: 'YYYY-0M-0D'"]
```

