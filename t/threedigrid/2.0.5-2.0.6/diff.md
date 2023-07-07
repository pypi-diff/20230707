# Comparing `tmp/threedigrid-2.0.5.tar.gz` & `tmp/threedigrid-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedigrid-2.0.5.tar", last modified: Mon Mar 27 09:59:24 2023, max compression
+gzip compressed data, was "threedigrid-2.0.6.tar", last modified: Fri Jul  7 09:45:41 2023, max compression
```

## Comparing `threedigrid-2.0.5.tar` & `threedigrid-2.0.6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      296 2023-03-27 09:59:24.000000 threedigrid-2.0.5/AUTHORS.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3527 2023-03-27 09:59:24.000000 threedigrid-2.0.5/CONTRIBUTING.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    16712 2023-03-27 09:59:24.000000 threedigrid-2.0.5/HISTORY.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1507 2023-03-27 09:59:24.000000 threedigrid-2.0.5/LICENSE
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      174 2023-03-27 09:59:24.000000 threedigrid-2.0.5/MANIFEST.in
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    21662 2023-03-27 09:59:24.955631 threedigrid-2.0.5/PKG-INFO
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4257 2023-03-27 09:59:24.000000 threedigrid-2.0.5/README.rst
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/docs/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      612 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/Makefile
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       63 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/api.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4628 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/api_reference.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       28 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/authors.rst
--rwxrwxr-x   0 jprins    (1000) jprins    (1000)     5259 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/conf.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       72 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/console.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       33 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/contributing.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       28 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/history.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      341 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/index.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1555 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/installation.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      773 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/make.bat
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      386 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/miscellaneous.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       27 2023-03-27 09:59:24.000000 threedigrid-2.0.5/docs/readme.rst
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      590 2023-03-27 09:59:24.955631 threedigrid-2.0.5/setup.cfg
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2429 2023-03-27 09:59:24.000000 threedigrid-2.0.5/setup.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      160 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/__init__.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      220 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/__init__.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/breaches/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/breaches/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3617 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/breaches/exporters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2881 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/breaches/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3118 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/breaches/prepare.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1546 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/breaches/timeseries_mixin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     6714 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/constants.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/crosssections/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/crosssections/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      519 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/crosssections/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4039 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/exporter_constants.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/exporters/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/exporters/__init__.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       86 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4553 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/default.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     7572 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/exporter.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     9428 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/gridadmin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     9150 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/gridresultadmin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     7932 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/h5py_datasource.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      958 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/h5py_swmr.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3923 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/idmapper.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/levees/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/levees/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3078 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/levees/exporters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1461 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/levees/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1278 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/levees/prepare.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid/admin/lines/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4270 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/exporters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     7063 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    16777 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/prepare.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      828 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/subsets.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2239 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/lines/timeseries_mixin.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/admin/nodes/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     5261 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/exporters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    12290 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     5316 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/prepare.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      961 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/subsets.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     3599 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/nodes/timeseries_mixin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    21660 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/prepare.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2731 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/prepare_utils.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/admin/pumps/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/pumps/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1454 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/pumps/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     4304 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/pumps/prepare.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1560 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/pumps/timeseries_mixin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     8926 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/rpc_datasource.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     7302 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/serializers.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     7474 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/admin/utils.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    10204 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/geo_utils.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/management/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/management/__init__.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/management/commands/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/management/commands/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2247 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/management/commands/kick.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1189 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/management/help_texts.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     9564 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/numpy_utils.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/orm/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/__init__.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.955631 threedigrid-2.0.5/threedigrid/orm/base/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/__init__.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      947 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/datasource.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      814 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/encoder.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      451 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/exceptions.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2396 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/exporters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     8803 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/fields.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     6511 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/filters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    17964 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/models.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    11698 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/options.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    16212 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/timeseries_mixin.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      596 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/base/utils.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     1248 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/constants.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     8933 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/fields.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     5047 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/filters.py
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     5389 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid/orm/models.py
-drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-03-27 09:59:24.951631 threedigrid-2.0.5/threedigrid.egg-info/
--rw-rw-r--   0 jprins    (1000) jprins    (1000)    21662 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/PKG-INFO
--rw-rw-r--   0 jprins    (1000) jprins    (1000)     2939 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/SOURCES.txt
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/dependency_links.txt
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      149 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/entry_points.txt
--rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/not-zip-safe
--rw-rw-r--   0 jprins    (1000) jprins    (1000)      152 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/requires.txt
--rw-rw-r--   0 jprins    (1000) jprins    (1000)       12 2023-03-27 09:59:24.000000 threedigrid-2.0.5/threedigrid.egg-info/top_level.txt
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      296 2023-07-07 09:45:41.000000 threedigrid-2.0.6/AUTHORS.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3527 2023-07-07 09:45:41.000000 threedigrid-2.0.6/CONTRIBUTING.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    16814 2023-07-07 09:45:41.000000 threedigrid-2.0.6/HISTORY.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1507 2023-07-07 09:45:41.000000 threedigrid-2.0.6/LICENSE
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      174 2023-07-07 09:45:41.000000 threedigrid-2.0.6/MANIFEST.in
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    21764 2023-07-07 09:45:41.791873 threedigrid-2.0.6/PKG-INFO
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4257 2023-07-07 09:45:41.000000 threedigrid-2.0.6/README.rst
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.787873 threedigrid-2.0.6/docs/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      612 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/Makefile
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       63 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/api.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4628 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/api_reference.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       28 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/authors.rst
+-rwxrwxr-x   0 jprins    (1000) jprins    (1000)     5259 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/conf.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       72 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/console.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       33 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/contributing.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       28 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/history.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      341 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/index.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1555 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/installation.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      773 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/make.bat
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      386 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/miscellaneous.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       27 2023-07-07 09:45:41.000000 threedigrid-2.0.6/docs/readme.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      590 2023-07-07 09:45:41.791873 threedigrid-2.0.6/setup.cfg
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2429 2023-07-07 09:45:41.000000 threedigrid-2.0.6/setup.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.787873 threedigrid-2.0.6/threedigrid/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      160 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/__init__.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      220 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/__init__.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/breaches/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/breaches/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3617 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/breaches/exporters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2881 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/breaches/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3118 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/breaches/prepare.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1546 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/breaches/timeseries_mixin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     6762 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/constants.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/crosssections/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/crosssections/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      519 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/crosssections/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4039 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/exporter_constants.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/exporters/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/exporters/__init__.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       86 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4553 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/default.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     7572 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/exporter.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     9428 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/gridadmin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     9150 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/gridresultadmin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     7932 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/h5py_datasource.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      958 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/h5py_swmr.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3923 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/idmapper.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/levees/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/levees/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3078 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/levees/exporters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1461 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/levees/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1278 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/levees/prepare.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/lines/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4270 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/exporters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     7215 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    16777 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/prepare.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      828 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/subsets.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2239 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/lines/timeseries_mixin.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/nodes/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     5261 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/exporters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    12288 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     5316 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/prepare.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      961 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/subsets.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3599 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/nodes/timeseries_mixin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    21660 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/prepare.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2731 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/prepare_utils.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/admin/pumps/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/pumps/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1454 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/pumps/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4304 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/pumps/prepare.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1560 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/pumps/timeseries_mixin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     8926 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/rpc_datasource.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     7302 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/serializers.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     7474 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/admin/utils.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    10204 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/geo_utils.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/management/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/management/__init__.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/management/commands/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/management/commands/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2247 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/management/commands/kick.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1189 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/management/help_texts.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     9564 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/numpy_utils.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/orm/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/__init__.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.791873 threedigrid-2.0.6/threedigrid/orm/base/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      947 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/datasource.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      814 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/encoder.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      451 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/exceptions.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2396 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/exporters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     8803 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/fields.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     6511 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/filters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    17964 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    11698 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/options.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    16212 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/timeseries_mixin.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      596 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/base/utils.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1248 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/constants.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     8933 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/fields.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     5047 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/filters.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     5389 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid/orm/models.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2023-07-07 09:45:41.787873 threedigrid-2.0.6/threedigrid.egg-info/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    21764 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/PKG-INFO
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2939 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/SOURCES.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/dependency_links.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      149 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/entry_points.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/not-zip-safe
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      152 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/requires.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       12 2023-07-07 09:45:41.000000 threedigrid-2.0.6/threedigrid.egg-info/top_level.txt
```

### Comparing `threedigrid-2.0.5/CONTRIBUTING.rst` & `threedigrid-2.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/HISTORY.rst` & `threedigrid-2.0.6/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+2.0.6 (2023-07-07)
+------------------
+
+- Added `sewerage` and `sewerage_type` fields to Line model.
+
+
 2.0.5 (2023-03-27)
 ------------------
 
 - Switch to using 'line_geometries' for Breaches model.
 
 
 2.0.4 (2023-03-24)
