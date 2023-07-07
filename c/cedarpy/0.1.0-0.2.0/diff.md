# Comparing `tmp/cedarpy-0.1.0.tar.gz` & `tmp/cedarpy-0.2.0.tar.gz`

## Comparing `cedarpy-0.1.0.tar` & `cedarpy-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 cedarpy-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     4079 2023-07-06 23:04:46.000000 cedarpy-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      703 2023-07-06 23:04:46.000000 cedarpy-0.1.0/.gitignore
--rw-r--r--   0     1001      123       95 2023-07-06 23:04:46.000000 cedarpy-0.1.0/.gitmodules
--rw-r--r--   0     1001      123    11358 2023-07-06 23:04:46.000000 cedarpy-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1024 2023-07-06 23:04:46.000000 cedarpy-0.1.0/Makefile
--rw-r--r--   0     1001      123     6167 2023-07-06 23:04:46.000000 cedarpy-0.1.0/README.md
--rw-r--r--   0     1001      123     3085 2023-07-06 23:04:46.000000 cedarpy-0.1.0/cedarpy/__init__.py
--rw-r--r--   0     1001      123        0 2023-07-06 23:04:46.000000 cedarpy-0.1.0/cedarpy/cedarpolicy.pyi
--rw-r--r--   0     1001      123        0 2023-07-06 23:04:46.000000 cedarpy-0.1.0/cedarpy/py.typed
--rw-r--r--   0     1001      123      615 2023-07-06 23:04:46.000000 cedarpy-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      845 2023-07-06 23:04:46.000000 cedarpy-0.1.0/requirements.dev.txt
--rw-r--r--   0     1001      123      157 2023-07-06 23:04:46.000000 cedarpy-0.1.0/requirements.txt
--rw-r--r--   0     1001      123     9833 2023-07-06 23:04:46.000000 cedarpy-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      456 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/integration/__init__.py
--rw-r--r--   0     1001      123    20328 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/integration/test_cedar_integration_tests.py
--rw-r--r--   0     1001      123     1152 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/shared/__init__.py
--rw-r--r--   0     1001      123      456 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3737 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/resources/sandbox_b/entities.json
--rw-r--r--   0     1001      123     6627 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/resources/sandbox_b/schema.json
--rw-r--r--   0     1001      123     6935 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/resources/sandbox_b/schema_exts.json
--rw-r--r--   0     1001      123    13884 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/test_authorize.py
--rw-r--r--   0     1001      123     4526 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/test_domain.py
--rw-r--r--   0     1001      123      536 2023-07-06 23:04:46.000000 cedarpy-0.1.0/tests/unit/test_import_module.py
--rw-r--r--   0     1001      123      129 2023-07-06 23:04:46.000000 cedarpy-0.1.0/third_party/README.md
--rw-r--r--   0     1001      123    36554 2023-07-06 23:04:46.000000 cedarpy-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 cedarpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 cedarpy-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     4611 2023-07-07 17:29:08.000000 cedarpy-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      703 2023-07-07 17:29:08.000000 cedarpy-0.2.0/.gitignore
+-rw-r--r--   0     1001      123       95 2023-07-07 17:29:08.000000 cedarpy-0.2.0/.gitmodules
+-rw-r--r--   0     1001      123    11358 2023-07-07 17:29:08.000000 cedarpy-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1024 2023-07-07 17:29:08.000000 cedarpy-0.2.0/Makefile
+-rw-r--r--   0     1001      123     7871 2023-07-07 17:29:08.000000 cedarpy-0.2.0/README.md
+-rw-r--r--   0     1001      123     3670 2023-07-07 17:29:08.000000 cedarpy-0.2.0/cedarpy/__init__.py
+-rw-r--r--   0     1001      123        0 2023-07-07 17:29:08.000000 cedarpy-0.2.0/cedarpy/cedarpolicy.pyi
+-rw-r--r--   0     1001      123        0 2023-07-07 17:29:08.000000 cedarpy-0.2.0/cedarpy/py.typed
+-rw-r--r--   0     1001      123      615 2023-07-07 17:29:08.000000 cedarpy-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      845 2023-07-07 17:29:08.000000 cedarpy-0.2.0/requirements.dev.txt
+-rw-r--r--   0     1001      123      157 2023-07-07 17:29:08.000000 cedarpy-0.2.0/requirements.txt
+-rw-r--r--   0     1001      123    10416 2023-07-07 17:29:08.000000 cedarpy-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123      456 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0     1001      123    20328 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/integration/test_cedar_integration_tests.py
+-rw-r--r--   0     1001      123     1152 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/shared/__init__.py
+-rw-r--r--   0     1001      123      456 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3737 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/resources/sandbox_b/entities.json
+-rw-r--r--   0     1001      123     6627 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/resources/sandbox_b/schema.json
+-rw-r--r--   0     1001      123     6935 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/resources/sandbox_b/schema_exts.json
+-rw-r--r--   0     1001      123    13884 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/test_authorize.py
+-rw-r--r--   0     1001      123     4526 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/test_domain.py
+-rw-r--r--   0     1001      123     1325 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/test_format_policy.py
+-rw-r--r--   0     1001      123      536 2023-07-07 17:29:08.000000 cedarpy-0.2.0/tests/unit/test_import_module.py
+-rw-r--r--   0     1001      123      129 2023-07-07 17:29:08.000000 cedarpy-0.2.0/third_party/README.md
+-rw-r--r--   0     1001      123    36554 2023-07-07 17:29:08.000000 cedarpy-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     8439 1970-01-01 00:00:00.000000 cedarpy-0.2.0/PKG-INFO
```

### Comparing `cedarpy-0.1.0/.github/workflows/CI.yml` & `cedarpy-0.2.0/.github/workflows/CI.yml`

 * *Files 19% similar despite different names*

```diff
@@ -39,33 +39,37 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
         if: ${{ startsWith(matrix.target, 'x86_64') }}
         shell: bash
