# Comparing `tmp/py_book_util-0.1.8.tar.gz` & `tmp/py_book_util-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_book_util-0.1.8.tar", max compression
+gzip compressed data, was "py_book_util-0.1.9.tar", max compression
```

## Comparing `py_book_util-0.1.8.tar` & `py_book_util-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2022-10-12 08:33:50.856206 py_book_util-0.1.8/py_book_util/__init__.py
--rw-r--r--   0        0        0      132 2022-10-12 09:00:19.644224 py_book_util-0.1.8/py_book_util/__main__.py
--rw-r--r--   0        0        0     4796 2022-10-25 07:14:25.591594 py_book_util-0.1.8/py_book_util/util.py
--rw-r--r--   0        0        0      449 2022-10-25 07:16:21.124622 py_book_util-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-12 08:33:50.856206 py_book_util-0.1.8/README.md
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 py_book_util-0.1.8/setup.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 py_book_util-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-12 08:33:50.856206 py_book_util-0.1.9/py_book_util/__init__.py
+-rw-r--r--   0        0        0      132 2022-10-12 09:00:19.644224 py_book_util-0.1.9/py_book_util/__main__.py
+-rw-r--r--   0        0        0     4912 2022-10-28 03:24:25.903252 py_book_util-0.1.9/py_book_util/util.py
+-rw-r--r--   0        0        0      469 2022-10-28 05:40:28.963225 py_book_util-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-12 08:33:50.856206 py_book_util-0.1.9/README.md
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 py_book_util-0.1.9/setup.py
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 py_book_util-0.1.9/PKG-INFO
```

### Comparing `py_book_util-0.1.8/py_book_util/util.py` & `py_book_util-0.1.9/py_book_util/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,7 +139,11 @@
                 pass
             else:
                 print(line, end='')
 
 def read_text_file(file_path):
     from pathlib import Path
     return Path(file_path).read_text()
+
+def display_text(content):
+    from IPython.display import Code
+    return Code(data=content, language="text")
```

