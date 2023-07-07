# Comparing `tmp/readfcs-1.1.3.tar.gz` & `tmp/readfcs-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readfcs-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "readfcs-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `readfcs-1.1.3.tar` & `readfcs-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2597 2023-02-07 14:48:53.579433 readfcs-1.1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-25 08:22:00.201619 readfcs-1.1.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-25 08:22:00.201910 readfcs-1.1.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1207 2022-08-30 14:21:07.236348 readfcs-1.1.3/.gitignore
--rw-r--r--   0        0        0     1943 2022-07-10 14:01:24.300288 readfcs-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      624 2022-08-30 14:11:54.721602 readfcs-1.1.3/CITATION.cff
--rw-r--r--   0        0        0    11324 2022-05-28 11:31:06.237861 readfcs-1.1.3/LICENSE
--rw-r--r--   0        0        0      759 2023-02-07 14:32:21.099727 readfcs-1.1.3/README.md
--rw-r--r--   0        0        0       49 2022-05-28 10:53:31.440992 readfcs-1.1.3/docs/api.md
--rw-r--r--   0        0        0     3552 2023-06-27 12:27:46.234811 readfcs-1.1.3/docs/changelog.md
--rw-r--r--   0        0        0      277 2023-01-12 16:27:09.497287 readfcs-1.1.3/docs/index.md
--rw-r--r--   0        0        0     5188 2023-06-16 12:31:22.584637 readfcs-1.1.3/docs/quickstart.ipynb
--rw-r--r--   0        0        0      119 2022-08-30 14:11:54.723988 readfcs-1.1.3/lamin-project.yaml
--rw-r--r--   0        0        0      726 2023-01-12 16:27:09.497510 readfcs-1.1.3/noxfile.py
--rw-r--r--   0        0        0      929 2023-06-16 12:31:22.585587 readfcs-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      390 2023-06-27 12:27:40.266451 readfcs-1.1.3/readfcs/__init__.py
--rw-r--r--   0        0        0     8398 2023-06-27 12:27:18.948750 readfcs-1.1.3/readfcs/_core.py
--rw-r--r--   0        0        0       94 2022-08-22 13:26:31.136399 readfcs-1.1.3/readfcs/datasets/__init__.py
--rw-r--r--   0        0        0      362 2022-08-22 13:56:28.582426 readfcs-1.1.3/readfcs/datasets/_datasets.py
--rw-r--r--   0        0        0       88 2022-07-11 14:13:41.976849 readfcs-1.1.3/tests/test_base.py
--rw-r--r--   0        0        0      510 2023-06-16 12:09:07.152399 readfcs-1.1.3/tests/test_notebooks.py
--rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 readfcs-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2597 2023-02-07 14:48:53.579433 readfcs-1.1.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-25 08:22:00.201619 readfcs-1.1.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-25 08:22:00.201910 readfcs-1.1.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1207 2022-08-30 14:21:07.236348 readfcs-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1943 2022-07-10 14:01:24.300288 readfcs-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      624 2022-08-30 14:11:54.721602 readfcs-1.1.4/CITATION.cff
+-rw-r--r--   0        0        0    11324 2022-05-28 11:31:06.237861 readfcs-1.1.4/LICENSE
+-rw-r--r--   0        0        0      759 2023-02-07 14:32:21.099727 readfcs-1.1.4/README.md
+-rw-r--r--   0        0        0       49 2022-05-28 10:53:31.440992 readfcs-1.1.4/docs/api.md
+-rw-r--r--   0        0        0     3713 2023-07-07 09:06:51.394489 readfcs-1.1.4/docs/changelog.md
+-rw-r--r--   0        0        0      277 2023-01-12 16:27:09.497287 readfcs-1.1.4/docs/index.md
+-rw-r--r--   0        0        0     5188 2023-07-06 16:05:30.927180 readfcs-1.1.4/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      119 2022-08-30 14:11:54.723988 readfcs-1.1.4/lamin-project.yaml
+-rw-r--r--   0        0        0      726 2023-01-12 16:27:09.497510 readfcs-1.1.4/noxfile.py
+-rw-r--r--   0        0        0      929 2023-06-16 12:31:22.585587 readfcs-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-07-07 09:06:37.712931 readfcs-1.1.4/readfcs/__init__.py
+-rw-r--r--   0        0        0     8436 2023-07-07 09:05:54.014810 readfcs-1.1.4/readfcs/_core.py
+-rw-r--r--   0        0        0       94 2022-08-22 13:26:31.136399 readfcs-1.1.4/readfcs/datasets/__init__.py
+-rw-r--r--   0        0        0      362 2022-08-22 13:56:28.582426 readfcs-1.1.4/readfcs/datasets/_datasets.py
+-rw-r--r--   0        0        0       88 2022-07-11 14:13:41.976849 readfcs-1.1.4/tests/test_base.py
+-rw-r--r--   0        0        0      510 2023-06-16 12:09:07.152399 readfcs-1.1.4/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 readfcs-1.1.4/PKG-INFO
```

### Comparing `readfcs-1.1.3/.github/workflows/build.yml` & `readfcs-1.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/.github/workflows/latest-changes.yml` & `readfcs-1.1.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/.gitignore` & `readfcs-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/.pre-commit-config.yaml` & `readfcs-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/CITATION.cff` & `readfcs-1.1.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/LICENSE` & `readfcs-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/README.md` & `readfcs-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/docs/changelog.md` & `readfcs-1.1.4/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑️ Make sure channels are sorted by n | [29](https://github.com/laminlabs/readfcs/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-07 | 1.1.4
 🩹 Remove whitespace only markers | [26](https://github.com/laminlabs/readfcs/pull/26) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-27 | 1.1.3
 ➖ Remove nbproject from dependencies | [25](https://github.com/laminlabs/readfcs/pull/25) | [Koncopd](https://github.com/Koncopd) | 2023-06-04 | 1.1.2
 💚 Fix docs | [23](https://github.com/laminlabs/readfcs/pull/23) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-07 |
 🩹 Fill nan with empty string in channels | [22](https://github.com/laminlabs/readfcs/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-07 | 1.1.1
 🚑 Wrote new channels formater | [21](https://github.com/laminlabs/readfcs/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-20 | 1.1.0
 👷 Extend CI to py3.8-3.10 | [20](https://github.com/laminlabs/readfcs/pull/20) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-12 | 1.0.4
 🩹 Convert list columns to str so it saves properly | [19](https://github.com/laminlabs/readfcs/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-08 | 1.0.3
```

### Comparing `readfcs-1.1.3/docs/quickstart.ipynb` & `readfcs-1.1.4/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/noxfile.py` & `readfcs-1.1.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/pyproject.toml` & `readfcs-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.3/readfcs/_core.py` & `readfcs-1.1.4/readfcs/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,25 @@
     # format channels into a dataframe
     k = "$PnN"
     df_groups = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
 
     for k, group in channel_groups.items():
         if k == "$PnN":
             continue
-        df_group = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
+        df_group = pd.DataFrame(group, columns=["n", k]).set_index("n")
         df_groups = df_groups.join(df_group)
 
     # reorder df_groups columns
     df_groups.insert(0, "$PnN", df_groups.pop("$PnN"))
     if "$PnS" in df_groups.columns:
         df_groups.insert(1, "$PnS", df_groups.pop("$PnS"))
     # convert nan to '' otherwise saving to anndata will error
     df_groups.fillna("", inplace=True)
-    meta["channels"] = df_groups
+    # make sure channels are sorted by n
+    meta["channels"] = df_groups.sort_index()
 
     return meta
 
 
 def _get_spill_matrix(matrix_string: str) -> pd.DataFrame:
     """Generate a spill matrix for string.
```

### Comparing `readfcs-1.1.3/PKG-INFO` & `readfcs-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readfcs
-Version: 1.1.3
+Version: 1.1.4
 Summary: Parse fcs files into AnnData.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

