# Comparing `tmp/coiled-0.8.4.dev4.tar.gz` & `tmp/coiled-0.8.4.dev5.tar.gz`

## Comparing `coiled-0.8.4.dev4.tar` & `coiled-0.8.4.dev5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/exceptions.py
--rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/magic.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/run.py
--rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/types.py
--rw-r--r--   0        0        0    54075 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45637 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26637 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.4.dev4/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/exceptions.py
+-rw-r--r--   0        0        0    25251 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/magic.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/run.py
+-rw-r--r--   0        0        0    19898 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/types.py
+-rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45637 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26637 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.4.dev5/PKG-INFO
```

### Comparing `coiled-0.8.4.dev4/coiled/__init__.py` & `coiled-0.8.4.dev5/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/analytics.py` & `coiled-0.8.4.dev5/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/auth.py` & `coiled-0.8.4.dev5/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cluster.py` & `coiled-0.8.4.dev5/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/coiled.yaml` & `coiled-0.8.4.dev5/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/context.py` & `coiled-0.8.4.dev5/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/core.py` & `coiled-0.8.4.dev5/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/exceptions.py` & `coiled-0.8.4.dev5/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/magic.py` & `coiled-0.8.4.dev5/coiled/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from filelock import BaseFileLock, FileLock
 from packaging.utils import parse_wheel_filename
 from rich.progress import Progress
 
 from coiled.context import track_context
 from coiled.scan import PackageInfo, scan_prefix
 from coiled.types import ArchitectureTypesEnum, PackageLevelEnum, ResolvedPackageInfo
-from coiled.utils import validate_wheel
+from coiled.utils import COILED_LOCAL_PACKAGE_PREFIX, recurse_importable_python_files, validate_wheel
 from coiled.v2.core import CloudV2
 from coiled.v2.widgets.util import simple_progress
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 ANY_AVAILABLE = "ANY-AVAILABLE"
@@ -236,23 +236,22 @@
                 # Create fake metadata to make wheel work
                 dist_info_dir = unpacked_dir / f"{unpacked_dir.name}.dist-info"
                 dist_info_dir.mkdir(parents=True)
                 with open(dist_info_dir / "METADATA", "w") as f:
                     f.write(f"Metadata-Version: 2.1\nName: {pkg_name}\nVersion: {version}\n")
                 with open(dist_info_dir / "WHEEL", "w") as f:
                     f.write("Wheel-Version: 1.0\nGenerator: coiled\nRoot-Is-Purelib: true\nTag: py3-none-any\n")
-                for file in Path(src).rglob("*.py"):
-                    rel_file = file.relative_to(src)
-                    # Skip top-level __init__.py or __main__.py because they
-                    # should not go in site-packages
-                    if str(rel_file) in ("__init__.py", "__main__.py"):
+                src_path = Path(src)
+                for file in recurse_importable_python_files(src_path):
+                    if str(file) in ("__init__.py", "__main__.py"):
                         continue
-                    dest = unpacked_dir / rel_file
+                    dest = unpacked_dir / file
                     dest.parent.mkdir(parents=True, exist_ok=True)
-                    shutil.copy(file, dest)
+                    logger.error(f"{file}, {dest}, {src}")
+                    shutil.copy(src_path / file, dest)
                 p = await create_subprocess_shell(
                     cmd=f"{executable} -m wheel pack --dest-dir {outdir} {unpacked_dir}",
                     stderr=subprocess.STDOUT,
                     stdout=subprocess.PIPE,
                 )
                 if p.returncode:
                     print(
@@ -365,14 +364,18 @@
             )
     coiled_selected_python = None
     if not user_conda_installed_python:
         # insert a special python package
         # that the backend will pick a channel for
         coiled_selected_python = await default_python()
         packages.append(coiled_selected_python)
