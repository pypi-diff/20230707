# Comparing `tmp/basedmypy-2.0.0.tar.gz` & `tmp/basedmypy-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedmypy-2.0.0.tar", last modified: Fri Jul  7 10:26:51 2023, max compression
+gzip compressed data, was "basedmypy-2.0.0rc1.tar", last modified: Thu Jul  6 12:51:13 2023, max compression
```

## Comparing `basedmypy-2.0.0.tar` & `basedmypy-2.0.0rc1.tar`

### file list

```diff
@@ -1,1556 +1,1556 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.097070 basedmypy-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 10:26:08.000000 basedmypy-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-07 10:26:51.097070 basedmypy-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-07 10:26:08.000000 basedmypy-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.697065 basedmypy-2.0.0/basedmypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 10:26:50.000000 basedmypy-2.0.0/basedmypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 10:26:08.000000 basedmypy-2.0.0/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-07 10:26:08.000000 basedmypy-2.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.697065 basedmypy-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     6711 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.709066 basedmypy-2.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/additional_features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/based_features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/baseline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/builtin_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/cheat_sheet_py3.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/class_basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36377 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/common_issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    35820 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/config_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/duck_type_compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/dynamic_typing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/error_code_list.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/error_code_list2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/error_codes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/existing_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/extending_mypy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/final_attrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30636 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/generics.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/html_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/inline_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/installed_packages.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24825 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/kinds_of_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/literal_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/metaclasses.rst
--rw-r--r--   0 runner    (1001) docker     (123)    33198 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/more_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/mypy_daemon.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/mypy_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/running_mypy.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/runtime_troubles.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/stubgen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/stubs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/stubtest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/supported_python_features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/type_inference_and_annotations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/type_narrowing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/source/typed_dict.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.709066 basedmypy-2.0.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)  1155079 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)  1123389 2023-07-07 10:26:08.000000 basedmypy-2.0.0/docs/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.713066 basedmypy-2.0.0/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-07 10:26:08.000000 basedmypy-2.0.0/misc/proper_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.745066 basedmypy-2.0.0/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/applytype.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/argmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/binder.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/bogus_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   152026 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/build.py
--rw-r--r--   0 runner    (1001) docker     (123)   361120 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)   250842 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/checkexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    51394 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/checkmember.py
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/checkpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    45859 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/checkstrformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/constant_fold.py
--rw-r--r--   0 runner    (1001) docker     (123)    56094 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/copytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.745066 basedmypy-2.0.0/mypy/dmypy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24637 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy_os.py
--rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/dmypy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/erasetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    55674 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/evalexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/expandtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/exprtotype.py
--rw-r--r--   0 runner    (1001) docker     (123)    83491 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/fastparse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/fastparse2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/find_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/fixup.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/freetree.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/fscache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/fswatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/gclogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/indirection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/inspections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    59591 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/maptype.py
--rw-r--r--   0 runner    (1001) docker     (123)    41184 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/meet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/memprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/message_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   125621 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/metastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/mixedtraverser.py
--rw-r--r--   0 runner    (1001) docker     (123)    39359 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/modulefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/moduleinspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/mro.py
--rw-r--r--   0 runner    (1001) docker     (123)   133334 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/partially_defined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.749066 basedmypy-2.0.0/mypy/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    37276 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/default.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/plugins/singledispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/pyinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/refinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    34170 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)   303979 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_classprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_newtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_pass1.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_typeargs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/semanal_typeddict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.749066 basedmypy-2.0.0/mypy/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/astdiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/astmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/aststrip.py
--rw-r--r--   0 runner    (1001) docker     (123)    49962 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/mergecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/objgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/subexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    53008 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/server/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/sharedparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/split_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    23401 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/strconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubdoc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    74519 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24880 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubgenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/stubutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    79273 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/subtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    38046 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/suggestions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.761066 basedmypy-2.0.0/mypy/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/test_find_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/test_ref_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testargs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testcmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testconstraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testdaemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testdeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testdiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testerrorstream.py
--rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testfinegrained.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testfinegrainedcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testfscache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testinfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testmodulefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testmypyc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testpep561.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testpythoneval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testreports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testsemanal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testsolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    52599 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/teststubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/teststubinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    64523 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/teststubtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testsubtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testtransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testtypegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    60277 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testupdatedata.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/typefixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/update_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/test/visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26849 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/traverser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/treetransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/tvar_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/type_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    91942 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeanal.py
--rw-r--r--   0 runner    (1001) docker     (123)    45750 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeops.py
--rw-r--r--   0 runner    (1001) docker     (123)   132586 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/types_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.761066 basedmypy-2.0.0/mypy/typeshed/
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.817067 basedmypy-2.0.0/mypy/typeshed/stdlib/
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/VERSIONS
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/__future__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_ast.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_bisect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_bootlocale.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_codecs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_collections_abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_compat_pickle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_compression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_csv.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_ctypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_curses.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_decimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_dummy_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_dummy_threading.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_heapq.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_imp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_json.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_markupbase.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_msi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_operator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_osx_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_posixsubprocess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_py_abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_pydecimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_random.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_sitebuiltins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_socket.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_stat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_threading_local.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_tkinter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_tracemalloc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.817067 basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/dbapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/xml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_weakref.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_weakrefset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/aifc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/antigravity.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20275 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/argparse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/array.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ast.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asynchat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.829067 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/coroutines.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/locks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/protocols.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/queues.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/runners.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/selector_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/sslproto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/staggered.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/streams.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/subprocess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/taskgroups.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/threads.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/timeouts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/transports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/trsock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/unix_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/windows_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/asyncore.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/atexit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/audioop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/base64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/bdb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/binascii.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/binhex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/bisect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    83441 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/bz2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/cProfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/calendar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/cgi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/cgitb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/chunk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/cmath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/cmd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/codecs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/codeop.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.829067 basedmypy-2.0.0/mypy/typeshed/stdlib/collections/
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/collections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/collections/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/colorsys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/compileall.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.829067 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.829067 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/process.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/configparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/contextlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/contextvars.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/copy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/copyreg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/csv.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.833067 basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/wintypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.833067 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/ascii.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/has_key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/panel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/curses/textpad.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dataclasses.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/datetime.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.833067 basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/dumb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/gnu.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/ndbm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/decimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/difflib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dis.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.841067 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.849067 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/clean.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/dir_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/file_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/spawn.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/text_file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/doctest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/dummy_threading.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.853067 basedmypy-2.0.0/mypy/typeshed/stdlib/email/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/_header_value_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/base64mime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/charset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/contentmanager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/encoders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/feedparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/generator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/header.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/headerregistry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/iterators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/message.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/application.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/multipart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/mime/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/policy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/quoprimime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/email/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/utf_8.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/ensurepip/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ensurepip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/errno.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/faulthandler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/fcntl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/filecmp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/fileinput.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/formatter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/fractions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ftplib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/functools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/gc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/genericpath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/getopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/getpass.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/gettext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/graphlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/grp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/gzip.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/hashlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/heapq.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/hmac.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/html/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/html/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/html/entities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/html/parser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/http/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/http/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/http/cookiejar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/http/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/http/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/imaplib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/imghdr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/imp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/machinery.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/resources/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/inspect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/io.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ipaddress.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/itertools.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.861067 basedmypy-2.0.0/mypy/typeshed/stdlib/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/json/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/json/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/json/tool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/keyword.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.865068 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/btm_matcher.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixer_base.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.881068 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_apply.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_asserts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_basestring.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_buffer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_except.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_exec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_execfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_exitfunc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_filter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_funcattrs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_future.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_getcwdu.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_has_key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_idioms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_import.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_input.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_intern.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_isinstance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools_imports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_long.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_map.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_metaclass.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_methodattrs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_ne.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_next.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_nonzero.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_numliterals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_operator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_paren.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_print.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_raise.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_raw_input.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_reduce.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_reload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_renames.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_repr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_set_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_standarderror.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_sys_exc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_throw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_tuple_params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_unicode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_urllib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_ws_comma.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_xrange.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_xreadlines.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_zip.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/main.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.885068 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pygram.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pytree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/refactor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/linecache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/locale.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.885068 basedmypy-2.0.0/mypy/typeshed/stdlib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/logging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/logging/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/logging/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/lzma.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/macpath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/mailbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/mailcap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/marshal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/math.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/mimetypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/mmap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/modulefinder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.885068 basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/msvcrt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.893068 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.893068 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/forkserver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/heap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/managers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/pool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_fork.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_forkserver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_spawn_posix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_spawn_win32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/process.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/queues.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/reduction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/resource_sharer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/resource_tracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/netrc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/nis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/nntplib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ntpath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/nturl2path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/opcode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/operator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/optparse.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.893068 basedmypy-2.0.0/mypy/typeshed/stdlib/os/
--rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/os/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/os/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ossaudiodev.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pathlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pdb.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pickle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pickletools.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pipes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pkgutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/platform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/plistlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/poplib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/posix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/posixpath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pprint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/profile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pstats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pty.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pwd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/py_compile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pyclbr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pydoc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.893068 basedmypy-2.0.0/mypy/typeshed/stdlib/pydoc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pydoc_data/topics.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.893068 basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/queue.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/quopri.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/random.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/re.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/readline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/reprlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/rlcompleter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/runpy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sched.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/select.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/selectors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/shelve.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/shlex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/shutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/signal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/site.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/smtpd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/smtplib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sndhdr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/socketserver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/spwd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.897068 basedmypy-2.0.0/mypy/typeshed/stdlib/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sqlite3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sre_compile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sre_constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sre_parse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18327 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/ssl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/stat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/statistics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/string.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/stringprep.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/struct.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    91091 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/subprocess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sunau.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/symbol.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/symtable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/syslog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tabnanny.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tarfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/telnetlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tempfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/termios.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/textwrap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/this.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/threading.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/time.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/timeit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.901068 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/
--rw-r--r--   0 runner    (1001) docker     (123)   134288 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/commondialog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/dialog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/dnd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/filedialog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/font.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/messagebox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/tix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44712 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/ttk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tomllib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/trace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/traceback.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tracemalloc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/tty.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/turtle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/typing_extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unicodedata.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.905068 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/_log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/async_case.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/case.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/main.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/suite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.905068 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/parse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/robotparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/uu.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/uuid.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.905068 basedmypy-2.0.0/mypy/typeshed/stdlib/venv/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/venv/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wave.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/weakref.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/webbrowser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/winreg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/winsound.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.909068 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/validate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xdrlib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.909068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.913068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/domreg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/minidom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.913068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.913068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.913068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/expat/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.917068 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.917068 basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/xxlimited.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/zipapp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/zipfile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/zipimport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/zlib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.917068 basedmypy-2.0.0/mypy/typeshed/stdlib/zoneinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.681065 basedmypy-2.0.0/mypy/typeshed/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.917068 basedmypy-2.0.0/mypy/typeshed/stubs/mypy-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typestate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typetraverser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typevars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/typevartuples.py
--rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/versionutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    15882 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.917068 basedmypy-2.0.0/mypy/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/xml/mypy-html.css
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/xml/mypy-html.xslt
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/xml/mypy-txt.xslt
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy/xml/mypy.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy_bootstrap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypy_self_check.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.921068 basedmypy-2.0.0/mypyc/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.925068 basedmypy-2.0.0/mypyc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/attrdefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/blockfreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/ircheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/analysis/selfleaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.925068 basedmypy-2.0.0/mypyc/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/cstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    45913 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/emitclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    32111 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/emitfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45702 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/emitmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    37928 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/emitwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/codegen/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/crash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.933068 basedmypy-2.0.0/mypyc/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/bool_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/compilation_units.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/cpython-timings.md
--rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/dev-intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/dict_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/differences_from_python.rst
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/float_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/future.md
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/int_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/list_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/native_classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/native_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/performance_tips_and_tricks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/set_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/str_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/tuple_operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/doc/using_type_annotations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.681065 basedmypy-2.0.0/mypyc/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.933068 basedmypy-2.0.0/mypyc/external/googletest/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.681065 basedmypy-2.0.0/mypyc/external/googletest/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.933068 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/
--rw-r--r--   0 runner    (1001) docker     (123)    11523 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-death-test.h
--rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-message.h
--rw-r--r--   0 runner    (1001) docker     (123)    77062 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-param-test.h
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-param-test.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)    36806 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-spi.h
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-test-part.h
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-typed-test.h
--rw-r--r--   0 runner    (1001) docker     (123)    85459 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest.h
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest_prod.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.937068 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.937068 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 runner    (1001) docker     (123)    47284 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-linked_ptr.h
--rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0 runner    (1001) docker     (123)    90022 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-string.h
--rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)   185666 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h.pump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.941068 basedmypy-2.0.0/mypyc/external/googletest/make/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/make/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.941068 basedmypy-2.0.0/mypyc/external/googletest/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-all.cc
--rw-r--r--   0 runner    (1001) docker     (123)    50942 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-death-test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-filepath.cc
--rw-r--r--   0 runner    (1001) docker     (123)    45475 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-internal-inl.h
--rw-r--r--   0 runner    (1001) docker     (123)    42985 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-port.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-printers.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-test-part.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest-typed-test.cc
--rw-r--r--   0 runner    (1001) docker     (123)   195751 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/external/googletest/src/gtest_main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.945068 basedmypy-2.0.0/mypyc/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/class_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/func_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/module_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    45902 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    31758 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/ir/rtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.953069 basedmypy-2.0.0/mypyc/irbuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    55651 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/callable_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/classdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/constant_fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/env_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    38818 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    39520 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/for_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/format_str_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41812 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    97428 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/ll_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/nonlocalcontrol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/prebuildvisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/specialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    35303 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/irbuild/vtable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.961068 basedmypy-2.0.0/mypyc/lib-rt/
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/CPy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/bytes_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/dict_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/exc_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/float_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/generic_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/getargs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/getargsfast.c
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/init.c
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/int_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/list_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)    30958 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/misc_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/module_shim.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/mypyc_util.h
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/pythoncapi_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/pythonsupport.h
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/set_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/str_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/test_capi.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/lib-rt/tuple_ops.c
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/namegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.965069 basedmypy-2.0.0/mypyc/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/bytes_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/dict_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/exc_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/float_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/generic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/int_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/list_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/misc_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/set_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/str_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/primitives/tuple_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/rt_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/sametype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/subtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.977069 basedmypy-2.0.0/mypyc/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_alwaysdefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_cheader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_commandline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_emitclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    32815 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_emitfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_emitwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_irbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_ircheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_namegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_rarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_tuplename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/test_typeops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.993069 basedmypy-2.0.0/mypyc/test-data/
--rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/alwaysdefined.test
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/analysis.test
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/commandline.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.993069 basedmypy-2.0.0/mypyc/test-data/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/driver/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/exceptions-freq.test
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/exceptions.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.993069 basedmypy-2.0.0/mypyc/test-data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/fixtures/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/fixtures/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/fixtures/typing-full.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-any.test
--rw-r--r--   0 runner    (1001) docker     (123)    70646 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-basic.test
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-bool.test
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-bytes.test
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-classes.test
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-constant-fold.test
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-dict.test
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-dunders.test
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-float.test
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-generics.test
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-glue-methods.test
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-i32.test
--rw-r--r--   0 runner    (1001) docker     (123)    36084 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-i64.test
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-int.test
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-isinstance.test
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-lists.test
--rw-r--r--   0 runner    (1001) docker     (123)    35078 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-match.test
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-math.test
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-nested.test
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-optional.test
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-set.test
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-singledispatch.test
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-statements.test
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-str.test
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-strip-asserts.test
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-try.test
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-tuple.test
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-unreachable.test
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/irbuild-vectorcall.test
--rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/refcount.test
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-async.test
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-attrs.test
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-bench.test
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-bools.test
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-bytes.test
--rw-r--r--   0 runner    (1001) docker     (123)    49505 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-classes.test
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-dicts.test
--rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-dunders.test
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-exceptions.test
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-floats.test
--rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-functions.test
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-generators.test
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-i32.test
--rw-r--r--   0 runner    (1001) docker     (123)    35450 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-i64.test
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-imports.test
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-integers.test
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-lists.test
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-loops.test
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-match.test
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-math.test
--rw-r--r--   0 runner    (1001) docker     (123)    25066 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-misc.test
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-multimodule.test
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-mypy-sim.test
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-primitives.test
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-python37.test
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-python38.test
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-sets.test
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-singledispatch.test
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-strings.test
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-traits.test
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/test-data/run-tuples.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/mypyc/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/transform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/transform/refcount.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-07 10:26:08.000000 basedmypy-2.0.0/mypyc/transform/uninit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-07 10:26:08.000000 basedmypy-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 10:26:08.000000 basedmypy-2.0.0/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     4292 2023-07-07 10:26:08.000000 basedmypy-2.0.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 10:26:51.097070 basedmypy-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-07-07 10:26:08.000000 basedmypy-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.693066 basedmypy-2.0.0/test-data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg1/nsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg1/nsx/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg1/nsx/a/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg2/nsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg2/nsx/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg2/nsx/b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg3/nsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg3/nsx/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg3/nsx/c/c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsx-pkg3/nsx/c/c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg1/nsy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg1/nsy/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg1/nsy/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg1/nsy/a/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/b.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/c.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/nsy-pkg2/nsy/c.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/pkg1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/pkg1/a
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/pkg1/a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder/pkg2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/modulefinder/pkg2/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/pkg2/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.685065 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/baz_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/baz_pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/baz_pkg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/foo-stubs/bar.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_typed/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_typed/a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_typed/b/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_typed/b/c.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_typed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.997069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/b/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/b/c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.685065 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/untyped/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/untyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.685065 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/typed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/typed/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/b/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/b/c.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_typed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/b/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/pkg_untyped/b/c.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-site-packages/standalone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.689065 basedmypy-2.0.0/test-data/packages/modulefinder-src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-src/neighbor_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-src/neighbor_pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-src/neighbor_pkg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.001069 basedmypy-2.0.0/test-data/packages/modulefinder-src/ns_neighbor_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-src/ns_neighbor_pkg/a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/modulefinder-src/ns_neighbor_pkg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/typedpkg/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/dne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/pkg/aaa.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/pkg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg/typedpkg/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.005069 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/typedpkg-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/typedpkg-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/typedpkg-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg-stubs/typedpkg-stubs/sample.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/bbb.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/typedpkg_ns/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/typedpkg_ns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/bbb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.693066 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.009069 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/bbb.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.013069 basedmypy-2.0.0/test-data/pybind11_mypy_demo/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/pybind11_mypy_demo/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/pybind11_mypy_demo/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.013069 basedmypy-2.0.0/test-data/pybind11_mypy_demo/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/pybind11_mypy_demo/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:50.693066 basedmypy-2.0.0/test-data/pybind11_mypy_demo/stubgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.013069 basedmypy-2.0.0/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/basics.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.061070 basedmypy-2.0.0/test-data/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    42164 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-abstract.test
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-annotated.test
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-assert-type-fail.test
--rw-r--r--   0 runner    (1001) docker     (123)    30739 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-async-await.test
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-bare-literals.test
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-default-return.test
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-generic-typevar-bound.test
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-ignore-any-from-error.test
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-incomplete-defs.test
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-infer-function-types.test
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-intersection.test
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-tuple-literal.test
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-type-render.test
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-union-join.test
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-unsafe-variance.test
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-based-untyped.test
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-basic.test
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-bound.test
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-callable.test
--rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-class-namedtuple.test
--rw-r--r--   0 runner    (1001) docker     (123)   215939 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-classes.test
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-classvar.test
--rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-columns.test
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-ctypes.test
--rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-custom-plugin.test
--rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-dataclass-transform.test
--rw-r--r--   0 runner    (1001) docker     (123)    54501 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-dataclasses.test
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-dynamic-typing.test
--rw-r--r--   0 runner    (1001) docker     (123)    63494 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-enum.test
--rw-r--r--   0 runner    (1001) docker     (123)    38320 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-errorcodes.test
--rw-r--r--   0 runner    (1001) docker     (123)    61694 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-expressions.test
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-fastparse.test
--rw-r--r--   0 runner    (1001) docker     (123)    30815 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-final.test
--rw-r--r--   0 runner    (1001) docker     (123)    57176 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-flags.test
--rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-formatting.test
--rw-r--r--   0 runner    (1001) docker     (123)    81858 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-functions.test
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-functools.test
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-generic-alias.test
--rw-r--r--   0 runner    (1001) docker     (123)    30434 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-generic-subtyping.test
--rw-r--r--   0 runner    (1001) docker     (123)    76773 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-generics.test
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-ignore.test
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-incomplete-fixture.test
--rw-r--r--   0 runner    (1001) docker     (123)   125858 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-incremental.test
--rw-r--r--   0 runner    (1001) docker     (123)    37744 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-inference-context.test
--rw-r--r--   0 runner    (1001) docker     (123)    94339 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-inference.test
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-inline-config.test
--rw-r--r--   0 runner    (1001) docker     (123)    78974 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-isinstance.test
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-kwargs.test
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-lists.test
--rw-r--r--   0 runner    (1001) docker     (123)   107115 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-literal.test
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-lowercase.test
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-modules-case.test
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-modules-fast.test
--rw-r--r--   0 runner    (1001) docker     (123)    79380 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-modules.test
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-multiple-inheritance.test
--rw-r--r--   0 runner    (1001) docker     (123)    39906 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-namedtuple.test
--rw-r--r--   0 runner    (1001) docker     (123)    45227 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-narrowing.test
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-native-int.test
--rw-r--r--   0 runner    (1001) docker     (123)    76787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-newsemanal.test
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-newsyntax.test
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-newtype.test
--rw-r--r--   0 runner    (1001) docker     (123)    35200 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-optional.test
--rw-r--r--   0 runner    (1001) docker     (123)   178876 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-overloading.test
--rw-r--r--   0 runner    (1001) docker     (123)    52495 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-parameter-specification.test
--rw-r--r--   0 runner    (1001) docker     (123)    56373 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-plugin-attrs.test
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-possibly-undefined.test
--rw-r--r--   0 runner    (1001) docker     (123)   105645 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-protocols.test
--rw-r--r--   0 runner    (1001) docker     (123)    46873 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-python310.test
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-python311.test
--rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-python38.test
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-python39.test
--rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-recursive-types.test
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-redefine.test
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-reports.test
--rw-r--r--   0 runner    (1001) docker     (123)    55241 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-selftype.test
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-semanal-error.test
--rw-r--r--   0 runner    (1001) docker     (123)    30408 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-serialize.test
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-singledispatch.test
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-slots.test
--rw-r--r--   0 runner    (1001) docker     (123)    58590 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-statements.test
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-super.test
--rw-r--r--   0 runner    (1001) docker     (123)    46677 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-tuples.test
--rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-type-aliases.test
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-type-checks.test
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-type-promotion.test
--rw-r--r--   0 runner    (1001) docker     (123)    93440 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typeddict.test
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typeguard.test
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typevar-defaults.test
--rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typevar-tuple.test
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typevar-unbound.test
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-typevar-values.test
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-underscores.test
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-union-error-syntax.test
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-union-or-syntax.test
--rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-unions.test
--rw-r--r--   0 runner    (1001) docker     (123)    38441 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-unreachable-code.test
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-unsupported.test
--rw-r--r--   0 runner    (1001) docker     (123)    30967 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-varargs.test
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/check-warnings.test
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/cmdline-based-baseline.test
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/cmdline-based.test
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/cmdline.pyproject.test
--rw-r--r--   0 runner    (1001) docker     (123)    41364 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/cmdline.test
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/daemon-based.test
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/daemon.test
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps-classes.test
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps-expressions.test
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps-generics.test
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps-statements.test
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps-types.test
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/deps.test
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/diff.test
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/envvars.test
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/errorstream.test
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-attr.test
--rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-blockers.test
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-cache-incremental.test
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-cycles.test
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-dataclass-transform.test
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-follow-imports.test
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-inspect.test
--rw-r--r--   0 runner    (1001) docker     (123)    47853 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-modules.test
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained-suggest.test
--rw-r--r--   0 runner    (1001) docker     (123)   199051 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fine-grained.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.077070 basedmypy-2.0.0/test-data/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/__init_subclass__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/__new__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/any.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/args.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/async_await.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/bool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/callable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/classmethod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/complex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/complex_tuple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/dataclasses.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/divmod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/f_string.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/fine_grained.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/float.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/floatdict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/for.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/function.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/isinstance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/isinstance_python3_10.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/isinstancelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/module.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/module_all.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/narrowing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/notimplemented.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/object_hashable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/object_with_init_subclass.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/ops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/paramspec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/plugin_attrs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/primitives.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/property.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/set.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/slice.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/staticmethod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/tuple-simple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/tuple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/typing-async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/typing-full.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/typing-medium.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/typing-namedtuple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/typing-typeddict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/fixtures/union.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/hacks.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.085070 basedmypy-2.0.0/test-data/unit/lib-stub/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/_decimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/_typeshed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/abc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.085070 basedmypy-2.0.0/test-data/unit/lib-stub/attr/
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/attr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/attr/converters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.085070 basedmypy-2.0.0/test-data/unit/lib-stub/attrs/
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/attrs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/attrs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/basedtyping.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/blocker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/blocker2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/broken.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/collections.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/contextlib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/dataclasses.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/decimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/functools.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.089070 basedmypy-2.0.0/test-data/unit/lib-stub/future/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/future/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/future/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/helper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/math.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/mypy_extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/six.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/sys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/traceback.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/typing_extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/lib-stub/unannotated_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/merge.test
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/parse-errors.test
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/parse-python310.test
--rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/parse.test
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/pep561.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:51.097070 basedmypy-2.0.0/test-data/unit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/add_classmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/arg_kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/arg_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/attrhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/attrhook2.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/badreturn.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/badreturn2.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/callable_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/class_attr_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/class_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/common_api_incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/custom_errorcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/customentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/customize_mro.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/decimal_to_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/depshook.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/dyn_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/dyn_class_from_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/fnplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/fully_qualified_test_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/function_sig_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/method_in_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/method_sig_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/named_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/noentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/plugin2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/type_anal_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/plugins/union_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/pythoneval-asyncio.test
--rw-r--r--   0 runner    (1001) docker     (123)    56249 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/pythoneval.test
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/ref-info.test
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/reports.test
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-abstractclasses.test
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-basic.test
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-classes.test
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-classvar.test
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-errors-python310.test
--rw-r--r--   0 runner    (1001) docker     (123)    37948 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-errors.test
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-expressions.test
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-lambda.test
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-literal.test
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-modules.test
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-namedtuple.test
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-python310.test
--rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-statements.test
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-symtable.test
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-typealiases.test
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-typeddict.test
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-typeinfo.test
--rw-r--r--   0 runner    (1001) docker     (123)    31826 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/semanal-types.test
--rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/stubgen-based.test
--rw-r--r--   0 runner    (1001) docker     (123)    54798 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/stubgen.test
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-data/unit/typexport-basic.test
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 10:26:08.000000 basedmypy-2.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.257829 basedmypy-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-06 12:51:13.257829 basedmypy-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.953828 basedmypy-2.0.0rc1/basedmypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 12:51:12.000000 basedmypy-2.0.0rc1/basedmypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.953828 basedmypy-2.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6711 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.965828 basedmypy-2.0.0rc1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/additional_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/based_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/baseline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/builtin_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/cheat_sheet_py3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/class_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36377 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/common_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35820 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/config_file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/duck_type_compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/dynamic_typing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/error_code_list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/error_code_list2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/error_codes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/existing_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/extending_mypy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/final_attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30636 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/generics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/html_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/inline_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/installed_packages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24825 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/kinds_of_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/literal_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/metaclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    33198 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/more_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/mypy_daemon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/mypy_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/running_mypy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/runtime_troubles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/stubgen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/stubs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/stubtest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/supported_python_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/type_inference_and_annotations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/type_narrowing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/source/typed_dict.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.969828 basedmypy-2.0.0rc1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)  1155079 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1123389 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/docs/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.969828 basedmypy-2.0.0rc1/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/misc/proper_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.997828 basedmypy-2.0.0rc1/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/applytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/argmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/binder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/bogus_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152026 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)   361120 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)   251141 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/checkexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51394 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/checkmember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/checkpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45859 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/checkstrformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/constant_fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56094 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/copytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.997828 basedmypy-2.0.0rc1/mypy/dmypy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24637 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/dmypy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/erasetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55674 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/evalexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/expandtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/exprtotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83491 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/fastparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/fastparse2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/find_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/fixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/freetree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/fscache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/fswatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/gclogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/indirection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/inspections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59591 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/maptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41184 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/meet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/memprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/message_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125621 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/mixedtraverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39359 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/modulefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/moduleinspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/mro.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133334 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/partially_defined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.001828 basedmypy-2.0.0rc1/mypy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37276 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/plugins/singledispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/pyinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/refinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34170 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)   303979 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_classprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_newtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_pass1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_typeargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/semanal_typeddict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.001828 basedmypy-2.0.0rc1/mypy/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/astdiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/astmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/aststrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49962 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/mergecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/objgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/subexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53008 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/server/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/sharedparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/split_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23401 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/strconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubdoc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    74519 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24880 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubgenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/stubutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79273 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/subtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38046 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/suggestions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.009828 basedmypy-2.0.0rc1/mypy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/test_find_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/test_ref_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testcmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testconstraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testdaemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testdeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testdiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testerrorstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testfinegrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testfinegrainedcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testfscache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testinfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testmodulefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testmypyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testpep561.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testpythoneval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testreports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testsemanal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testsolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52599 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/teststubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/teststubinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64523 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/teststubtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testsubtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testtransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testtypegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60277 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testupdatedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/typefixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/update_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/test/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26849 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/traverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/treetransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/tvar_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/type_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91942 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeanal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45750 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeops.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132586 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/types_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.013828 basedmypy-2.0.0rc1/mypy/typeshed/
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.061828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/VERSIONS
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/__future__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_ast.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_bisect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_bootlocale.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_codecs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_collections_abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_compat_pickle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_compression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_csv.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_ctypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_curses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_decimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_dummy_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_dummy_threading.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_heapq.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_imp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_json.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_markupbase.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_msi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_operator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_osx_support.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_posixsubprocess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_py_abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_pydecimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_random.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_sitebuiltins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_stat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_threading_local.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_tkinter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_tracemalloc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.061828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/dbapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/xml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_weakref.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_weakrefset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/aifc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/antigravity.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20275 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/argparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ast.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asynchat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/coroutines.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/locks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/protocols.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/queues.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/runners.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/selector_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/sslproto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/staggered.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/streams.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/subprocess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/taskgroups.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/threads.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/timeouts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/transports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/trsock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/unix_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/windows_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncore.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/atexit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/audioop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/base64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/bdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/binascii.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/binhex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/bisect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    83441 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/bz2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cProfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/calendar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cgitb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/chunk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cmath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cmd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/codecs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/codeop.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/collections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/collections/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/colorsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/compileall.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/configparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/contextlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/contextvars.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/copy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/copyreg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/csv.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/wintypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.069828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/ascii.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/has_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/panel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/textpad.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dataclasses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/datetime.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.073829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/dumb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/gnu.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/ndbm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/decimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/difflib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dis.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.077829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.081828 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/clean.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/dir_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/file_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/spawn.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/text_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/doctest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dummy_threading.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.085829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/_header_value_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/base64mime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/contentmanager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/encoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/feedparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/header.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/headerregistry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/iterators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/message.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.085829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/application.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/multipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/mime/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/quoprimime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.085829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/utf_8.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ensurepip/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ensurepip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/errno.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/faulthandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fcntl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/filecmp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fileinput.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/formatter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fractions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ftplib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/functools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/genericpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/getopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/getpass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gettext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/graphlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/grp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/hashlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/heapq.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/hmac.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/html/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/html/entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/html/parser.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/cookiejar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/imaplib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/imghdr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/imp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/machinery.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.089829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/resources/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/inspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ipaddress.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/itertools.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.093829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/tool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/keyword.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.093829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/btm_matcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixer_base.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.101829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_apply.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_asserts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_basestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_buffer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_except.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_exec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_execfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_exitfunc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_funcattrs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_future.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_getcwdu.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_has_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_idioms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_import.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_input.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_intern.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_isinstance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_itertools_imports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_long.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_map.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_metaclass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_methodattrs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_ne.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_next.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_nonzero.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_numliterals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_operator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_paren.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_print.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_raise.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_raw_input.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_reduce.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_reload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_renames.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_set_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_standarderror.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_sys_exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_throw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_tuple_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_unicode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_urllib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_ws_comma.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_xrange.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_xreadlines.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_zip.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/main.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.105829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pygram.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pytree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/refactor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/linecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/locale.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.105829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lzma.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/macpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mailbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mailcap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/marshal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mimetypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/modulefinder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.105829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msvcrt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.109829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.109829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/forkserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/heap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/managers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_fork.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_forkserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_spawn_posix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_spawn_win32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/queues.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/reduction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/resource_sharer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/resource_tracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/netrc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/nis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/nntplib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ntpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/nturl2path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/opcode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/operator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/optparse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.109829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/os/
+-rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/os/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/os/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ossaudiodev.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pathlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pickle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pickletools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pipes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pkgutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/platform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/plistlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/poplib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/posix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/posixpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pprint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/profile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pstats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pty.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pwd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/py_compile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyclbr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pydoc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.113829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pydoc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pydoc_data/topics.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.113829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/quopri.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/re.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/readline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/reprlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/rlcompleter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/runpy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sched.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/select.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/selectors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shelve.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shlex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/signal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/site.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/smtpd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/smtplib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sndhdr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/socketserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/spwd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.113829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sqlite3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sre_compile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sre_constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sre_parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18327 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ssl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/stat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/statistics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/string.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/stringprep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/struct.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    91091 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/subprocess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sunau.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/symbol.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/symtable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/syslog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tabnanny.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tarfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/telnetlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tempfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/termios.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/textwrap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/this.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/threading.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/time.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/timeit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.117829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/
+-rw-r--r--   0 runner    (1001) docker     (123)   134288 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/commondialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/dialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/dnd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/filedialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/font.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/messagebox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/tix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44712 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/ttk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tomllib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/trace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/traceback.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tracemalloc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tty.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/turtle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/typing_extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unicodedata.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.117829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/_log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/async_case.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/case.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/suite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.121829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/robotparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/uu.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/uuid.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.121829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/venv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/venv/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wave.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/weakref.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/webbrowser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/winreg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/winsound.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.121829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/validate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xdrlib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.121829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.121829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/domreg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/minidom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/expat/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xxlimited.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipapp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipimport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zlib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zoneinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.921828 basedmypy-2.0.0rc1/mypy/typeshed/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.125829 basedmypy-2.0.0rc1/mypy/typeshed/stubs/mypy-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typestate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typetraverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typevars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/typevartuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/versionutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15882 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.129829 basedmypy-2.0.0rc1/mypy/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/xml/mypy-html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/xml/mypy-html.xslt
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/xml/mypy-txt.xslt
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy/xml/mypy.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy_bootstrap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypy_self_check.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.129829 basedmypy-2.0.0rc1/mypyc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.133829 basedmypy-2.0.0rc1/mypyc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/attrdefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/blockfreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/ircheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/analysis/selfleaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.133829 basedmypy-2.0.0rc1/mypyc/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/cstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45913 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/emitclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32111 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/emitfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45702 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/emitmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37928 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/emitwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/codegen/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/crash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.137829 basedmypy-2.0.0rc1/mypyc/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/bool_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/compilation_units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/cpython-timings.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/dev-intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/dict_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/differences_from_python.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/float_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/future.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/int_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/list_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/native_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/native_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/performance_tips_and_tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/set_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/str_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/tuple_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/doc/using_type_annotations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.921828 basedmypy-2.0.0rc1/mypyc/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.137829 basedmypy-2.0.0rc1/mypyc/external/googletest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.921828 basedmypy-2.0.0rc1/mypyc/external/googletest/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.141829 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/
+-rw-r--r--   0 runner    (1001) docker     (123)    11523 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-death-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-message.h
+-rw-r--r--   0 runner    (1001) docker     (123)    77062 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-param-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-param-test.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)    36806 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-spi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-test-part.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-typed-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    85459 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest_prod.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.145829 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.145829 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47284 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-linked_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-port-arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    90022 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-string.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)   185666 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h.pump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.145829 basedmypy-2.0.0rc1/mypyc/external/googletest/make/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/make/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.145829 basedmypy-2.0.0rc1/mypyc/external/googletest/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-all.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    50942 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-death-test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-filepath.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    45475 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-internal-inl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42985 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-port.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-printers.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-test-part.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-typed-test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   195751 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest_main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.149829 basedmypy-2.0.0rc1/mypyc/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/class_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/func_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/module_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45902 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31758 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/ir/rtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.153829 basedmypy-2.0.0rc1/mypyc/irbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55651 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/callable_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/classdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/constant_fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/env_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38818 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39520 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/for_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/format_str_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41812 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97428 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/ll_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/nonlocalcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/prebuildvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/specialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35303 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/irbuild/vtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.161829 basedmypy-2.0.0rc1/mypyc/lib-rt/
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/CPy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/bytes_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/dict_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/exc_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/float_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/generic_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/getargs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/getargsfast.c
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/init.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/int_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/list_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30958 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/misc_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/module_shim.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/mypyc_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/pythoncapi_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/pythonsupport.h
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/set_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/str_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/test_capi.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/lib-rt/tuple_ops.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/namegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.161829 basedmypy-2.0.0rc1/mypyc/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/bytes_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/dict_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/exc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/float_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/generic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/int_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/list_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/misc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/set_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/str_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/primitives/tuple_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/rt_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/sametype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/subtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.165829 basedmypy-2.0.0rc1/mypyc/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_alwaysdefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_cheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_emitclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32815 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_emitfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_emitwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_irbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_ircheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_namegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_rarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_tuplename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/test_typeops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.181829 basedmypy-2.0.0rc1/mypyc/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/alwaysdefined.test
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/analysis.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/commandline.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.181829 basedmypy-2.0.0rc1/mypyc/test-data/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/driver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/exceptions-freq.test
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/exceptions.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.181829 basedmypy-2.0.0rc1/mypyc/test-data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/fixtures/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/fixtures/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/fixtures/typing-full.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-any.test
+-rw-r--r--   0 runner    (1001) docker     (123)    70646 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-basic.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-bool.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-bytes.test
+-rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-classes.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-constant-fold.test
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-dict.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-dunders.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-float.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-generics.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-glue-methods.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-i32.test
+-rw-r--r--   0 runner    (1001) docker     (123)    36084 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-i64.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-int.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-isinstance.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-lists.test
+-rw-r--r--   0 runner    (1001) docker     (123)    35078 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-match.test
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-math.test
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-nested.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-optional.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-set.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-singledispatch.test
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-statements.test
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-str.test
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-strip-asserts.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-try.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-tuple.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-unreachable.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/irbuild-vectorcall.test
+-rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/refcount.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-async.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-attrs.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-bench.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-bools.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-bytes.test
+-rw-r--r--   0 runner    (1001) docker     (123)    49505 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-classes.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-dicts.test
+-rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-dunders.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-exceptions.test
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-floats.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-functions.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-generators.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-i32.test
+-rw-r--r--   0 runner    (1001) docker     (123)    35450 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-i64.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-imports.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-integers.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-lists.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-loops.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-match.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-math.test
+-rw-r--r--   0 runner    (1001) docker     (123)    25066 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-misc.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-multimodule.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-mypy-sim.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-primitives.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-python37.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-python38.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-sets.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-singledispatch.test
+-rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-strings.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-traits.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/test-data/run-tuples.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.181829 basedmypy-2.0.0rc1/mypyc/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/transform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/transform/refcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/mypyc/transform/uninit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4292 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 12:51:13.257829 basedmypy-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.181829 basedmypy-2.0.0rc1/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.945828 basedmypy-2.0.0rc1/test-data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.937828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.937828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg1/nsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg1/nsx/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg1/nsx/a/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.937828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg2/nsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg2/nsx/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg2/nsx/b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg3/nsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg3/nsx/c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg3/nsx/c/c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsx-pkg3/nsx/c/c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg1/nsy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg1/nsy/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg1/nsy/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg1/nsy/a/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.941828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/b.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/c.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/nsy-pkg2/nsy/c.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg1/a
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg1/a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.945828 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg2/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/pkg2/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.929828 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/baz_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/baz_pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/baz_pkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/baz/ns_baz_pkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo/bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/foo-stubs/bar.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_typed/a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_typed/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_typed/b/c.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_typed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_untyped/b/c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.933828 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/typed_inline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/untyped/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs/untyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.933828 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.185829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/typed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/ns_pkg_w_stubs-stubs/typed/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/b/c.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_typed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/pkg_untyped/b/c.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-site-packages/standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.937828 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/neighbor_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/neighbor_pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/neighbor_pkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.189829 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/ns_neighbor_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/ns_neighbor_pkg/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/modulefinder-src/ns_neighbor_pkg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/dne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/pkg/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/pkg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg/typedpkg/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/typedpkg-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/typedpkg-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/typedpkg-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg-stubs/typedpkg-stubs/sample.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.193829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_a/typedpkg_ns/a/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/typedpkg_ns/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/typedpkg_ns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b/typedpkg_ns/b/bbb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.945828 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/packages/typedpkg_ns_b-stubs/typedpkg_ns-stubs/b/bbb.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:12.945828 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/stubgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.197829 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/basics.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.233829 basedmypy-2.0.0rc1/test-data/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42164 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-abstract.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-annotated.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-assert-type-fail.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30739 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-async-await.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-bare-literals.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-default-return.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-generic-typevar-bound.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-ignore-any-from-error.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-incomplete-defs.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-infer-function-types.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-intersection.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-tuple-literal.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-type-render.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-union-join.test
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-unsafe-variance.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-based-untyped.test
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-basic.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-bound.test
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-callable.test
+-rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-class-namedtuple.test
+-rw-r--r--   0 runner    (1001) docker     (123)   215939 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-classes.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-classvar.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-columns.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-ctypes.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-custom-plugin.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30453 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-dataclass-transform.test
+-rw-r--r--   0 runner    (1001) docker     (123)    54501 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-dataclasses.test
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-dynamic-typing.test
+-rw-r--r--   0 runner    (1001) docker     (123)    63494 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-enum.test
+-rw-r--r--   0 runner    (1001) docker     (123)    38320 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-errorcodes.test
+-rw-r--r--   0 runner    (1001) docker     (123)    61694 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-expressions.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-fastparse.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30815 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-final.test
+-rw-r--r--   0 runner    (1001) docker     (123)    57176 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-flags.test
+-rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-formatting.test
+-rw-r--r--   0 runner    (1001) docker     (123)    81858 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-functions.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-functools.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-generic-alias.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30434 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-generic-subtyping.test
+-rw-r--r--   0 runner    (1001) docker     (123)    76773 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-generics.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-ignore.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-incomplete-fixture.test
+-rw-r--r--   0 runner    (1001) docker     (123)   125858 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-incremental.test
+-rw-r--r--   0 runner    (1001) docker     (123)    37744 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-inference-context.test
+-rw-r--r--   0 runner    (1001) docker     (123)    94339 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-inference.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-inline-config.test
+-rw-r--r--   0 runner    (1001) docker     (123)    78974 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-isinstance.test
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-kwargs.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-lists.test
+-rw-r--r--   0 runner    (1001) docker     (123)   107115 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-literal.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-lowercase.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-modules-case.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-modules-fast.test
+-rw-r--r--   0 runner    (1001) docker     (123)    79380 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-modules.test
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-multiple-inheritance.test
+-rw-r--r--   0 runner    (1001) docker     (123)    39906 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-namedtuple.test
+-rw-r--r--   0 runner    (1001) docker     (123)    45227 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-narrowing.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-native-int.test
+-rw-r--r--   0 runner    (1001) docker     (123)    76787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-newsemanal.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-newsyntax.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-newtype.test
+-rw-r--r--   0 runner    (1001) docker     (123)    35200 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-optional.test
+-rw-r--r--   0 runner    (1001) docker     (123)   178876 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-overloading.test
+-rw-r--r--   0 runner    (1001) docker     (123)    52495 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-parameter-specification.test
+-rw-r--r--   0 runner    (1001) docker     (123)    56373 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-plugin-attrs.test
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-possibly-undefined.test
+-rw-r--r--   0 runner    (1001) docker     (123)   105645 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-protocols.test
+-rw-r--r--   0 runner    (1001) docker     (123)    46873 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-python310.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-python311.test
+-rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-python38.test
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-python39.test
+-rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-recursive-types.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-redefine.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-reports.test
+-rw-r--r--   0 runner    (1001) docker     (123)    55241 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-selftype.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-semanal-error.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30408 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-serialize.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-singledispatch.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-slots.test
+-rw-r--r--   0 runner    (1001) docker     (123)    58590 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-statements.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-super.test
+-rw-r--r--   0 runner    (1001) docker     (123)    46677 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-tuples.test
+-rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-type-aliases.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-type-checks.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-type-promotion.test
+-rw-r--r--   0 runner    (1001) docker     (123)    93440 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typeddict.test
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typeguard.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typevar-defaults.test
+-rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typevar-tuple.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typevar-unbound.test
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-typevar-values.test
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-underscores.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-union-error-syntax.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-union-or-syntax.test
+-rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-unions.test
+-rw-r--r--   0 runner    (1001) docker     (123)    38441 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-unreachable-code.test
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-unsupported.test
+-rw-r--r--   0 runner    (1001) docker     (123)    30967 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-varargs.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/check-warnings.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/cmdline-based-baseline.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/cmdline-based.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/cmdline.pyproject.test
+-rw-r--r--   0 runner    (1001) docker     (123)    41364 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/cmdline.test
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/daemon-based.test
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/daemon.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps-classes.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps-expressions.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps-generics.test
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps-statements.test
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps-types.test
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/deps.test
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/diff.test
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/envvars.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/errorstream.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-attr.test
+-rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-blockers.test
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-cache-incremental.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-cycles.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-dataclass-transform.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-follow-imports.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-inspect.test
+-rw-r--r--   0 runner    (1001) docker     (123)    47853 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-modules.test
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained-suggest.test
+-rw-r--r--   0 runner    (1001) docker     (123)   199051 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fine-grained.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.245829 basedmypy-2.0.0rc1/test-data/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/__init_subclass__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/__new__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/any.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/args.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/async_await.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/bool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/callable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/classmethod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/complex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/complex_tuple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/dataclasses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/divmod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/f_string.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/fine_grained.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/float.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/floatdict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/for.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/function.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstance_python3_10.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstancelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/module.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/module_all.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/narrowing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/notimplemented.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/object_hashable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/object_with_init_subclass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/paramspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/plugin_attrs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/primitives.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/property.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/set.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/slice.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/staticmethod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/tuple-simple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/tuple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-full.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-medium.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-namedtuple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-typeddict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/fixtures/union.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/hacks.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.249829 basedmypy-2.0.0rc1/test-data/unit/lib-stub/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/_decimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/_typeshed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/abc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.249829 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attr/converters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.249829 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attrs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attrs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/attrs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/basedtyping.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/blocker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/blocker2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/broken.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/contextlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/dataclasses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/decimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/functools.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.249829 basedmypy-2.0.0rc1/test-data/unit/lib-stub/future/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/future/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/future/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/mypy_extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/six.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/sys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/traceback.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/typing_extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/lib-stub/unannotated_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/merge.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/parse-errors.test
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/parse-python310.test
+-rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/parse.test
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/pep561.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:51:13.257829 basedmypy-2.0.0rc1/test-data/unit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/add_classmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/arg_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/arg_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/attrhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/attrhook2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/badreturn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/badreturn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/callable_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/class_attr_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/class_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/common_api_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/custom_errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/customentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/customize_mro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/decimal_to_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/depshook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/dyn_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/dyn_class_from_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/fnplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/fully_qualified_test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/function_sig_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/method_in_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/method_sig_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/named_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/noentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/plugin2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/type_anal_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/plugins/union_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/pythoneval-asyncio.test
+-rw-r--r--   0 runner    (1001) docker     (123)    56249 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/pythoneval.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/ref-info.test
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/reports.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-abstractclasses.test
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-basic.test
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-classes.test
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-classvar.test
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-errors-python310.test
+-rw-r--r--   0 runner    (1001) docker     (123)    37948 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-errors.test
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-expressions.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-lambda.test
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-literal.test
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-modules.test
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-namedtuple.test
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-python310.test
+-rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-statements.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-symtable.test
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-typealiases.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-typeddict.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-typeinfo.test
+-rw-r--r--   0 runner    (1001) docker     (123)    31826 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/semanal-types.test
+-rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/stubgen-based.test
+-rw-r--r--   0 runner    (1001) docker     (123)    54798 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/stubgen.test
+-rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-data/unit/typexport-basic.test
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-06 12:50:31.000000 basedmypy-2.0.0rc1/test-requirements.txt
```

### Comparing `basedmypy-2.0.0/LICENSE` & `basedmypy-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/MANIFEST.in` & `basedmypy-2.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/PKG-INFO` & `basedmypy-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedmypy
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Based static typing for Python
 Author: KotlinIsland
 License: MIT License
 Project-URL: News, https://github.com/KotlinIsland/basedmypy/releases
 Project-URL: Documentation, https://KotlinIsland.github.io/basedmypy
 Project-URL: Repository, https://github.com/KotlinIsland/basedmypy
 Project-URL: Discord, https://discord.gg/7y9upqPrk2
