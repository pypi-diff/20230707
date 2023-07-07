# Comparing `tmp/pytest_dogu_report-1.0.0.tar.gz` & `tmp/pytest_dogu_report-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dogu_report-1.0.0.tar", max compression
+gzip compressed data, was "pytest_dogu_report-1.0.1.tar", max compression
```

## Comparing `pytest_dogu_report-1.0.0.tar` & `pytest_dogu_report-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1693 2023-06-30 04:38:35.394263 pytest_dogu_report-1.0.0/README.md
--rw-r--r--   0        0        0     1079 2023-07-03 07:31:40.467889 pytest_dogu_report-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      540 2023-06-28 08:30:52.468263 pytest_dogu_report-1.0.0/src/pytest_dogu_report/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-28 08:30:52.468424 pytest_dogu_report-1.0.0/src/pytest_dogu_report/protocols.py
--rw-r--r--   0        0        0     9032 2023-06-28 08:30:52.468629 pytest_dogu_report-1.0.0/src/pytest_dogu_report/step_reporter.py
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 pytest_dogu_report-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      874 2023-07-07 07:38:34.576473 pytest_dogu_report-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1693 2023-07-01 06:42:05.070785 pytest_dogu_report-1.0.1/README.md
+-rw-r--r--   0        0        0      540 2023-06-29 07:23:27.711622 pytest_dogu_report-1.0.1/src/pytest_dogu_report/__init__.py
+-rw-r--r--   0        0        0     4373 2023-07-06 12:44:38.708643 pytest_dogu_report-1.0.1/src/pytest_dogu_report/protocols.py
+-rw-r--r--   0        0        0     9080 2023-07-07 07:34:48.424131 pytest_dogu_report-1.0.1/src/pytest_dogu_report/step_reporter.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 pytest_dogu_report-1.0.1/PKG-INFO
```

### Comparing `pytest_dogu_report-1.0.0/README.md` & `pytest_dogu_report-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_dogu_report-1.0.0/pyproject.toml` & `pytest_dogu_report-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dogu-report"
-version = "1.0.0"
+version = "1.0.1"
 description = "pytest plugin for dogu report"
 readme = "README.md"
 packages = [{include = "pytest_dogu_report", from = "src"}]
 authors = ["henry"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,26 +17,16 @@
 black = "^23.3.0"
 pylint = "^2.17.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[project]
-name = "pytest-dogu-report"
-version = "1.0.0"
-description = "pytest plugin for dogu report"
-license = {text = "MIT License"}
-classifiers = [
-    "Framework :: Pytest",
-]
-requires-python = '>=3.9,<4.0'
-
 [project.entry-points.pytest11]
-dogu_report = "pytest_dogu_report"
+pytest_dogu_report = "pytest_dogu_report"
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 180
 disable = """
     missing-module-docstring,
     missing-class-docstring,
     missing-function-docstring,
```

### Comparing `pytest_dogu_report-1.0.0/src/pytest_dogu_report/__init__.py` & `pytest_dogu_report-1.0.1/src/pytest_dogu_report/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_report-1.0.0/src/pytest_dogu_report/protocols.py` & `pytest_dogu_report-1.0.1/src/pytest_dogu_report/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 import requests
 from dacite import Config, from_dict
 
 
 T = TypeVar("T")
-DEFAULT_TIMEOUT = 60
+DEFAULT_TIMEOUT = 60  # unit: seconds
 
 
 @unique
 class DestType(IntEnum):
     JOB = 0
     UNIT = 1
 
@@ -38,15 +38,15 @@
 class DestInfo:
     name: str
     type: DestType
     children: List["DestInfo"] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
-class UpdateDestStateRequestBody:
+class UpdateDestStatusRequestBody:
     # pylint: disable=invalid-name
     destStatus: DestState
 
     # pylint: disable=invalid-name
     localTimeStamp: str
 
 
@@ -120,15 +120,15 @@
             CreateDestResponse, response_body_raw
         )
         return response_body.dests
 
     def update_dest_status(self, dest_id: str, status: DestState, local_time: datetime):
         url = f"{self.options.api_base_url}/public/organizations/{self.options.organization_id}/devices/{self.options.device_id}/dests/{dest_id}/status"
         headers = self._create_headers()
-        request_body = UpdateDestStateRequestBody(
+        request_body = UpdateDestStatusRequestBody(
             destStatus=status, localTimeStamp=local_time.isoformat()
         )
         request_body_raw = self._create_request_body_raw(request_body)
         response = requests.patch(
             url, json=request_body_raw, headers=headers, timeout=DEFAULT_TIMEOUT
         )
         response.raise_for_status()
```

### Comparing `pytest_dogu_report-1.0.0/src/pytest_dogu_report/step_reporter.py` & `pytest_dogu_report-1.0.1/src/pytest_dogu_report/step_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 PyTestLocation = Tuple[str, Optional[int], str]
 
 
 @dataclass
 class UnitInfo:
     dest_id: str
     status: DestState = DestState.PENDING
-    start_time: Optional[datetime] = None
-    end_time: Optional[datetime] = None
+    started_at: Optional[datetime] = None
+    finished_at: Optional[datetime] = None
 
 
 unit_info_key = StashKey()
 
 
 @dataclass
 class JobInfo:
     dest_id: str
     status: DestState = DestState.PENDING
-    start_time: Optional[datetime] = None
-    end_time: Optional[datetime] = None
+    started_at: Optional[datetime] = None
+    finished_at: Optional[datetime] = None
     children: List[UnitInfo] = field(default_factory=list)
 
 
 job_info_key = StashKey()
 
 
 @dataclass
@@ -95,102 +95,102 @@
     @hookimpl(trylast=True)
     def pytest_collection_modifyitems(
         self, session: Session, config: Config, items: List[Item]
     ) -> None:
         try:
             self._on_pytest_collection_modifyitems(session, config, items)
         except Exception as e:
-            print(f"failed on pytest_collection_modifyitems: {e}")
+            print(f"[dogu] failed on pytest_collection_modifyitems: {e}")
 
     def _on_pytest_collection_modifyitems(
         self, session: Session, config: Config, items: List[Item]
     ) -> None:
         dest_infos = self._create_dest_infos(items)
         dest_datas = self._client.create_dest(dest_infos)
         self._stash_items(items, dest_datas)
 
     @hookimpl(trylast=True)
     def pytest_runtest_logstart(self, nodeid: str, location: PyTestLocation) -> None:
         try:
             self._on_pytest_runtest_logstart(nodeid, location)
         except Exception as e:
-            print(f"failed on pytest_runtest_logstart: {e}")
+            print(f"[dogu] failed on pytest_runtest_logstart: {e}")
 
     def _on_pytest_runtest_logstart(
         self, nodeid: str, location: PyTestLocation
     ) -> None:
         item = self._item_map.get(nodeid)
         if item is None:
             raise Exception(f"nodeid {nodeid} is not found")
         job_info = _get_job_info(item)
         if job_info.status == DestState.PENDING:
-            job_info.start_time = datetime.now()
+            job_info.started_at = datetime.now()
             job_info.status = DestState.RUNNING
             self._client.update_dest_status(
-                job_info.dest_id, job_info.status, job_info.start_time
+                job_info.dest_id, job_info.status, job_info.started_at
             )
 
         unit_info = _get_unit_info(item)
-        unit_info.start_time = datetime.now()
+        unit_info.started_at = datetime.now()
         unit_info.status = DestState.RUNNING
         self._client.update_dest_status(
-            unit_info.dest_id, unit_info.status, unit_info.start_time
+            unit_info.dest_id, unit_info.status, unit_info.started_at
         )
 
     @hookimpl(trylast=True)
     def pytest_runtest_logfinish(self, nodeid: str, location: PyTestLocation) -> None:
         try:
             self._on_pytest_runtest_logfinish(nodeid, location)
         except Exception as e:
-            print(f"failed on pytest_runtest_logfinish: {e}")
+            print(f"[dogu] failed on pytest_runtest_logfinish: {e}")
 
     def _on_pytest_runtest_logfinish(
         self, nodeid: str, location: PyTestLocation
     ) -> None:
         item = self._item_map.get(nodeid)
         if item is None:
             raise Exception(f"nodeid {nodeid} is not found")
         unit_info = _get_unit_info(item)
         self._client.update_dest_status(
-            unit_info.dest_id, unit_info.status, unit_info.end_time
+            unit_info.dest_id, unit_info.status, unit_info.finished_at
         )
 
         job_info = _get_job_info(item)
         if all(child.status.is_completed() for child in job_info.children):
             self._client.update_dest_status(
-                job_info.dest_id, job_info.status, job_info.end_time
+                job_info.dest_id, job_info.status, job_info.finished_at
             )
 
     @hookimpl(trylast=True)
     def pytest_runtest_logreport(self, report: TestReport) -> None:
         try:
             self._on_pytest_runtest_logreport(report)
         except Exception as e:
-            print(f"failed on pytest_runtest_logreport: {e}")
+            print(f"[dogu] failed on pytest_runtest_logreport: {e}")
 
     def _on_pytest_runtest_logreport(self, report: TestReport) -> None:
         if report.when != "call":
             return
         item = self._item_map.get(report.nodeid)
         if item is None:
             raise Exception(f"nodeid {report.nodeid} is not found")
         unit_info = _get_unit_info(item)
-        unit_info.end_time = datetime.now()
+        unit_info.finished_at = datetime.now()
         if report.passed:
             unit_info.status = DestState.PASSED
         elif report.failed:
             unit_info.status = DestState.FAILED
         elif report.skipped:
             unit_info.status = DestState.SKIPPED
         else:
             raise Exception(f"unknown report status {report.outcome}")
 
         job_info = _get_job_info(item)
         if all(child.status.is_completed() for child in job_info.children):
-            job_info.end_time = datetime.now()
+            job_info.finished_at = datetime.now()
             if all(child.status == DestState.PASSED for child in job_info.children):
                 job_info.status = DestState.PASSED
             elif any(child.status == DestState.FAILED for child in job_info.children):
                 job_info.status = DestState.FAILED
             elif any(child.status == DestState.SKIPPED for child in job_info.children):
                 job_info.status = DestState.SKIPPED
             else:
@@ -255,10 +255,10 @@
 
 class StepReporterFactory:
     def __init__(self, options: StepOptions):
         self.options = options
 
     def create(self) -> StepReporter:
         if self.options.api_base_url == "":
-            print("dogu api base url is not specified. step reporter is disabled.")
+            print("[dogu] api base url is not specified. step reporter is disabled.")
             return NullStepReporter()
         return StepReporterImpl(self.options)
```

### Comparing `pytest_dogu_report-1.0.0/PKG-INFO` & `pytest_dogu_report-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dogu-report
-Version: 1.0.0
+Version: 1.0.1
 Summary: pytest plugin for dogu report
 Author: henry
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

