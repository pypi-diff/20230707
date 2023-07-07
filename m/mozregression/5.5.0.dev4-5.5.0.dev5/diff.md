# Comparing `tmp/mozregression-5.5.0.dev4.tar.gz` & `tmp/mozregression-5.5.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.5.0.dev4.tar", last modified: Thu Jun 15 13:21:33 2023, max compression
+gzip compressed data, was "mozregression-5.5.0.dev5.tar", last modified: Mon Jun 19 19:34:56 2023, max compression
```

## Comparing `mozregression-5.5.0.dev4.tar` & `mozregression-5.5.0.dev5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:21:33.653942 mozregression-5.5.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:21:33.645942 mozregression-5.5.0.dev4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:21:33.645942 mozregression-5.5.0.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-15 13:21:33.653942 mozregression-5.5.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:21:33.653942 mozregression-5.5.0.dev4/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:21:33.653942 mozregression-5.5.0.dev4/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 13:21:33.000000 mozregression-5.5.0.dev4/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:21:33.653942 mozregression-5.5.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-15 13:20:20.000000 mozregression-5.5.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:34:56.301314 mozregression-5.5.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:34:56.297314 mozregression-5.5.0.dev5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:34:56.297314 mozregression-5.5.0.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 19:34:56.301314 mozregression-5.5.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:34:56.301314 mozregression-5.5.0.dev5/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:34:56.301314 mozregression-5.5.0.dev5/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 19:34:56.000000 mozregression-5.5.0.dev5/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:34:56.301314 mozregression-5.5.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-19 19:33:45.000000 mozregression-5.5.0.dev5/setup.py
```

### Comparing `mozregression-5.5.0.dev4/.github/workflows/build.yml` & `mozregression-5.5.0.dev5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/.github/workflows/compile-requirements.yml` & `mozregression-5.5.0.dev5/.github/workflows/compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/.github/workflows/deploy-gui.yml` & `mozregression-5.5.0.dev5/.github/workflows/deploy-gui.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/.github/workflows/deploy.yml` & `mozregression-5.5.0.dev5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/.github/workflows/run-compile-requirements.yml` & `mozregression-5.5.0.dev5/.github/workflows/run-compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/LICENSE` & `mozregression-5.5.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/PKG-INFO` & `mozregression-5.5.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.0.dev4
+Version: 5.5.0.dev5
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.5.0.dev4/README.md` & `mozregression-5.5.0.dev5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,9 +126,9 @@
 
 Uploading the signed artifacts is a manual process at this time. To sign and notarize a macOS release, follow these steps:
 
 - Copy the signing manifest output from the build job.
 - Create a pull request to update `signing-manifests/mozregression-macOS.yml` in the [adhoc-signing](https://github.com/mozilla-releng/adhoc-signing) repo with those changes.
 - Wait for pull request to be merged, and the signing task to finish.
 - After the signing task is finished, download `mozregression-gui-app-bundle.tar.gz` and extract it in `gui/dist`.
-- Run bin/dmgbuild.
+- Run `./bin/dmgbuild`.
 - Upload new dmg artifact (gui/dist/mozregression-gui.dmg) to the corresponding release.
```

### Comparing `mozregression-5.5.0.dev4/mozregression/approx_persist.py` & `mozregression-5.5.0.dev5/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/bisector.py` & `mozregression-5.5.0.dev5/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/branches.py` & `mozregression-5.5.0.dev5/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/bugzilla.py` & `mozregression-5.5.0.dev5/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/build_info.py` & `mozregression-5.5.0.dev5/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/build_range.py` & `mozregression-5.5.0.dev5/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/class_registry.py` & `mozregression-5.5.0.dev5/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/cli.py` & `mozregression-5.5.0.dev5/mozregression/cli.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/config.py` & `mozregression-5.5.0.dev5/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/dates.py` & `mozregression-5.5.0.dev5/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/download_manager.py` & `mozregression-5.5.0.dev5/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/errors.py` & `mozregression-5.5.0.dev5/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/fetch_build_info.py` & `mozregression-5.5.0.dev5/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/fetch_configs.py` & `mozregression-5.5.0.dev5/mozregression/fetch_configs.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/history.py` & `mozregression-5.5.0.dev5/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/json_pushes.py` & `mozregression-5.5.0.dev5/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/launchers.py` & `mozregression-5.5.0.dev5/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/log.py` & `mozregression-5.5.0.dev5/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/mach_interface.py` & `mozregression-5.5.0.dev5/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/main.py` & `mozregression-5.5.0.dev5/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/metrics.yaml` & `mozregression-5.5.0.dev5/mozregression/metrics.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/network.py` & `mozregression-5.5.0.dev5/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/persist_limit.py` & `mozregression-5.5.0.dev5/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/pings.yaml` & `mozregression-5.5.0.dev5/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/releases.py` & `mozregression-5.5.0.dev5/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/tc_authenticate.py` & `mozregression-5.5.0.dev5/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/telemetry.py` & `mozregression-5.5.0.dev5/mozregression/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if mozinfo.os == "mac":
         try:
             # Fetch the "release" from tuple containing macOS version information.
             # See https://docs.python.org/3/library/platform.html#macos-platform.
             info["mac_version"] = platform.mac_ver()[0]
         except (AttributeError, IndexError):
             info["mac_version"] = UNKNOWN
-    elif mozinfo.os == "windows":
+    elif mozinfo.os == "win":
         try:
             # Fetch "version" from tuple containing Windows version information.
             # See https://docs.python.org/3/library/platform.html#windows-platform.
             info["windows_version"] = platform.win32_ver()[1]
         except (AttributeError, IndexError):
             info["windows_version"] = UNKNOWN
     elif mozinfo.os == "linux":
```

### Comparing `mozregression-5.5.0.dev4/mozregression/tempdir.py` & `mozregression-5.5.0.dev5/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression/test_runner.py` & `mozregression-5.5.0.dev5/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/mozregression.egg-info/PKG-INFO` & `mozregression-5.5.0.dev5/mozregression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.0.dev4
+Version: 5.5.0.dev5
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.5.0.dev4/mozregression.egg-info/SOURCES.txt` & `mozregression-5.5.0.dev5/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/pyproject.toml` & `mozregression-5.5.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev4/setup.py` & `mozregression-5.5.0.dev5/setup.py`

 * *Files identical despite different names*

