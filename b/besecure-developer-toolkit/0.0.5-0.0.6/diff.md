# Comparing `tmp/besecure_developer_toolkit-0.0.5.tar.gz` & `tmp/besecure_developer_toolkit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besecure_developer_toolkit-0.0.5.tar", max compression
+gzip compressed data, was "besecure_developer_toolkit-0.0.6.tar", max compression
```

## Comparing `besecure_developer_toolkit-0.0.5.tar` & `besecure_developer_toolkit-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/LICENSE
--rw-r--r--   0        0        0     3127 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/README.md
--rw-r--r--   0        0        0      341 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/__init__.py
--rw-r--r--   0        0        0      203 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/__main__.py
--rw-r--r--   0        0        0     9271 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/cli.py
--rw-r--r--   0        0        0        0 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/config.py
--rw-r--r--   0        0        0     9392 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_ossp_master.py
--rw-r--r--   0        0        0     5720 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_version_data.py
--rw-r--r--   0        0        0     5302 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/generate_report.py
--rw-r--r--   0        0        0     1662 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_assessment.py
--rw-r--r--   0        0        0     5254 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/License_compliance.py
--rw-r--r--   0        0        0      906 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/New_line_char.py
--rw-r--r--   0        0        0     3185 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Objective.py
--rw-r--r--   0        0        0     4467 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Sbom_report.py
--rw-r--r--   0        0        0     5310 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Scorecard_report.py
--rw-r--r--   0        0        0     7109 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Static_code_analysis.py
--rw-r--r--   0        0        0    10043 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_report_file.py
--rw-r--r--   0        0        0     4644 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_version_file.py
--rw-r--r--   0        0        0      654 2023-05-23 08:24:03.038484 besecure_developer_toolkit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3233 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/README.md
+-rw-r--r--   0        0        0      325 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/__main__.py
+-rw-r--r--   0        0        0     9838 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/cli.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/config.py
+-rw-r--r--   0        0        0     9392 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_ossp_master.py
+-rw-r--r--   0        0        0     5720 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_version_data.py
+-rw-r--r--   0        0        0     9349 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/generate_report.py
+-rw-r--r--   0        0        0     1587 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_assessment.py
+-rw-r--r--   0        0        0     5239 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/License_compliance.py
+-rw-r--r--   0        0        0      906 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/New_line_char.py
+-rw-r--r--   0        0        0     3185 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Objective.py
+-rw-r--r--   0        0        0     4452 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Sbom_report.py
+-rw-r--r--   0        0        0     5295 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Scorecard_report.py
+-rw-r--r--   0        0        0     7094 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Static_code_analysis.py
+-rw-r--r--   0        0        0    10013 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_report_file.py
+-rw-r--r--   0        0        0     4629 2023-07-07 11:53:04.873712 besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_version_file.py
+-rw-r--r--   0        0        0      668 2023-07-07 11:53:04.881712 besecure_developer_toolkit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.6/PKG-INFO
```

### Comparing `besecure_developer_toolkit-0.0.5/LICENSE` & `besecure_developer_toolkit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.5/README.md` & `besecure_developer_toolkit-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Be-Secure Developer Toolkit (bes-dev-kit)
+# BeS-dev-kit
 
-bes-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
+BeS-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 
 # Pre-requisites
 
 1. Python 3.10
 2. pip
 3. Github personal access token
 
 # Installation
 
-`$ python3 -m pip install besecure-developer-toolkit`
+`$ python3 -m pip install bes-dev-kit`
 
 # Usage
 
 If you are running the command for the first time, you will be prompted to provide the complete path to your `besecure-osspoi-datastore` and `besecure-assessment-datastore` and your `personal access token`
 
 ### Generate Metadata
 
@@ -30,15 +30,17 @@
 
 `Note: For the first time use this command will ask for three extra inputs - OSSPOI_DIR: location of besecure-osspoi-datastore in local system, ASSESSMENT_DIR: location of besecure-assessment-datastore, GITHUB_AUTH_TOKEN`
 
 ![metadata first time](docs/generate-metadata-first-time.jpg)
 
 ### Generate Reports
 