```

### Comparing `threedigrid-2.0.5/LICENSE` & `threedigrid-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/PKG-INFO` & `threedigrid-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Platform: UNKNOWN
@@ -172,14 +172,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.0.6 (2023-07-07)
+------------------
+
+- Added `sewerage` and `sewerage_type` fields to Line model.
+
+
 2.0.5 (2023-03-27)
 ------------------
 
 - Switch to using 'line_geometries' for Breaches model.
 
 
 2.0.4 (2023-03-24)
```

### Comparing `threedigrid-2.0.5/README.rst` & `threedigrid-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/docs/Makefile` & `threedigrid-2.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/docs/api_reference.rst` & `threedigrid-2.0.6/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/docs/conf.py` & `threedigrid-2.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/docs/installation.rst` & `threedigrid-2.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/docs/make.bat` & `threedigrid-2.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/setup.cfg` & `threedigrid-2.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/setup.py` & `threedigrid-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/breaches/exporters.py` & `threedigrid-2.0.6/threedigrid/admin/breaches/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/breaches/models.py` & `threedigrid-2.0.6/threedigrid/admin/breaches/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/breaches/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/breaches/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/breaches/timeseries_mixin.py` & `threedigrid-2.0.6/threedigrid/admin/breaches/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/constants.py` & `threedigrid-2.0.6/threedigrid/admin/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
 
 TYPE_FUNC_MAP = {
     "int": int,
     int: to_int,
     float: to_float,
     str: to_string,
-    bool: bool,
+    bool: lambda x: None if x in (-9999, "-9999") else bool(x),
     "float": to_float,
     "str": to_string,
 }
 
 
 ###############################################################################
 # shapefile names (served by tilestache)
