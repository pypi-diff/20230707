# Comparing `tmp/reps_new-0.2.0.tar.gz` & `tmp/reps_new-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reps_new-0.2.0.tar", max compression
+gzip compressed data, was "reps_new-0.3.0.tar", max compression
```

## Comparing `reps_new-0.2.0.tar` & `reps_new-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.2.0/LICENSE
--rw-r--r--   0        0        0     1008 2023-07-06 19:30:10.728667 reps_new-0.2.0/README.md
--rw-r--r--   0        0        0      550 2023-07-06 20:48:57.587349 reps_new-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.2.0/reps/__init__.py
--rw-r--r--   0        0        0     1556 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/console.py
--rw-r--r--   0        0        0     2915 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/hooks.py
--rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.2.0/reps/templates/base/cookiecutter.json
--rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.2.0/reps/templates/base/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
--rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
--rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2023-06-26 17:21:43.703711 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
--rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
--rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
--rw-r--r--   0        0        0      958 2023-07-06 14:55:10.046283 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
--rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
--rw-r--r--   0        0        0     1732 2023-06-27 15:07:07.525755 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
--rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
--rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
--rw-r--r--   0        0        0     1120 2023-07-06 19:29:54.578671 reps_new-0.2.0/reps/templates/python/cookiecutter.json
--rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/hooks/post_gen_project.py
--rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/hooks/pre_gen_project.py
--rw-r--r--   0        0        0    16185 2023-07-06 19:30:10.728667 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
--rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 20:18:22.754371 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/src/{{cookiecutter.__package_name}}/__init__.py
--rw-r--r--   0        0        0     1175 2023-07-06 20:25:24.507743 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
--rw-r--r--   0        0        0      570 2023-07-05 13:50:01.939464 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
--rw-r--r--   0        0        0      512 2023-07-06 19:29:54.578671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
--rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
--rw-r--r--   0        0        0      993 2023-07-06 20:28:44.257688 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
--rw-r--r--   0        0        0      518 2023-07-04 19:06:10.348905 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile
--rw-r--r--   0        0        0     1306 2023-07-06 20:23:53.167770 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile
--rw-r--r--   0        0        0       22 2023-07-04 19:26:34.218564 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/requirements.in
--rw-r--r--   0        0        0      701 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
--rwxr-xr-x   0        0        0      179 2023-07-06 19:29:56.058671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/poetry-setup
--rwxr-xr-x   0        0        0      658 2023-07-06 20:36:16.647561 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
--rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
--rw-r--r--   0        0        0      164 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
--rw-r--r--   0        0        0      957 2023-07-06 19:30:10.738667 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 reps_new-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1008 2023-07-06 19:30:10.728667 reps_new-0.3.0/README.md
+-rw-r--r--   0        0        0      567 2023-07-07 14:17:15.744508 reps_new-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.3.0/reps/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-06 19:29:55.318671 reps_new-0.3.0/reps/console.py
+-rw-r--r--   0        0        0     3233 2023-07-07 14:13:20.518572 reps_new-0.3.0/reps/hooks.py
+-rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.3.0/reps/templates/base/cookiecutter.json
+-rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.3.0/reps/templates/base/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
+-rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
+-rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 17:21:43.703711 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
+-rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
+-rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
+-rw-r--r--   0        0        0      958 2023-07-06 14:55:10.046283 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
+-rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
+-rw-r--r--   0        0        0     1732 2023-06-27 15:07:07.525755 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
+-rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
+-rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
+-rw-r--r--   0        0        0     1120 2023-07-06 19:29:54.578671 reps_new-0.3.0/reps/templates/python/cookiecutter.json
+-rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.3.0/reps/templates/python/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.3.0/reps/templates/python/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0    16185 2023-07-06 19:30:10.728667 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
+-rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:18:22.754371 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/src/{{cookiecutter.__package_name}}/__init__.py
+-rw-r--r--   0        0        0     1175 2023-07-06 20:25:24.507743 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
+-rw-r--r--   0        0        0      570 2023-07-05 13:50:01.939464 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
+-rw-r--r--   0        0        0      512 2023-07-06 19:29:54.578671 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
+-rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
+-rw-r--r--   0        0        0      993 2023-07-06 20:28:44.257688 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
+-rw-r--r--   0        0        0      518 2023-07-04 19:06:10.348905 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile
+-rw-r--r--   0        0        0     1306 2023-07-06 20:23:53.167770 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile
+-rw-r--r--   0        0        0       22 2023-07-04 19:26:34.218564 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/requirements.in
+-rw-r--r--   0        0        0      701 2023-07-06 19:29:55.318671 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
+-rwxr-xr-x   0        0        0      179 2023-07-06 19:29:56.058671 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/poetry-setup
+-rwxr-xr-x   0        0        0      658 2023-07-06 20:36:16.647561 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
+-rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
+-rw-r--r--   0        0        0      164 2023-07-06 19:29:55.318671 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:30:10.738667 reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
+-rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 reps_new-0.3.0/PKG-INFO
```

### Comparing `reps_new-0.2.0/LICENSE` & `reps_new-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/README.md` & `reps_new-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/pyproject.toml` & `reps_new-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "reps-new"
-version = "0.2.0"
+version = "0.3.0"
 description = "Mozilla Release Engineering Project Standard"
 authors = ["Mozilla Release Engineering <release@mozilla.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 packages = [{ include = "reps" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 cookiecutter = "^2.1.1"
 pre-commit = "^3.3.3"
 taskcluster-taskgraph = "^5.4.0"
 pyyaml = "^6.0"
 pip-tools = "^6.14.0"
+halo = "^0.0.31"
 
 [tool.poetry.scripts]
 reps-new = "reps.console:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reps_new-0.2.0/reps/console.py` & `reps_new-0.3.0/reps/console.py`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/hooks.py` & `reps_new-0.3.0/reps/hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import subprocess
 from collections import defaultdict
 from pathlib import Path
+import sys
 
 import yaml
+from halo import Halo
 
 from reps.console import command_new
 
 
 HOOKS = defaultdict(list)
 
 
@@ -16,21 +18,30 @@
         return func
 
     return wrapper
 
 
 def run_hooks(group, items):
     for hook_fn in HOOKS[group]:
-        print(f"running {group} hook '{hook_fn.__name__}'")
-        hook_fn(items)
+        with Halo(f"running {hook_fn.__name__}") as spinner:
+            hook_fn(items)
+            spinner.succeed()
 
 
 def run(cmd, **kwargs):
     kwargs.setdefault("check", True)
-    subprocess.run(cmd, **kwargs)
+    kwargs.setdefault("stdout", subprocess.PIPE)
+    kwargs.setdefault("stderr", subprocess.STDOUT)
+    try:
+        subprocess.run(cmd, **kwargs)
+    except subprocess.CalledProcessError as e:
+        print("+ command failed: {' '.join(cmd)}")
+        print(e.output)
+        raise
+
 
 
 @hook("pre-gen-py")
 def base_init(items):
     """Generate the 'base' template first."""
     if "_copy_without_render" in items:
         del items["_copy_without_render"]
```

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py` & `reps_new-0.3.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/cookiecutter.json` & `reps_new-0.3.0/reps/templates/python/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini` & `reps_new-0.3.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `reps_new-0.2.0/PKG-INFO` & `reps_new-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: reps-new
-Version: 0.2.0
+Version: 0.3.0
 Summary: Mozilla Release Engineering Project Standard
 License: MPL-2.0
 Author: Mozilla Release Engineering
 Author-email: release@mozilla.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
+Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: pip-tools (>=6.14.0,<7.0.0)
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: taskcluster-taskgraph (>=5.4.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Release Engineering Project Standard
```

