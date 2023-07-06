# Comparing `tmp/ocdsextensionregistry-0.2.2.tar.gz` & `tmp/ocdsextensionregistry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.2.2.tar", last modified: Mon Jun  5 20:53:07 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.0.tar", last modified: Thu Jul  6 22:32:23 2023, max compression
```

## Comparing `ocdsextensionregistry-0.2.2.tar` & `ocdsextensionregistry-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.309322 ocdsextensionregistry-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.309322 ocdsextensionregistry-0.2.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.313322 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 20:53:07.000000 ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:53:07.317322 ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 20:52:58.000000 ocdsextensionregistry-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.401330 ocdsextensionregistry-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.401330 ocdsextensionregistry-0.3.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.405330 ocdsextensionregistry-0.3.0/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.409330 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.405330 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.409330 ocdsextensionregistry-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tox.ini
```

### Comparing `ocdsextensionregistry-0.2.2/LICENSE` & `ocdsextensionregistry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/PKG-INFO` & `ocdsextensionregistry-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.2
+Version: 0.3.0
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.2.2/README.rst` & `ocdsextensionregistry-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/docs/Makefile` & `ocdsextensionregistry-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/docs/changelog.rst` & `ocdsextensionregistry-0.3.0/docs/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 Changelog
 =========
 
+0.3.0 (2023-07-06)
+------------------
+
+-  feat: Make ProfileBuilder more robust to bad data, when using a package's ``extensions`` field as input.
+
+   -  Skip a package's ``extensions`` field if it is not an array.
+   -  Skip an entry in the package's ``extensions`` array if it is blank or is not a string.
+   -  Warn if an extension's ``release-schema.json`` file is not available in bulk, if the request errors (unreachable host, request timeout, HTTP error, too many redirects, etc.), if the bulk file is not a ZIP file, or if the release schema is not a JSON file.
+
+      The previous behavior of raising an exception can be restored with:
+
+      .. code-block:: python
+
+         import warnings
+
+         from ocdsextensionregistry.exceptions import ExtensionWarning
+
+
+         with warnings.catch_warnings():
+             warnings.filterwarnings('error', category=ExtensionWarning)
+             # Use of ProfileBuilder that warns.
+
+-  feat: Configure the expiration behavior of the responses cache using a ``REQUESTS_CACHE_EXPIRE_AFTER`` environment variable. See `requests-cache's documentation <https://requests-cache.readthedocs.io/en/stable/user_guide/expiration.html>`__ (``NEVER_EXPIRE`` is ``-1`` and ``EXPIRE_IMMEDIATELY`` is ``0``, in the `source <https://github.com/requests-cache/requests-cache/blob/main/requests_cache/policy/expiration.py>`__).
+-  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.__repr__`: No longer errors if initialized with ``file_urls`` only.
+-  fix: :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.get_url`: Raises clearer error if initialized with a Download URL only.
+-  Add support for Sphinx 6.2 on Python 3.11.
+
 0.2.2 (2023-06-05)
 ------------------
 
 -  fix: :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name` and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name` return the correct name for GitLab URLs.
 -  fix: Clarify error message for ``AttributeError`` on :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_full_name`, :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_name`, and :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.repository_user`.
 
 0.2.1 (2023-05-24)
 ------------------
 
 -  feat: Add a ``--no-frozen`` option to all commands.
--  Drop Python 3.7 support.
+-  Drop support for Python 3.7.
 
 0.2.0 (2022-10-29)
 ------------------
 
 -  fix: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.release_package_schema` and :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.record_package_schema` return a JSON-serializable object when ``embed=True``.
 
 0.1.14 (2022-09-07)
@@ -48,31 +75,31 @@
 ------------------
 
 -  fix: Convert the ``REQUESTS_POOL_MAXSIZE`` environment variable to ``int``.
 
 0.1.8 (2022-01-20)
 ------------------
 
--  fix: Fix the default value for an extension's ``release-schema.json`` file.
+-  fix: Fix the default value for an extension's ``release-schema.json`` file (``{}``).
 
 0.1.7 (2022-01-12)
 ------------------
 
 -  feat: Use the ``REQUESTS_POOL_MAXSIZE`` environment variable to set the maximum number of connections to save in the `connection pool <https://urllib3.readthedocs.io/en/latest/advanced-usage.html#customizing-pool-behavior>`__.
 -  Drop support for Python 3.6 (end-of-life 2021-12-23).
 
 0.1.6 (2021-11-29)
 ------------------
 
