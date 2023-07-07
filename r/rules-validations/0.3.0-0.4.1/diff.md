# Comparing `tmp/rules_validations-0.3.0.tar.gz` & `tmp/rules_validations-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules_validations-0.3.0.tar", max compression
+gzip compressed data, was "rules_validations-0.4.1.tar", max compression
```

## Comparing `rules_validations-0.3.0.tar` & `rules_validations-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-07-07 15:22:27.334001 rules_validations-0.3.0/README.md
--rw-r--r--   0        0        0      347 2023-07-07 15:22:41.718017 rules_validations-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2321 2023-07-07 15:22:27.334001 rules_validations-0.3.0/rules_validations/__init__.py
--rw-r--r--   0        0        0     1872 2023-07-07 15:22:27.334001 rules_validations-0.3.0/rules_validations/baseEnum.py
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-07-07 19:37:10.825817 rules_validations-0.4.1/README.md
+-rw-r--r--   0        0        0      347 2023-07-07 19:37:27.273934 rules_validations-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/baseEnum.py
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.4.1/PKG-INFO
```

### Comparing `rules_validations-0.3.0/rules_validations/__init__.py` & `rules_validations-0.4.1/rules_validations/__init__.py`

 * *Files identical despite different names*

### Comparing `rules_validations-0.3.0/rules_validations/baseEnum.py` & `rules_validations-0.4.1/rules_validations/baseEnum.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     return value \
         .lower() \
         .replace('á', 'a').replace('ä', 'a') \
         .replace('é', 'e').replace('ë', 'e') \
         .replace('í', 'i').replace('ï', 'i') \
         .replace('ó', 'o').replace('ö', 'o') \
         .replace('ú', 'u').replace('ü', 'u') \
+        .replace('ñ', 'n') \
         .replace('(', '_') \
         .replace(')', '_') \
         .replace('/', '_') \
         .replace('+', 'p') \
         .replace('.', '') \
         .replace(',', '_') \
         .replace(':', '') \
@@ -24,26 +25,21 @@
 class BaseEnum(IntEnum):
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, value: str):
-        print(1, value)
         try:
             if type(value) == str:
                 clean_value = normalize_value(value)
-                print(3, clean_value)
                 try:
-                    print(2, cls[clean_value])
                     return cls[clean_value]
                 except KeyError:
-                    print(4, cls(clean_value))
                     return cls(clean_value)
-
             elif type(value) == int:
                 return cls(value)
             else:
                 raise ValueError(f'{value} is not a valid {cls.__name__}')
         except KeyError as e:
             raise ValueError(f'{e} is not a valid {cls.__name__}')
```

