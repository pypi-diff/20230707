# Comparing `tmp/opentelemetry_instrument_openai-0.5.0.tar.gz` & `tmp/opentelemetry_instrument_openai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrument_openai-0.5.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrument_openai-0.6.0.tar", max compression
```

## Comparing `opentelemetry_instrument_openai-0.5.0.tar` & `opentelemetry_instrument_openai-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-06-13 22:46:01.950351 opentelemetry_instrument_openai-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     1360 2023-06-13 22:46:01.950351 opentelemetry_instrument_openai-0.5.0/README.md
--rw-r--r--   0        0        0      875 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    24295 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      611 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/package.py
--rw-r--r--   0        0        0      596 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-07 14:11:58.756375 opentelemetry_instrument_openai-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     1360 2023-07-07 14:11:58.756375 opentelemetry_instrument_openai-0.6.0/README.md
+-rw-r--r--   0        0        0      875 2023-07-07 14:11:58.764376 opentelemetry_instrument_openai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12352 2023-07-07 14:11:58.764376 opentelemetry_instrument_openai-0.6.0/src/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-07 14:11:58.764376 opentelemetry_instrument_openai-0.6.0/src/opentelemetry/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      596 2023-07-07 14:11:58.764376 opentelemetry_instrument_openai-0.6.0/src/opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.6.0/PKG-INFO
```

### Comparing `opentelemetry_instrument_openai-0.5.0/LICENSE.md` & `opentelemetry_instrument_openai-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.5.0/README.md` & `opentelemetry_instrument_openai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.5.0/pyproject.toml` & `opentelemetry_instrument_openai-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentelemetry-instrument-openai"
-version = "0.5.0"
+version = "0.6.0"
 description = "OpenTelemetry openai instrumentation"
 license = "Apache-2.0"
 authors = ["cartermp <pcarter@fastmail.com>"]
 maintainers = ["cartermp <pcarter@fastmail.com>"]
 readme = "README.md"
 packages = [{include = "opentelemetry", from = "src" }]
```

### Comparing `opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/package.py` & `opentelemetry_instrument_openai-0.6.0/src/opentelemetry/instrumentation/openai/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/version.py` & `opentelemetry_instrument_openai-0.6.0/src/opentelemetry/instrumentation/openai/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `opentelemetry_instrument_openai-0.5.0/PKG-INFO` & `opentelemetry_instrument_openai-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrument-openai
-Version: 0.5.0
+Version: 0.6.0
 Summary: OpenTelemetry openai instrumentation
 License: Apache-2.0
 Author: cartermp
 Author-email: pcarter@fastmail.com
 Maintainer: cartermp
 Maintainer-email: pcarter@fastmail.com
 Requires-Python: >=3.7.1,<4.0
```