```

### Comparing `threedigrid-2.0.5/threedigrid/admin/crosssections/models.py` & `threedigrid-2.0.6/threedigrid/admin/crosssections/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/exporter_constants.py` & `threedigrid-2.0.6/threedigrid/admin/exporter_constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/default.py` & `threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/default.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/exporters/geopackage/exporter.py` & `threedigrid-2.0.6/threedigrid/admin/exporters/geopackage/exporter.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/gridadmin.py` & `threedigrid-2.0.6/threedigrid/admin/gridadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/gridresultadmin.py` & `threedigrid-2.0.6/threedigrid/admin/gridresultadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/h5py_datasource.py` & `threedigrid-2.0.6/threedigrid/admin/h5py_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/h5py_swmr.py` & `threedigrid-2.0.6/threedigrid/admin/h5py_swmr.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/idmapper.py` & `threedigrid-2.0.6/threedigrid/admin/idmapper.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/levees/exporters.py` & `threedigrid-2.0.6/threedigrid/admin/levees/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/levees/models.py` & `threedigrid-2.0.6/threedigrid/admin/levees/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/levees/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/levees/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/lines/exporters.py` & `threedigrid-2.0.6/threedigrid/admin/lines/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/lines/models.py` & `threedigrid-2.0.6/threedigrid/admin/lines/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     content_type = ArrayField(type=str)
     zoom_category = ArrayField(type=int)
     cross_pix_coords = LineArrayField()
     line_coords = LineArrayField()
     line_geometries = MultiLineArrayField()
     discharge_coefficient_negative = ArrayField(type=float)
     discharge_coefficient_positive = ArrayField(type=float)
