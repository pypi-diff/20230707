# Comparing `tmp/threemystic_common-0.1.6.tar.gz` & `tmp/threemystic_common-0.1.7.tar.gz`

## Comparing `threemystic_common-0.1.6.tar` & `threemystic_common-0.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/__version__.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/common.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/base.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/base_common.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/base_general.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/base_provider.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/base_script_options.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/generate_data/generate_data_handlers.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/base_class/generate_data/handlers/base.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/cli/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/app_monitoring/common.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/app_monitoring/performance.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/cmdb/aws.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/cmdb/azure.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/cmdb/common.py
--rw-r--r--   0        0        0    15045 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/cmdb/base_class/base.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/encryption/common.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/encryption/hash.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/exception/argument.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/exception/common.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/exception/function.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/exception/generic.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/exception/base_class/base.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/generate_data/generate.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/graph/common.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/graph/msgraph.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/graph/base_class/base.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/graph/config/msgraph.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/hashicorp/common.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/hashicorp/vault.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/app.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/config.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/json.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/parallel_processing.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/path.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/yaml.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/bool.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/common.py
--rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/datetime.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/dictionary.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/general.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/int.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/list.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/logging.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/openpyxl.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/regex.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/requests.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/domain/helpers/type/string.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/threemystic_common/exceptions/generate_data/quit.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/hatch.toml
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 threemystic_common-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/__version__.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/common.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/base.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/base_common.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/base_general.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/base_provider.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/base_script_options.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/generate_data/generate_data_handlers.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/base_class/generate_data/handlers/base.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/cli/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/app_monitoring/common.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/app_monitoring/performance.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/cmdb/aws.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/cmdb/azure.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/cmdb/common.py
+-rw-r--r--   0        0        0    15045 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/cmdb/base_class/base.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/encryption/common.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/encryption/hash.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/exception/argument.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/exception/common.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/exception/function.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/exception/generic.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/exception/base_class/base.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/generate_data/generate.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/graph/common.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/graph/msgraph.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/graph/base_class/base.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/graph/config/msgraph.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/hashicorp/common.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/hashicorp/vault.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/app.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/config.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/json.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/parallel_processing.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/path.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/yaml.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/bool.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/common.py
+-rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/datetime.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/dictionary.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/general.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/int.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/list.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/logging.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/openpyxl.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/regex.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/requests.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/domain/helpers/type/string.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/threemystic_common/exceptions/generate_data/quit.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/hatch.toml
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 threemystic_common-0.1.7/PKG-INFO
```

### Comparing `threemystic_common-0.1.6/threemystic_common/common.py` & `threemystic_common-0.1.7/threemystic_common/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/base_class/base.py` & `threemystic_common-0.1.7/threemystic_common/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/base_class/base_provider.py` & `threemystic_common-0.1.7/threemystic_common/base_class/base_provider.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/base_class/base_script_options.py` & `threemystic_common-0.1.7/threemystic_common/base_class/base_script_options.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/base_class/generate_data/handlers/base.py` & `threemystic_common-0.1.7/threemystic_common/base_class/generate_data/handlers/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/app_monitoring/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/app_monitoring/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/app_monitoring/performance.py` & `threemystic_common-0.1.7/threemystic_common/domain/app_monitoring/performance.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/cmdb/aws.py` & `threemystic_common-0.1.7/threemystic_common/domain/cmdb/aws.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/cmdb/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/cmdb/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/cmdb/base_class/base.py` & `threemystic_common-0.1.7/threemystic_common/domain/cmdb/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/encryption/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/encryption/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/encryption/hash.py` & `threemystic_common-0.1.7/threemystic_common/domain/encryption/hash.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/exception/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/exception/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/exception/base_class/base.py` & `threemystic_common-0.1.7/threemystic_common/domain/exception/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/generate_data/generate.py` & `threemystic_common-0.1.7/threemystic_common/domain/generate_data/generate.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/graph/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/graph/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/graph/msgraph.py` & `threemystic_common-0.1.7/threemystic_common/domain/graph/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/graph/base_class/base.py` & `threemystic_common-0.1.7/threemystic_common/domain/graph/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/graph/config/msgraph.py` & `threemystic_common-0.1.7/threemystic_common/domain/graph/config/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/hashicorp/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/hashicorp/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/app.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/app.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/config.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/config.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/json.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/json.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/parallel_processing.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/parallel_processing.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/path.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/path.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/yaml.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/bool.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/bool.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/common.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/datetime.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
       tick_startdate = datetime(year= 1, month= 1, day= 1, hour= 0, minute= 0, tzinfo= dateutil_tz.tzutc())
 
     tick_startdate = self.convert_to_utc(tick_startdate)
     return (dt - tick_startdate).total_seconds()
 
   # datetime_ticks
   def ticks(self, dt, tick_startdate = datetime(year= 1, month= 1, day= 1, hour= 0, minute= 0, tzinfo= dateutil_tz.tzutc()), *args, **kwargs):
-    return self.datetime_ticks_as_seconds(dt= dt, tick_startdate= tick_startdate) * 10**7
+    return self.ticks_as_seconds(dt= dt, tick_startdate= tick_startdate) * 10**7
   
   # isTokenExpired_Now
   def is_token_expired_now(self, compare_datetime, buffer_delta = timedelta(seconds=300)):   
     return (self.convert_utc(compare_datetime) <= (self.convert_utc(self.get(time_zone= "local")) - buffer_delta))
 
   # isTokenExpired_Duration
   def is_token_expired(self, token_life_duration, start_time = None, buffer_delta = timedelta(seconds=60), time_zone= "utc", *args, **kwargs):
```

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/dictionary.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/dictionary.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/general.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/general.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/list.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/list.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/logging.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/logging.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/regex.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/regex.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/requests.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/requests.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/threemystic_common/domain/helpers/type/string.py` & `threemystic_common-0.1.7/threemystic_common/domain/helpers/type/string.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/.gitignore` & `threemystic_common-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/LICENSE` & `threemystic_common-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/README.md` & `threemystic_common-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/hatch.toml` & `threemystic_common-0.1.7/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/pyproject.toml` & `threemystic_common-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.6/PKG-INFO` & `threemystic_common-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-common
-Version: 0.1.6
+Version: 0.1.7
 Summary: Common Library for for various tool sets
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_common
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_common/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