+
+    local_packages: List[PackageInfo] = [pkg for pkg in packages if pkg["name"].startswith(COILED_LOCAL_PACKAGE_PREFIX)]
+    packages = [pkg for pkg in packages if not pkg["name"].startswith(COILED_LOCAL_PACKAGE_PREFIX)]
+
     with simple_progress("Validating environment", progress=progress):
         results = await cloud._approximate_packages(
             packages=[
                 {
                     "name": pkg["name"],
                     "priority_override": (
                         PackageLevelEnum.CRITICAL
@@ -439,14 +442,24 @@
                     "sdist": None,
                     "md5": None,
                 }
             )
         # we can pull our special python package out of the list
         # now
         packages.remove(coiled_selected_python)
+    for pkg in local_packages:
+        if pkg["wheel_target"]:
+            with simple_progress(f'Creating wheel for {pkg["wheel_target"]}', progress=progress):
+                finalized_packages.append(
+                    await create_wheel_from_src_dir(
+                        pkg_name=pkg["name"],
+                        version=pkg["version"],
+                        src=pkg["wheel_target"],
+                    )
+                )
     for pkg in packages:
         package_result = result_map[(pkg["name"], pkg["conda_name"])]
         if pkg["wheel_target"] and package_result["include"]:
             p = urlparse(pkg["wheel_target"])
             if p.scheme == "" and not Path(pkg["wheel_target"]).exists():
                 # lack of scheme means a local file
                 # sometimes the wheel target taken from
@@ -474,23 +487,14 @@
                     finalized_packages.append(
                         await create_wheel_from_egg(
                             pkg_name=pkg["name"],
                             version=pkg["version"],
                             src=pkg["wheel_target"],
                         )
                     )
-            elif pkg["name"].startswith("coiled_local_"):
-                with simple_progress(f'Creating wheel for {pkg["wheel_target"]}', progress=progress):
-                    finalized_packages.append(
-                        await create_wheel_from_src_dir(
-                            pkg_name=pkg["name"],
-                            version=pkg["version"],
-                            src=pkg["wheel_target"],
-                        )
-                    )
             else:
                 with simple_progress(f'Creating wheel for {pkg["name"]}', progress=progress):
                     finalized_packages.append(
                         await create_wheel(
                             pkg_name=pkg["name"],
                             version=pkg["version"],
                             src=pkg["wheel_target"],
```

### Comparing `coiled-0.8.4.dev4/coiled/run.py` & `coiled-0.8.4.dev5/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/scan.py` & `coiled-0.8.4.dev5/coiled/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from importlib_metadata import Distribution, PackagePath, PathDistribution
 from packaging.version import InvalidVersion
 from packaging.version import parse as parse_version
 from rich.progress import Progress
 from typing_extensions import Literal
 
 from coiled.types import CondaPackage, CondaPlaceHolder, PackageInfo
-from coiled.utils import parse_file_uri
+from coiled.utils import COILED_LOCAL_PACKAGE_PREFIX, parse_file_uri
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 
 
 class ResilientDistribution(PathDistribution):
@@ -448,15 +448,15 @@
     pkg_paths = {pkg["path"].resolve() for pkg in results if pkg["path"]}
     extra_paths = {p.resolve() for p in locations if prefix not in p.parents} - pkg_paths
     for extra_path in extra_paths:
         if not extra_path.is_dir():
             continue
         results.append(
             {
-                "name": f"coiled_local_{extra_path.name.replace('-', '_')}",
+                "name": f"{COILED_LOCAL_PACKAGE_PREFIX}{extra_path.name.replace('-', '_')}",
                 "path": extra_path,
                 "source": "pip",
                 "version": "0.0.0",
                 "channel_url": None,
                 "channel": None,
                 "subdir": None,
                 "conda_name": None,
```

### Comparing `coiled-0.8.4.dev4/coiled/software.py` & `coiled-0.8.4.dev5/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/types.py` & `coiled-0.8.4.dev5/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/utils.py` & `coiled-0.8.4.dev5/coiled/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
     "scheduler_accelerator_type": "nvidia-tesla-t4",
     "scheduler_accelerator_count": 1,
 }
 
 # Directories to ignore when building wheels from source
 IGNORE_PYTHON_DIRS = {"build", "dist", "docs", "tests"}
 
+COILED_LOCAL_PACKAGE_PREFIX = "coiled_local_"
+
 
 class VmType(TypedDict):
     """
     Example:
         {
         'name': 't2d-standard-8',
         'cores': 8,
@@ -1370,32 +1372,55 @@
     if http:
         ports.append(80)
     if https:
         ports.append(443)
     return {"ingress": [{"ports": ports, "cidr": cidr}]}
 
 
+def is_legal_module_file(fpath: Path):
+    return not any([part for part in fpath.parts if contains_invalid_import_characters(part)])
+
+
+def contains_invalid_import_characters(s: str):
+    return any(char in s for char in [".", "-", " "])
+
+
+def is_legal_python_filename(filename: str):
+    return filename.endswith(".py") and not contains_invalid_import_characters(filename[:-3])
+
+
+def recurse_importable_python_files(src: Path):
+    for root, dirs, files in os.walk(src, topdown=True):
+        root_path = Path(root)
+        for d in [d for d in dirs if not is_legal_module_file((root_path / d).relative_to(src))]:
+            # pruning inplace like this works as long as topdown=True
+            dirs.remove(d)
+        for file in [f for f in files if is_legal_python_filename(f)]:
+            fpath = root_path / file
+            rel_file = fpath.relative_to(src)
+            yield rel_file
+
+
 async def validate_wheel(wheel: Path, src: str) -> Tuple[bool, str, Set[str]]:
     """
     Validate a wheel contains some python files and return the md5
 
     Also, warn if there are Python files in src directory that are not
     in the wheel.
     """
     hash = md5()
     has_python = False
     src_path = Path(src)
     if (src_path / "src").exists():
         src_path = src_path / "src"
     src_python_files = set()
-    for p in src_path.rglob("*.py"):
-        relative_path = p.relative_to(src_path)
-        parent_names = {parent.name for parent in relative_path.parents}
+    for p in recurse_importable_python_files(src_path):
+        parent_names = {parent.name for parent in p.parents}
         if not parent_names.intersection(IGNORE_PYTHON_DIRS):
-            src_python_files.add(str(relative_path))
+            src_python_files.add(str(p))
 
     with PyZipFile(str(wheel), mode="r") as wheelzip:
         info = wheelzip.infolist()
         for file in info:
             src_python_files.discard(file.filename)
 
             if not has_python and file.filename != "__init__.py" and file.filename.endswith(".py"):
```

### Comparing `coiled-0.8.4.dev4/coiled/websockets.py` & `coiled-0.8.4.dev5/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/config.py` & `coiled-0.8.4.dev5/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/core.py` & `coiled-0.8.4.dev5/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/curl.py` & `coiled-0.8.4.dev5/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/env.py` & `coiled-0.8.4.dev5/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/login.py` & `coiled-0.8.4.dev5/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/package_sync.py` & `coiled-0.8.4.dev5/coiled/cli/package_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 import click
 from rich.console import Console
 from rich.table import Table
 
 from coiled.scan import scan_prefix
-from coiled.utils import IGNORE_PYTHON_DIRS
+from coiled.utils import COILED_LOCAL_PACKAGE_PREFIX, IGNORE_PYTHON_DIRS, recurse_importable_python_files
 
 
 @click.group()
 def package_sync():
     basicConfig(level=logging.INFO)
 
 
@@ -43,24 +43,23 @@
             pkg["source"],
             pkg["channel"] or "",
             pkg["channel_url"] or "",
             pkg["wheel_target"] or "",
             str(pkg["path"]) if pkg["path"] else "",
         ]
         if verbose:
-            if pkg["name"].startswith("coiled_local_") and pkg["path"]:
+            if pkg["name"].startswith(COILED_LOCAL_PACKAGE_PREFIX) and pkg["path"]:
                 modules = []
-                for path in pkg["path"].rglob("*.py"):
-                    relative_path = path.relative_to(pkg["path"])
-                    parent_names = {parent.name for parent in relative_path.parents}
-                    if not parent_names.intersection(IGNORE_PYTHON_DIRS) and str(relative_path) not in (
+                for path in recurse_importable_python_files(pkg["path"]):
+                    parent_names = {parent.name for parent in path.parents}
+                    if not parent_names.intersection(IGNORE_PYTHON_DIRS) and str(path) not in (
                         "__init__.py",
                         "__main__.py",
                     ):
-                        modules.append(str(relative_path))
+                        modules.append(str(path))
                 row.append("\n".join(modules))
             else:
                 row.append("")
 
         rows.append(row)
 
     rows = sorted(rows, key=lambda x: (x[3], x[0].lower()))
```

### Comparing `coiled-0.8.4.dev4/coiled/cli/prefect.py` & `coiled-0.8.4.dev5/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/run.py` & `coiled-0.8.4.dev5/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/utils.py` & `coiled-0.8.4.dev5/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/__init__.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/better_logs.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/logs.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/metrics.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/ssh.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/cluster/utils.py` & `coiled-0.8.4.dev5/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/notebook/__init__.py` & `coiled-0.8.4.dev5/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/notebook/notebook.py` & `coiled-0.8.4.dev5/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/__init__.py` & `coiled-0.8.4.dev5/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/amp.py` & `coiled-0.8.4.dev5/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/aws.py` & `coiled-0.8.4.dev5/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/entry.py` & `coiled-0.8.4.dev5/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/gcp.py` & `coiled-0.8.4.dev5/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/cli/setup/prometheus.py` & `coiled-0.8.4.dev5/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/extensions/prefect/runners.py` & `coiled-0.8.4.dev5/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/extensions/prefect/workers.py` & `coiled-0.8.4.dev5/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/__init__.py` & `coiled-0.8.4.dev5/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/cluster.py` & `coiled-0.8.4.dev5/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/core.py` & `coiled-0.8.4.dev5/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/cwi_log_link.py` & `coiled-0.8.4.dev5/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/states.py` & `coiled-0.8.4.dev5/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/widgets/__init__.py` & `coiled-0.8.4.dev5/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/widgets/rich.py` & `coiled-0.8.4.dev5/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/coiled/v2/widgets/util.py` & `coiled-0.8.4.dev5/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/LICENSE` & `coiled-0.8.4.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/README.md` & `coiled-0.8.4.dev5/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/pyproject.toml` & `coiled-0.8.4.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.4.dev4/PKG-INFO` & `coiled-0.8.4.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.4.dev4
+Version: 0.8.4.dev5
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.4.dev4 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.4.dev5 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

