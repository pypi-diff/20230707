# Comparing `tmp/git_remote_oracle-0.0.3.tar.gz` & `tmp/git-remote-oracle-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_remote_oracle-0.0.3.tar", last modified: Thu Jul  6 16:53:04 2023, max compression
+gzip compressed data, was "git-remote-oracle-0.0.4.tar", last modified: Fri Jul  7 18:00:43 2023, max compression
```

## Comparing `git_remote_oracle-0.0.3.tar` & `git-remote-oracle-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/
--rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git_remote_oracle-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      233 2023-07-02 09:48:14.000000 git_remote_oracle-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      764 2023-07-06 16:41:24.000000 git_remote_oracle-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/src/git_remote_oracle/
--rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git_remote_oracle-0.0.3/src/git_remote_oracle/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7866 2023-07-06 16:39:42.000000 git_remote_oracle-0.0.3/src/git_remote_oracle/git_remote_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:00:43.549493 git-remote-oracle-0.0.4/
+-rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git-remote-oracle-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-07-07 18:00:43.549493 git-remote-oracle-0.0.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1000 2023-07-07 17:13:22.000000 git-remote-oracle-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:00:43.539492 git-remote-oracle-0.0.4/git_remote_oracle/
+-rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git-remote-oracle-0.0.4/git_remote_oracle/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9547 2023-07-07 17:01:03.000000 git-remote-oracle-0.0.4/git_remote_oracle/git_remote_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:00:43.549493 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-07 18:00:43.000000 git-remote-oracle-0.0.4/git_remote_oracle.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      836 2023-07-07 18:00:22.000000 git-remote-oracle-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 18:00:43.549493 git-remote-oracle-0.0.4/setup.cfg
```

### Comparing `git_remote_oracle-0.0.3/LICENSE` & `git-remote-oracle-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `git_remote_oracle-0.0.3/pyproject.toml` & `git-remote-oracle-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
+build-backend = 'setuptools.build_meta'
 
 [project]
-name = "git_remote_oracle"
-version = "0.0.3"
+name = "git-remote-oracle"
+version = "0.0.4"
 authors = [
   { name="CrazyT", email="crazyt2019+gro@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -24,8 +25,9 @@
 git-remote-oracle = "git_remote_oracle:main_cli"
 
 [project.urls]
 "Homepage" = "https://github.com/TheCrazyT/git-remote-oracle"
 "Bug Tracker" = "https://github.com/TheCrazyT/git-remote-oracle/issues"
 
 [tool.setuptools.packages.find]
-exclude = ["*.ipynb"]
+exclude = ["*.ipynb"]
+include = ["git_remote_oracle"]
```

### Comparing `git_remote_oracle-0.0.3/src/git_remote_oracle/git_remote_oracle.py` & `git-remote-oracle-0.0.4/git_remote_oracle/git_remote_oracle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+# documentation links:
+#  https://git-scm.com/docs/gitremote-helpers
+#  https://git-scm.com/docs/git-fast-import
+
 import time
 import oracledb
 import pexpect
 import os
 import sys
 from configparser import ConfigParser
 from datetime import datetime
 
 DEBUG = ("1" == os.getenv("GR_ORACLE_DEBUG"))
 DEBUG_GIT_OUTPUT = ("1" == os.getenv("GR_ORACLE_DEBUG_GIT"))
 CONNECT_AS_SYSDBA = ("1" == os.getenv("GR_ORACLE_SYSDBA"))
 DATETIME_FORMAT = "%d.%m.%Y %H:%M:%S"
+PROGRESS = True
+BATCH_SIZE = 20 if (os.getenv("GR_ORACLE_BATCHSIZE") is None) else int(os.getenv("GR_ORACLE_BATCHSIZE"))
 
 def print_fl(*args, **kwargs):
   print(*args, **kwargs, flush=True)
   if DEBUG_GIT_OUTPUT and ('file' not in kwargs):
     print_to_err(*args, **kwargs)
 
 def print_to_err(*args, **kwargs):
@@ -86,19 +92,46 @@
 def cmd_list():
   dbg("in func: cmd_list")
   print_fl(":object-format sha1")
   print_fl("? refs/heads/main")
   print_fl("@refs/heads/main HEAD")
   print_fl("")
 
+def cmd_option_verbosity(params):
+  global DEBUG, DEBUG_GIT_OUTPUT
+  param_val = int(params)
+  if param_val > 0:
+    DEBUG = True
+  if param_val > 1:
+    DEBUG_GIT_OUTPUT = True
+
+def cmd_option_progress(params):
+  global PROGRESS
+  if params == "true":
+    PROGRESS = True
+  else:
+    PROGRESS = False
+
+def cmd_option(params):
+  dbg("in func: cmd_option")
+  if(params.startswith("verbosity")):
+    params = int(params[len("verbosity "):])
+    cmd_option_verbosity(params)
+  elif(params.startswith("progress ")):
+    params = int(params[len("progress  "):])
+    cmd_option_progress(params)
+  else:
+    print_fl("unsupported")
+
 def cmd_capabilities():
   dbg("in func: cmd_capabilities")
   print_fl("import")
   print_fl("export")
   print_fl("refspec refs/heads/*:refs/heads/*")
+  print_fl("option")
   print_fl("")
 
 def commit_block(curr_time, formatted_datetime, last_ddl):
   print_fl("commit refs/heads/main")
   print_fl(f"committer <notexisting@notexisting.com> {curr_time} +0000")
   if last_ddl is None:
     msg = f"> {formatted_datetime}"
