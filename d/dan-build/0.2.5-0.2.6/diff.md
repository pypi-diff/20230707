# Comparing `tmp/dan-build-0.2.5.tar.gz` & `tmp/dan-build-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.5.tar", last modified: Sat Jul  1 13:06:01 2023, max compression
+gzip compressed data, was "dan-build-0.2.6.tar", last modified: Fri Jul  7 07:20:39 2023, max compression
```

## Comparing `dan-build-0.2.5.tar` & `dan-build-0.2.6.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.412398 dan-build-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 13:05:53.000000 dan-build-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-01 13:06:01.412398 dan-build-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-01 13:05:53.000000 dan-build-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cmake/configure_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-01 13:05:53.000000 dan-build-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 13:06:01.412398 dan-build-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.412398 dan-build-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_src_catch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_python_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 07:20:29.000000 dan-build-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 07:20:39.300667 dan-build-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-07 07:20:29.000000 dan-build-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/configure_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.292667 dan-build-0.2.6/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 07:20:29.000000 dan-build-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:20:39.300667 dan-build-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_src_catch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_python_errors.py
```

### Comparing `dan-build-0.2.5/LICENSE` & `dan-build-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/PKG-INFO` & `dan-build-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.5/README.md` & `dan-build-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/completion/bash/dan-io.sh` & `dan-build-0.2.6/completion/bash/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/completion/bash/dan.sh` & `dan-build-0.2.6/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/completion/zsh/dan-io.sh` & `dan-build-0.2.6/completion/zsh/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/completion/zsh/dan.sh` & `dan-build-0.2.6/completion/zsh/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cli/click.py` & `dan-build-0.2.6/dan/cli/click.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
 from enum import Enum
 import types as typs
-import typing as t
 from click import *
 
 import inspect
 import asyncio
 
+import dan.core.typing as t
 from dan import logging
 
 class AsyncContext(Context):
     def invoke(__self, __callback, *args, **kwargs):
         ret = super().invoke(__callback, *args, **kwargs)
         if inspect.isawaitable(ret):
             loop = asyncio.get_event_loop()
@@ -45,14 +45,16 @@
             elif '+=' in part or '-=' in part:
                 part, value = part.split(part[:-2])
             for field in fields:
                 if part.startswith(field.name):
                     type = field.type
                     if isinstance(type, typs.GenericAlias):
                         type = t.get_origin(type)
+                    elif t.is_optional(type):
+                        type = t.get_args(type)[0]
                     if dataclasses.is_dataclass(type):
                         subfields = dataclasses.fields(type)
                         subparts = parts[1:]
                         gen_comps(subfields, subparts, f'{field.name}.')
                     elif issubclass(type, (set, list)):
                         if part.endswith(('+', '-')):
                             completions.append(CompletionItem(f'{prefix}{field.name}{part[-1]}=', type='nospace'))
```

### Comparing `dan-build-0.2.5/dan/cli/io.py` & `dan-build-0.2.6/dan/cli/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 import asyncio
 import fnmatch
 import os
 import contextlib
 
 from dan.cli import click
 from dan.core.requirements import parse_package
+from dan.core.cache import Cache
+from dan.io.repositories import RepositoriesSettings, _get_settings
 from dan.make import Make
 
+def get_source_path():
+    from dan.cxx.detect import get_dan_path
+    source_path = get_dan_path() / 'deps'
+    source_path.mkdir(exist_ok=True, parents=True)
+    return source_path
+
 _make : Make = None
 async def get_make(toolchain='default', quiet=True):
     global _make
     if _make is None:
-        from dan.cxx.detect import get_dan_path
-        source_path = get_dan_path() / 'deps'
-        source_path.mkdir(exist_ok=True, parents=True)
+        source_path = get_source_path()
         os.chdir(source_path)
         (source_path / 'dan-build.py').touch()
         make = Make(source_path / 'build', quiet=quiet)
         make.config.source_path = str(source_path)
         make.config.build_path = str(source_path / 'build')
         make.config.toolchain = toolchain
         await make._config.save()
@@ -54,14 +60,22 @@
         yield make
 
 
 @click.group()
 def cli():
     pass
 
+@cli.command()
+@click.option('--setting', '-s', 'settings', type=click.SettingsParamType(RepositoriesSettings), multiple=True)
+async def configure(settings):
+    io_settings = _get_settings()
+    from dan.core.settings import apply_settings
+    apply_settings(io_settings, *settings, logger=click.logger)
+    await Cache.save_all()
+
 @cli.group()
 def ls():
     """Inspect stuff"""
     pass
 
 
 @ls.command()
@@ -111,14 +125,27 @@
         available_versions = sorted(available_versions.keys())
         for v in available_versions:
             if v == lib.version:
                 click.echo(f' - {v} (default)')
             else:
                 click.echo(f' - {v}')
 
+@ls.command()
+@click.argument('LIBRARY')
+async def options(library: str):
+    """Get LIBRARY's available options"""
+    async with make_context():
+        lib = await get_library(library)
+        await lib.initialize()
+        for o in lib.options:
+            current = ''
+            if o.value != o.default:
+                current = f', current: {o.value}'
+            click.echo(f'{o.name}: {o.help} (type: {o.type.__name__}, default: {o.default}{current})')
+
 @cli.command()
 @click.argument('NAME')
 async def search(name):
     """Search for NAME in repositories"""
     async with make_context():
         name = f'*{name}*'
         repos = await get_repositories()
```

### Comparing `dan-build-0.2.5/dan/cli/main.py` & `dan-build-0.2.6/dan/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,29 @@
     ctx.call_on_close(show_diags)
 
 
 @cli.command()
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--toolchain', '-t', help='The toolchain to use',
-              type=click.ToolchainParamType())
+              type=click.ToolchainParamType(), envvar='DAN_TOOLCHAIN')
 @click.option('--setting', '-s', 'settings', help='Set or change a setting', multiple=True, type=click.SettingsParamType(Settings))
 @click.option('--option', '-o', 'options', help='Set or change an option', multiple=True, type=click.OptionsParamType())
 @click.option('--build-path', '-B', help='Path where dan has been initialized.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH')
 @click.option('--source-path', '-S', help='Path where source is located.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='.')
 @pass_context
 async def configure(ctx: CommandsContext, toolchain: str, settings: tuple[str], options: tuple[str], source_path: Path, **kwds):
     """Configure dan project"""
     ctx(**kwds)  # update kwds
     if toolchain is None and ctx.make.config.toolchain is None:
-        toolchain = click.prompt('Toolchain', type=click.ToolchainParamType(), default='default')
+        from dan.cxx.detect import get_toolchains
+        tp = click.Choice(get_toolchains(create=False)["toolchains"].keys())
+        toolchain = click.prompt('Toolchain', type=tp, default='default')
 
     await ctx.make.configure(source_path, toolchain)
 
     if len(settings):
         await ctx.make.apply_settings(*settings)
 
     # NOTE: intializing make after applying setting
@@ -132,17 +134,23 @@
 @pass_context
 async def build(ctx: CommandsContext, force=False, **kwds):
     """Build targets"""
     ctx(**kwds)  # update kwds
     if force:
         await ctx.make.clean()
     await ctx.make.build()
-    # from dan.cxx import target_toolchain
-    # target_toolchain.compile_commands.update()
 
+@cli.command()
+@common_opts
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
+@pass_context
+async def install_dependencies(ctx: CommandsContext, **kwds):
+    """Build targets"""
+    ctx(**kwds)  # update kwds
+    await ctx.make.install_dependencies()
 
 @cli.command()
 @common_opts
 @click.argument('MODE', type=click.Choice([v.name for v in InstallMode]), default=InstallMode.user.name)
 @click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def install(ctx: CommandsContext, mode: str, **kwargs):
```

### Comparing `dan-build-0.2.5/dan/cli/vscode.py` & `dan-build-0.2.6/dan/cli/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cmake/configure_file.py` & `dan-build-0.2.6/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/conan/requirements.py` & `dan-build-0.2.6/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/asyncio.py` & `dan-build-0.2.6/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/cache.py` & `dan-build-0.2.6/dan/core/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -124,8 +124,39 @@
         
         result = fn(self, *args, **kwds)
         setattr(self, result_name, result)
         return result
 
     return wrapper
 
+class _CachedProperty:
+    def __init__(self, getter: t.Callable[[], t.Any], cache_name=None):
+        self.__getter = getter
+        self.__name = getter.__name__
+        self.__cache_name = 'cache' if cache_name is None else cache_name
 
+    def __get__(self, instance, owner: type | None = None):
+        cache = getattr(instance, self.__cache_name)
+        if isinstance(cache, Cache):
+            cache = cache.data
+        value = cache.get(self.__name)
+        if value is None:
+            value = self.__getter(instance)
+            if value is not None:
+                cache[self.__name] = value
+        return value
+
+    def __set__(self, instance, value):
+        cache = getattr(instance, self.__cache_name)
+        if isinstance(cache, Cache):
+            cache = cache.data
+        cache[self.__name] = value
+
+    def __delete__(self, instance):
+        cache = getattr(instance, self.__cache_name)
+        del cache[self.__name]
+
+
+def cached_property(cache_name=None):
+    def wrapper(fn):
+        return _CachedProperty(fn, cache_name=cache_name)
+    return wrapper
```

### Comparing `dan-build-0.2.5/dan/core/diagnostics.py` & `dan-build-0.2.6/dan/core/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/find.py` & `dan-build-0.2.6/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/functools.py` & `dan-build-0.2.6/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/generator.py` & `dan-build-0.2.6/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/include.py` & `dan-build-0.2.6/dan/core/include.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 class MakeFileError(RuntimeError):
     def __init__(self, path) -> None:
         self.path = Path(path)
         super().__init__(f'failed to load {self.path}')
 
 
-def _init_makefile(module, name: str = 'root', build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None):
+def _init_makefile(module, name: str = 'root', build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None, is_requirement=False):
     global context
     source_path = Path(module.__file__).parent
     if parent is None and context.current is not None:
         parent = context.current
 
     if build_path is None:
         assert parent is not None
@@ -112,26 +112,33 @@
     module.__class__ = MakeFile
     context.current = module
     module._setup(
         name,
         source_path,
         build_path,
         requirements,
-        parent)
+        parent,
+        is_requirement)
 
