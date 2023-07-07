# Comparing `tmp/xbootstrap-0.0.4.tar.gz` & `tmp/xbootstrap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbootstrap-0.0.4.tar", last modified: Wed Aug 24 11:29:26 2022, max compression
+gzip compressed data, was "xbootstrap-0.0.5.tar", last modified: Fri Jul  7 03:37:04 2023, max compression
```

## Comparing `xbootstrap-0.0.4.tar` & `xbootstrap-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/xbootstrap/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/xbootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/xbootstrap/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    15839 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/xbootstrap/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/xbootstrap/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7822 2022-08-24 11:29:21.000000 xbootstrap-0.0.4/xbootstrap/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 11:29:26.471296 xbootstrap-0.0.4/xbootstrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-08-24 11:29:26.000000 xbootstrap-0.0.4/xbootstrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-08-24 11:29:26.000000 xbootstrap-0.0.4/xbootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 11:29:26.000000 xbootstrap-0.0.4/xbootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-24 11:29:26.000000 xbootstrap-0.0.4/xbootstrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-24 11:29:26.000000 xbootstrap-0.0.4/xbootstrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81141 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/xbootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/xbootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/xbootstrap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/xbootstrap/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/xbootstrap/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-07 03:36:51.000000 xbootstrap-0.0.5/xbootstrap/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:37:04.755712 xbootstrap-0.0.5/xbootstrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-07 03:37:04.000000 xbootstrap-0.0.5/xbootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 03:37:04.000000 xbootstrap-0.0.5/xbootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:37:04.000000 xbootstrap-0.0.5/xbootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 03:37:04.000000 xbootstrap-0.0.5/xbootstrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 03:37:04.000000 xbootstrap-0.0.5/xbootstrap.egg-info/top_level.txt
```

### Comparing `xbootstrap-0.0.4/LICENSE` & `xbootstrap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xbootstrap-0.0.4/README.md` & `xbootstrap-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # xbootstrap
 
 [![PyPI](https://img.shields.io/pypi/v/xbootstrap)](https://pypi.org/project/xbootstrap)
-[![tests](https://github.com/dougiesquire/xbootstrap/actions/workflows/tests.yml/badge.svg)](https://github.com/dougiesquire/xbootstrap/actions/workflows/tests.yml)
-[![pre-commit](https://github.com/dougiesquire/xbootstrap/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/dougiesquire/xbootstrap/actions/workflows/pre-commit.yml)
+[![tests](https://github.com/dougiesquire/xbootstrap/actions/workflows/test.yml/badge.svg)](https://github.com/dougiesquire/xbootstrap/actions/workflows/test.yml)
+[![build](https://github.com/dougiesquire/xbootstrap/actions/workflows/build.yml/badge.svg)](https://github.com/dougiesquire/xbootstrap/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/dougiesquire/xbootstrap/branch/main/graph/badge.svg?token=N0XB8OZ2AE)](https://codecov.io/gh/dougiesquire/xbootstrap)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/dougiesquire/xbootstrap/blob/master/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
-`xbootstrap` is a simple package for performing **nested circular block bootstrapping** (random resampling with replacement) of xarray objects. Here, "nested" means that, when multiple dimensions are specified, the first dimension is randomly resampled, then for each randomly sampled element along that dimension the second dimension is randomly resampled, then for each randomly sampled element along that dimension the third dimension is randomly resampled etc. "Block" boostrapping is a simple way to account for autocorrelation in the data being randomly resampled and "circular" block bootstrapping avoids undersampling data values near the beginning and end of the dimension(s) being resampled (see [Wilks, Chapter 5.3](https://www.sciencedirect.com/science/article/pii/B9780128158234000055#s0100)).  
+`xbootstrap` is a simple package for performing **nested<sup>*</sup> circular<sup>&dagger;</sup> block<sup>&Dagger;</sup> bootstrapping<sup>¶</sup>** of xarray objects. 
+
+- <sup>¶</sup> Bootstrapping is random resampling with replacement.
+- <sup>&Dagger;</sup> Block boostrapping is a simple way to account for autocorrelation in the data being randomly resampled.
+- <sup>&dagger;</sup> Circular block bootstrapping avoids undersampling data values near the beginning and end of the dimension(s) being resampled. This is optional in `xbootstrap`.
+- <sup>*</sup> Here, nested bootstrapping means that, when multiple dimensions are specified, the first dimension is randomly resampled, then for each resampled element along that dimension the second dimension is randomly resampled, then for each resampled element along that dimension the third dimension is randomly resampled etc.
 
 ### Installation
 To install this package from PyPI:
 ```
 pip install xbootstrap
 ```
 
@@ -31,33 +36,38 @@
 )
 ds2 = xr.DataArray(
     np.random.random((n_time, n_ensemble)),
     coords={"time": range(n_time), "ensemble": range(n_ensemble)},
 )
 ds3 = xr.DataArray(np.random.random((n_time)), coords={"time": range(n_time)})
 
-# Create 1000 bootstrapped resamples of ds1, ds2 and ds3 using a
-# blocksize of 5 for the time dimension and 1 for the ensemble
+# Create 1000 circularly bootstrapped resamples of ds1, ds2 and ds3
+# using a blocksize of 5 for the time dimension and 1 for the ensemble
 # dimension, and only bootstrapping the time dimension for ds2
 ds1_bs, ds2_bs, ds3_bs = block_bootstrap(
     ds1,
     ds2,
     ds3,
     blocks={"time": 5, "ensemble": 1},
     n_iteration=1000,
     exclude_dims=[[], ["ensemble"], []],
+    circular=True,
 )
 ```
 `block_bootstrap` also operates lazily with dask-backed xarray objects, but this requires `dask` to be installed:
 ```python
 ds1_bs, ds2_bs, ds3_bs = block_bootstrap(
     ds1.chunk(),
     ds2.chunk(),
     ds3.chunk(),
     blocks={"time": 5, "ensemble": 1},
     n_iteration=10,
     exclude_dims=[[], ["ensemble"], []],
+    circular=True,
 )
 ```
 
 ### Contributing
 Contributions are very welcome, particularly in the form of reporting bugs and writing tests. Please open an issue and check out the [contributor guide](CONTRIBUTING.md).
+
+### References
+Wilks, D.S., 2011. *Statistical methods in the atmospheric sciences* (Vol. 100). Academic press. (particularly [Chapter 5.3](https://www.sciencedirect.com/science/article/pii/B9780128158234000055#s0100))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xbootstrap-0.0.4/versioneer.py` & `xbootstrap-0.0.5/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,21 +277,21 @@
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
+import functools
 import json
 import os
 import re
 import subprocess
 import sys
-from typing import Callable, Dict
-import functools
+from typing import Callable
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -341,15 +341,15 @@
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
     parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
+    with open(setup_cfg) as cfg_file:
         parser.read_file(cfg_file)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     # Dict-like interface for non-mandatory entries
     section = parser["versioneer"]
 
     cfg = VersioneerConfig()
@@ -366,16 +366,16 @@
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY: dict[str, str] = {}
+HANDLERS: dict[str, dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
@@ -416,15 +416,15 @@
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
-            print("unable to find command, tried %s" % (commands,))
+            print(f"unable to find command, tried {commands}")
         return None, None
     stdout = process.communicate()[0].strip().decode()
     if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
@@ -1099,15 +1099,15 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
+        with open(versionfile_abs) as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
                 if line.strip().startswith("git_full ="):
                     mo = re.search(r'=\s*"(.*)"', line)
@@ -1295,15 +1295,15 @@
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+            pieces["error"] = "tag '{}' doesn't start with prefix '{}'".format(
                 full_tag,
                 tag_prefix,
             )
             return pieces
         pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
@@ -1346,15 +1346,15 @@
             my_path = os.path.splitext(my_path)[0] + ".py"
         versioneer_file = os.path.relpath(my_path)
     except NameError:
         versioneer_file = "versioneer.py"
     files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
+        with open(".gitattributes") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
                         break
     except OSError:
         pass
@@ -1435,15 +1435,15 @@
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
-    print("set %s to '%s'" % (filename, versions["version"]))
+    print("set {} to '{}'".format(filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
@@ -1740,15 +1740,15 @@
             return ver
         except NotThisMethod:
             pass
 
     try:
         ver = versions_from_file(versionfile_abs)
         if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
+            print(f"got version from file {versionfile_abs} {ver}")
         return ver
     except NotThisMethod:
         pass
 
     from_vcs_f = handlers.get("pieces_from_vcs")
     if from_vcs_f:
         try:
@@ -2078,15 +2078,15 @@
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
-            with open(ipy, "r") as f:
+            with open(ipy) as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
             print(" replacing boilerplate in %s" % ipy)
@@ -2105,15 +2105,15 @@
     # Make sure both the top-level "versioneer.py" and versionfile_source
     # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
     # they'll be copied into source distributions. Pip won't be able to
     # install the package without this.
     manifest_in = os.path.join(root, "MANIFEST.in")
     simple_includes = set()
     try:
-        with open(manifest_in, "r") as f:
+        with open(manifest_in) as f:
             for line in f:
                 if line.startswith("include "):
                     for include in line.split()[1:]:
                         simple_includes.add(include)
     except OSError:
         pass
     # That doesn't cover everything MANIFEST.in can do
@@ -2144,15 +2144,15 @@
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
-    with open("setup.py", "r") as f:
+    with open("setup.py") as f:
         for line in f.readlines():
             if "import versioneer" in line:
                 found.add("import")
             if "versioneer.get_cmdclass()" in line:
                 found.add("cmdclass")
             if "versioneer.get_version()" in line:
                 found.add("get_version")
```

### Comparing `xbootstrap-0.0.4/xbootstrap/core.py` & `xbootstrap-0.0.5/xbootstrap/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from collections import OrderedDict
-from itertools import chain, islice, cycle
+from itertools import chain, cycle, islice
 
 import numpy as np
 import xarray as xr
 
 
 def _get_blocked_random_indices(
     shape, block_axis, block_size, prev_block_sizes, circular
@@ -395,26 +395,23 @@
                 blocks=blocks,
                 n_iteration=leftover,
                 exclude_dims=exclude_dims,
                 circular=circular,
             )
         )
 
+    bootstraps_concat = tuple(
+        [
+            xr.concat(
+                b,
+                dim="iteration",
+                coords="minimal",
+                compat="override",
+            )
+            for b in zip(*bootstraps)
+        ]
+    )
+
     if len(objects) == 1:
-        return xr.concat(
-            *bootstraps,
-            dim="iteration",
-            coords="minimal",
-            compat="override",
-        )
+        return bootstraps_concat[0]
     else:
-        return tuple(
-            [
-                xr.concat(
-                    b,
-                    dim="iteration",
-                    coords="minimal",
-                    compat="override",
-                )
-                for b in zip(*bootstraps)
-            ]
-        )
+        return bootstraps_concat
```

### Comparing `xbootstrap-0.0.4/xbootstrap/tests/test_core.py` & `xbootstrap-0.0.5/xbootstrap/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import itertools
 
-import pytest
+import dask.array
 import numpy as np
+import pytest
 import xarray as xr
 
 from xbootstrap.core import (
-    _n_nested_blocked_random_indices,
     _expand_n_nested_random_indices,
+    _n_nested_blocked_random_indices,
     block_bootstrap,
 )
 
 
 @pytest.mark.parametrize("shape", [(1,), (2, 50, 6)])
 @pytest.mark.parametrize("n_iteration", [1, 5])
 @pytest.mark.parametrize("circular", [True, False])
@@ -183,19 +184,24 @@
     y = xr.DataArray(data[:, 0], coords={"d0": range(shape[0])})
     x_bs, y_bs = block_bootstrap(x, y, blocks={"d0": block}, n_iteration=n_iteration)
     assert (
         x_bs.isel({f"d{i}": 0 for i in range(1, len(shape))}).values == y_bs.values
     ).all()
 
 
-def test_block_bootstrap_output_type():
-    """Test that"""
-    shape = (10, 5)
-    data = np.zeros(shape)
+@pytest.mark.parametrize(
+    "data",
+    [np.zeros(shape=(10, 5)), dask.array.zeros((240, 240, 240), chunks=(-1, -1, -1))],
+)
+@pytest.mark.parametrize("blocks", [1, 3])
+@pytest.mark.parametrize("n_iteration", [1, 2])
+def test_block_bootstrap_output_type(data, blocks, n_iteration):
+    """Test that output type is correct"""
+    shape = data.shape
     x = xr.DataArray(
         data,
         coords={f"d{i}": range(shape[i]) for i in range(len(shape))},
     )
-    out = block_bootstrap(x, blocks={"d0": 3}, n_iteration=5)
+    out = block_bootstrap(x, blocks={"d0": blocks}, n_iteration=n_iteration)
     assert isinstance(out, xr.DataArray)
-    out = block_bootstrap(x, x, blocks={"d0": 3}, n_iteration=5)
+    out = block_bootstrap(x, x, blocks={"d0": blocks}, n_iteration=n_iteration)
     assert isinstance(out, tuple)
```

