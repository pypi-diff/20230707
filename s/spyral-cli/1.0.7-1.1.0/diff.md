# Comparing `tmp/spyral_cli-1.0.7.tar.gz` & `tmp/spyral_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.7.tar", max compression
+gzip compressed data, was "spyral_cli-1.1.0.tar", max compression
```

## Comparing `spyral_cli-1.0.7.tar` & `spyral_cli-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-06 13:33:29.779202 spyral_cli-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.7/src/spyral/__init__.py
--rw-r--r--   0        0        0     7083 2023-07-06 08:53:53.525992 spyral_cli-1.0.7/src/spyral/cli.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 spyral_cli-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-07 10:36:11.542344 spyral_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.1.0/src/spyral/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-07 10:35:10.675160 spyral_cli-1.1.0/src/spyral/cli.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 spyral_cli-1.1.0/PKG-INFO
```

### Comparing `spyral_cli-1.0.7/pyproject.toml` & `spyral_cli-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.7"
+version = "1.1.0"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.0.7/src/spyral/cli.py` & `spyral_cli-1.1.0/src/spyral/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,8 +225,10 @@
                         label = m.group(1).strip()
                         break
             assert cmd or label
             if label is None:
                 label = cmd
 
             df = pd.read_csv(i, comment="#")
-            writer.writerow(extra_columns + [label, df.rss.max(), df.vms.max()])
+            writer.writerow(
+                extra_columns + [label, df.time.iloc[-1], df.rss.max(), df.vms.max()]
+            )
```

### Comparing `spyral_cli-1.0.7/PKG-INFO` & `spyral_cli-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.7
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

