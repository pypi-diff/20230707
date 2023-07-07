# Comparing `tmp/texplain-0.8.1.tar.gz` & `tmp/texplain-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplain-0.8.1.tar", last modified: Tue May 16 13:24:05 2023, max compression
+gzip compressed data, was "texplain-0.8.2.tar", last modified: Fri Jul  7 10:06:36 2023, max compression
```

## Comparing `texplain-0.8.1.tar` & `texplain-0.8.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.617575 texplain-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-16 13:23:56.000000 texplain-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-16 13:23:56.000000 texplain-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-16 13:23:56.000000 texplain-0.8.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 13:23:56.000000 texplain-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 13:23:56.000000 texplain-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-16 13:24:05.617575 texplain-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-16 13:23:56.000000 texplain-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/pre-commit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 13:23:56.000000 texplain-0.8.1/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 13:23:56.000000 texplain-0.8.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 13:23:56.000000 texplain-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:24:05.617575 texplain-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/input1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/example.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/input1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/figures/Diverging.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/figures/Sequential.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/unsrtnat.bst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/output1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/figure_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/figure_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/library.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/unsrtnat.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_find_command.py
--rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_texindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_texplain_example1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/texplain/
--rw-r--r--   0 runner    (1001) docker     (123)    87198 2023-05-16 13:23:56.000000 texplain-0.8.1/texplain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.617575 texplain-0.8.1/texplain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.846135 texplain-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.834135 texplain-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.834135 texplain-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 10:06:24.000000 texplain-0.8.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 10:06:24.000000 texplain-0.8.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-07 10:06:24.000000 texplain-0.8.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-07 10:06:24.000000 texplain-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-07 10:06:24.000000 texplain-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-07 10:06:24.000000 texplain-0.8.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 10:06:24.000000 texplain-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 10:06:24.000000 texplain-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-07 10:06:36.846135 texplain-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-07 10:06:24.000000 texplain-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.838135 texplain-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/pre-commit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-07 10:06:24.000000 texplain-0.8.2/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 10:06:24.000000 texplain-0.8.2/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 10:06:24.000000 texplain-0.8.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-07 10:06:24.000000 texplain-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:06:36.846135 texplain-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.838135 texplain-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.842136 texplain-0.8.2/tests/input1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/example.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.842136 texplain-0.8.2/tests/input1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/figures/Diverging.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/figures/Sequential.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/input1/unsrtnat.bst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.842136 texplain-0.8.2/tests/output1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/figure_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/figure_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/library.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/output1/unsrtnat.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_find_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_indent_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_indent_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_indent_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_indent_texindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 10:06:24.000000 texplain-0.8.2/tests/test_texplain_example1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.842136 texplain-0.8.2/texplain/
+-rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-07-07 10:06:24.000000 texplain-0.8.2/texplain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:06:36.846135 texplain-0.8.2/texplain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 10:06:36.000000 texplain-0.8.2/texplain.egg-info/top_level.txt
```

### Comparing `texplain-0.8.1/.github/workflows/ci.yml` & `texplain-0.8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/.github/workflows/pythonpublish.yml` & `texplain-0.8.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/.gitignore` & `texplain-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/.pre-commit-config.yaml` & `texplain-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/LICENSE` & `texplain-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/PKG-INFO` & `texplain-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.1
+Version: 0.8.2
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.1/README.md` & `texplain-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/docs/Makefile` & `texplain-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/docs/make.bat` & `texplain-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/docs/module.rst` & `texplain-0.8.2/docs/module.rst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/pyproject.toml` & `texplain-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/apalike.bst` & `texplain-0.8.2/tests/input1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/example.tex` & `texplain-0.8.2/tests/input1/example.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/figures/Diverging.pdf` & `texplain-0.8.2/tests/input1/figures/Diverging.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/figures/Sequential.pdf` & `texplain-0.8.2/tests/input1/figures/Sequential.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/goose-article.cls` & `texplain-0.8.2/tests/input1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/refs.bib` & `texplain-0.8.2/tests/input1/refs.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/input1/unsrtnat.bst` & `texplain-0.8.2/tests/input1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/apalike.bst` & `texplain-0.8.2/tests/output1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/figure_1.pdf` & `texplain-0.8.2/tests/output1/figure_1.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/figure_2.pdf` & `texplain-0.8.2/tests/output1/figure_2.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/goose-article.cls` & `texplain-0.8.2/tests/output1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/library.bib` & `texplain-0.8.2/tests/output1/library.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/main.tex` & `texplain-0.8.2/tests/output1/main.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/output1/unsrtnat.bst` & `texplain-0.8.2/tests/output1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_align.py` & `texplain-0.8.2/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_classify.py` & `texplain-0.8.2/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_find_command.py` & `texplain-0.8.2/tests/test_find_command.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_indent_long.py` & `texplain-0.8.2/tests/test_indent_long.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_indent_options.py` & `texplain-0.8.2/tests/test_indent_options.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_indent_simple.py` & `texplain-0.8.2/tests/test_indent_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_indent_texindent.py` & `texplain-0.8.2/tests/test_indent_texindent.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_placeholders.py` & `texplain-0.8.2/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/tests/test_simple.py` & `texplain-0.8.2/tests/test_simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -447,10 +447,38 @@
         source = r"Foo \TG{bar.}%\TG{Foo bar.}"
         expect = r"Foo bar.%\TG{Foo bar.}"
 
         tex = texplain.TeX(text=source)
         tex.replace_command(r"{\TG}[1]", "#1", ignore_commented=True)
         self.assertEqual(expect.strip(), str(tex).strip())
 
