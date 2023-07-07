# Comparing `tmp/make_argocd_fly-0.0.6.tar.gz` & `tmp/make_argocd_fly-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.6.tar", last modified: Thu Jul  6 05:25:42 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.7.tar", last modified: Fri Jul  7 12:50:03 2023, max compression
```

## Comparing `make_argocd_fly-0.0.6.tar` & `make_argocd_fly-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.6/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.6/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2303 2023-07-06 05:25:22.000000 make_argocd_fly-0.0.6/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.6/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.6/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.6/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.6/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.6/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.6/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-06 05:21:09.000000 make_argocd_fly-0.0.6/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.6/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.7/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.7/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3361 2023-07-07 12:47:38.000000 make_argocd_fly-0.0.7/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.7/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      808 2023-07-07 12:36:36.000000 make_argocd_fly-0.0.7/make_argocd_fly/application.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.7/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.7/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5938 2023-07-07 10:19:53.000000 make_argocd_fly-0.0.7/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      688 2023-07-06 21:07:13.000000 make_argocd_fly-0.0.7/make_argocd_fly/renderer.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4255 2023-07-07 09:12:59.000000 make_argocd_fly-0.0.7/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      930 2023-07-06 18:44:06.000000 make_argocd_fly-0.0.7/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      522 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-07 12:49:49.000000 make_argocd_fly-0.0.7/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.7/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/setup.cfg
```

### Comparing `make_argocd_fly-0.0.6/LICENSE` & `make_argocd_fly-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.6/PKG-INFO` & `make_argocd_fly-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,74 @@
-Metadata-Version: 2.1
-Name: make_argocd_fly
-Version: 0.0.6
-Summary: A project to generate ArgoCD application resources
-Author-email: Andrei Lapin <karandash8@gmail.com>
-License: GPLv3+
-Keywords: argocd,kustomize,jinja2
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Description
-A project to generate on the user side per environemnt Kubernetes manifests that can be deployed with ArgoCD.
+A tool to generate on the user side per environemnt Kubernetes manifests that can be deployed with ArgoCD.
+
+ArcoCD resources of type `Application` are generated automatically based on the provided configuration.
 
 ## Motivation
 Manifests that are written in kustomize/helm/jsonnet might easily become hard to read and debug. The development lifecycle becomes longer when after each change you need to commit, wait for ArgoCD to pick it up and deploy it. Only after that you see the actual end manifest in ArcoCD UI.
 
 With this tool you can quickly render jinja2/kustomize files, run yaml linter and continuer development.
 
 ## Benefits
+- Application resources are generated automatically
 - Easier to grasp end manifests
 - Shared variables between applications
 
 ## Configuration
 ### config.yml
 Expected file structure
 ```
 config:
   source_dir: source
   output_dir: output
   tmp_dir: .tmp
 
 envs:
-  - dev
-  - stage
-  - prod
-
+  dev:
+    apps:
+      bootstrap: {}
+      app_1:
+        app_deployer: bootstrap
+        project: default
+        destination_namespace: namespace_1
+      app_2:
+        app_deployer: bootstrap
+        project: default
+        destination_namespace: namespace_2
+    params:
+      argocd_namespace: argocd
+      repo_url: url
+      target_revision: revision
+      api_server: management-api-server
+  prod:
+    apps:
+      app_1:
+        app_deployer: bootstrap
+        project: default
+        destination_namespace: namespace_1
 vars:
   var_1:
     var_2: value_2
   var_3: value_3
 ```
 
-With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
+With such configuration file you can have kustomize overlays for `dev/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
 
 ## Caveats
 ### Currently supported directory structure
 ```
 repo
   source
     app_1
       base
         yaml.yml(.j2)
         kustomization.yml(.j2)
       dev
         yaml.yml(.j2)
         kustomization.yml(.j2)
-      stage
-        yaml.yml(.j2)
-        kustomization.yml(.j2)
       prod
         yaml.yml(.j2)
         kustomization.yml(.j2)
     app_2
       yaml.yml(.j2)
       kustomization.yml(.j2)
     app_3
