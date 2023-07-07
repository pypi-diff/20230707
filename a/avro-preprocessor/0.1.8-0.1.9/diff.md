# Comparing `tmp/avro-preprocessor-0.1.8.tar.gz` & `tmp/avro-preprocessor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/avro-preprocessor-0.1.8.tar", last modified: Mon Aug 30 15:02:41 2021, max compression
+gzip compressed data, was "avro-preprocessor-0.1.9.tar", last modified: Mon Aug 30 16:06:42 2021, max compression
```

## Comparing `avro-preprocessor-0.1.8.tar` & `avro-preprocessor-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      550 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/COPYING
--rw-r--r--   0 root         (0) root         (0)    12536 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12201 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/avro_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3136 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/avro_naming.py
--rw-rw-rw-   0 root         (0) root         (0)     7186 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/avro_paths.py
--rw-rw-rw-   0 root         (0) root         (0)     6137 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/avropreprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/colored_json.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/extended_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3042 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/avro_sorter.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/documentation_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/documentation_list_condenser.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/java_classes_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/keys_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/metadata_adder.py
--rw-rw-rw-   0 root         (0) root         (0)     3588 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/names_checker.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/namespace_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     6513 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/nullable_optional_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/references_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_dependencies_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     6679 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_mapping_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5029 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_registrar.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_registry_checker.py
--rwxrwxrwx   0 root         (0) root         (0)     6023 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/preprocessor_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/schemas_container.py
--rw-rw-rw-   0 root         (0) root         (0)    34039 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/avro_preprocessor/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12536 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1337 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/avro_preprocessor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-30 15:02:41.000000 avro-preprocessor-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      821 2021-08-30 15:02:30.000000 avro-preprocessor-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 16:06:42.253311 avro-preprocessor-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/COPYING
+-rw-r--r--   0 root         (0) root         (0)    12536 2021-08-30 16:06:42.253311 avro-preprocessor-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12201 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 16:06:42.246894 avro-preprocessor-0.1.9/avro_preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/avro_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3136 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/avro_naming.py
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/avro_paths.py
+-rw-rw-rw-   0 root         (0) root         (0)     6137 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/avropreprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/colored_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/extended_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 16:06:42.253311 avro-preprocessor-0.1.9/avro_preprocessor/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/avro_sorter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/documentation_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/documentation_list_condenser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/java_classes_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/keys_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/metadata_adder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/names_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/namespace_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6513 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/nullable_optional_expander.py
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/references_expander.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_dependencies_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6679 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_mapping_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5029 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_registry_checker.py
+-rwxrwxrwx   0 root         (0) root         (0)     6023 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/preprocessor_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/schemas_container.py
+-rw-rw-rw-   0 root         (0) root         (0)    34039 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/avro_preprocessor/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-30 16:06:42.248728 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12536 2021-08-30 16:06:42.000000 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1337 2021-08-30 16:06:42.000000 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-30 16:06:42.000000 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2021-08-30 16:06:42.000000 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2021-08-30 16:06:42.000000 avro-preprocessor-0.1.9/avro_preprocessor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-30 16:06:42.253311 avro-preprocessor-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      821 2021-08-30 16:06:31.000000 avro-preprocessor-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `avro-preprocessor-0.1.8/COPYING` & `avro-preprocessor-0.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/PKG-INFO` & `avro-preprocessor-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro-preprocessor
-Version: 0.1.8
+Version: 0.1.9
 Summary: A preprocessor for Avro Schemata
 Home-page: https://gitlab.com/Jaumo/avro-preprocessor
 Author: Jaumo GmbH
 Author-email: nicola.bova@jaumo.com
 License: Apache2
 Keywords: avro,preprocessor,schema,schemas,schemata
 Platform: UNKNOWN
```

### Comparing `avro-preprocessor-0.1.8/README.md` & `avro-preprocessor-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/avro_domain.py` & `avro-preprocessor-0.1.9/avro_preprocessor/avro_domain.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/avro_naming.py` & `avro-preprocessor-0.1.9/avro_preprocessor/avro_naming.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/avro_paths.py` & `avro-preprocessor-0.1.9/avro_preprocessor/avro_paths.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/avropreprocessor.py` & `avro-preprocessor-0.1.9/avro_preprocessor/avropreprocessor.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/colored_json.py` & `avro-preprocessor-0.1.9/avro_preprocessor/colored_json.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/avro_sorter.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/avro_sorter.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/documentation_checker.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/documentation_checker.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/documentation_list_condenser.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/documentation_list_condenser.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/java_classes_creator.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/java_classes_creator.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/keys_generator.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/keys_generator.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/metadata_adder.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/metadata_adder.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/names_checker.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/names_checker.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/namespace_checker.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/namespace_checker.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/nullable_optional_expander.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/nullable_optional_expander.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/references_expander.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/references_expander.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_dependencies_checker.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_dependencies_checker.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_mapping_generator.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_registrar.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_registrar.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/modules/schema_registry_checker.py` & `avro-preprocessor-0.1.9/avro_preprocessor/modules/schema_registry_checker.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/preprocessor.py` & `avro-preprocessor-0.1.9/avro_preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/preprocessor_module.py` & `avro-preprocessor-0.1.9/avro_preprocessor/preprocessor_module.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/schemas_container.py` & `avro-preprocessor-0.1.9/avro_preprocessor/schemas_container.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor/tests.py` & `avro-preprocessor-0.1.9/avro_preprocessor/tests.py`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor.egg-info/PKG-INFO` & `avro-preprocessor-0.1.9/avro_preprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro-preprocessor
-Version: 0.1.8
+Version: 0.1.9
 Summary: A preprocessor for Avro Schemata
 Home-page: https://gitlab.com/Jaumo/avro-preprocessor
 Author: Jaumo GmbH
 Author-email: nicola.bova@jaumo.com
 License: Apache2
 Keywords: avro,preprocessor,schema,schemas,schemata
 Platform: UNKNOWN
```

### Comparing `avro-preprocessor-0.1.8/avro_preprocessor.egg-info/SOURCES.txt` & `avro-preprocessor-0.1.9/avro_preprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avro-preprocessor-0.1.8/setup.py` & `avro-preprocessor-0.1.9/setup.py`

 * *Files identical despite different names*

