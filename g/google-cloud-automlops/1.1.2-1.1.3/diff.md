# Comparing `tmp/google-cloud-automlops-1.1.2.tar.gz` & `tmp/google-cloud-automlops-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.1.2.tar", last modified: Wed May 31 20:15:39 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.3.tar", last modified: Fri Jul  7 16:21:21 2023, max compression
```

## Comparing `google-cloud-automlops-1.1.2.tar` & `google-cloud-automlops-1.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.844866 google-cloud-automlops-1.1.2/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.837869 google-cloud-automlops-1.1.2/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15625 2023-05-31 14:59:43.000000 google-cloud-automlops-1.1.2/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-30 16:10:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.838063 google-cloud-automlops-1.1.2/AutoMLOps/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.838674 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.839003 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.839460 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/base.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.840225 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11141 2023-05-31 15:01:47.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.841402 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20675 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-05-31 15:06:44.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/component.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/pipeline.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24885 2023-05-30 13:56:22.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/scripts.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8731 2023-05-31 14:09:50.000000 google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/scaffold.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842058 google-cloud-automlops-1.1.2/AutoMLOps/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3167 2023-05-31 14:13:28.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/constants.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9886 2023-05-31 15:19:43.000000 google-cloud-automlops-1.1.2/AutoMLOps/utils/utils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.2/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13880 2023-05-31 20:15:39.844672 google-cloud-automlops-1.1.2/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13012 2023-05-31 17:17:30.000000 google-cloud-automlops-1.1.2/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842846 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13880 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-05-31 20:15:39.000000 google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-31 20:15:39.844920 google-cloud-automlops-1.1.2/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-05-30 16:09:56.000000 google-cloud-automlops-1.1.2/setup.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.842996 google-cloud-automlops-1.1.2/tests/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843382 google-cloud-automlops-1.1.2/tests/unit/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/AutoMLOps_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843562 google-cloud-automlops-1.1.2/tests/unit/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843748 google-cloud-automlops-1.1.2/tests/unit/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/frameworks/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.843945 google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-31 20:15:39.844317 google-cloud-automlops-1.1.2/tests/unit/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.2/tests/unit/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11523 2023-05-30 14:04:41.000000 google-cloud-automlops-1.1.2/tests/unit/utils/utils_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.187656 google-cloud-automlops-1.1.3/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.180937 google-cloud-automlops-1.1.3/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    16076 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-07-07 16:21:06.000000 google-cloud-automlops-1.1.3/AutoMLOps/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181115 google-cloud-automlops-1.1.3/AutoMLOps/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181450 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181774 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.182131 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/base.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.182642 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11141 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.183957 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20750 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-07-07 01:44:52.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/component.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-07-07 01:45:27.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/pipeline.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    25214 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/scripts.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8731 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/scaffold.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.184651 google-cloud-automlops-1.1.3/AutoMLOps/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3229 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9886 2023-07-07 01:45:42.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/utils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.3/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14008 2023-07-07 16:21:21.187439 google-cloud-automlops-1.1.3/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13140 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.185561 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14008 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-07-07 16:21:21.187703 google-cloud-automlops-1.1.3/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-07-07 16:20:51.000000 google-cloud-automlops-1.1.3/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.185735 google-cloud-automlops-1.1.3/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186102 google-cloud-automlops-1.1.3/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/AutoMLOps_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186501 google-cloud-automlops-1.1.3/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186674 google-cloud-automlops-1.1.3/tests/unit/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/frameworks/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186851 google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.187204 google-cloud-automlops-1.1.3/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11523 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/AutoMLOps.py` & `google-cloud-automlops-1.1.3/AutoMLOps/AutoMLOps.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,33 +211,39 @@
         logging.info('Cloud Scheduler Job: https://console.cloud.google.com/cloudscheduler')
 
 def _push_to_csr():
     """Initializes a git repo if one doesn't already exist,
        then pushes to the specified branch and triggers the cloudbuild job.
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
+    csr_remote_origin_url = f'''https://source.developers.google.com/p/{defaults['gcp']['project_id']}/r/{defaults['gcp']['cloud_source_repository']}'''
 
     if not os.path.exists('.git'):
 
         # Initialize git and configure credentials
         execute_process('git init', to_null=False)
         execute_process('''git config --global credential.'https://source.developers.google.com'.helper gcloud.sh''', to_null=False)
 
         # Add repo and branch
-        execute_process(f'''git remote add origin https://source.developers.google.com/p/{defaults['gcp']['project_id']}/r/{defaults['gcp']['cloud_source_repository']}''', to_null=False)
+        execute_process(f'''git remote add origin {csr_remote_origin_url}''', to_null=False)
         execute_process(f'''git checkout -B {defaults['gcp']['cloud_source_repository_branch']}''', to_null=False)
         has_remote_branch = subprocess.check_output([f'''git ls-remote origin {defaults['gcp']['cloud_source_repository_branch']}'''], shell=True, stderr=subprocess.STDOUT)
 
         # This will initialize the branch, a second push will be required to trigger the cloudbuild job after initializing
         if not has_remote_branch:
             execute_process('touch .gitkeep', to_null=False) # needed to keep dir here
             execute_process('git add .gitkeep', to_null=False)
             execute_process('''git commit -m 'init' ''', to_null=False)
             execute_process(f'''git push origin {defaults['gcp']['cloud_source_repository_branch']} --force''', to_null=False)
 
+    # Check for remote origin url mismatch
+    actual_remote = subprocess.check_output(['git config --get remote.origin.url'], shell=True, stderr=subprocess.STDOUT).decode('utf-8').strip('\n')
+    if actual_remote != csr_remote_origin_url:
+        raise RuntimeError(f'Expected remote origin url {csr_remote_origin_url} but found {actual_remote}. Reset your remote origin url to continue.')
+
     # Add, commit, and push changes to CSR
     execute_process(f'touch {BASE_DIR}scripts/pipeline_spec/.gitkeep', to_null=False) # needed to keep dir here
     execute_process('git add .', to_null=False)
     execute_process('''git commit -m 'Run AutoMLOps' ''', to_null=False)
     execute_process(f'''git push origin {defaults['gcp']['cloud_source_repository_branch']} --force''', to_null=False)
     # pylint: disable=logging-fstring-interpolation
     logging.info(f'''Pushing code to {defaults['gcp']['cloud_source_repository_branch']} branch, triggering cloudbuild...''')
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/deployments/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/builder.py` & `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/builder.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/deployments/cloudbuild/constructs/scripts.py` & `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/scripts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/base.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/builder.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/builder.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/cloudrun.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/cloudrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 """Code strings for a kfp cloud run instance."""
 
 # pylint: disable=line-too-long
 
 from AutoMLOps.utils.utils import read_yaml_file
 from AutoMLOps.utils.constants import (
     GENERATED_LICENSE,
+    GENERATED_PIPELINE_JOB_SPEC_PATH,
     LEFT_BRACKET,
+    PINNED_KFP_VERSION,
     RIGHT_BRACKET
 )
 
 class KfpCloudRun():
     """Generates files related to cloud runner service."""
     def __init__(self, defaults_file: str):
         """Instantiate Cloud Run scripts object with all necessary attributes.
