# Comparing `tmp/pyxargs-2.1.1.tar.gz` & `tmp/pyxargs-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxargs-2.1.1.tar", last modified: Tue Feb 21 07:08:26 2023, max compression
+gzip compressed data, was "pyxargs-2.2.0.tar", last modified: Fri Jul  7 21:51:02 2023, max compression
```

## Comparing `pyxargs-2.1.1.tar` & `pyxargs-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:08:26.220157 pyxargs-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-21 07:08:12.000000 pyxargs-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-02-21 07:08:26.220157 pyxargs-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-02-21 07:08:12.000000 pyxargs-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:08:26.220157 pyxargs-2.1.1/pyxargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-02-21 07:08:26.000000 pyxargs-2.1.1/pyxargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-21 07:08:26.000000 pyxargs-2.1.1/pyxargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 07:08:26.000000 pyxargs-2.1.1/pyxargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-21 07:08:26.000000 pyxargs-2.1.1/pyxargs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 07:08:26.000000 pyxargs-2.1.1/pyxargs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-02-21 07:08:12.000000 pyxargs-2.1.1/pyxargs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 07:08:26.220157 pyxargs-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-21 07:08:12.000000 pyxargs-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:51:02.823599 pyxargs-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 21:50:53.000000 pyxargs-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-07 21:51:02.819599 pyxargs-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-07 21:50:53.000000 pyxargs-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:51:02.819599 pyxargs-2.2.0/pyxargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-07 21:50:53.000000 pyxargs-2.2.0/pyxargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:51:02.823599 pyxargs-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 21:50:53.000000 pyxargs-2.2.0/setup.py
```

### Comparing `pyxargs-2.1.1/LICENSE` & `pyxargs-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxargs-2.1.1/PKG-INFO` & `pyxargs-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.1.1
+Version: 2.2.0
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
@@ -35,17 +35,17 @@
 Build and execute command lines or python code from standard input or file
 paths, a partial and opinionated implementation of xargs in python with some
 added features. The file input mode (default if stdin is not connected) builds
 commands using filenames only and executes them in their respective
 directories, this is useful when dealing with file paths containing multiple
 character encodings.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --examples            print example usage
+  --examples            show example usage and exit
   --version             show program's version number and exit
   -m input-mode         options are:
                         file    = build commands from filenames and execute in
                                   each subdirectory respectively
                         path    = build commands from file paths relative to
                                   the current directory and execute in the
                                   current directory
@@ -89,39 +89,50 @@
   --post "code"         runs exec(code) after execution
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
-```
-by default, pyxargs will use filenames and run commands in each directory
-    pyxargs echo
-instead of appending inputs, you can specify a location with {}
-    pyxargs echo spam {} spam
-and like xargs, you can also specify the replace-str with -I
-    pyxargs -I eggs echo spam eggs spam literal {}
-if stdin is connected, it will be used instead of filenames by default
-    echo bacon eggs | pyxargs echo spam
-python code can be used in place of a command
-    pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
-python code can also run before or after all the commands
-    pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
-regular expressions can be used to filter and modify inputs
-    pyxargs -r \.py --resub \.py .txt {} echo {}
-the original inputs can easily be used with the substituted versions
-    pyxargs -r \.py --resub \.py .txt new echo {} new
-
-comparing usage with find & xargs (these commands produce the same output)
-    find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
-    find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
-pyxargs does not require '-I' to specify a replace-str (default: {})
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
-and in the absence of a replace-str, exactly one input is appended
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
-pyxargs can use file paths as input without piping from another program
-    pyxargs -m path echo ./{}
-and now for something completely different, python code for the command
-    pyxargs -m path --py "print('./{}')"
+```bash
+# by default, pyxargs will use filenames and run commands in each directory
+  > pyxargs echo
+
+# instead of appending inputs, you can specify a location with {}
+  > pyxargs echo spam {} spam
+
+# and like xargs, you can also specify the replace-str with -I
+  > pyxargs -I eggs echo spam eggs spam literal {}
+
+# if stdin is connected, it will be used instead of filenames by default
+  > echo bacon eggs | pyxargs echo spam
+
+# python code can be used in place of a command
+  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+
+# python code can also run before or after all the commands
+  > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
+
+# regular expressions can be used to filter and modify inputs
+  > pyxargs -r \.py --resub \.py .txt {} echo {}
+
+# the original inputs can easily be used with the substituted versions
+  > pyxargs -r \.py --resub \.py .txt new echo {} new
+
+# this and the following examples will compare usage with find & xargs
+  > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
+  > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
+
+# pyxargs does not require '-I' to specify a replace-str (default: {})
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
+
+# and in the absence of a replace-str, exactly one input is appended
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
+
+# pyxargs can use file paths as input without piping from another program
+  > pyxargs -m path echo ./{}
+
+# and now for something completely different, python code for the command
+  > pyxargs -m path --py "print('./{}')"
 ```
```