-def load_makefile(module_path: Path, name: str = None, module_name: str = None, build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None) -> MakeFile:
+def load_makefile(module_path: Path,
+                  name: str = None,
+                  module_name: str = None,
+                  build_path: Path = None,
+                  requirements: MakeFile = None,
+                  parent: MakeFile = None,
+                  is_requirement=False) -> MakeFile:
     name = name or module_path.stem
     module_name = module_name or name
     if module_path in context.imported_makefiles:
         return context.imported_makefiles[module_path]
     spec = importlib.util.spec_from_file_location(
         module_name, module_path)
     module = importlib.util.module_from_spec(spec)
     context.imported_makefiles[module_path] = module
-    _init_makefile(module, name, build_path, requirements, parent)
+    _init_makefile(module, name, build_path, requirements, parent, is_requirement)
     try:
         spec.loader.exec_module(module)
     except Exception as err:
         context.error('makefile error while loading \'%s\': %s', module_path, err)
         raise MakeFileError(module_path) from err
     context.up()
     return module
@@ -169,15 +176,15 @@
     module = importlib.util.module_from_spec(spec)
     context.imported_makefiles[module_path] = module
     _init_makefile(module, name, build_path)
 
     requirements_file = module_path.with_stem('dan-requires')
     if module_path.stem == 'dan-build' and requirements_file.exists():
         context.current.requirements = load_makefile(
-            requirements_file, name='dan-requires', module_name=f'{name}.requirements')
+            requirements_file, name='dan-requires', module_name=f'{name}.requirements', is_requirement=True)
 
     try:
         spec.loader.exec_module(module)
     except TargetNotFound as err:
         if len(context.missing) == 0:
             raise err
     except Exception as err:
```

### Comparing `dan-build-0.2.5/dan/core/makefile.py` & `dan-build-0.2.6/dan/core/makefile.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 class MakeFile(sys.__class__):
 
     def _setup(self,
                name: str,
                source_path: Path,
                build_path: Path,
                requirements: 'MakeFile' = None,
-               parent: 'MakeFile' = None) -> None:
+               parent: 'MakeFile' = None,
+               is_requirement = False) -> None:
         self.name = name
         self.description = None
         self.version = None
         self.source_path = source_path
         self.build_path = build_path
         self.__requirements = requirements
+        self.__pkgs_path = None
         self.parent = parent
+        self.__is_requirement = is_requirement
         self.__cache: Cache = None
         self.children: list[MakeFile] = list()
         if self.name != 'dan-requires' and self.parent:
             self.parent.children.append(self)
         self.options = Options(self)
         self.__targets: set[Target] = set()
         self.__tests: set[Test] = set()
@@ -48,14 +51,22 @@
     @property
     def parents(self):
         parent = self.parent
         while parent is not None:
             yield parent
             parent = parent.parent
 
+    @property
+    def is_requirement(self):
+        if self.__is_requirement:
+            return True
+        for parent in self.parents:
+            if parent.__is_requirement:
+                return True
+        return False
 
     __target_fullnames = list()
     __test_fullnames = list()
     def register(self, cls: type[Target | Test]):
         """Register Target/Test class"""
         t = cls()
         if issubclass(cls, Target):
@@ -88,15 +99,15 @@
     @functools.cache
     def __find(self, name_or_class) -> Target:
         if isinstance(name_or_class, type):
             def check(t: Target):
                 return type(t) == name_or_class
         else:
             def check(t: Target):
-                return t.name == name_or_class
+                return name_or_class in t.provides
         for t in self.targets:
             if check(t):
                 return t
         for c in self.children:
             t = c.__find(name_or_class)
             if t:
                 return t
@@ -127,18 +138,25 @@
         if self.__requirements is not None:
             return self.__requirements
         elif self.parent is not None:
             return self.parent.requirements
 
     @property
     def pkgs_path(self):
-        if self.requirements:
-            return self.requirements.parent.build_path / 'pkgs'
+        if self.__pkgs_path is None:
+            if self.requirements:
+                return self.requirements.parent.build_path / 'pkgs'
+            else:
+                return self.build_path / 'pkgs'
         else:
-            return self.build_path / 'pkgs'
+            return self.__pkgs_path
+        
+    @pkgs_path.setter
+    def pkgs_path(self, value):
+        self.__pkgs_path = value
 
     @requirements.setter
     def requirements(self, value: 'MakeFile'):
         self.__requirements = value
 
     @property
     def targets(self) -> set[Target]:
```

### Comparing `dan-build-0.2.5/dan/core/osinfo.py` & `dan-build-0.2.6/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/pathlib.py` & `dan-build-0.2.6/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/pm.py` & `dan-build-0.2.6/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/register.py` & `dan-build-0.2.6/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/requirements.py` & `dan-build-0.2.6/dan/core/requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,27 @@
             library = name
             repository = None
     
     return package, library, repository
 
 
 class RequiredPackage(Logging):
-    def __init__(self, name: str, version_spec: VersionSpec = None):
-        self.version_spec = version_spec
+    
+    @t.overload
+    def __init__(self, specification_str: str): ...
+    
+    @t.overload
+    def __init__(self, name: str, version_spec: VersionSpec): ...
+
+    def __init__(self, *args):
+        if len(args) == 2:
+            name = args[0]
+            self.version_spec = args[1]
+        else:
+            name, self.version_spec = VersionSpec.parse(args[0])
         super().__init__(name)
         self.target : 'Target' = None
         self.package, self.name, self.repository = parse_package(name)
         self.__skipped = list()
 
     def is_compatible(self, t: 'Target'):
         if self.version_spec is not None:
@@ -118,32 +129,33 @@
                 continue
 
             t = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
             if t is not None and req.is_compatible(t):
                 logger.debug('%s: using package %s', req, t.fullname)
                 req.target = t
                 resolved.append(req)
-            elif install:
-                if makefile.requirements:
-                    # install requirement from dan-requires.py
-                    t = makefile.requirements.find(req.name)
-                    if not t:
-                        raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
-                    logger.debug('%s using requirements\' target %s', req, t.fullname)
-                else:
-                    with makefile.context:
-                        t, is_new = Package.instance(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile.root)
-                    if is_new:
-                        logger.debug('%s: adding package %s', req, t.fullname)
-                    else:
-                        logger.debug('%s: package already beeing installed at version %s', req, t.version)
-                group.create_task(t.install(deps_settings, InstallMode.dev))
-                unresolved.append(req)
-
+                continue
+            
+            if makefile.requirements:
+                # install requirement from dan-requires.py
+                t = makefile.requirements.find(req.name)
+                if not t:
+                    raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
+                logger.debug('%s using requirements\' target %s', req, t.fullname)
+            else:
+                with makefile.context:
+                    t, is_new = Package.instance(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile.root)
+                if is_new:
+                    logger.debug('%s: adding package %s', req, t.fullname)
+                elif install:
+                    logger.debug('%s: package already beeing installed at version %s', req, t.version)
 
+            if install:
+                group.create_task(t.install(deps_settings, InstallMode.dev))
+            unresolved.append(req)
 
     if install:
         for req in unresolved:
             pkg = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
             if pkg is None:
                 raise RuntimeError(f'Unresolved requirement {req}')
             req.target = pkg
```

### Comparing `dan-build-0.2.5/dan/core/runners.py` & `dan-build-0.2.6/dan/core/runners.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import io
 import logging
 import os
+from pathlib import Path
 import subprocess
 import sys
 
 import tqdm
 
 import asyncio
 
@@ -145,20 +146,31 @@
                 escaped = False
 
     if current:
         result.append(''.join(current))
 
     return result
 
