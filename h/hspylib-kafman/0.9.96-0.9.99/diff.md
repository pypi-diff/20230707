# Comparing `tmp/hspylib-kafman-0.9.96.tar.gz` & `tmp/hspylib-kafman-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-kafman-0.9.96.tar", last modified: Fri Dec 23 04:58:49 2022, max compression
+gzip compressed data, was "hspylib-kafman-0.9.99.tar", last modified: Fri Dec 23 05:25:07 2022, max compression
```

## Comparing `hspylib-kafman-0.9.96.tar` & `hspylib-kafman-0.9.99.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.117659 hspylib-kafman-0.9.96/
--rw-r--r--   0 hugo       (503) staff       (20)      193 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.96/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     1405 2022-12-23 04:58:49.117333 hspylib-kafman-0.9.96/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      688 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.081822 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     1405 2022-12-23 04:58:49.000000 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     2671 2022-12-23 04:58:49.000000 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2022-12-23 04:58:49.000000 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)      128 2022-12-23 04:58:49.000000 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)        7 2022-12-23 04:58:49.000000 hspylib-kafman-0.9.96/hspylib_kafman.egg-info/top_level.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.083249 hspylib-kafman-0.9.96/kafman/
--rw-r--r--   0 hugo       (503) staff       (20)        6 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/.version
--rw-r--r--   0 hugo       (503) staff       (20)      718 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2032 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.084960 hspylib-kafman-0.9.96/kafman/core/
--rw-r--r--   0 hugo       (503) staff       (20)      266 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      782 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/constants.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.085960 hspylib-kafman-0.9.96/kafman/core/consumer/
--rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/consumer/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1464 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/consumer/consumer_config.py
--rw-r--r--   0 hugo       (503) staff       (20)     4151 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/consumer/consumer_worker.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.086632 hspylib-kafman-0.9.96/kafman/core/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      174 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      659 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/exception/exceptions.py
--rw-r--r--   0 hugo       (503) staff       (20)      949 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/kafka_message.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.087483 hspylib-kafman-0.9.96/kafman/core/producer/
--rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/producer/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      882 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/producer/producer_config.py
--rw-r--r--   0 hugo       (503) staff       (20)     4841 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/producer/producer_worker.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.090578 hspylib-kafman-0.9.96/kafman/core/schema/
--rw-r--r--   0 hugo       (503) staff       (20)      336 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/schema/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.091470 hspylib-kafman-0.9.96/kafman/core/schema/avro/
--rw-r--r--   0 hugo       (503) staff       (20)      205 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     4902 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/avro_schema.py
--rw-r--r--   0 hugo       (503) staff       (20)     2327 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/avro_type.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.094235 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/
--rw-r--r--   0 hugo       (503) staff       (20)      295 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1093 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/array_field.py
--rw-r--r--   0 hugo       (503) staff       (20)     1174 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/enum_field.py
--rw-r--r--   0 hugo       (503) staff       (20)     3684 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/field_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)      667 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/fixed_field.py
--rw-r--r--   0 hugo       (503) staff       (20)      752 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/map_field.py
--rw-r--r--   0 hugo       (503) staff       (20)      756 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/primitive_field.py
--rw-r--r--   0 hugo       (503) staff       (20)      796 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/avro/field/record_field.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.095813 hspylib-kafman-0.9.96/kafman/core/schema/json/
--rw-r--r--   0 hugo       (503) staff       (20)      226 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2995 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/json_parser.py
--rw-r--r--   0 hugo       (503) staff       (20)     5043 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/json_schema.py
--rw-r--r--   0 hugo       (503) staff       (20)     1534 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/json_type.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.098040 hspylib-kafman-0.9.96/kafman/core/schema/json/property/
--rw-r--r--   0 hugo       (503) staff       (20)      294 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1072 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/array_property.py
--rw-r--r--   0 hugo       (503) staff       (20)     1088 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/enum_property.py
--rw-r--r--   0 hugo       (503) staff       (20)      868 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/object_property.py
--rw-r--r--   0 hugo       (503) staff       (20)      772 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/primitive_property.py
--rw-r--r--   0 hugo       (503) staff       (20)     1487 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/property.py
--rw-r--r--   0 hugo       (503) staff       (20)     2776 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/json/property/property_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)     6035 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/kafka_schema.py
--rw-r--r--   0 hugo       (503) staff       (20)     1597 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/plain_schema.py
--rw-r--r--   0 hugo       (503) staff       (20)     1187 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/registry_subject.py
--rw-r--r--   0 hugo       (503) staff       (20)     1304 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/schema_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)     1698 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/schema_field.py
--rw-r--r--   0 hugo       (503) staff       (20)     6511 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/schema_registry.py
--rw-r--r--   0 hugo       (503) staff       (20)      638 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/schema_type.py
--rw-r--r--   0 hugo       (503) staff       (20)     5071 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/schema/widget_utils.py
--rw-r--r--   0 hugo       (503) staff       (20)     2530 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/core/statistics_worker.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.100584 hspylib-kafman-0.9.96/kafman/resources/
--rw-r--r--   0 hugo       (503) staff       (20)    54865 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.96/kafman/resources/app-icon.png
--rw-r--r--   0 hugo       (503) staff       (20)        0 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.96/kafman/resources/application.properties
--rw-r--r--   0 hugo       (503) staff       (20)     5717 2022-06-04 02:51:50.000000 hspylib-kafman-0.9.96/kafman/resources/consumer-settings.properties
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.101126 hspylib-kafman-0.9.96/kafman/resources/fonts/
--rw-r--r--   0 hugo       (503) staff       (20)  2209264 2022-05-30 21:06:41.000000 hspylib-kafman-0.9.96/kafman/resources/fonts/Droid-Sans-Mono-for-Powerline-Nerd-Font-Complete.otf
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.112804 hspylib-kafman-0.9.96/kafman/resources/forms/
--rw-r--r--   0 hugo       (503) staff       (20)     9123 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.96/kafman/resources/forms/filters_dlg.ui
--rw-r--r--   0 hugo       (503) staff       (20)   121048 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.96/kafman/resources/forms/main_qt_view.ui
--rw-r--r--   0 hugo       (503) staff       (20)     5001 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.96/kafman/resources/forms/settings_dlg.ui
--rw-r--r--   0 hugo       (503) staff       (20)     5216 2022-06-04 02:51:50.000000 hspylib-kafman-0.9.96/kafman/resources/producer-settings.properties
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.114489 hspylib-kafman-0.9.96/kafman/views/
--rw-r--r--   0 hugo       (503) staff       (20)      212 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/views/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.115930 hspylib-kafman-0.9.96/kafman/views/dialogs/
--rw-r--r--   0 hugo       (503) staff       (20)      199 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/views/dialogs/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     5453 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/dialogs/filters_dialog.py
--rw-r--r--   0 hugo       (503) staff       (20)     4203 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/dialogs/settings_dialog.py
--rw-r--r--   0 hugo       (503) staff       (20)      797 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/indexes.py
--rw-r--r--   0 hugo       (503) staff       (20)    44565 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/main_qt_view.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 04:58:49.116790 hspylib-kafman-0.9.96/kafman/views/promotions/
--rw-r--r--   0 hugo       (503) staff       (20)      191 2022-12-23 04:58:48.000000 hspylib-kafman-0.9.96/kafman/views/promotions/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2124 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/promotions/form_area.py
--rw-r--r--   0 hugo       (503) staff       (20)     5453 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/kafman/views/promotions/form_pane.py
--rw-r--r--   0 hugo       (503) staff       (20)      219 2022-03-03 17:56:14.000000 hspylib-kafman-0.9.96/kafman/welcome.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2022-12-23 04:58:49.117758 hspylib-kafman-0.9.96/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     1710 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.96/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.156067 hspylib-kafman-0.9.99/
+-rw-r--r--   0 hugo       (503) staff       (20)      193 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.99/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     1579 2022-12-23 05:25:07.155618 hspylib-kafman-0.9.99/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      688 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.118434 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     1579 2022-12-23 05:25:07.000000 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     2671 2022-12-23 05:25:07.000000 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2022-12-23 05:25:07.000000 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)      128 2022-12-23 05:25:07.000000 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        7 2022-12-23 05:25:07.000000 hspylib-kafman-0.9.99/hspylib_kafman.egg-info/top_level.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.120241 hspylib-kafman-0.9.99/kafman/
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      718 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2032 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.121959 hspylib-kafman-0.9.99/kafman/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      266 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      782 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/constants.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.122984 hspylib-kafman-0.9.99/kafman/core/consumer/
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/consumer/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1464 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/consumer/consumer_config.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4151 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/consumer/consumer_worker.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.123641 hspylib-kafman-0.9.99/kafman/core/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      174 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      659 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/exception/exceptions.py
+-rw-r--r--   0 hugo       (503) staff       (20)      949 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/kafka_message.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.124565 hspylib-kafman-0.9.99/kafman/core/producer/
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/producer/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      882 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/producer/producer_config.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4841 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/producer/producer_worker.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.127230 hspylib-kafman-0.9.99/kafman/core/schema/
+-rw-r--r--   0 hugo       (503) staff       (20)      336 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/schema/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.128184 hspylib-kafman-0.9.99/kafman/core/schema/avro/
+-rw-r--r--   0 hugo       (503) staff       (20)      205 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4902 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/avro_schema.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2327 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/avro_type.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.130968 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/
+-rw-r--r--   0 hugo       (503) staff       (20)      295 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1093 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/array_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1174 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/enum_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3684 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/field_factory.py
+-rw-r--r--   0 hugo       (503) staff       (20)      667 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/fixed_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)      752 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/map_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)      756 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/primitive_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)      796 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/avro/field/record_field.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.132550 hspylib-kafman-0.9.99/kafman/core/schema/json/
+-rw-r--r--   0 hugo       (503) staff       (20)      226 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2995 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/json_parser.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5043 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/json_schema.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1534 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/json_type.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.135122 hspylib-kafman-0.9.99/kafman/core/schema/json/property/
+-rw-r--r--   0 hugo       (503) staff       (20)      294 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1072 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/array_property.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1088 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/enum_property.py
+-rw-r--r--   0 hugo       (503) staff       (20)      868 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/object_property.py
+-rw-r--r--   0 hugo       (503) staff       (20)      772 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/primitive_property.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1487 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/property.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2776 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/json/property/property_factory.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6035 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/kafka_schema.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1597 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/plain_schema.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1187 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/registry_subject.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1304 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/schema_factory.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1698 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/schema_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6511 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/schema_registry.py
+-rw-r--r--   0 hugo       (503) staff       (20)      638 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/schema_type.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5071 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/schema/widget_utils.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2530 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/core/statistics_worker.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.138058 hspylib-kafman-0.9.99/kafman/resources/
+-rw-r--r--   0 hugo       (503) staff       (20)    54865 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.99/kafman/resources/app-icon.png
+-rw-r--r--   0 hugo       (503) staff       (20)        0 2022-07-02 02:40:02.000000 hspylib-kafman-0.9.99/kafman/resources/application.properties
+-rw-r--r--   0 hugo       (503) staff       (20)     5717 2022-06-04 02:51:50.000000 hspylib-kafman-0.9.99/kafman/resources/consumer-settings.properties
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.138652 hspylib-kafman-0.9.99/kafman/resources/fonts/
+-rw-r--r--   0 hugo       (503) staff       (20)  2209264 2022-05-30 21:06:41.000000 hspylib-kafman-0.9.99/kafman/resources/fonts/Droid-Sans-Mono-for-Powerline-Nerd-Font-Complete.otf
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.151033 hspylib-kafman-0.9.99/kafman/resources/forms/
+-rw-r--r--   0 hugo       (503) staff       (20)     9123 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.99/kafman/resources/forms/filters_dlg.ui
+-rw-r--r--   0 hugo       (503) staff       (20)   121048 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.99/kafman/resources/forms/main_qt_view.ui
+-rw-r--r--   0 hugo       (503) staff       (20)     5001 2022-11-28 23:07:30.000000 hspylib-kafman-0.9.99/kafman/resources/forms/settings_dlg.ui
+-rw-r--r--   0 hugo       (503) staff       (20)     5216 2022-06-04 02:51:50.000000 hspylib-kafman-0.9.99/kafman/resources/producer-settings.properties
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.152594 hspylib-kafman-0.9.99/kafman/views/
+-rw-r--r--   0 hugo       (503) staff       (20)      212 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/views/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.153938 hspylib-kafman-0.9.99/kafman/views/dialogs/
+-rw-r--r--   0 hugo       (503) staff       (20)      199 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/views/dialogs/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5453 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/dialogs/filters_dialog.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4203 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/dialogs/settings_dialog.py
+-rw-r--r--   0 hugo       (503) staff       (20)      797 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/indexes.py
+-rw-r--r--   0 hugo       (503) staff       (20)    44565 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/main_qt_view.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2022-12-23 05:25:07.155119 hspylib-kafman-0.9.99/kafman/views/promotions/
+-rw-r--r--   0 hugo       (503) staff       (20)      191 2022-12-23 05:25:06.000000 hspylib-kafman-0.9.99/kafman/views/promotions/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2124 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/promotions/form_area.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5453 2022-12-23 01:45:32.000000 hspylib-kafman-0.9.99/kafman/views/promotions/form_pane.py
+-rw-r--r--   0 hugo       (503) staff       (20)      219 2022-03-03 17:56:14.000000 hspylib-kafman-0.9.99/kafman/welcome.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2022-12-23 05:25:07.156184 hspylib-kafman-0.9.99/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     1880 2022-12-23 05:25:00.000000 hspylib-kafman-0.9.99/setup.py
```

### Comparing `hspylib-kafman-0.9.96/PKG-INFO` & `hspylib-kafman-0.9.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-kafman
-Version: 0.9.96
+Version: 0.9.99
 Summary: HSPyLib - Apache Kafka Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-kafman/
