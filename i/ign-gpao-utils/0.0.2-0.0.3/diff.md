# Comparing `tmp/ign-gpao-utils-0.0.2.tar.gz` & `tmp/ign-gpao-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-utils-0.0.2.tar", last modified: Thu May 25 15:31:26 2023, max compression
+gzip compressed data, was "ign-gpao-utils-0.0.3.tar", last modified: Fri Jul  7 12:51:38 2023, max compression
```

## Comparing `ign-gpao-utils-0.0.2.tar` & `ign-gpao-utils-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/gpao_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/gpao_utils/utils_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 15:31:26.000000 ign-gpao-utils-0.0.2/ign_gpao_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:26.540844 ign-gpao-utils-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 15:31:22.000000 ign-gpao-utils-0.0.2/test/test_utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/gpao_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/gpao_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/gpao_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/gpao_utils/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/gpao_utils/utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/ign_gpao_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-07 12:51:38.000000 ign-gpao-utils-0.0.3/ign_gpao_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 12:51:38.000000 ign-gpao-utils-0.0.3/ign_gpao_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:51:38.000000 ign-gpao-utils-0.0.3/ign_gpao_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 12:51:38.000000 ign-gpao-utils-0.0.3/ign_gpao_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:51:38.510029 ign-gpao-utils-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 12:51:24.000000 ign-gpao-utils-0.0.3/test/test_utils_store.py
```

### Comparing `ign-gpao-utils-0.0.2/gpao_utils/utils_store.py` & `ign-gpao-utils-0.0.3/gpao_utils/utils_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     def to_win(self, dir: str):
         res = dir.replace(self._unix_path, self._win_path)
         # res = res.replace("/", "\\")
         return res
 
 @staticmethod    
-def frame_store(i: int):
-    layout_store = [
-        [   sg.Text(f" {i} - Lettre (sur ma machine Windows)", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{i}-WIN-LETTER", "L:"), key=f"-MAP-STORE{i}-WIN-LETTER", size=(iu.size_text_big, {i})) ],
-        [   sg.Text(f" {i} - store Windows ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{i}-WIN", "//store.ign.fr/store-lidarhd"), key=f"-MAP-STORE{i}-WIN", size=(iu.size_text_big, 1))],
-        [   sg.Text(f" {i} - store Linux ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{i}-UNIX", "/var/data/store-lidarhd"), key=f"-MAP-STORE{i}-UNIX", size=(iu.size_text_big, 1)) ]
-    ]
+def frame_store(i: int, L: list):
+    if len(L)!=i :
+        raise RuntimeError(f"Not the same number of store in parameters. Number : {i}, List : {L}")
+    layout_store = []
+    for j in range(i):
+        layout_store.append([   sg.Text(f" {j} - Lettre (sur ma machine Windows)", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN-LETTER", "L:"), key=f"-MAP-STORE{j}-WIN-LETTER", size=(iu.size_text_big,{j})) ])
+        layout_store.append([   sg.Text(f" {j} - store Windows ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN", f"//store.ign.fr/{L[j]}"), key=f"-MAP-STORE{j}-WIN", size=(iu.size_text_big, 1))])
+        layout_store.append([   sg.Text(f" {j} - store Linux ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-UNIX", f"/var/data/store-{L[j]}"), key=f"-MAP-STORE{j}-UNIX", size=(iu.size_text_big, 1)) ])
     return sg.Frame("", layout_store)
```

### Comparing `ign-gpao-utils-0.0.2/setup.py` & `ign-gpao-utils-0.0.3/setup.py`

 * *Files identical despite different names*