+        # disabling the PyPI index on `pip install cedarpy` to ensure we
+        # install cedarpy from the local folder
         run: |
           set -e
-          pip install cedarpy --find-links dist --force-reinstall
+          pip install cedarpy --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'x86') && matrix.target != 'ppc64' }}
         uses: uraimo/run-on-arch-action@v2.5.0
         with:
           arch: ${{ matrix.target }}
           distro: ubuntu22.04
           githubToken: ${{ github.token }}
           install: |
             apt-get update
             apt-get install -y --no-install-recommends python3 python3-pip
             pip3 install -U pip pytest
+          # disabling the PyPI index on `pip install cedarpy` to ensure we
+          # install cedarpy from the local folder
           run: |
             set -e
-            pip3 install cedarpy --find-links dist --force-reinstall
+            pip3 install cedarpy --no-index --find-links dist --force-reinstall
             pytest
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64]
@@ -85,17 +89,19 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'aarch64') }}
         shell: bash
+        # disabling the PyPI index on `pip install cedarpy` to ensure we
+        # install cedarpy from the local folder
         run: |
           set -e
-          pip install cedarpy --find-links dist --force-reinstall
+          pip install cedarpy --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
 
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
@@ -115,17 +121,19 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'aarch64') }}
         shell: bash
+        # disabling the PyPI index on `pip install cedarpy` to ensure we
+        # install cedarpy from the local folder
         run: |
           set -e