+def list2cmdline(command: list|str):
+    if isinstance(command, list):
+        cmd = list()
+        for part in command:
+            if isinstance(part, Path):
+                cmd.append(part.as_posix())
+            else:
+                cmd.append(part)
+        return subprocess.list2cmdline(cmd)
+    return command
+
+
 async def async_run(command, log=True, logger: logging.Logger = None, no_raise=False, env=None, cwd=None, out_capture=None, err_capture=None, all_capture=None, input: str = None) -> tuple[str, str, int]:
     if _jobs_sem is not None:
         await _jobs_sem.acquire()
     try:
-        if not isinstance(command, str):
-            command = subprocess.list2cmdline(command)
+        command = list2cmdline(command)
         if env is not None:
             e = dict(os.environ)
             for k, v in env.items():
                 e[k] = v
             env = e
         if input is not None:
             stdin = asyncio.subprocess.PIPE
@@ -221,16 +233,15 @@
         return out, err, proc.returncode
     finally:
         if _jobs_sem is not None:
             _jobs_sem.release()
 
 
 def sync_run(command, pipe=True, logger: logging.Logger = None, no_raise=False, shell=True, env=None, cwd=None):
-    if not isinstance(command, str):
-        command = subprocess.list2cmdline(command)
+    command = list2cmdline(command)
     if pipe:
         stdout = subprocess.PIPE
     else:
         stdout = None
     if logger:
         logger.debug(f'executing: {command}')
     if env:
```

### Comparing `dan-build-0.2.5/dan/core/target.py` & `dan-build-0.2.6/dan/core/target.py`

 * *Files 16% similar despite different names*

```diff
@@ -91,20 +91,23 @@
 TargetDependencyLike: TypeAlias = Union[list['Target'], 'Target']
 
 
 PathImpl = type(Path())
 
 
 class FileDependency(PathImpl):
-    up_to_date = True
-
+    
     def __init__(self, *args, **kwargs):
         super(PathImpl, self).__init__()
 
     @property
+    def up_to_date(self):
+        return self.exists()
+
+    @property
     def modification_time(self):
         return self.stat().st_mtime
 
 
 class Option:
     def __init__(self, parent: 'Options', fullname: str, default, help: str = None) -> None:
         self.fullname = fullname
@@ -164,14 +167,16 @@
         if not 'options' in cache:
             cache['options'] = dict()
         self._cache = cache['options']
         self.__items: list[Option] = list()
         self.update(default)
 
     def add(self, name: str, default_value, help=None):
+        if self.get(name) is not None:
+            raise RuntimeError(f'duplicate options detected ({name})')
         opt = Option(self, f'{self.__parent.fullname}.{name}',
                      default_value, help=help)
         self.__items.append(opt)
         return opt
 
     def get(self, name: str):
         for o in self.__items:
@@ -216,42 +221,99 @@
         opt = self.get(name)
         if opt:
             return opt.value
 
     def __iter__(self):
         return iter(self.__items)
 
+class Installer:
+    def __init__(self, settings: InstallSettings, mode: InstallMode, logger: Logging) -> None:
+        self.settings = settings
+        self.mode = mode
+        self.installed_files = list()
+        self._logger = logger
+    
+    async def _install(self, src: Path|str, dest: Path, subdir: Path = None):
+        if subdir is not None:
+            dest /= subdir
+        if isinstance(src, Path):
+            dest /= src.name
+            if dest.exists() and dest.younger_than(src):
+                self._logger.info('%s is up-to-date', dest)
+                self.installed_files.append(dest)
+                return
+            self._logger.debug('installing: %s', dest)
+            await aiofiles.copy(src, dest)
+        else:
+            dest.parent.mkdir(parents=True, exist_ok=True)
+            self._logger.debug('installing: %s', dest)
+            async with aiofiles.open(dest, 'w') as f:
+                await f.write(src)
+        self.installed_files.append(dest)
+
+    @property
+    def dev(self):
+        return self.mode == InstallMode.dev
+    
+    async def install_bin(self, src, subdir = None):
+        await self._install(src, self.settings.runtime_destination, subdir)
+
+    async def install_shared_library(self, src, subdir = None):
+        await self._install(src, self.settings.libraries_destination, subdir)
+
+    async def install_static_library(self, src, subdir = None):
+        if not self.dev:
+            return
+        await self._install(src, self.settings.libraries_destination, subdir)
+
+    async def install_header(self, src, subdir = None):
+        if not self.dev:
+            return
+        await self._install(src, self.settings.includes_destination, subdir)
+
+    async def install_data(self, src, subdir = None, dev=False):
+        if dev and not self.dev:
+            return
+        await self._install(src, self.settings.data_destination, subdir)
+
 
 class Target(Logging, MakefileRegister, internal=True):
     name: str = None
     fullname: str = None
     description: str = None,
     default: bool = True
     installed: bool = False
     output: Path = None
-    options: dict[str, Any] = dict()
+    options: dict[str, Any]|Options = dict()
+    provides: Iterable[str] = None
 
     dependencies: set[TargetDependencyLike] = set()
     preload_dependencies: set[TargetDependencyLike] = set()
 
     def __init__(self,
                  name: str = None,
                  parent: 'Target' = None,
                  version: str = None,
                  default: bool = None,
                  makefile=None) -> None:
         
         self.parent = parent
         self.__cache: dict = None
+        self.__source_path : Path = None
 
         if name is not None:
             self.name = name
 
         if self.name is None:
             self.name = self.__class__.__name__
+        
+        if self.provides is None:
+            self.provides = [self.name]
+        else:
+            self.provides = set([self.name, *self.provides])
 
         if default is not None:
             self.default = default
 
         if parent is not None:
             self.makefile = parent.makefile
             self.fullname = f'{parent.fullname}.{self.name}'
@@ -281,14 +343,15 @@
         self.dependencies = Dependencies(self, self.dependencies)
         self.preload_dependencies = Dependencies(
             self, self.preload_dependencies)
 
         super().__init__(self.fullname)
 
         self._output: Path = None
+        self._build_path = None
 
         if type(self).output != Target.output:
             # hack class-defined output
             #   transform it to classproperty for build_path resolution
             output = self.output
             type(self).output = utils.classproperty(lambda: self.build_path / output)
 
@@ -325,23 +388,33 @@
         elif path.is_absolute() and self.build_path in path.parents:
             self._output = path.relative_to(self.build_path)
         else:
             self._output = path
 
     @property
     def is_requirement(self) -> bool:
-        return self.makefile.name.endswith('requirements')
+        return self.makefile.is_requirement
 
     @property
     def source_path(self) -> Path:
-        return self.makefile.source_path
+        if self.__source_path is None:
+            return self.makefile.source_path
+        else:
+            return self.__source_path
+    
+    @source_path.setter
+    def source_path(self, value):
+        self.__source_path = value
 
     @property
     def build_path(self) -> Path:
-        return self.makefile.build_path
+        if self._build_path is None:
+            return self.makefile.build_path
+        else:
+            return self._build_path
     
     @property
     def requires(self):
         from dan.pkgconfig.package import RequiredPackage
         return [dep for dep in self.dependencies if isinstance(dep, RequiredPackage)]
 
     @cached_property
@@ -475,29 +548,18 @@
 
     @asyncio.cached(unique = True)
     async def install(self, settings: InstallSettings, mode: InstallMode):
         await self.build()
 
         self.debug('installing %s to %s', self.name, settings.destination)
 
-        installed_files = list()
-        if mode == InstallMode.dev:
-            if len(self.utils) > 0:
-                lines = list()
-                for fn in self.utils:
-                    tmp = inspect.getsourcelines(fn)[0]
-                    tmp[0] = f'\n\n@self.utility\n'
-                    lines.extend(tmp)
-                filepath = settings.libraries_destination / \
-                    'dan' / f'{self.name}.py'
-                filepath.parent.mkdir(exist_ok=True, parents=True)
-                async with aiofiles.open(filepath, 'w') as f:
-                    await f.writelines(lines)
-                    installed_files.append(filepath)
-        return installed_files
+        installer = Installer(settings, mode, self)
+        await self.__install__(installer)
+        return installer.installed_files
+
 
     def get_dependency(self, dep: str | type, recursive=True) -> TargetDependencyLike:
         """Search for dependency"""
         if isinstance(dep, str):
             def check(d): return d.name == dep
         else:
             def check(d): return isinstance(d, dep)
@@ -522,16 +584,23 @@
 
     async def __prebuild__(self):
         ...
 
     async def __build__(self):
         ...
 
-    async def __install__(self):
-        ...
+    async def __install__(self, installer: Installer):
+        if installer.dev:
+            if len(self.utils) > 0:
+                body = str()
+                for fn in self.utils:
+                    tmp = inspect.getsourcelines(fn)[0]
+                    tmp[0] = f'\n\n@self.utility\n'
+                    body += '\n'.join(tmp)
+                await installer.install_data(body, f'dan/{self.name}.py')
 
     async def __clean__(self):
         ...
 
     @utils.classproperty
     def utils(cls) -> list:
         utils_name = f'_{cls.__name__}_utils__'
