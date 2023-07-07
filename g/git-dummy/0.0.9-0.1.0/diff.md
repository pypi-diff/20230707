# Comparing `tmp/git-dummy-0.0.9.tar.gz` & `tmp/git-dummy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-dummy-0.0.9.tar", last modified: Wed Jul  5 01:56:23 2023, max compression
+gzip compressed data, was "git-dummy-0.1.0.tar", last modified: Fri Jul  7 14:42:59 2023, max compression
```

## Comparing `git-dummy-0.0.9.tar` & `git-dummy-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.680722 git-dummy-0.0.9/
--rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     5804 2023-07-05 01:56:23.680722 git-dummy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5092 2023-06-14 06:01:15.000000 git-dummy-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.671844 git-dummy-0.0.9/git_dummy/
--rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.0.9/git_dummy/__init__.py
--rw-rw-rw-   0        0        0     5146 2023-06-14 06:17:47.000000 git-dummy-0.0.9/git_dummy/__main__.py
--rw-rw-rw-   0        0        0      405 2023-07-05 01:19:31.000000 git-dummy-0.0.9/git_dummy/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:56:23.679507 git-dummy-0.0.9/git_dummy.egg-info/
--rw-rw-rw-   0        0        0     5804 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 01:56:23.000000 git-dummy-0.0.9/git_dummy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 01:56:23.680722 git-dummy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1223 2023-07-05 01:55:53.000000 git-dummy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:42:59.492655 git-dummy-0.1.0/
+-rw-rw-rw-   0        0        0    18431 2023-03-23 15:27:25.000000 git-dummy-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5845 2023-07-07 14:42:59.492655 git-dummy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5092 2023-06-14 06:01:15.000000 git-dummy-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 14:42:59.484424 git-dummy-0.1.0/git_dummy/
+-rw-rw-rw-   0        0        0        0 2023-03-23 15:27:25.000000 git-dummy-0.1.0/git_dummy/__init__.py
+-rw-rw-rw-   0        0        0     5159 2023-07-07 14:36:37.000000 git-dummy-0.1.0/git_dummy/__main__.py
+-rw-rw-rw-   0        0        0      405 2023-07-05 01:19:31.000000 git-dummy-0.1.0/git_dummy/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:42:59.492655 git-dummy-0.1.0/git_dummy.egg-info/
+-rw-rw-rw-   0        0        0     5845 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 14:42:59.000000 git-dummy-0.1.0/git_dummy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:42:59.492655 git-dummy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1223 2023-07-07 14:38:04.000000 git-dummy-0.1.0/setup.py
```

### Comparing `git-dummy-0.0.9/LICENSE` & `git-dummy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.9/PKG-INFO` & `git-dummy-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
+License: UNKNOWN
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -127,7 +129,9 @@
 Explicitly specifying options at the command-line takes precedence over the corresponding environment variable values.
 
 ## Learn More
 Learn more about this tool on the [git-dummy project page](https://initialcommit.com/tools/git-dummy).
 
 ## Authors
 **Jacob Stopak** - on behalf of [Initial Commit](https://initialcommit.com)
+
+
```

### Comparing `git-dummy-0.0.9/README.md` & `git-dummy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `git-dummy-0.0.9/git_dummy/__main__.py` & `git-dummy-0.1.0/git_dummy/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,18 +74,18 @@
             )
             sys.exit(1)
         except git.exc.InvalidGitRepositoryError:
             print(
                 f"git-dummy: Generating dummy Git repo at {settings.git_dir} with {settings.branches} branch(es) and {settings.commits} commit(s)."
             )
 
-    repo = git.Repo.init(settings.git_dir)
+    repo = git.Repo.init(settings.git_dir, initial_branch="main")
 
     config_writer = repo.config_writer()
-    config_writer.set_value("init", "defaultBranch", "main").release()
+    config_writer.set_value("init", "defaultBranch", "main")
     if settings.constant_sha:
         config_writer.set_value("user", "name", "Git Dummy")
         config_writer.set_value("user", "email", "dumdum@git.dummy")
     config_writer.release()
     
     if settings.constant_sha:
         os.environ["GIT_AUTHOR_DATE"] = "2023-01-01T00:00:00"
```

### Comparing `git-dummy-0.0.9/git_dummy.egg-info/PKG-INFO` & `git-dummy-0.1.0/git_dummy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: git-dummy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generate dummy Git repositories populated with the desired number of commits, branches, and structure.
 Home-page: https://initialcommit.com/tools/git-dummy
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
+License: UNKNOWN
 Project-URL: Homepage, https://initialcommit.com/tools/git-dummy
 Project-URL: Source, https://github.com/initialcommit-com/git-dummy
 Keywords: git dummy generate populate repo repository
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -127,7 +129,9 @@
 Explicitly specifying options at the command-line takes precedence over the corresponding environment variable values.
 
 ## Learn More
 Learn more about this tool on the [git-dummy project page](https://initialcommit.com/tools/git-dummy).
 
 ## Authors
 **Jacob Stopak** - on behalf of [Initial Commit](https://initialcommit.com)
+
+
```

### Comparing `git-dummy-0.0.9/setup.py` & `git-dummy-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="git-dummy",
-    version="0.0.9",
+    version="0.1.0",
     author="Jacob Stopak",
     author_email="jacob@initialcommit.io",
     description="Generate dummy Git repositories populated with the desired number of commits, branches, and structure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://initialcommit.com/tools/git-dummy",
     packages=setuptools.find_packages(),
```