-          pip install cedarpy --find-links dist --force-reinstall
+          pip install cedarpy --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `cedarpy-0.1.0/.gitignore` & `cedarpy-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/LICENSE` & `cedarpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/Makefile` & `cedarpy-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/README.md` & `cedarpy-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,108 @@
 # Cedar Python
 ![CI (main)](https://github.com/k9securityio/cedar-py/actions/workflows/CI.yml/badge.svg?branch=main)
+&nbsp;[![PyPI version](https://badge.fury.io/py/cedarpy.svg)](https://badge.fury.io/py/cedarpy)
 
-This repository contains `cedarpy`, a Python package that allows using the (Rust) [Cedar Policy](https://github.com/cedar-policy/cedar/tree/main) library from Python more convenient.
-
-This project is built on the [PyO3](https://docs.rs/pyo3/latest/pyo3/index.html) and [maturin](https://www.maturin.rs/index.html) projects.  These projects are designed to enable Python to use Rust code and vice versa.
+`cedarpy` helps you use the (Rust) [Cedar Policy](https://github.com/cedar-policy/cedar/tree/main) library from Python. You can use `cedarpy` to:
+* check whether a request is authorized by the [Cedar Policy](https://www.cedarpolicy.com) engine
+* format policies
+
+`cedarpy` packages are availble for the following platforms:
+<table>
+<thead><tr><th>Operating System</th><th>Processor Architectures</th></tr></thead>
+<tbody>
+    <tr><td>Linux</td><td>x86_64, aarch64</td></tr>
+    <tr><td>Mac</td><td>x86_64, aarch64</td></tr>
+    <tr><td>Windows</td><td>x86_64</td></tr>
+</tbody>
+</table>
 
 Note: This project is _not_ officially supported by AWS or the Cedar Policy team.
 
-## Getting started
+## Using the library
+Releases of [`cedarpy`](https://pypi.org/project/cedarpy/) are available on PyPi.  You can install the latest release with:
+```shell
+pip install cedarpy
+```
+
+(See the Developing section for how to use artifacts you've built locally.)
+
+### Authorizing access with Cedar policies in Python
+Now you can use the library to authorize access with Cedar from your Python project using the `is_authorized` function.  Here's an example of basic use:
+
+```python
+from cedarpy import is_authorized, AuthzResult, Decision
+
+policies: str = "//a string containing cedar policies"
+entities: list = [  # a list of Cedar entities; can also be a json-formatted string of Cedar entities
+    {"uid": {"__expr": "User::\"alice\""}, "attrs": {}, "parents": []}
+    # ...
+]
+request = {
+    "principal": "User::\"bob\"",
+    "action": "Action::\"view\"",
+    "resource": "Photo::\"1234-abcd\"",
+    "context": {}
+}
+
+authz_result: AuthzResult = is_authorized(request, policies, entities)
+
+# so you can assert on the decision like:
+assert Decision.Allow == authz_result.decision
+
+# or use the 'allowed' convenience method 
+assert authz_result.allowed
+
+# or even via AuthzResult's attribute subscripting support 
+assert authz_result['allowed']
+
+```
+The [`AuthzResult`](cedarpy/__init__.py) class also provides diagnostics and metrics for the access evaluation request. 
+
+See the [unit tests](tests/unit) for more examples of use and expected behavior.
+
+### Formatting Cedar policies
+
+You can use `format_policies` to pretty-print Cedar policies according to
+convention.
+
+```python
+from cedarpy import format_policies
+
+policies: str = """
+    permit(
+        principal,
+        action == Action::"edit",
+        resource
+    )
+    when {
+        resource.owner == principal
+    };
+"""
+
+print(format_policies(policies))
+# permit (
+#   principal,
+#   action == Action::"edit",
+#   resource
+# )
+# when { resource.owner == principal };
+```
+
+## Developing
+
 
 You'll need a few things to get started:
 
 * Python +3.9
 * Rust and `cargo`
 
-The most common development commands are in the `Makefile`
+This project is built on the [PyO3](https://docs.rs/pyo3/latest/pyo3/index.html) and [maturin](https://www.maturin.rs/index.html) projects.  These projects are designed to enable Python to use Rust code and vice versa.
 
-Note: This project is developed on an M1 Mac with Python 3.9.
+The most common development commands are in the `Makefile`
 
 ### Create virtual env
 
 First create a Python virtual environment for this project with:
 `make venv-dev`
 
 In addition to creating a dedicated virtual environment, this will install `cedar-py`'s dependencies.
@@ -88,62 +170,38 @@
 ```
 
 Then you can run:
 ```shell
 make integration-tests
 ```
 