```

### Comparing `dan-build-0.2.5/dan/core/test.py` & `dan-build-0.2.6/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/utils.py` & `dan-build-0.2.6/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/core/version.py` & `dan-build-0.2.6/dan/core/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     def parse(data: str) -> tuple[str|None, 'VersionSpec']:
         m = re.match(r'(.+?)?\s+?([><]=?|=)\s+([\d\.]+)', data)
         if m:
             name = m[1]
             op = m[2]
             version = Version(m[3])
             return name, VersionSpec(version, op)
-        return None, None
+        return data, None
 
 
     def __init__(self, version: Version, op: str) -> None:
         self.version = version
         self.op = op
         
     def is_compatible(self, version: Version):
```

### Comparing `dan-build-0.2.5/dan/core/win.py` & `dan-build-0.2.6/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cxx/__init__.py` & `dan-build-0.2.6/dan/cxx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from dan.core.cache import Cache
 
 from dan.core.errors import InvalidConfiguration
 from dan.core.settings import Settings
-from dan.cxx.toolchain import Toolchain
+from dan.cxx.toolchain import Toolchain, BuildType
 from dan.cxx.detect import get_toolchains
 
 target_toolchain: Toolchain = None
 """The target toolchain.
 """
 
 host_toolchain: Toolchain = None
@@ -65,16 +65,16 @@
             'target': dict(),
         }
     target_toolchain = tc_type(toolchain_data, data['tools'], settings=target_settings, cache=cache['toolchains']['target'])
     target_toolchain.init()
     if target_toolchain.is_host:
         host_toolchain = target_toolchain
     else:
-        import logging
-        logging.warning(f'Cross compilation is currently not tested !')
+        from dan import logging
+        logging.getLogger('cxx').warning('Cross compilation is currently not tested !')
         host_toolchain = None
 
     from dan.core.include import context
     context.set('cxx_target_toolchain', target_toolchain)
     context.set('cxx_host_toolchain', host_toolchain)
```

### Comparing `dan-build-0.2.5/dan/cxx/compile_commands.py` & `dan-build-0.2.6/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cxx/detect.py` & `dan-build-0.2.6/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.6/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cxx/support/qt.py` & `dan-build-0.2.6/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/cxx/targets.py` & `dan-build-0.2.6/dan/cxx/targets.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import typing as t
 
 from collections.abc import Iterable
 from enum import Enum
 from functools import cached_property
 
 from dan.core.pathlib import Path
-from dan.core import aiofiles, cache
-from dan.core.settings import InstallMode, InstallSettings
-from dan.core.target import Target
+from dan.core import cache
+from dan.core.target import Target, Installer
 from dan.core.utils import chunks, unique
 from dan.core.runners import async_run
 from dan.core import asyncio
 from dan.cxx.toolchain import CompilationFailure, LibraryList, LinkageFailure, Toolchain
-
+from dan.core.cache import cached_property as dan_cached
 
 class CXXObject(Target, internal=True):
     def __init__(self, source:Path, parent: 'CXXTarget', root: Path = None) -> None:
         if source.is_absolute():
             if root is None:
                 root = parent.build_path
             name = '-'.join(source.relative_to(root).with_suffix(f'').parts)
@@ -46,29 +45,35 @@
     @property
     def includes(self):
         return self.parent.includes
 
     @property
     def compile_definitions(self):
         return self.parent.compile_definitions
+    
+    @dan_cached()
+    def deps(self): ...
+
+    @dan_cached()
+    def compile_args(self): ...
 
     async def __initialize__(self):
         await self.parent.preload()
 
-        deps = self.cache.get('deps')
+        deps = self.deps
         if deps is not None:
             self.dependencies.update(deps)
 
         self.dependencies.add(self.source)
 
         self.other_generated_files.update(
             self.toolchain.compile_generated_files(self.output))
 
-        previous_args = self.cache.get('compile_args')
-        if previous_args:
+        previous_args = self.compile_args
+        if previous_args is not None:
             args = self.toolchain.make_compile_commands(
                 self.source_path / self.source, self.output, self.private_cxx_flags)[0]
             args = [str(arg) for arg in args]
             if sorted(args) != sorted(previous_args):
                 self.__dirty = True
         else:
             self.__dirty = True
@@ -85,42 +90,48 @@
             self.output.parent.mkdir(parents=True, exist_ok=True)
             commands, diags = await self.toolchain.compile(self.source_path / self.source, self.output, self.private_cxx_flags)
             self.parent.diagnostics.insert(diags, str(self.source))
         except CompilationFailure as err:
             self.parent.diagnostics.insert(err.diags, str(self.source))
             err.target = self
             raise
-        self.cache['compile_args'] = [str(a) for a in commands[0]]
+        self.compile_args = [str(a) for a in commands[0]]
         self.debug('scanning dependencies of %s', self.source.name)
         deps = await self.toolchain.scan_dependencies(self.source_path / self.source, self.private_cxx_flags, self.build_path)
         deps = [d for d in deps
                 if self.makefile.root.source_path in Path(d).parents
                 or self.build_path in Path(d).parents]
-        self.cache['deps'] = deps
+        self.deps = deps
 
 
 class OptionSet:
     def __init__(self, parent: 'CXXTarget',
                  name: str,
                  public: list | set = set(),
                  private: list | set = set(),
-                 transform: t.Callable = None) -> None:
+                 transform_out: t.Callable[[t.Any], t.Any] = None,
+                 transform_in: t.Callable[[t.Any], t.Any] = None) -> None:
         self._parent = parent
         self._name = name
-        self._transform = transform or (lambda x: x)
+        self._transform_out = transform_out or self.__nop_transform
+        self._transform_in = transform_in or self.__nop_transform
         self._public = list(public)
         self._private = list(private)
 
+    @staticmethod
+    def __nop_transform(x):
+        return x
+
     @property
     def private(self) -> list:
-        return unique(self._transform(self._private))
+        return unique(self._transform_out(self._private))
 
     @property
     def public(self) -> list:
-        items: list = self._transform(self._public)
+        items: list = self._transform_out(self._public)
         for dep in self._parent.cxx_dependencies:
             items.extend(getattr(dep, self._name).public)
         return unique(items)
     
     def __recurse_public(self) -> list:
         opts = list()
         for dep in self._parent.cxx_dependencies:
@@ -145,19 +156,19 @@
     def public_raw(self) -> list:
         return self._public
 
     def add(self, *values, public=False):
         if public:
             for value in values:
                 if not value in self._public:
-                    self._public.append(value)
+                    self._public.append(self._transform_in(value))
         else:
             for value in values:
                 if not value in self._private:
-                    self._private.append(value)
+                    self._private.append(self._transform_in(value))
 
     def update(self, values: 'OptionSet', private=False):
         self._public = values._public
         if private:
             self._private = values._private
 
 class CXXTarget(Target, internal=True):
@@ -175,49 +186,48 @@
 
     public_link_libraries: set[str] = set()
     private_link_libraries: set[str] = set()
 
     public_link_options: set[str] = set()
     private_link_options: set[str] = set()
 
+    def __make_src_path(self, path):
+        if not isinstance(path, Path):
+            path = Path(path)
+        return path if path.is_absolute() else self.source_path / path
+
     def __init__(self,
                  *args,
                  **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.toolchain : Toolchain = self.context.get('cxx_target_toolchain')
 
         self.includes = OptionSet(self, 'includes',
-                                #   self.public_includes, self.private_includes,
-                                  transform=self.toolchain.make_include_options)
+                                  self.public_includes, self.private_includes,
+                                  transform_out=self.toolchain.make_include_options,
+                                  transform_in=self.__make_src_path)
 
         self.compile_options = OptionSet(self, 'compile_options',
                                          self.public_compile_options, self.private_compile_options)
 
         self.link_libraries = OptionSet(self, 'link_libraries',
-                                        self.public_link_libraries, self.private_link_libraries, transform=self.toolchain.make_link_options)
+                                        self.public_link_libraries, self.private_link_libraries,
+                                        transform_out=self.toolchain.make_link_options)
         
         self.library_paths = OptionSet(self, 'library_paths',
-                                        self.public_lib_paths, self.private_lib_paths, transform=self.toolchain.make_libpath_options)
+                                        self.public_lib_paths, self.private_lib_paths,
+                                        transform_out=self.toolchain.make_libpath_options)
 
         self.compile_definitions = OptionSet(self, 'compile_definitions',
-                                             self.public_compile_definitions, self.private_compile_definitions, transform=self.toolchain.make_compile_definitions)
+                                             self.public_compile_definitions, self.private_compile_definitions,
+                                             transform_out=self.toolchain.make_compile_definitions)
 
         self.link_options = OptionSet(self, 'link_options',
                                       self.public_link_options, self.private_link_options)
