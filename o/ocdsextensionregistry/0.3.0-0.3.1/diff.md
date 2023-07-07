# Comparing `tmp/ocdsextensionregistry-0.3.0.tar.gz` & `tmp/ocdsextensionregistry-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.0.tar", last modified: Thu Jul  6 22:32:23 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.1.tar", last modified: Fri Jul  7 17:40:58 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.0.tar` & `ocdsextensionregistry-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.401330 ocdsextensionregistry-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.401330 ocdsextensionregistry-0.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.405330 ocdsextensionregistry-0.3.0/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.409330 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.405330 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 22:32:23.000000 ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.409330 ocdsextensionregistry-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:32:23.413330 ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 22:32:10.000000 ocdsextensionregistry-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.261345 ocdsextensionregistry-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.261345 ocdsextensionregistry-0.3.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.265345 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 17:40:58.000000 ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-07 17:40:58.273346 ocdsextensionregistry-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:40:58.269346 ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 17:40:46.000000 ocdsextensionregistry-0.3.1/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.0/LICENSE` & `ocdsextensionregistry-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/PKG-INFO` & `ocdsextensionregistry-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.0
+Version: 0.3.1
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.0/README.rst` & `ocdsextensionregistry-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/docs/Makefile` & `ocdsextensionregistry-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/docs/changelog.rst` & `ocdsextensionregistry-0.3.1/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.3.1 (2023-07-07)
+------------------
+
+-  fix: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.extensions`: Support retrieval of the metadata file, if the ``extension_versions`` argument is a list of extensions' metadata files served via API.
+
 0.3.0 (2023-07-06)
 ------------------
 
 -  feat: Make ProfileBuilder more robust to bad data, when using a package's ``extensions`` field as input.
 
    -  Skip a package's ``extensions`` field if it is not an array.
    -  Skip an entry in the package's ``extensions`` array if it is blank or is not a string.
```

### Comparing `ocdsextensionregistry-0.3.0/docs/cli.rst` & `ocdsextensionregistry-0.3.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/docs/conf.py` & `ocdsextensionregistry-0.3.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.0"
+version = "0.3.1"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.0/docs/index.rst` & `ocdsextensionregistry-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/docs/translation.rst` & `ocdsextensionregistry-0.3.1/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/profile_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,18 @@
                     data['Base URL'] = url[:-14]
                 elif url.endswith('/'):
                     data['Base URL'] = url
                 elif parsed.path.endswith('.json'):
                     kwargs['file_urls'] = {'release-schema.json': url}
                 # If the files are served via API, with the filename as a query string parameter.
                 elif 'extension.json' in url:
-                    kwargs['file_urls'] = {'release-schema.json': url.replace('extension.json', 'release-schema.json')}
+                    kwargs['file_urls'] = {
+                        'extension.json': url,
+                        'release-schema.json': url.replace('extension.json', 'release-schema.json'),
+                    }
                 else:
                     data['Download URL'] = url
                 yield ExtensionVersion(data, **kwargs)
 
     def release_schema_patch(self, extension_field=None, language='en'):
         """
         Returns the consolidated release schema patch.
```

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.0
+Version: 0.3.1
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.0/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.1/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/setup.cfg` & `ocdsextensionregistry-0.3.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.0
+version = 0.3.1
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.3.0/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.1/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.1/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.1/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.1/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_api.py` & `ocdsextensionregistry-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_codelist.py` & `ocdsextensionregistry-0.3.1/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.1/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_extension.py` & `ocdsextensionregistry-0.3.1/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.1/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.1/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.1/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tests/test_util.py` & `ocdsextensionregistry-0.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.0/tox.ini` & `ocdsextensionregistry-0.3.1/tox.ini`

 * *Files identical despite different names*