-`$ bes-dev-kit generate-report <report name>`
+`$ bes-dev-kit generate-report` -  generate all reports (scorecard, sciticality_score, codeql, sbom)
+
+`$ bes-dev-kit generate-report < report name > ... < report name >` - generate specific report
 
 ![generate report](docs/generate-report.gif)
 
 `<report name> - scorecard, codeql, criticality_score`
 
 For more options use `--help` at end.
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/cli.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-"""This module provides the Be-Secure Developer Toolkit CLI."""
+"""This module provides the BeS-dev-kit CLI."""
 # src/cli.py
 import os
 import ssl
 import json
 import sys
+from sys import platform
 from typing import Optional
 from typing import List
 from rich import print
 import typer
-from besecure_developer_toolkit import __app_name__, __version__
-from besecure_developer_toolkit.src.create_ossp_master import OSSPMaster
-from besecure_developer_toolkit.src.create_version_data import Version
-from besecure_developer_toolkit.src.generate_report import Report
-from besecure_developer_toolkit.src.validate_version_file import VersionFileValidate
-from besecure_developer_toolkit.src.risk_assessment import Generate_report
-from besecure_developer_toolkit.src.validate_report_file import ReportFileValidate
+from bes_dev_kit import __app_name__, __version__
+from bes_dev_kit.src.create_ossp_master import OSSPMaster
+from bes_dev_kit.src.create_version_data import Version
+from bes_dev_kit.src.generate_report import Report
+from bes_dev_kit.src.validate_version_file import VersionFileValidate
+from bes_dev_kit.src.risk_assessment import Generate_report
+from bes_dev_kit.src.validate_report_file import ReportFileValidate
 
 ssl._create_default_https_context = ssl._create_stdlib_context
 
 def write_env_vars_file():
     """Creates an env var file
     """
     user_home = os.path.expanduser('~')
@@ -95,64 +96,68 @@
 @app.command("generate-metadata")
 def ossp(
     issue_id: int = typer.Option(None, prompt="Enter OSSP id", help="OSSP id"),
     name: str = typer.Option(None, prompt="Enter OSSP name", help="OSSP name"),
     overwrite: bool = typer.Option(False, help="Overwrite the existing entries")
     ):
     """ Update OSSP-master.json file and add/update version file to osspoi datastore """
+    if platform != "linux":
+        print("[bold red]BeS-dev-kit is compatible"
+              " only with Linux operating systems")
+        raise typer.Exit()
     write_env_vars_file()
     check_if_value_empty()
     set_env_vars()
     ossp_data = OSSPMaster(issue_id, name)
     ossp_data.generate_ossp_master(overwrite)
     version_data = Version(issue_id, name)
     version_data.generate_version_data(overwrite)
 
 
 @app.command("generate-report")
 def report(
     reports: List[str] = typer.Argument(None),
-    get_all: bool = typer.Option(False, help="Get all 3 reports"),
     issue_id: int = typer.Option(None, prompt="Enter OSSP id", help="OSSP id"),
     name: str = typer.Option(None, prompt="Enter OSSP name", help="OSSP name"),
     version: str = typer.Option(None, prompt="Enter version", help="Version of OSSP"),
     update_version_file: bool = typer.Option(True, help="Update scores to version file"),
     ):
-    """ Following reports can be generated - scorecard, criticality_score, codeql"""
+    """ Following reports can be generated - scorecard, criticality_score, codeql, sbom"""
+    if platform != "linux":
+        print("[bold red]BeS-dev-kit is compatible"
+              " only with Linux operating systems")
+        raise typer.Exit()
     write_env_vars_file()
     check_if_value_empty()
     set_env_vars()
