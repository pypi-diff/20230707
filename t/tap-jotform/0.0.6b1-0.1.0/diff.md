# Comparing `tmp/tap_jotform-0.0.6b1.tar.gz` & `tmp/tap_jotform-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_jotform-0.0.6b1.tar", max compression
+gzip compressed data, was "tap_jotform-0.1.0.tar", max compression
```

## Comparing `tap_jotform-0.0.6b1.tar` & `tap_jotform-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/LICENSE
--rw-r--r--   0        0        0     3508 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/README.md
--rw-r--r--   0        0        0     1838 2023-04-24 20:19:28.196800 tap_jotform-0.0.6b1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/__init__.py
--rw-r--r--   0        0        0      116 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/__main__.py
--rw-r--r--   0        0        0     5305 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/client.py
--rw-r--r--   0        0        0     8462 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/streams.py
--rw-r--r--   0        0        0     2738 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/tap.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 tap_jotform-0.0.6b1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-07 16:27:18.414427 tap_jotform-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3508 2023-07-07 16:27:18.414427 tap_jotform-0.1.0/README.md
+-rw-r--r--   0        0        0     1845 2023-07-07 16:27:43.370377 tap_jotform-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/__main__.py
+-rw-r--r--   0        0        0     5296 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/client.py
+-rw-r--r--   0        0        0     8428 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/streams.py
+-rw-r--r--   0        0        0     2738 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/tap.py
+-rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 tap_jotform-0.1.0/PKG-INFO
```

### Comparing `tap_jotform-0.0.6b1/LICENSE` & `tap_jotform-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.6b1/README.md` & `tap_jotform-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.6b1/pyproject.toml` & `tap_jotform-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 [build-system]
-requires = ["poetry-core>=1.1.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
-
-[tool.black]
-line-length = 88
+requires = [
+  "poetry-core>=1.1",
+  "poetry-dynamic-versioning",
+]
 
 [tool.poetry]
 name = "tap-jotform"
-version = "0.0.6b1"
+version = "0.1.0"
 description = "Singer tap for Jotform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-jotform"
 repository = "https://github.com/edgarrmondragon/tap-jotform"
 documentation = "https://github.com/edgarrmondragon/tap-jotform/#readme"
 keywords = ["ELT", "Jotform"]
 
 [tool.poetry.dependencies]
-colorama = "==0.4.6"
+colorama = "==0.4.*"
 importlib-metadata = {version = "<5.0.0", python = "<3.8"}
 python = "<3.12,>=3.7.1"
-requests-cache = "==1.0.1"
-singer-sdk = "==0.24.0"
-structlog = "==23.1.0"
+requests-cache = "==1.1.*"
+singer-sdk = ">=0.28,<0.30"
+structlog = "==23.1.*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.poetry.scripts]
 # CLI declaration
 tap-jotform = 'tap_jotform.tap:TapJotform.cli'
 
-[tool.poetry-dynamic-versioning]
-enable = false
-format-jinja = """
-    {%- if distance == 0 -%}
-        {{ serialize_pep440(base, stage, revision) }}
-    {%- elif revision is not none -%}
-        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
-    {%- else -%}
-        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
-    {%- endif -%}
-"""
-metadata = true
-style = "pep440"
-vcs = "git"
+[tool.black]
+line-length = 88
 
 [tool.ruff]
 ignore = ["ANN101", "DJ", "PD"]
 line-length = 88
 select = ["ALL"]
 src = ["tap_jotform", "tests", "noxfile.py"]
 target-version = "py37"
@@ -60,7 +48,22 @@
 
 [tool.ruff.per-file-ignores]
 "noxfile.py" = ["ANN"]
 "tests/*" = ["ANN"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+format-jinja = """
+    {%- if distance == 0 -%}
+        {{ serialize_pep440(base, stage, revision) }}
+    {%- elif revision is not none -%}
+        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
+    {%- else -%}
+        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
+    {%- endif -%}
+"""
+metadata = true
+style = "pep440"
+vcs = "git"
```

### Comparing `tap_jotform-0.0.6b1/tap_jotform/client.py` & `tap_jotform-0.1.0/tap_jotform/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,25 @@
 
         Returns:
             True if there are more pages to fetch, False otherwise.
         """
         result_set = response.json()["resultSet"]
         count = int(result_set["count"])
 
-        if count == self._page_size:
-            return True
-
-        return False
+        return count == self._page_size
 
 
 class JotformStream(RESTStream):
     """Jotform stream class."""
 
     page_size = 100
-    primary_keys: list[str] | None = ["id"]
+    primary_keys: tuple[str, ...] = ("id",)  # type: ignore[assignment]
     records_jsonpath = "$.content[*]"
 
-    INTEGER_FIELDS: list[str] = []
+    INTEGER_FIELDS: tuple[str, ...] = ()
 
     @property
     def url_base(self) -> str:
         """Return the API URL root, configurable via tap settings.
 
         Returns:
             The API URL root.
```

### Comparing `tap_jotform-0.0.6b1/tap_jotform/streams.py` & `tap_jotform-0.1.0/tap_jotform/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
 class FormsStream(JotformPaginatedStream):
     """Forms stream."""
 
     name = "forms"
     path = "/user/forms"
 
-    INTEGER_FIELDS = [
+    INTEGER_FIELDS = (
         "height",
         "new",
         "count",
         "favorite",
         "archived",
-    ]
+    )
 
     schema = th.PropertiesList(
         th.Property("id", th.StringType, description="The Form ID"),
         th.Property("username", th.StringType),
         th.Property("title", th.StringType),
         th.Property("height", th.IntegerType),
         th.Property("url", th.StringType),
@@ -77,19 +77,19 @@
         """
         return {"form_id": record["id"]}
 
 
 class QuestionsStream(JotformStream):
     """Questions stream."""
 
-    INTEGER_FIELDS = ["order"]
+    INTEGER_FIELDS = ("order",)
 
     name = "questions"
     path = "/form/{form_id}/questions"
-    primary_keys = ["form_id", "qid"]
+    primary_keys = ("form_id", "qid")
     replication_key = None
     parent_stream_type = FormsStream
 
     schema = th.PropertiesList(
         th.Property("qid", th.StringType, required=True, description="Question ID"),
         th.Property("form_id", th.StringType, required=True, description="Form ID"),
         th.Property(
@@ -135,18 +135,18 @@
 
 class SubmissionsStream(JotformPaginatedStream):
     """Submissions stream."""
 
     name = "submissions"
     path = "/user/submissions"
 
-    INTEGER_FIELDS = [
+    INTEGER_FIELDS = (
         "flag",
         "new",
-    ]
+    )
 
     schema = th.PropertiesList(
         th.Property("id", th.StringType, description="The Submission ID"),
         th.Property("form_id", th.StringType),
         th.Property("ip", th.StringType),
         th.Property("flag", th.IntegerType),
         th.Property("notes", th.StringType),
@@ -250,15 +250,15 @@
 
 
 class UserHistory(JotformStream):
     """User History stream."""
 
     name = "user_history"
     path = "/user/history"
-    primary_keys = ["username", "timestamp", "type"]
+    primary_keys = ("username", "timestamp", "type")
 
     schema = th.PropertiesList(
         th.Property(
             "type",
             th.StringType,
             allowed_values=[
                 "userCreation",
@@ -276,24 +276,24 @@
         th.Property("email", th.EmailType),
         th.Property("parent", th.StringType),
         th.Property("subuser", th.StringType),
     ).to_dict()
 
     def get_url_params(
         self,
-        context: dict | None,
-        next_page_token: tuple[datetime.date, datetime.date] | None,
-    ) -> dict[str, t.Any]:
+        context: dict | None,  # noqa: ARG002
+        next_page_token: tuple[datetime.date, datetime.date] | None,  # noqa: ARG002
+    ) -> dict[str, t.Any] | str:
         """Get the URL parameters.
 
         Args:
             context: The context object.
             next_page_token: The next page token.
 
         Returns:
             The URL parameters.
         """
-        params = super().get_url_params(context, next_page_token)
-        params["action"] = "all"
-        params["date"] = "all"
-        params["sortBy"] = "ASC"
-        return params
+        return {
+            "action": "all",
+            "date": "all",
+            "sortBy": "ASC",
+        }
```

### Comparing `tap_jotform-0.0.6b1/tap_jotform/tap.py` & `tap_jotform-0.1.0/tap_jotform/tap.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.6b1/PKG-INFO` & `tap_jotform-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-jotform
-Version: 0.0.6b1
+Version: 0.1.0
 Summary: Singer tap for Jotform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-jotform
 License: Apache-2.0
 Keywords: ELT,Jotform
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -12,19 +12,19 @@
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorama (==0.4.6)
+Requires-Dist: colorama (==0.4.*)
 Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
-Requires-Dist: requests-cache (==1.0.1)
-Requires-Dist: singer-sdk (==0.24.0)
-Requires-Dist: structlog (==23.1.0)
+Requires-Dist: requests-cache (==1.1.*)
+Requires-Dist: singer-sdk (>=0.28,<0.30)
+Requires-Dist: structlog (==23.1.*)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-jotform/#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-jotform
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-jotform
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: tap-jotform Version: 0.0.6b1 Summary: Singer tap
-for Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
+Metadata-Version: 2.1 Name: tap-jotform Version: 0.1.0 Summary: Singer tap for
+Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-jotform License: Apache-2.0 Keywords:
 ELT,Jotform Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: colorama
-(==0.4.6) Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
-Requires-Dist: requests-cache (==1.0.1) Requires-Dist: singer-sdk (==0.24.0)
-Requires-Dist: structlog (==23.1.0) Project-URL: Documentation, https://
-github.com/edgarrmondragon/tap-jotform/#readme Project-URL: Repository, https:/
-/github.com/edgarrmondragon/tap-jotform Description-Content-Type: text/markdown
+(==0.4.*) Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
+Requires-Dist: requests-cache (==1.1.*) Requires-Dist: singer-sdk
+(>=0.28,<0.30) Requires-Dist: structlog (==23.1.*) Project-URL: Documentation,
+https://github.com/edgarrmondragon/tap-jotform/#readme Project-URL: Repository,
+https://github.com/edgarrmondragon/tap-jotform Description-Content-Type: text/
+markdown
                                  # tap-jotform
                        [pre-commit.ci_status] [License]
      Singer Tap for Jotform. Built with the [Meltano Singer SDK](https://
                                sdk.meltano.com).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
 `schema-flattening` ## Settings | Setting | Required | Default | Description |
 |:--------------------|:--------:|:-------:|:------------| | api_key | True |
```