-
-        for path in self.public_includes:
-            path = Path(path)
-            self.includes.add(
-                path if path.is_absolute() else self.source_path / path,
-                public=True)
-
-        for path in self.private_includes:
-            path = Path(path)
-            self.includes.add(
-                path if path.is_absolute() else self.source_path / path)
+       
 
     @property
     def cxx_dependencies(self) -> list['CXXTarget']:
         return [dep for dep in self.dependencies if isinstance(dep, CXXTarget)]
 
     @property
     def library_dependencies(self) -> list['Library']:
@@ -426,64 +436,46 @@
                     f'{self.name.upper()}_IMPORT=1', public=True)
         else:
             assert self.interface
             self.output.touch()
 
         self.debug('done')
 
-    @asyncio.cached
-    async def install(self, settings: InstallSettings, mode: InstallMode) -> list[Path]:
-        if mode == InstallMode.user and not self.shared:
-            return list()
-
-        await self.build()
+    async def __install__(self, installer: Installer):
 
         tasks = list()
 
-        if settings.create_pkg_config:
+        if installer.settings.create_pkg_config:
             from dan.pkgconfig.package import create_pkg_config
-            tasks.append(create_pkg_config(self, settings))
-
-        async def do_install(src: Path, dest: Path):
-            if dest.exists() and dest.younger_than(src):
-                self.info('%s is up-to-date', dest)
-            else:
-                self.debug('installing %s', dest)
-                dest.parent.mkdir(parents=True, exist_ok=True)
-                await aiofiles.copy(src, dest)
-            return dest
+            tasks.append(create_pkg_config(self, installer.settings))
 
-        dest = settings.libraries_destination / self.output.name
-        self.info('installing %s to %s', self.name, dest)
-
-        if not self.interface:
-            tasks.append(do_install(self.output, dest))
+        if self.shared:
+            tasks.append(installer.install_shared_library(self.output))
+        elif self.static:
+            tasks.append(installer.install_static_library(self.output))
 
-        if mode == InstallMode.dev:
+        if installer.dev:
             header_expr = re.compile(self.header_match)
-            includes_dest = settings.includes_destination
             for public_include_dir in self.includes.public_raw:
                 headers = public_include_dir.rglob('*.h*')
                 for header in headers:
                     if header_expr.match(str(header)):
-                        dest = includes_dest / \
-                            header.relative_to(public_include_dir)
-                        tasks.append(do_install(header, dest))
+                        subdirs = header.relative_to(public_include_dir).parent
+                        tasks.append(installer.install_header(header, subdirs))
 
-            for obj in self.objs:
-                for dbg_file in self.toolchain.debug_files(obj.output):
-                    tasks.append(do_install(dbg_file, settings.libraries_destination / dbg_file.name))
+            # TODO: how to handle debug symbols ? check where debug it is usually installed and do the same
+            # for obj in self.objs:
+            #     for dbg_file in self.toolchain.debug_files(obj.output):
+            #         tasks.append(do_install(dbg_file, settings.libraries_destination / dbg_file.name))
 
-        tasks.insert(0, super().install(settings, mode))
+        tasks.insert(0, super().__install__(installer))
 
-        result = list()
         for tchunk in chunks(tasks, 100):
-            result.append(await asyncio.gather(*tchunk))
+            await asyncio.gather(*tchunk)
 
-        return result
 
 class Module(CXXObjectsTarget, internal=True):
     def __init__(self, name: str, sources: list[str], *args, **kwargs):
         super().__init__(name, sources, *args, **kwargs)
 
     @property
     def cxx_flags(self):
@@ -491,28 +483,39 @@
 
     async def __build__(self):
         return await super().__build__()
 
 class Executable(CXXObjectsTarget, internal=True):
 
     installed = True
+    subsystem: str = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        if self.subsystem is None:
+            self.subsystem = 'console'
+
         self.output = self.toolchain.make_executable_name(self.name)
         self.__dirty = False
 
+    def _make_link_options(self):
+        subsystem_opt = []
+        if self.toolchain.type == 'msvc':
+            subsystem_opt.append(f'/subsystem:{self.subsystem}')
+        return [*subsystem_opt, *self.lib_paths, *self.libs, *self.link_options.public, *self.link_options.private]
+
+
     async def __initialize__(self):
         await super().__initialize__()
 
         previous_args = self.cache.get('link_args')
         if previous_args:
             args = self.toolchain.make_link_commands([obj.routput for obj in self.objs], self.output,
-                                                     [*self.lib_paths, *self.libs, *self.link_options.public, *self.link_options.private])[0]
+                                                     self._make_link_options())[0]
             args = [str(a) for a in args]
             if sorted(previous_args) != sorted(args):
                 self.__dirty = True
 
     @cached_property
     def up_to_date(self):
         if self.__dirty:
@@ -522,31 +525,24 @@
     async def __build__(self):
         await super().__build__()
 
         # link
         self.info('linking %s...', self.output.name)
         try:
             commands, diags = await self.toolchain.link([obj.routput for obj in self.objs], self.output,
-                                                        [*self.lib_paths, *self.libs, *self.link_options.public, *self.link_options.private])
+                                                        self._make_link_options())
             self.diagnostics.insert(diags, str(self.output))
         except LinkageFailure as err:
             self.diagnostics.insert(err.diags, str(self.output))
             err.target = self
             raise
         self.cache['link_args'] = [str(a) for a in commands[0]]
         self.debug('done')
 
-    @asyncio.cached
-    async def install(self, settings: InstallSettings, mode: InstallMode) -> list[Path]:
-        dest = settings.runtime_destination / self.output.name
-        if dest.exists() and dest.younger_than(self.output):
-            self.info('%s is up-to-date', dest)
-        else:
-            self.info('installing %s', dest)
-            dest.parent.mkdir(parents=True, exist_ok=True)
-            await aiofiles.copy(self.output, dest)
-        return [dest]
+    async def __install__(self, installer: Installer):
+        await installer.install_bin(self.output)
+        await super().__install__(installer)
 
     async def execute(self, *args, build=True, **kwargs):
         if build:
             await self.build()
         return await async_run([self.output, *args], logger=self, env=self.toolchain.env, **kwargs)
```

### Comparing `dan-build-0.2.5/dan/cxx/toolchain.py` & `dan-build-0.2.6/dan/cxx/toolchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,26 +62,40 @@
 
 
 class LinkageFailure(BaseFailure):
     def __init__(self, err: CommandError, objects: set[Path], options: set[str], command: str, toolchain: 'Toolchain', diags: list[diag.Diagnostic] = [], target = None) -> None:
         super().__init__(f'failed to link {", ".join([str(o) for o in objects])}: {err.stdout}{err.stderr}', err, options, command, toolchain, diags, target)
         self.objects = objects
 
+class SystemName(str):
+    
+    @property
+    def is_windows(self):
+        if self == 'windows':
+            return True
+        if self.startswith('msys'):
+            return True
+        return False
+    
+    @property
+    def is_linux(self):
+        return self == 'linux'
+
 
 class Toolchain(Logging):
     def __init__(self, data: dict[str,str], tools: dict, settings: ToolchainSettings, cache: dict = None) -> None:
         self.cc : Path = None
         self.cxx : Path = None
         self.tools = tools
         self._compile_commands: CompileCommands = None
         self.cxx_flags = set()
         self.cpp_std = 17
         self.type = data['type']
         # self.arch = data['arch']
-        self.system = data['system']
+        self.system = SystemName(data['system'])
         self.version = Version(data['version'])
         self.settings = settings
         self.cache = dict() if cache is None else cache
         Logging.__init__(self, f'{self.type}-{self.version}')
         self.env = None
         self.rpath = None
         self._build_type = BuildType.debug
@@ -119,15 +133,21 @@
         arch = get_target_arch(defines)
         self.cache['defines'] = defines
         self.cache['arch'] = arch
         self.cache['arch_detect_flags'] = self.settings.cxx_flags
         
         from dan.core.osinfo import OSInfo
         osi = OSInfo()
-        self.cache['is_host'] = self.system == osi.name and self.arch == osi.arch
+        osi.name = SystemName(osi.name)
+        is_host = False
+        if self.arch == osi.arch:
+            if self.system == osi.name or self.system.is_windows and osi.name.is_windows:
+                is_host = True
+
+        self.cache['is_host'] = is_host
 
     async def get_default_defines(self) -> dict[str, str]:
         return self.cache['defines']
 
     # @property
     # def compile_commands(self):
     #     if not self._compile_commands:
```

### Comparing `dan-build-0.2.5/dan/cxx/unix_toolchain.py` & `dan-build-0.2.6/dan/cxx/unix_toolchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 cxx_extensions = ['.cpp', '.cxx', '.C', '.cc']
 c_extensions = ['.c']
 
 
 class UnixToolchain(Toolchain):
     def __init__(self, data, tools, *args, **kwargs):
         Toolchain.__init__(self, data, tools, *args, **kwargs)