-`cedar-py` currently passes 46 of the 50 'example_use_cases_doc' tests.  We will support executing more tests shortly. See [test_cedar_integration_tests.py](tests/integration/test_cedar_integration_tests.py) for details.
+`cedar-py` currently passes 69 of the 82 tests defined in the `example_use_cases_doc`, `multi`, `ip`, and `decimal` suites. (The pass rate is actually higher, but we skip some tests that pass due to the way test suites are loaded.)  See [test_cedar_integration_tests.py](tests/integration/test_cedar_integration_tests.py) for details.
 
-## Using the library
-Releases of `cedarpy` will be available on PyPi soon.  For now, if you'd like to use the library, you can build a release locally and install it with `pip`.
+### Using locally-built artifacts
 
-If you used `make quick` above, the `cedarpy` module will already be installed. You can also use `make release` to build a release locally.
+If you used `make quick` above, then a development build of the `cedarpy` module will already be installed in the virtual environment. 
 
-The release process will build a wheel and output it into `target/wheels/`
+If you want to use your local `cedarpy` changes in another Python environment, you'll need to build a release with:
 
-You can install that file with pip, e.g.:
 ```shell
-pip install /path/to/cedar-py/target/wheels/cedarpy-0.1.0-cp39-cp39-macosx_11_0_arm64.whl
+make release
 ```
 
-Then you can use the library from your Python project just like the [tests](tests/unit) demonstrate:
-
-```python
-from cedarpy import is_authorized, AuthzResult, Decision
-
-policies: str = "//a string containing cedar policies"
-entities: list = [  # a list of Cedar entities; can also be a json-formatted string of Cedar entities
-    {"uid": {"__expr": "User::\"alice\""}, "attrs": {}, "parents": []}
-    # ...
-]
-request = {
-    "principal": "User::\"bob\"",
-    "action": "Action::\"view\"",
-    "resource": "Photo::\"1234-abcd\"",
-    "context": {}
-}
-
-authz_result: AuthzResult = is_authorized(request, policies, entities)
-
-# so you can assert on the decision like:
-assert Decision.Allow == authz_result.decision
-
-# or use the 'allowed' convenience method 
-assert authz_result.allowed
-
-# or even via AuthzResult's attribute subscripting support 
-assert authz_result['allowed']
+The release process will build a wheel and output it into `target/wheels/`
 
+Now you can install that file with pip, e.g.:
+```shell
+pip install --force-reinstall /path/to/cedar-py/target/wheels/ccedarpy-*.whl
 ```
 
+
 ## Contributing
 
-This project is very early stage. This project uses GitHub [issues](https://github.com/k9securityio/cedar-py/issues). Contributions are welcome.
+This project is in its early stages and contributions are welcome. Please check the project's GitHub [issues](https://github.com/k9securityio/cedar-py/issues) for work we've already identified.
 
 Some ways to contribute are:
 * Use the project and report experience and issues
 * Document usage and limitations
 * Enhance the library with additional functionality you need
 * Add test cases, particularly those from [`cedar-integration-tests`](https://github.com/k9securityio/cedar-py/issues/3)
 
-You can reach peopel interested in this project in the `cedar-py` channel of the Cedar Policy Slack workspace.
+You can reach people interested in this project in the `#cedar-py` channel of the [Cedar Policy Slack workspace](https://communityinviter.com/apps/cedar-policy/cedar-policy-language).
```

### Comparing `cedarpy-0.1.0/cedarpy/__init__.py` & `cedarpy-0.2.0/cedarpy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,7 +93,21 @@
         if isinstance(schema, str):
             pass
         elif isinstance(schema, dict):
             schema = json.dumps(schema)
 
     authz_response = _internal.is_authorized(request, policies, entities, schema, verbose)
     return AuthzResult(json.loads(authz_response))
