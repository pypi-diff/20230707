# Comparing `tmp/rules_validations-0.1.0.tar.gz` & `tmp/rules_validations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules_validations-0.1.0.tar", max compression
+gzip compressed data, was "rules_validations-0.2.0.tar", max compression
```

## Comparing `rules_validations-0.1.0.tar` & `rules_validations-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       19 2023-07-05 20:31:05.082577 rules_validations-0.1.0/README.md
--rw-r--r--   0        0        0      347 2023-07-05 20:31:21.154800 rules_validations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2321 2023-07-05 20:31:05.082577 rules_validations-0.1.0/rules_validations/__init__.py
--rw-r--r--   0        0        0     1635 2023-07-05 20:31:05.082577 rules_validations-0.1.0/rules_validations/baseEnum.py
--rw-r--r--   0        0        0     1725 2023-07-05 20:31:05.082577 rules_validations-0.1.0/rules_validations/phone.py
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-07-07 15:15:53.543334 rules_validations-0.2.0/README.md
+-rw-r--r--   0        0        0      347 2023-07-07 15:16:05.251261 rules_validations-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-07-07 15:15:53.543334 rules_validations-0.2.0/rules_validations/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-07 15:15:53.543334 rules_validations-0.2.0/rules_validations/baseEnum.py
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.2.0/PKG-INFO
```

### Comparing `rules_validations-0.1.0/rules_validations/__init__.py` & `rules_validations-0.2.0/rules_validations/__init__.py`

 * *Files identical despite different names*

### Comparing `rules_validations-0.1.0/rules_validations/baseEnum.py` & `rules_validations-0.2.0/rules_validations/baseEnum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from enum import IntEnum
 
 
 def normalize_value(value) -> str:
     return value \
         .lower() \
-        .replace('á', 'a') \
-        .replace('é', 'e') \
-        .replace('í', 'i') \
-        .replace('ó', 'o') \
-        .replace('ú', 'u') \
+        .replace('á', 'a').replace('ä', 'a') \
+        .replace('é', 'e').replace('ë', 'e') \
+        .replace('í', 'i').replace('ï', 'i') \
+        .replace('ó', 'o').replace('ö', 'o') \
+        .replace('ú', 'u').replace('ü', 'u') \
         .replace('(', '_') \
         .replace(')', '_') \
         .replace('/', '_') \
         .replace('+', 'p') \
+        .replace(',', '_') \
+        .replace('-', '_') \
         .replace(' ', '_')
 
 
 class BaseEnum(IntEnum):
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
```

