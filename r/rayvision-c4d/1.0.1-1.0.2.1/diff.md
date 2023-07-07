# Comparing `tmp/rayvision_c4d-1.0.1.tar.gz` & `tmp/rayvision_c4d-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_c4d-1.0.1.tar", last modified: Tue Aug  3 08:13:11 2021, max compression
+gzip compressed data, was "dist/rayvision_c4d-1.0.2.1.tar", last modified: Fri Jul  7 06:52:27 2023, max compression
```

## Comparing `rayvision_c4d-1.0.1.tar` & `rayvision_c4d-1.0.2.1.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      265 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      235 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      464 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       17 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/help/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/help/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3346 2021-08-02 09:23:38.000000 rayvision_c4d-1.0.1/help/examples/c4d_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2021-04-21 08:19:39.000000 rayvision_c4d-1.0.1/help/examples/only_analyze_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d/
--rw-rw-rw-   0 root         (0) root         (0)      467 2021-04-21 02:13:20.000000 rayvision_c4d-1.0.1/rayvision_c4d/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13623 2021-04-21 02:13:20.000000 rayvision_c4d-1.0.1/rayvision_c4d/analyze_c4d.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/rayvision_c4d/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5754 2021-04-21 02:13:20.000000 rayvision_c4d-1.0.1/rayvision_c4d/get_preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/rayvision_c4d/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2021-04-20 03:36:36.000000 rayvision_c4d-1.0.1/rayvision_c4d/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-04-20 10:02:40.000000 rayvision_c4d-1.0.1/rayvision_c4d/tests/test_analyse.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2021-04-20 03:14:34.000000 rayvision_c4d-1.0.1/rayvision_c4d/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d/tool/
--rw-rw-rw-   0 root         (0) root         (0)      781 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/rayvision_c4d/tool/RBAnalyzer.pyp
--rw-rw-rw-   0 root         (0) root         (0)     4639 2021-04-21 02:13:20.000000 rayvision_c4d-1.0.1/rayvision_c4d/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/
--rw-r--r--   0 root         (0) root         (0)      464 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1013 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/rayvision_c4d.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       43 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2021-08-03 08:13:11.000000 rayvision_c4d-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      999 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2021-04-20 03:01:05.000000 rayvision_c4d-1.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/help/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/help/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3346 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/help/examples/c4d_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/help/examples/only_analyze_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13623 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/analyze_c4d.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/get_preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tests/test_analyse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/RBAnalyzer.pyp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python26/
+-rw-rw-rw-   0 root         (0) root         (0)   572928 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python26/RBAnalyzer.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python27/
+-rw-rw-rw-   0 root         (0) root         (0)   569856 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python27/RBAnalyzer.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python27x/
+-rw-rw-rw-   0 root         (0) root         (0)   527360 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python27x/RBAnalyzer.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python310/
+-rw-rw-rw-   0 root         (0) root         (0)   503808 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python310/RBAnalyzer.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python37/
+-rw-rw-rw-   0 root         (0) root         (0)   546816 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python37/RBAnalyzer.pyd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python39/
+-rw-rw-rw-   0 root         (0) root         (0)   532480 2023-05-31 11:15:31.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/tool/python39/RBAnalyzer.pyd
+-rw-rw-rw-   0 root         (0) root         (0)     4639 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/rayvision_c4d/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-07 06:52:27.000000 rayvision_c4d-1.0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-05-31 11:12:03.000000 rayvision_c4d-1.0.2.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3045 2023-07-07 06:37:59.000000 rayvision_c4d-1.0.2.1/tox.ini
```

### Comparing `rayvision_c4d-1.0.1/.pre-commit-config.yaml` & `rayvision_c4d-1.0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/help/examples/c4d_demo.py` & `rayvision_c4d-1.0.2.1/help/examples/c4d_demo.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/analyze_c4d.py` & `rayvision_c4d-1.0.2.1/rayvision_c4d/analyze_c4d.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/get_preferences.py` & `rayvision_c4d-1.0.2.1/rayvision_c4d/get_preferences.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/tests/conftest.py` & `rayvision_c4d-1.0.2.1/rayvision_c4d/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/tests/test_utils.py` & `rayvision_c4d-1.0.2.1/rayvision_c4d/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/tool/RBAnalyzer.pyp` & `rayvision_c4d-1.0.2.1/rayvision_c4d/tool/RBAnalyzer.pyp`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding=utf-8 -*-
 # author: kanada
-
+# the python version is py26/27/27x and py37/py39
 import sys,os,c4d
 
-version = c4d.GetC4DVersion()
-
+version = int(c4d.GetC4DVersion())
+print("version: %s" % version)
 defaultencoding = 'utf-8'
 if sys.getdefaultencoding() != defaultencoding:
     reload(sys)
     sys.setdefaultencoding(defaultencoding)
 
 if version < 17000:
     sys.path.append(os.path.join(os.path.dirname(__file__), 'python26'))
 elif version < 20000:
     sys.path.append(os.path.join(os.path.dirname(__file__), 'python27x'))
 elif version < 23000:
     sys.path.append(os.path.join(os.path.dirname(__file__), 'python27'))
-else:
+elif version < 24000:
     sys.path.append(os.path.join(os.path.dirname(__file__), 'python37'))
+elif version < 2023200:
+    sys.path.append(os.path.join(os.path.dirname(__file__), 'python39'))
+else:
+    sys.path.append(os.path.join(os.path.dirname(__file__), 'python310'))
 
 
 def PluginMessage(id, data):
     if id==c4d.C4DPL_COMMANDLINEARGS:
         try:
             import RBAnalyzer
         finally:
```

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d/utils.py` & `rayvision_c4d-1.0.2.1/rayvision_c4d/utils.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/rayvision_c4d.egg-info/SOURCES.txt` & `rayvision_c4d-1.0.2.1/rayvision_c4d.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 ./rayvision_c4d/get_preferences.py
 ./rayvision_c4d/utils.py
 ./rayvision_c4d/tests/__init__.py
 ./rayvision_c4d/tests/conftest.py
 ./rayvision_c4d/tests/test_analyse.py
 ./rayvision_c4d/tests/test_utils.py
 ./rayvision_c4d/tool/RBAnalyzer.pyp