### Comparing `pyxargs-2.1.1/README.md` & `pyxargs-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 Build and execute command lines or python code from standard input or file
 paths, a partial and opinionated implementation of xargs in python with some
 added features. The file input mode (default if stdin is not connected) builds
 commands using filenames only and executes them in their respective
 directories, this is useful when dealing with file paths containing multiple
 character encodings.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --examples            print example usage
+  --examples            show example usage and exit
   --version             show program's version number and exit
   -m input-mode         options are:
                         file    = build commands from filenames and execute in
                                   each subdirectory respectively
                         path    = build commands from file paths relative to
                                   the current directory and execute in the
                                   current directory
@@ -67,39 +67,50 @@
   --post "code"         runs exec(code) after execution
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
-```
-by default, pyxargs will use filenames and run commands in each directory
-    pyxargs echo
-instead of appending inputs, you can specify a location with {}
-    pyxargs echo spam {} spam
-and like xargs, you can also specify the replace-str with -I
-    pyxargs -I eggs echo spam eggs spam literal {}
-if stdin is connected, it will be used instead of filenames by default
-    echo bacon eggs | pyxargs echo spam
-python code can be used in place of a command
-    pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
-python code can also run before or after all the commands
-    pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
-regular expressions can be used to filter and modify inputs
-    pyxargs -r \.py --resub \.py .txt {} echo {}
-the original inputs can easily be used with the substituted versions
-    pyxargs -r \.py --resub \.py .txt new echo {} new
-
-comparing usage with find & xargs (these commands produce the same output)
-    find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
-    find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
-pyxargs does not require '-I' to specify a replace-str (default: {})
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
-and in the absence of a replace-str, exactly one input is appended
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
-pyxargs can use file paths as input without piping from another program
-    pyxargs -m path echo ./{}
-and now for something completely different, python code for the command
-    pyxargs -m path --py "print('./{}')"
+```bash
+# by default, pyxargs will use filenames and run commands in each directory
+  > pyxargs echo
+
+# instead of appending inputs, you can specify a location with {}
+  > pyxargs echo spam {} spam
+
+# and like xargs, you can also specify the replace-str with -I
+  > pyxargs -I eggs echo spam eggs spam literal {}
+
+# if stdin is connected, it will be used instead of filenames by default
+  > echo bacon eggs | pyxargs echo spam
+
+# python code can be used in place of a command
+  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+
+# python code can also run before or after all the commands
+  > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
+
+# regular expressions can be used to filter and modify inputs
+  > pyxargs -r \.py --resub \.py .txt {} echo {}
+
+# the original inputs can easily be used with the substituted versions
+  > pyxargs -r \.py --resub \.py .txt new echo {} new
+
+# this and the following examples will compare usage with find & xargs
+  > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
+  > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
+
+# pyxargs does not require '-I' to specify a replace-str (default: {})
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
+
+# and in the absence of a replace-str, exactly one input is appended
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
+
+# pyxargs can use file paths as input without piping from another program
+  > pyxargs -m path echo ./{}
+
+# and now for something completely different, python code for the command
+  > pyxargs -m path --py "print('./{}')"
 ```
```

### Comparing `pyxargs-2.1.1/pyxargs.egg-info/PKG-INFO` & `pyxargs-2.2.0/pyxargs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.1.1
+Version: 2.2.0
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
@@ -35,17 +35,17 @@
 Build and execute command lines or python code from standard input or file
 paths, a partial and opinionated implementation of xargs in python with some
 added features. The file input mode (default if stdin is not connected) builds
 commands using filenames only and executes them in their respective
 directories, this is useful when dealing with file paths containing multiple
 character encodings.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --examples            print example usage
+  --examples            show example usage and exit
   --version             show program's version number and exit
   -m input-mode         options are:
                         file    = build commands from filenames and execute in
                                   each subdirectory respectively
                         path    = build commands from file paths relative to
                                   the current directory and execute in the
                                   current directory