-    if get_all:
-        assessment_reports = ["scorecard", "criticality_score", "codeql"]
-        for i in assessment_reports:
-            obj = Report(issue_id, name, version, i)
-            obj.main()
-            if update_version_file and i != "codeql":
-                obj.update_version_data()
-        raise typer.Exit()
-    if len(reports) > 3:
-        print("[bold red]Alert! [green]Too many arguments")
-        raise typer.Exit()
-    for i in reports:
-        if i == "scorecard":
-            scorecard_obj = Report(issue_id, name, version, i)
-            scorecard_obj.main()
-            if update_version_file:
-                scorecard_obj.update_version_data()
-        elif i == "criticality_score":
-            criticality_obj = Report(issue_id, name, version, i)
-            criticality_obj.main()
-            if update_version_file:
-                criticality_obj.update_version_data()
-        elif i == "codeql":
-            codeql_obj = Report(issue_id, name, version, i)
-            codeql_obj.main()
-        else:
-            print(f"[red bold]Alert! [yellow]Invalid report [green]{i}")
+    assessment_reports = [
+                'scorecard',
+                'criticality_score',
+                'codeql',
+                'sbom']
+    if reports:
+        if len(reports) > 4:
+            print("[bold red]Alert! [green]Too many arguments")
             raise typer.Exit()