@@ -73,14 +79,30 @@
 Files referenced in the `resources` section shall be named after Kubernetes resource types with lower case letters as a single word. Example:
 
 ```
 resources:
   - deployment.yml
   - serviceaccount.yml
 ```
+### Initial app-of-apps application
+`bootstrap` application shall be deployed externally
+
+### Multiple ArgoCD deployments referencing the same repo
+If there is an argocd deployment per environment then app_deployer applications shall have different names for different environments
+
+### Variable names
+The folloving variable names are resenved:
+- _application_name
+- _argocd_namespace
+- _project
+- _repo_url
+- _target_revision
+- _path
+- _api_server
+- _destination_namespace
 
 ## For developers
 ### Build instructions
 https://setuptools.pypa.io/en/latest/userguide/quickstart.html
 https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 https://setuptools.pypa.io/en/latest/userguide/datafiles.html
 https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

### Comparing `make_argocd_fly-0.0.6/make_argocd_fly/config.py` & `make_argocd_fly-0.0.7/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.6/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.7/make_argocd_fly/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,126 @@
 import logging
 import logging.config
 import yaml
 import os
 import argparse
 import subprocess
 import shutil
-from jinja2 import Environment, FileSystemLoader
 
 from make_argocd_fly.config import read_config, Config
 from make_argocd_fly.utils import extract_dir_rel_path, multi_resource_parser, resource_parser
 from make_argocd_fly.resource import build_resource_viewer, build_resource_writer, ResourceViewer, ResourceWriter
+from make_argocd_fly.application import generate_application
 
 LOG_CONFIG_FILE = 'log_config.yml'
 CONFIG_FILE = 'config.yml'
 
 try:
   with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), LOG_CONFIG_FILE)) as f:
     yaml_config = yaml.safe_load(f.read())
     logging.config.dictConfig(yaml_config)
 except FileNotFoundError:
   logging.basicConfig(level='DEBUG')
 
 log = logging.getLogger(__name__)
 
 
-def step_1(viewer: ResourceViewer, writer: ResourceWriter, config: Config) -> None:
-  # step 1: copy .yml files, render .j2 files
-  environment = Environment(loader=FileSystemLoader(viewer.root_element_abs_path))
-  apps = [app for app in viewer.get_dirs_children(depth=1)]
-  for app in apps:
-    yml_children = viewer.get_child(app.name).get_files_children('.yml$')
-    j2_children = viewer.get_child(app.name).get_files_children('.j2$')
-    log.debug('app: {}, yml files: {}, j2_files: {}'.format(app.name, [child.element_rel_path for child in yml_children], [child.element_rel_path for child in j2_children]))
-
-    for yml_child in yml_children:
-      dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
-      for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
-        writer.update_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
-
-    for j2_child in j2_children:
-      dir_rel_path = extract_dir_rel_path(j2_child.element_rel_path)
-      template = environment.get_template(j2_child.element_rel_path)
-      for resource_kind, resource_name, resource_yml in multi_resource_parser(template.render(config.vars)):
-        writer.update_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
-
-def step_2(viewer: ResourceViewer, writer: ResourceWriter, config: Config) -> None:
-  # step 2: run kustomize
-  apps = [app for app in viewer.get_dirs_children(depth=1)]
-  for env in config.envs:
-    for app in apps:
-      env_child = app.get_child(env)
+def find_app_in_envs(target_app_name: str, envs: dict) -> str:
+  for env_name, env_data in envs.items():
+    if target_app_name in env_data['apps'].keys():
+      return env_name
+
+# TODO: rework this nonsense
+def run(viewer: ResourceViewer, writer: ResourceWriter, config: Config) -> None:
+  # write apps in a tmp dir and run kustomize
+  for env_name, env_data in config.envs.items():
+    if os.path.exists(config.config['tmp_dir']):
+      shutil.rmtree(config.config['tmp_dir'])
+    tmp_writer = build_resource_writer(config.config['tmp_dir'], None)
+
+    for app_name in env_data['apps'].keys():
+      app = viewer.get_child(app_name)
+      if not app:
+        continue
+
+      yml_children = app.get_files_children('.yml$')
+      for yml_child in yml_children:
+        dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
+        for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
+          tmp_writer.store_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
+      tmp_writer.write_resources()
+
+      env_child = app.get_child(env_name)
       if env_child:
         yml_child = env_child.get_child('kustomization.yml')
         if yml_child:
           dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
           process = subprocess.Popen(['kubectl', 'kustomize',
-                                      os.path.join(viewer.root_element_abs_path, dir_rel_path)],
+                                      os.path.join(viewer.tmp_dir_abs_path, dir_rel_path)],
                                       stdout=subprocess.PIPE,stderr=subprocess.PIPE,
                                       universal_newlines=True)
