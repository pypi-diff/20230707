# Comparing `tmp/tap_messagebird-0.0.8.tar.gz` & `tmp/tap_messagebird-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_messagebird-0.0.8.tar", max compression
+gzip compressed data, was "tap_messagebird-0.0.9.tar", max compression
```

## Comparing `tap_messagebird-0.0.8.tar` & `tap_messagebird-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-05-03 19:46:52.737018 tap_messagebird-0.0.8/LICENSE
--rw-r--r--   0        0        0     3380 2023-05-03 19:46:52.737018 tap_messagebird-0.0.8/README.md
--rw-r--r--   0        0        0     1225 2023-05-03 19:47:10.681314 tap_messagebird-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      117 2023-05-03 19:47:10.685314 tap_messagebird-0.0.8/tap_messagebird/__init__.py
--rw-r--r--   0        0        0     3857 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/client.py
--rw-r--r--   0        0        0     3329 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/conversation.json
--rw-r--r--   0        0        0      993 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/conversation_message.json
--rw-r--r--   0        0        0     4240 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/schemas/message.json
--rw-r--r--   0        0        0     6789 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/streams.py
--rw-r--r--   0        0        0     1590 2023-05-03 19:46:52.741018 tap_messagebird-0.0.8/tap_messagebird/tap.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 tap_messagebird-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-05 16:02:26.786563 tap_messagebird-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3380 2023-06-05 16:02:26.786563 tap_messagebird-0.0.9/README.md
+-rw-r--r--   0        0        0     1225 2023-06-05 16:02:44.602956 tap_messagebird-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-06-05 16:02:44.606956 tap_messagebird-0.0.9/tap_messagebird/__init__.py
+-rw-r--r--   0        0        0     3857 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/client.py
+-rw-r--r--   0        0        0     3329 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/schemas/conversation.json
+-rw-r--r--   0        0        0      993 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/schemas/conversation_message.json
+-rw-r--r--   0        0        0     4240 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/schemas/message.json
+-rw-r--r--   0        0        0     6789 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/streams.py
+-rw-r--r--   0        0        0     1590 2023-06-05 16:02:26.790563 tap_messagebird-0.0.9/tap_messagebird/tap.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 tap_messagebird-0.0.9/PKG-INFO
```

### Comparing `tap_messagebird-0.0.8/LICENSE` & `tap_messagebird-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/README.md` & `tap_messagebird-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Messagebird tap class.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
 ## Capabilities
 
 * `catalog`
-# `state`
+* `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
```

### Comparing `tap_messagebird-0.0.8/pyproject.toml` & `tap_messagebird-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "tap-messagebird"
-version = "0.0.8"
+version = "0.0.9"
 description = "`tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Meltano Team <hello@meltano.com>"]
 keywords = [
     "ELT",
     "Messagebird",
 ]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "<3.11,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = { version=">=0.24,<0.27"}
+singer-sdk = { version=">=0.24,<0.29"}
 fs-s3fs = { version = "^1.1.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 responses = "0.23.1"
 
 [tool.poetry.extras]
```

### Comparing `tap_messagebird-0.0.8/tap_messagebird/client.py` & `tap_messagebird-0.0.9/tap_messagebird/client.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/tap_messagebird/schemas/conversation.json` & `tap_messagebird-0.0.9/tap_messagebird/schemas/conversation.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/tap_messagebird/schemas/conversation_message.json` & `tap_messagebird-0.0.9/tap_messagebird/schemas/conversation_message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/tap_messagebird/schemas/message.json` & `tap_messagebird-0.0.9/tap_messagebird/schemas/message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/tap_messagebird/streams.py` & `tap_messagebird-0.0.9/tap_messagebird/streams.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/tap_messagebird/tap.py` & `tap_messagebird-0.0.9/tap_messagebird/tap.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.8/PKG-INFO` & `tap_messagebird-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: tap-messagebird
-Version: 0.0.8
+Version: 0.0.9
 Summary: `tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Messagebird
 Author: Meltano Team
 Author-email: hello@meltano.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: s3
 Requires-Dist: fs-s3fs (>=1.1.1,<2.0.0) ; extra == "s3"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: singer-sdk (>=0.24,<0.27)
+Requires-Dist: singer-sdk (>=0.24,<0.29)
 Description-Content-Type: text/markdown
 
 # `tap-messagebird`
 
 Messagebird tap class.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
 ## Capabilities
 
 * `catalog`
-# `state`
+* `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
```

