# Comparing `tmp/nautilus-sampler-0.7.0.tar.gz` & `tmp/nautilus_sampler-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus-sampler-0.7.0.tar", last modified: Tue Jun 20 17:39:24 2023, max compression
+gzip compressed data, was "nautilus_sampler-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nautilus-sampler-0.7.0.tar` & `nautilus_sampler-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     8542 2023-06-20 17:19:59.212240 nautilus-sampler-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2022-09-13 17:16:29.198585 nautilus-sampler-0.7.0/LICENSE
--rw-r--r--   0        0        0     2609 2023-06-04 19:28:22.216277 nautilus-sampler-0.7.0/README.md
--rw-r--r--   0        0        0      218 2023-06-20 17:20:06.770110 nautilus-sampler-0.7.0/nautilus/__init__.py
--rw-r--r--   0        0        0      316 2023-04-13 13:59:25.226473 nautilus-sampler-0.7.0/nautilus/bounds/__init__.py
--rw-r--r--   0        0        0    22429 2023-06-09 12:58:17.902177 nautilus-sampler-0.7.0/nautilus/bounds/basic.py
--rw-r--r--   0        0        0    17825 2023-06-20 17:18:56.732706 nautilus-sampler-0.7.0/nautilus/bounds/neural.py
--rw-r--r--   0        0        0    13354 2023-06-20 17:18:56.733706 nautilus-sampler-0.7.0/nautilus/bounds/union.py
--rw-r--r--   0        0        0     5750 2023-06-09 12:58:17.902177 nautilus-sampler-0.7.0/nautilus/neural.py
--rw-r--r--   0        0        0     5967 2023-02-09 20:46:18.826604 nautilus-sampler-0.7.0/nautilus/prior.py
--rw-r--r--   0        0        0    49690 2023-06-20 17:18:56.733706 nautilus-sampler-0.7.0/nautilus/sampler.py
--rw-r--r--   0        0        0      676 2023-02-09 20:46:18.827604 nautilus-sampler-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3871 2023-05-29 16:06:55.225559 nautilus-sampler-0.7.0/tests/test_blobs.py
--rw-r--r--   0        0        0    14060 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_bounds.py
--rw-r--r--   0        0        0     5647 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_io.py
--rw-r--r--   0        0        0      486 2023-04-17 13:39:44.039203 nautilus-sampler-0.7.0/tests/test_neural.py
--rw-r--r--   0        0        0     1040 2023-06-12 14:24:46.370732 nautilus-sampler-0.7.0/tests/test_pool.py
--rw-r--r--   0        0        0     3714 2023-02-09 20:46:18.827604 nautilus-sampler-0.7.0/tests/test_prior.py
--rw-r--r--   0        0        0     7563 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_sampler.py
--rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 nautilus-sampler-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     8644 2023-07-07 10:14:17.431483 nautilus_sampler-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-04-08 20:18:18.001727 nautilus_sampler-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2938 2023-07-07 10:08:39.691790 nautilus_sampler-0.7.1/README.md
+-rw-r--r--   0        0        0      218 2023-07-07 10:14:38.112204 nautilus_sampler-0.7.1/nautilus/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-14 03:07:30.928925 nautilus_sampler-0.7.1/nautilus/bounds/__init__.py
+-rw-r--r--   0        0        0    22429 2023-06-07 11:06:55.121515 nautilus_sampler-0.7.1/nautilus/bounds/basic.py
+-rw-r--r--   0        0        0    17901 2023-07-07 10:09:46.370971 nautilus_sampler-0.7.1/nautilus/bounds/neural.py
+-rw-r--r--   0        0        0    13354 2023-06-22 17:16:37.897613 nautilus_sampler-0.7.1/nautilus/bounds/union.py
+-rw-r--r--   0        0        0     5757 2023-07-07 10:09:46.370971 nautilus_sampler-0.7.1/nautilus/neural.py
+-rw-r--r--   0        0        0     5967 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.1/nautilus/prior.py
+-rw-r--r--   0        0        0    49690 2023-06-22 17:16:37.899613 nautilus_sampler-0.7.1/nautilus/sampler.py
+-rw-r--r--   0        0        0      676 2023-04-08 20:18:18.032727 nautilus_sampler-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3871 2023-06-04 02:02:40.543916 nautilus_sampler-0.7.1/tests/test_blobs.py
+-rw-r--r--   0        0        0    14060 2023-06-22 17:16:37.953613 nautilus_sampler-0.7.1/tests/test_bounds.py
+-rw-r--r--   0        0        0     5647 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.1/tests/test_io.py
+-rw-r--r--   0        0        0      486 2023-04-14 03:07:30.932925 nautilus_sampler-0.7.1/tests/test_neural.py
+-rw-r--r--   0        0        0     1040 2023-06-04 02:02:40.544916 nautilus_sampler-0.7.1/tests/test_pool.py
+-rw-r--r--   0        0        0     3714 2023-04-08 20:18:18.033727 nautilus_sampler-0.7.1/tests/test_prior.py
+-rw-r--r--   0        0        0     7563 2023-06-22 17:16:37.954613 nautilus_sampler-0.7.1/tests/test_sampler.py
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 nautilus_sampler-0.7.1/PKG-INFO
```

### Comparing `nautilus-sampler-0.7.0/CHANGELOG.md` & `nautilus_sampler-0.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to nautilus will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.1] - 2023-07-07
+
+### Fixed
+- Parallelization with MPIPoolExecutor should now work correctly.
+
 ## [0.7.0] - 2023-06-20
 
 ### Changed
 - One can now change whether to discard points in the exploration phase after calling `run` by changing the `discard_exploration` argument of the sampler. To achieve this, information about points in the exploration phase is never dropped. Consequently, the sampler does not create a backup of the end of the exploration stage under "filename_exp.hdf5", anymore.
 - The computational overhead was slightly reduced when new bounds are rejected. Also, the output now specifically mentions when adding a new bound failed because the volume increased.
 - Added the function `sampler.asymptotic_sampling_efficiency` which returns an estimate of the sampling efficiency in the sampling phase.