-          stdout, stderr = process.communicate()
+          stdout, _ = process.communicate()
 
           for resource_kind, resource_name, resource_yml in multi_resource_parser(stdout):
-            writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
+            writer.store_resource(os.path.join(env_name, app.name), resource_kind, resource_name, resource_yml)
           log.debug(stdout)
       else:
         yml_child = app.get_child('kustomization.yml')
         if yml_child:
           dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
           process = subprocess.Popen(['kubectl', 'kustomize',
-                                      os.path.join(viewer.root_element_abs_path, dir_rel_path)],
+                                      os.path.join(viewer.tmp_dir_abs_path, dir_rel_path)],
                                       stdout=subprocess.PIPE,stderr=subprocess.PIPE,
                                       universal_newlines=True)
           stdout, _ = process.communicate()
 
           for resource_kind, resource_name, resource_yml in multi_resource_parser(stdout):
-            writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
+            writer.store_resource(os.path.join(env_name, app.name), resource_kind, resource_name, resource_yml)
           log.debug(stdout)
         else:
           yml_children = app.get_files_children('.yml$')
 
           for yml_child in yml_children:
             dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
             for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
-              writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
+              writer.store_resource(os.path.join(env_name, app.name), resource_kind, resource_name, resource_yml)
+
+  # generate Application resources
+  for env_name, env_data in config.envs.items():
+    for app_name, app_data in env_data['apps'].items():
+      if app_data:
+        template_vars = config.vars
+        full_app_name = '-'.join([app_name, env_name]).replace('_', '-')
+        template_vars['_application_name'] = full_app_name
+        template_vars['_argocd_namespace'] = env_data['params']['argocd_namespace']
+        template_vars['_project'] = app_data['project']
+        template_vars['_repo_url'] = env_data['params']['repo_url']
+        template_vars['_target_revision'] = env_data['params']['target_revision']
+        template_vars['_path'] = os.path.join(os.path.basename(config.config['output_dir']), env_name, app_name)
+        template_vars['_api_server'] = env_data['params']['api_server']
+        template_vars['_destination_namespace'] = app_data['destination_namespace']
+
+        content = generate_application(template_vars)
+
+        app_deployer_env = find_app_in_envs(app_data['app_deployer'], config.envs)
+        writer.store_resource(os.path.join(app_deployer_env, app_data['app_deployer']), 'Application', full_app_name, content)
 
 def main() -> None:
   parser = argparse.ArgumentParser(description='Render ArgoCD Applications.')
   parser.add_argument('--env', type=str, default=None, help='Environment to render')
   parser.add_argument('--app', type=str, default=None, help='Application to render')
   parser.add_argument('--root-dir', type=str, default=os.getcwd(), help='Root directory')
   parser.add_argument('--config-file', type=str, default=CONFIG_FILE, help='Configuration file')
   args = parser.parse_args()
 
   root_dir = args.root_dir
   log.debug('Root directory path: {}'.format(root_dir))
 
   config = read_config(root_dir, args.config_file)