--  feat: :class:`~ocdsextensionregistry.extension_version.ExtensionVersion`: :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.remote` returns the ``default`` argument, if provided, if the file does not exist.
+-  feat: :class:`~ocdsextensionregistry.extension_version.ExtensionVersion`: :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.remote` returns the ``default`` argument, if provided, if the file does not exist. :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.release_schema_patch` uses a default of ``{}`` for ``release-schema.json``.
 
 0.1.5 (2021-11-24)
 ------------------
 
--  Do not globally patch requests.
+-  Do not patch ``requests`` to cache responses.
 
 0.1.4 (2021-04-10)
 ------------------
 
 -  Add Python wheels distribution.
 
 0.1.3 (2021-03-05)
@@ -181,15 +208,15 @@
 -------------------
 
 -  Add a ``update_codelist_urls`` argument to :meth:`ocdsextensionregistry.api.build_profile` to modify codelist reference URLs.
 
 0.0.14 (2019-09-18)
 -------------------
 
--  Use in-memory HTTP requests cache.
+-  Use in-memory cache for HTTP responses.
 
 0.0.13 (2019-08-29)
 -------------------
 
 -  :class:`~ocdsextensionregistry.profile_builder.ProfileBuilder`: Add a ``schema`` argument to :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.patched_release_schema` and :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.release_package_schema` methods to override the release schema or release package schema.
 
 0.0.12 (2019-08-29)
```

### Comparing `ocdsextensionregistry-0.2.2/docs/cli.rst` & `ocdsextensionregistry-0.3.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/docs/conf.py` & `ocdsextensionregistry-0.3.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.2.2"
+version = "0.3.0"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.2.2/docs/index.rst` & `ocdsextensionregistry-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/docs/translation.rst` & `ocdsextensionregistry-0.3.0/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 import sphinx
 from babel.messages.catalog import Catalog
 from babel.messages.extract import extract, pathmatch
 from babel.messages.pofile import write_po
 from ocds_babel.extract import extract_codelist, extract_extension_metadata, extract_schema
 from sphinx.application import Sphinx
 from sphinx.util.docutils import docutils_namespace, patch_docutils
-from sphinx.util.osutil import cd
 
 from ocdsextensionregistry import EXTENSION_VERSIONS_DATA, EXTENSIONS_DATA
 from ocdsextensionregistry.commands.base import BaseCommand
 
+try:
+    from contextlib import chdir
+except ImportError:
+    from sphinx.util.osutil import cd as chdir
+
 logger = logging.getLogger('ocdsextensionregistry')
 
 
 class Command(BaseCommand):
     name = 'generate-pot-files'
     help = 'generates POT files (message catalogs) for versions of extensions'
 
@@ -169,15 +173,15 @@
                         filename = info.filename[start:]
                         if filename == 'README.md':
                             # This avoids writing an unnecessary directory.
                             info.filename = filename
                             zipfile.extract(info, srcdir)
                             break
 
-                    with cd(srcdir):
+                    with chdir(srcdir):
                         # Eliminates a warning, without changing the output.
                         with open('index.rst', 'w') as f:
                             f.write('.. toctree::\n   :hidden:\n\n   README')
 
                         # Sphinx's config.py pop()'s extensions.
                         # https://github.com/sphinx-doc/sphinx/issues/6848
                         kwargs['confoverrides']['extensions'] = ['myst_parser']
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,7 +16,22 @@
 
 class UnknownLatestVersion(OCDSExtensionRegistryError):
     """Raised if the latest version of an extension can't be determined"""
 
 
 class CommandError(OCDSExtensionRegistryError):
     """Errors from within this package's CLI"""
+
+
+class OCDSExtensionRegistryWarning(UserWarning):
+    """Base class for warnings from within this package"""
+
+
+class ExtensionWarning(OCDSExtensionRegistryWarning):
+    """Used when an extension can't be retrieved or merged."""
+
+    def __init__(self, extension, exc):
+        self.extension = extension
+        self.exc = exc
+
+    def __str__(self):
+        return f"{self.extension}: {self.exc.__class__.__module__}.{self.exc.__class__.__name__}: {self.exc}"
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         self._codelists = None
 
     def __repr__(self):
         if self.id and self.version:
             return f'{self.id}=={self.version}'
         elif self.base_url:
             return self.base_url