@@ -21,14 +21,17 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: dmypy
 Provides-Extra: reports
 Provides-Extra: install-types
 License-File: LICENSE
 
+Basedmypy -- Based Static Typing for Python
+===========================================
+
 .. image:: https://raw.githubusercontent.com/KotlinIsland/basedmypy/master/docs/static/logo-light.png
 
 Basedmypy is a type checker that is built on top of the work done by the
 `mypy project <https://github.com/python/mypy>`_. It adds based functionality and breaks compatibility with
 the cringe parts of pep 484.
 
 Based features
```

### Comparing `basedmypy-2.0.0/README.md` & `basedmypy-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/basedmypy.egg-info/PKG-INFO` & `basedmypy-2.0.0rc1/basedmypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedmypy
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Based static typing for Python
 Author: KotlinIsland
 License: MIT License
 Project-URL: News, https://github.com/KotlinIsland/basedmypy/releases
 Project-URL: Documentation, https://KotlinIsland.github.io/basedmypy
 Project-URL: Repository, https://github.com/KotlinIsland/basedmypy
 Project-URL: Discord, https://discord.gg/7y9upqPrk2
@@ -21,14 +21,17 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: dmypy
 Provides-Extra: reports
 Provides-Extra: install-types
 License-File: LICENSE
 