-  if os.path.exists(config.config['tmp_dir']):
-    shutil.rmtree(config.config['tmp_dir'])
+  source_viewer = build_resource_viewer(config.config['source_dir'], config.config['tmp_dir'], config.vars, args.app)
+  output_writer = build_resource_writer(config.config['output_dir'], args.env)
+
+  run(source_viewer, output_writer, config)
 
-  source_viewer = build_resource_viewer(config.config['source_dir'], args.app)
-  tmp_writer = build_resource_writer(config.config['tmp_dir'], config.envs, args.env)
-  step_1(source_viewer, tmp_writer, config)
-  tmp_writer.write_updates()
-
-  tmp_viewer = build_resource_viewer(config.config['tmp_dir'], args.app)
-  output_writer = build_resource_writer(config.config['output_dir'], config.envs, args.env)
-  step_2(tmp_viewer, output_writer, config)
-  #TODO: clean only filtered apps/envs
   if os.path.exists(config.config['output_dir']):
     shutil.rmtree(config.config['output_dir'])
-  output_writer.write_updates()
+  output_writer.write_resources()
```

### Comparing `make_argocd_fly-0.0.6/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.7/make_argocd_fly/resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 import logging
 import os
 import re
 
 from make_argocd_fly.utils import resource_parser, multi_resource_parser, extract_dir_rel_path
+from make_argocd_fly.renderer import AbstractRenderer, JinjaRenderer
 
 log = logging.getLogger(__name__)
 
 
 class ResourceViewer:
-  def __init__(self, root_element_abs_path: str) -> None:
+  def __init__(self, root_element_abs_path: str, tmp_dir_abs_path: str, renderer: AbstractRenderer, template_vars: dict) -> None:
     if not os.path.exists(root_element_abs_path):
       log.error('Path does not exist {}'.format(root_element_abs_path))
       raise Exception
 
     self.root_element_abs_path = root_element_abs_path
+    self.tmp_dir_abs_path = tmp_dir_abs_path
+    self.renderer = renderer
+    self.template_vars = template_vars
     self.element_rel_path = None
     self.name = None
     self.is_dir = None
     self.content = None
     self.children = []
 
-  def build(self, element_rel_path:str, is_root_element: bool = True) -> None:
+  def build(self, element_rel_path:str, is_root_element: bool = False) -> None:
     self.element_rel_path = element_rel_path
     if is_root_element:
       self.name = os.path.basename(self.root_element_abs_path)
     else:
       self.name = os.path.basename(element_rel_path)
 
     path = os.path.join(self.root_element_abs_path, element_rel_path)
     self.is_dir = os.path.isdir(path)
     if self.is_dir:
       for child_name in os.listdir(path):
-        child = ResourceViewer(self.root_element_abs_path)
-        child.build(os.path.join(element_rel_path, child_name), is_root_element=False)
+        child = ResourceViewer(self.root_element_abs_path, self.tmp_dir_abs_path, self.renderer, self.template_vars)
+        child.build(os.path.join(element_rel_path, child_name))
         self.children.append(child)
     else:
       with open(path) as f:
-        self.content = ''.join(f.readlines())
+        content = ''.join(f.readlines())
+
+        if self.name.endswith('.j2'):
+          self.content = self.renderer.render(content, self.template_vars)
+          self.name = self.name[:-3]
+        else:
+          self.content = content
 
     log.debug('Created element ({})'.format(self))
 
   def get_child(self, name: str) -> 'ResourceViewer':
     for child in self.children:
       if child.name == name:
         return child
@@ -70,51 +80,43 @@
 
     return dirs
 
   def __str__(self) -> str:
     return 'name: {}, is_dir: {}, element_rel_path: {}'.format(self.name, self.is_dir, self.element_rel_path)
 
 
