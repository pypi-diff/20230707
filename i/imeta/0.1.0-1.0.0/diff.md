# Comparing `tmp/imeta-0.1.0-py3-none-any.whl.zip` & `tmp/imeta-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4118 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1756 b- defN 23-Jul-07 03:14 imeta/__init__.py
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 03:14 imeta/exceptions.py
--rw-r--r--  2.0 unx      849 b- defN 23-Jul-07 03:14 imeta/schema.py
--rw-r--r--  2.0 unx      891 b- defN 23-Jul-07 03:14 imeta/serializer.py
--rw-r--r--  2.0 unx     1881 b- defN 23-Jul-07 03:15 imeta/schema/1.0.json
--rw-r--r--  2.0 unx      924 b- defN 23-Jul-07 03:15 imeta-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 03:15 imeta-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 03:15 imeta-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      661 b- defN 23-Jul-07 03:15 imeta-0.1.0.dist-info/RECORD
-9 files, 7212 bytes uncompressed, 2990 bytes compressed:  58.5%
+Zip file size: 4119 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1756 b- defN 23-Jul-07 03:25 imeta/__init__.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 03:25 imeta/exceptions.py
+-rw-r--r--  2.0 unx      849 b- defN 23-Jul-07 03:25 imeta/schema.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Jul-07 03:25 imeta/serializer.py
+-rw-r--r--  2.0 unx     1881 b- defN 23-Jul-07 03:25 imeta/schema/1.0.json
+-rw-r--r--  2.0 unx      924 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      661 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/RECORD
+9 files, 7212 bytes uncompressed, 2991 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: imeta/serializer.py
 Comment: 
 
 Filename: imeta/schema/1.0.json
 Comment: 
 
-Filename: imeta-0.1.0.dist-info/METADATA
+Filename: imeta-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: imeta-0.1.0.dist-info/WHEEL
+Filename: imeta-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: imeta-0.1.0.dist-info/top_level.txt
+Filename: imeta-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: imeta-0.1.0.dist-info/RECORD
+Filename: imeta-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imeta/__init__.py

```diff
@@ -3,15 +3,15 @@
 from jsonschema.validators import validator_for
 
 from .schema import Schema
 from .serializer import Serializer
 from .exceptions import ValidationError
 
 
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 
 class ImageMetadata:
     def __init__(self, data):
         if not isinstance(data, dict) or "$version" not in data:
             raise ValidationError(
                 "Image metadata must contain a top-level $version key"
```

## Comparing `imeta-0.1.0.dist-info/METADATA` & `imeta-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imeta
-Version: 0.1.0
+Version: 1.0.0
 Summary: Standard for capturing metadata about an image on the web
 Author-email: Matt Wisniewski <imeta@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/imeta
 Keywords: imeta,utility,image,metadata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