-        self.cc = data['cc']
-        self.cxx = data['cxx']
+        self.cc = Path(data['cc'])
+        self.cxx = Path(data['cxx'])
         self.ar = data['ar'] if 'ar' in data else tools['ar']
         self.ranlib = data['ranlib'] if 'ranlib' in data else tools['ranlib']
         # self.as_ = data['as'] if 'as' in data else tools['as']
         # self.strip = data['env']['STRIP'] if 'env' in data and 'STRIP' in data['env'] else tools['strip']
         self.env = data['env'] if 'env' in data else None
         self.debug('cxx compiler is %s %s (%s)', self.type, self.version, self.cc)
         self.debug('cxx compiler is %s %s (%s)', self.type, self.version, self.cxx)
```

### Comparing `dan-build-0.2.5/dan/io/package.py` & `dan-build-0.2.6/dan/io/package.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from dan.core.target import Target
 from dan.core.find import find_file, find_files
 from dan.core.version import Version, VersionSpec
 from dan.io.repositories import get_packages_path, get_repo_instance
 
 
 class PackageBuild(Target, internal=True):
-
-    _all_builds: dict[str, 'PackageBuild'] = dict()
     
     def __init__(self, name, version, package, repository, *args, spec: VersionSpec = None, **kwargs):
         self.spec = spec
         self.pn = name
         super().__init__(f'{name}-build', *args, version=version, **kwargs)
         self.package = name if package is None else package
         self.repo = get_repo_instance(repository, self.makefile)
         self.preload_dependencies.add(self.repo)
         self._package_makefile = None
         self._build_path = None
+        self.toolchain = self.context.get('cxx_target_toolchain')
+        self.lock: aiofiles.FileLock = None
 
     @property
     def package_makefile(self):
         if self._package_makefile is None:
             target = self.repo.find(self.pn, self.package)
             if target is None:
                 raise RuntimeError(f'cannot find {self.pn} in {self.repo.name}')
@@ -62,67 +62,76 @@
         # set package version
         version_option = makefile.options.get('version')
         if self.version is None:
             self.version = Version(version_option.value)
         else:
             version_option.value = str(self.version)
 
-        toolchain = self.context.get('cxx_target_toolchain')
-        self._build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / self.package / str(self.version)
+        pkgs_root = packages_path / self.toolchain.system / self.toolchain.arch / self.toolchain.build_type.name
+        makefile.pkgs_path = pkgs_root / self.package / str(self.version)
+
+        self._build_path = makefile.pkgs_path
+        self.lock = aiofiles.FileLock(self.build_path / 'build.lock')
+
         self.install_settings = InstallSettings(self.build_path)
         
         # update package build-path
         makefile.build_path = self.build_path / 'build'
 
 
         # set our output to the last installed package
         # TODO handle multiple outputs, then set our outputs to all installed packages
         pkg_name = makefile.all_installed[-1].name     
         self.output = Path(self.install_settings.libraries_prefix) / 'pkgconfig' / f'{pkg_name}.pc'
+        
+        for pkg in find_files(r'.+\.pc$', [self.install_settings.libraries_destination, self.install_settings.data_destination]):
+            self.output = pkg
+            break
+
         sources.output = self.build_path / 'src' # TODO source_prefix in install settings
 
         return await super().__initialize__()
     
     @property
     def build_path(self) -> Path:
         return self._build_path
     
     async def __build__(self):