@@ -12,20 +12,24 @@
 Platform: Darwin
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Natural Language :: English
+Classifier: Topic :: Desktop Environment
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # HomeSetup - Apache Kafka Manager
 
 ## Manage and test you kafka applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-kafman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-kafman-0.9.96/README.md` & `hspylib-kafman-0.9.99/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Apache Kafka Manager
 
 ## Manage and test you kafka applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-kafman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-kafman-0.9.96/hspylib_kafman.egg-info/PKG-INFO` & `hspylib-kafman-0.9.99/hspylib_kafman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-kafman
-Version: 0.9.96
+Version: 0.9.99
 Summary: HSPyLib - Apache Kafka Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-kafman/
@@ -12,20 +12,24 @@
 Platform: Darwin
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Natural Language :: English
+Classifier: Topic :: Desktop Environment
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # HomeSetup - Apache Kafka Manager
 
 ## Manage and test you kafka applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-kafman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-kafman-0.9.96/hspylib_kafman.egg-info/SOURCES.txt` & `hspylib-kafman-0.9.99/hspylib_kafman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/__classpath__.py` & `hspylib-kafman-0.9.99/kafman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/__main__.py` & `hspylib-kafman-0.9.99/kafman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/constants.py` & `hspylib-kafman-0.9.99/kafman/core/constants.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/consumer/consumer_config.py` & `hspylib-kafman-0.9.99/kafman/core/consumer/consumer_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/consumer/consumer_worker.py` & `hspylib-kafman-0.9.99/kafman/core/consumer/consumer_worker.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/exception/exceptions.py` & `hspylib-kafman-0.9.99/kafman/core/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/kafka_message.py` & `hspylib-kafman-0.9.99/kafman/core/kafka_message.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/producer/producer_config.py` & `hspylib-kafman-0.9.99/kafman/core/producer/producer_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/producer/producer_worker.py` & `hspylib-kafman-0.9.99/kafman/core/producer/producer_worker.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/avro_schema.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/avro_schema.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/avro_type.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/avro_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/array_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/array_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/enum_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/enum_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/field_factory.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/field_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/fixed_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/fixed_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/map_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/map_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/primitive_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/primitive_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/avro/field/record_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/avro/field/record_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/json_parser.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/json_parser.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/json_schema.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/json_schema.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/json_type.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/json_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/array_property.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/array_property.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/enum_property.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/enum_property.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/object_property.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/object_property.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/primitive_property.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/primitive_property.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/property.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/property.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/json/property/property_factory.py` & `hspylib-kafman-0.9.99/kafman/core/schema/json/property/property_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/kafka_schema.py` & `hspylib-kafman-0.9.99/kafman/core/schema/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/plain_schema.py` & `hspylib-kafman-0.9.99/kafman/core/schema/plain_schema.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/registry_subject.py` & `hspylib-kafman-0.9.99/kafman/core/schema/registry_subject.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/schema_factory.py` & `hspylib-kafman-0.9.99/kafman/core/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/schema_field.py` & `hspylib-kafman-0.9.99/kafman/core/schema/schema_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/schema_registry.py` & `hspylib-kafman-0.9.99/kafman/core/schema/schema_registry.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/schema_type.py` & `hspylib-kafman-0.9.99/kafman/core/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/schema/widget_utils.py` & `hspylib-kafman-0.9.99/kafman/core/schema/widget_utils.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/core/statistics_worker.py` & `hspylib-kafman-0.9.99/kafman/core/statistics_worker.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/app-icon.png` & `hspylib-kafman-0.9.99/kafman/resources/app-icon.png`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/consumer-settings.properties` & `hspylib-kafman-0.9.99/kafman/resources/consumer-settings.properties`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/fonts/Droid-Sans-Mono-for-Powerline-Nerd-Font-Complete.otf` & `hspylib-kafman-0.9.99/kafman/resources/fonts/Droid-Sans-Mono-for-Powerline-Nerd-Font-Complete.otf`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/forms/filters_dlg.ui` & `hspylib-kafman-0.9.99/kafman/resources/forms/filters_dlg.ui`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/forms/main_qt_view.ui` & `hspylib-kafman-0.9.99/kafman/resources/forms/main_qt_view.ui`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/forms/settings_dlg.ui` & `hspylib-kafman-0.9.99/kafman/resources/forms/settings_dlg.ui`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/resources/producer-settings.properties` & `hspylib-kafman-0.9.99/kafman/resources/producer-settings.properties`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/dialogs/filters_dialog.py` & `hspylib-kafman-0.9.99/kafman/views/dialogs/filters_dialog.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/dialogs/settings_dialog.py` & `hspylib-kafman-0.9.99/kafman/views/dialogs/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/indexes.py` & `hspylib-kafman-0.9.99/kafman/views/indexes.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/main_qt_view.py` & `hspylib-kafman-0.9.99/kafman/views/main_qt_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/promotions/form_area.py` & `hspylib-kafman-0.9.99/kafman/views/promotions/form_area.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/kafman/views/promotions/form_pane.py` & `hspylib-kafman-0.9.99/kafman/views/promotions/form_pane.py`

 * *Files identical despite different names*

### Comparing `hspylib-kafman-0.9.96/setup.py` & `hspylib-kafman-0.9.99/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,13 +44,17 @@
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Unix",
+        "Development Status :: 4 - Beta",
+        "Environment :: X11 Applications :: Qt",
+        "Natural Language :: English",
+        "Topic :: Desktop Environment",
     ],
     python_requires=">=3.10",
     install_requires=REQUIREMENTS,
     keywords="apache,kafka,queue,manager,application",
     platforms="Darwin,Linux",
 )
```

