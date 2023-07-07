# Comparing `tmp/task2a-1.0.1.tar.gz` & `tmp/task2a-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.1.tar", max compression
+gzip compressed data, was "task2a-1.0.2.tar", max compression
```

## Comparing `task2a-1.0.1.tar` & `task2a-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      318 2023-07-06 22:19:40.173023 task2a-1.0.1/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-06 22:19:40.173023 task2a-1.0.1/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-07 01:46:40.263858 task2a-1.0.1/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-06 22:19:40.174021 task2a-1.0.1/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-06 22:19:40.174021 task2a-1.0.1/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-06 22:19:40.174021 task2a-1.0.1/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8361 2023-07-06 22:19:40.175016 task2a-1.0.1/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 01:33:29.604917 task2a-1.0.1/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 01:33:29.604917 task2a-1.0.1/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 01:33:29.604917 task2a-1.0.1/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 01:33:29.605916 task2a-1.0.1/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    19900 2023-07-07 01:33:29.605916 task2a-1.0.1/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      447 2023-07-07 01:46:40.258853 task2a-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    35592 2023-07-07 01:45:50.481449 task2a-1.0.1/README.md
--rw-r--r--   0        0        0    35342 1970-01-01 00:00:00.000000 task2a-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      318 2023-07-06 22:19:40.173023 task2a-1.0.2/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-06 22:19:40.173023 task2a-1.0.2/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-07 02:46:06.969859 task2a-1.0.2/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8361 2023-07-06 22:19:40.175016 task2a-1.0.2/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-07 01:33:29.605916 task2a-1.0.2/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    19900 2023-07-07 01:33:29.605916 task2a-1.0.2/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      447 2023-07-07 02:45:55.874863 task2a-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    35645 2023-07-07 02:45:47.386179 task2a-1.0.2/README.md
+-rw-r--r--   0        0        0    35395 1970-01-01 00:00:00.000000 task2a-1.0.2/PKG-INFO
```

### Comparing `task2a-1.0.1/pwgen/cli/cli.py` & `task2a-1.0.2/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.1/pwgen/pwgen.py` & `task2a-1.0.2/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.1/pwgen/showcase/showcase.py` & `task2a-1.0.2/pwgen/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.1/README.md` & `task2a-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -618,15 +618,15 @@
 #### Showcase
 
 To showcase the behavior of the pwgen library, an interactive command called "pwgen_showcase" has been created.
 This command utilizes both the pwgen CLI and the pwgen library. It's an interactive command you can invoke via `pwgen_showcase` or `python -m pwgen.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `pwgen_showcase --all` to activate this feature.
 
-
+![showcase_demo.gif](assets/images/showcase_demo.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
 reproduced or disclosed to any third party or to any other person, other than those persons who have a bona fide need to review it
 for the purpose of participation in the online courses being provided by EPAM.
 The intellectual property rights in all materials (including any trademarks) are owned by EPAM Systems Inc or its associated companies,
```

#### html2text {}

```diff
@@ -386,19 +386,20 @@
 input to the sort command. The sort command will sort passwords in reverse
 order and print them out. The -n flag will be ignored. | #### Showcase To
 showcase the behavior of the pwgen library, an interactive command called
 "pwgen_showcase" has been created. This command utilizes both the pwgen CLI and
 the pwgen library. It's an interactive command you can invoke via
 `pwgen_showcase` or `python -m pwgen.showcase`. It has an optional flag that
 allows you to view all use cases at once without any interaction. You can use
-the command `pwgen_showcase --all` to activate this feature. ## General
-provisions All materials provided and/or made available contain EPAMâs
-proprietary and confidential information and must not to be copied, reproduced
-or disclosed to any third party or to any other person, other than those
-persons who have a bona fide need to review it for the purpose of participation
-in the online courses being provided by EPAM. The intellectual property rights
-in all materials (including any trademarks) are owned by EPAM Systems Inc or
-its associated companies, and a limited license, terminable at the discretion
-of EPAM without notice, is hereby granted to you solely for the purpose of
+the command `pwgen_showcase --all` to activate this feature. !
+[showcase_demo.gif](assets/images/showcase_demo.gif) ## General provisions All
+materials provided and/or made available contain EPAMâs proprietary and
+confidential information and must not to be copied, reproduced or disclosed to
+any third party or to any other person, other than those persons who have a
+bona fide need to review it for the purpose of participation in the online
+courses being provided by EPAM. The intellectual property rights in all
+materials (including any trademarks) are owned by EPAM Systems Inc or its
+associated companies, and a limited license, terminable at the discretion of
+EPAM without notice, is hereby granted to you solely for the purpose of
 participating in the online courses being provided by EPAM. Neither you nor any
 other party shall acquire any intellectual property rights of any kind in such
 materials.
```

### Comparing `task2a-1.0.1/PKG-INFO` & `task2a-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -631,15 +631,15 @@
 #### Showcase
 
 To showcase the behavior of the pwgen library, an interactive command called "pwgen_showcase" has been created.
 This command utilizes both the pwgen CLI and the pwgen library. It's an interactive command you can invoke via `pwgen_showcase` or `python -m pwgen.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `pwgen_showcase --all` to activate this feature.
 
-
+![showcase_demo.gif](assets/images/showcase_demo.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
 reproduced or disclosed to any third party or to any other person, other than those persons who have a bona fide need to review it
 for the purpose of participation in the online courses being provided by EPAM.
 The intellectual property rights in all materials (including any trademarks) are owned by EPAM Systems Inc or its associated companies,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.1 Summary: Author:
+Metadata-Version: 2.1 Name: task2a Version: 1.0.2 Summary: Author:
 Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0) Description-
 Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
@@ -392,19 +392,20 @@
 input to the sort command. The sort command will sort passwords in reverse
 order and print them out. The -n flag will be ignored. | #### Showcase To
 showcase the behavior of the pwgen library, an interactive command called
 "pwgen_showcase" has been created. This command utilizes both the pwgen CLI and
 the pwgen library. It's an interactive command you can invoke via
 `pwgen_showcase` or `python -m pwgen.showcase`. It has an optional flag that
 allows you to view all use cases at once without any interaction. You can use
-the command `pwgen_showcase --all` to activate this feature. ## General
-provisions All materials provided and/or made available contain EPAMâs
-proprietary and confidential information and must not to be copied, reproduced
-or disclosed to any third party or to any other person, other than those
-persons who have a bona fide need to review it for the purpose of participation
-in the online courses being provided by EPAM. The intellectual property rights
-in all materials (including any trademarks) are owned by EPAM Systems Inc or
-its associated companies, and a limited license, terminable at the discretion
-of EPAM without notice, is hereby granted to you solely for the purpose of
+the command `pwgen_showcase --all` to activate this feature. !
+[showcase_demo.gif](assets/images/showcase_demo.gif) ## General provisions All
+materials provided and/or made available contain EPAMâs proprietary and
+confidential information and must not to be copied, reproduced or disclosed to
+any third party or to any other person, other than those persons who have a
+bona fide need to review it for the purpose of participation in the online
+courses being provided by EPAM. The intellectual property rights in all
+materials (including any trademarks) are owned by EPAM Systems Inc or its
+associated companies, and a limited license, terminable at the discretion of
+EPAM without notice, is hereby granted to you solely for the purpose of
 participating in the online courses being provided by EPAM. Neither you nor any
 other party shall acquire any intellectual property rights of any kind in such
 materials.
```