+Basedmypy -- Based Static Typing for Python
+===========================================
+
 .. image:: https://raw.githubusercontent.com/KotlinIsland/basedmypy/master/docs/static/logo-light.png
 
 Basedmypy is a type checker that is built on top of the work done by the
 `mypy project <https://github.com/python/mypy>`_. It adds based functionality and breaks compatibility with
 the cringe parts of pep 484.
 
 Based features
```

### Comparing `basedmypy-2.0.0/basedmypy.egg-info/SOURCES.txt` & `basedmypy-2.0.0rc1/basedmypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/conftest.py` & `basedmypy-2.0.0rc1/conftest.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/Makefile` & `basedmypy-2.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/README.md` & `basedmypy-2.0.0rc1/docs/README.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/make.bat` & `basedmypy-2.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/additional_features.rst` & `basedmypy-2.0.0rc1/docs/source/additional_features.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/based_features.rst` & `basedmypy-2.0.0rc1/docs/source/based_features.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/baseline.rst` & `basedmypy-2.0.0rc1/docs/source/baseline.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/builtin_types.rst` & `basedmypy-2.0.0rc1/docs/source/builtin_types.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/cheat_sheet_py3.rst` & `basedmypy-2.0.0rc1/docs/source/cheat_sheet_py3.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/class_basics.rst` & `basedmypy-2.0.0rc1/docs/source/class_basics.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/command_line.rst` & `basedmypy-2.0.0rc1/docs/source/command_line.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/common_issues.rst` & `basedmypy-2.0.0rc1/docs/source/common_issues.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/conf.py` & `basedmypy-2.0.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/config_file.rst` & `basedmypy-2.0.0rc1/docs/source/config_file.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/duck_type_compatibility.rst` & `basedmypy-2.0.0rc1/docs/source/duck_type_compatibility.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/dynamic_typing.rst` & `basedmypy-2.0.0rc1/docs/source/dynamic_typing.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/error_code_list.rst` & `basedmypy-2.0.0rc1/docs/source/error_code_list.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/error_code_list2.rst` & `basedmypy-2.0.0rc1/docs/source/error_code_list2.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/error_codes.rst` & `basedmypy-2.0.0rc1/docs/source/error_codes.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/existing_code.rst` & `basedmypy-2.0.0rc1/docs/source/existing_code.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/extending_mypy.rst` & `basedmypy-2.0.0rc1/docs/source/extending_mypy.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/faq.rst` & `basedmypy-2.0.0rc1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/final_attrs.rst` & `basedmypy-2.0.0rc1/docs/source/final_attrs.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/generics.rst` & `basedmypy-2.0.0rc1/docs/source/generics.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/getting_started.rst` & `basedmypy-2.0.0rc1/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/html_builder.py` & `basedmypy-2.0.0rc1/docs/source/html_builder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/index.rst` & `basedmypy-2.0.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/inline_config.rst` & `basedmypy-2.0.0rc1/docs/source/inline_config.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/installed_packages.rst` & `basedmypy-2.0.0rc1/docs/source/installed_packages.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/kinds_of_types.rst` & `basedmypy-2.0.0rc1/docs/source/kinds_of_types.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/literal_types.rst` & `basedmypy-2.0.0rc1/docs/source/literal_types.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/metaclasses.rst` & `basedmypy-2.0.0rc1/docs/source/metaclasses.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/more_types.rst` & `basedmypy-2.0.0rc1/docs/source/more_types.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/mypy_daemon.rst` & `basedmypy-2.0.0rc1/docs/source/mypy_daemon.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/mypy_light.svg` & `basedmypy-2.0.0rc1/docs/source/mypy_light.svg`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/protocols.rst` & `basedmypy-2.0.0rc1/docs/source/protocols.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/running_mypy.rst` & `basedmypy-2.0.0rc1/docs/source/running_mypy.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/runtime_troubles.rst` & `basedmypy-2.0.0rc1/docs/source/runtime_troubles.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/stubgen.rst` & `basedmypy-2.0.0rc1/docs/source/stubgen.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/stubs.rst` & `basedmypy-2.0.0rc1/docs/source/stubs.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/stubtest.rst` & `basedmypy-2.0.0rc1/docs/source/stubtest.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/supported_python_features.rst` & `basedmypy-2.0.0rc1/docs/source/supported_python_features.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/type_inference_and_annotations.rst` & `basedmypy-2.0.0rc1/docs/source/type_inference_and_annotations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/type_narrowing.rst` & `basedmypy-2.0.0rc1/docs/source/type_narrowing.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/source/typed_dict.rst` & `basedmypy-2.0.0rc1/docs/source/typed_dict.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/static/favicon.ico` & `basedmypy-2.0.0rc1/docs/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/static/logo-dark.png` & `basedmypy-2.0.0rc1/docs/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/docs/static/logo-light.png` & `basedmypy-2.0.0rc1/docs/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/misc/proper_plugin.py` & `basedmypy-2.0.0rc1/misc/proper_plugin.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/__main__.py` & `basedmypy-2.0.0rc1/mypy/__main__.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/api.py` & `basedmypy-2.0.0rc1/mypy/api.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/applytype.py` & `basedmypy-2.0.0rc1/mypy/applytype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/argmap.py` & `basedmypy-2.0.0rc1/mypy/argmap.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/binder.py` & `basedmypy-2.0.0rc1/mypy/binder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/bogus_type.py` & `basedmypy-2.0.0rc1/mypy/bogus_type.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/build.py` & `basedmypy-2.0.0rc1/mypy/build.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/checker.py` & `basedmypy-2.0.0rc1/mypy/checker.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/checkexpr.py` & `basedmypy-2.0.0rc1/mypy/checkexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5097,19 +5097,15 @@
         self.chk.store_type(node, typ)
 
         if (
             self.chk.options.disallow_any_expr
             and not always_allow_any
             and not self.chk.is_stub
             and self.chk.in_checked_function()
-            and has_any_type(
-                typ,
-                ignore_in_type_obj=True,
-                ignore_any_from_error=self.chk.options.hide_any_from_error,
-            )
+            and has_any_type(typ, ignore_any_from_error=self.chk.options.hide_any_from_error)
             and not self.chk.current_node_deferred
         ):
             self.msg.disallowed_any_type(typ, node)
 
         if not self.chk.in_checked_function() or self.chk.current_node_deferred:
             # this is more of a placeholder I think
             result: Type = AnyType(TypeOfAny.unannotated)
@@ -5465,17 +5461,24 @@
         return self.query_types([t.upper_bound, *default])
 
     def visit_type_var_tuple(self, t: TypeVarTupleType) -> bool:
         default = [t.default] if t.has_default() else []
         return self.query_types([t.upper_bound, *default])
 
 
-class HasUntypedType(HasAnyType):
+class HasUntypedType(types.TypeQuery[bool]):
     def __init__(self) -> None:
-        super().__init__(True, True)
+        super().__init__(any)
+
+    def visit_type_var(self, t: TypeVarType) -> bool:
+        # type var defaults are Any (from omitted generics), so catch it here
+        default = get_proper_type(t.default)
+        if isinstance(default, AnyType) and default.type_of_any == TypeOfAny.from_omitted_generics:
+            return self.query_types([t.upper_bound] + t.values)
+        return super().visit_type_var(t)
 
     def visit_any(self, t: AnyType) -> bool:
         return isinstance(t, UntypedType) or t.type_of_any in (
             TypeOfAny.unannotated,
             TypeOfAny.from_omitted_generics,
         )
```

