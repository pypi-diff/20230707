# Comparing `tmp/dbt_lineage_viewer-1.0.3.tar.gz` & `tmp/dbt_lineage_viewer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-1.0.3.tar", last modified: Fri Jul  7 03:48:34 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-1.0.4.tar", last modified: Fri Jul  7 03:51:51 2023, max compression
```

## Comparing `dbt_lineage_viewer-1.0.3.tar` & `dbt_lineage_viewer-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:48:34.104230 dbt_lineage_viewer-1.0.3/
--rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-07-07 03:48:34.104230 dbt_lineage_viewer-1.0.3/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-1.0.3/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:48:34.104230 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/
--rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/__init__.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3131 2023-07-07 03:46:06.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/main.py
--rw-r--r--   0 yang      (1000) yang      (1000)     1637 2023-05-01 19:41:55.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/mermaid.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3703 2023-07-07 03:41:26.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/model.py
--rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/utils.py
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:48:34.104230 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-07-07 03:48:34.000000 dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-07-07 03:48:34.104230 dbt_lineage_viewer-1.0.3/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      677 2023-07-07 03:41:11.000000 dbt_lineage_viewer-1.0.3/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:51:51.005553 dbt_lineage_viewer-1.0.4/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-07-07 03:51:51.005553 dbt_lineage_viewer-1.0.4/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-1.0.4/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:51:51.002220 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3130 2023-07-07 03:51:03.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1637 2023-05-01 19:41:55.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3703 2023-07-07 03:41:26.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/model.py
+-rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/utils.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-07-07 03:51:51.005553 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-07-07 03:51:50.000000 dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-07-07 03:51:51.005553 dbt_lineage_viewer-1.0.4/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      677 2023-07-07 03:51:45.000000 dbt_lineage_viewer-1.0.4/setup.py
```

### Comparing `dbt_lineage_viewer-1.0.3/PKG-INFO` & `dbt_lineage_viewer-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 1.0.3
+Version: 1.0.4
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-1.0.3/README.md` & `dbt_lineage_viewer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/main.py` & `dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @click.option("--max-depth", default=0, help="Maximum depth of dependencies.")
 @click.option("--output", default="test.html", help="Output file path.")
 @click.option("--model-dir-name", default="models", help="Model folder name")
 @click.option("--data-dir-name", default="data", help="Data folder name")
 @click.option("--snapshot-dir-name", default="snapshots", help="Snapshots folder name")
 @click.option("--upstream-only", is_flag=True, help="Show upstream models only.")
 @click.option("--downstream-only", is_flag=True, help="Show downstream models only.")
-@click.option("--mermaid-code-only", is_flag=False, help="Show mermaid code only.")
+@click.option("--mermaid-code-only", is_flag=True, help="Show mermaid code only.")
 def main(
     model_name: str,
     max_depth: int,
     output: str,
     model_dir_name: str,
     data_dir_name: str,
     snapshot_dir_name,
```

### Comparing `dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/mermaid.py` & `dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/mermaid.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0.3/dbt_lineage_viewer/model.py` & `dbt_lineage_viewer-1.0.4/dbt_lineage_viewer/model.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0.3/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-1.0.4/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 1.0.3
+Version: 1.0.4
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-1.0.3/setup.py` & `dbt_lineage_viewer-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="1.0.3",
+    version="1.0.4",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

