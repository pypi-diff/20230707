# Comparing `tmp/pcg_springer_features-0.2.tar.gz` & `tmp/pcg_springer_features-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pcg_springer_features-0.2.tar", last modified: Tue Jan  3 07:56:28 2023, max compression
+gzip compressed data, was "pcg_springer_features-0.3.tar", last modified: Fri Jul  7 01:48:10 2023, max compression
```

## Comparing `pcg_springer_features-0.2.tar` & `pcg_springer_features-0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      244 2022-05-23 16:36:53.000000 pcg_springer_features-0.2/pcg_springer_features/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3933 2023-01-02 16:27:14.000000 pcg_springer_features-0.2/pcg_springer_features/springer_dwt.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6988 2023-01-02 16:22:14.000000 pcg_springer_features-0.2/pcg_springer_features/springer_features.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2171 2023-01-03 07:48:26.000000 pcg_springer_features-0.2/pcg_springer_features/schmidt_spike_removal.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2363 2023-01-02 16:22:14.000000 pcg_springer_features-0.2/pcg_springer_features/schmidt_heart_rate.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       20 2023-01-03 07:52:32.000000 pcg_springer_features-0.2/pcg_springer_features/version.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      767 2023-01-02 08:14:29.000000 pcg_springer_features-0.2/README.md
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1512 2023-01-02 08:03:10.000000 pcg_springer_features-0.2/setup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/setup.cfg
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/top_level.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      573 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/SOURCES.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/dependency_links.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1696 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/PKG-INFO
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/pcg_springer_features.egg-info/requires.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1696 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/PKG-INFO
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2023-01-03 07:56:28.000000 pcg_springer_features-0.2/test/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1473 2023-01-03 07:48:40.000000 pcg_springer_features-0.2/test/test_schmidt_spike_removal.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1299 2023-01-02 15:16:19.000000 pcg_springer_features-0.2/test/test_springer_features.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2499 2023-01-02 16:32:22.000000 pcg_springer_features-0.2/test/test_springer_dwt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:48:10.443329 pcg_springer_features-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 01:48:10.443329 pcg_springer_features-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:48:10.439329 pcg_springer_features-0.3/pcg_springer_features/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/schmidt_heart_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/schmidt_spike_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/springer_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/springer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/pcg_springer_features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:48:10.439329 pcg_springer_features-0.3/pcg_springer_features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 01:48:10.000000 pcg_springer_features-0.3/pcg_springer_features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 01:48:10.000000 pcg_springer_features-0.3/pcg_springer_features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:48:10.000000 pcg_springer_features-0.3/pcg_springer_features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 01:48:10.000000 pcg_springer_features-0.3/pcg_springer_features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 01:48:10.000000 pcg_springer_features-0.3/pcg_springer_features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:48:10.443329 pcg_springer_features-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:48:10.439329 pcg_springer_features-0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/test/test_schmidt_spike_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/test/test_springer_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-07 01:45:08.000000 pcg_springer_features-0.3/test/test_springer_features.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pcg_springer_features-0.2/pcg_springer_features/springer_dwt.py` & `pcg_springer_features-0.3/pcg_springer_features/springer_dwt.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,34 +13,40 @@
     "get_full_dwt_features",
 ]
 
 
 def get_dwt_features(
     signal: np.ndarray, fs: int, config: Optional[dict] = None
 ) -> np.ndarray:
-    """
-    compute the discrete wavelet transform (DWT) features using Springer's algorithm
+    """Compute the discrete wavelet transform (DWT)
+    features using Springer's algorithm [1]_.
 
     Parameters
     ----------
-    signal : np.ndarray,
-        the (PCG) signal, of shape (nsamples,)
-    fs : int,
-        the sampling frequency
-    config : dict, optional,
-        the configuration, with the following keys:
-        - ``'wavelet_level'``: int,
+    signal : numpy.ndarray
+        The (PCG) signal, of shape ``(nsamples,)``.
+    fs : int
+        Sampling frequency of the signal.
+    config : dict, optional
+        The configuration for computing the features, with the following items:
+
+        - ``'wavelet_level'`` : int,
             the level of the wavelet decomposition, default: 3
-        - ``'wavelet_name'``: str,
+        - ``'wavelet_name'`` : str,
             the name of the wavelet, default: "db7"
 
     Returns
     -------
