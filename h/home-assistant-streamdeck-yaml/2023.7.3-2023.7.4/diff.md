# Comparing `tmp/home_assistant_streamdeck_yaml-2023.7.3.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.3.tar", last modified: Wed Jul  5 20:54:19 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.4.tar", last modified: Fri Jul  7 07:20:36 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.7.3.tar` & `home_assistant_streamdeck_yaml-2023.7.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.400606 home_assistant_streamdeck_yaml-2023.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.396606 home_assistant_streamdeck_yaml-2023.7.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.396606 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-05 20:54:19.400606 home_assistant_streamdeck_yaml-2023.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.396606 home_assistant_streamdeck_yaml-2023.7.3/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.396606 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 20:54:19.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    60223 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:54:19.400606 home_assistant_streamdeck_yaml-2023.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.400606 home_assistant_streamdeck_yaml-2023.7.3/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:54:19.400606 home_assistant_streamdeck_yaml-2023.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-05 20:53:57.000000 home_assistant_streamdeck_yaml-2023.7.3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60076 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.github/release.py` & `home_assistant_streamdeck_yaml-2023.7.4/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.gitignore` & `home_assistant_streamdeck_yaml-2023.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/Dockerfile` & `home_assistant_streamdeck_yaml-2023.7.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/LICENSE` & `home_assistant_streamdeck_yaml-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/README.md` & `home_assistant_streamdeck_yaml-2023.7.4/README.md`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.7.4/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.7.4/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/configuration.yaml` & `home_assistant_streamdeck_yaml-2023.7.4/configuration.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/docker-compose.yaml` & `home_assistant_streamdeck_yaml-2023.7.4/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1276,17 +1276,14 @@
     if icon_filename is not None:
         icon_path = Path(icon_filename)
         path = icon_path if icon_path.is_absolute() else ASSETS_PATH / icon_path
         icon = Image.open(path)
         # Convert to RGB if needed
         if icon.mode != "RGB":
             icon = icon.convert("RGB")
-        if icon.size != size:
-            # Resize image to the correct resolution if needed
-            icon = icon.resize(size, Image.ANTIALIAS)
         return icon
     if icon_mdi is not None:
         assert icon_mdi_margin is not None
         filename_svg = _download_and_save_mdi(icon_mdi)
         return _convert_svg_to_png(
             filename_svg=filename_svg,
             color=icon_mdi_color,
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.7.4/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/tests/state.json` & `home_assistant_streamdeck_yaml-2023.7.4/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.7.4/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.3/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.7.4/tests/test_examples.py`

 * *Files identical despite different names*

