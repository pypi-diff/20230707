# Comparing `tmp/taskcat-0.9.9.dev29.tar.gz` & `tmp/taskcat-0.9.9.dev30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taskcat-0.9.9.dev29.tar", last modified: Thu Jan 16 00:22:02 2020, max compression
+gzip compressed data, was "dist/taskcat-0.9.9.dev30.tar", last modified: Thu Jan 16 01:43:10 2020, max compression
```

## Comparing `taskcat-0.9.9.dev29.tar` & `taskcat-0.9.9.dev30.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-01-16 00:20:08.000000 taskcat-0.9.9.dev29/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    14766 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11378 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      284 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/bin/taskcat
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14766 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      324 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      742 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1723 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5397 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn_lint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_s3_stage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13196 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_logger.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/_cfn/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5587 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn/template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5017 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn/_log_stack_events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18616 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn/stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10540 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cfn/threaded.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/cfg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/cfg/animals.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12022 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/cfg/config_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/cfg/descriptors.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5508 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/cfg/amiupdater.cfg.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6403 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_common_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14044 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_template_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5322 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_lambda_build.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_project_generator_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4411 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_legacy_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_client_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15101 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_amiupdater.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1197 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/lint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3940 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6238 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2008 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/delete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7172 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/deploy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2132 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_modules/update_ami.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4142 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_project_generator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/project_templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/README.md.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/templates/debug.template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     3096 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/templates/debug-yaml.template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/taskcat-autobucket.yml.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      985 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/debug-input.json.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/taskcat.yml.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/taskcat-autobucket-json.yml.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 00:22:02.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/scripts/scripts_userdata.sh.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     6360 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_generate_reports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16335 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_dataclasses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5033 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_name_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2494 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_tui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8680 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_s3_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8757 2020-01-16 00:19:40.000000 taskcat-0.9.9.dev29/taskcat/_cli_core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-01-16 01:41:04.000000 taskcat-0.9.9.dev30/VERSION
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14766 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11378 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      284 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/bin/taskcat
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14766 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      324 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      742 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1723 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5397 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn_lint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_s3_stage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13196 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_logger.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/_cfn/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5587 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn/template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5017 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn/_log_stack_events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18616 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn/stack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10540 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cfn/threaded.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/cfg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/cfg/animals.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12022 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/cfg/config_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/cfg/descriptors.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5508 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/cfg/amiupdater.cfg.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6403 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_common_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14044 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_template_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5322 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_lambda_build.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_project_generator_runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4411 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_legacy_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5986 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_client_factory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15101 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_amiupdater.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1197 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/lint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3940 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6238 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2008 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/delete.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7172 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/deploy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      284 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2132 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_modules/update_ami.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4142 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_project_generator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/project_templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/README.md.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/templates/debug.template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3096 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/templates/debug-yaml.template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/taskcat-autobucket.yml.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      985 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/debug-input.json.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      320 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/taskcat.yml.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      320 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/taskcat-autobucket-json.yml.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-16 01:43:10.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/scripts/scripts_userdata.sh.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6360 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_generate_reports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16335 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_dataclasses.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5033 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      555 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_name_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2494 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_tui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8680 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_s3_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8757 2020-01-16 01:40:39.000000 taskcat-0.9.9.dev30/taskcat/_cli_core.py
```

### Comparing `taskcat-0.9.9.dev29/PKG-INFO` & `taskcat-0.9.9.dev30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcat
-Version: 0.9.9.dev29
+Version: 0.9.9.dev30
 Summary: An OpenSource Cloudformation Deployment Framework
 Home-page: https://aws-quickstart.github.io/taskcat/
 Author: Tony Vattathil, Jay McConnell, Andrew Glenn, Santiago Cardenas, Shivansh Singh
 Author-email: tonynv@amazon.com, jmmccon@amazon.com, andglenn@amazon.com, sshvans@amazon.com
 License: Apache License 2.0
 Download-URL: https://github.com/aws-quickstart/taskcat/tarball/master
 Description: # taskcat