@@ -114,14 +147,45 @@
     print_fl(f"from {id}")
 
 def print_file_list(file_list):
   for fl in file_list:
     print_fl(f"M 100644 :{fl['id']} {fl['name']}")
   print_fl("")
 
+def build_query(columns):
+  return """
+    SELECT 
+      """ + columns + """
+    FROM all_objects
+    WHERE 
+      lower(owner) = lower(:1)
+      AND object_type IN (
+        'PACKAGE',
+        'PACKAGE BODY',
+        'TRIGGER',
+        'VIEW',
+        'TABLE',
+        'PROCEDURE',
+        'FUNCTION',
+        'INDEX',
+        'TYPE',
+        'TYPE BODY',
+        'SYNONYM',
+        'JOB',
+        'JAVA SOURCE',
+        'JAVA RESOURCE'
+      )
+      AND sharing <> 'METADATA LINK'
+      AND last_ddl_time > :3
+      AND generated = 'N'
+      AND temporary = 'N'
+      AND oracle_maintained = 'N'
+    ORDER BY object_id
+    """
+
 def cmd_import_MAIN(protocol, host, service_name, schema, port, username, password):
   global DATETIME_FORMAT
   dbg("in func: cmd_import")
   l = sys.stdin.readline()
   while l.startswith("import"):
     dbg("  %s" % l)
     l = sys.stdin.readline()
@@ -147,64 +211,60 @@
   dbg(f"last_ddl_path: {last_ddl_path}")
   if os.path.isfile(last_ddl_path):
     with open(last_ddl_path, 'r') as f:
       last_ddl = f.read()
       last_ddl_time = datetime.strptime(last_ddl, DATETIME_FORMAT)
   dbg(f"last_ddl_time: {last_ddl_time}")
   file_list = []
-  qry = """
-    SELECT 
+  if PROGRESS:
+    print_fl(f"progress 1/?")
+  qry_columns = """
       object_id,
       object_name,
       owner,
       object_type,
       DBMS_METADATA.GET_DDL(REPLACE(DECODE(
 							object_type,
 							'PACKAGE','PACKAGE SPEC',
 							'TYPE','TYPE SPEC',
 							'JOB','PROCOBJ',
 							object_type 
 						),' ','_'), object_name, UPPER(:2)) AS DDL
-    FROM all_objects
-    WHERE 
-      lower(owner) = lower(:1)
-      AND object_type IN (
-        'PACKAGE',
-        'PACKAGE BODY',
-        'TRIGGER',
-        'VIEW',
-        'TABLE',
-        'PROCEDURE',
-        'FUNCTION',
-        'INDEX',
-        'TYPE',
-        'TYPE BODY',
-        'SYNONYM',
-        'JOB',
-        'JAVA SOURCE',
-        'JAVA RESOURCE'
-      )
-      AND sharing <> 'METADATA LINK'
-      AND last_ddl_time > :3
-      AND generated = 'N'
-      AND temporary = 'N'
-      AND oracle_maintained = 'N'
-    ORDER BY object_id
-    """
+  """
+  qry_cnt = build_query("COUNT(*) AS cnt,:2 AS ignore")
+  res = cursor.execute(qry_cnt, [schema, schema, last_ddl_time])
+  if PROGRESS:
+    print_fl(f"progress 2/?")
+  
+  qry = build_query(qry_columns)
   dbg(f"qry: {qry}")
-  for object_id, object_name, owner, object_type, ddl in cursor.execute(qry, [schema, schema, last_ddl_time]):
-    #print(object_name)
-    #print(ddl)
-    ddl_str = ddl.read()
-    dbg(f"object_name: {object_name}")
-    print_fl(f"blob")
-    print_fl(f"mark :{object_id}")
-    print_fl(f"data {len(ddl_str)}")
-    print_fl(ddl_str)
-    file_list.append({"id":f"{object_id}", "name":f"{object_type}/{object_name}.sql"})
+  total = res.fetchone()[0]
+
+  for i in range(0,total-1,BATCH_SIZE):
+    qry_offset = f"""
+     OFFSET {i} ROWS FETCH NEXT {BATCH_SIZE} ROWS ONLY
+    """
+    row = cursor.execute(qry+qry_offset, [schema, schema, last_ddl_time])
+    while True:
+      row = cursor.fetchone()
+      if row is None:
+          break
+      object_id, object_name, owner, object_type, ddl = row
+      i += 1
+      #print(object_name)
+      #print(ddl)
+      ddl_str = ddl.read()
+      dbg(f"object_name: {object_name}")
+      print_fl(f"blob")
+      print_fl(f"mark :{object_id}")
+      print_fl(f"data {len(ddl_str)}")
+      print_fl(ddl_str)
+      file_list.append({"id":f"{object_id}", "name":f"{object_type}/{object_name}.sql"})
+      if PROGRESS:
+        print_fl(f"progress {i+2}/{total+2}")
   
   utcnow = datetime.utcnow()
   formatted_datetime = utcnow.strftime(DATETIME_FORMAT)
   curr_time = round(time.time())
   
   str = f"{formatted_datetime}"
   print_fl(f"blob")
@@ -257,14 +317,17 @@
         cmd = cmd.strip()
         if len(cmd) > 0:
           dbg(f"cmd: {cmd}")
           if(cmd == "capabilities"):
             cmd_capabilities()
           elif(cmd == "list"):
             cmd_list()
+          elif(cmd.startswith("option")):
+            params = cmd[len("option "):]
+            cmd_option(params)
           elif(cmd == "import refs/heads/main"):
             cmd_import_MAIN(protocol=protocol,
             host=host,
             service_name=service,
             schema=schema,
             port=port,
             username=username,
```

