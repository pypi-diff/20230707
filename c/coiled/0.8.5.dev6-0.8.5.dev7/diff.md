# Comparing `tmp/coiled-0.8.5.dev6.tar.gz` & `tmp/coiled-0.8.5.dev7.tar.gz`

## Comparing `coiled-0.8.5.dev6.tar` & `coiled-0.8.5.dev7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/exceptions.py
--rw-r--r--   0        0        0    25251 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/magic.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/run.py
--rw-r--r--   0        0        0    19898 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/types.py
--rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.5.dev6/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/exceptions.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/magic.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/run.py
+-rw-r--r--   0        0        0    19898 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/types.py
+-rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.5.dev7/PKG-INFO
```

### Comparing `coiled-0.8.5.dev6/coiled/__init__.py` & `coiled-0.8.5.dev7/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/analytics.py` & `coiled-0.8.5.dev7/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/auth.py` & `coiled-0.8.5.dev7/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cluster.py` & `coiled-0.8.5.dev7/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/coiled.yaml` & `coiled-0.8.5.dev7/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/context.py` & `coiled-0.8.5.dev7/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/core.py` & `coiled-0.8.5.dev7/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/exceptions.py` & `coiled-0.8.5.dev7/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/magic.py` & `coiled-0.8.5.dev7/coiled/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,14 @@
                     f.write("Wheel-Version: 1.0\nGenerator: coiled\nRoot-Is-Purelib: true\nTag: py3-none-any\n")
                 src_path = Path(src)
                 for file in recurse_importable_python_files(src_path):
                     if str(file) in ("__init__.py", "__main__.py"):
                         continue
                     dest = unpacked_dir / file
                     dest.parent.mkdir(parents=True, exist_ok=True)
-                    logger.error(f"{file}, {dest}, {src}")
                     shutil.copy(src_path / file, dest)
                 p = await create_subprocess_shell(
                     cmd=f"{executable} -m wheel pack --dest-dir {outdir} {unpacked_dir}",
                     stderr=subprocess.STDOUT,
                     stdout=subprocess.PIPE,
                 )
                 if p.returncode:
```

### Comparing `coiled-0.8.5.dev6/coiled/run.py` & `coiled-0.8.5.dev7/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/scan.py` & `coiled-0.8.5.dev7/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/software.py` & `coiled-0.8.5.dev7/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/types.py` & `coiled-0.8.5.dev7/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/utils.py` & `coiled-0.8.5.dev7/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/websockets.py` & `coiled-0.8.5.dev7/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/config.py` & `coiled-0.8.5.dev7/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/core.py` & `coiled-0.8.5.dev7/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/curl.py` & `coiled-0.8.5.dev7/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/env.py` & `coiled-0.8.5.dev7/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/login.py` & `coiled-0.8.5.dev7/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/package_sync.py` & `coiled-0.8.5.dev7/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/prefect.py` & `coiled-0.8.5.dev7/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/run.py` & `coiled-0.8.5.dev7/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/utils.py` & `coiled-0.8.5.dev7/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/__init__.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/better_logs.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/logs.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/metrics.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/ssh.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/cluster/utils.py` & `coiled-0.8.5.dev7/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/notebook/__init__.py` & `coiled-0.8.5.dev7/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/notebook/notebook.py` & `coiled-0.8.5.dev7/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/__init__.py` & `coiled-0.8.5.dev7/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/amp.py` & `coiled-0.8.5.dev7/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/aws.py` & `coiled-0.8.5.dev7/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/entry.py` & `coiled-0.8.5.dev7/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/gcp.py` & `coiled-0.8.5.dev7/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/cli/setup/prometheus.py` & `coiled-0.8.5.dev7/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/extensions/prefect/runners.py` & `coiled-0.8.5.dev7/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/extensions/prefect/workers.py` & `coiled-0.8.5.dev7/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/__init__.py` & `coiled-0.8.5.dev7/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/cluster.py` & `coiled-0.8.5.dev7/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/core.py` & `coiled-0.8.5.dev7/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/cwi_log_link.py` & `coiled-0.8.5.dev7/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/states.py` & `coiled-0.8.5.dev7/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/widgets/__init__.py` & `coiled-0.8.5.dev7/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/widgets/rich.py` & `coiled-0.8.5.dev7/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/coiled/v2/widgets/util.py` & `coiled-0.8.5.dev7/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/LICENSE` & `coiled-0.8.5.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/README.md` & `coiled-0.8.5.dev7/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/pyproject.toml` & `coiled-0.8.5.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.5.dev6/PKG-INFO` & `coiled-0.8.5.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.5.dev6
+Version: 0.8.5.dev7
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
-Metadata-Version: 2.1 Name: coiled Version: 0.8.5.dev6 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.5.dev7 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

