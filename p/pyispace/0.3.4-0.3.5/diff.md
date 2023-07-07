# Comparing `tmp/pyispace-0.3.4.tar.gz` & `tmp/pyispace-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyispace-0.3.4.tar", last modified: Fri Sep  9 20:14:44 2022, max compression
+gzip compressed data, was "pyispace-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyispace-0.3.4.tar` & `pyispace-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-09-09 20:14:44.351919 pyispace-0.3.4/
--rw-rw-rw-   0        0        0     1089 2021-11-05 17:44:13.000000 pyispace-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     2359 2022-09-09 20:14:44.351919 pyispace-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1769 2022-05-20 12:08:49.000000 pyispace-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-09 20:14:44.347920 pyispace-0.3.4/pyispace/
--rw-rw-rw-   0        0        0      330 2021-11-05 17:44:13.000000 pyispace-0.3.4/pyispace/__init__.py
--rw-rw-rw-   0        0        0       75 2021-11-05 17:44:13.000000 pyispace-0.3.4/pyispace/__main__.py
--rw-rw-rw-   0        0        0     1543 2021-11-05 17:44:13.000000 pyispace-0.3.4/pyispace/cli.py
--rw-rw-rw-   0        0        0     1202 2021-11-05 17:44:13.000000 pyispace-0.3.4/pyispace/example.py
--rw-rw-rw-   0        0        0     3485 2021-11-05 17:44:13.000000 pyispace-0.3.4/pyispace/pilot.py
--rw-rw-rw-   0        0        0      514 2022-01-13 14:36:06.000000 pyispace-0.3.4/pyispace/preprocessing.py
--rw-rw-rw-   0        0        0    18573 2022-07-25 12:42:25.000000 pyispace-0.3.4/pyispace/trace.py
--rw-rw-rw-   0        0        0     6639 2022-09-09 20:02:39.000000 pyispace-0.3.4/pyispace/train.py
--rw-rw-rw-   0        0        0     3499 2021-11-05 18:17:06.000000 pyispace-0.3.4/pyispace/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-09 20:14:44.351919 pyispace-0.3.4/pyispace.egg-info/
--rw-rw-rw-   0        0        0     2359 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-09 20:14:44.000000 pyispace-0.3.4/pyispace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-09-09 20:14:44.352920 pyispace-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1070 2022-09-09 20:14:11.000000 pyispace-0.3.4/setup.py
+-rw-r--r--   0        0        0     1710 2023-07-07 19:18:02.786790 pyispace-0.3.5/README.md
+-rw-r--r--   0        0        0      340 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/__main__.py
+-rw-r--r--   0        0        0     1495 2023-07-07 19:18:02.786790 pyispace-0.3.5/pyispace/cli.py
+-rw-r--r--   0        0        0     1171 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/example.py
+-rw-r--r--   0        0        0     3382 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/pilot.py
+-rw-r--r--   0        0        0      495 2023-07-07 19:18:02.787790 pyispace-0.3.5/pyispace/preprocessing.py
+-rw-r--r--   0        0        0    18062 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/trace.py
+-rw-r--r--   0        0        0     6482 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/train.py
+-rw-r--r--   0        0        0     3414 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyispace/utils.py
+-rw-r--r--   0        0        0      948 2023-07-07 19:18:02.791790 pyispace-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyispace-0.3.5/PKG-INFO
```

### Comparing `pyispace-0.3.4/PKG-INFO` & `pyispace-0.3.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,81 @@
-Metadata-Version: 2.1
-Name: pyispace
-Version: 0.3.4
-Summary: Python Instance Space Analysis package
-Home-page: https://gitlab.com/ita-ml/pyispace
-Download-URL: https://gitlab.com/ita-ml/pyispace/-/archive/v0.3.4/pyispace-v0.3.4.tar.gz
-Author: Pedro Paiva
-Author-email: paiva@ita.br
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyISpace
-
-_Python Instance Space Analysis Toolkit_
-
-<!--![picture](docs/img/circle-fs.png)-->
-
-## Getting Started
-
-This is the Python version of the [Instance Space Analysis](https://github.com/andremun/InstanceSpace) (ISA) toolkit, originally written in Matlab code. The original ISA toolkit was developed as part of the project [MATILDA](https://matilda.unimelb.edu.au/matilda/about-matilda), at the University of Melbourne, Australia.
-
-PyISpace is a Python package that contains a subset of the tools present in the original Matlab code repository. It is not our intention to add new features to the toolkit. For a complete experience of all tools, we recommend the original code, or the [web version](https://matilda.unimelb.edu.au/matilda/).
-
-### Requirements
-Python 3.7 or newer.
-
-### Installation
-
-Via PyPi:
-
-```
-pip install pyispace
-```
-
-Or directly from the repository code:
-```
-git clone https://gitlab.com/ita-ml/pyispace.git
-cd pyispace/
-pip install -e .
-```
-
-
-### Usage
-
-1. Command Line Interface
-
-Inside the folder (`rootdir`) containing the required files [options.json](./options.json) and ``metadata.csv``, run  
-```
-isa
-```
-
-Optionally, the `rootdir` path may be passed with `-r` or `--rootdir`:
-```
-isa -r /Users/user/workspace/
-```
-
-For more information about these files, please refer to the original repository instructions.
-
-2. Python package
-
-```
-from pyispace import train_is
-model = train_is(metadata, opts)
-```
-
-#### Disabling messages
-PyISpace uses [logging](https://docs.python.org/3/library/logging.html) to display messages. You can disable the messages, for example, changing the level associated to the package: 
-
-```
-logging.getLogger("pyispace").setLevel(logging.ERROR)
-```
+Metadata-Version: 2.1
+Name: pyispace
+Version: 0.3.5
+Summary: Instance Space Analysis Python package
+Author-email: Pedro Paiva <paiva@ita.br>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Requires-Dist: numpy>=1.18.5
+Requires-Dist: scipy>=1.9.0
+Requires-Dist: scikit-learn>=0.23.1
+Requires-Dist: shapely~=1.8.0
+Requires-Dist: pandas>=1.1
+Requires-Dist: alphashape>=1.3.1
+Project-URL: repository, https://gitlab.com/ita-ml/pyispace
+
+# PyISpace
+
+_Python Instance Space Analysis Toolkit_
+
+<!--![picture](docs/img/circle-fs.png)-->
+
+## Getting Started
+
+This is the Python version of the [Instance Space Analysis](https://github.com/andremun/InstanceSpace) (ISA) toolkit, originally written in Matlab code. The original ISA toolkit was developed as part of the project [MATILDA](https://matilda.unimelb.edu.au/matilda/about-matilda), at the University of Melbourne, Australia.
+
+PyISpace is a Python package that contains a subset of the tools present in the original Matlab code repository. It is not our intention to add new features to the toolkit. For a complete experience of all tools, we recommend the original code, or the [web version](https://matilda.unimelb.edu.au/matilda/).
+
+### Requirements
+Python 3.7 or newer.
+
+### Installation
+
+Via PyPi:
+
+```
+pip install pyispace
+```
+
+Or directly from the repository code:
+```
+git clone https://gitlab.com/ita-ml/pyispace.git
+cd pyispace/
+pip install -e .
+```
+
+
+### Usage
+
+1. Command Line Interface
+
+Inside the folder (`rootdir`) containing the required files [options.json](./options.json) and ``metadata.csv``, run  
+```
+isa
+```
+
+Optionally, the `rootdir` path may be passed with `-r` or `--rootdir`:
+```
+isa -r /Users/user/workspace/
+```
+
+For more information about these files, please refer to the original repository instructions.
+
+2. Python package
+
+```
+from pyispace import train_is
+model = train_is(metadata, opts)
+```
+
+#### Disabling messages
+PyISpace uses [logging](https://docs.python.org/3/library/logging.html) to display messages. You can disable the messages, for example, changing the level associated to the package: 
+
+```
+logging.getLogger("pyispace").setLevel(logging.ERROR)
+```
```

### Comparing `pyispace-0.3.4/README.md` & `pyispace-0.3.5/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# PyISpace
-
-_Python Instance Space Analysis Toolkit_
-
-<!--![picture](docs/img/circle-fs.png)-->
-
-## Getting Started
-
-This is the Python version of the [Instance Space Analysis](https://github.com/andremun/InstanceSpace) (ISA) toolkit, originally written in Matlab code. The original ISA toolkit was developed as part of the project [MATILDA](https://matilda.unimelb.edu.au/matilda/about-matilda), at the University of Melbourne, Australia.
-
-PyISpace is a Python package that contains a subset of the tools present in the original Matlab code repository. It is not our intention to add new features to the toolkit. For a complete experience of all tools, we recommend the original code, or the [web version](https://matilda.unimelb.edu.au/matilda/).
-
-### Requirements
-Python 3.7 or newer.
-
-### Installation
-
-Via PyPi:
-
-```
-pip install pyispace
-```
-
-Or directly from the repository code:
-```
-git clone https://gitlab.com/ita-ml/pyispace.git
-cd pyispace/
-pip install -e .
-```
-
-
-### Usage
-
-1. Command Line Interface
-
-Inside the folder (`rootdir`) containing the required files [options.json](./options.json) and ``metadata.csv``, run  
-```
-isa
-```
-
-Optionally, the `rootdir` path may be passed with `-r` or `--rootdir`:
-```
-isa -r /Users/user/workspace/
-```
-
-For more information about these files, please refer to the original repository instructions.
-
-2. Python package
-
-```
-from pyispace import train_is
-model = train_is(metadata, opts)
-```
-
-#### Disabling messages
-PyISpace uses [logging](https://docs.python.org/3/library/logging.html) to display messages. You can disable the messages, for example, changing the level associated to the package: 
-
-```
-logging.getLogger("pyispace").setLevel(logging.ERROR)
+# PyISpace
+
+_Python Instance Space Analysis Toolkit_
+
+<!--![picture](docs/img/circle-fs.png)-->
+
+## Getting Started
+
+This is the Python version of the [Instance Space Analysis](https://github.com/andremun/InstanceSpace) (ISA) toolkit, originally written in Matlab code. The original ISA toolkit was developed as part of the project [MATILDA](https://matilda.unimelb.edu.au/matilda/about-matilda), at the University of Melbourne, Australia.
+
+PyISpace is a Python package that contains a subset of the tools present in the original Matlab code repository. It is not our intention to add new features to the toolkit. For a complete experience of all tools, we recommend the original code, or the [web version](https://matilda.unimelb.edu.au/matilda/).
+
+### Requirements
+Python 3.7 or newer.
+
+### Installation
+
+Via PyPi:
+
+```
+pip install pyispace
+```
+
+Or directly from the repository code:
+```
+git clone https://gitlab.com/ita-ml/pyispace.git
+cd pyispace/
+pip install -e .
+```
+
+
+### Usage
+
+1. Command Line Interface
+
+Inside the folder (`rootdir`) containing the required files [options.json](./options.json) and ``metadata.csv``, run  
+```
+isa
+```
+
+Optionally, the `rootdir` path may be passed with `-r` or `--rootdir`:
+```
+isa -r /Users/user/workspace/
+```
+
+For more information about these files, please refer to the original repository instructions.
+
+2. Python package
+
+```
+from pyispace import train_is
+model = train_is(metadata, opts)
+```
+
+#### Disabling messages
+PyISpace uses [logging](https://docs.python.org/3/library/logging.html) to display messages. You can disable the messages, for example, changing the level associated to the package: 
+
+```
+logging.getLogger("pyispace").setLevel(logging.ERROR)
 ```
```

### Comparing `pyispace-0.3.4/pyispace/cli.py` & `pyispace-0.3.5/pyispace/cli.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import time
-import argparse
-import json
-from pathlib import Path
-
-import pandas as pd
-
-from . import train_is
-from .utils import scriptcsv
-
-
-def main():
-    start = time.time()
-
-    parser = argparse.ArgumentParser(description="PyISpace - Python Instance Space Analysis toolkit.")
-    parser.add_argument('-r', '--rootdir', dest='rootdir', default=None, required=False, metavar='FILE',
-                        help="rootdir path")
-    args = parser.parse_args()
-
-    if args.rootdir is not None:
-        rootdir = Path(args.rootdir)
-        if not rootdir.exists():
-            raise NotADirectoryError(f"Invalid directory {repr(args.rootdir)}.")
-    else:
-        rootdir = Path().absolute()
-    print(f"Root Directory: {repr(str(rootdir))}")
-
-    opts_path = rootdir / 'options.json'
-    if opts_path.is_file():
-        with open(opts_path) as f:
-            opts = json.load(f)
-    else:
-        raise FileNotFoundError(f"File 'options.json' not found in specified path {repr(str(rootdir))}.")
-
-    print("Loading the data.")
-    meta_path = rootdir / 'metadata.csv'
-    if meta_path.is_file():
-        metadata = pd.read_csv(meta_path, index_col='instances')
-    else:
-        raise FileNotFoundError(f"File 'metadata.csv' not found in specified path {repr(str(rootdir))}.")
-
-    out = train_is(metadata, opts)
-
-    print("Writing the data on CSV files for posterior analysis.")
-    scriptcsv(out, rootdir)
-
-    end = time.time()
-    print(f"Completed! Elapsed time: {(end - start):.1f} s")
+import time
+import argparse
+import json
+from pathlib import Path
+
+import pandas as pd
+
+from . import train_is
+from .utils import scriptcsv
+
+
+def main():
+    start = time.time()
+
+    parser = argparse.ArgumentParser(description="PyISpace - Python Instance Space Analysis toolkit.")
+    parser.add_argument('-r', '--rootdir', dest='rootdir', default=None, required=False, metavar='FILE',
+                        help="rootdir path")
+    args = parser.parse_args()
+
+    if args.rootdir is not None:
+        rootdir = Path(args.rootdir)
+        if not rootdir.exists():
+            raise NotADirectoryError(f"Invalid directory {repr(args.rootdir)}.")
+    else:
+        rootdir = Path().absolute()
+    print(f"Root Directory: {repr(str(rootdir))}")
+
+    opts_path = rootdir / 'options.json'
+    if opts_path.is_file():
+        with open(opts_path) as f:
+            opts = json.load(f)
+    else:
+        raise FileNotFoundError(f"File 'options.json' not found in specified path {repr(str(rootdir))}.")
+
+    print("Loading the data.")
+    meta_path = rootdir / 'metadata.csv'
+    if meta_path.is_file():
+        metadata = pd.read_csv(meta_path, index_col='instances')
+    else:
+        raise FileNotFoundError(f"File 'metadata.csv' not found in specified path {repr(str(rootdir))}.")
+
+    out = train_is(metadata, opts)
+
+    print("Writing the data on CSV files for posterior analysis.")
+    scriptcsv(out, rootdir)
+
+    end = time.time()
+    print(f"Completed! Elapsed time: {(end - start):.1f} s")
```

### Comparing `pyispace-0.3.4/pyispace/example.py` & `pyispace-0.3.5/pyispace/example.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import json
-from pathlib import Path
-
-
-opts = {
-    "perf": {"MaxPerf": False, "AbsPerf": True, "epsilon": 0.69},
-    "general": {"betaThreshold": 0.55},
-    "parallel": {"flag": False, "ncores": 2},
-    "auto": {"preproc": True, "featsel": False},
-    "bound": {"flag": True},
-    "norm": {"flag": True},
-    "corr": {"flag": True, "threshold": 10},
-    "clust": {"flag": True, "KDEFAULT": 10, "SILTHRESHOLD": 0.9, "NTREES": 50, "MaxIter": 1000, "Replicates": 100},
-    "pilot": {"analytic": False, "ntries": 5},
-    "cloister": {"pval": 0.05, "cthres": 0.7},
-    "pythia": {"cvfolds": 5, "ispolykrnl": True, "useweights": False, "uselibsvm": False},
-    "trace": {"usesim": False, "PI": 0.55},
-    "selvars": {"smallscaleflag": False, "smallscale": 0.5, "fileidxflag": False, "fileidx": "", "densityflag": False,
-                "mindistance": 0.1},
-    "outputs": {"csv": True, "web": False, "png": False}
-}
-
-
-def save_opts(path):
-    path = Path(path)
-    if path.is_dir():
-        opts_path = path / 'options.json'
-        with open(opts_path, 'w') as f:
-            json.dump(opts, f)
-    else:
-        raise NotADirectoryError(f"Invalid directory '{str(path)}'.")
+import json
+from pathlib import Path
+
+
+opts = {
+    "perf": {"MaxPerf": False, "AbsPerf": True, "epsilon": 0.69},
+    "general": {"betaThreshold": 0.55},
+    "parallel": {"flag": False, "ncores": 2},
+    "auto": {"preproc": True, "featsel": False},
+    "bound": {"flag": True},
+    "norm": {"flag": True},
+    "corr": {"flag": True, "threshold": 10},
+    "clust": {"flag": True, "KDEFAULT": 10, "SILTHRESHOLD": 0.9, "NTREES": 50, "MaxIter": 1000, "Replicates": 100},
+    "pilot": {"analytic": False, "ntries": 5},
+    "cloister": {"pval": 0.05, "cthres": 0.7},
+    "pythia": {"cvfolds": 5, "ispolykrnl": True, "useweights": False, "uselibsvm": False},
+    "trace": {"usesim": False, "PI": 0.55},
+    "selvars": {"smallscaleflag": False, "smallscale": 0.5, "fileidxflag": False, "fileidx": "", "densityflag": False,
+                "mindistance": 0.1},
+    "outputs": {"csv": True, "web": False, "png": False}
+}
+
+
+def save_opts(path):
+    path = Path(path)
+    if path.is_dir():
+        opts_path = path / 'options.json'
+        with open(opts_path, 'w') as f:
+            json.dump(opts, f)
+    else:
+        raise NotADirectoryError(f"Invalid directory '{str(path)}'.")
```

### Comparing `pyispace-0.3.4/pyispace/pilot.py` & `pyispace-0.3.5/pyispace/pilot.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import logging
-import warnings
-from dataclasses import dataclass
-from typing import Tuple
-
-import numpy as np
-from scipy.linalg import eig
-from scipy.optimize import fmin_bfgs
-from scipy.spatial.distance import pdist
-
-
-_required_opts = ['analytic', 'ntries']
-_logger = logging.getLogger(__name__)
-
-
-@dataclass
-class PilotOutput:
-    A: np.ndarray
-    B: np.ndarray
-    C: np.ndarray
-    Z: np.ndarray
-    error: float
-    R2: np.ndarray
-
-
-def errorfcn(alpha, Xbar, n, m):
-    f1 = np.reshape(alpha[(2 * n):], (m, 2))
-    f2 = np.reshape(alpha[0:2 * n], (2, n))
-    f3 = Xbar[:, 0:n].T
-    r = (Xbar - np.dot(f1, np.dot(f2, f3)).T) ** 2
-    return np.nanmean(np.nanmean(r, axis=0))
-
-
-def pilot(X, Y, featlabels=None, **kwargs):
-    for opt in _required_opts:
-        if opt not in kwargs:
-            raise KeyError(f"Pilot required parameter {repr(opt)} missing.")
-
-    Xbar = np.hstack((X, Y))
-    n = X.shape[1]
-    m = Xbar.shape[1]
-
-    if kwargs['analytic']:
-        _logger.info("PILOT is solving analyticaly the projection problem.")
-        X = X.T
-        Xbar = Xbar.T
-
-        D, V = eig(np.dot(Xbar, Xbar.T), right=True, left=False)
-
-        idx = np.argsort(np.abs(D))[::-1]
-        V = V[:, idx[0:2]]
-        B = V[0:n, :]
-        C = V[n:m + 1, :].T
-        Xr = np.dot(X.T, np.linalg.pinv(np.dot(X, X.T)))
-        A = np.dot(V.T, np.dot(Xbar, Xr))
-        Z = np.dot(A, X)
-        Xhat = np.vstack((np.dot(B, Z), np.dot(C.T, Z)))
-        error = float(np.sum((Xbar - Xhat) ** 2))
-        R2 = np.diagonal(np.corrcoef(Xbar, Xhat, rowvar=False)[:m, m:]) ** 2
-        Z = Z.T
-    else:
-        _logger.info("PILOT is solving numerically the projection problem.")
-        ntries = kwargs['ntries']
-        seed = kwargs['seed'] if 'seed' in kwargs else 1
-        np.random.seed(seed)
-        X0 = 2 * np.random.random((ntries, 2 * m + 2 * n)).T - 1
-        alpha = np.zeros((2 * m + 2 * n, ntries))
-        eoptim = np.zeros(ntries)
-        perf = np.zeros(ntries)
-        Hd = pdist(X)[np.newaxis].T
-
-        for i in range(ntries):
-            alpha[:, i], eoptim[i] = fmin_bfgs(lambda a: errorfcn(a, Xbar, n, m), x0=X0[:, i],
-                                               full_output=True, disp=False)[:2]
-            aux = alpha[:, [i]]
-            A = np.reshape(aux[0:2 * n], (2, n))
-            Z = np.dot(X, A.T)
-            perf[i] = np.corrcoef(Hd, pdist(Z)[np.newaxis].T, rowvar=False)[0][1]
-            _logger.info(f"PILOT has completed trial {i+1}")
-
-        idx = np.argmax(perf)
-        A = np.reshape(alpha[0:2 * n, idx], (2, n))
-        Z = np.dot(X, A.T)
-        B = np.reshape(alpha[(2 * n):, idx], (m, 2))
-        Xhat = np.dot(Z, B.T)
-        C = B[n:m + 1, :].T
-        B = B[0:n + 1, :]
-        error = np.sum((Xbar - Xhat) ** 2)
-        with warnings.catch_warnings(record=True) as w:
-            R2 = np.diagonal(np.corrcoef(Xbar, Xhat, rowvar=False)[:m, m:]) ** 2
-
-    out = PilotOutput(A, B, C, Z, error, R2)
-    _logger.info("PILOT has completed.")
-    return out
-
-
-def adjust_rotation(Z: np.ndarray, Ybad: np.ndarray, theta: float = 135.0) -> Tuple[np.ndarray, np.ndarray]:
-    cenroid_bad = np.mean(Z[Ybad], axis=0)[::-1]
-    theta = np.radians(theta) - np.arctan2(*cenroid_bad)
-    rot = np.array(((np.cos(theta), -np.sin(theta)),
-                    (np.sin(theta), np.cos(theta))))
-    Z_rot = np.dot(rot, Z.T)
-    return Z_rot.T, rot
+import logging
+import warnings
+from dataclasses import dataclass
+from typing import Tuple
+
+import numpy as np
+from scipy.linalg import eig
+from scipy.optimize import fmin_bfgs
+from scipy.spatial.distance import pdist
+
+
+_required_opts = ['analytic', 'ntries']
+_logger = logging.getLogger(__name__)
+
+
+@dataclass
+class PilotOutput:
+    A: np.ndarray
+    B: np.ndarray
+    C: np.ndarray
+    Z: np.ndarray
+    error: float
+    R2: np.ndarray
+
+
+def errorfcn(alpha, Xbar, n, m):
+    f1 = np.reshape(alpha[(2 * n):], (m, 2))
+    f2 = np.reshape(alpha[0:2 * n], (2, n))
+    f3 = Xbar[:, 0:n].T
+    r = (Xbar - np.dot(f1, np.dot(f2, f3)).T) ** 2
+    return np.nanmean(np.nanmean(r, axis=0))
+
+
+def pilot(X, Y, featlabels=None, **kwargs):
+    for opt in _required_opts:
+        if opt not in kwargs:
+            raise KeyError(f"Pilot required parameter {repr(opt)} missing.")
+
+    Xbar = np.hstack((X, Y))
+    n = X.shape[1]
+    m = Xbar.shape[1]
+
+    if kwargs['analytic']:
+        _logger.info("PILOT is solving analyticaly the projection problem.")
+        X = X.T
+        Xbar = Xbar.T
+
+        D, V = eig(np.dot(Xbar, Xbar.T), right=True, left=False)
+
+        idx = np.argsort(np.abs(D))[::-1]
+        V = V[:, idx[0:2]]
+        B = V[0:n, :]
+        C = V[n:m + 1, :].T
+        Xr = np.dot(X.T, np.linalg.pinv(np.dot(X, X.T)))
+        A = np.dot(V.T, np.dot(Xbar, Xr))
+        Z = np.dot(A, X)
+        Xhat = np.vstack((np.dot(B, Z), np.dot(C.T, Z)))
+        error = float(np.sum((Xbar - Xhat) ** 2))
+        R2 = np.diagonal(np.corrcoef(Xbar, Xhat, rowvar=False)[:m, m:]) ** 2
+        Z = Z.T
+    else:
+        _logger.info("PILOT is solving numerically the projection problem.")
+        ntries = kwargs['ntries']
+        seed = kwargs['seed'] if 'seed' in kwargs else 1
+        np.random.seed(seed)
+        X0 = 2 * np.random.random((ntries, 2 * m + 2 * n)).T - 1
+        alpha = np.zeros((2 * m + 2 * n, ntries))
+        eoptim = np.zeros(ntries)
+        perf = np.zeros(ntries)
+        Hd = pdist(X)[np.newaxis].T
+
+        for i in range(ntries):
+            alpha[:, i], eoptim[i] = fmin_bfgs(lambda a: errorfcn(a, Xbar, n, m), x0=X0[:, i],
+                                               full_output=True, disp=False)[:2]
+            aux = alpha[:, [i]]
+            A = np.reshape(aux[0:2 * n], (2, n))
+            Z = np.dot(X, A.T)
+            perf[i] = np.corrcoef(Hd, pdist(Z)[np.newaxis].T, rowvar=False)[0][1]
+            _logger.info(f"PILOT has completed trial {i+1}")
+
+        idx = np.argmax(perf)
+        A = np.reshape(alpha[0:2 * n, idx], (2, n))
+        Z = np.dot(X, A.T)
+        B = np.reshape(alpha[(2 * n):, idx], (m, 2))
+        Xhat = np.dot(Z, B.T)
+        C = B[n:m + 1, :].T
+        B = B[0:n + 1, :]
+        error = np.sum((Xbar - Xhat) ** 2)
+        with warnings.catch_warnings(record=True) as w:
+            R2 = np.diagonal(np.corrcoef(Xbar, Xhat, rowvar=False)[:m, m:]) ** 2
+
+    out = PilotOutput(A, B, C, Z, error, R2)
+    _logger.info("PILOT has completed.")
+    return out
+
+
+def adjust_rotation(Z: np.ndarray, Ybad: np.ndarray, theta: float = 135.0) -> Tuple[np.ndarray, np.ndarray]:
+    cenroid_bad = np.mean(Z[Ybad], axis=0)[::-1]
+    theta = np.radians(theta) - np.arctan2(*cenroid_bad)
+    rot = np.array(((np.cos(theta), -np.sin(theta)),
+                    (np.sin(theta), np.cos(theta))))
+    Z_rot = np.dot(rot, Z.T)
+    return Z_rot.T, rot
```

### Comparing `pyispace-0.3.4/pyispace/trace.py` & `pyispace-0.3.5/pyispace/trace.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,511 +1,511 @@
-import logging
-import time
-import warnings
-from dataclasses import dataclass
-from itertools import repeat
-from math import ceil
-from multiprocessing import Pool, cpu_count
-from typing import List, Union
-
-import alphashape
-import numpy as np
-import pandas as pd
-from scipy.spatial import Delaunay
-from scipy.spatial.qhull import QhullError
-from scipy.special import gamma
-from shapely import geometry
-from shapely.ops import polygonize, triangulate, unary_union
-from sklearn.cluster import DBSCAN
-
-
-_required_opts = ['PI']
-_logger = logging.getLogger(__name__)
-
-
-# TODO: remove temporary workaround in future
-class AlphashapeFilter(logging.Filter):
-    def filter(self, record: logging.LogRecord) -> bool:
-        return "Likely caused by all points lying in an N-1 space" not in record.getMessage()
-
-
-logging.getLogger().addFilter(AlphashapeFilter())
-
-
-@dataclass
-class FootprintOutput:
-    polygon: geometry.MultiPolygon
-    area: float
-    elements: int
-    good_elements: int
-    density: float
-    purity: float
-
-
-def _empty_footprint() -> FootprintOutput:
-    return FootprintOutput(geometry.MultiPolygon(), 0, 0, 0, 0, 0)
-
-
-def _copy_footprint(obj: FootprintOutput) -> FootprintOutput:
-    return FootprintOutput(**obj.__dict__)
-
-
-@dataclass
-class TraceOutput:
-    space: FootprintOutput
-    good: List[FootprintOutput]
-    best: List[FootprintOutput]
-    hard: FootprintOutput
-    summary: pd.DataFrame
-
-
-class TraceException(Exception):
-    def __init__(self):
-        super().__init__("There are not enough instances to calculate a footprint. "
-                         "The subset of instances used is too small.")
-
-
-def alpha_shape(points: np.ndarray, alpha=1.0):
-    """
-    Compute the alpha shape (concave hull) of a set of points.
-
-    :param points: array of points (x,y)
-    :param float alpha: alpha value to influence the gooeyness of the border. Smaller numbers don't fall inward as much
-        as larger numbers. Too large, and you lose everything!
-    """
-    if len(points) < 3:
-        # When you have a triangle, there is no sense
-        # in computing an alpha shape.
-        return geometry.MultiPoint(list(points)).convex_hull, points
-    elif len(points) == 3:
-        return geometry.Polygon(points), points
-
-    # coords = np.array([point.coords[0] for point in points])
-    tri = Delaunay(points)
-    triangles = points[tri.simplices]
-    a = ((triangles[:, 0, 0] - triangles[:, 1, 0]) ** 2 + (triangles[:, 0, 1] - triangles[:, 1, 1]) ** 2) ** 0.5
-    b = ((triangles[:, 1, 0] - triangles[:, 2, 0]) ** 2 + (triangles[:, 1, 1] - triangles[:, 2, 1]) ** 2) ** 0.5
-    c = ((triangles[:, 2, 0] - triangles[:, 0, 0]) ** 2 + (triangles[:, 2, 1] - triangles[:, 0, 1]) ** 2) ** 0.5
-    s = (a + b + c) / 2.0
-    areas = (s * (s - a) * (s - b) * (s - c)) ** 0.5
-    circums = a * b * c / (4.0 * areas)
-    filtered = triangles[circums < (1.0 / alpha)]
-    edge1 = filtered[:, (0, 1)]
-    edge2 = filtered[:, (1, 2)]
-    edge3 = filtered[:, (2, 0)]
-    edge_points = np.unique(np.concatenate((edge1, edge2, edge3)), axis=0).tolist()
-    m = geometry.MultiLineString(edge_points)
-    triangles = list(polygonize(m))
-    return unary_union(triangles), edge_points
-
-
-def alphashape_optm(points: np.ndarray, alpha_ini):
-    # TODO: remove temporary workaround in future
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        points = list(map(tuple, points))
-        hull = alphashape.alphashape(points, alpha_ini)
-        if not isinstance(hull, geometry.Polygon):
-            alpha = 0.9 * alphashape.optimizealpha(points)
-            hull = alphashape.alphashape(points, alpha)
-        return hull
-
-
-def count_points(pts: Union[geometry.Point, geometry.MultiPoint]) -> int:
-    if pts.is_empty:
-        return 0
-    elif pts.type == 'Point':
-        return 1
-    elif pts.type == 'MultiPoint':
-        return len(pts.geoms)
-    else:
-        raise TypeError
-
-
-def inner_intersection(poly: geometry.Polygon, pts: geometry.MultiPoint) -> Union[geometry.Point, geometry.MultiPoint]:
-    intersec = poly.intersection(pts)
-    intersec_bound = poly.boundary.intersection(intersec)
-    return intersec.difference(intersec_bound)
-
-
-def copy_polygon(poly: Union[geometry.Polygon, geometry.MultiPolygon]):
-    return poly.__class__(poly)
-
-
-def estimate_epsilon(x, k):
-    m, n = np.shape(x)
-    eps = ((np.prod(x.max(axis=0) - x.min(axis=0)) * k * gamma(.5 * n + 1)) / (m * np.sqrt(np.pi ** n))) ** (1 / n)
-    return eps
-
-
-def make_summary(space: FootprintOutput, good: List[FootprintOutput], best: List[FootprintOutput], algolabels: List):
-    assert len(good) == len(best)
-    cols = ['Area_Good_Normalized', 'Density_Good_Normalized', 'Purity_Good',
-            'Area_Best_Normalized', 'Density_Best_Normalized', 'Purity_Best']
-    rows = []
-    for i in range(len(good)):
-        rows.append([good[i].area / space.area,
-                     good[i].density / space.density,
-                     good[i].purity,
-                     best[i].area / space.area,
-                     best[i].density / space.density,
-                     best[i].purity]
-                    )
-    summary = pd.DataFrame(rows, index=pd.Index(algolabels, name='Row'), columns=cols)
-    return summary
-
-
-def trace(Z: np.ndarray, Ybin: np.ndarray, P: np.ndarray, beta: np.ndarray, algolabels: list, parallel=True, **kwargs):
-    _logger.info("TRACE is calculating the space area and density.")
-    ninst = Z.shape[0]
-    nalgos = Ybin.shape[1]
-    space = trace_build(Z, np.ones(ninst, dtype=bool), kwargs['PI'])
-    _logger.debug(f"Space area: {space.area}")
-    _logger.debug(f"Space density: {space.density}")
-
-    _logger.info("TRACE is calculating the algorithm footprints.")
-    if parallel:
-        _logger.warning("Some log messages are temporarily disabled in parallel mode. This functionality will be added "
-                        "in future versions")
-        with Pool(processes=cpu_count()) as pool:
-            _logger.info(f"Calculating footprints...")
-            good = pool.starmap_async(trace_build_wrapper,
-                                      zip(repeat(Z), (Ybin[:, i] for i in range(nalgos)), repeat(kwargs['PI'])))
-            best = pool.starmap_async(trace_build_wrapper,
-                                      zip(repeat(Z), (P == i for i in range(nalgos)), repeat(kwargs['PI'])))
-            good = good.get()
-            best = best.get()
-    else:
-        good = []
-        best = []
-        for i in range(nalgos):
-            start = time.time()
-            _logger.info(f"Good performance footprint for {repr(algolabels[i])}")
-            try:
-                good.append(trace_build(Z, Ybin[:, i], kwargs['PI']))
-            except TraceException as e:
-                good.append(_empty_footprint())
-                _logger.warning(str(e))
-
-            _logger.info(f"Best performance footprint for {repr(algolabels[i])}")
-            try:
-                best.append(trace_build(Z, P == i, kwargs['PI']))
-            except TraceException as e:
-                good.append(_empty_footprint())
-                _logger.warning(str(e))
-
-            end = time.time()
-            _logger.debug(f"Algorithm {repr(algolabels[i])} completed. Elapsed time: {(end - start):.2f} s")
-
-    _logger.info("TRACE is detecting and removing contradictory sections of the footprints.")
-    for i in range(nalgos - 1):
-        _logger.debug(f"Base algorithm {repr(algolabels[i])}")
-        for j in range(i + 1, nalgos):
-            _logger.debug(f"TRACE is comparing {repr(algolabels[i])} with {repr(algolabels[j])}")
-            best[i], best[j] = trace_contra(best[i], best[j], Z, P == i, P == j, kwargs['PI'])
-            _logger.debug(f"Test algorithm {repr(algolabels[j])} completed.")
-        _logger.debug(f"Base algorithm {repr(algolabels[i])} completed.")
-
-    _logger.info("TRACE is calculating the beta-footprint.")
-    hard = trace_build_wrapper(Z, ~beta, kwargs['PI'])
-
-    _logger.info("TRACE is preparing the summary table.")
-    summary = make_summary(space, good, best, algolabels)
-    _logger.info("TRACE has completed.")
-    return TraceOutput(space, good, best, hard, summary)
-
-
-def trace_build_wrapper(*args):
-    try:
-        return trace_build(*args)
-    except TraceException:
-        return _empty_footprint()
-
-
-def trace_build(Z, Ybin, PI) -> FootprintOutput:
-    Ig = np.unique(Z[Ybin, :], axis=0)
-    if Ig.shape[0] < 3:
-        raise TraceException
-
-    nn = max(min(ceil(sum(Ybin) / 20), 50), 3)
-    eps = estimate_epsilon(Ig, nn)
-    clustering = DBSCAN(eps=eps, min_samples=nn).fit(Ig)
-
-    polygon = geometry.Polygon()
-    for i in range(np.max(clustering.labels_) + 1):
-        polydata = Ig[clustering.labels_ == i, :]
-        if polydata.shape[0] < 3:
-            continue
-
-        try:
-            concave_hull = alphashape_optm(polydata, 2)
-        except QhullError:
-            continue
-
-        if concave_hull.is_empty:
-            raise TraceException
-        else:
-            boundary = np.array(concave_hull.exterior.xy).T
-
-        aux = trace_fitpoly(boundary, Z, Ybin, PI)
-        if not aux.is_empty:
-            polygon = polygon.union(aux)
-
-    if not polygon.is_empty:
-        area = polygon.area
-        elements = count_points(polygon.intersection(geometry.MultiPoint(Z)))
-        good_elements = count_points(polygon.intersection(geometry.MultiPoint(Z[Ybin, :])))
-        density = elements / area
-        purity = good_elements / elements
-        return FootprintOutput(polygon, area, elements, good_elements, density, purity)
-    else:
-        raise TraceException
-
-
-def trace_contra(base: FootprintOutput, test: FootprintOutput, Z: np.ndarray,
-                 Ybase: np.ndarray, Ytest: np.ndarray, *args):
-    if base.polygon.is_empty or test.polygon.is_empty:
-        return base, test
-
-    def degenerate(p):
-        if not (isinstance(p, geometry.Polygon) or isinstance(p, geometry.MultiPolygon)):
-            return True
-        else:
-            return False
-
-    base = _copy_footprint(base)
-    base.polygon = copy_polygon(base.polygon)
-    test = _copy_footprint(test)
-    test.polygon = copy_polygon(test.polygon)
-
-    z_points = geometry.MultiPoint(Z)
-    z_base = geometry.MultiPoint(Z[Ybase, :])
-    z_test = geometry.MultiPoint(Z[Ytest, :])
-    contradiction = base.polygon.intersection(test.polygon)
-
-    maxtries = 3
-    numtries = 1
-
-    while (not contradiction.is_empty) and (numtries <= maxtries):
-        n_elements = count_points(contradiction.intersection(z_points))
-        if n_elements == 0:
-            break
-        n_good_elements_base = count_points(contradiction.intersection(z_base))
-        n_good_elements_test = count_points(contradiction.intersection(z_test))
-        purity_base = n_good_elements_base / n_elements
-        purity_test = n_good_elements_test / n_elements
-
-        if purity_base > purity_test:
-            test.polygon = test.polygon.difference(contradiction)
-            if numtries < maxtries:
-                test.polygon = trace_tight(test.polygon, Z, Ytest, *args)
-        elif purity_test > purity_base:
-            base.polygon = base.polygon.difference(contradiction)
-            if numtries < maxtries:
-                base.polygon = trace_tight(base.polygon, Z, Ybase, *args)
-        else:
-            break
-        if base.polygon.is_empty or test.polygon.is_empty:
-            break
-        else:
-            contradiction = base.polygon.intersection(test.polygon)
-            if degenerate(contradiction):
-                break
-        numtries += 1
-
-    if base.polygon.is_empty:
-        base = _empty_footprint()
-    else:
-        base.area = base.polygon.area
-        base.elements = count_points(base.polygon.intersection(z_points))
-        base.good_elements = count_points(base.polygon.intersection(z_base))
-        base.density = base.elements / base.area
-        base.purity = base.good_elements / base.elements
-    if test.polygon.is_empty:
-        test = _empty_footprint()
-    else:
-        test.area = test.polygon.area
-        test.elements = count_points(test.polygon.intersection(z_points))
-        test.good_elements = count_points(test.polygon.intersection(z_base))
-        test.density = test.elements / test.area
-        test.purity = test.good_elements / test.elements
-
-    return base, test
-
-
-def trace_tight(polygon: Union[geometry.Polygon, geometry.MultiPolygon],
-                Z: np.ndarray, Ybin: np.ndarray, *args):
-    if isinstance(polygon, geometry.Polygon):
-        nregions = 1
-        polygon = geometry.MultiPolygon([polygon])
-    else:
-        nregions = len(polygon.geoms)
-
-    z_points = geometry.MultiPoint(Z)
-    splits = []
-
-    for i in range(nregions):
-        criteria = inner_intersection(polygon.geoms[i], z_points)
-        if criteria.type == 'Point':
-            polydata = np.array(criteria.coords)
-        else:
-            polydata = np.vstack([np.array(p.coords) for p in criteria.geoms])
-
-        if polydata.shape[0] < 3:
-            continue
-
-        try:
-            concave_hull = alphashape_optm(polydata, 1)
-        except QhullError:
-            continue
-
-        if concave_hull.is_empty:
-            continue
-        else:
-            boundary = np.array(concave_hull.exterior.xy).T
-        aux = trace_fitpoly(boundary, Z, Ybin, *args)
-        if aux.is_empty:
-            continue
-        splits.append(aux)
-
-    if len(splits) > 0:
-        return unary_union(splits)
-    else:
-        return geometry.Polygon()
-
-
-def trace_fitpoly(polydata: np.ndarray, Z: np.ndarray, Ybin: np.ndarray, PI):
-    if Ybin.dtype != bool:
-        raise TypeError("Ybin must be an array of bools.")
-    if polydata.shape[0] < 3:
-        return geometry.Polygon()
-
-    triangles = triangulate_within(geometry.Polygon(polydata))
-    if ~Ybin.all():
-        z_points = geometry.MultiPoint(Z)
-        good_points = geometry.MultiPoint(Z[Ybin])
-        if len(triangles) == 0:
-            return geometry.Polygon()
-
-        keep = []
-        for tri in triangles:
-            n_elements = count_points(inner_intersection(tri, z_points))
-            n_good_elements = count_points(inner_intersection(tri, good_points))
-            # n_elements = count_points(tri.intersection(z_points))
-            # n_good_elements = count_points(tri.intersection(good_points))
-
-            if n_elements > 0:
-                if (n_good_elements / n_elements) < PI:
-                    continue
-                else:
-                    keep.append(tri)
-        return unary_union(keep)
-    else:
-        return unary_union(triangles)
-
-
-def triangulate_within(polygon):
-    """
-    Produces a triangulation and removes triangles outside the (non-convex) polygon.
-
-    :param polygon: shapely Polygon
-    :return: list of triangles
-    """
-    return [triangle for triangle in triangulate(polygon) if triangle.within(polygon)]
-
-
-def remove_tiny_areas(footprint: FootprintOutput, threshold: float, Z: np.ndarray, Ybin: np.ndarray) -> FootprintOutput:
-    """
-    Eliminates tiny parts of a MultiPolygon (or Polygon).
-
-    :param FootprintOutput footprint: footprint struct object
-    :param float threshold: small area reference value
-    :param np.ndarray Z: IS coordinates
-    :param np.ndarray Ybin: binarized response variable
-    """
-    poly = footprint.polygon
-    z_points = geometry.MultiPoint(Z)
-    z_good = geometry.MultiPoint(Z[Ybin, :])
-
-    if poly.area < threshold:
-        return _empty_footprint()
-    elif isinstance(poly, geometry.Polygon):
-        return footprint
-    elif isinstance(poly, geometry.MultiPolygon):
-        poly_list = [p for p in poly if p.area > threshold]
-        if len(poly_list) == 0:
-            return _empty_footprint()
-        elif len(poly_list) == 1:
-            polygon = poly_list[0]
-        else:
-            polygon = geometry.MultiPolygon(poly_list)
-        area = polygon.area
-        elements = count_points(polygon.intersection(z_points))
-        good_elements = count_points(polygon.intersection(z_good))
-        density = elements / area
-        purity = good_elements / elements
-        return FootprintOutput(polygon, area, elements, good_elements, density, purity)
-    else:
-        raise TypeError("Accepts only Polygon or MultiPolygon as input.")
-
-
-def dbscan(x: np.ndarray, k, eps):
-    m = x.shape[0]
-    x = np.hstack((np.arange(0, m).reshape((-1, 1)), x))
-    m, n = x.shape
-    type_ = np.zeros(m)
-    no = 1
-    touched = np.zeros(m)
-    class_ = np.zeros(m)
-
-    for i in range(m):
-        if touched[i] == 0:
-            ob = x[np.newaxis, i, :]
-            D = dist(ob[:, 1:n], x[:, 1:n])
-            ind = np.argwhere(D <= eps)[:, 0]
-
-            if 1 < len(ind) < k + 1:
-                type_[i] = class_[i] = 0
-            if len(ind) == 1:
-                type_[i] = class_[i] = -1
-                touched[i] = 1
-
-            if len(ind) > k + 1:
-                type_[i] = 1
-                class_[ind] = np.ones(len(ind)) * np.max(no)
-
-                while ind.size != 0:
-                    ob = x[np.newaxis, ind[0], :]
-                    touched[ind[0]] = 1
-                    ind = ind[1:]
-                    D = dist(ob[:, 1:n], x[:, 1:n])
-                    i1 = np.argwhere(D <= eps)
-
-                    if len(i1) > 1:
-                        class_[i1] = no
-                        if len(i1) >= k + 1:
-                            type_[ob[0, 0].astype(int)] = 1
-                        else:
-                            type_[ob[0, 0].astype(int)] = 0
-
-                        for j in range(len(i1)):
-                            if touched[i1[j]] == 0:
-                                touched[i1[j]] = 1
-                                ind = np.hstack((ind, i1[j]))
-                                class_[i1[j]] = no
-                no += 1
-
-    i1 = np.argwhere(class_ == 0)
-    class_[i1] = -1
-    type_[i1] = -1
-
-    return class_.astype(int), type_.astype(int)
-
-
-def dist(x0: np.ndarray, x: np.ndarray):
-    m, n = x.shape
-    D = np.sqrt(np.sum(((np.ones((m, 1)).dot(x0) - x) ** 2).T, axis=0))
-
-    if n == 1:
-        D = np.abs(np.ones((m, 1)).dot(x0) - x).T
-
-    return D
+import logging
+import time
+import warnings
+from dataclasses import dataclass
+from itertools import repeat
+from math import ceil
+from multiprocessing import Pool, cpu_count
+from typing import List, Union
+
+import alphashape
+import numpy as np
+import pandas as pd
+from scipy.spatial import Delaunay
+from scipy.spatial.qhull import QhullError
+from scipy.special import gamma
+from shapely import geometry
+from shapely.ops import polygonize, triangulate, unary_union
+from sklearn.cluster import DBSCAN
+
+
+_required_opts = ['PI']
+_logger = logging.getLogger(__name__)
+
+
+# TODO: remove temporary workaround in future
+class AlphashapeFilter(logging.Filter):
+    def filter(self, record: logging.LogRecord) -> bool:
+        return "Likely caused by all points lying in an N-1 space" not in record.getMessage()
+
+
+logging.getLogger().addFilter(AlphashapeFilter())
+
+
+@dataclass
+class FootprintOutput:
+    polygon: geometry.MultiPolygon
+    area: float
+    elements: int
+    good_elements: int
+    density: float
+    purity: float
+
+
+def _empty_footprint() -> FootprintOutput:
+    return FootprintOutput(geometry.MultiPolygon(), 0, 0, 0, 0, 0)
+
+
+def _copy_footprint(obj: FootprintOutput) -> FootprintOutput:
+    return FootprintOutput(**obj.__dict__)
+
+
+@dataclass
+class TraceOutput:
+    space: FootprintOutput
+    good: List[FootprintOutput]
+    best: List[FootprintOutput]
+    hard: FootprintOutput
+    summary: pd.DataFrame
+
+
+class TraceException(Exception):
+    def __init__(self):
+        super().__init__("There are not enough instances to calculate a footprint. "
+                         "The subset of instances used is too small.")
+
+
+def alpha_shape(points: np.ndarray, alpha=1.0):
+    """
+    Compute the alpha shape (concave hull) of a set of points.
+
+    :param points: array of points (x,y)
+    :param float alpha: alpha value to influence the gooeyness of the border. Smaller numbers don't fall inward as much
+        as larger numbers. Too large, and you lose everything!
+    """
+    if len(points) < 3:
+        # When you have a triangle, there is no sense
+        # in computing an alpha shape.
+        return geometry.MultiPoint(list(points)).convex_hull, points
+    elif len(points) == 3:
+        return geometry.Polygon(points), points
+
+    # coords = np.array([point.coords[0] for point in points])
+    tri = Delaunay(points)
+    triangles = points[tri.simplices]
+    a = ((triangles[:, 0, 0] - triangles[:, 1, 0]) ** 2 + (triangles[:, 0, 1] - triangles[:, 1, 1]) ** 2) ** 0.5
+    b = ((triangles[:, 1, 0] - triangles[:, 2, 0]) ** 2 + (triangles[:, 1, 1] - triangles[:, 2, 1]) ** 2) ** 0.5
+    c = ((triangles[:, 2, 0] - triangles[:, 0, 0]) ** 2 + (triangles[:, 2, 1] - triangles[:, 0, 1]) ** 2) ** 0.5
+    s = (a + b + c) / 2.0
+    areas = (s * (s - a) * (s - b) * (s - c)) ** 0.5
+    circums = a * b * c / (4.0 * areas)
+    filtered = triangles[circums < (1.0 / alpha)]
+    edge1 = filtered[:, (0, 1)]
+    edge2 = filtered[:, (1, 2)]
+    edge3 = filtered[:, (2, 0)]
+    edge_points = np.unique(np.concatenate((edge1, edge2, edge3)), axis=0).tolist()
+    m = geometry.MultiLineString(edge_points)
+    triangles = list(polygonize(m))
+    return unary_union(triangles), edge_points
+
+
+def alphashape_optm(points: np.ndarray, alpha_ini):
+    # TODO: remove temporary workaround in future
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        points = list(map(tuple, points))
+        hull = alphashape.alphashape(points, alpha_ini)
+        if not isinstance(hull, geometry.Polygon):
+            alpha = 0.9 * alphashape.optimizealpha(points)
+            hull = alphashape.alphashape(points, alpha)
+        return hull
+
+
+def count_points(pts: Union[geometry.Point, geometry.MultiPoint]) -> int:
+    if pts.is_empty:
+        return 0
+    elif pts.type == 'Point':
+        return 1
+    elif pts.type == 'MultiPoint':
+        return len(pts.geoms)
+    else:
+        raise TypeError
+
+
+def inner_intersection(poly: geometry.Polygon, pts: geometry.MultiPoint) -> Union[geometry.Point, geometry.MultiPoint]:
+    intersec = poly.intersection(pts)
+    intersec_bound = poly.boundary.intersection(intersec)
+    return intersec.difference(intersec_bound)
+
+
+def copy_polygon(poly: Union[geometry.Polygon, geometry.MultiPolygon]):
+    return poly.__class__(poly)
+
+
+def estimate_epsilon(x, k):
+    m, n = np.shape(x)
+    eps = ((np.prod(x.max(axis=0) - x.min(axis=0)) * k * gamma(.5 * n + 1)) / (m * np.sqrt(np.pi ** n))) ** (1 / n)
+    return eps
+
+
+def make_summary(space: FootprintOutput, good: List[FootprintOutput], best: List[FootprintOutput], algolabels: List):
+    assert len(good) == len(best)
+    cols = ['Area_Good_Normalized', 'Density_Good_Normalized', 'Purity_Good',
+            'Area_Best_Normalized', 'Density_Best_Normalized', 'Purity_Best']
+    rows = []
+    for i in range(len(good)):
+        rows.append([good[i].area / space.area,
+                     good[i].density / space.density,
+                     good[i].purity,
+                     best[i].area / space.area,
+                     best[i].density / space.density,
+                     best[i].purity]
+                    )
+    summary = pd.DataFrame(rows, index=pd.Index(algolabels, name='Row'), columns=cols)
+    return summary
+
+
+def trace(Z: np.ndarray, Ybin: np.ndarray, P: np.ndarray, beta: np.ndarray, algolabels: list, parallel=True, **kwargs):
+    _logger.info("TRACE is calculating the space area and density.")
+    ninst = Z.shape[0]
+    nalgos = Ybin.shape[1]
+    space = trace_build(Z, np.ones(ninst, dtype=bool), kwargs['PI'])
+    _logger.debug(f"Space area: {space.area}")
+    _logger.debug(f"Space density: {space.density}")
+
+    _logger.info("TRACE is calculating the algorithm footprints.")
+    if parallel:
+        _logger.warning("Some log messages are temporarily disabled in parallel mode. This functionality will be added "
+                        "in future versions")
+        with Pool(processes=cpu_count()) as pool:
+            _logger.info(f"Calculating footprints...")
+            good = pool.starmap_async(trace_build_wrapper,
+                                      zip(repeat(Z), (Ybin[:, i] for i in range(nalgos)), repeat(kwargs['PI'])))
+            best = pool.starmap_async(trace_build_wrapper,
+                                      zip(repeat(Z), (P == i for i in range(nalgos)), repeat(kwargs['PI'])))
+            good = good.get()
+            best = best.get()
+    else:
+        good = []
+        best = []
+        for i in range(nalgos):
+            start = time.time()
+            _logger.info(f"Good performance footprint for {repr(algolabels[i])}")
+            try:
+                good.append(trace_build(Z, Ybin[:, i], kwargs['PI']))
+            except TraceException as e:
+                good.append(_empty_footprint())
+                _logger.warning(str(e))
+
+            _logger.info(f"Best performance footprint for {repr(algolabels[i])}")
+            try:
+                best.append(trace_build(Z, P == i, kwargs['PI']))
+            except TraceException as e:
+                good.append(_empty_footprint())
+                _logger.warning(str(e))
+
+            end = time.time()
+            _logger.debug(f"Algorithm {repr(algolabels[i])} completed. Elapsed time: {(end - start):.2f} s")
+
+    _logger.info("TRACE is detecting and removing contradictory sections of the footprints.")
+    for i in range(nalgos - 1):
+        _logger.debug(f"Base algorithm {repr(algolabels[i])}")
+        for j in range(i + 1, nalgos):
+            _logger.debug(f"TRACE is comparing {repr(algolabels[i])} with {repr(algolabels[j])}")
+            best[i], best[j] = trace_contra(best[i], best[j], Z, P == i, P == j, kwargs['PI'])
+            _logger.debug(f"Test algorithm {repr(algolabels[j])} completed.")
+        _logger.debug(f"Base algorithm {repr(algolabels[i])} completed.")
+
+    _logger.info("TRACE is calculating the beta-footprint.")
+    hard = trace_build_wrapper(Z, ~beta, kwargs['PI'])
+
+    _logger.info("TRACE is preparing the summary table.")
+    summary = make_summary(space, good, best, algolabels)
+    _logger.info("TRACE has completed.")
+    return TraceOutput(space, good, best, hard, summary)
+
+
+def trace_build_wrapper(*args):
+    try:
+        return trace_build(*args)
+    except TraceException:
+        return _empty_footprint()
+
+
+def trace_build(Z, Ybin, PI) -> FootprintOutput:
+    Ig = np.unique(Z[Ybin, :], axis=0)
+    if Ig.shape[0] < 3:
+        raise TraceException
+
+    nn = max(min(ceil(sum(Ybin) / 20), 50), 3)
+    eps = estimate_epsilon(Ig, nn)
+    clustering = DBSCAN(eps=eps, min_samples=nn).fit(Ig)
+
+    polygon = geometry.Polygon()
+    for i in range(np.max(clustering.labels_) + 1):
+        polydata = Ig[clustering.labels_ == i, :]
+        if polydata.shape[0] < 3:
+            continue
+
+        try:
+            concave_hull = alphashape_optm(polydata, 2)
+        except QhullError:
+            continue
+
+        if concave_hull.is_empty:
+            raise TraceException
+        else:
+            boundary = np.array(concave_hull.exterior.xy).T
+
+        aux = trace_fitpoly(boundary, Z, Ybin, PI)
+        if not aux.is_empty:
+            polygon = polygon.union(aux)
+
+    if not polygon.is_empty:
+        area = polygon.area
+        elements = count_points(polygon.intersection(geometry.MultiPoint(Z)))
+        good_elements = count_points(polygon.intersection(geometry.MultiPoint(Z[Ybin, :])))
+        density = elements / area
+        purity = good_elements / elements
+        return FootprintOutput(polygon, area, elements, good_elements, density, purity)
+    else:
+        raise TraceException
+
+
+def trace_contra(base: FootprintOutput, test: FootprintOutput, Z: np.ndarray,
+                 Ybase: np.ndarray, Ytest: np.ndarray, *args):
+    if base.polygon.is_empty or test.polygon.is_empty:
+        return base, test
+
+    def degenerate(p):
+        if not (isinstance(p, geometry.Polygon) or isinstance(p, geometry.MultiPolygon)):
+            return True
+        else:
+            return False
+
+    base = _copy_footprint(base)
+    base.polygon = copy_polygon(base.polygon)
+    test = _copy_footprint(test)
+    test.polygon = copy_polygon(test.polygon)
+
+    z_points = geometry.MultiPoint(Z)
+    z_base = geometry.MultiPoint(Z[Ybase, :])
+    z_test = geometry.MultiPoint(Z[Ytest, :])
+    contradiction = base.polygon.intersection(test.polygon)
+
+    maxtries = 3
+    numtries = 1
+
+    while (not contradiction.is_empty) and (numtries <= maxtries):
+        n_elements = count_points(contradiction.intersection(z_points))
+        if n_elements == 0:
+            break
+        n_good_elements_base = count_points(contradiction.intersection(z_base))
+        n_good_elements_test = count_points(contradiction.intersection(z_test))
+        purity_base = n_good_elements_base / n_elements
+        purity_test = n_good_elements_test / n_elements
+
+        if purity_base > purity_test:
+            test.polygon = test.polygon.difference(contradiction)
+            if numtries < maxtries:
+                test.polygon = trace_tight(test.polygon, Z, Ytest, *args)
+        elif purity_test > purity_base:
+            base.polygon = base.polygon.difference(contradiction)
+            if numtries < maxtries:
+                base.polygon = trace_tight(base.polygon, Z, Ybase, *args)
+        else:
+            break
+        if base.polygon.is_empty or test.polygon.is_empty:
+            break
+        else:
+            contradiction = base.polygon.intersection(test.polygon)
+            if degenerate(contradiction):
+                break
+        numtries += 1
+
+    if base.polygon.is_empty:
+        base = _empty_footprint()
+    else:
+        base.area = base.polygon.area
+        base.elements = count_points(base.polygon.intersection(z_points))
+        base.good_elements = count_points(base.polygon.intersection(z_base))
+        base.density = base.elements / base.area
+        base.purity = base.good_elements / base.elements
+    if test.polygon.is_empty:
+        test = _empty_footprint()
+    else:
+        test.area = test.polygon.area
+        test.elements = count_points(test.polygon.intersection(z_points))
+        test.good_elements = count_points(test.polygon.intersection(z_base))
+        test.density = test.elements / test.area
+        test.purity = test.good_elements / test.elements
+
+    return base, test
+
+
+def trace_tight(polygon: Union[geometry.Polygon, geometry.MultiPolygon],
+                Z: np.ndarray, Ybin: np.ndarray, *args):
+    if isinstance(polygon, geometry.Polygon):
+        nregions = 1
+        polygon = geometry.MultiPolygon([polygon])
+    else:
+        nregions = len(polygon.geoms)
+
+    z_points = geometry.MultiPoint(Z)
+    splits = []
+
+    for i in range(nregions):
+        criteria = inner_intersection(polygon.geoms[i], z_points)
+        if criteria.type == 'Point':
+            polydata = np.array(criteria.coords)
+        else:
+            polydata = np.vstack([np.array(p.coords) for p in criteria.geoms])
+
+        if polydata.shape[0] < 3:
+            continue
+
+        try:
+            concave_hull = alphashape_optm(polydata, 1)
+        except QhullError:
+            continue
+
+        if concave_hull.is_empty:
+            continue
+        else:
+            boundary = np.array(concave_hull.exterior.xy).T
+        aux = trace_fitpoly(boundary, Z, Ybin, *args)
+        if aux.is_empty:
+            continue
+        splits.append(aux)
+
+    if len(splits) > 0:
+        return unary_union(splits)
+    else:
+        return geometry.Polygon()
+
+
+def trace_fitpoly(polydata: np.ndarray, Z: np.ndarray, Ybin: np.ndarray, PI):
+    if Ybin.dtype != bool:
+        raise TypeError("Ybin must be an array of bools.")
+    if polydata.shape[0] < 3:
+        return geometry.Polygon()
+
+    triangles = triangulate_within(geometry.Polygon(polydata))
+    if ~Ybin.all():
+        z_points = geometry.MultiPoint(Z)
+        good_points = geometry.MultiPoint(Z[Ybin])
+        if len(triangles) == 0:
+            return geometry.Polygon()
+
+        keep = []
+        for tri in triangles:
+            n_elements = count_points(inner_intersection(tri, z_points))
+            n_good_elements = count_points(inner_intersection(tri, good_points))
+            # n_elements = count_points(tri.intersection(z_points))
+            # n_good_elements = count_points(tri.intersection(good_points))
+
+            if n_elements > 0:
+                if (n_good_elements / n_elements) < PI:
+                    continue
+                else:
+                    keep.append(tri)
+        return unary_union(keep)
+    else:
+        return unary_union(triangles)
+
+
+def triangulate_within(polygon):
+    """
+    Produces a triangulation and removes triangles outside the (non-convex) polygon.
+
+    :param polygon: shapely Polygon
+    :return: list of triangles
+    """
+    return [triangle for triangle in triangulate(polygon) if triangle.within(polygon)]
+
+
+def remove_tiny_areas(footprint: FootprintOutput, threshold: float, Z: np.ndarray, Ybin: np.ndarray) -> FootprintOutput:
+    """
+    Eliminates tiny parts of a MultiPolygon (or Polygon).
+
+    :param FootprintOutput footprint: footprint struct object
+    :param float threshold: small area reference value
+    :param np.ndarray Z: IS coordinates
+    :param np.ndarray Ybin: binarized response variable
+    """
+    poly = footprint.polygon
+    z_points = geometry.MultiPoint(Z)
+    z_good = geometry.MultiPoint(Z[Ybin, :])
+
+    if poly.area < threshold:
+        return _empty_footprint()
+    elif isinstance(poly, geometry.Polygon):
+        return footprint
+    elif isinstance(poly, geometry.MultiPolygon):
+        poly_list = [p for p in poly if p.area > threshold]
+        if len(poly_list) == 0:
+            return _empty_footprint()
+        elif len(poly_list) == 1:
+            polygon = poly_list[0]
+        else:
+            polygon = geometry.MultiPolygon(poly_list)
+        area = polygon.area
+        elements = count_points(polygon.intersection(z_points))
+        good_elements = count_points(polygon.intersection(z_good))
+        density = elements / area
+        purity = good_elements / elements
+        return FootprintOutput(polygon, area, elements, good_elements, density, purity)
+    else:
+        raise TypeError("Accepts only Polygon or MultiPolygon as input.")
+
+
+def dbscan(x: np.ndarray, k, eps):
+    m = x.shape[0]
+    x = np.hstack((np.arange(0, m).reshape((-1, 1)), x))
+    m, n = x.shape
+    type_ = np.zeros(m)
+    no = 1
+    touched = np.zeros(m)
+    class_ = np.zeros(m)
+
+    for i in range(m):
+        if touched[i] == 0:
+            ob = x[np.newaxis, i, :]
+            D = dist(ob[:, 1:n], x[:, 1:n])
+            ind = np.argwhere(D <= eps)[:, 0]
+
+            if 1 < len(ind) < k + 1:
+                type_[i] = class_[i] = 0
+            if len(ind) == 1:
+                type_[i] = class_[i] = -1
+                touched[i] = 1
+
+            if len(ind) > k + 1:
+                type_[i] = 1
+                class_[ind] = np.ones(len(ind)) * np.max(no)
+
+                while ind.size != 0:
+                    ob = x[np.newaxis, ind[0], :]
+                    touched[ind[0]] = 1
+                    ind = ind[1:]
+                    D = dist(ob[:, 1:n], x[:, 1:n])
+                    i1 = np.argwhere(D <= eps)
+
+                    if len(i1) > 1:
+                        class_[i1] = no
+                        if len(i1) >= k + 1:
+                            type_[ob[0, 0].astype(int)] = 1
+                        else:
+                            type_[ob[0, 0].astype(int)] = 0
+
+                        for j in range(len(i1)):
+                            if touched[i1[j]] == 0:
+                                touched[i1[j]] = 1
+                                ind = np.hstack((ind, i1[j]))
+                                class_[i1[j]] = no
+                no += 1
+
+    i1 = np.argwhere(class_ == 0)
+    class_[i1] = -1
+    type_[i1] = -1
+
+    return class_.astype(int), type_.astype(int)
+
+
+def dist(x0: np.ndarray, x: np.ndarray):
+    m, n = x.shape
+    D = np.sqrt(np.sum(((np.ones((m, 1)).dot(x0) - x) ** 2).T, axis=0))
+
+    if n == 1:
+        D = np.abs(np.ones((m, 1)).dot(x0) - x).T
+
+    return D
```

### Comparing `pyispace-0.3.4/pyispace/train.py` & `pyispace-0.3.5/pyispace/train.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import logging
-from dataclasses import dataclass, field
-from itertools import compress
-
-import numpy as np
-import pandas as pd
-from scipy.stats import mode
-
-from . import preprocessing
-from .pilot import PilotOutput, pilot, adjust_rotation
-from .trace import TraceOutput, trace
-
-
-_feature_prefix = 'feature_'
-_algo_prefix = 'algo_'
-
-
-@dataclass
-class Data:
-    instlabels: pd.Index = field(init=False)
-    X: np.ndarray = field(init=False)
-    Y: np.ndarray = field(init=False)
-    Yraw: np.ndarray = field(init=False, default=np.array([]))
-    Xraw: np.ndarray = field(init=False, default=np.array([]))
-    Ybin: np.ndarray = field(init=False)
-    beta: np.ndarray = field(init=False)
-    numGoodAlgos: list = field(init=False, default_factory=list)
-    bestPerformace: list = field(init=False, default_factory=list)
-    P: np.ndarray = field(init=False)
-    featlabels: list = field(init=False, default_factory=list)
-    algolabels: list = field(init=False, default_factory=list)
-
-
-@dataclass
-class Model:
-    data: Data = field(init=False)
-    pilot: PilotOutput = field(init=False)
-    trace: TraceOutput = field(init=False)
-
-
-def train_is(metadata: pd.DataFrame, opts: dict, rotation_adjust: bool = False) -> Model:
-    """
-    Train Instance Space model.
-
-    :param pandas.DataFrame metadata: dataframe where each row corresponds to an instance
-    :param dict opts: (nested) dictionary with options
-    :param bool rotation_adjust: attempts to adjust the IS angle (bad instances at 135 degrees) - default False
-    :return: model with results for all the steps according to the options passed
-    :rtype: Model
-    """
-    logger = logging.getLogger(__name__)
-    eps = np.spacing(1)
-
-    data = Data()
-    data.instlabels = metadata.index.copy()
-    Xraw = metadata.filter(regex=f'^{_feature_prefix}')
-    Yraw = metadata.filter(regex=f'^{_algo_prefix}')
-    data.Xraw = Xraw.values
-    data.Yraw = Yraw.values
-    data.X = Xraw.values
-    data.Y = Yraw.values
-    data.featlabels = [x.replace(_feature_prefix, '') for x in Xraw.columns.tolist()]
-    data.algolabels = [y.replace(_algo_prefix, '') for y in Yraw.columns.tolist()]
-
-    logger.info("Calculating the binary measure of performance")
-    msg = "An algorithm is good if its performace is "
-    epsilon = opts['perf']['epsilon']
-    if opts['perf']['MaxPerf']:
-        Yaux = Yraw.fillna(-np.inf).values
-        rankPerf = np.sort(Yaux, axis=1)[:, ::-1]
-        rankAlgo = np.argsort(Yaux, axis=1)[:, ::-1]
-        data.bestPerformace = rankPerf[:, [0]]
-        data.P = rankAlgo[:, 0]
-        if opts['perf']['AbsPerf']:
-            data.Ybin = Yaux >= epsilon
-            msg = msg + f"higher than {epsilon}"
-        else:
-            data.bestPerformace[data.bestPerformace == 0] = eps
-            data.Y[data.Y == 0] = eps
-            data.Y = 1 - data.Y / data.bestPerformace
-            data.Ybin = np.greater_equal(Yaux, (1 - epsilon) * data.bestPerformace)
-            msg = msg + f"within {np.round(100 * epsilon)}% of the best."
-    else:
-        Yaux = Yraw.fillna(np.inf).values
-        rankPerf = np.sort(Yaux, axis=1)
-        rankAlgo = np.argsort(Yaux, axis=1)
-        data.bestPerformace = rankPerf[:, [0]]
-        data.P = rankAlgo[:, 0]
-        if opts['perf']['AbsPerf']:
-            data.Ybin = Yaux <= epsilon
-            msg = msg + f"less than {epsilon}"
-        else:
-            data.bestPerformace[data.bestPerformace == 0] = eps
-            data.Y[data.Y == 0] = eps
-            data.Y = data.Y / data.bestPerformace - 1
-            data.Ybin = np.less_equal(Yaux, (1 + epsilon) * data.bestPerformace)
-            msg = msg + f"within {np.round(100 * epsilon)}% of the best."
-    logger.info(msg)
-
-    nalgos = data.Y.shape[1]
-    idx = np.all(~data.Ybin, axis=0)
-    if np.any(idx):
-        logger.warning("There are algorithms with no 'good' instances. They are being removed to increase speed.")
-        data.Yraw = data.Yraw[:, ~idx]
-        data.Y = data.Y[:, ~idx]
-        data.Ybin = data.Ybin[:, ~idx]
-        data.algolabels = list(compress(data.algolabels, ~idx))
-        nalgos = data.Y.shape[1]
-        if nalgos == 0:
-            logger.error("There are no 'good' algorithms. Please verify the binary performance measure. STOPPING!")
-            raise RuntimeError("There are no 'good' algorithms.")
-
-    # Testing for ties
-    bestAlgos = np.equal(data.Y, data.bestPerformace)
-    multipleBestAlgos = np.sum(bestAlgos, axis=1) > 1
-    aidx = np.arange(nalgos)
-    for i in range(data.Y.shape[0]):
-        if multipleBestAlgos[i]:
-            data.P[i] = np.random.choice(aidx[bestAlgos[i]])
-    logger.info(f"For {np.round(100 * np.mean(multipleBestAlgos))}% of the instances there is more than one best "
-                f"algorithm. Random selection is used to break ties.")
-
-    data.numGoodAlgos = np.sum(data.Ybin, axis=1)
-    data.beta = data.numGoodAlgos > opts['general']['betaThreshold'] * nalgos
-
-    if opts['auto']['preproc']:
-        logger.info("Auto pre-processing.")
-        if opts['bound']['flag']:
-            logger.info("Removing extreme outliers from the feature values.")
-            data.X = preprocessing.bound_outliers(data.X)
-        if opts['norm']['flag']:
-            logger.info("Auto-normalizing the data using Box-Cox and Z transformations.")
-            # data.X, data.Y = preprocessing.auto_normalize(data.X, data.Y)
-            data.X = preprocessing.auto_normalize(data.X)
-            data.Y = preprocessing.auto_normalize(data.Y)
-
-    model = Model()
-    model.data = data
-
-    logger.info("Calling PILOT to find the optimal projection.")
-    model.pilot = pilot(data.X, data.Y, featlabels=data.featlabels, **opts['pilot'])
-
-    if rotation_adjust:
-        bad_instances = mode(model.data.Ybin * 1, axis=1, keepdims=True)[0] == 0
-        if bad_instances.any():
-            logger.info("Adjusting the IS rotation.")
-            model.pilot.Z, R_theta = adjust_rotation(model.pilot.Z, bad_instances[:, 0])
-            model.pilot.A = R_theta.dot(model.pilot.A)
-            logger.info(f"The space was rotated by {np.round(np.degrees(np.arccos(R_theta[0, 0])), 1)} degrees.")
-        else:
-            logger.info("It is not possible to adjust the IS rotation because there are no bad instances.")
-
-    logger.info("Calling TRACE to perform the footprint analysis.")
-    model.trace = trace(model.pilot.Z, model.data.Ybin, model.data.P,
-                        model.data.beta, model.data.algolabels, **opts['trace'])
-
-    return model
+import logging
+from dataclasses import dataclass, field
+from itertools import compress
+
+import numpy as np
+import pandas as pd
+from scipy.stats import mode
+
+from . import preprocessing
+from .pilot import PilotOutput, pilot, adjust_rotation
+from .trace import TraceOutput, trace
+
+
+_feature_prefix = 'feature_'
+_algo_prefix = 'algo_'
+
+
+@dataclass
+class Data:
+    instlabels: pd.Index = field(init=False)
+    X: np.ndarray = field(init=False)
+    Y: np.ndarray = field(init=False)
+    Yraw: np.ndarray = field(init=False, default=np.array([]))
+    Xraw: np.ndarray = field(init=False, default=np.array([]))
+    Ybin: np.ndarray = field(init=False)
+    beta: np.ndarray = field(init=False)
+    numGoodAlgos: list = field(init=False, default_factory=list)
+    bestPerformace: list = field(init=False, default_factory=list)
+    P: np.ndarray = field(init=False)
+    featlabels: list = field(init=False, default_factory=list)
+    algolabels: list = field(init=False, default_factory=list)
+
+
+@dataclass
+class Model:
+    data: Data = field(init=False)
+    pilot: PilotOutput = field(init=False)
+    trace: TraceOutput = field(init=False)
+
+
+def train_is(metadata: pd.DataFrame, opts: dict, rotation_adjust: bool = False) -> Model:
+    """
+    Train Instance Space model.
+
+    :param pandas.DataFrame metadata: dataframe where each row corresponds to an instance
+    :param dict opts: (nested) dictionary with options
+    :param bool rotation_adjust: attempts to adjust the IS angle (bad instances at 135 degrees) - default False
+    :return: model with results for all the steps according to the options passed
+    :rtype: Model
+    """
+    logger = logging.getLogger(__name__)
+    eps = np.spacing(1)
+
+    data = Data()
+    data.instlabels = metadata.index.copy()
+    Xraw = metadata.filter(regex=f'^{_feature_prefix}')
+    Yraw = metadata.filter(regex=f'^{_algo_prefix}')
+    data.Xraw = Xraw.values
+    data.Yraw = Yraw.values
+    data.X = Xraw.values
+    data.Y = Yraw.values
+    data.featlabels = [x.replace(_feature_prefix, '') for x in Xraw.columns.tolist()]
+    data.algolabels = [y.replace(_algo_prefix, '') for y in Yraw.columns.tolist()]
+
+    logger.info("Calculating the binary measure of performance")
+    msg = "An algorithm is good if its performace is "
+    epsilon = opts['perf']['epsilon']
+    if opts['perf']['MaxPerf']:
+        Yaux = Yraw.fillna(-np.inf).values
+        rankPerf = np.sort(Yaux, axis=1)[:, ::-1]
+        rankAlgo = np.argsort(Yaux, axis=1)[:, ::-1]
+        data.bestPerformace = rankPerf[:, [0]]
+        data.P = rankAlgo[:, 0]
+        if opts['perf']['AbsPerf']:
+            data.Ybin = Yaux >= epsilon
+            msg = msg + f"higher than {epsilon}"
+        else:
+            data.bestPerformace[data.bestPerformace == 0] = eps
+            data.Y[data.Y == 0] = eps
+            data.Y = 1 - data.Y / data.bestPerformace
+            data.Ybin = np.greater_equal(Yaux, (1 - epsilon) * data.bestPerformace)
+            msg = msg + f"within {np.round(100 * epsilon)}% of the best."
+    else:
+        Yaux = Yraw.fillna(np.inf).values
+        rankPerf = np.sort(Yaux, axis=1)
+        rankAlgo = np.argsort(Yaux, axis=1)
+        data.bestPerformace = rankPerf[:, [0]]
+        data.P = rankAlgo[:, 0]
+        if opts['perf']['AbsPerf']:
+            data.Ybin = Yaux <= epsilon
+            msg = msg + f"less than {epsilon}"
+        else:
+            data.bestPerformace[data.bestPerformace == 0] = eps
+            data.Y[data.Y == 0] = eps
+            data.Y = data.Y / data.bestPerformace - 1
+            data.Ybin = np.less_equal(Yaux, (1 + epsilon) * data.bestPerformace)
+            msg = msg + f"within {np.round(100 * epsilon)}% of the best."
+    logger.info(msg)
+
+    nalgos = data.Y.shape[1]
+    idx = np.all(~data.Ybin, axis=0)
+    if np.any(idx):
+        logger.warning("There are algorithms with no 'good' instances. They are being removed to increase speed.")
+        data.Yraw = data.Yraw[:, ~idx]
+        data.Y = data.Y[:, ~idx]
+        data.Ybin = data.Ybin[:, ~idx]
+        data.algolabels = list(compress(data.algolabels, ~idx))
+        nalgos = data.Y.shape[1]
+        if nalgos == 0:
+            logger.error("There are no 'good' algorithms. Please verify the binary performance measure. STOPPING!")
+            raise RuntimeError("There are no 'good' algorithms.")
+
+    # Testing for ties
+    bestAlgos = np.equal(data.Y, data.bestPerformace)
+    multipleBestAlgos = np.sum(bestAlgos, axis=1) > 1
+    aidx = np.arange(nalgos)
+    for i in range(data.Y.shape[0]):
+        if multipleBestAlgos[i]:
+            data.P[i] = np.random.choice(aidx[bestAlgos[i]])
+    logger.info(f"For {np.round(100 * np.mean(multipleBestAlgos))}% of the instances there is more than one best "
+                f"algorithm. Random selection is used to break ties.")
+
+    data.numGoodAlgos = np.sum(data.Ybin, axis=1)
+    data.beta = data.numGoodAlgos > opts['general']['betaThreshold'] * nalgos
+
+    if opts['auto']['preproc']:
+        logger.info("Auto pre-processing.")
+        if opts['bound']['flag']:
+            logger.info("Removing extreme outliers from the feature values.")
+            data.X = preprocessing.bound_outliers(data.X)
+        if opts['norm']['flag']:
+            logger.info("Auto-normalizing the data using Box-Cox and Z transformations.")
+            # data.X, data.Y = preprocessing.auto_normalize(data.X, data.Y)
+            data.X = preprocessing.auto_normalize(data.X)
+            data.Y = preprocessing.auto_normalize(data.Y)
+
+    model = Model()
+    model.data = data
+
+    logger.info("Calling PILOT to find the optimal projection.")
+    model.pilot = pilot(data.X, data.Y, featlabels=data.featlabels, **opts['pilot'])
+
+    if rotation_adjust:
+        bad_instances = mode(model.data.Ybin * 1, axis=1, keepdims=True)[0] == 0
+        if bad_instances.any():
+            logger.info("Adjusting the IS rotation.")
+            model.pilot.Z, R_theta = adjust_rotation(model.pilot.Z, bad_instances[:, 0])
+            model.pilot.A = R_theta.dot(model.pilot.A)
+            logger.info(f"The space was rotated by {np.round(np.degrees(np.arccos(R_theta[0, 0])), 1)} degrees.")
+        else:
+            logger.info("It is not possible to adjust the IS rotation because there are no bad instances.")
+
+    logger.info("Calling TRACE to perform the footprint analysis.")
+    model.trace = trace(model.pilot.Z, model.data.Ybin, model.data.P,
+                        model.data.beta, model.data.algolabels, **opts['trace'])
+
+    return model
```

### Comparing `pyispace-0.3.4/pyispace/utils.py` & `pyispace-0.3.5/pyispace/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import pickle
-from functools import reduce
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-from shapely import geometry
-
-from .trace import FootprintOutput
-from .train import Model
-
-
-z_cols = ['z_1', 'z_2']
-output_idx_name = 'Row'
-
-
-def vstack_with_sep(a: np.ndarray, b: np.ndarray, sep=np.nan):
-    assert a.shape[1] == b.shape[1]
-    sep_arr = np.ones((1, a.shape[1])) * sep
-    return np.vstack((a, sep_arr, b))
-
-
-def join_polygons(poly):
-    if isinstance(poly, geometry.Polygon):
-        return np.array(poly.exterior.coords.xy).T[:-1, :]
-
-    if poly.is_empty:
-        return None
-    poly_gen = (np.array(p.exterior.coords.xy).T[:-1, :] for p in poly.geoms)
-    return reduce(vstack_with_sep, poly_gen)
-
-
-def scriptcsv(container: Model, rootdir: Path):
-    """
-    Writes ISA model data to files.
-
-    :param Model container: the ISA model
-    :param pathlib.Path rootdir: path where the files will be saved
-    """
-    idx = pd.Index(list(range(1, container.pilot.Z.shape[0] + 1)), name=output_idx_name)
-    algolabels = container.data.algolabels
-    nalgos = len(algolabels)
-    for i in range(nalgos):
-        save_footprint(container.trace.good[i], rootdir, algolabels[i], 'good')
-        save_footprint(container.trace.best[i], rootdir, algolabels[i], 'best')
-
-    pd.DataFrame(container.pilot.Z, index=idx, columns=z_cols).to_csv(rootdir / 'coordinates.csv')
-    pd.DataFrame(container.pilot.A, index=pd.Index(z_cols, name=output_idx_name),
-                 columns=container.data.featlabels).to_csv(rootdir / 'projection_matrix.csv')
-
-    pd.DataFrame(container.data.Ybin.astype(int), index=idx,
-                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_bin.csv')
-    pd.DataFrame(container.data.Y, index=idx,
-                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_process.csv')
-    pd.DataFrame(container.data.Yraw, index=idx,
-                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_raw.csv')
-    pd.DataFrame(container.data.X, index=idx,
-                 columns=container.data.featlabels).to_csv(rootdir / 'feature_process.csv')
-    pd.DataFrame(container.data.Xraw, index=idx,
-                 columns=container.data.featlabels).to_csv(rootdir / 'feature_raw.csv')
-
-    pd.DataFrame(container.data.beta.astype(int), index=idx, columns=['IsBetaEasy']).to_csv(rootdir / 'beta_easy.csv')
-    pd.DataFrame(container.data.P + 1, index=idx, columns=['Best_Algorithm']).to_csv(rootdir / 'portfolio.csv')
-    pd.DataFrame(container.data.numGoodAlgos, index=idx, columns=['NumGoodAlgos']).to_csv(rootdir / 'good_algos.csv')
-
-    container.trace.summary.to_csv(rootdir / 'footprint_performance.csv')
-
-    model_file = rootdir / 'model.pkl'
-    with model_file.open('wb') as f:
-        pickle.dump(container, f)
-
-
-def save_footprint(footprint: FootprintOutput, rootdir: Path, name: str, suffix='good'):
-    """
-    Convenient function to save footprint polygons.
-
-    :param trace.FootprintOutput footprint: footprint output object
-    :param pathlib.Path rootdir: path where the files will be saved
-    :param str name: the algorithm name
-    :param str suffix: either 'good', 'best' or 'bad'
-    """
-    footprint_good = join_polygons(footprint.polygon)
-    df_good = pd.DataFrame(footprint_good, columns=z_cols)
-    df_good.index.name = output_idx_name
-    df_good.to_csv(rootdir / f'footprint_{name}_{suffix}.csv')
+import pickle
+from functools import reduce
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+from shapely import geometry
+
+from .trace import FootprintOutput
+from .train import Model
+
+
+z_cols = ['z_1', 'z_2']
+output_idx_name = 'Row'
+
+
+def vstack_with_sep(a: np.ndarray, b: np.ndarray, sep=np.nan):
+    assert a.shape[1] == b.shape[1]
+    sep_arr = np.ones((1, a.shape[1])) * sep
+    return np.vstack((a, sep_arr, b))
+
+
+def join_polygons(poly):
+    if isinstance(poly, geometry.Polygon):
+        return np.array(poly.exterior.coords.xy).T[:-1, :]
+
+    if poly.is_empty:
+        return None
+    poly_gen = (np.array(p.exterior.coords.xy).T[:-1, :] for p in poly.geoms)
+    return reduce(vstack_with_sep, poly_gen)
+
+
+def scriptcsv(container: Model, rootdir: Path):
+    """
+    Writes ISA model data to files.
+
+    :param Model container: the ISA model
+    :param pathlib.Path rootdir: path where the files will be saved
+    """
+    idx = pd.Index(list(range(1, container.pilot.Z.shape[0] + 1)), name=output_idx_name)
+    algolabels = container.data.algolabels
+    nalgos = len(algolabels)
+    for i in range(nalgos):
+        save_footprint(container.trace.good[i], rootdir, algolabels[i], 'good')
+        save_footprint(container.trace.best[i], rootdir, algolabels[i], 'best')
+
+    pd.DataFrame(container.pilot.Z, index=idx, columns=z_cols).to_csv(rootdir / 'coordinates.csv')
+    pd.DataFrame(container.pilot.A, index=pd.Index(z_cols, name=output_idx_name),
+                 columns=container.data.featlabels).to_csv(rootdir / 'projection_matrix.csv')
+
+    pd.DataFrame(container.data.Ybin.astype(int), index=idx,
+                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_bin.csv')
+    pd.DataFrame(container.data.Y, index=idx,
+                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_process.csv')
+    pd.DataFrame(container.data.Yraw, index=idx,
+                 columns=container.data.algolabels).to_csv(rootdir / 'algorithm_raw.csv')
+    pd.DataFrame(container.data.X, index=idx,
+                 columns=container.data.featlabels).to_csv(rootdir / 'feature_process.csv')
+    pd.DataFrame(container.data.Xraw, index=idx,
+                 columns=container.data.featlabels).to_csv(rootdir / 'feature_raw.csv')
+
+    pd.DataFrame(container.data.beta.astype(int), index=idx, columns=['IsBetaEasy']).to_csv(rootdir / 'beta_easy.csv')
+    pd.DataFrame(container.data.P + 1, index=idx, columns=['Best_Algorithm']).to_csv(rootdir / 'portfolio.csv')
+    pd.DataFrame(container.data.numGoodAlgos, index=idx, columns=['NumGoodAlgos']).to_csv(rootdir / 'good_algos.csv')
+
+    container.trace.summary.to_csv(rootdir / 'footprint_performance.csv')
+
+    model_file = rootdir / 'model.pkl'
+    with model_file.open('wb') as f:
+        pickle.dump(container, f)
+
+
+def save_footprint(footprint: FootprintOutput, rootdir: Path, name: str, suffix='good'):
+    """
+    Convenient function to save footprint polygons.
+
+    :param trace.FootprintOutput footprint: footprint output object
+    :param pathlib.Path rootdir: path where the files will be saved
+    :param str name: the algorithm name
+    :param str suffix: either 'good', 'best' or 'bad'
+    """
+    footprint_good = join_polygons(footprint.polygon)
+    df_good = pd.DataFrame(footprint_good, columns=z_cols)
+    df_good.index.name = output_idx_name
+    df_good.to_csv(rootdir / f'footprint_{name}_{suffix}.csv')
```