### Comparing `basedmypy-2.0.0/mypy/checkmember.py` & `basedmypy-2.0.0rc1/mypy/checkmember.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/checkpattern.py` & `basedmypy-2.0.0rc1/mypy/checkpattern.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/checkstrformat.py` & `basedmypy-2.0.0rc1/mypy/checkstrformat.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/config_parser.py` & `basedmypy-2.0.0rc1/mypy/config_parser.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/constant_fold.py` & `basedmypy-2.0.0rc1/mypy/constant_fold.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/constraints.py` & `basedmypy-2.0.0rc1/mypy/constraints.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/copytype.py` & `basedmypy-2.0.0rc1/mypy/copytype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/defaults.py` & `basedmypy-2.0.0rc1/mypy/defaults.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/dmypy/client.py` & `basedmypy-2.0.0rc1/mypy/dmypy/client.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/dmypy_os.py` & `basedmypy-2.0.0rc1/mypy/dmypy_os.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/dmypy_server.py` & `basedmypy-2.0.0rc1/mypy/dmypy_server.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/dmypy_util.py` & `basedmypy-2.0.0rc1/mypy/dmypy_util.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/erasetype.py` & `basedmypy-2.0.0rc1/mypy/erasetype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/errorcodes.py` & `basedmypy-2.0.0rc1/mypy/errorcodes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/errors.py` & `basedmypy-2.0.0rc1/mypy/errors.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/evalexpr.py` & `basedmypy-2.0.0rc1/mypy/evalexpr.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/expandtype.py` & `basedmypy-2.0.0rc1/mypy/expandtype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/exprtotype.py` & `basedmypy-2.0.0rc1/mypy/exprtotype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/fastparse.py` & `basedmypy-2.0.0rc1/mypy/fastparse.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/find_sources.py` & `basedmypy-2.0.0rc1/mypy/find_sources.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/fixup.py` & `basedmypy-2.0.0rc1/mypy/fixup.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/freetree.py` & `basedmypy-2.0.0rc1/mypy/freetree.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/fscache.py` & `basedmypy-2.0.0rc1/mypy/fscache.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/fswatcher.py` & `basedmypy-2.0.0rc1/mypy/fswatcher.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/gclogger.py` & `basedmypy-2.0.0rc1/mypy/gclogger.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/git.py` & `basedmypy-2.0.0rc1/mypy/git.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/indirection.py` & `basedmypy-2.0.0rc1/mypy/indirection.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/infer.py` & `basedmypy-2.0.0rc1/mypy/infer.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/inspections.py` & `basedmypy-2.0.0rc1/mypy/inspections.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/ipc.py` & `basedmypy-2.0.0rc1/mypy/ipc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/join.py` & `basedmypy-2.0.0rc1/mypy/join.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/literals.py` & `basedmypy-2.0.0rc1/mypy/literals.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/lookup.py` & `basedmypy-2.0.0rc1/mypy/lookup.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/main.py` & `basedmypy-2.0.0rc1/mypy/main.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/maptype.py` & `basedmypy-2.0.0rc1/mypy/maptype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/meet.py` & `basedmypy-2.0.0rc1/mypy/meet.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/memprofile.py` & `basedmypy-2.0.0rc1/mypy/memprofile.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/message_registry.py` & `basedmypy-2.0.0rc1/mypy/message_registry.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/messages.py` & `basedmypy-2.0.0rc1/mypy/messages.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/metastore.py` & `basedmypy-2.0.0rc1/mypy/metastore.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/mixedtraverser.py` & `basedmypy-2.0.0rc1/mypy/mixedtraverser.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/modulefinder.py` & `basedmypy-2.0.0rc1/mypy/modulefinder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/moduleinspect.py` & `basedmypy-2.0.0rc1/mypy/moduleinspect.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/mro.py` & `basedmypy-2.0.0rc1/mypy/mro.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/nodes.py` & `basedmypy-2.0.0rc1/mypy/nodes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/operators.py` & `basedmypy-2.0.0rc1/mypy/operators.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/options.py` & `basedmypy-2.0.0rc1/mypy/options.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/parse.py` & `basedmypy-2.0.0rc1/mypy/parse.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/partially_defined.py` & `basedmypy-2.0.0rc1/mypy/partially_defined.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/patterns.py` & `basedmypy-2.0.0rc1/mypy/patterns.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugin.py` & `basedmypy-2.0.0rc1/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/attrs.py` & `basedmypy-2.0.0rc1/mypy/plugins/attrs.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/common.py` & `basedmypy-2.0.0rc1/mypy/plugins/common.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/ctypes.py` & `basedmypy-2.0.0rc1/mypy/plugins/ctypes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/dataclasses.py` & `basedmypy-2.0.0rc1/mypy/plugins/dataclasses.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/default.py` & `basedmypy-2.0.0rc1/mypy/plugins/default.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/enums.py` & `basedmypy-2.0.0rc1/mypy/plugins/enums.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/functools.py` & `basedmypy-2.0.0rc1/mypy/plugins/functools.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/plugins/singledispatch.py` & `basedmypy-2.0.0rc1/mypy/plugins/singledispatch.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/pyinfo.py` & `basedmypy-2.0.0rc1/mypy/pyinfo.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/reachability.py` & `basedmypy-2.0.0rc1/mypy/reachability.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/refinfo.py` & `basedmypy-2.0.0rc1/mypy/refinfo.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/renaming.py` & `basedmypy-2.0.0rc1/mypy/renaming.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/report.py` & `basedmypy-2.0.0rc1/mypy/report.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/scope.py` & `basedmypy-2.0.0rc1/mypy/scope.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal.py` & `basedmypy-2.0.0rc1/mypy/semanal.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_classprop.py` & `basedmypy-2.0.0rc1/mypy/semanal_classprop.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_enum.py` & `basedmypy-2.0.0rc1/mypy/semanal_enum.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_infer.py` & `basedmypy-2.0.0rc1/mypy/semanal_infer.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_main.py` & `basedmypy-2.0.0rc1/mypy/semanal_main.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_namedtuple.py` & `basedmypy-2.0.0rc1/mypy/semanal_namedtuple.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_newtype.py` & `basedmypy-2.0.0rc1/mypy/semanal_newtype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_pass1.py` & `basedmypy-2.0.0rc1/mypy/semanal_pass1.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_shared.py` & `basedmypy-2.0.0rc1/mypy/semanal_shared.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_typeargs.py` & `basedmypy-2.0.0rc1/mypy/semanal_typeargs.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/semanal_typeddict.py` & `basedmypy-2.0.0rc1/mypy/semanal_typeddict.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/astdiff.py` & `basedmypy-2.0.0rc1/mypy/server/astdiff.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/astmerge.py` & `basedmypy-2.0.0rc1/mypy/server/astmerge.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/aststrip.py` & `basedmypy-2.0.0rc1/mypy/server/aststrip.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/deps.py` & `basedmypy-2.0.0rc1/mypy/server/deps.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/mergecheck.py` & `basedmypy-2.0.0rc1/mypy/server/mergecheck.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/objgraph.py` & `basedmypy-2.0.0rc1/mypy/server/objgraph.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/subexpr.py` & `basedmypy-2.0.0rc1/mypy/server/subexpr.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/trigger.py` & `basedmypy-2.0.0rc1/mypy/server/trigger.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/server/update.py` & `basedmypy-2.0.0rc1/mypy/server/update.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/sharedparse.py` & `basedmypy-2.0.0rc1/mypy/sharedparse.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/solve.py` & `basedmypy-2.0.0rc1/mypy/solve.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/split_namespace.py` & `basedmypy-2.0.0rc1/mypy/split_namespace.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/state.py` & `basedmypy-2.0.0rc1/mypy/state.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stats.py` & `basedmypy-2.0.0rc1/mypy/stats.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/strconv.py` & `basedmypy-2.0.0rc1/mypy/strconv.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubdoc.py` & `basedmypy-2.0.0rc1/mypy/stubdoc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubgen.py` & `basedmypy-2.0.0rc1/mypy/stubgen.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubgenc.py` & `basedmypy-2.0.0rc1/mypy/stubgenc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubinfo.py` & `basedmypy-2.0.0rc1/mypy/stubinfo.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubtest.py` & `basedmypy-2.0.0rc1/mypy/stubtest.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/stubutil.py` & `basedmypy-2.0.0rc1/mypy/stubutil.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/subtypes.py` & `basedmypy-2.0.0rc1/mypy/subtypes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/suggestions.py` & `basedmypy-2.0.0rc1/mypy/suggestions.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/config.py` & `basedmypy-2.0.0rc1/mypy/test/config.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/data.py` & `basedmypy-2.0.0rc1/mypy/test/data.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/helpers.py` & `basedmypy-2.0.0rc1/mypy/test/helpers.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/test_find_sources.py` & `basedmypy-2.0.0rc1/mypy/test/test_find_sources.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/test_ref_info.py` & `basedmypy-2.0.0rc1/mypy/test/test_ref_info.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testapi.py` & `basedmypy-2.0.0rc1/mypy/test/testapi.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testargs.py` & `basedmypy-2.0.0rc1/mypy/test/testargs.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testcheck.py` & `basedmypy-2.0.0rc1/mypy/test/testcheck.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testcmdline.py` & `basedmypy-2.0.0rc1/mypy/test/testcmdline.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testconstraints.py` & `basedmypy-2.0.0rc1/mypy/test/testconstraints.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testdaemon.py` & `basedmypy-2.0.0rc1/mypy/test/testdaemon.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testdeps.py` & `basedmypy-2.0.0rc1/mypy/test/testdeps.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testdiff.py` & `basedmypy-2.0.0rc1/mypy/test/testdiff.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testerrorstream.py` & `basedmypy-2.0.0rc1/mypy/test/testerrorstream.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testfinegrained.py` & `basedmypy-2.0.0rc1/mypy/test/testfinegrained.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testfinegrainedcache.py` & `basedmypy-2.0.0rc1/mypy/test/testfinegrainedcache.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testformatter.py` & `basedmypy-2.0.0rc1/mypy/test/testformatter.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testfscache.py` & `basedmypy-2.0.0rc1/mypy/test/testfscache.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testgraph.py` & `basedmypy-2.0.0rc1/mypy/test/testgraph.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testinfer.py` & `basedmypy-2.0.0rc1/mypy/test/testinfer.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testipc.py` & `basedmypy-2.0.0rc1/mypy/test/testipc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testmerge.py` & `basedmypy-2.0.0rc1/mypy/test/testmerge.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testmodulefinder.py` & `basedmypy-2.0.0rc1/mypy/test/testmodulefinder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testparse.py` & `basedmypy-2.0.0rc1/mypy/test/testparse.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testpep561.py` & `basedmypy-2.0.0rc1/mypy/test/testpep561.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testpythoneval.py` & `basedmypy-2.0.0rc1/mypy/test/testpythoneval.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testreports.py` & `basedmypy-2.0.0rc1/mypy/test/testreports.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testsemanal.py` & `basedmypy-2.0.0rc1/mypy/test/testsemanal.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testsolve.py` & `basedmypy-2.0.0rc1/mypy/test/testsolve.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/teststubgen.py` & `basedmypy-2.0.0rc1/mypy/test/teststubgen.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/teststubtest.py` & `basedmypy-2.0.0rc1/mypy/test/teststubtest.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testsubtypes.py` & `basedmypy-2.0.0rc1/mypy/test/testsubtypes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testtransform.py` & `basedmypy-2.0.0rc1/mypy/test/testtransform.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testtypegen.py` & `basedmypy-2.0.0rc1/mypy/test/testtypegen.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testtypes.py` & `basedmypy-2.0.0rc1/mypy/test/testtypes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testupdatedata.py` & `basedmypy-2.0.0rc1/mypy/test/testupdatedata.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/testutil.py` & `basedmypy-2.0.0rc1/mypy/test/testutil.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/typefixture.py` & `basedmypy-2.0.0rc1/mypy/test/typefixture.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/update_data.py` & `basedmypy-2.0.0rc1/mypy/test/update_data.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/test/visitors.py` & `basedmypy-2.0.0rc1/mypy/test/visitors.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/traverser.py` & `basedmypy-2.0.0rc1/mypy/traverser.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/treetransform.py` & `basedmypy-2.0.0rc1/mypy/treetransform.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/tvar_scope.py` & `basedmypy-2.0.0rc1/mypy/tvar_scope.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/type_visitor.py` & `basedmypy-2.0.0rc1/mypy/type_visitor.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeanal.py` & `basedmypy-2.0.0rc1/mypy/typeanal.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeops.py` & `basedmypy-2.0.0rc1/mypy/typeops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/types.py` & `basedmypy-2.0.0rc1/mypy/types.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/types_utils.py` & `basedmypy-2.0.0rc1/mypy/types_utils.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/LICENSE` & `basedmypy-2.0.0rc1/mypy/typeshed/LICENSE`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/VERSIONS` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/VERSIONS`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/__future__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/__future__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_ast.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_ast.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_bisect.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_bisect.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_codecs.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_codecs.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_collections_abc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_collections_abc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_compression.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_compression.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_csv.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_csv.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_ctypes.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_ctypes.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_curses.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_curses.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_decimal.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_decimal.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_dummy_thread.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_dummy_thread.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_dummy_threading.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_dummy_threading.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_imp.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_imp.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_json.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_json.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_markupbase.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_markupbase.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_msi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_msi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_operator.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_operator.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_osx_support.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_osx_support.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_posixsubprocess.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_posixsubprocess.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_pydecimal.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_pydecimal.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_sitebuiltins.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_sitebuiltins.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_socket.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_socket.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_stat.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_stat.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_thread.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_thread.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_threading_local.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_threading_local.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_tkinter.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_tkinter.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_tracemalloc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_tracemalloc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/dbapi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/dbapi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_typeshed/wsgi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_typeshed/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_warnings.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_warnings.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_weakref.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_weakref.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_weakrefset.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_weakrefset.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/_winapi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/abc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/abc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/aifc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/aifc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/argparse.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/argparse.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/array.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/array.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ast.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ast.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asynchat.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asynchat.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_events.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_events.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_futures.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_futures.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/coroutines.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/coroutines.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/events.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/events.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/exceptions.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/format_helpers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/format_helpers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/futures.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/futures.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/locks.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/locks.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/proactor_events.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/proactor_events.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/protocols.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/protocols.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/queues.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/queues.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/runners.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/runners.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/sslproto.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/sslproto.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/streams.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/streams.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/subprocess.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/taskgroups.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/taskgroups.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/tasks.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/tasks.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/timeouts.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/timeouts.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/transports.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/transports.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/trsock.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/trsock.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/unix_events.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/unix_events.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/windows_events.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/windows_events.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncio/windows_utils.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncio/windows_utils.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/asyncore.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/asyncore.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/audioop.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/audioop.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/base64.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/base64.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/bdb.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/bdb.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/binascii.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/binascii.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/binhex.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/binhex.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/builtins.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/builtins.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/bz2.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/bz2.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/cProfile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cProfile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/calendar.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/calendar.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/cgi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cgi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/cgitb.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cgitb.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/chunk.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/chunk.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/cmath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cmath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/cmd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/cmd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/code.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/code.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/codecs.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/codecs.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/collections/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/collections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/colorsys.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/colorsys.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/compileall.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/compileall.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/_base.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/_base.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/process.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/process.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/concurrent/futures/thread.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/concurrent/futures/thread.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/configparser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/configparser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/contextlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/contextlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/contextvars.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/contextvars.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/copyreg.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/copyreg.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/csv.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/csv.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ctypes/wintypes.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ctypes/wintypes.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/curses/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/curses/ascii.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/ascii.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/curses/panel.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/panel.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/curses/textpad.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/curses/textpad.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dataclasses.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/datetime.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/datetime.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/dumb.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/dumb.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/gnu.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/gnu.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dbm/ndbm.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dbm/ndbm.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/difflib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/difflib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/dis.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/dis.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/archive_util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/ccompiler.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/cmd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_clib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_ext.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_py.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/check.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/check.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/config.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/config.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/install_lib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/register.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/command/sdist.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/core.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/core.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/dist.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/errors.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/extension.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/filelist.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/log.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/log.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/sysconfig.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/text_file.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/text_file.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/distutils/version.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/distutils/version.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/doctest.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/doctest.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/_header_value_parser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/_header_value_parser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/base64mime.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/base64mime.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/charset.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/charset.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/errors.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/errors.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/feedparser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/feedparser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/generator.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/generator.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/header.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/header.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/headerregistry.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/headerregistry.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/iterators.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/iterators.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/message.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/message.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/parser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/parser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/policy.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/policy.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/quoprimime.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/quoprimime.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/email/utils.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/email/utils.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/utf_8.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/utf_8.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/enum.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/enum.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/errno.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/errno.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/faulthandler.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/faulthandler.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/fcntl.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fcntl.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/filecmp.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/filecmp.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/fileinput.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fileinput.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/formatter.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/formatter.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/fractions.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/fractions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ftplib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ftplib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/functools.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/functools.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/gc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/genericpath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/genericpath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/gettext.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gettext.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/glob.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/glob.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/graphlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/graphlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/grp.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/grp.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/gzip.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/gzip.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/hashlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/heapq.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/heapq.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/hmac.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/hmac.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/html/parser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/html/parser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/http/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/http/client.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/client.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/http/cookiejar.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/cookiejar.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/http/cookies.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/cookies.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/http/server.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/http/server.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/imaplib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/imaplib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/imp.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/imp.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/abc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/abc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/machinery.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/machinery.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/resources/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/resources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/importlib/util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/importlib/util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/inspect.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/inspect.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/io.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/io.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ipaddress.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ipaddress.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/itertools.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/itertools.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/json/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/json/decoder.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/decoder.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/json/encoder.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/json/encoder.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/keyword.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/keyword.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/btm_matcher.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/btm_matcher.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixer_base.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixer_base.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_import.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_import.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_imports.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_metaclass.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_metaclass.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_next.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_next.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_renames.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_renames.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_tuple_params.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_tuple_params.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_urllib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_urllib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/fixes/fix_xrange.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/fixes/fix_xrange.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/main.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/main.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pygram.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pygram.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/pytree.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/pytree.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lib2to3/refactor.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lib2to3/refactor.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/linecache.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/linecache.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/locale.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/locale.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/logging/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/logging/config.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/config.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/logging/handlers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/logging/handlers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/lzma.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/lzma.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/macpath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/macpath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/mailbox.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mailbox.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/marshal.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/marshal.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/math.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/math.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/mimetypes.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mimetypes.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/mmap.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/mmap.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/modulefinder.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/modulefinder.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/msilib/schema.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msilib/schema.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/msvcrt.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/msvcrt.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/connection.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/connection.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/context.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/context.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/forkserver.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/forkserver.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/heap.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/heap.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/managers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/managers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/pool.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/pool.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_fork.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_fork.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_spawn_posix.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_spawn_posix.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/popen_spawn_win32.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/popen_spawn_win32.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/process.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/process.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/queues.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/queues.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/reduction.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/reduction.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/resource_tracker.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/resource_tracker.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/spawn.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/spawn.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/multiprocessing/util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/multiprocessing/util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/netrc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/netrc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/nntplib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/nntplib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ntpath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ntpath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/numbers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/numbers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/opcode.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/opcode.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/operator.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/operator.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/optparse.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/optparse.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/os/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ossaudiodev.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ossaudiodev.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/parser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/parser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pathlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pathlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pdb.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pdb.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pickle.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pickle.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pickletools.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pickletools.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pkgutil.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pkgutil.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/platform.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/platform.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/plistlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/plistlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/poplib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/poplib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/posix.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/posix.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/posixpath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/posixpath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pprint.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pprint.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/profile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/profile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pstats.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pstats.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pty.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pty.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pwd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pwd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/py_compile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/py_compile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pyclbr.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyclbr.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pydoc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pydoc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/pyexpat/errors.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/pyexpat/errors.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/queue.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/queue.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/quopri.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/quopri.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/random.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/random.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/re.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/re.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/readline.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/readline.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/reprlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/reprlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/resource.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/resource.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/runpy.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/runpy.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sched.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sched.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/secrets.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/secrets.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/select.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/select.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/selectors.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/selectors.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/shelve.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shelve.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/shlex.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shlex.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/shutil.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/shutil.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/signal.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/signal.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/site.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/site.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/smtpd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/smtpd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/smtplib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/smtplib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/socket.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/socket.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/socketserver.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/socketserver.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/spwd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/spwd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sre_constants.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sre_constants.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sre_parse.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sre_parse.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/ssl.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/ssl.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/statistics.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/statistics.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/string.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/string.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/stringprep.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/stringprep.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/struct.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/struct.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/subprocess.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sunau.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sunau.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/symbol.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/symbol.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/symtable.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/symtable.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sys.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sys.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/sysconfig.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/syslog.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/syslog.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tabnanny.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tabnanny.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tarfile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tarfile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/telnetlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/telnetlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tempfile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tempfile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/termios.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/termios.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/textwrap.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/textwrap.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/threading.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/threading.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/time.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/time.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/timeit.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/timeit.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/colorchooser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/colorchooser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/constants.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/constants.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/dnd.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/dnd.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/filedialog.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/filedialog.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/font.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/font.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/messagebox.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/messagebox.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/simpledialog.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/simpledialog.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/tix.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/tix.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tkinter/ttk.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tkinter/ttk.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/token.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/token.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tokenize.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/trace.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/trace.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/traceback.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/traceback.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/tracemalloc.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/tracemalloc.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/turtle.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/turtle.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/types.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/types.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/typing.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/typing.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/typing_extensions.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/typing_extensions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unicodedata.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unicodedata.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/_log.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/_log.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/async_case.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/async_case.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/case.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/case.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/loader.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/loader.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/main.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/main.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/mock.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/mock.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/result.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/result.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/runner.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/runner.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/suite.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/suite.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/unittest/util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/unittest/util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/error.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/error.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/parse.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/request.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/request.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/response.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/response.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/urllib/robotparser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/urllib/robotparser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/uuid.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/uuid.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/venv/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/venv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/warnings.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/warnings.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wave.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wave.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/weakref.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/weakref.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/webbrowser.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/webbrowser.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/winreg.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/winreg.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/winsound.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/winsound.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/handlers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/handlers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/headers.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/headers.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/simple_server.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/simple_server.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/types.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/types.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/util.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/util.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/wsgiref/validate.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/wsgiref/validate.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xdrlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xdrlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/minicompat.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/minicompat.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/minidom.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/minidom.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/pulldom.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/pulldom.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/handler.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/handler.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/saxutils.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/saxutils.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/client.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/client.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/xmlrpc/server.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/xmlrpc/server.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/zipapp.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipapp.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/zipfile.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipfile.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/zipimport.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zipimport.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/zlib.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stdlib/zoneinfo/__init__.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stdlib/zoneinfo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi` & `basedmypy-2.0.0rc1/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typestate.py` & `basedmypy-2.0.0rc1/mypy/typestate.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typetraverser.py` & `basedmypy-2.0.0rc1/mypy/typetraverser.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typevars.py` & `basedmypy-2.0.0rc1/mypy/typevars.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/typevartuples.py` & `basedmypy-2.0.0rc1/mypy/typevartuples.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/util.py` & `basedmypy-2.0.0rc1/mypy/util.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/version.py` & `basedmypy-2.0.0rc1/mypy/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # - Dev versions have the form "1.2.3+dev" (PLUS sign to conform to PEP 440).
 # - Before 1.0 we had the form "0.NNN".
 __version__ = "1.4.1"
 base_version = __version__
 
 # friendly version information
 based_version_info = VersionInfo(
-    2, 0, 0, "final", 0, __version__.split("+dev")[0], "dev" if "+dev" in __version__ else "final"
+    2, 0, 0, "rc", 1, __version__.split("+dev")[0], "dev" if "+dev" in __version__ else "final"
 )
 # simple string version with git info
 __based_version__ = based_version_info.simple_str()
 # simple string version without git info
 base_based_version = __based_version__
 
 mypy_dir = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