+
+def format_policies(policies: str,
+                    line_width: int = 80,
+                    indent_width: int = 2) -> str:
+    """Format the provided policies according to the Cedar conventions.
+
+    :param policies is a str containing the policies to be formatted
+    :param line_width (optional) is the desired maximum line length
+    :param indent_width (optional) is the desired indentation width
+
+    :returns the formatted policy
+    :raises ValueError: if the input policies cannot be parsed
+    """
+    return _internal.format_policies(policies, line_width, indent_width)
```

### Comparing `cedarpy-0.1.0/pyproject.toml` & `cedarpy-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/requirements.dev.txt` & `cedarpy-0.2.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/src/lib.rs` & `cedarpy-0.2.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 use std::collections::HashMap;
 use std::str::FromStr;
 use std::time::Instant;
 
 use anyhow::{Context as _, Error, Result};
 use cedar_policy::*;
+use cedar_policy_formatter::{Config, policies_str_to_pretty};
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyString};
 use serde::{Deserialize, Serialize};
 
 /// Echo (return) the input string
 #[pyfunction]
 #[pyo3(signature = (s))]
 fn echo(s: String) -> PyResult<String> {
     Ok(s)
 }
 
+// Pretty-print the input policy according to the input parameters.
+#[pyfunction]
+#[pyo3(signature = (s, line_width, indent_width))]
+fn format_policies(s: String, line_width: usize, indent_width: isize) -> PyResult<String> {
+    let config = Config {
+        line_width,
+        indent_width,
+    };
+
+    match policies_str_to_pretty(&s, &config) {
+        Ok(s) => Ok(s),
+        Err(e) => Err(pyo3::exceptions::PyValueError::new_err(e.to_string())),
+    }
+}
+
 pub struct RequestArgs {
     /// Principal for the request, e.g., User::"alice"
     pub principal: Option<String>,
     /// Action for the request, e.g., Action::"view"
     pub action: Option<String>,
     /// Resource for the request, e.g., File::"myfile.txt"
     pub resource: Option<String>,
@@ -279,9 +295,10 @@
 
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn _internal(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(echo, m)?)?;
     m.add_function(wrap_pyfunction!(is_authorized, m)?)?;
+    m.add_function(wrap_pyfunction!(format_policies, m)?)?;
     Ok(())
 }
```

### Comparing `cedarpy-0.1.0/tests/integration/test_cedar_integration_tests.py` & `cedarpy-0.2.0/tests/integration/test_cedar_integration_tests.py`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/shared/__init__.py` & `cedarpy-0.2.0/tests/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/resources/sandbox_b/entities.json` & `cedarpy-0.2.0/tests/unit/resources/sandbox_b/entities.json`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/resources/sandbox_b/schema.json` & `cedarpy-0.2.0/tests/unit/resources/sandbox_b/schema.json`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/resources/sandbox_b/schema_exts.json` & `cedarpy-0.2.0/tests/unit/resources/sandbox_b/schema_exts.json`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/test_authorize.py` & `cedarpy-0.2.0/tests/unit/test_authorize.py`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/test_domain.py` & `cedarpy-0.2.0/tests/unit/test_domain.py`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/tests/unit/test_import_module.py` & `cedarpy-0.2.0/tests/unit/test_import_module.py`

 * *Files identical despite different names*

### Comparing `cedarpy-0.1.0/Cargo.lock` & `cedarpy-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
  "stacker",
  "thiserror",
  "unicode-security",
 ]
 
 [[package]]
 name = "cedarpy"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "anyhow",
  "cedar-policy",
  "cedar-policy-cli",
  "cedar-policy-formatter",
  "pyo3",
  "serde",
```

