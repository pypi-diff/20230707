# Comparing `tmp/gs_engine-0.23.0a20230705-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.23.0a20230706-py2.py3-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11922 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-05 19:07 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      840 b- defN 23-Jul-05 21:16 gs_engine-0.23.0a20230705.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-Jul-05 21:00 gs_engine-0.23.0a20230705.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-05 21:00 gs_engine-0.23.0a20230705.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21680 b- defN 23-Jul-05 21:00 gs_engine-0.23.0a20230705.dist-info/METADATA
--rw-r--r--  2.0 unx     1573 b- defN 23-Jul-05 19:07 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-05 19:07 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      503 b- defN 23-Jul-05 19:07 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-05 19:07 graphscope.runtime/conf/log4rs.yml
-9 files, 26051 bytes uncompressed, 10460 bytes compressed:  59.8%
+Zip file size: 11941 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      840 b- defN 23-Jul-06 21:25 gs_engine-0.23.0a20230706.dist-info/RECORD
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-06 21:07 gs_engine-0.23.0a20230706.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-06 21:07 gs_engine-0.23.0a20230706.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jul-06 21:07 gs_engine-0.23.0a20230706.dist-info/METADATA
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-06 19:07 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-06 19:07 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-06 19:07 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-06 19:07 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-06 19:07 graphscope.runtime/conf/log4rs.yml
+9 files, 26097 bytes uncompressed, 10479 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: graphscope_runtime/__init__.py
+Filename: gs_engine-0.23.0a20230706.dist-info/RECORD
 Comment: 
 
-Filename: gs_engine-0.23.0a20230705.dist-info/RECORD
+Filename: gs_engine-0.23.0a20230706.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.23.0a20230705.dist-info/WHEEL
+Filename: gs_engine-0.23.0a20230706.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.23.0a20230705.dist-info/top_level.txt
+Filename: gs_engine-0.23.0a20230706.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.23.0a20230705.dist-info/METADATA
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
 Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
 Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment:
```

## graphscope.runtime/conf/frontend.vineyard.properties

```diff
@@ -10,12 +10,13 @@
 # e.g. 1.2.3.4:1234,1.2.3.5:1234
 pegasus.hosts = PEGASUS_HOSTS
 
 # graph schema path
 graph.schema = GRAPH_SCHEMA
 
 ## Frontend Config
-gremlin.server.port = FRONTEND_SERVICE_PORT
+gremlin.server.port = FRONTEND_GREMLIN_PORT
 
+neo4j.bolt.server.port = FRONTEND_CYPHER_PORT
 # disable the authentication if username or password is not set
 #auth.username = default
 #auth.password = default
```

## Comparing `gs_engine-0.23.0a20230705.dist-info/METADATA` & `gs_engine-0.23.0a20230706.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.23.0a20230705
+Version: 0.23.0a20230706
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