-    dwt_features : np.ndarray,
-        the DWT features, of shape (nsamples,)
+    dwt_features : numpy.ndarray
+        The DWT features, of shape ``(nsamples,)``.
+
+    References
+    ----------
+    .. [1] Springer, David B., Lionel Tarassenko, and Gari D. Clifford. "Logistic regression-HSMM-based heart sound segmentation."
+           IEEE transactions on biomedical engineering 63.4 (2015): 822-832.
 
     """
     cfg = ED(
         wavelet_level=3,
         wavelet_name="db7",
     )
     cfg.update(config or {})
```

### Comparing `pcg_springer_features-0.2/pcg_springer_features/springer_features.py` & `pcg_springer_features-0.3/pcg_springer_features/springer_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,46 +21,53 @@
 def get_springer_features(
     signal: np.ndarray,
     fs: int,
     feature_fs: int,
     feature_format: str = "flat",
     config: Optional[dict] = None,
 ) -> np.ndarray:
-    """
-    This function **almost** re-implements the original matlab
-    implementation of the Springer features.
+    """This function **almost** re-implements the original matlab
+    implementation of the Springer features [1]_ [2]_.
 
     Parameters
     ----------
-    signal: np.ndarray,
+    signal : numpy.ndarray
         The signal (1D) to extract features from.
-    fs: int,
-        The sampling frequency of the signal.
-    feature_fs: int,
-        The sampling frequency of the features.
-    feature_format: str, default "flat",
-        The format of the features, can be one of
-        "flat", "channel_first", "channel_last",
-        case insensitive.
-    config: dict, optional,
+    fs : int
+        Sampling frequency of the signal.
+    feature_fs : int
+        Sampling frequency of the features.
+    feature_format : {"flat", "channel_first", "channel_last"}
+        The format of the features, case insensitive.
+        By default, "flat".
+    config : dict, optional
         The configuration for extraction methods of the features.
 
     Returns
     -------
-    springer_features: np.ndarray,
+    springer_features : numpy.ndarray
         The extracted features, of shape
-        (4 * feature_len,) if `feature_format` is "flat",
-        (4, feature_len) if `feature_format` is "channel_first",
-        (feature_len, 4) if `feature_format` is "channel_last".
+
+        - ``(4 * feature_len,)`` if `feature_format` is ``"flat"``,
+        - ``(4, feature_len)`` if `feature_format` is ``"channel_first"``,
+        - ``(feature_len, 4)`` if `feature_format` is ``"channel_last"``.
+
         The features are in the following order:
+
         - homomorphic_envelope
         - hilbert envelope
         - PSD
         - DWT
 
+    References
+    ----------
+    .. [1] Springer, David B., Lionel Tarassenko, and Gari D. Clifford. "Logistic regression-HSMM-based heart sound segmentation."
+           IEEE transactions on biomedical engineering 63.4 (2015): 822-832.
+    .. [2] https://physionet.org/content/hss/1.0/
+
     """
     assert feature_format.lower() in [
         "flat",
         "channel_first",
         "channel_last",
     ], f"`feature_format` must be one of 'flat', 'channel_first', 'channel_last', but got {feature_format}"
     cfg = ED(
```

### Comparing `pcg_springer_features-0.2/pcg_springer_features/schmidt_spike_removal.py` & `pcg_springer_features-0.3/pcg_springer_features/schmidt_spike_removal.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,38 @@
 def schmidt_spike_removal(
     original_signal: np.ndarray,
     fs: int,
     window_size: float = 0.5,
     threshold: float = 3.0,
     eps: float = 1e-4,
 ) -> np.ndarray:
-    """
-    spike removal using Schmidt algorithm
+    """Spike removal using Schmidt algorithm [1]_.
 
     Parameters
     ----------
-    original_signal : np.ndarray,
-        the original signal
-    fs : int,
-        the sampling frequency
-    window_size : float, default 0.5,
-        the sliding window size, with units in seconds
-    threshold : float, default 3.0,
-        the threshold (multiplier for the median value) for detecting spikes
-    eps : float, default 1e-4,
-        the epsilon for numerical stability
+    original_signal : numpy.ndarray
+        The original signal.
+    fs : int
+        Sampling frequency of the signal.
+    window_size : float, default 0.5
+        Sliding window size, with units in seconds.
+    threshold : float, default 3.0
+        Threshold (multiplier for the median value) for detecting spikes.
+    eps : float, default 1e-4
+        Epsilon for numerical stability.
 
     Returns
     -------
-    despiked_signal : np.ndarray,
-        the despiked signal
+    despiked_signal : numpy.ndarray
+        Despiked signal.
+
+    References
+    ----------
+    .. [1] Schmidt, Samuel E., et al. "Segmentation of heart sound recordings by a duration-dependent hidden Markov model."
+           Physiological measurement 31.4 (2010): 513.
 
     """
     window_size = round(fs * window_size)
     nframes, res = divmod(original_signal.shape[0], window_size)
     frames = original_signal[: window_size * nframes].reshape((nframes, window_size))
     if res > 0:
         nframes += 1
```

### Comparing `pcg_springer_features-0.2/pcg_springer_features/schmidt_heart_rate.py` & `pcg_springer_features-0.3/pcg_springer_features/schmidt_heart_rate.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,41 +15,49 @@
     "get_schmidt_heart_rate",
 ]
 
 
 def get_schmidt_heart_rate(
     signal: np.ndarray, fs: int, config: Optional[dict] = None
 ) -> Tuple[float, float]:
-    """
-    compute heart rate from (PCG) signal using Schmidt algorithm (using autocorrelation)
+    """Compute heart rate from (PCG) signal using
+    Schmidt algorithm (an autocorrelation-based method) [1]_ [2]_.
 
     Parameters
     ----------
-    signal : np.ndarray,
-        the (PCG) signal
-    fs : int,
-        the sampling frequency
-    config : dict, optional,
+    signal : numpy.ndarray
+        The (PCG) signal.
+    fs : int
+        Sampling frequency of the signal.
+    config : dict, optional
         the configuration, with the following keys:
-        - ``'order'``: int,
+
+        - ``'order'`` : int,
             the order of the filter, default: 2
-        - ``'lowcut'``: real number,
+        - ``'lowcut'`` : real number,
             the low cutoff frequency, default: 25
-        - ``'highcut'``: real number,
+        - ``'highcut'`` : real number,
             the high cutoff frequency, default: 400
-        - ``'lpf_freq'``: real number,
+        - ``'lpf_freq'`` : real number,
             the frequency of the low pass filter for computing the envelope,
             default 8
 
     Returns
     -------
-    mean_hr : float,
-        the mean heart rate
-    systolic_time_interval: float,
-        the systolic time interval
+    mean_hr : float
+        Mean heart rate.
+    systolic_time_interval : float
+        Systolic time interval.
+
+    References
+    ----------
+    .. [1] Schmidt, Samuel E., et al. "Segmentation of heart sound recordings by a duration-dependent hidden Markov model."
+           Physiological measurement 31.4 (2010): 513.
+    .. [2] Springer, David B., Lionel Tarassenko, and Gari D. Clifford. "Logistic regression-HSMM-based heart sound segmentation."
+           IEEE transactions on biomedical engineering 63.4 (2015): 822-832.
 
     """
     cfg = ED(
         order=2,
         lowcut=25,
         highcut=400,
         lpf_freq=8,
```

### Comparing `pcg_springer_features-0.2/README.md` & `pcg_springer_features-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pcg_springer_features-0.2/setup.py` & `pcg_springer_features-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pcg_springer_features-0.2/pcg_springer_features.egg-info/SOURCES.txt` & `pcg_springer_features-0.3/pcg_springer_features.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 pcg_springer_features/__init__.py
 pcg_springer_features/schmidt_heart_rate.py
 pcg_springer_features/schmidt_spike_removal.py
 pcg_springer_features/springer_dwt.py
 pcg_springer_features/springer_features.py
```

### Comparing `pcg_springer_features-0.2/pcg_springer_features.egg-info/PKG-INFO` & `pcg_springer_features-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
-Name: pcg-springer-features
-Version: 0.2
+Name: pcg_springer_features
+Version: 0.3
 Summary: Tools for Computation of Springer's Features from Phonocardiogram (PCG).
 Home-page: https://github.com/DeepPSP/pcg_springer_features
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
-Description: # pcg_springer_features
-        
-        Computation of Springer's Features from Phonocardiogram (PCG)
-        
-        ![format-check](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/check-formatting.yml/badge.svg)
-        ![pytest](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/run-pytest.yml/badge.svg)
-        [![codecov](https://codecov.io/gh/DeepPSP/pcg_springer_features/branch/master/graph/badge.svg?token=LIML5LHY3Q)](https://codecov.io/gh/DeepPSP/pcg_springer_features)
-        ![PyPI](https://img.shields.io/pypi/v/pcg_springer_features?style=flat-square)
-        ![downloads](https://img.shields.io/pypi/dm/pcg_springer_features?style=flat-square)
-        
-        A part (feature extraction) of the [original Matlab code](https://physionet.org/content/hss/1.0/) is re-implemented using Python.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+# pcg_springer_features
+
+Computation of Springer's Features from Phonocardiogram (PCG)
+
+![format-check](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/check-formatting.yml/badge.svg)
+![pytest](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/run-pytest.yml/badge.svg)
+[![codecov](https://codecov.io/gh/DeepPSP/pcg_springer_features/branch/master/graph/badge.svg?token=LIML5LHY3Q)](https://codecov.io/gh/DeepPSP/pcg_springer_features)
+![PyPI](https://img.shields.io/pypi/v/pcg_springer_features?style=flat-square)
+![downloads](https://img.shields.io/pypi/dm/pcg_springer_features?style=flat-square)
+
+A part (feature extraction) of the [original Matlab code](https://physionet.org/content/hss/1.0/) is re-implemented using Python.
```

### Comparing `pcg_springer_features-0.2/PKG-INFO` & `pcg_springer_features-0.3/pcg_springer_features.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
-Name: pcg_springer_features
-Version: 0.2
+Name: pcg-springer-features
+Version: 0.3
 Summary: Tools for Computation of Springer's Features from Phonocardiogram (PCG).
 Home-page: https://github.com/DeepPSP/pcg_springer_features
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
-Description: # pcg_springer_features
-        
-        Computation of Springer's Features from Phonocardiogram (PCG)
-        
-        ![format-check](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/check-formatting.yml/badge.svg)
-        ![pytest](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/run-pytest.yml/badge.svg)
-        [![codecov](https://codecov.io/gh/DeepPSP/pcg_springer_features/branch/master/graph/badge.svg?token=LIML5LHY3Q)](https://codecov.io/gh/DeepPSP/pcg_springer_features)
-        ![PyPI](https://img.shields.io/pypi/v/pcg_springer_features?style=flat-square)
-        ![downloads](https://img.shields.io/pypi/dm/pcg_springer_features?style=flat-square)
-        
-        A part (feature extraction) of the [original Matlab code](https://physionet.org/content/hss/1.0/) is re-implemented using Python.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+# pcg_springer_features
+
+Computation of Springer's Features from Phonocardiogram (PCG)
+
+![format-check](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/check-formatting.yml/badge.svg)
+![pytest](https://github.com/DeepPSP/pcg_springer_features/actions/workflows/run-pytest.yml/badge.svg)
+[![codecov](https://codecov.io/gh/DeepPSP/pcg_springer_features/branch/master/graph/badge.svg?token=LIML5LHY3Q)](https://codecov.io/gh/DeepPSP/pcg_springer_features)
+![PyPI](https://img.shields.io/pypi/v/pcg_springer_features?style=flat-square)
+![downloads](https://img.shields.io/pypi/dm/pcg_springer_features?style=flat-square)
+
+A part (feature extraction) of the [original Matlab code](https://physionet.org/content/hss/1.0/) is re-implemented using Python.
```

### Comparing `pcg_springer_features-0.2/test/test_schmidt_spike_removal.py` & `pcg_springer_features-0.3/test/test_schmidt_spike_removal.py`

 * *Files identical despite different names*

### Comparing `pcg_springer_features-0.2/test/test_springer_features.py` & `pcg_springer_features-0.3/test/test_springer_features.py`

 * *Files identical despite different names*

### Comparing `pcg_springer_features-0.2/test/test_springer_dwt.py` & `pcg_springer_features-0.3/test/test_springer_dwt.py`

 * *Files identical despite different names*