+./rayvision_c4d/tool/python26/RBAnalyzer.pyd
+./rayvision_c4d/tool/python27/RBAnalyzer.pyd
+./rayvision_c4d/tool/python27x/RBAnalyzer.pyd
+./rayvision_c4d/tool/python310/RBAnalyzer.pyd
+./rayvision_c4d/tool/python37/RBAnalyzer.pyd
+./rayvision_c4d/tool/python39/RBAnalyzer.pyd
 help/examples/c4d_demo.py
 help/examples/only_analyze_demo.py
 rayvision_c4d/__init__.py
 rayvision_c4d/analyze_c4d.py
 rayvision_c4d/constants.py
 rayvision_c4d/get_preferences.py
 rayvision_c4d/utils.py
@@ -30,8 +36,14 @@
 rayvision_c4d.egg-info/dependency_links.txt
 rayvision_c4d.egg-info/requires.txt
 rayvision_c4d.egg-info/top_level.txt
 rayvision_c4d/tests/__init__.py
 rayvision_c4d/tests/conftest.py
 rayvision_c4d/tests/test_analyse.py
 rayvision_c4d/tests/test_utils.py
-rayvision_c4d/tool/RBAnalyzer.pyp
+rayvision_c4d/tool/RBAnalyzer.pyp
+rayvision_c4d/tool/python26/RBAnalyzer.pyd
+rayvision_c4d/tool/python27/RBAnalyzer.pyd
+rayvision_c4d/tool/python27x/RBAnalyzer.pyd
+rayvision_c4d/tool/python310/RBAnalyzer.pyd
+rayvision_c4d/tool/python37/RBAnalyzer.pyd
+rayvision_c4d/tool/python39/RBAnalyzer.pyd
```

### Comparing `rayvision_c4d-1.0.1/setup.py` & `rayvision_c4d-1.0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_c4d-1.0.1/tox.ini` & `rayvision_c4d-1.0.2.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 commands =
   pytest --cov={env:CI_PROJECT_NAME} --cov-append {posargs}
 
 [testenv:deploy]
 deps =
     twine
 commands =
+    pip install requests==2.28.2
     python setup.py bdist_wheel register -r rayvision_pip upload -r rayvision_pip
     python setup.py sdist
     twine upload --repository pypi dist/*
 
 [testenv:pre-commit]
 skip_install = true
 deps =  pre-commit
```

