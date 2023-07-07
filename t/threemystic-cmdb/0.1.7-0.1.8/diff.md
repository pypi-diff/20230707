# Comparing `tmp/threemystic_cmdb-0.1.7.tar.gz` & `tmp/threemystic_cmdb-0.1.8.tar.gz`

## Comparing `threemystic_cmdb-0.1.7.tar` & `threemystic_cmdb-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18763 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/README.md
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    18763 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/README.md
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   
   def _load_cmdb_general_data(self, *args, **kwargs):
     if hasattr(self, "_cmdb_general_data_loaded"):
       return self._cmdb_general_data_loaded
     
     self._cmdb_general_data_loaded = {
       self.get_cmdb_data_action():{
-        "display":"BlobStorage",
+        "display":"CloudStorage",
       }
     }
     return self._load_cmdb_general_data()
   
   def _load_cmdb_column_data(self, *args, **kwargs):
     if hasattr(self, "_cmdb_column_data_loaded"):
       return self._cmdb_column_data_loaded
```

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     cloud_client = main_cloud_data_client( common= self.get_common(), logger_name= "cmdb_init", logger= self.get_common().get_logger())
     cloud_client._setup_another_config(force_config= True)
     
     return False
 
     
   def is_provider_config_completed_only(self, *args, **kwargs):
-    return self.get_config().get("_config_process") is True 
+    return self.get_config().get("_config_process") is True
 
   def is_provider_config_completed(self, *args, **kwargs):
     return self.is_provider_config_completed_only() and self.is_data_client_config_completed()
     
   
   def get_main_directory_name(self, *args, **kwargs):
     return "cmdb"
```

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/.gitignore` & `threemystic_cmdb-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/LICENSE` & `threemystic_cmdb-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/README.md` & `threemystic_cmdb-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.7/pyproject.toml` & `threemystic_cmdb-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.4",
-  "threemystic-cloud-data-client >= 0.1.7",
+  "threemystic-common >= 0.1.5",
+  "threemystic-cloud-data-client >= 0.1.8",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
   "lxml >= 4.9.2",
   "msgraph-sdk >= 1.0.0a12",  
   "polling2 >= 0.5.0",
```

### Comparing `threemystic_cmdb-0.1.7/PKG-INFO` & `threemystic_cmdb-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.7
+Version: 0.1.8
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,16 @@
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-cloud-data-client>=0.1.7
-Requires-Dist: threemystic-common>=0.1.4
+Requires-Dist: threemystic-cloud-data-client>=0.1.8
+Requires-Dist: threemystic-common>=0.1.5
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
 Currently supports AWS/Azure
```