@@ -89,39 +89,50 @@
   --post "code"         runs exec(code) after execution
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
-```
-by default, pyxargs will use filenames and run commands in each directory
-    pyxargs echo
-instead of appending inputs, you can specify a location with {}
-    pyxargs echo spam {} spam
-and like xargs, you can also specify the replace-str with -I
-    pyxargs -I eggs echo spam eggs spam literal {}
-if stdin is connected, it will be used instead of filenames by default
-    echo bacon eggs | pyxargs echo spam
-python code can be used in place of a command
-    pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
-python code can also run before or after all the commands
-    pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
-regular expressions can be used to filter and modify inputs
-    pyxargs -r \.py --resub \.py .txt {} echo {}
-the original inputs can easily be used with the substituted versions
-    pyxargs -r \.py --resub \.py .txt new echo {} new
-
-comparing usage with find & xargs (these commands produce the same output)
-    find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
-    find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
-pyxargs does not require '-I' to specify a replace-str (default: {})
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
-and in the absence of a replace-str, exactly one input is appended
-    find ./ -name "*" -type f -print0 | pyxargs -0 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
-    find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
-pyxargs can use file paths as input without piping from another program
-    pyxargs -m path echo ./{}
-and now for something completely different, python code for the command
-    pyxargs -m path --py "print('./{}')"
+```bash
+# by default, pyxargs will use filenames and run commands in each directory
+  > pyxargs echo
+
+# instead of appending inputs, you can specify a location with {}
+  > pyxargs echo spam {} spam
+
+# and like xargs, you can also specify the replace-str with -I
+  > pyxargs -I eggs echo spam eggs spam literal {}
+
+# if stdin is connected, it will be used instead of filenames by default
+  > echo bacon eggs | pyxargs echo spam
+
+# python code can be used in place of a command
+  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+
+# python code can also run before or after all the commands
+  > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
+
+# regular expressions can be used to filter and modify inputs
+  > pyxargs -r \.py --resub \.py .txt {} echo {}
+
+# the original inputs can easily be used with the substituted versions
+  > pyxargs -r \.py --resub \.py .txt new echo {} new
+
+# this and the following examples will compare usage with find & xargs
+  > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
+  > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
+
+# pyxargs does not require '-I' to specify a replace-str (default: {})
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
+
+# and in the absence of a replace-str, exactly one input is appended
+  > find ./ -name "*" -type f -print0 | pyxargs -0 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
+  > find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
+
+# pyxargs can use file paths as input without piping from another program
+  > pyxargs -m path echo ./{}
+
+# and now for something completely different, python code for the command
+  > pyxargs -m path --py "print('./{}')"
 ```
```

### Comparing `pyxargs-2.1.1/pyxargs.py` & `pyxargs-2.2.0/pyxargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import signal
 import subprocess
 import sys
 import textwrap
 import typing
 
 
-__version__: typing.Final[str] = "2.1.1"
+__version__: typing.Final[str] = "2.2.0"
 
 
 def replace_surrogates(string: str) -> str:
     return string.encode('utf16', 'surrogatepass').decode('utf16', 'replace')
 
 
 def colour_print(string: str, colour: str) -> None:
