# Comparing `tmp/pyvipe-0.2.0.tar.gz` & `tmp/pyvipe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvipe-0.2.0.tar", last modified: Thu Jul  6 14:03:07 2023, max compression
+gzip compressed data, was "pyvipe-0.2.1.tar", last modified: Fri Jul  7 19:45:54 2023, max compression
```

## Comparing `pyvipe-0.2.0.tar` & `pyvipe-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.151829 pyvipe-0.2.0/
--rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.2.0/LICENSE
--rw-r--r--   0 constantinhong   (501) staff       (20)    23767 2023-07-06 14:03:07.151471 pyvipe-0.2.0/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)     1971 2023-07-06 14:01:53.000000 pyvipe-0.2.0/README.md
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.143688 pyvipe-0.2.0/completion/
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.146060 pyvipe-0.2.0/completion/bash/
--rw-r--r--   0 constantinhong   (501) staff       (20)      263 2023-07-06 14:01:53.000000 pyvipe-0.2.0/completion/bash/vipe
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.146390 pyvipe-0.2.0/completion/zsh/
--rw-r--r--   0 constantinhong   (501) staff       (20)      374 2023-07-06 14:01:53.000000 pyvipe-0.2.0/completion/zsh/_vipe
--rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-07-06 14:01:53.000000 pyvipe-0.2.0/pyproject.toml
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.148517 pyvipe-0.2.0/pyvipe/
--rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-07-06 12:47:12.000000 pyvipe-0.2.0/pyvipe/__init__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.2.0/pyvipe/__main__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     3108 2023-07-06 14:01:53.000000 pyvipe-0.2.0/pyvipe/pyvipe.py
--rw-r--r--   0 constantinhong   (501) staff       (20)       22 2023-07-06 12:39:52.000000 pyvipe-0.2.0/pyvipe/version.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.150923 pyvipe-0.2.0/pyvipe.egg-info/
--rw-r--r--   0 constantinhong   (501) staff       (20)    23767 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      309 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/SOURCES.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/dependency_links.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/entry_points.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/top_level.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-07-06 14:03:07.151938 pyvipe-0.2.0/setup.cfg
--rw-r--r--   0 constantinhong   (501) staff       (20)     1456 2023-07-06 14:01:53.000000 pyvipe-0.2.0/setup.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.542585 pyvipe-0.2.1/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.2.1/LICENSE
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23807 2023-07-07 19:45:54.542209 pyvipe-0.2.1/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)     2011 2023-07-07 19:43:33.000000 pyvipe-0.2.1/README.md
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.533627 pyvipe-0.2.1/completion/
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.535693 pyvipe-0.2.1/completion/bash/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      263 2023-07-06 14:01:53.000000 pyvipe-0.2.1/completion/bash/vipe
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.536379 pyvipe-0.2.1/completion/zsh/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      374 2023-07-06 14:01:53.000000 pyvipe-0.2.1/completion/zsh/_vipe
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-07-07 19:43:51.000000 pyvipe-0.2.1/pyproject.toml
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.538719 pyvipe-0.2.1/pyvipe/
+-rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-07-06 12:47:12.000000 pyvipe-0.2.1/pyvipe/__init__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.2.1/pyvipe/__main__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     3108 2023-07-07 19:44:21.000000 pyvipe-0.2.1/pyvipe/pyvipe.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)       22 2023-07-06 12:39:52.000000 pyvipe-0.2.1/pyvipe/version.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-07 19:45:54.541511 pyvipe-0.2.1/pyvipe.egg-info/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23807 2023-07-07 19:45:54.000000 pyvipe-0.2.1/pyvipe.egg-info/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      309 2023-07-07 19:45:54.000000 pyvipe-0.2.1/pyvipe.egg-info/SOURCES.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-07-07 19:45:54.000000 pyvipe-0.2.1/pyvipe.egg-info/dependency_links.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-07-07 19:45:54.000000 pyvipe-0.2.1/pyvipe.egg-info/entry_points.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-07-07 19:45:54.000000 pyvipe-0.2.1/pyvipe.egg-info/top_level.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-07-07 19:45:54.542693 pyvipe-0.2.1/setup.cfg
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1456 2023-07-07 19:44:35.000000 pyvipe-0.2.1/setup.py
```

### Comparing `pyvipe-0.2.0/LICENSE` & `pyvipe-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvipe-0.2.0/PKG-INFO` & `pyvipe-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.2.0
+Version: 0.2.1
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
@@ -413,21 +413,22 @@
 
 ### Editor exited nonzero, aborting.
 
 In general, editor can exit with nonzero when you execute some command for various purposes. e.g preventing git rebase.
 But if you didn't execute the command but the editor exited with nonzero, it may be because
 of wrong user configuration for the editor.
 