+    sewerage = ArrayField(type=bool)
+    sewerage_type = ArrayField(type=int)
 
     SUBSETS = LINE_SUBSETS
 
     GPKG_DEFAULT_FIELD_MAP = {
         "id": "id",
         "discharge_coefficient_positive": "discharge_coefficient_positive",
         "discharge_coefficient_negative": "discharge_coefficient_negative",
@@ -79,14 +81,16 @@
         "content_pk": "source_table_id",
         "invert_level_start_point": "invert_level_start_point",
         "invert_level_end_point": "invert_level_end_point",
         "dpumax": "exchange_level",
         "line__0": "calculation_node_id_start",
         "line__1": "calculation_node_id_end",
         "line_geometries": "the_geom",
+        "sewerage": "sewerage",
+        "sewerage_type": "sewerage_type",
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._exporters = [
             exporters.LinesOgrExporter(self),
```

### Comparing `threedigrid-2.0.5/threedigrid/admin/lines/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/lines/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/lines/subsets.py` & `threedigrid-2.0.6/threedigrid/admin/lines/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/lines/timeseries_mixin.py` & `threedigrid-2.0.6/threedigrid/admin/lines/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/nodes/exporters.py` & `threedigrid-2.0.6/threedigrid/admin/nodes/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/nodes/models.py` & `threedigrid-2.0.6/threedigrid/admin/nodes/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "node_type__in": subsets.NODE_TYPE__IN_SUBSETS,
 }
 
 
 class Nodes(Model):
     content_pk = ArrayField(type=int)
     seq_id = ArrayField(type=int)
-    calculation_type = ArrayField(type=float)
+    calculation_type = ArrayField(type=int)
     coordinates = PointArrayField()
     cell_coords = BboxArrayField()
     zoom_category = ArrayField(type=float)
     node_type = ArrayField(type=int)
     is_manhole = BooleanArrayField()
     sumax = ArrayField(type=float)
     drain_level = ArrayField(type=float)
```

### Comparing `threedigrid-2.0.5/threedigrid/admin/nodes/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/nodes/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/nodes/subsets.py` & `threedigrid-2.0.6/threedigrid/admin/nodes/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/nodes/timeseries_mixin.py` & `threedigrid-2.0.6/threedigrid/admin/nodes/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/prepare_utils.py` & `threedigrid-2.0.6/threedigrid/admin/prepare_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/pumps/models.py` & `threedigrid-2.0.6/threedigrid/admin/pumps/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/pumps/prepare.py` & `threedigrid-2.0.6/threedigrid/admin/pumps/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/pumps/timeseries_mixin.py` & `threedigrid-2.0.6/threedigrid/admin/pumps/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/rpc_datasource.py` & `threedigrid-2.0.6/threedigrid/admin/rpc_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/serializers.py` & `threedigrid-2.0.6/threedigrid/admin/serializers.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/admin/utils.py` & `threedigrid-2.0.6/threedigrid/admin/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/geo_utils.py` & `threedigrid-2.0.6/threedigrid/geo_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/management/commands/kick.py` & `threedigrid-2.0.6/threedigrid/management/commands/kick.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/management/help_texts.py` & `threedigrid-2.0.6/threedigrid/management/help_texts.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/numpy_utils.py` & `threedigrid-2.0.6/threedigrid/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/datasource.py` & `threedigrid-2.0.6/threedigrid/orm/base/datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/encoder.py` & `threedigrid-2.0.6/threedigrid/orm/base/encoder.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/exporters.py` & `threedigrid-2.0.6/threedigrid/orm/base/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/fields.py` & `threedigrid-2.0.6/threedigrid/orm/base/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/filters.py` & `threedigrid-2.0.6/threedigrid/orm/base/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/models.py` & `threedigrid-2.0.6/threedigrid/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/options.py` & `threedigrid-2.0.6/threedigrid/orm/base/options.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/timeseries_mixin.py` & `threedigrid-2.0.6/threedigrid/orm/base/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/base/utils.py` & `threedigrid-2.0.6/threedigrid/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/constants.py` & `threedigrid-2.0.6/threedigrid/orm/constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/fields.py` & `threedigrid-2.0.6/threedigrid/orm/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/filters.py` & `threedigrid-2.0.6/threedigrid/orm/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid/orm/models.py` & `threedigrid-2.0.6/threedigrid/orm/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.0.5/threedigrid.egg-info/PKG-INFO` & `threedigrid-2.0.6/threedigrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Platform: UNKNOWN
@@ -172,14 +172,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.0.6 (2023-07-07)
+------------------
+
+- Added `sewerage` and `sewerage_type` fields to Line model.
+
+
 2.0.5 (2023-03-27)
 ------------------
 
 - Switch to using 'line_geometries' for Breaches model.
 
 
 2.0.4 (2023-03-24)
```

### Comparing `threedigrid-2.0.5/threedigrid.egg-info/SOURCES.txt` & `threedigrid-2.0.6/threedigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

