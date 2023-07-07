# Comparing `tmp/imeta-1.0.0-py3-none-any.whl.zip` & `tmp/imeta-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4119 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1756 b- defN 23-Jul-07 03:25 imeta/__init__.py
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 03:25 imeta/exceptions.py
--rw-r--r--  2.0 unx      849 b- defN 23-Jul-07 03:25 imeta/schema.py
--rw-r--r--  2.0 unx      891 b- defN 23-Jul-07 03:25 imeta/serializer.py
--rw-r--r--  2.0 unx     1881 b- defN 23-Jul-07 03:25 imeta/schema/1.0.json
--rw-r--r--  2.0 unx      924 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      661 b- defN 23-Jul-07 03:25 imeta-1.0.0.dist-info/RECORD
-9 files, 7212 bytes uncompressed, 2991 bytes compressed:  58.5%
+Zip file size: 4196 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     2125 b- defN 23-Jul-07 19:16 imeta/__init__.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 19:16 imeta/exceptions.py
+-rw-r--r--  2.0 unx      849 b- defN 23-Jul-07 19:16 imeta/schema.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Jul-07 19:16 imeta/serializer.py
+-rw-r--r--  2.0 unx     1881 b- defN 23-Jul-07 19:16 imeta/schema/1.0.json
+-rw-r--r--  2.0 unx      931 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      661 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/RECORD
+9 files, 7588 bytes uncompressed, 3068 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: imeta/serializer.py
 Comment: 
 
 Filename: imeta/schema/1.0.json
 Comment: 
 
-Filename: imeta-1.0.0.dist-info/METADATA
+Filename: imeta-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: imeta-1.0.0.dist-info/WHEEL
+Filename: imeta-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: imeta-1.0.0.dist-info/top_level.txt
+Filename: imeta-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: imeta-1.0.0.dist-info/RECORD
+Filename: imeta-1.1.0.dist-info/RECORD
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
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 class ImageMetadata:
     def __init__(self, data):
         if not isinstance(data, dict) or "$version" not in data:
             raise ValidationError(
                 "Image metadata must contain a top-level $version key"
@@ -36,14 +36,24 @@
         return cls(data)
 
     @classmethod
     def from_file(cls, filename):
         data_str = Path(filename).read_text()
         return cls.from_str(data_str)
 
+    @classmethod
+    def for_image(cls, filename):
+        filepath = Path(filename)
+        metapath = filepath.parents[0] / f"{filepath.stem}.json"
+        return str(metapath)
+
+    @classmethod
+    def from_image(cls, filename):
+        return cls.from_file(cls.for_image(filename))
+
     def __iter__(self):
         data = self._serializer.serialize(self)
         data["$version"] = self._serializer._VERSION
         data.move_to_end("$version", last=False)
         for key in self._raw_data.keys():
             if key not in data:
                 data[key] = self._raw_data[key]
@@ -52,7 +62,10 @@
     def __repr__(self):
         data_str = json.dumps(dict(self))
         return data_str
 
     def to_file(self, filename):
         data_str = str(self)
         Path(filename).write_text(data_str)
+
+    def to_image(self, filename):
+        self.to_file(self.for_image(filename))
```

## Comparing `imeta-1.0.0.dist-info/METADATA` & `imeta-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: imeta
-Version: 1.0.0
+Version: 1.1.0
 Summary: Standard for capturing metadata about an image on the web
-Author-email: Matt Wisniewski <imeta@mattw.life>
+Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/imeta
 Keywords: imeta,utility,image,metadata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

## Comparing `imeta-1.0.0.dist-info/RECORD` & `imeta-1.1.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-imeta/__init__.py,sha256=qjayDvgJ0RUhqKkPArauX7i3PBlcDSbvv4Ju10GoWBY,1756
+imeta/__init__.py,sha256=B95mY22kW_9lRn5hE4BHxrRiay3GmKjlBY3Z9rfxTcQ,2125
 imeta/exceptions.py,sha256=LsmGqVLqWROo3n_s3y7ktJJvra2SoCYuHIOpsakW5aw,152
 imeta/schema.py,sha256=MQa2yHJoo7mHw77DlQR_G-H2dLGMizkrADT4SUbes8o,849
 imeta/serializer.py,sha256=AjIfx7nCKIDiDbwsjhukH6GLTJcQ60hNkwZcZmDlmPU,891
 imeta/schema/1.0.json,sha256=h199lN1CXr8fDq1n8s_mpmv_kjWBcCKVDKrTVrVIshg,1881
-imeta-1.0.0.dist-info/METADATA,sha256=gP5MOsGgRSriZ5ZyWnBwNlnMSoMLWyMzrJp7F5IeP4A,924
-imeta-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-imeta-1.0.0.dist-info/top_level.txt,sha256=FBV8zF4u9Jdo2epLMcKy2JDK2csjrdQLIAGvi3alf9Y,6
-imeta-1.0.0.dist-info/RECORD,,
+imeta-1.1.0.dist-info/METADATA,sha256=9KshWfpUyX02ab2kN-zA7Qd7kRHPeIvfL25JSyxxugU,931
+imeta-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+imeta-1.1.0.dist-info/top_level.txt,sha256=FBV8zF4u9Jdo2epLMcKy2JDK2csjrdQLIAGvi3alf9Y,6
+imeta-1.1.0.dist-info/RECORD,,
```