-        else:
+        elif self.download_url:
             return self.download_url
+        return self._file_urls['release-schema.json']
 
     def update(self, other):
         """
         Merges in the properties of another Extension or ExtensionVersion object.
         """
         for k, v in other.as_dict().items():
             setattr(self, k, v)
@@ -51,18 +52,22 @@
         Returns the object's public properties as a dictionary.
         """
         return {key: value for key, value in self.__dict__.items() if not key.startswith('_')}
 
     def get_url(self, basename):
         """
         Returns the URL of the file within the extension.
+
+        :raises NotImplementedError: if the basename is not in the file URLs and the base URL is not set
         """
         if basename in self._file_urls:
             return self._file_urls[basename]
-        return self.base_url + basename
+        if self.base_url:
+            return self.base_url + basename
+        raise NotImplementedError("get_url() with no base URL or matching file URL is not implemented")
 
     def remote(self, basename, default=None):
         """
         Returns the contents of the file within the extension. If the ``default`` is set and the file does not exist,
         returns the provided ``default`` value.
 
         If the extension has a download URL, caches all the files' contents. Otherwise, downloads and caches the
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/profile_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,26 @@
 """  # noqa: E501
 
 import csv
 import json
 import logging
 import os
 import re
+import warnings
+import zipfile
+from collections.abc import Iterable
 from io import StringIO
 from urllib.parse import urljoin, urlsplit
 
 import json_merge_patch
 import jsonref
+import requests
 
 from .codelist import Codelist
+from .exceptions import ExtensionWarning, NotAvailableInBulk
 from .extension_registry import ExtensionRegistry
 from .extension_version import ExtensionVersion
 from .util import _resolve_zip
 
 logger = logging.getLogger('ocdsextensionregistry')
 
 
@@ -89,16 +94,18 @@
     def extensions(self):
         """
         Returns the matching extension versions from the registry.
         """
         if isinstance(self.extension_versions, dict):
             for identifier, version in self.extension_versions.items():
                 yield self.registry.get(id=identifier, version=version)
-        else:
+        elif isinstance(self.extension_versions, Iterable):
             for url in self.extension_versions:
+                if not url or not isinstance(url, str):
+                    continue
                 parsed = urlsplit(url)
                 data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
                 kwargs = {}
                 if parsed.scheme == 'file':
                     data['Download URL'] = url
                 elif url.endswith('/extension.json'):
                     data['Base URL'] = url[:-14]
@@ -121,16 +128,25 @@
                                     extension in which the definition or field is defined
         :param str language: the language to use for the name of the extension
         """
         output = {}
 
         # Replaces `null` with sentinel values, to preserve the null'ing of fields by extensions in the final patch.
         for extension in self.extensions():
-            patch = extension.remote('release-schema.json', default='{}')
-            patch = json.loads(re.sub(r':\s*null\b', ': "REPLACE_WITH_NULL"', patch))
+            try:
+                patch = extension.remote('release-schema.json', default='{}')
+                patch = json.loads(re.sub(r':\s*null\b', ':"REPLACE_WITH_NULL"', patch))
+            except (
+                NotAvailableInBulk,
+                json.JSONDecodeError,
+                requests.RequestException,
+                zipfile.BadZipFile,
+            ) as e:
+                warnings.warn(ExtensionWarning(extension, e))
+                continue
             if extension_field:
                 _add_extension_field(patch, extension.metadata['name'][language], extension_field)
             json_merge_patch.merge(output, patch)
 
         return json.loads(json.dumps(output).replace('"REPLACE_WITH_NULL"', 'null'))
 
     def patched_release_schema(self, schema=None, extension_field=None, language='en'):
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import warnings
 from io import BytesIO
 from urllib.parse import urlsplit
 from zipfile import ZipFile
 
 from requests.adapters import HTTPAdapter
-from requests_cache import CachedSession
+from requests_cache import NEVER_EXPIRE, CachedSession
 
 from .exceptions import UnknownLatestVersion
 
 if os.name == 'nt':
     FILE_URI_OFFSET = 8  # "file:///C|/tmp"
 else:
     FILE_URI_OFFSET = 7  # "file:///tmp"