@@ -84,15 +86,15 @@
     def _create_cloudrun_base_reqs(self):
         """Returns the text of a cloudrun base requirements file to be written to the cloud_run/run_pipeline directory.
 
         Returns:
             str: Package requirements for cloudrun base.
         """
         return (
-            'kfp\n'
+            f'{PINNED_KFP_VERSION}\n'
             'google-cloud-aiplatform\n'
             'google-cloud-pipeline-components\n'
             'Flask\n'
             'gunicorn\n'
             'pyyaml\n'
         )
 
@@ -132,15 +134,15 @@
             f'''app = flask.Flask(__name__)\n'''
             f'\n'
             f'''logger = logging.getLogger()\n'''
             f'''log_level = os.environ.get('LOG_LEVEL', 'INFO')\n'''
             f'''logger.setLevel(log_level)\n'''
             f'\n'
             f'''CONFIG_FILE = '../../configs/defaults.yaml'\n'''
-            f'''PIPELINE_SPEC_PATH_LOCAL = '../../scripts/pipeline_spec/pipeline_job.json'\n'''
+            f'''PIPELINE_SPEC_PATH_LOCAL = '../../{GENERATED_PIPELINE_JOB_SPEC_PATH}'\n'''
             f'\n'
             f'''@app.route('/', methods=['POST'])\n'''
             f'''def process_request() -> flask.Response:\n'''
             f'''    """HTTP web service to trigger pipeline execution.\n'''
             f'\n'
             f'''    Returns:\n'''
             f'''        The response text, or any set of values that can be turned into a\n'''
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/component.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/component.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/pipeline.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/pipeline.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/constructs/scripts.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 from AutoMLOps.utils.utils import (
     execute_process,
     get_components_list,
     read_file,
     read_yaml_file
 )
 from AutoMLOps.utils.constants import (
-    GENERATED_LICENSE,
-    NEWLINE,
-    LEFT_BRACKET,
-    RIGHT_BRACKET,
     GENERATED_COMPONENT_BASE,
+    GENERATED_LICENSE,
     GENERATED_PARAMETER_VALUES_PATH,
-    GENERATED_PIPELINE_JOB_SPEC_PATH
+    GENERATED_PIPELINE_JOB_SPEC_PATH,
+    LEFT_BRACKET,
+    NEWLINE,
+    PINNED_KFP_VERSION,
+    RIGHT_BRACKET
 )
 
 class KfpScripts():
     """Generates files related to running kubeflow pipelines."""
     def __init__(self,
                  af_registry_location: str,
                  af_registry_name: str,
@@ -488,9 +489,17 @@
         for component_path in components_path_list:
             component_spec = read_yaml_file(component_path)
             reqs = component_spec['implementation']['container']['command'][2]
             formatted_reqs = re.findall('\'([^\']*)\'', reqs)
             user_inp_reqs.extend(formatted_reqs)
         # Remove duplicates
         set_of_requirements = set(user_inp_reqs) if user_inp_reqs else set(pipreqs + default_gcp_reqs)
+        # Remove empty string
+        if '' in set_of_requirements:
+            set_of_requirements.remove('')
+        # Pin kfp version
+        if 'kfp' in set_of_requirements:
+            set_of_requirements.remove('kfp')
+        set_of_requirements.add(PINNED_KFP_VERSION)
+        # Stringify and sort
         reqs_str = ''.join(r+'\n' for r in sorted(set_of_requirements))
         return reqs_str
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/frameworks/kfp/scaffold.py` & `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/scaffold.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/utils/__init__.py` & `google-cloud-automlops-1.1.3/AutoMLOps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/utils/constants.py` & `google-cloud-automlops-1.1.3/AutoMLOps/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,10 @@
 # Generated kfp pipeline metadata name
 DEFAULT_PIPELINE_NAME = 'automlops-pipeline'
 
 # Character substitution constants
 LEFT_BRACKET = '{'
 RIGHT_BRACKET = '}'
 NEWLINE = '\n'
+
+# KFP v2 Migration constant
+PINNED_KFP_VERSION = 'kfp<2.0.0'
```

### Comparing `google-cloud-automlops-1.1.2/AutoMLOps/utils/utils.py` & `google-cloud-automlops-1.1.3/AutoMLOps/utils/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/LICENSE` & `google-cloud-automlops-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/PKG-INFO` & `google-cloud-automlops-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.2
+Version: 1.1.3
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,16 @@
 ```
 - [Application Default Credentials (ADC)](https://cloud.google.com/docs/authentication/provide-credentials-adc) are setup. This can be done through the following commands:
 ```
 gcloud auth application-default login
 gcloud config set account <account@example.com>
 ```
 
+AutoMLOps generates code that is compatible with `kfp<2.0.0`.
+
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
@@ -253,14 +255,16 @@
 
 [Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
 
 [Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
 
 [Alex Ho](mailto:alexanderho@google.com): Engineer
 
+[Kyle Sorensen](mailto:kylesorensen@google.com): Cloud Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `google-cloud-automlops-1.1.2/README.md` & `google-cloud-automlops-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ```
 - [Application Default Credentials (ADC)](https://cloud.google.com/docs/authentication/provide-credentials-adc) are setup. This can be done through the following commands:
 ```
 gcloud auth application-default login
 gcloud config set account <account@example.com>
 ```
 
+AutoMLOps generates code that is compatible with `kfp<2.0.0`.
+
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
@@ -232,14 +234,16 @@
 
 [Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
 
 [Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
 
 [Alex Ho](mailto:alexanderho@google.com): Engineer
 
+[Kyle Sorensen](mailto:kylesorensen@google.com): Cloud Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.2
+Version: 1.1.3
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,16 @@
 ```
 - [Application Default Credentials (ADC)](https://cloud.google.com/docs/authentication/provide-credentials-adc) are setup. This can be done through the following commands:
 ```
 gcloud auth application-default login
 gcloud config set account <account@example.com>
 ```
 
+AutoMLOps generates code that is compatible with `kfp<2.0.0`.
+
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
@@ -253,14 +255,16 @@
 
 [Jesus Orozco](mailto:jesusfc@google.com): Cloud Engineer
 
 [Erin Horning](mailto:ehorning@google.com): Infrastructure Engineer
 
 [Alex Ho](mailto:alexanderho@google.com): Engineer
 
+[Kyle Sorensen](mailto:kylesorensen@google.com): Cloud Engineer
+
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `google-cloud-automlops-1.1.2/google_cloud_automlops.egg-info/SOURCES.txt` & `google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/setup.py` & `google-cloud-automlops-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.1.2',
+    version='1.1.3',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
```

### Comparing `google-cloud-automlops-1.1.2/tests/__init__.py` & `google-cloud-automlops-1.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/AutoMLOps_test.py` & `google-cloud-automlops-1.1.3/tests/unit/AutoMLOps_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/__init__.py` & `google-cloud-automlops-1.1.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/deployments/__init__.py` & `google-cloud-automlops-1.1.3/tests/unit/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/frameworks/__init__.py` & `google-cloud-automlops-1.1.3/tests/unit/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/utils/__init__.py` & `google-cloud-automlops-1.1.3/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.2/tests/unit/utils/utils_test.py` & `google-cloud-automlops-1.1.3/tests/unit/utils/utils_test.py`

 * *Files identical despite different names*

