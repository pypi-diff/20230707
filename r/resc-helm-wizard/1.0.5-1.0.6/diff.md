# Comparing `tmp/resc_helm_wizard-1.0.5.tar.gz` & `tmp/resc_helm_wizard-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.5.tar", last modified: Fri Jun 16 07:51:12 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.0.6.tar", last modified: Fri Jul  7 10:58:25 2023, max compression
```

## Comparing `resc_helm_wizard-1.0.5.tar` & `resc_helm_wizard-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.438409 resc_helm_wizard-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.438409 resc_helm_wizard-1.0.5/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/example-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.400952 resc_helm_wizard-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/example-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.5/PKG-INFO` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resc_helm_wizard
-Version: 1.0.5
+Name: resc-helm-wizard
+Version: 1.0.6
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.5/setup.cfg` & `resc_helm_wizard-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.5
+version = 1.0.6
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/common.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/example-values.yaml` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/example-values.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 resc-vcs-scraper-projects:
   config:
     schedule: "0 6 * * 6"
     successfulJobsHistoryLimit: 1
     failedJobsHistoryLimit: 1
 
-resc-vcs-scraper-repositories:
-  config:
-    scan_only_master_branch: true # Set this to false if you want to scan all branches
-
 resc-vcs-scanner-secrets:
   config:
     force_base_scan: "false" # force_base_scan is set to false in order to enable incremental scanning of commits. If set to true, all commits will be scanned each time.
   resources:
     requests:
       cpu: 300m
       memory: 300M
```

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_value.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/questions.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/run_wizard.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/validator.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resc-helm-wizard
-Version: 1.0.5
+Name: resc_helm_wizard
+Version: 1.0.6
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