```

### Comparing `basedmypy-2.0.0/mypy/versionutil.py` & `basedmypy-2.0.0rc1/mypy/versionutil.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/visitor.py` & `basedmypy-2.0.0rc1/mypy/visitor.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/xml/mypy-html.css` & `basedmypy-2.0.0rc1/mypy/xml/mypy-html.css`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/xml/mypy-html.xslt` & `basedmypy-2.0.0rc1/mypy/xml/mypy-html.xslt`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/xml/mypy-txt.xslt` & `basedmypy-2.0.0rc1/mypy/xml/mypy-txt.xslt`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy/xml/mypy.xsd` & `basedmypy-2.0.0rc1/mypy/xml/mypy.xsd`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy_bootstrap.ini` & `basedmypy-2.0.0rc1/mypy_bootstrap.ini`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypy_self_check.ini` & `basedmypy-2.0.0rc1/mypy_self_check.ini`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/README.md` & `basedmypy-2.0.0rc1/mypyc/README.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/__main__.py` & `basedmypy-2.0.0rc1/mypyc/__main__.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/analysis/attrdefined.py` & `basedmypy-2.0.0rc1/mypyc/analysis/attrdefined.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/analysis/blockfreq.py` & `basedmypy-2.0.0rc1/mypyc/analysis/blockfreq.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/analysis/dataflow.py` & `basedmypy-2.0.0rc1/mypyc/analysis/dataflow.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/analysis/ircheck.py` & `basedmypy-2.0.0rc1/mypyc/analysis/ircheck.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/analysis/selfleaks.py` & `basedmypy-2.0.0rc1/mypyc/analysis/selfleaks.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/build.py` & `basedmypy-2.0.0rc1/mypyc/build.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/cstring.py` & `basedmypy-2.0.0rc1/mypyc/codegen/cstring.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/emit.py` & `basedmypy-2.0.0rc1/mypyc/codegen/emit.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/emitclass.py` & `basedmypy-2.0.0rc1/mypyc/codegen/emitclass.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/emitfunc.py` & `basedmypy-2.0.0rc1/mypyc/codegen/emitfunc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/emitmodule.py` & `basedmypy-2.0.0rc1/mypyc/codegen/emitmodule.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/emitwrapper.py` & `basedmypy-2.0.0rc1/mypyc/codegen/emitwrapper.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/codegen/literals.py` & `basedmypy-2.0.0rc1/mypyc/codegen/literals.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/common.py` & `basedmypy-2.0.0rc1/mypyc/common.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/crash.py` & `basedmypy-2.0.0rc1/mypyc/crash.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/Makefile` & `basedmypy-2.0.0rc1/mypyc/doc/Makefile`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/compilation_units.rst` & `basedmypy-2.0.0rc1/mypyc/doc/compilation_units.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/conf.py` & `basedmypy-2.0.0rc1/mypyc/doc/conf.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/cpython-timings.md` & `basedmypy-2.0.0rc1/mypyc/doc/cpython-timings.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/dev-intro.md` & `basedmypy-2.0.0rc1/mypyc/doc/dev-intro.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/dict_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/dict_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/differences_from_python.rst` & `basedmypy-2.0.0rc1/mypyc/doc/differences_from_python.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/float_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/float_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/future.md` & `basedmypy-2.0.0rc1/mypyc/doc/future.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/getting_started.rst` & `basedmypy-2.0.0rc1/mypyc/doc/getting_started.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/index.rst` & `basedmypy-2.0.0rc1/mypyc/doc/index.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/int_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/int_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/introduction.rst` & `basedmypy-2.0.0rc1/mypyc/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/list_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/list_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/make.bat` & `basedmypy-2.0.0rc1/mypyc/doc/make.bat`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/native_classes.rst` & `basedmypy-2.0.0rc1/mypyc/doc/native_classes.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/native_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/native_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/performance_tips_and_tricks.rst` & `basedmypy-2.0.0rc1/mypyc/doc/performance_tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/set_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/set_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/str_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/str_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/tuple_operations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/tuple_operations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/doc/using_type_annotations.rst` & `basedmypy-2.0.0rc1/mypyc/doc/using_type_annotations.rst`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/errors.py` & `basedmypy-2.0.0rc1/mypyc/errors.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/LICENSE` & `basedmypy-2.0.0rc1/mypyc/external/googletest/LICENSE`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/README.md` & `basedmypy-2.0.0rc1/mypyc/external/googletest/README.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-death-test.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-message.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-param-test.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-param-test.h.pump` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-param-test.h.pump`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-printers.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-spi.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-test-part.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest-typed-test.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest_pred_impl.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/gtest_prod.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest-port.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest-port.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest-printers.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/custom/gtest.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/custom/gtest.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-death-test-internal.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-filepath.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-internal.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-linked_ptr.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-linked_ptr.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h.pump` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util-generated.h.pump`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-param-util.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-port-arch.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-port-arch.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-port.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-string.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h.pump` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-tuple.h.pump`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h.pump` & `basedmypy-2.0.0rc1/mypyc/external/googletest/include/gtest/internal/gtest-type-util.h.pump`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/make/Makefile` & `basedmypy-2.0.0rc1/mypyc/external/googletest/make/Makefile`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-all.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-death-test.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-death-test.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-filepath.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-filepath.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-internal-inl.h` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-port.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-port.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-printers.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-printers.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-test-part.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-test-part.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest-typed-test.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest-typed-test.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/external/googletest/src/gtest_main.cc` & `basedmypy-2.0.0rc1/mypyc/external/googletest/src/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/class_ir.py` & `basedmypy-2.0.0rc1/mypyc/ir/class_ir.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/func_ir.py` & `basedmypy-2.0.0rc1/mypyc/ir/func_ir.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/module_ir.py` & `basedmypy-2.0.0rc1/mypyc/ir/module_ir.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/ops.py` & `basedmypy-2.0.0rc1/mypyc/ir/ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/pprint.py` & `basedmypy-2.0.0rc1/mypyc/ir/pprint.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/ir/rtypes.py` & `basedmypy-2.0.0rc1/mypyc/ir/rtypes.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/ast_helpers.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/builder.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/builder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/callable_class.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/callable_class.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/classdef.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/classdef.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/constant_fold.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/constant_fold.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/context.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/context.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/env_class.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/env_class.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/expression.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/expression.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/for_helpers.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/for_helpers.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/format_str_tokenizer.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/format_str_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/function.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/function.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/generator.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/generator.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/ll_builder.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/ll_builder.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/main.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/main.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/mapper.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/mapper.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/match.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/match.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/nonlocalcontrol.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/nonlocalcontrol.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/prebuildvisitor.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/prebuildvisitor.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/prepare.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/prepare.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/specialize.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/specialize.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/statement.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/statement.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/targets.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/targets.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/util.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/util.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/visitor.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/visitor.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/irbuild/vtable.py` & `basedmypy-2.0.0rc1/mypyc/irbuild/vtable.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/CPy.h` & `basedmypy-2.0.0rc1/mypyc/lib-rt/CPy.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/bytes_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/bytes_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/dict_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/dict_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/exc_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/exc_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/float_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/float_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/generic_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/generic_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/getargs.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/getargs.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/getargsfast.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/getargsfast.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/int_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/int_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/list_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/list_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/misc_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/misc_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/module_shim.tmpl` & `basedmypy-2.0.0rc1/mypyc/lib-rt/module_shim.tmpl`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/mypyc_util.h` & `basedmypy-2.0.0rc1/mypyc/lib-rt/mypyc_util.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/pythoncapi_compat.h` & `basedmypy-2.0.0rc1/mypyc/lib-rt/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/pythonsupport.h` & `basedmypy-2.0.0rc1/mypyc/lib-rt/pythonsupport.h`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/setup.py` & `basedmypy-2.0.0rc1/mypyc/lib-rt/setup.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/str_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/str_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/test_capi.cc` & `basedmypy-2.0.0rc1/mypyc/lib-rt/test_capi.cc`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/lib-rt/tuple_ops.c` & `basedmypy-2.0.0rc1/mypyc/lib-rt/tuple_ops.c`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/namegen.py` & `basedmypy-2.0.0rc1/mypyc/namegen.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/options.py` & `basedmypy-2.0.0rc1/mypyc/options.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/bytes_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/bytes_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/dict_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/dict_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/exc_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/exc_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/float_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/float_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/generic_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/generic_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/int_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/int_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/list_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/list_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/misc_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/misc_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/registry.py` & `basedmypy-2.0.0rc1/mypyc/primitives/registry.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/set_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/set_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/str_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/str_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/primitives/tuple_ops.py` & `basedmypy-2.0.0rc1/mypyc/primitives/tuple_ops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/rt_subtype.py` & `basedmypy-2.0.0rc1/mypyc/rt_subtype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/sametype.py` & `basedmypy-2.0.0rc1/mypyc/sametype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/subtype.py` & `basedmypy-2.0.0rc1/mypyc/subtype.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_alwaysdefined.py` & `basedmypy-2.0.0rc1/mypyc/test/test_alwaysdefined.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_analysis.py` & `basedmypy-2.0.0rc1/mypyc/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_cheader.py` & `basedmypy-2.0.0rc1/mypyc/test/test_cheader.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_commandline.py` & `basedmypy-2.0.0rc1/mypyc/test/test_commandline.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_emit.py` & `basedmypy-2.0.0rc1/mypyc/test/test_emit.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_emitclass.py` & `basedmypy-2.0.0rc1/mypyc/test/test_emitclass.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_emitfunc.py` & `basedmypy-2.0.0rc1/mypyc/test/test_emitfunc.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_emitwrapper.py` & `basedmypy-2.0.0rc1/mypyc/test/test_emitwrapper.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_exceptions.py` & `basedmypy-2.0.0rc1/mypyc/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_external.py` & `basedmypy-2.0.0rc1/mypyc/test/test_external.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_irbuild.py` & `basedmypy-2.0.0rc1/mypyc/test/test_irbuild.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_ircheck.py` & `basedmypy-2.0.0rc1/mypyc/test/test_ircheck.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_literals.py` & `basedmypy-2.0.0rc1/mypyc/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_namegen.py` & `basedmypy-2.0.0rc1/mypyc/test/test_namegen.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_pprint.py` & `basedmypy-2.0.0rc1/mypyc/test/test_pprint.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_rarray.py` & `basedmypy-2.0.0rc1/mypyc/test/test_rarray.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_refcount.py` & `basedmypy-2.0.0rc1/mypyc/test/test_refcount.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_run.py` & `basedmypy-2.0.0rc1/mypyc/test/test_run.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_serialization.py` & `basedmypy-2.0.0rc1/mypyc/test/test_serialization.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_struct.py` & `basedmypy-2.0.0rc1/mypyc/test/test_struct.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_tuplename.py` & `basedmypy-2.0.0rc1/mypyc/test/test_tuplename.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/test_typeops.py` & `basedmypy-2.0.0rc1/mypyc/test/test_typeops.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test/testutil.py` & `basedmypy-2.0.0rc1/mypyc/test/testutil.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/alwaysdefined.test` & `basedmypy-2.0.0rc1/mypyc/test-data/alwaysdefined.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/analysis.test` & `basedmypy-2.0.0rc1/mypyc/test-data/analysis.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/commandline.test` & `basedmypy-2.0.0rc1/mypyc/test-data/commandline.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/driver/driver.py` & `basedmypy-2.0.0rc1/mypyc/test-data/driver/driver.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/exceptions-freq.test` & `basedmypy-2.0.0rc1/mypyc/test-data/exceptions-freq.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/exceptions.test` & `basedmypy-2.0.0rc1/mypyc/test-data/exceptions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/fixtures/ir.py` & `basedmypy-2.0.0rc1/mypyc/test-data/fixtures/ir.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/fixtures/testutil.py` & `basedmypy-2.0.0rc1/mypyc/test-data/fixtures/testutil.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/fixtures/typing-full.pyi` & `basedmypy-2.0.0rc1/mypyc/test-data/fixtures/typing-full.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-any.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-any.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-basic.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-basic.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-bool.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-bool.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-bytes.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-bytes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-classes.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-classes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-constant-fold.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-constant-fold.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-dict.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-dict.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-dunders.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-dunders.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-float.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-float.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-generics.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-generics.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-glue-methods.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-glue-methods.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-i32.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-i32.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-i64.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-i64.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-int.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-int.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-isinstance.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-isinstance.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-lists.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-lists.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-match.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-match.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-math.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-math.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-nested.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-nested.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-optional.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-optional.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-set.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-set.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-singledispatch.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-singledispatch.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-statements.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-statements.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-str.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-str.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-try.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-try.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-tuple.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-tuple.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-unreachable.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-unreachable.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/irbuild-vectorcall.test` & `basedmypy-2.0.0rc1/mypyc/test-data/irbuild-vectorcall.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/refcount.test` & `basedmypy-2.0.0rc1/mypyc/test-data/refcount.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-async.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-async.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-attrs.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-attrs.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-bench.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-bench.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-bools.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-bools.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-bytes.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-bytes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-classes.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-classes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-dicts.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-dicts.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-dunders.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-dunders.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-exceptions.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-exceptions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-floats.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-floats.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-functions.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-functions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-generators.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-generators.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-i32.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-i32.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-i64.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-i64.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-imports.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-imports.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-integers.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-integers.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-lists.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-lists.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-loops.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-loops.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-match.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-match.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-math.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-math.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-misc.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-misc.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-multimodule.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-multimodule.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-mypy-sim.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-mypy-sim.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-primitives.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-primitives.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-python37.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-python37.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-python38.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-python38.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-sets.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-sets.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-singledispatch.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-singledispatch.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-strings.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-strings.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-traits.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-traits.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/test-data/run-tuples.test` & `basedmypy-2.0.0rc1/mypyc/test-data/run-tuples.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/transform/exceptions.py` & `basedmypy-2.0.0rc1/mypyc/transform/exceptions.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/transform/refcount.py` & `basedmypy-2.0.0rc1/mypyc/transform/refcount.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/mypyc/transform/uninit.py` & `basedmypy-2.0.0rc1/mypyc/transform/uninit.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/pyproject.toml` & `basedmypy-2.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/pytest.ini` & `basedmypy-2.0.0rc1/pytest.ini`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/runtests.py` & `basedmypy-2.0.0rc1/runtests.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/setup.cfg` & `basedmypy-2.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/setup.py` & `basedmypy-2.0.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from mypy.version import __based_version__, __version__, based_version_info
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
 description = "Based static typing for Python"
 long_description = """
+Basedmypy -- Based Static Typing for Python
+===========================================
+
 .. image:: https://raw.githubusercontent.com/KotlinIsland/basedmypy/master/docs/static/logo-light.png
 
 Basedmypy is a type checker that is built on top of the work done by the
 `mypy project <https://github.com/python/mypy>`_. It adds based functionality and breaks compatibility with
 the cringe parts of pep 484.
 
 Based features
```

### Comparing `basedmypy-2.0.0/test-data/.flake8` & `basedmypy-2.0.0rc1/test-data/.flake8`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/pybind11_mypy_demo/src/main.cpp` & `basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/src/main.cpp`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/basics.pyi` & `basedmypy-2.0.0rc1/test-data/pybind11_mypy_demo/stubgen/pybind11_mypy_demo/basics.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/README.md` & `basedmypy-2.0.0rc1/test-data/unit/README.md`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-abstract.test` & `basedmypy-2.0.0rc1/test-data/unit/check-abstract.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-annotated.test` & `basedmypy-2.0.0rc1/test-data/unit/check-annotated.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-assert-type-fail.test` & `basedmypy-2.0.0rc1/test-data/unit/check-assert-type-fail.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-async-await.test` & `basedmypy-2.0.0rc1/test-data/unit/check-async-await.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-bare-literals.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-bare-literals.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-default-return.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-default-return.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-generic-typevar-bound.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-generic-typevar-bound.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-ignore-any-from-error.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-ignore-any-from-error.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-incomplete-defs.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-incomplete-defs.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-infer-function-types.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-infer-function-types.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-intersection.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-intersection.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-tuple-literal.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-tuple-literal.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-type-render.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-type-render.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-union-join.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-union-join.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-unsafe-variance.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-unsafe-variance.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-based-untyped.test` & `basedmypy-2.0.0rc1/test-data/unit/check-based-untyped.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-basic.test` & `basedmypy-2.0.0rc1/test-data/unit/check-basic.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-bound.test` & `basedmypy-2.0.0rc1/test-data/unit/check-bound.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-callable.test` & `basedmypy-2.0.0rc1/test-data/unit/check-callable.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-class-namedtuple.test` & `basedmypy-2.0.0rc1/test-data/unit/check-class-namedtuple.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-classes.test` & `basedmypy-2.0.0rc1/test-data/unit/check-classes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-classvar.test` & `basedmypy-2.0.0rc1/test-data/unit/check-classvar.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-columns.test` & `basedmypy-2.0.0rc1/test-data/unit/check-columns.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-ctypes.test` & `basedmypy-2.0.0rc1/test-data/unit/check-ctypes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-custom-plugin.test` & `basedmypy-2.0.0rc1/test-data/unit/check-custom-plugin.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-dataclass-transform.test` & `basedmypy-2.0.0rc1/test-data/unit/check-dataclass-transform.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-dataclasses.test` & `basedmypy-2.0.0rc1/test-data/unit/check-dataclasses.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-dynamic-typing.test` & `basedmypy-2.0.0rc1/test-data/unit/check-dynamic-typing.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-enum.test` & `basedmypy-2.0.0rc1/test-data/unit/check-enum.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-errorcodes.test` & `basedmypy-2.0.0rc1/test-data/unit/check-errorcodes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-expressions.test` & `basedmypy-2.0.0rc1/test-data/unit/check-expressions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-fastparse.test` & `basedmypy-2.0.0rc1/test-data/unit/check-fastparse.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-final.test` & `basedmypy-2.0.0rc1/test-data/unit/check-final.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-flags.test` & `basedmypy-2.0.0rc1/test-data/unit/check-flags.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-formatting.test` & `basedmypy-2.0.0rc1/test-data/unit/check-formatting.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-functions.test` & `basedmypy-2.0.0rc1/test-data/unit/check-functions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-functools.test` & `basedmypy-2.0.0rc1/test-data/unit/check-functools.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-generic-alias.test` & `basedmypy-2.0.0rc1/test-data/unit/check-generic-alias.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-generic-subtyping.test` & `basedmypy-2.0.0rc1/test-data/unit/check-generic-subtyping.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-generics.test` & `basedmypy-2.0.0rc1/test-data/unit/check-generics.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-ignore.test` & `basedmypy-2.0.0rc1/test-data/unit/check-ignore.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-incomplete-fixture.test` & `basedmypy-2.0.0rc1/test-data/unit/check-incomplete-fixture.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-incremental.test` & `basedmypy-2.0.0rc1/test-data/unit/check-incremental.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-inference-context.test` & `basedmypy-2.0.0rc1/test-data/unit/check-inference-context.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-inference.test` & `basedmypy-2.0.0rc1/test-data/unit/check-inference.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-inline-config.test` & `basedmypy-2.0.0rc1/test-data/unit/check-inline-config.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-isinstance.test` & `basedmypy-2.0.0rc1/test-data/unit/check-isinstance.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-kwargs.test` & `basedmypy-2.0.0rc1/test-data/unit/check-kwargs.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-lists.test` & `basedmypy-2.0.0rc1/test-data/unit/check-lists.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-literal.test` & `basedmypy-2.0.0rc1/test-data/unit/check-literal.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-lowercase.test` & `basedmypy-2.0.0rc1/test-data/unit/check-lowercase.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-modules-case.test` & `basedmypy-2.0.0rc1/test-data/unit/check-modules-case.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-modules-fast.test` & `basedmypy-2.0.0rc1/test-data/unit/check-modules-fast.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-modules.test` & `basedmypy-2.0.0rc1/test-data/unit/check-modules.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-multiple-inheritance.test` & `basedmypy-2.0.0rc1/test-data/unit/check-multiple-inheritance.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-namedtuple.test` & `basedmypy-2.0.0rc1/test-data/unit/check-namedtuple.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-narrowing.test` & `basedmypy-2.0.0rc1/test-data/unit/check-narrowing.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-native-int.test` & `basedmypy-2.0.0rc1/test-data/unit/check-native-int.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-newsemanal.test` & `basedmypy-2.0.0rc1/test-data/unit/check-newsemanal.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-newsyntax.test` & `basedmypy-2.0.0rc1/test-data/unit/check-newsyntax.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-newtype.test` & `basedmypy-2.0.0rc1/test-data/unit/check-newtype.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-optional.test` & `basedmypy-2.0.0rc1/test-data/unit/check-optional.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-overloading.test` & `basedmypy-2.0.0rc1/test-data/unit/check-overloading.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-parameter-specification.test` & `basedmypy-2.0.0rc1/test-data/unit/check-parameter-specification.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-plugin-attrs.test` & `basedmypy-2.0.0rc1/test-data/unit/check-plugin-attrs.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-possibly-undefined.test` & `basedmypy-2.0.0rc1/test-data/unit/check-possibly-undefined.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-protocols.test` & `basedmypy-2.0.0rc1/test-data/unit/check-protocols.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-python310.test` & `basedmypy-2.0.0rc1/test-data/unit/check-python310.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-python311.test` & `basedmypy-2.0.0rc1/test-data/unit/check-python311.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-python38.test` & `basedmypy-2.0.0rc1/test-data/unit/check-python38.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-python39.test` & `basedmypy-2.0.0rc1/test-data/unit/check-python39.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-recursive-types.test` & `basedmypy-2.0.0rc1/test-data/unit/check-recursive-types.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-redefine.test` & `basedmypy-2.0.0rc1/test-data/unit/check-redefine.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-reports.test` & `basedmypy-2.0.0rc1/test-data/unit/check-reports.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-selftype.test` & `basedmypy-2.0.0rc1/test-data/unit/check-selftype.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-semanal-error.test` & `basedmypy-2.0.0rc1/test-data/unit/check-semanal-error.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-serialize.test` & `basedmypy-2.0.0rc1/test-data/unit/check-serialize.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-singledispatch.test` & `basedmypy-2.0.0rc1/test-data/unit/check-singledispatch.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-slots.test` & `basedmypy-2.0.0rc1/test-data/unit/check-slots.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-statements.test` & `basedmypy-2.0.0rc1/test-data/unit/check-statements.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-super.test` & `basedmypy-2.0.0rc1/test-data/unit/check-super.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-tuples.test` & `basedmypy-2.0.0rc1/test-data/unit/check-tuples.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-type-aliases.test` & `basedmypy-2.0.0rc1/test-data/unit/check-type-aliases.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-type-checks.test` & `basedmypy-2.0.0rc1/test-data/unit/check-type-checks.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-type-promotion.test` & `basedmypy-2.0.0rc1/test-data/unit/check-type-promotion.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typeddict.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typeddict.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typeguard.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typeguard.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typevar-defaults.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typevar-defaults.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typevar-tuple.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typevar-tuple.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typevar-unbound.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typevar-unbound.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-typevar-values.test` & `basedmypy-2.0.0rc1/test-data/unit/check-typevar-values.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-union-error-syntax.test` & `basedmypy-2.0.0rc1/test-data/unit/check-union-error-syntax.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-union-or-syntax.test` & `basedmypy-2.0.0rc1/test-data/unit/check-union-or-syntax.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-unions.test` & `basedmypy-2.0.0rc1/test-data/unit/check-unions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-unreachable-code.test` & `basedmypy-2.0.0rc1/test-data/unit/check-unreachable-code.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-varargs.test` & `basedmypy-2.0.0rc1/test-data/unit/check-varargs.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/check-warnings.test` & `basedmypy-2.0.0rc1/test-data/unit/check-warnings.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/cmdline-based-baseline.test` & `basedmypy-2.0.0rc1/test-data/unit/cmdline-based-baseline.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/cmdline-based.test` & `basedmypy-2.0.0rc1/test-data/unit/cmdline-based.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/cmdline.pyproject.test` & `basedmypy-2.0.0rc1/test-data/unit/cmdline.pyproject.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/cmdline.test` & `basedmypy-2.0.0rc1/test-data/unit/cmdline.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/daemon-based.test` & `basedmypy-2.0.0rc1/test-data/unit/daemon-based.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/daemon.test` & `basedmypy-2.0.0rc1/test-data/unit/daemon.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps-classes.test` & `basedmypy-2.0.0rc1/test-data/unit/deps-classes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps-expressions.test` & `basedmypy-2.0.0rc1/test-data/unit/deps-expressions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps-generics.test` & `basedmypy-2.0.0rc1/test-data/unit/deps-generics.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps-statements.test` & `basedmypy-2.0.0rc1/test-data/unit/deps-statements.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps-types.test` & `basedmypy-2.0.0rc1/test-data/unit/deps-types.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/deps.test` & `basedmypy-2.0.0rc1/test-data/unit/deps.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/diff.test` & `basedmypy-2.0.0rc1/test-data/unit/diff.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/errorstream.test` & `basedmypy-2.0.0rc1/test-data/unit/errorstream.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-attr.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-attr.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-blockers.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-blockers.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-cache-incremental.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-cache-incremental.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-cycles.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-cycles.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-dataclass-transform.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-dataclass-transform.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-follow-imports.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-follow-imports.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-inspect.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-inspect.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-modules.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-modules.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained-suggest.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained-suggest.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fine-grained.test` & `basedmypy-2.0.0rc1/test-data/unit/fine-grained.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/args.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/args.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/async_await.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/async_await.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/callable.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/callable.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/classmethod.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/classmethod.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/dataclasses.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/dict.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/dict.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/divmod.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/divmod.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/exception.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/exception.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/f_string.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/f_string.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/fine_grained.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/fine_grained.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/float.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/float.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/floatdict.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/floatdict.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/for.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/for.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/isinstance.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstance.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/isinstance_python3_10.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstance_python3_10.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/isinstancelist.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/isinstancelist.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/list.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/list.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/module_all.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/module_all.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/object_with_init_subclass.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/object_with_init_subclass.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/ops.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/ops.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/paramspec.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/paramspec.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/plugin_attrs.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/plugin_attrs.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/primitives.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/primitives.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/set.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/set.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/transform.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/transform.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/tuple.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/tuple.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/type.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/type.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/typing-async.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-async.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/typing-full.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-full.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/typing-medium.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-medium.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/typing-namedtuple.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-namedtuple.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/fixtures/typing-typeddict.pyi` & `basedmypy-2.0.0rc1/test-data/unit/fixtures/typing-typeddict.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/hacks.txt` & `basedmypy-2.0.0rc1/test-data/unit/hacks.txt`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/attr/__init__.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/attrs/__init__.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/attrs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/builtins.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/builtins.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/collections.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/collections.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/contextlib.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/contextlib.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/dataclasses.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/enum.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/enum.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/functools.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/functools.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/math.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/math.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/mypy_extensions.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/mypy_extensions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/typing.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/typing.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/lib-stub/typing_extensions.pyi` & `basedmypy-2.0.0rc1/test-data/unit/lib-stub/typing_extensions.pyi`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/merge.test` & `basedmypy-2.0.0rc1/test-data/unit/merge.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/parse-errors.test` & `basedmypy-2.0.0rc1/test-data/unit/parse-errors.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/parse-python310.test` & `basedmypy-2.0.0rc1/test-data/unit/parse-python310.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/parse.test` & `basedmypy-2.0.0rc1/test-data/unit/parse.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/pep561.test` & `basedmypy-2.0.0rc1/test-data/unit/pep561.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/add_classmethod.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/add_classmethod.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/arg_kinds.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/arg_kinds.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/arg_names.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/arg_names.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/attrhook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/attrhook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/attrhook2.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/attrhook2.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/callable_instance.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/callable_instance.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/class_attr_hook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/class_attr_hook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/class_callable.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/class_callable.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/common_api_incremental.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/common_api_incremental.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/custom_errorcode.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/custom_errorcode.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/descriptor.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/descriptor.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/dyn_class.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/dyn_class.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/dyn_class_from_method.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/dyn_class_from_method.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/fully_qualified_test_hook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/fully_qualified_test_hook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/function_sig_hook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/function_sig_hook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/method_in_decorator.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/method_in_decorator.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/method_sig_hook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/method_sig_hook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/named_callable.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/named_callable.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/type_anal_hook.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/type_anal_hook.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/plugins/union_method.py` & `basedmypy-2.0.0rc1/test-data/unit/plugins/union_method.py`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/pythoneval-asyncio.test` & `basedmypy-2.0.0rc1/test-data/unit/pythoneval-asyncio.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/pythoneval.test` & `basedmypy-2.0.0rc1/test-data/unit/pythoneval.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/ref-info.test` & `basedmypy-2.0.0rc1/test-data/unit/ref-info.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/reports.test` & `basedmypy-2.0.0rc1/test-data/unit/reports.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-abstractclasses.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-abstractclasses.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-basic.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-basic.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-classes.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-classes.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-classvar.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-classvar.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-errors-python310.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-errors-python310.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-errors.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-errors.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-expressions.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-expressions.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-lambda.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-lambda.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-literal.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-literal.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-modules.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-modules.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-namedtuple.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-namedtuple.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-python310.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-python310.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-statements.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-statements.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-symtable.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-symtable.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-typealiases.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-typealiases.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-typeddict.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-typeddict.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-typeinfo.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-typeinfo.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/semanal-types.test` & `basedmypy-2.0.0rc1/test-data/unit/semanal-types.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/stubgen-based.test` & `basedmypy-2.0.0rc1/test-data/unit/stubgen-based.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/stubgen.test` & `basedmypy-2.0.0rc1/test-data/unit/stubgen.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-data/unit/typexport-basic.test` & `basedmypy-2.0.0rc1/test-data/unit/typexport-basic.test`

 * *Files identical despite different names*

### Comparing `basedmypy-2.0.0/test-requirements.txt` & `basedmypy-2.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

