# Comparing `tmp/libcove-0.30.0.tar.gz` & `tmp/libcove-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcove-0.30.0.tar", last modified: Wed Mar 15 14:46:45 2023, max compression
+gzip compressed data, was "libcove-0.31.0.tar", last modified: Fri Jul  7 10:21:00 2023, max compression
```

## Comparing `libcove-0.30.0.tar` & `libcove-0.31.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-15 14:46:45.584982 libcove-0.30.0/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      899 2022-11-23 18:22:15.000000 libcove-0.30.0/LICENSE
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      383 2023-03-15 14:46:45.584982 libcove-0.30.0/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      791 2022-11-23 18:22:15.000000 libcove-0.30.0/README.md
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-15 14:46:45.580982 libcove-0.30.0/libcove/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      440 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/config.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-15 14:46:45.584982 libcove-0.30.0/libcove/lib/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/lib/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    56964 2023-03-10 10:52:56.000000 libcove-0.30.0/libcove/lib/common.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9076 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/lib/converters.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      812 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/lib/exceptions.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3046 2022-11-23 18:22:15.000000 libcove-0.30.0/libcove/lib/tools.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-15 14:46:45.580982 libcove-0.30.0/libcove.egg-info/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      383 2023-03-15 14:46:45.000000 libcove-0.30.0/libcove.egg-info/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      347 2023-03-15 14:46:45.000000 libcove-0.30.0/libcove.egg-info/SOURCES.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-03-15 14:46:45.000000 libcove-0.30.0/libcove.egg-info/dependency_links.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      120 2023-03-15 14:46:45.000000 libcove-0.30.0/libcove.egg-info/requires.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        8 2023-03-15 14:46:45.000000 libcove-0.30.0/libcove.egg-info/top_level.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       61 2023-03-15 14:46:45.584982 libcove-0.30.0/setup.cfg
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      795 2023-03-10 14:25:28.000000 libcove-0.30.0/setup.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-07 10:21:00.851448 libcove-0.31.0/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      899 2022-11-23 18:22:15.000000 libcove-0.31.0/LICENSE
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      383 2023-07-07 10:21:00.851448 libcove-0.31.0/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      791 2022-11-23 18:22:15.000000 libcove-0.31.0/README.md
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-07 10:21:00.847448 libcove-0.31.0/libcove/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2022-11-23 18:22:15.000000 libcove-0.31.0/libcove/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      440 2022-11-23 18:22:15.000000 libcove-0.31.0/libcove/config.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-07 10:21:00.851448 libcove-0.31.0/libcove/lib/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2022-11-23 18:22:15.000000 libcove-0.31.0/libcove/lib/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    57474 2023-07-06 14:23:47.000000 libcove-0.31.0/libcove/lib/common.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9076 2022-11-23 18:22:15.000000 libcove-0.31.0/libcove/lib/converters.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      812 2022-11-23 18:22:15.000000 libcove-0.31.0/libcove/lib/exceptions.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3048 2023-07-06 14:43:28.000000 libcove-0.31.0/libcove/lib/tools.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-07 10:21:00.847448 libcove-0.31.0/libcove.egg-info/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      383 2023-07-07 10:21:00.000000 libcove-0.31.0/libcove.egg-info/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      347 2023-07-07 10:21:00.000000 libcove-0.31.0/libcove.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-07-07 10:21:00.000000 libcove-0.31.0/libcove.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      120 2023-07-07 10:21:00.000000 libcove-0.31.0/libcove.egg-info/requires.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        8 2023-07-07 10:21:00.000000 libcove-0.31.0/libcove.egg-info/top_level.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       61 2023-07-07 10:21:00.851448 libcove-0.31.0/setup.cfg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      795 2023-07-06 15:19:23.000000 libcove-0.31.0/setup.py
```

### Comparing `libcove-0.30.0/LICENSE` & `libcove-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libcove-0.30.0/README.md` & `libcove-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `libcove-0.30.0/libcove/lib/common.py` & `libcove-0.31.0/libcove/lib/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 import functools
 import json
 import logging
 import numbers
 import os
 import re
+import shutil
 from tempfile import NamedTemporaryFile
 from urllib.parse import urljoin, urlparse, urlsplit
 from urllib.request import urlopen
 
 import jsonref
 import jsonschema.validators
 import requests
@@ -716,19 +717,17 @@
         for value in values:
             if str(value) in codelist_values:
                 continue
 
             path_string = "/".join(path_no_num)
 
             if path_string not in additional_codelist_values:
-
                 codelist_url = schema_obj.codelists + codelist
                 codelist_amend_urls = []
                 if hasattr(schema_obj, "extended_codelist_urls"):
-
                     # Replace URL if this codelist is overridden by an extension.
                     # Last one to be applied wins.
                     if schema_obj.extended_codelist_urls.get(codelist):
                         codelist_url = schema_obj.extended_codelist_urls[codelist][-1]
 
                     codelistadd = f"+{codelist}"
                     codelistsub = f"-{codelist}"
@@ -767,15 +766,14 @@
 def get_additional_fields_info(json_data, schema_fields, context, fields_regex=False):
     fields_present = get_fields_present_with_examples(json_data)
 
     additional_fields = {}
     root_additional_fields = set()
 
     for field, field_info in fields_present.items():
-
         if field in schema_fields:
             continue
         if fields_regex and LANGUAGE_RE.search(field.split("/")[-1]):
             continue
 
         for root_additional_field in root_additional_fields:
             if field.startswith(root_additional_field):
@@ -800,15 +798,14 @@
     json_data,
     schema_obj,
     schema_name,
     context,
     fields_regex=False,
     additional_fields_info=None,
 ):
-
     if not additional_fields_info:
         schema_fields = schema_obj.get_pkg_schema_fields()
         additional_fields_info = get_additional_fields_info(
             json_data, schema_fields, context, fields_regex=False
         )
 
     return [
@@ -846,14 +843,20 @@
         resolver = CustomRefResolver(
             "",
             pkg_schema_obj,
             config=getattr(schema_obj, "config", None),
             schema_url=schema_obj.schema_host,
         )
 
+    # Force jsonschema to use our validator.
+    # https://github.com/python-jsonschema/jsonschema/issues/994
+    jsonschema.validators.validates("http://json-schema.org/draft-04/schema#")(
+        validator
+    )
+
     our_validator = validator(
         pkg_schema_obj, format_checker=format_checker, resolver=resolver
     )
     for e in our_validator.iter_errors(json_data):
         message = e.message
         path = "/".join(str(item) for item in e.path)
         path_no_number = "/".join(
@@ -883,15 +886,15 @@
         # set it
         instance = None
 
         if not header and len(e.path):
             header = e.path[-1]
             if isinstance(e.path[-1], int) and len(e.path) >= 2:
                 # We're dealing with elements in an array of items at this point
-                pre_header = "Array Element "
+                pre_header = "Array element "
                 header_extra = "{}/[number]".format(e.path[-2])
 
         null_clause = ""
         validator_type = e.validator
         if e.validator in ("format", "type"):
             validator_type = e.validator_value
             if isinstance(e.validator_value, list):
@@ -996,14 +999,21 @@
             "reprs": getattr(e, "reprs", None),
         }
         if instance is not None:
             unique_validator_key["instance"] = instance
         validation_errors[
             json.dumps(unique_validator_key, default=decimal_default)
         ].append(value)
+
+    # Restore jsonschema's default validator, to not interfere with other software.
+    # https://github.com/python-jsonschema/jsonschema/issues/994
+    jsonschema.validators.validates("http://json-schema.org/draft-04/schema#")(
+        jsonschema.validators.Draft4Validator
+    )
+
     return dict(validation_errors)
 
 
 def get_json_data_generic_paths(json_data, generic_paths, path=(), generic_key=()):
     """Transform json data into a dictionary with keys made of json paths.
 
     Key are json paths (as tuples). Values are dictionaries with keys including specific
@@ -1441,15 +1451,15 @@
             # We have tried locally and remotely with no luck. We have to raise.
             raise e
 
         org_id_file_contents["downloaded"] = "%s" % today
         # Use a tempfile and move to create new file here for atomicity
         with NamedTemporaryFile(mode="w", delete=False) as tmp:
             json.dump(org_id_file_contents, tmp, indent=2)
-        os.rename(tmp.name, local_org_ids_file)
+        shutil.move(tmp.name, local_org_ids_file)
     # Return either the original file data, if it was found to be fresh, or the new data, if we were able to retrieve it.
     return [org_list["code"] for org_list in org_id_file_contents["lists"]]
 
 
 def add_field_coverage(schema_dict, json_data):
     """
     Takes a schema dict and adds non-zero coverage counts of successes and
```

### Comparing `libcove-0.30.0/libcove/lib/converters.py` & `libcove-0.31.0/libcove/lib/converters.py`

 * *Files identical despite different names*

### Comparing `libcove-0.30.0/libcove/lib/exceptions.py` & `libcove-0.31.0/libcove/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `libcove-0.30.0/libcove/lib/tools.py` & `libcove-0.31.0/libcove/lib/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import lru_cache, wraps
 
 import requests
 
 from .exceptions import UnrecognisedFileType
 
 
-@lru_cache(maxsize=64)
+@lru_cache(maxsize=None)
 def cached_get_request(url):
     return requests.get(url)
 
 
 def get_request(url, config=None, force_cache=False):
     if force_cache or (
         config
```

### Comparing `libcove-0.30.0/setup.py` & `libcove-0.31.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="libcove",
-    version="0.30.0",
+    version="0.31.0",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     url="https://github.com/OpenDataServices/lib-cove",
     description="A data review library",
     packages=find_packages(),
     long_description="A data review library",
     install_requires=[
```

