# Comparing `tmp/tap_betterstack-0.0.1a1.tar.gz` & `tmp/tap_betterstack-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_betterstack-0.0.1a1.tar", max compression
+gzip compressed data, was "tap_betterstack-0.0.1a2.tar", max compression
```

## Comparing `tap_betterstack-0.0.1a1.tar` & `tap_betterstack-0.0.1a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11355 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     5162 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/README.md
--rw-r--r--   0        0        0     2259 2023-06-22 23:51:58.032940 tap_betterstack-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/__init__.py
--rw-r--r--   0        0        0      128 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/__main__.py
--rw-r--r--   0        0        0     2807 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/client.py
--rw-r--r--   0        0        0       28 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/streams/__init__.py
--rw-r--r--   0        0        0    17940 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/streams/uptime.py
--rw-r--r--   0        0        0     1372 2023-06-22 23:51:41.068722 tap_betterstack-0.0.1a1/tap_betterstack/tap.py
--rw-r--r--   0        0        0     6101 1970-01-01 00:00:00.000000 tap_betterstack-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     5162 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/README.md
+-rw-r--r--   0        0        0     2259 2023-07-07 17:35:16.554053 tap_betterstack-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/__main__.py
+-rw-r--r--   0        0        0     2807 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/client.py
+-rw-r--r--   0        0        0       28 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/streams/__init__.py
+-rw-r--r--   0        0        0    17940 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/streams/uptime.py
+-rw-r--r--   0        0        0     1372 2023-07-07 17:34:59.693933 tap_betterstack-0.0.1a2/tap_betterstack/tap.py
+-rw-r--r--   0        0        0     6101 1970-01-01 00:00:00.000000 tap_betterstack-0.0.1a2/PKG-INFO
```

### Comparing `tap_betterstack-0.0.1a1/LICENSE` & `tap_betterstack-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.0.1a1/README.md` & `tap_betterstack-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.0.1a1/pyproject.toml` & `tap_betterstack-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-betterstack"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "`tap-betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Better Stack",
 ]
@@ -19,15 +19,15 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-betterstack"
 repository = "https://github.com/edgarrmondragon/tap-betterstack"
 documentation = "https://github.com/edgarrmondragon/tap-betterstack#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.28.0"
+singer-sdk = "0.29.0"
 
 [tool.poetry.group.dev.dependencies]
 singer-sdk = {version = "*", extras = ["testing"]}
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-betterstack" = "tap_betterstack.tap:TapBetterStack.cli"
```

### Comparing `tap_betterstack-0.0.1a1/tap_betterstack/client.py` & `tap_betterstack-0.0.1a2/tap_betterstack/client.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.0.1a1/tap_betterstack/streams/uptime.py` & `tap_betterstack-0.0.1a2/tap_betterstack/streams/uptime.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.0.1a1/tap_betterstack/tap.py` & `tap_betterstack-0.0.1a2/tap_betterstack/tap.py`

 * *Files identical despite different names*

### Comparing `tap_betterstack-0.0.1a1/PKG-INFO` & `tap_betterstack-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-betterstack
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: `tap-betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-betterstack
 License: Apache-2.0
 Keywords: ELT,singer.io,Better Stack
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.28.0)
+Requires-Dist: singer-sdk (==0.29.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-betterstack#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-betterstack
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-betterstack
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: tap-betterstack Version: 0.0.1a1 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-betterstack Version: 0.0.1a2 Summary: `tap-
 betterstack` is a Singer tap for Better Stack, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-betterstack
 License: Apache-2.0 Keywords: ELT,singer.io,Better Stack Author: Edgar
 RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com Requires-Python:
 >=3.7.1,<3.12 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: singer-sdk (==0.28.0) Project-URL:
+Language :: Python :: 3.11 Requires-Dist: singer-sdk (==0.29.0) Project-URL:
 Documentation, https://github.com/edgarrmondragon/tap-betterstack#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-betterstack
 Description-Content-Type: text/markdown
                                # tap-betterstack
                     [pre-commit.ci_status] [License] [Ruff]
 Singer tap for [Better Stack](https://betterstack.com). Built with the [Meltano
                     Singer SDK](https://sdk.meltano.com).
```