```

### Comparing `taskcat-0.9.9.dev29/README.md` & `taskcat-0.9.9.dev30/README.md`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat.egg-info/PKG-INFO` & `taskcat-0.9.9.dev30/taskcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcat
-Version: 0.9.9.dev29
+Version: 0.9.9.dev30
 Summary: An OpenSource Cloudformation Deployment Framework
 Home-page: https://aws-quickstart.github.io/taskcat/
 Author: Tony Vattathil, Jay McConnell, Andrew Glenn, Santiago Cardenas, Shivansh Singh
 Author-email: tonynv@amazon.com, jmmccon@amazon.com, andglenn@amazon.com, sshvans@amazon.com
 License: Apache License 2.0
 Download-URL: https://github.com/aws-quickstart/taskcat/tarball/master
 Description: # taskcat
```

### Comparing `taskcat-0.9.9.dev29/taskcat.egg-info/SOURCES.txt` & `taskcat-0.9.9.dev30/taskcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/setup.cfg` & `taskcat-0.9.9.dev30/setup.cfg`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/setup.py` & `taskcat-0.9.9.dev30/setup.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cfn_lint.py` & `taskcat-0.9.9.dev30/taskcat/_cfn_lint.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_s3_stage.py` & `taskcat-0.9.9.dev30/taskcat/_s3_stage.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_config.py` & `taskcat-0.9.9.dev30/taskcat/_config.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_logger.py` & `taskcat-0.9.9.dev30/taskcat/_logger.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cfn/template.py` & `taskcat-0.9.9.dev30/taskcat/_cfn/template.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cfn/_log_stack_events.py` & `taskcat-0.9.9.dev30/taskcat/_cfn/_log_stack_events.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cfn/stack.py` & `taskcat-0.9.9.dev30/taskcat/_cfn/stack.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cfn/threaded.py` & `taskcat-0.9.9.dev30/taskcat/_cfn/threaded.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/cfg/animals.txt` & `taskcat-0.9.9.dev30/taskcat/cfg/animals.txt`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/cfg/config_schema.json` & `taskcat-0.9.9.dev30/taskcat/cfg/config_schema.json`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/cfg/descriptors.txt` & `taskcat-0.9.9.dev30/taskcat/cfg/descriptors.txt`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/cfg/amiupdater.cfg.yml` & `taskcat-0.9.9.dev30/taskcat/cfg/amiupdater.cfg.yml`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_common_utils.py` & `taskcat-0.9.9.dev30/taskcat/_common_utils.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_template_params.py` & `taskcat-0.9.9.dev30/taskcat/_template_params.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_lambda_build.py` & `taskcat-0.9.9.dev30/taskcat/_lambda_build.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_project_generator_runner.py` & `taskcat-0.9.9.dev30/taskcat/_project_generator_runner.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_legacy_config.py` & `taskcat-0.9.9.dev30/taskcat/_legacy_config.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_client_factory.py` & `taskcat-0.9.9.dev30/taskcat/_client_factory.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_amiupdater.py` & `taskcat-0.9.9.dev30/taskcat/_amiupdater.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/lint.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/lint.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/list.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/list.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/test.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/delete.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/delete.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/deploy.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/deploy.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/package.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/package.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_modules/update_ami.py` & `taskcat-0.9.9.dev30/taskcat/_cli_modules/update_ami.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_project_generator.py` & `taskcat-0.9.9.dev30/taskcat/_project_generator.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/templates/debug.template.jinja` & `taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/templates/debug.template.jinja`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/templates/debug-yaml.template.jinja` & `taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/templates/debug-yaml.template.jinja`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/project_templates/quickstart/ci/debug-input.json.jinja` & `taskcat-0.9.9.dev30/taskcat/project_templates/quickstart/ci/debug-input.json.jinja`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_generate_reports.py` & `taskcat-0.9.9.dev30/taskcat/_generate_reports.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_dataclasses.py` & `taskcat-0.9.9.dev30/taskcat/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli.py` & `taskcat-0.9.9.dev30/taskcat/_cli.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_name_generator.py` & `taskcat-0.9.9.dev30/taskcat/_name_generator.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_tui.py` & `taskcat-0.9.9.dev30/taskcat/_tui.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_s3_sync.py` & `taskcat-0.9.9.dev30/taskcat/_s3_sync.py`

 * *Files identical despite different names*

### Comparing `taskcat-0.9.9.dev29/taskcat/_cli_core.py` & `taskcat-0.9.9.dev30/taskcat/_cli_core.py`

 * *Files identical despite different names*