-For vi, you can debug it with `EDITOR='vi -u NONE vipe'`
+For vi, you can debug it with `EDITOR='vi -u NONE' vipe`
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | add universal-newline option. support editor variable with option. | 
+| HEAD    | fix UnicodeEncodeError. | 
+| 0.2.0    | add universal-newline option. support editor variable with option. | 
 | 0.1.3    | fix shell completion. | 
 | 0.1.2    | add suffix option. fix error. | 
 | 0.1.1   | init                     | 
 
 ## CONTRIBUTION
 
 If it doesn't work as original [vipe](http://joeyh.name/code/moreutils/), then it's a bug.
```

### Comparing `pyvipe-0.2.0/README.md` & `pyvipe-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,21 +47,22 @@
 
 ### Editor exited nonzero, aborting.
 
 In general, editor can exit with nonzero when you execute some command for various purposes. e.g preventing git rebase.
 But if you didn't execute the command but the editor exited with nonzero, it may be because
 of wrong user configuration for the editor.
 
-For vi, you can debug it with `EDITOR='vi -u NONE vipe'`
+For vi, you can debug it with `EDITOR='vi -u NONE' vipe`
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | add universal-newline option. support editor variable with option. | 
+| HEAD    | fix UnicodeEncodeError. | 
+| 0.2.0    | add universal-newline option. support editor variable with option. | 
 | 0.1.3    | fix shell completion. | 
 | 0.1.2    | add suffix option. fix error. | 
 | 0.1.1   | init                     | 
 
 ## CONTRIBUTION
 
 If it doesn't work as original [vipe](http://joeyh.name/code/moreutils/), then it's a bug.
```

### Comparing `pyvipe-0.2.0/pyproject.toml` & `pyvipe-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyvipe"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 maintainers = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 license = {file = "LICENSE"}
```

### Comparing `pyvipe-0.2.0/pyvipe/pyvipe.py` & `pyvipe-0.2.1/pyvipe/pyvipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import subprocess
 import sys
 import tempfile
 import argparse
 
-VERSION_HELP = """pyvipe - 0.2.0
+VERSION_HELP = """pyvipe - 0.2.1
 Copyright (C) 2023 Constantin Hong
 License GPLv2: GNU GPL version 2 <https://gnu.org/licenses/gpl.html>.
 This is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law."""
 
 def pyvipe():
     """Run pyvipe program."""
@@ -85,15 +85,15 @@
                 print(f'{editor} exited nonzero, aborting', file=sys.stderr)
                 sys.exit(1)
 
             try:
                 # if option is true, then read CRLF PIPE and return \n stdout.
                 newline = None if parsed_arg.universal_newline else ""
                 with open(temporary_file.name, 'r', newline=newline) as edited_pipe:
-                    byte_edited_pipe = edited_pipe.read().encode('ascii')
+                    byte_edited_pipe = bytes(edited_pipe.read(), 'utf-8')
                     os.write(out, byte_edited_pipe)
 
             except PermissionError:
                 print('cannot read tempfile', file=sys.stderr)
                 sys.exit(1)
 
     except PermissionError:
```

### Comparing `pyvipe-0.2.0/pyvipe.egg-info/PKG-INFO` & `pyvipe-0.2.1/pyvipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.2.0
+Version: 0.2.1
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
@@ -413,21 +413,22 @@
 
 ### Editor exited nonzero, aborting.
 
 In general, editor can exit with nonzero when you execute some command for various purposes. e.g preventing git rebase.
 But if you didn't execute the command but the editor exited with nonzero, it may be because
 of wrong user configuration for the editor.
 
-For vi, you can debug it with `EDITOR='vi -u NONE vipe'`
+For vi, you can debug it with `EDITOR='vi -u NONE' vipe`
 
 ## Changelog
 
 | Version | Note                     | 
 |:--------|:-------------------------|
-| HEAD    | add universal-newline option. support editor variable with option. | 
+| HEAD    | fix UnicodeEncodeError. | 
+| 0.2.0    | add universal-newline option. support editor variable with option. | 
 | 0.1.3    | fix shell completion. | 
 | 0.1.2    | add suffix option. fix error. | 
 | 0.1.1   | init                     | 
 
 ## CONTRIBUTION
 
 If it doesn't work as original [vipe](http://joeyh.name/code/moreutils/), then it's a bug.
```

### Comparing `pyvipe-0.2.0/setup.py` & `pyvipe-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name = 'pyvipe',
-    version = '0.2.0',
+    version = '0.2.1',
     description='edit pipe with your editor.',
     author='Constantin Hong',
     author_email='hongconstantin@gmail.com',
     url='https://github.com/Constantin1489/pyvipe',
     maintainer='Constantin Hong',
     maintainer_email='hongconstantin@gmail.com',
     readme = "README.md",
```

