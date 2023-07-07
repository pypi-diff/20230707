# Comparing `tmp/inspectds-0.2.0.tar.gz` & `tmp/inspectds-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectds-0.2.0.tar", max compression
+gzip compressed data, was "inspectds-0.2.1.tar", max compression
```

## Comparing `inspectds-0.2.0.tar` & `inspectds-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-04-26 07:05:35.386016 inspectds-0.2.0/LICENSE
--rw-r--r--   0        0        0     2557 2023-04-26 07:05:35.386016 inspectds-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-01-12 14:50:49.718152 inspectds-0.2.0/inspectds/__init__.py
--rw-r--r--   0        0        0     6512 2023-05-15 11:55:20.992929 inspectds-0.2.0/inspectds/cli.py
--rw-r--r--   0        0        0     2284 2023-05-15 11:56:06.299375 inspectds-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 inspectds-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-26 07:05:35.386016 inspectds-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2557 2023-04-26 07:05:35.386016 inspectds-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-01-12 14:50:49.718152 inspectds-0.2.1/inspectds/__init__.py
+-rw-r--r--   0        0        0     6777 2023-07-07 09:27:12.559491 inspectds-0.2.1/inspectds/cli.py
+-rw-r--r--   0        0        0     2284 2023-07-07 09:45:32.167035 inspectds-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 inspectds-0.2.1/PKG-INFO
```

### Comparing `inspectds-0.2.0/LICENSE` & `inspectds-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inspectds-0.2.0/README.md` & `inspectds-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `inspectds-0.2.0/inspectds/cli.py` & `inspectds-0.2.1/inspectds/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,14 +99,41 @@
     elif path.is_dir() or path.suffix == ".zarr" or path.suffix == ".zip":
         dataset_type = DATASET_TYPE.ZARR
     else:
         dataset_type = DATASET_TYPE.NETCDF
     return dataset_type
 
 
+def get_kwargs(dataset_type: DATASET_TYPE) -> dict[str, Any]:
+    open_dataset_kwargs: dict[str, Any] = {}
+    if IS_GRIB_AVAILABLE and dataset_type == DATASET_TYPE.GRIB:
+        open_dataset_kwargs.update(
+            dict(
+                engine="cfgrib",
+                backend_kwargs={"indexpath": ""},
+            )
+        )
+    elif dataset_type == DATASET_TYPE.ZARR:
+        open_dataset_kwargs.update(
+            dict(
+                engine="zarr",
+                consolidated=False,
+            )
+        )
+    elif dataset_type == DATASET_TYPE.NETCDF:
+        open_dataset_kwargs.update(
+            dict(
+                engine="netcdf4",
+            )
+        )
+    else:
+        raise ValueError("WTF??? Unknown Dataset type...")
+    return open_dataset_kwargs
+
+
 def version_callback(value: bool) -> None:
     if value:
         typer.echo(f"inspectds version: {version('inspectds')}")
         raise typer.Exit(code=0)
 
 
 app = typer.Typer(
@@ -130,37 +157,15 @@
     full: Annotated[bool, typer.Option(help="Display full output. Overrides any other option")] = False,
     version: Annotated[bool, typer.Option("--version", help="Display the version", callback=version_callback, is_eager=True)] = False,
     # fmt: on
 ) -> int:
     if dataset_type == DATASET_TYPE.AUTO:
         dataset_type = infer_dataset_type(path)
 
-    open_dataset_kwargs: dict[str, Any] = {}
-    if IS_GRIB_AVAILABLE and dataset_type == DATASET_TYPE.GRIB:
-        open_dataset_kwargs.update(
-            dict(
-                engine="cfgrib",
-                backend_kwargs={"indexpath": ""},
-            )
-        )
-    elif dataset_type == DATASET_TYPE.ZARR:
-        open_dataset_kwargs.update(
-            dict(
-                engine="zarr",
-                consolidated=False,
-            )
-        )
-    elif dataset_type == DATASET_TYPE.NETCDF:
-        open_dataset_kwargs.update(
-            dict(
-                engine="netcdf4",
-            )
-        )
-    else:
-        raise ValueError("WTF??? Unknown Dataset type...")
+    open_dataset_kwargs = get_kwargs(dataset_type=dataset_type)
 
     # Some netcdf files are not compatible with Xarray
     # More specifically you can't have a dimension as a variable too.
     # https://github.com/pydata/xarray/issues/1709#issuecomment-343714896
     # When we find such variables we drop them:
     drop_variables: list[str] = []
     while True:
@@ -178,14 +183,18 @@
                 warnings.warn(f"Dropping scalar variable: {to_be_dropped}", RuntimeWarning)
             else:
                 typer.echo(f"Couldn't open {dataset_type.value} dataset: {str(exc)}")
                 raise typer.Exit(code=33)
         else:
             break
 
+    # Make sure that all the coordinates are loaded
+    for coord in ds.coords:
+        ds[coord].load()
+
     if full:
         dimensions = coordinates = variables = variable_attributes = global_attributes = True
 
     echo_dataset(
         ds=ds,
         dimensions=dimensions,
         coordinates=coordinates,
```

### Comparing `inspectds-0.2.0/pyproject.toml` & `inspectds-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspectds"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Panos Mavrogiorgos <pmav99@gmail.com>"]
 license = "Unlicense"
 readme = "README.md"
 repository = "https://github.com/pmav99/inspectds.git"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `inspectds-0.2.0/PKG-INFO` & `inspectds-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectds
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/pmav99/inspectds.git
 License: Unlicense
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
```