+def build_resource_viewer(root_element_abs_path: str, tmp_dir_abs_path: str, template_vars: dict, filter: str = None) -> ResourceViewer:
+  source_viewer = ResourceViewer(root_element_abs_path, tmp_dir_abs_path, JinjaRenderer(), template_vars)
+  source_viewer.build('.', is_root_element=True)
+
+  return source_viewer
+
+
 class ResourceWriter:
-  def __init__(self, output_dir_abs_path: str, envs: list, existing_resources: list = None) -> None:
+  def __init__(self, output_dir_abs_path: str) -> None:
     self.output_dir_abs_path = output_dir_abs_path
-    self.envs = envs
-    self.existing_resources = existing_resources
+    self.resources = {}
 
-  def update_resource(self, dir_rel_path: str, resource_kind: str, resource_name: str, resource_yml: str) -> None:
-    self.existing_resources[(dir_rel_path, resource_kind, resource_name)] = resource_yml
+  def store_resource(self, dir_rel_path: str, resource_kind: str, resource_name: str, resource_yml: str) -> None:
+    self.resources[(dir_rel_path, resource_kind, resource_name)] = resource_yml
 
-  def write_updates(self) -> None:
-    for (dir_rel_path, resource_kind, _), resource_yml in self.existing_resources.items():
-      self.write_file(dir_rel_path, resource_kind + '.yml', resource_yml)
+  def write_resources(self) -> None:
+    for (dir_rel_path, resource_kind, _), resource_yml in self.resources.items():
+      self._write_file_resource(dir_rel_path, resource_kind + '.yml', resource_yml)
 
-  def write_file(self, dir_rel_path: str, filename: str, resource_yml: str) -> None:
+  def _write_file_resource(self, dir_rel_path: str, filename: str, resource_yml: str) -> None:
     path = os.path.join(self.output_dir_abs_path, dir_rel_path)
     os.makedirs(path, exist_ok=True)
 
     if not os.path.exists(os.path.join(path, filename.lower())):
       with open(os.path.join(path, filename.lower()), 'w') as f:
         f.write(resource_yml)
         f.write('\n')
     else:
       with open(os.path.join(path, filename.lower()), 'a') as f:
         f.write('---\n')
         f.write(resource_yml)
         f.write('\n')
 
 
-def build_resource_viewer(root_element_abs_path: str, filter: str = None) -> ResourceViewer:
-  source_viewer = ResourceViewer(root_element_abs_path)
-  source_viewer.build('.')
-
-  return source_viewer
-
-def build_resource_writer(output_dir_abs_path: str, envs: list, filter: str = None) -> ResourceWriter:
-  existing_resources = {}
-
-  if os.path.exists(output_dir_abs_path):
-    output_viewer = build_resource_viewer(output_dir_abs_path)
-    yml_children = output_viewer.get_files_children('.yml$')
-    existing_resources = {(extract_dir_rel_path(yml_child.element_rel_path), resource_kind, resource_name): resource_yml
-                         for yml_child in yml_children for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content)}
-
-  return ResourceWriter(output_dir_abs_path, envs, existing_resources)
+def build_resource_writer(output_dir_abs_path: str, filter: str = None) -> ResourceWriter:
+  return ResourceWriter(output_dir_abs_path)
```

### Comparing `make_argocd_fly-0.0.6/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.7/make_argocd_fly/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def extract_dir_rel_path(path: str) -> str:
   return os.path.normpath('/'.join(path.split('/')[:-1]))
 
 def resource_parser(resource_yml: str) -> tuple[str, str]:
   resource_kind = None
   resource_name = None
 
-  match = re.search('kind:(.*)', resource_yml)
+  match = re.search('kind:(.*)', resource_yml)  # TODO: test if "kind:(.*)" fixes the issue with commented out manifests
   if match and match.groups():
     resource_kind = match.group(1).strip()
 
   match = re.search('\n  name:(.*)', resource_yml)
   if match and match.groups():
     resource_name = match.group(1).strip()
```

### Comparing `make_argocd_fly-0.0.6/pyproject.toml` & `make_argocd_fly-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
```