@@ -204,55 +204,66 @@
                 return text.splitlines()[1:]
             return argparse.HelpFormatter._split_lines(self, text, width)
     readme = ("Build and execute command lines or python code from standard input or file paths, "
               "a partial and opinionated implementation of xargs in python with some added features. "
               "The file input mode (default if stdin is not connected) builds commands using filenames only and executes them in their respective directories, "
               "this is useful when dealing with file paths containing multiple character encodings.")
     examples = textwrap.dedent(r"""
-    by default, pyxargs will use filenames and run commands in each directory
-        pyxargs echo
-    instead of appending inputs, you can specify a location with {}
-        pyxargs echo spam {} spam
-    and like xargs, you can also specify the replace-str with -I
-        pyxargs -I eggs echo spam eggs spam literal {}
-    if stdin is connected, it will be used instead of filenames by default
-        echo bacon eggs | pyxargs echo spam
-    python code can be used in place of a command
-        pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
-    python code can also run before or after all the commands
-        pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
-    regular expressions can be used to filter and modify inputs
-        pyxargs -r \.py --resub \.py .txt {} echo {}
-    the original inputs can easily be used with the substituted versions
-        pyxargs -r \.py --resub \.py .txt new echo {} new
-
-    comparing usage with find & xargs (these commands produce the same output)
-        find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
-        find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
-    pyxargs does not require '-I' to specify a replace-str (default: {})
-        find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
-    and in the absence of a replace-str, exactly one input is appended
-        find ./ -name "*" -type f -print0 | pyxargs -0 echo
-        find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
-        find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
-    pyxargs can use file paths as input without piping from another program
-        pyxargs -m path echo ./{}
-    and now for something completely different, python code for the command
-        pyxargs -m path --py "print('./{}')"
+    # by default, pyxargs will use filenames and run commands in each directory
+      > pyxargs echo
+
+    # instead of appending inputs, you can specify a location with {}
+      > pyxargs echo spam {} spam
+
+    # and like xargs, you can also specify the replace-str with -I
+      > pyxargs -I eggs echo spam eggs spam literal {}
+
+    # if stdin is connected, it will be used instead of filenames by default
+      > echo bacon eggs | pyxargs echo spam
+
+    # python code can be used in place of a command
+      > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+
+    # python code can also run before or after all the commands
+      > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
+
+    # regular expressions can be used to filter and modify inputs
+      > pyxargs -r \.py --resub \.py .txt {} echo {}
+
+    # the original inputs can easily be used with the substituted versions
+      > pyxargs -r \.py --resub \.py .txt new echo {} new
+
+    # this and the following examples will compare usage with find & xargs
+      > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
+      > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
+
+    # pyxargs does not require '-I' to specify a replace-str (default: {})
+      > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
+
+    # and in the absence of a replace-str, exactly one input is appended
+      > find ./ -name "*" -type f -print0 | pyxargs -0 echo
+      > find ./ -name "*" -type f -print0 | xargs -0 --max-args=1 echo
+      > find ./ -name "*" -type f -print0 | xargs -0 --max-lines=1 echo
+
+    # pyxargs can use file paths as input without piping from another program
+      > pyxargs -m path echo ./{}
+
+    # and now for something completely different, python code for the command
+      > pyxargs -m path --py "print('./{}')"
     """)
     parser = argparse.ArgumentParser(description=readme,
                                      formatter_class=lambda prog: ArgparseCustomFormatter(prog, max_help_position=24),
                                      usage="%(prog)s [options] command [initial-arguments ...]\n"
                                            "       %(prog)s -h | --help | --examples | --version")
     group0 = parser.add_mutually_exclusive_group()
     group1 = parser.add_mutually_exclusive_group()
     parser.add_argument("command", action="store", type=str, nargs=argparse.REMAINDER,
                         help=argparse.SUPPRESS)
     parser.add_argument("--examples", action="store_true", dest="examples",
-                        help="print example usage")
+                        help="show example usage and exit")
     parser.add_argument("--version", action="version", version=__version__)
     parser.add_argument("--base-directory", type=str, default=os.getcwd(), metavar="base-directory", dest="base_dir",
                         help=argparse.SUPPRESS)
     parser.add_argument("-m", type=str, default=None, metavar="input-mode", choices=['file', 'path', 'abspath', 'stdin', "f", "p", "a", "s"], dest="input_mode",
                         help="F!\n"
                              "options are:\n"
                              "file    = build commands from filenames and execute in\n"
@@ -320,24 +331,26 @@
         if not sys.stdin.isatty():
             stdin = sys.stdin.read()
             args.input_mode = "stdin"
         else:
             args.input_mode = "file"
     elif args.input_mode == "stdin":
         stdin = sys.stdin.read()
+    # need to open new tty for interactive mode if input was read from stdin
+    if args.interactive and stdin:
+        sys.stdin = open("/dev/tty")
     # set delimiter
     if args.null:
         args.delim = "\0"
     # enable shell on windows
     if sys.platform.startswith("win32"):
         args.subprocess_shell = True
     # check for invalid arguments
     assert os.path.isdir(args.base_dir) and os.getcwd() == args.base_dir
     if args.input_mode == "stdin":
-        assert not args.interactive, "invalid option --interactive for input mode: stdin"
         assert not args.folders, "invalid option --folders for input mode: stdin"
         assert not args.top_level, "invalid option --top for input mode: stdin"
         assert not args.symlinks, "invalid option --symlinks for input mode: stdin"
         assert not args.regex_basename, "invalid option -b for input mode: stdin"
     else:
         assert not args.null, f"invalid option --null for input mode: {args.input_mode}"
         assert not args.delim, f"invalid option --delimiter for input mode: {args.input_mode}"
```

### Comparing `pyxargs-2.1.1/setup.py` & `pyxargs-2.2.0/setup.py`

 * *Files identical despite different names*

