# Comparing `tmp/dbsa-0.0.8.tar.gz` & `tmp/dbsa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbsa-0.0.8.tar", last modified: Sun Jul 28 07:52:31 2019, max compression
+gzip compressed data, was "dist/dbsa-0.0.9.tar", last modified: Mon Jul 29 15:36:42 2019, max compression
```

## Comparing `dbsa-0.0.8.tar` & `dbsa-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-28 07:52:31.000000 dbsa-0.0.8/
--rw-r--r--   0 bfaludi    (501) staff       (20)      234 2019-07-28 07:52:31.000000 dbsa-0.0.8/PKG-INFO
-drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/
--rw-r--r--   0 bfaludi    (501) staff       (20)      234 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/PKG-INFO
--rw-r--r--   0 bfaludi    (501) staff       (20)        1 2019-06-21 09:01:52.000000 dbsa-0.0.8/dbsa.egg-info/not-zip-safe
--rw-r--r--   0 bfaludi    (501) staff       (20)      304 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/SOURCES.txt
--rw-r--r--   0 bfaludi    (501) staff       (20)       54 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/entry_points.txt
--rw-r--r--   0 bfaludi    (501) staff       (20)        7 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/requires.txt
--rw-r--r--   0 bfaludi    (501) staff       (20)        5 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/top_level.txt
--rw-r--r--   0 bfaludi    (501) staff       (20)        1 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa.egg-info/dependency_links.txt
--rw-r--r--   0 bfaludi    (501) staff       (20)       36 2019-06-20 08:22:02.000000 dbsa-0.0.8/README.md
--rw-r--r--   0 bfaludi    (501) staff       (20)      578 2019-07-28 07:51:58.000000 dbsa-0.0.8/setup.py
--rw-r--r--   0 bfaludi    (501) staff       (20)       79 2019-07-28 07:52:31.000000 dbsa-0.0.8/setup.cfg
-drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-28 07:52:31.000000 dbsa-0.0.8/dbsa/
--rw-r--r--   0 bfaludi    (501) staff       (20)     8748 2019-07-26 05:04:56.000000 dbsa-0.0.8/dbsa/redshift.py
--rw-r--r--   0 bfaludi    (501) staff       (20)    15978 2019-07-26 04:54:30.000000 dbsa-0.0.8/dbsa/__init__.py
--rw-r--r--   0 bfaludi    (501) staff       (20)     7768 2019-07-28 07:50:08.000000 dbsa-0.0.8/dbsa/hive.py
--rw-r--r--   0 bfaludi    (501) staff       (20)     1210 2019-07-26 05:20:38.000000 dbsa-0.0.8/dbsa/markdown.py
--rw-r--r--   0 bfaludi    (501) staff       (20)     6001 2019-07-28 07:51:53.000000 dbsa-0.0.8/dbsa/presto.py
+drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-29 15:36:42.000000 dbsa-0.0.9/
+-rw-r--r--   0 bfaludi    (501) staff       (20)      234 2019-07-29 15:36:42.000000 dbsa-0.0.9/PKG-INFO
+drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/
+-rw-r--r--   0 bfaludi    (501) staff       (20)      234 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/PKG-INFO
+-rw-r--r--   0 bfaludi    (501) staff       (20)        1 2019-06-21 09:01:52.000000 dbsa-0.0.9/dbsa.egg-info/not-zip-safe
+-rw-r--r--   0 bfaludi    (501) staff       (20)      304 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/SOURCES.txt
+-rw-r--r--   0 bfaludi    (501) staff       (20)       54 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/entry_points.txt
+-rw-r--r--   0 bfaludi    (501) staff       (20)        7 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/requires.txt
+-rw-r--r--   0 bfaludi    (501) staff       (20)        5 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/top_level.txt
+-rw-r--r--   0 bfaludi    (501) staff       (20)        1 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa.egg-info/dependency_links.txt
+-rw-r--r--   0 bfaludi    (501) staff       (20)     2324 2019-07-28 09:20:05.000000 dbsa-0.0.9/README.md
+-rw-r--r--   0 bfaludi    (501) staff       (20)      578 2019-07-29 15:34:20.000000 dbsa-0.0.9/setup.py
+-rw-r--r--   0 bfaludi    (501) staff       (20)       79 2019-07-29 15:36:42.000000 dbsa-0.0.9/setup.cfg
+drwxr-xr-x   0 bfaludi    (501) staff       (20)        0 2019-07-29 15:36:42.000000 dbsa-0.0.9/dbsa/
+-rw-r--r--   0 bfaludi    (501) staff       (20)     8748 2019-07-26 05:04:56.000000 dbsa-0.0.9/dbsa/redshift.py
+-rw-r--r--   0 bfaludi    (501) staff       (20)    15978 2019-07-29 15:35:05.000000 dbsa-0.0.9/dbsa/__init__.py
+-rw-r--r--   0 bfaludi    (501) staff       (20)     7884 2019-07-29 15:34:13.000000 dbsa-0.0.9/dbsa/hive.py
+-rw-r--r--   0 bfaludi    (501) staff       (20)     1210 2019-07-26 05:20:38.000000 dbsa-0.0.9/dbsa/markdown.py
+-rw-r--r--   0 bfaludi    (501) staff       (20)     6001 2019-07-28 07:51:53.000000 dbsa-0.0.9/dbsa/presto.py
```

### Comparing `dbsa-0.0.8/setup.py` & `dbsa-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-version = '0.0.8'
+version = '0.0.9'
 
 setup(
     name='dbsa',
     version=version,
     description="Database schema definitions",
     packages=find_packages(exclude=['ez_setup']),
     include_package_data=True,
```

### Comparing `dbsa-0.0.8/dbsa/redshift.py` & `dbsa-0.0.9/dbsa/redshift.py`

 * *Files identical despite different names*

### Comparing `dbsa-0.0.8/dbsa/__init__.py` & `dbsa-0.0.9/dbsa/__init__.py`

 * *Files identical despite different names*

### Comparing `dbsa-0.0.8/dbsa/hive.py` & `dbsa-0.0.9/dbsa/hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Date,
     Timestamp,
     Array,
     Map,
     Row,
     IPAddress,
     Format,
+    Bucket,
     Dialect as BaseDialect,
 )
 from jinja2 import Template
 import inspect
 
 class Table(BaseDialect):
     _column_types = {
@@ -45,36 +46,38 @@
         IPAddress: 'STRING',
     }
     _req_properties = {
         Decimal: {'precision', 'scale'},
         Char: {'length'},
         Varbinary: {'length'},
         Format: {'format'},
+        Bucket: {'by', 'count'},
     }
     _property_types = {
         Format: 'STORED AS {{ format }}',
+        Bucket: 'CLUSTERED BY ({{ by }}) INTO {{ count }} BUCKETS',
     }
     _how_to_quote_table = '`{}`'
     _how_to_quote_column = '`{}`'
     _column_setter = '{} {}'
 
     def get_create_table(self, filter_fn=None, external_table=False, hdfs_path=None, tblformat=None, tblproperties=None):
         return Template("""
             CREATE {% if external_table %}EXTERNAL {% endif %}TABLE IF NOT EXISTS {{ t.full_table_name(quoted=True, with_prefix=True) }} (
               {%- for column in t.columns(filter_fn=filter_fn, include_partitions=False) %}
-              {{ column.quoted_name }} {{ column.column_type}}{% if column.comment %} COMMENT '{{ column.comment|replace("'", "\'") }}'{% endif %}{% if not loop.last %},{% endif %}
+              {{ column.quoted_name }} {{ column.column_type}}{% if column.comment %} COMMENT '{{ column.comment|replace("'", "\\'") }}'{% endif %}{% if not loop.last %},{% endif %}
               {%- endfor %}
             )
             {%- if inspect.getdoc(t) %}
-            COMMENT '{{ inspect.getdoc(t)|replace("'", "\'")|trim }}'
+            COMMENT '{{ inspect.getdoc(t)|replace("'", "\\'")|trim }}'
             {%- endif %}
             {%- if t.partitions %}
             PARTITIONED BY (
               {%- for partition in t.partitions %}
-              {{ partition.quoted_name }} {{ partition.column_type }}{% if partition.comment %} COMMENT '{{ partition.comment|replace("'", "\'") }}'{% endif %}{% if not loop.last %},{% endif %}
+              {{ partition.quoted_name }} {{ partition.column_type }}{% if partition.comment %} COMMENT '{{ partition.comment|replace("'", "\\'") }}'{% endif %}{% if not loop.last %},{% endif %}
               {%- endfor %}
             )
             {%- endif %}
             {%- if tblformat %}
             {{ tblformat }}
             {%- endif %}
             {%- for property in t.properties %}
```

### Comparing `dbsa-0.0.8/dbsa/markdown.py` & `dbsa-0.0.9/dbsa/markdown.py`

 * *Files identical despite different names*

### Comparing `dbsa-0.0.8/dbsa/presto.py` & `dbsa-0.0.9/dbsa/presto.py`

 * *Files identical despite different names*