+        # check if given parameters are valid
+        for i in reports:
+            if i.lower() not in assessment_reports:
+                print('[red bold]Alart! [green]'
+                    'Invalid input'
+                    f' [yellow]{i}')
+                sys.exit(1)
+        assessment_reports = reports
+    for i in assessment_reports:
+        print('\n')
+        print("[bold yellow]Generating " + i.lower() + ' report....')
+        obj = Report(issue_id, name, version, i.lower())
+        obj.main()
+        if update_version_file and (i.lower() == "scorecard" or i.lower() == "criticality_score"):
+            obj.update_version_data()
+    raise typer.Exit()
 
 
 @app.command("validate-version-file")
 def version_data_naming_convention_validation(
     issue_id: int = typer.Option(
                         None,
                         prompt="Enter OSSP id",
@@ -171,14 +176,18 @@
     branch: str = typer.Option(
                         None,
                         prompt="Enter branch",
                         help="besecure-osspoi-datastore branch"
                     ),
     ):
     """ Check version details file naming convention """
+    if platform != "linux":
+        print("[bold red]BeS-dev-kit is compatible"
+              " only with Linux operating systems")
+        raise typer.Exit()
     version_data = VersionFileValidate(issue_id, name, namespace, branch)
     version_data.verify_versiondetails_name()
 
 
 @app.command("validate-report-file")
 def report_naming_convention_validation(
     reports: List[str] = typer.Argument(None),
@@ -201,26 +210,33 @@
     branch: str = typer.Option(
                         None,
                         prompt="Enter branch",
                         help="besecure-osspoi-datastore branch"
                     )
 ):
     """ Check report file naming convention """
+    if platform != "linux":
+        print("[bold red]BeS-dev-kit is compatible"
+              " only with Linux operating systems")
+        raise typer.Exit()
     report_list = ["scorecard",
                    "criticality_score",
                    "codeql",
                    'fossology',
                    'sonarqube',
                    'sbom']
     if reports:
+        if len(reports) > 6:
+            print("[bold red]Alert! [green]Too many arguments")
+            raise typer.Exit()
         # check if given parameters are valid
         for i in reports:
             if i.lower() not in report_list:
-                print(f'[red bold]Alart! [green]'\
-                    f'Invalid report name:'\
+                print('[red bold]Alart! [green]'
+                    'Invalid input:'
                     f' [yellow]{i}')
                 sys.exit(1)
         report_list = reports
     obj = ReportFileValidate(
             issue_id,
             name.strip(),
             namespace.strip(),
@@ -241,14 +257,18 @@
     version: str = typer.Option(
                     None,
                     prompt="Enter OSSP Version",
                     help="OSSP Version"
                 ),
     ):
     """Download consolidated assessment report in pdf format"""
+    if platform != "linux":
+        print("[bold red]BeS-dev-kit is compatible"
+              " only with Linux operating systems")
+        raise typer.Exit()
     report = Generate_report()
     report.download_pdf(OSSP_name, version)
 
 @app.callback()
 def main(
     version: Optional[bool] = typer.Option(
         None,
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_ossp_master.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_ossp_master.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_version_data.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/create_version_data.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_assessment.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_assessment.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     utility for generate 
     assessment report summary
 '''
 import os
 from reportlab.platypus import SimpleDocTemplate
 from reportlab.lib.pagesizes import letter
 from rich import print
-from besecure_developer_toolkit.src.risk_summary.Scorecard_report import scorecard
-from besecure_developer_toolkit.src.risk_summary.Sbom_report import sbom
-from besecure_developer_toolkit.src.risk_summary.License_compliance import fossology
-from besecure_developer_toolkit.src.risk_summary.Static_code_analysis import sonarqube
-from besecure_developer_toolkit.src.risk_summary.Objective import objective
+from bes_dev_kit.src.risk_summary.Scorecard_report import scorecard
+from bes_dev_kit.src.risk_summary.Sbom_report import sbom
+from bes_dev_kit.src.risk_summary.License_compliance import fossology
+from bes_dev_kit.src.risk_summary.Static_code_analysis import sonarqube
+from bes_dev_kit.src.risk_summary.Objective import objective
 
 class Generate_report():
 
     def generate_report(self):
         obj = objective(self.OSSP_Name, self.version)
         elem1 = scorecard(self.OSSP_Name, self.version)
         elem2 = sbom(self.OSSP_Name, self.version)
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/License_compliance.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/License_compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rich import print
 from reportlab.platypus import Paragraph, Table
 from reportlab.lib.pagesizes import mm
 from reportlab.platypus import TableStyle
 from reportlab.lib import colors
 from reportlab.lib.colors import HexColor
 from reportlab.lib.styles import ParagraphStyle
-from besecure_developer_toolkit.src.risk_summary.New_line_char import insert_newline_char
+from bes_dev_kit.src.risk_summary.New_line_char import insert_newline_char
 
 def fossology(ossp_name, version):
     resp = getApiData(ossp_name, version)
     data = []
     data.append(["File Name",
                  "License Concluded",
                  "File Copyright Text"])
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/New_line_char.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/New_line_char.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Objective.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Objective.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Sbom_report.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Sbom_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from reportlab.platypus import Paragraph, Table
 from reportlab.lib.pagesizes import mm
 from reportlab.platypus import TableStyle
 from reportlab.lib import colors
 from reportlab.lib.colors import HexColor
 from reportlab.lib.styles import ParagraphStyle
 from rich import print
-from besecure_developer_toolkit.src.risk_summary.New_line_char import insert_newline_char
+from bes_dev_kit.src.risk_summary.New_line_char import insert_newline_char
 
 def sbom(OSSP_Name, version):
     '''return pdf elements of SBOM'''
     try:
         url = 'https://raw.githubusercontent.com/Be-Secure/'\
             'besecure-assessment-datastore/main/'\
             +OSSP_Name+'/'+version+\
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Scorecard_report.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Scorecard_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from reportlab.lib.pagesizes import mm
 from reportlab.platypus import TableStyle
 from reportlab.lib import colors
 from reportlab.lib.colors import HexColor
 from reportlab.lib.styles import ParagraphStyle
 import sys
 from rich import print
-from besecure_developer_toolkit.src.risk_summary.New_line_char import insert_newline_char
+from bes_dev_kit.src.risk_summary.New_line_char import insert_newline_char
 
 def scorecard(ossp_name, version):
     '''return pdf elements of Scorecard'''
     resp = getApiData(ossp_name, version)
     data = []
     data.append(["Name","Score","Reason"])
     for obj in resp["checks"]:
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Static_code_analysis.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/risk_summary/Static_code_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from reportlab.platypus import Paragraph, Table
 from reportlab.lib.pagesizes import mm
 from reportlab.platypus import TableStyle
 from reportlab.lib import colors
 from reportlab.lib.colors import HexColor
 from reportlab.lib.styles import ParagraphStyle
 from rich import print
-from besecure_developer_toolkit.src.risk_summary.New_line_char import insert_newline_char
+from bes_dev_kit.src.risk_summary.New_line_char import insert_newline_char
 
 def sonarqube(OSSP_Name, version):
     '''return pdf elements of sonarqube'''
     try:
         url = 'https://raw.githubusercontent.com/'\
             'Be-Secure/'\
             'besecure-assessment-datastore/main/'\
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_report_file.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_report_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''report-file-validate module'''
 import json
 import sys
 import requests
 from urllib.request import urlopen
 from urllib.error import HTTPError
-from besecure_developer_toolkit.src.validate_version_file import VersionFileValidate
-from besecure_developer_toolkit.src.create_ossp_master import OSSPMaster
+from bes_dev_kit.src.validate_version_file import VersionFileValidate
+from bes_dev_kit.src.create_ossp_master import OSSPMaster
 from rich import print
 
 class ReportFileValidate():
     """Report files naming convention validation class"""
 
     def __init__(
             self,
```

### Comparing `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_version_file.py` & `besecure_developer_toolkit-0.0.6/bes_dev_kit/src/validate_version_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Version details file validate"""
 import sys
 import json
 from urllib.error import HTTPError
 from urllib.request import urlopen
 from rich import print
-from besecure_developer_toolkit.src.create_ossp_master import OSSPMaster
+from bes_dev_kit.src.create_ossp_master import OSSPMaster
 
 
 class VersionFileValidate():
     """version details file naming convention validation class"""
 
     def __init__(self, issue_id: int, name: str, namespace: str, branch: str):
         self.issue_id = issue_id
```

### Comparing `besecure_developer_toolkit-0.0.5/pyproject.toml` & `besecure_developer_toolkit-0.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "besecure-developer-toolkit"
-version = "0.0.5"
+version = "0.0.6"
 description = "cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse)."
 authors = ["asa1997 <arunsureshampadath@gmail.com>"]
 readme = "README.md"
-packages = [{include = "besecure_developer_toolkit"}]
+packages = [{include = "bes_dev_kit"}]
 
 [tool.poetry.scripts]
-bes-dev-kit = "besecure_developer_toolkit.__main__:cli.app"
+besecure-developer-toolkit = "bes_dev_kit.__main__:cli.app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 pytest = "^7.3.0"
 requests = "^2.29.0"
 reportlab = "^3.6.8"
+criticality-score = "^1.0.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `besecure_developer_toolkit-0.0.5/PKG-INFO` & `besecure_developer_toolkit-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: besecure-developer-toolkit
-Version: 0.0.5
+Version: 0.0.6
 Summary: cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 Author: asa1997
 Author-email: arunsureshampadath@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: criticality-score (>=1.0.8,<2.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: reportlab (>=3.6.8,<4.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# Be-Secure Developer Toolkit (bes-dev-kit)
+# BeS-dev-kit
 
-bes-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
+BeS-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 
 # Pre-requisites
 
 1. Python 3.10
 2. pip
 3. Github personal access token
 
 # Installation
 
-`$ python3 -m pip install besecure-developer-toolkit`
+`$ python3 -m pip install bes-dev-kit`
 
 # Usage
 
 If you are running the command for the first time, you will be prompted to provide the complete path to your `besecure-osspoi-datastore` and `besecure-assessment-datastore` and your `personal access token`
 
 ### Generate Metadata
 
@@ -46,15 +47,17 @@
 
 `Note: For the first time use this command will ask for three extra inputs - OSSPOI_DIR: location of besecure-osspoi-datastore in local system, ASSESSMENT_DIR: location of besecure-assessment-datastore, GITHUB_AUTH_TOKEN`
 
 ![metadata first time](docs/generate-metadata-first-time.jpg)
 
 ### Generate Reports
 
-`$ bes-dev-kit generate-report <report name>`
+`$ bes-dev-kit generate-report` -  generate all reports (scorecard, sciticality_score, codeql, sbom)
+
+`$ bes-dev-kit generate-report < report name > ... < report name >` - generate specific report
 
 ![generate report](docs/generate-report.gif)
 
 `<report name> - scorecard, codeql, criticality_score`
 
 For more options use `--help` at end.
```