@@ -24,15 +24,15 @@
     category=ResourceWarning,
     message=r"^unclosed <ssl\.SSLSocket fd=\d+, family=AddressFamily\.AF_INET6?, type=SocketKind\.SOCK_STREAM, ",
 )
 
 # https://2.python-requests.org/projects/3/api/#requests.adapters.HTTPAdapter
 # https://urllib3.readthedocs.io/en/latest/advanced-usage.html#customizing-pool-behavior
 adapter = HTTPAdapter(max_retries=3, pool_maxsize=int(os.getenv('REQUESTS_POOL_MAXSIZE', 10)))
-session = CachedSession(backend='memory')
+session = CachedSession(backend='memory', expire_after=os.getenv('REQUESTS_CACHE_EXPIRE_AFTER', NEVER_EXPIRE))
 session.mount('https://', adapter)
 session.mount('http://', adapter)
 
 
 def json_dump(data, io):
     """
     Dumps JSON to a file-like object.
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.2
+Version: 0.3.0
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.2.2/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/setup.cfg` & `ocdsextensionregistry-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.2.2
+version = 0.3.0
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -21,15 +21,14 @@
 [options]
 packages = find:
 install_requires = 
 	json-merge-patch
 	jsonref>=1
 	requests
 	requests-cache
-	urllib3<2
 	cattrs!=22.1.0;platform_python_implementation=="PyPy"
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `ocdsextensionregistry-0.2.2/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.0/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.0/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.0/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.0/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_api.py` & `ocdsextensionregistry-0.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_codelist.py` & `ocdsextensionregistry-0.3.0/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.0/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_extension.py` & `ocdsextensionregistry-0.3.0/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.0/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.0/tests/test_extension_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     assert obj.date == args['Date']
     assert obj.version == args['Version']
     assert obj.base_url == args['Base URL']
     assert obj.download_url == args['Download URL']
 
 
 @pytest.mark.parametrize('args,expected', [
-    (arguments(), 'location==v1.1.3'),
+    (arguments(),
+     'location==v1.1.3'),
     (arguments(**{
         'Id': None,
         'Base URL': 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/',
     }), 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/'),
     (arguments(**{
         'Id': None,
         'Base URL': None,
@@ -46,14 +47,21 @@
 ])
 def test_repr(args, expected):
     obj = ExtensionVersion(args)
 
     assert repr(obj) == expected
 
 
+def test_repr_file_urls():
+    data = dict.fromkeys(['Id', 'Date', 'Version', 'Base URL', 'Download URL'])
+    obj = ExtensionVersion(data, file_urls={'release-schema.json': 'https://example.com/release-schema.json'})
+
+    assert repr(obj) == 'https://example.com/release-schema.json'
+
+
 def test_update():
     obj = ExtensionVersion(arguments())
     obj.update(Extension({'Id': 'location', 'Category': 'item', 'Core': 'true'}))
 
     assert obj.id == 'location'
     assert obj.category == 'item'
     assert obj.core is True
@@ -77,20 +85,39 @@
         'date': args['Date'],
         'version': args['Version'],
         'base_url': args['Base URL'],
         'download_url': args['Download URL'],
     }
 
 
-def test_get_url():
-    obj = ExtensionVersion(arguments())
+@pytest.mark.parametrize('args,expected', [
+    (arguments(),
+     'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/extension.json'),
+    (arguments(**{
+        'Id': None,
+        'Base URL': 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/',
+    }), 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/extension.json'),
+])
+def test_get_url(args, expected):
+    obj = ExtensionVersion(args)
+
+    assert obj.get_url('extension.json') == expected
+
+
+def test_get_url_download_url():
+    args = arguments(**{
+        'Id': None,
+        'Base URL': None,
+        'Download URL': 'https://api.github.com/repos/open-contracting-extensions/ocds_location_extension/zipball/v1.1.3',  # noqa: E501
+    })
 
-    url = 'https://raw.githubusercontent.com/open-contracting-extensions/ocds_location_extension/v1.1.3/extension.json'
+    with pytest.raises(NotImplementedError) as excinfo:
+        ExtensionVersion(args).get_url('extension.json')
 
-    assert obj.get_url('extension.json') == url
+    assert str(excinfo.value) == 'get_url() with no base URL or matching file URL is not implemented'
 
 
 def test_get_url_file_urls():
     url = 'https://example.com/release-schema.json'
 
     obj = ExtensionVersion(arguments(), file_urls={'release-schema.json': url})
```

### Comparing `ocdsextensionregistry-0.2.2/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.0/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.2/tests/test_util.py` & `ocdsextensionregistry-0.3.0/tests/test_util.py`

 * *Files identical despite different names*