```

### Comparing `nautilus-sampler-0.7.0/LICENSE` & `nautilus_sampler-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/README.md` & `nautilus_sampler-0.7.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![Logo](https://raw.githubusercontent.com/johannesulf/nautilus/main/docs/nautilus_text_image.png "Logo")
 
 [![Unit Testing Status](https://img.shields.io/github/actions/workflow/status/johannesulf/nautilus/tests.yml?branch=main&label=tests)](https://github.com/johannesulf/nautilus/actions)
-[![Code Coverage](https://img.shields.io/coverallsCoverage/github/johannesulf/nautilus)](https://coveralls.io/github/johannesulf/nautilus?branch=main)
 [![Documentation Status](https://img.shields.io/readthedocs/nautilus-sampler)](https://nautilus-sampler.readthedocs.io/en/latest/)
+[![Code Coverage](https://img.shields.io/coverallsCoverage/github/johannesulf/nautilus)](https://coveralls.io/github/johannesulf/nautilus?branch=main)
 [![PyPI](https://img.shields.io/pypi/v/nautilus-sampler?color=blue)](https://pypi.org/project/nautilus-sampler/)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/nautilus-sampler?color=blue)](https://anaconda.org/conda-forge/nautilus-sampler)
 [![License: MIT](https://img.shields.io/github/license/johannesulf/nautilus?color=blue)](https://raw.githubusercontent.com/johannesulf/nautilus/main/LICENSE)
 ![Language: Python](https://img.shields.io/github/languages/top/johannesulf/nautilus)
 
 Nautilus is an MIT-licensed pure-Python package for Bayesian posterior and evidence estimation. It utilizes importance sampling and efficient space exploration using neural networks. Compared to traditional MCMC and Nested Sampling codes, it needs fewer likelihood calls and produces much larger posterior samples. Additionally, nautilus is highly accurate and produces Bayesian evidence estimates with percent precision.
 
@@ -30,18 +30,32 @@
 
 sampler = Sampler(prior, likelihood)
 sampler.run(verbose=True)
 points, log_w, log_l = sampler.posterior()
 corner.corner(points, weights=np.exp(log_w), labels='abc')
 ```
 
+## Installation
+
+The most recent stable version of nautilus is listed in the Python Package Index (PyPI) and can be installed via ``pip``.
+
+```shell
+pip install nautilus-sampler
+```
+
+Additionally, nautilus is also on conda-forge. To install via ``conda`` use the following command.
+
+```shell
+conda install -c conda-forge nautilus-sampler
+```
+
 ## Documentation
 
 You can find the documentation at [nautilus-sampler.readthedocs.io](https://nautilus-sampler.readthedocs.io).
 
 ## Attribution
 
-A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper will be uploaded to arXiv around the end of June 2023. Please cite the paper, once available, if you found nautilus helpful in your research.
+A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper is available on [arXiv](https://arxiv.org/abs/2306.16923). Please cite the paper if you find nautilus helpful in your research.
 
 ## License
 
 Nautilus is licensed under the MIT License. The logo uses an image from the Illustris Collaboration.
```

### Comparing `nautilus-sampler-0.7.0/nautilus/bounds/basic.py` & `nautilus_sampler-0.7.1/nautilus/bounds/basic.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/nautilus/bounds/neural.py` & `nautilus_sampler-0.7.1/nautilus/bounds/neural.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         points = np.atleast_2d(points)
 
         in_bound = self.outer_bound.contains(points)
         if np.any(in_bound) and self.emulator is not None:
             points_t = self.outer_bound.transform(points)
             in_bound[in_bound] = (self.emulator.predict(points_t[in_bound]) >
                                   self.score_predict_min)
-
         return in_bound
 
     def write(self, group):
         """Write the bound to an HDF5 group.
 
         Parameters
         ----------
@@ -358,19 +357,20 @@
                     in_bound = np.any([bound.contains(points) for bound in
                                        self.neural_bounds], axis=0)
                     points = points[in_bound]
                     self.points = np.vstack([self.points, points])
                     self.n_sample += n_sample
                     self.n_reject += n_sample - len(points)
             else:
-                try:
-                    n_jobs = pool._processes
-                except AttributeError:
-                    n_jobs = pool.size
-                except AttributeError:
+                n_jobs = None
+                for attr in ['_processes', '_max_workers', 'size']:
+                    if hasattr(pool, attr):
+                        n_jobs = getattr(pool, attr)
+                        break
+                if n_jobs is None:
                     raise ValueError('Cannot determine size of pool.')
                 n_points_per_job = (
                     (max(n_points - len(self.points), 10000)) // n_jobs) + 1
                 func = partial(self._reset_and_sample, n_points_per_job)
                 rngs = [np.random.default_rng(seed) for seed in
                         np.random.SeedSequence(self.rng.integers(
                             2**32 - 1)).spawn(n_jobs)]
```

### Comparing `nautilus-sampler-0.7.0/nautilus/bounds/union.py` & `nautilus_sampler-0.7.1/nautilus/bounds/union.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/nautilus/neural.py` & `nautilus_sampler-0.7.1/nautilus/neural.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class NeuralNetworkEmulator():
     """Likelihood neural network emulator.
 
     Attributes
     ----------
     mean : numpy.ndarray
         Mean of input coordinates used for normalizing coordinates.
-    mean : numpy.ndarray
+    scale : numpy.ndarray
         Standard deviation of input coordinates used for normalizing
         coordinates.
     network : sklearn.neural_network.MLPRegressor
         Artifical neural network used for emulation.
 
     """
 
@@ -89,15 +89,15 @@
 
         f = partial(train_network, (x - emulator.mean) / emulator.scale, y,
                     neural_network_kwargs)
 
         if pool is None:
             emulator.neural_networks = list(map(f, range(n_networks)))
         else:
-            emulator.neural_networks = pool.map(f, range(n_networks))
+            emulator.neural_networks = list(pool.map(f, range(n_networks)))
 
         return emulator
 
     def predict(self, x):
         """Calculate the emulator likelihood prediction for a group of points.
 
         Parameters
```

### Comparing `nautilus-sampler-0.7.0/nautilus/prior.py` & `nautilus_sampler-0.7.1/nautilus/prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/nautilus/sampler.py` & `nautilus_sampler-0.7.1/nautilus/sampler.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/pyproject.toml` & `nautilus_sampler-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_blobs.py` & `nautilus_sampler-0.7.1/tests/test_blobs.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_bounds.py` & `nautilus_sampler-0.7.1/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_io.py` & `nautilus_sampler-0.7.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_pool.py` & `nautilus_sampler-0.7.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_prior.py` & `nautilus_sampler-0.7.1/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/tests/test_sampler.py` & `nautilus_sampler-0.7.1/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.7.0/PKG-INFO` & `nautilus_sampler-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus-sampler
-Version: 0.7.0
+Version: 0.7.1
 Summary: Neural Network-Boosted Importance Sampling for Bayesian Statistics
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
@@ -15,16 +15,16 @@
 Project-URL: Home, https://nautilus-sampler.readthedocs.io
 Provides-Extra: checkpointing
 Provides-Extra: tests
 
 ![Logo](https://raw.githubusercontent.com/johannesulf/nautilus/main/docs/nautilus_text_image.png "Logo")
 
 [![Unit Testing Status](https://img.shields.io/github/actions/workflow/status/johannesulf/nautilus/tests.yml?branch=main&label=tests)](https://github.com/johannesulf/nautilus/actions)
-[![Code Coverage](https://img.shields.io/coverallsCoverage/github/johannesulf/nautilus)](https://coveralls.io/github/johannesulf/nautilus?branch=main)
 [![Documentation Status](https://img.shields.io/readthedocs/nautilus-sampler)](https://nautilus-sampler.readthedocs.io/en/latest/)
+[![Code Coverage](https://img.shields.io/coverallsCoverage/github/johannesulf/nautilus)](https://coveralls.io/github/johannesulf/nautilus?branch=main)
 [![PyPI](https://img.shields.io/pypi/v/nautilus-sampler?color=blue)](https://pypi.org/project/nautilus-sampler/)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/nautilus-sampler?color=blue)](https://anaconda.org/conda-forge/nautilus-sampler)
 [![License: MIT](https://img.shields.io/github/license/johannesulf/nautilus?color=blue)](https://raw.githubusercontent.com/johannesulf/nautilus/main/LICENSE)
 ![Language: Python](https://img.shields.io/github/languages/top/johannesulf/nautilus)
 
 Nautilus is an MIT-licensed pure-Python package for Bayesian posterior and evidence estimation. It utilizes importance sampling and efficient space exploration using neural networks. Compared to traditional MCMC and Nested Sampling codes, it needs fewer likelihood calls and produces much larger posterior samples. Additionally, nautilus is highly accurate and produces Bayesian evidence estimates with percent precision.
 
@@ -48,19 +48,33 @@
 
 sampler = Sampler(prior, likelihood)
 sampler.run(verbose=True)
 points, log_w, log_l = sampler.posterior()
 corner.corner(points, weights=np.exp(log_w), labels='abc')
 ```
 
+## Installation
+
+The most recent stable version of nautilus is listed in the Python Package Index (PyPI) and can be installed via ``pip``.
+
+```shell
+pip install nautilus-sampler
+```
+
+Additionally, nautilus is also on conda-forge. To install via ``conda`` use the following command.
+
+```shell
+conda install -c conda-forge nautilus-sampler
+```
+
 ## Documentation
 
 You can find the documentation at [nautilus-sampler.readthedocs.io](https://nautilus-sampler.readthedocs.io).
 
 ## Attribution
 
-A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper will be uploaded to arXiv around the end of June 2023. Please cite the paper, once available, if you found nautilus helpful in your research.
+A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper is available on [arXiv](https://arxiv.org/abs/2306.16923). Please cite the paper if you find nautilus helpful in your research.
 
 ## License
 
 Nautilus is licensed under the MIT License. The logo uses an image from the Illustris Collaboration.
```