-        ident = f'{self.package}-{self.version}'
-        if ident in self._all_builds:
-            self.debug(f'{ident} already built by {self._all_builds[ident].fullname}')
-            await self._all_builds[ident].build()
-            return
-
-        self._all_builds[ident] = self
-
-        makefile = self.package_makefile
-        build_path = makefile.build_path
-
-        # FIXME: shall a makefile have an associated toolchain ?
-        toolchain = None
-        async with asyncio.TaskGroup(f'installing {self.package}\'s targets') as group:
-            for target in makefile.all_installed:
-                if hasattr(target, 'toolchain'):
-                    if toolchain is None:
-                        toolchain = target.toolchain
-                    else:
-                        assert toolchain == target.toolchain, 'Toolchain missmatch'
-                group.create_task(target.install(self.install_settings, InstallMode.dev))
-
-        makefile.cache.ignore()
-        del makefile
-
-        os.chdir(self.build_path.parent)
-
-        self.debug('cleaning')
-        async with asyncio.TaskGroup(f'cleanup {self.package}') as group:
-            if toolchain is not None and not toolchain.build_type.is_debug_mode:
-                group.create_task(aiofiles.rmtree(self.output / 'src'))
-            group.create_task(aiofiles.rmtree(build_path, force=True))
+        if self.lock.locked:
+            self.debug('package %s %s already building...', self.name, self.version)
+            # wait for it
+            async with self.lock:
+                return
+
+        async with self.lock:
+
+            makefile = self.package_makefile
+            build_path = makefile.build_path
+
+            # FIXME: shall a makefile have an associated toolchain ?
+            toolchain = None
+            async with asyncio.TaskGroup(f'installing {self.package}\'s targets') as group:
+                for target in makefile.all_installed:
+                    if hasattr(target, 'toolchain'):
+                        if toolchain is None:
+                            toolchain = target.toolchain
+                        else:
+                            assert toolchain == target.toolchain, 'Toolchain missmatch'
+                    group.create_task(target.install(self.install_settings, InstallMode.dev))
+
+            makefile.cache.ignore()
+            del makefile
+
+            os.chdir(self.build_path.parent)
+
+            self.debug('cleaning')
+            async with asyncio.TaskGroup(f'cleanup {self.package}') as group:
+                if toolchain is not None and not toolchain.build_type.is_debug_mode:
+                    group.create_task(aiofiles.rmtree(self.output / 'src'))
+                group.create_task(aiofiles.rmtree(build_path, force=True))
 
 
 class Package(Target, internal=True):
 
     __all: dict[str, 'Package'] = dict()
 
     def __init__(self,
@@ -135,25 +144,27 @@
         if version is not None:
             self.version = version
         if name is not None:
             self.name = name
         super().__init__(**kwargs)
         if self.name in self.__all:
             raise RuntimeError(f'duplicate package: {self.name}')
-        self.__all[self.name] = self
+        self.__all[self.package] = self
 
     @classmethod
-    def instance(cls, name, version, *args, **kwargs):
-        if name in cls.__all:
-            pkg = cls.__all[name]
-            if not version.is_compatible(pkg.version):
+    def instance(cls, name, version, *args, package=None, **kwargs):
+        if package is None:
+            package = name
+        if package in cls.__all:
+            pkg = cls.__all[package]
+            if version is not None and not version.is_compatible(pkg.version):
                 raise RuntimeError(f'incompatible package version: {pkg.version} {version}')
             return pkg, False
         else:
-            return Package(name, version, *args, **kwargs), True
+            return Package(name, version, package, *args, **kwargs), True
 
     
     async def __initialize__(self):
 
         match self.version:
             case str():
                 _name, spec = VersionSpec.parse(self.version)
@@ -175,32 +186,59 @@
         self.pkg_build = PackageBuild(self.name,
                                       self.version,
                                       self.package,
                                       self.repository,
                                       spec=self.spec,
                                       makefile=self.makefile)
         self.dependencies.add(self.pkg_build)
-        self.pkgconfig_path = Path('pkgs') / 'lib' / 'pkgconfig'
-        self.dan_path = Path('pkgs') / 'lib' / 'dan'
+        lib_path = Path('pkgs') / 'lib'
+        self.pkgconfig_path = lib_path / 'pkgconfig'
+        self.cmake_path = lib_path / 'cmake' / self.name
+        self.dan_path = lib_path / 'dan'
+        
         self.output = self.pkgconfig_path / f'{self.name}.pc'
+
         return await super().__initialize__()
     
+    async def _import_cmake_pkg(self, pkg: Path):
+        self.debug('copying %s to %s', pkg, self.build_path / self.cmake_path)
+        content = [
+            f'set(CMAKE_CURRENT_LIST_FILE "{pkg.absolute().as_posix()}")\n',
+            f'set(CMAKE_CURRENT_LIST_DIR "{pkg.parent.absolute().as_posix()}")\n'
+        ]
+        async with aiofiles.open(pkg) as f:
+            content.extend(await f.readlines())
+        dest = self.build_path / self.cmake_path / pkg.name
+        dest.parent.mkdir(parents=True, exist_ok=True)
+        async with aiofiles.open(dest, 'w') as f:
+            await f.writelines(content)
+
+    
     async def __build__(self):
-        self.pkgconfig_path.mkdir(exist_ok=True, parents=True)
-        self.dan_path.mkdir(exist_ok=True, parents=True)      
+        (self.build_path / self.pkgconfig_path).mkdir(exist_ok=True, parents=True)
+        (self.build_path / self.dan_path).mkdir(exist_ok=True, parents=True)
+        (self.build_path / self.cmake_path).mkdir(exist_ok=True, parents=True)
 
         async with asyncio.TaskGroup(f'importing {self.name} package') as group:
             for pkg in find_files(r'.+\.pc$', [self.pkg_build.install_settings.libraries_destination / 'pkgconfig']):
                 self.debug('copying %s to %s', pkg, self.build_path / self.pkgconfig_path)
                 group.create_task(aiofiles.copy(pkg, self.build_path / self.pkgconfig_path))
 
-            for pkg in find_files(r'.+\.py$', [self.pkg_build.install_settings.libraries_destination / 'dan']):
+            for pkg in find_files(r'.+\.pc$', [self.pkg_build.install_settings.data_destination / 'pkgconfig']):
+                self.debug('copying %s to %s', pkg, self.build_path / self.pkgconfig_path)
+                group.create_task(aiofiles.copy(pkg, self.build_path / self.pkgconfig_path))
+
+            for pkg in find_files(r'.+\.py$', [self.pkg_build.install_settings.data_destination / 'dan']):
                 self.debug('copying %s to %s', pkg, self.build_path / self.dan_path)
                 group.create_task(aiofiles.copy(pkg, self.build_path / self.dan_path))
-        
+
+            for pkg in find_files(r'.+\.cmake$', [self.pkg_build.install_settings.libraries_destination / 'cmake']):
+                self.debug('copying %s to %s', pkg, self.build_path / self.cmake_path)
+                group.create_task(self._import_cmake_pkg(pkg))
+
         if self.output.exists():
             from dan.pkgconfig.package import Data, find_package
             data = Data(self.output)
             async with asyncio.TaskGroup(f'importing {self.name} package requirements') as group:
                 toolchain = self.context.get('cxx_target_toolchain')
                 search_path = get_packages_path() / toolchain.system / toolchain.arch / toolchain.build_type.name
                 dest = self.build_path / self.pkgconfig_path
```

### Comparing `dan-build-0.2.5/dan/io/repositories.py` & `dan-build-0.2.6/dan/io/repositories.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from dan.core.asyncio import sync_wait
 from dan.core.makefile import MakeFile
 
 from dan.cxx.detect import get_dan_path
 from dan.core.target import Target
-from dan.core.runners import async_run
+from dan.core.runners import CommandError, async_run
 from dan.core import aiofiles
 from dan.core.cache import Cache
 
 from dataclasses_json import dataclass_json
 from dataclasses import dataclass, field
 
 import typing as t
@@ -16,113 +16,130 @@
 
 @dataclass
 class RepositoryConfig:
     name: str
     url: str
     branch: str = 'main'
 
+
 @dataclass
 class GitHubConfig:
-    api_token: str = None
+    api_token: t.Optional[str] = None
+
 
 @dataclass_json
 @dataclass
 class RepositoriesSettings:
-    github: t.Optional[GitHubConfig] = field(default_factory = GitHubConfig)
+    github: GitHubConfig = field(default_factory=GitHubConfig)
     repositories: list[RepositoryConfig] = field(default_factory=lambda: [
         RepositoryConfig('dan.io', 'https://github.com/Garcia6l20/dan.io.git'),
     ])
 
     def get(self, name):
         for config in self.repositories:
             if config.name == name:
                 return config
-    
+
     @property
     def default(self):
         return self.repositories[0]
 
 
 class RepositoriesConfig(Cache[RepositoriesSettings]):
     indent = 2
 
 
-
 _repo_settings: RepositoriesConfig = None
-_repo_instances : dict[str, 'PackageRepository'] = dict()
+_repo_instances: dict[str, 'PackageRepository'] = dict()
+
 
 def _get_settings() -> RepositoriesSettings:
     global _repo_settings
     if _repo_settings is None:
-        _repo_settings = RepositoriesConfig(get_dan_path() / 'repositories.json')
+        _repo_settings = RepositoriesConfig(
+            get_dan_path() / 'repositories.json')
         if not _repo_settings.path.exists():
             sync_wait(_repo_settings.save(force=True))
     return _repo_settings.data
 
 
 class PackageRepository(Target, internal=True):
 
     # never up-to-date
     up_to_date = False
 
-    def __init__(self, name : RepositoryConfig, *args, **kwargs):
+    def __init__(self, name: RepositoryConfig, *args, **kwargs):
         self.repo_data = _get_settings().get(name)
         super().__init__(name, *args, **kwargs)
         self.output = get_dan_path() / 'repositories' / self.name
+        self.toolchain = self.context.get('cxx_target_toolchain')
+        self.pkgs_root = get_packages_path() / self.toolchain.system / \
+            self.toolchain.arch / self.toolchain.build_type.name
         self._package_makefile = None
 
     async def __build__(self):
         if not self.output.exists():
             try:
                 self.output.parent.mkdir(exist_ok=True, parents=True)
                 await async_run(f'git clone -b {self.repo_data.branch} {self.repo_data.url} {self.name}', logger=self, cwd=self.output.parent)
 
             except Exception as e:
                 await aiofiles.rmtree(self.output)
                 raise e
         else:
+            try:
                 await async_run(f'git pull -q', logger=self, cwd=self.output)
+            except CommandError:
+                self.warning('cannot update %s', self.name)
 
     @property
     def pkgs_makefile(self) -> MakeFile:
         if self._package_makefile is None:
             from dan.core.include import load_makefile
             root = self.output / 'packages'
-            requirements = None
             with self.makefile.context:
-                self._package_makefile = load_makefile(root / 'dan-build.py', f'{self.name}.packages', requirements=requirements, build_path=self.build_path / self.name, parent=self.makefile)
+                self._package_makefile = load_makefile(root / 'dan-build.py',
+                                                       f'{self.name}.packages',
+                                                       requirements=None,
+                                                       build_path=self.build_path / self.name,
+                                                       parent=self.makefile,
+                                                       is_requirement=True)
+                self._package_makefile.pkgs_path = self.pkgs_root
 
         return self._package_makefile
 
     @property
     def installed(self) -> dict[str, Target]:
         pkgs = self.pkgs_makefile
-        return {f'{lib.makefile.name}:{lib.name}@{self.name}' : lib for lib in pkgs.all_installed}
-    
+        return {f'{lib.makefile.name}:{lib.name}@{self.name}': lib for lib in pkgs.all_installed}
+
     def find(self, name: str, package: str) -> Target:
         if package is None:
             package = name
 
         for lib in self.pkgs_makefile.all_installed:
-            if lib.name == name and lib.makefile.name == package:
+            if name in lib.provides and lib.makefile.name == package:
                 return lib
 
-def get_repo_instance(repo_name:str, makefile=None) -> PackageRepository:
+
+def get_repo_instance(repo_name: str, makefile=None) -> PackageRepository:
     if makefile is None:
         from dan.core.include import context
         makefile = context.root
 
     if repo_name is None:
         repo_name = _get_settings().default.name
 
     if not repo_name in _repo_instances:
-        _repo_instances[repo_name] = PackageRepository(repo_name, makefile=makefile)
+        _repo_instances[repo_name] = PackageRepository(
+            repo_name, makefile=makefile)
     return _repo_instances[repo_name]
 
 
 def get_all_repo_instances(makefile=None) -> list[PackageRepository]:
     for repo in _get_settings().repositories:
         get_repo_instance(repo.name, makefile)
     return _repo_instances.values()
 
+
 def get_packages_path() -> Path:
     return get_dan_path() / 'packages'
```

### Comparing `dan-build-0.2.5/dan/jinja.py` & `dan-build-0.2.6/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/logging.py` & `dan-build-0.2.6/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/make.py` & `dan-build-0.2.6/dan/make.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 import os
 import fnmatch
 import re
 
 from dataclasses_json import dataclass_json
 import sys
 import tqdm
-import typing as t
 from collections.abc import Iterable
 
+import dan.core.typing as t
 from dan.core import diagnostics as diag
 from dan.core.cache import Cache
 from dan.core.makefile import MakeFile
 from dan.core.pathlib import Path
 from dan.core.include import MakeFileError, include_makefile, Context
 from dan.core import aiofiles, asyncio
-from dan.core.settings import InstallMode, Settings
+from dan.core.requirements import load_requirements
+from dan.core.settings import InstallMode, InstallSettings, Settings
 from dan.core.test import Test
 from dan.core.utils import unique
 from dan.cxx import init_toolchains
 from dan.logging import Logging
 from dan.core.target import Option, Target
 from dan.cxx.targets import Executable
 from dan.core.runners import max_jobs
@@ -314,111 +315,27 @@
                 return False
         for target in [target for target in self.root.all_targets if isinstance(target, CXXObjectsTarget)]:            
             if target.source_path not in source.parents:
                 continue
             if check(target):
                 return target
 
-
-    @classmethod
-    def _parse_str_value(cls, name, value: str, orig: type, tp: type = None):
-        if issubclass(orig, Enum):
-            names = [n.lower()
-                        for n in orig._member_names_]
-            value = value.lower()
-            if value in names:
-                return orig(names.index(value))
-            else:
-                raise RuntimeError(f'{name} should be one of {names}')
-        elif issubclass(orig, (set, list)):
-            assert tp is not None
-            result = list()
-            for sub in value.split(';'):
-                result.append(cls._parse_str_value(name, sub, tp))
-            return orig(result)
-        elif orig == bool:
-            return value.lower() in ('true', 'yes', 'on', '1')
-        else:
-            if tp is not None:
-                raise TypeError(f'unhandled type {orig}[{tp}]')
-            return orig(value)
-
-    
-    @classmethod
-    def _apply_inputs(self, inputs: list[str], get_item: t.Callable[[str], tuple[t.Any, t.Any, t.Any]], info: t.Callable[[t.Any], t.Any]):
-        for input in inputs:
-            m = re.match(r'(.+?)([+-])?="?(.+)"?', input)
-            if m:
-                name = m[1]
-                op = m[2]
-                value = m[3]
-                input, out_value, orig = get_item(name)
-                sname = name.split('.')[-1]
-                if orig is None:
-                    orig = type(input)
-                if hasattr(orig, '__annotations__') and sname in orig.__annotations__:
-                    tp = orig.__annotations__[sname]
-                    orig = t.get_origin(tp)
-                    if orig is None:
-                        orig = tp
-                        tp = None
-                    else:
-                        args = t.get_args(tp)
-                        if args:
-                            tp = args[0]
-                else:
-                    tp = None
-                in_value = self._parse_str_value(name, value, orig, tp)
-                match (out_value, op, in_value):
-                    case (list()|set(), '-', list()|set()) if len(in_value) == 1 and list(in_value)[0] == '*':
-                        out_value.clear()
-                    case (set(), '+', set()):
-                        out_value.update(in_value)
-                    case (set(), '-', set()):
-                        out_value = out_value - in_value
-                    case (list(), '+', set()|list()):
-                        out_value.extend(in_value)
-                    case (list(), '-', set()|list()):
-                        for v in in_value:
-                            out_value.remove(v)
-                    case (_, '+' | '-', _):
-                        raise TypeError(f'unhandled "{op}=" operator on type {type(out_value)} ({name})')
-                    case _:
-                        out_value = in_value
-                if isinstance(input, dict):
-                    input[sname] = out_value
-                else:
-                    setattr(input, sname, out_value)
-                info(name, out_value)
-            else:
-                raise RuntimeError(f'cannot process given input: {input}')
-
     async def apply_options(self, *options):
         await self.initialize()
+        from dan.core.settings import _apply_inputs
         all_opts = self.all_options
         def get_option(name):
             for opt in all_opts:
                 if opt.fullname == name:
                     return opt.cache, opt.value, opt.type
-        self._apply_inputs(options, get_option, lambda k, v: self.info(f'option: {k} = {v}'))
+        _apply_inputs(options, get_option, logger=self, input_type_name='option')
 
     async def apply_settings(self, *settings):
-        # dont init for settings
-        def get_setting(name):
-            parts = name.split('.')
-            setting = self.settings
-            for part in parts[:-1]:
-                if not hasattr(setting, part):
-                    raise RuntimeError(f'no such setting: {name}')
-                setting = getattr(setting, part)
-            if not hasattr(setting, parts[-1]):
-                raise RuntimeError(f'no such setting: {name}')
-            value = getattr(setting, parts[-1])
-            return setting, value, type(setting)
-        self._apply_inputs(settings, get_setting, lambda k, v: self.info(f'setting: {k} = {v}'))
+        from dan.core.settings import apply_settings
+        apply_settings(self.settings, *settings, logger=self)
 
 
     @staticmethod
     def toolchains():
         from dan.cxx.detect import get_toolchains
         return get_toolchains()
 
@@ -485,14 +402,45 @@
                     self._logger.error(str(result))
                     errors.append(result)
             err_count = len(errors)
             if err_count == 1:
                 raise errors[0]
             elif err_count > 1:
                 raise asyncio.ExceptionGroup('Multiple errors occured while building the project', errors=errors)
+    
+    
+    async def _install_target_deps(self, t: Target):
+        deps_install_path = self.root.pkgs_path
+        deps_settings = InstallSettings(deps_install_path)
+        try:
+            await load_requirements(t.requires, makefile=self.root, logger=self, install=True)
+
+        except Exception as err:
+            self._diagnostics.update(gen_python_diags(err))
+            raise
+    
+    async def install_dependencies(self, targets: list[Target] = None):
+        await self.initialize()
+
+        if targets is None:
+            targets = self.targets
+
+        with self.context, \
+             self.progress('installing deps', targets, self._install_target_deps, self.no_progress) as tasks:
+            results = await asyncio.gather(*tasks, return_exceptions=True)
+            errors = list()
+            for result in results:
+                if isinstance(result, Exception):
+                    self._logger.error(str(result))
+                    errors.append(result)
+            err_count = len(errors)
+            if err_count == 1:
+                raise errors[0]
+            elif err_count > 1:
+                raise asyncio.ExceptionGroup('Multiple errors occured while installing project dependencies', errors=errors)
 
     async def _install_target(self, t: Target, mode: InstallMode):
         try:
             return await t.install(self.settings.install, mode)
         except Exception as err:
             self._diagnostics.update(gen_python_diags(err))
             raise
```

### Comparing `dan-build-0.2.5/dan/pkgconfig/package.py` & `dan-build-0.2.6/dan/pkgconfig/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,16 @@
             raise MissingPackage(name)
         self.search_paths.insert(0, self.config_path.parent)
         self.pn = name
         self.all[name] = self
 
         super().__init__(f'{name}-pkgconfig', **kwargs)
 
-        dan_plugin = self.config_path.parent.parent / \
-            'dan' / f'{name}.py'
-        if dan_plugin.exists():
+        dan_plugin = find_file(rf'{name}\.py', [self.config_path.parent.parent])
+        if dan_plugin is not None:
             spec = importlib.util.spec_from_file_location(
                 f'{name}_plugin', dan_plugin)
             module = importlib.util.module_from_spec(spec)
             setattr(module, 'self', self)
             spec.loader.exec_module(module)
         self.__cflags = None
         self.__libs = None
@@ -270,15 +269,15 @@
     if _jinja_env is None:
         _jinja_env = jinja2.Environment(
             loader=jinja2.PackageLoader('dan.pkgconfig'))
     return _jinja_env
 
 
 async def create_pkg_config(lib: Library, settings: InstallSettings) -> Path:
-    dest = settings.libraries_destination / 'pkgconfig' / f'{lib.name}.pc'
+    dest = settings.data_destination / 'pkgconfig' / f'{lib.name}.pc'
     lib.info(f'creating pkgconfig: {dest}')
 
     requires = list()
     for dep in lib.dependencies:
         match dep:
             case RequiredPackage():
                 if dep.version_spec:
```

### Comparing `dan-build-0.2.5/dan/src/git.py` & `dan-build-0.2.6/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/src/github.py` & `dan-build-0.2.6/dan/src/github.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan/src/tar.py` & `dan-build-0.2.6/dan/src/tar.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.6/dan_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.5/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.6/dan_build.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dan/cli/__init__.py
 dan/cli/click.py
 dan/cli/io.py
 dan/cli/main.py
 dan/cli/vscode.py
 dan/cmake/__init__.py
 dan/cmake/configure_file.py
+dan/cmake/project.py
 dan/conan/__init__.py
 dan/conan/requirements.py
 dan/core/__init__.py
 dan/core/aiofiles.py
 dan/core/asyncio.py
 dan/core/cache.py
 dan/core/detect.py
@@ -37,14 +38,15 @@
 dan/core/pm.py
 dan/core/register.py
 dan/core/requirements.py
 dan/core/runners.py
 dan/core/settings.py
 dan/core/target.py
 dan/core/test.py
+dan/core/typing.py
 dan/core/utils.py
 dan/core/version.py
 dan/core/win.py
 dan/cxx/__init__.py
 dan/cxx/compile_commands.py
 dan/cxx/detect.py
 dan/cxx/msvc_toolchain.py
```

### Comparing `dan-build-0.2.5/pyproject.toml` & `dan-build-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "pyyaml",
     "aiofiles",
     "aiohttp",
     "termcolor",
     "tqdm",
     'importlib-metadata',
     'dataclasses-json',
+    'lockfile',
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["dan*"]
```

### Comparing `dan-build-0.2.5/tests/test_cxx_errors.py` & `dan-build-0.2.6/tests/test_cxx_errors.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/tests/test_cxx_libraries.py` & `dan-build-0.2.6/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/tests/test_cxx_simple.py` & `dan-build-0.2.6/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/tests/test_cxx_src_catch2.py` & `dan-build-0.2.6/tests/test_cxx_src_catch2.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.5/tests/test_python_errors.py` & `dan-build-0.2.6/tests/test_python_errors.py`

 * *Files identical despite different names*

