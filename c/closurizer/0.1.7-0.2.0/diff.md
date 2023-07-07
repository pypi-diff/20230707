# Comparing `tmp/closurizer-0.1.7.tar.gz` & `tmp/closurizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closurizer-0.1.7.tar", max compression
+gzip compressed data, was "closurizer-0.2.0.tar", max compression
```

## Comparing `closurizer-0.1.7.tar` & `closurizer-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      641 2022-10-20 18:50:37.436741 closurizer-0.1.7/closurizer/cli.py
--rw-r--r--   0        0        0     3590 2022-10-20 18:50:37.436741 closurizer-0.1.7/closurizer/closurizer.py
--rw-r--r--   0        0        0      463 2022-10-20 18:50:37.436741 closurizer-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 closurizer-0.1.7/setup.py
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      641 2023-07-07 17:47:26.790480 closurizer-0.2.0/closurizer/cli.py
+-rw-r--r--   0        0        0     4384 2023-07-07 17:47:26.790480 closurizer-0.2.0/closurizer/closurizer.py
+-rw-r--r--   0        0        0      463 2023-07-07 17:47:26.790480 closurizer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.2.0/PKG-INFO
```

### Comparing `closurizer-0.1.7/closurizer/cli.py` & `closurizer-0.2.0/closurizer/cli.py`

 * *Files identical despite different names*

### Comparing `closurizer-0.1.7/closurizer/closurizer.py` & `closurizer-0.2.0/closurizer/closurizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,27 +11,43 @@
 
 def _cut_left_join(ltable, rtable, field, attribute):
     return etl.leftjoin(ltable,
                         (etl.cut(rtable, ['id', attribute]).rename(attribute, f"{field}_{attribute}")),
                         lkey=field,
                         rkey="id")
 
+def _length(value):
+    if value is None:
+        return 0
+    else:
+        return len(value.split("|"))
+
+def _length_of_field_values(rec, fields):
+    value = 0
+    for field in fields:
+        if field in rec and (field_value := rec[field]) is not None:
+            value += _length(field_value)
+    return value
 
 def add_closure(kg_archive: str,
                 closure_file: str,
                 output_file: str,
-                fields: List[str] = None
+                fields: List[str] = ['subject', 'object'],
+                evidence_fields: List[str] = ['has_evidence', 'publications', 'primary_knowledge_source', 'provided_by']
                 ):
     print("Generating closure KG...")
     print(f"kg_archive: {kg_archive}")
     print(f"closure_file: {closure_file}")
 
     if fields is None or len(fields) == 0:
         fields = ['subject', 'object']
 
+    if evidence_fields is None or len(evidence_fields) == 0:
+        evidence_fields = ['has_evidence', 'publications', 'primary_knowledge_source', 'provided_by']
+
     print(f"fields: {','.join(fields)}")
     print(f"output_file: {output_file}")
 
     tar = tarfile.open(f"{kg_archive}")
 
     print("Loading node table...")
     node_file_name = [member.name for member in tar.getmembers() if member.name.endswith('_nodes.tsv') ][0]
@@ -75,14 +91,19 @@
         edges = _cut_left_join(edges, nodes, field, "namespace")
         edges = _cut_left_join(edges, nodes, field, "category")
         edges = _cut_left_join(edges, closure_id_table, field, "closure")
         edges = _cut_left_join(edges, closure_label_table, field, "closure_label")
         edges = etl.leftjoin(edges, (etl.cut(nodes, ["id", "name"]).rename("name", f"{field}_label")), lkey=field,
                              rkey="id")
 
+    print("Adding evidence counts...")
+
+    edges = etl.addfield(edges, 'evidence_count',
+                         lambda rec: _length_of_field_values(rec, evidence_fields))
+
     print("Denormalizing...")
     etl.totsv(edges, f"{output_file}")
 
     # Clean up extracted node & edge files
     if os.path.exists(f"{node_file}"):
         os.remove(f"{node_file}")
     if os.path.exists(f"{edge_file}"):
```

### Comparing `closurizer-0.1.7/PKG-INFO` & `closurizer-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: closurizer
-Version: 0.1.7
+Version: 0.2.0
 Summary: Add closure expansion fields to kgx files following the Golr pattern
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

