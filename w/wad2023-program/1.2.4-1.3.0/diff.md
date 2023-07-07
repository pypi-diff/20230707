# Comparing `tmp/wad2023-program-1.2.4.tar.gz` & `tmp/wad2023-program-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.2.4.tar", last modified: Fri Jun 30 08:30:40 2023, max compression
+gzip compressed data, was "wad2023-program-1.3.0.tar", last modified: Fri Jul  7 21:00:07 2023, max compression
```

## Comparing `wad2023-program-1.2.4.tar` & `wad2023-program-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:30:40.983066 wad2023-program-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 08:30:40.983066 wad2023-program-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:30:40.987066 wad2023-program-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:30:40.979066 wad2023-program-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:30:40.983066 wad2023-program-1.2.4/src/wad2023_program/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/src/wad2023_program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/src/wad2023_program/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/src/wad2023_program/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/src/wad2023_program/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-30 08:30:29.000000 wad2023-program-1.2.4/src/wad2023_program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:30:40.983066 wad2023-program-1.2.4/src/wad2023_program.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 08:30:40.000000 wad2023-program-1.2.4/src/wad2023_program.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:07.433345 wad2023-program-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-07 21:00:07.433345 wad2023-program-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:00:07.433345 wad2023-program-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:07.429345 wad2023-program-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:07.429345 wad2023-program-1.3.0/src/wad2023_program/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/sessionize_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-07 20:59:57.000000 wad2023-program-1.3.0/src/wad2023_program/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:07.433345 wad2023-program-1.3.0/src/wad2023_program.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 21:00:07.000000 wad2023-program-1.3.0/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.2.4/LICENSE` & `wad2023-program-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.4/pyproject.toml` & `wad2023-program-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.2.4"
+version = "1.3.0"
 description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
 readme = "README.md"
 authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -18,41 +18,43 @@
     "requests >= 2.27.0",
     "pydantic >= 1.10.0",
     "beautifulsoup4 >= 4.12.0",
     "python-dateutil >= 2.8.0",
     "rich >= 13.4.0",
     "typer >= 0.9.0",
     "pytz >= 2023.3",
+    "sqlmodel == 0.0.8",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     'pytest >= 7.3.0',
     'pycodestyle == 2.10.0',
     'autopep8 == 2.0.0',
     'pylint == 2.17.0',
     'mypy == 1.3.0',
     'flake8 == 6.0.0',
     'pydocstyle == 6.3.0',
+    'pg8000 >= 1.29.0',
 ]
 
 [project.urls]
 homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 
 [project.scripts]
-wad23 = "wad2023_program.__main__:main"
+wad23 = "wad2023_program.__main__:app"
 
 [tool.bumpver]
-current_version = "1.2.4"
+current_version = "1.3.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
-tag = false
+tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/wad2023_program/__init__.py" = ["{version}"]
 
 [tool.pytest.ini_options]
```