+    def test_fix_quote(self):
+        test = []
+        test.append(['This is text "with quotes".', "This is text ``with quotes''."])
+        test.append(
+            [
+                'This is text "with quotes" but not matching".',
+                'This is text "with quotes" but not matching".',
+            ]
+        )
+        test.append(["This is text 'with quotes'.", "This is text `with quotes'."])
+        test.append(
+            [
+                "This is text 'with quotes' but not matching'.",
+                "This is text 'with quotes' but not matching'.",
+            ]
+        )
+        test.append(
+            [
+                'A "slipping load" is confusing, we replaced it with "frictional strength".',
+                "A ``slipping load'' is confusing, we replaced it with ``frictional strength''.",
+            ]
+        )
+
+        for source, expect in test:
+            tex = texplain.TeX(text=source)
+            tex.fix_quotes().fix_quotes()
+            self.assertEqual(expect.strip(), str(tex).strip())
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `texplain-0.8.1/tests/test_texplain_example1.py` & `texplain-0.8.2/tests/test_texplain_example1.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.1/texplain/__init__.py` & `texplain-0.8.2/texplain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2504,14 +2504,51 @@
                 r"(" + key + r"~?\s?\[\\ref)(\*?{)([^}]*})(\])",
                 r"\\cref\2\3",
                 self.main,
                 re.MULTILINE,
                 re.IGNORECASE,
             )
 
+    def fix_quotes(self):
+        r"""
+        Replace:
+
+        *   ``"..."`` by ``\`\`...''``.
+        *   ``'...'`` by ``\`...'``.
+        """
+        lines = self.main.splitlines()
+
+        for replace, (opening, closing) in zip(['"', "'"], [("``", "''"), ("`", "'")]):
+            pattern = rf"(.*)({re.escape(replace)})(.*)({re.escape(replace)})(.*)"
+            for i in range(len(lines)):
+                if re.match(pattern, lines[i]):
+                    try:
+                        match = np.sort(
+                            find_matching(lines[i], replace, replace, return_array=True)[:, 0]
+                        )
+                    except IndexError:
+                        continue
+                    if len(match) % 2 != 0:
+                        continue
+                    match = match.reshape(-1, 2)
+                    match = match[np.diff(match, axis=1).ravel() > 1]
+                    if match.size == 0:
+                        continue
+                    match = np.vstack((match, [-1, -1]))
+                    ret = lines[i][: match[0, 0]]
+                    for j in range(match.shape[0] - 1):
+                        a = match[j, 0]
+                        b = match[j, 1]
+                        c = match[j + 1, 0]
+                        ret += opening + lines[i][a + 1 : b] + closing + lines[i][b + 1 : c]
+                    lines[i] = ret + lines[i][-1]
+
+        self.main = "\n".join(lines)
+        return self
+
 
 def bib_select(text: str, keys: list[str]) -> str:
     r"""
     Limit a BibTeX file to a list of keys.
 
     :param test: The BibTeX file as string.
     :param keys: The list of keys to select.
@@ -2628,14 +2665,21 @@
     parser.add_argument(
         "-s",
         "--use-cleveref",
         action="store_true",
         help=r'Change "Fig.~\ref{...}" etc. to "\\cref{...}".',
     )
 
+    parser.add_argument(
+        "-a",
+        "--fix-quotes",
+        action="store_true",
+        help="Fix non-LaTeX quotation marks: \"...\" -> ``...''",
+    )
+
     parser.add_argument("-v", "--version", action="version", version=version)
     parser.add_argument("files", nargs="+", type=str, help="TeX file(s) (changed in-place).")
 
     return parser
 
 
 def texcleanup(args: list[str]):
@@ -2672,14 +2716,17 @@
 
         if args.prepend_format_labels:
             tex.format_labels(args.prepend_format_labels)
 
         if args.use_cleveref:
             tex.use_cleveref()
 
+        if args.fix_quotes:
+            tex.fix_quotes()
+
         if tex.changed():
             with open(file, "w") as file:
                 file.write(str(tex))
 
 
 def _texcleanup_cli():
     texcleanup(sys.argv[1:])
```

### Comparing `texplain-0.8.1/texplain.egg-info/PKG-INFO` & `texplain-0.8.2/texplain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.1
+Version: 0.8.2
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.1/texplain.egg-info/SOURCES.txt` & `texplain-0.8.2/texplain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

