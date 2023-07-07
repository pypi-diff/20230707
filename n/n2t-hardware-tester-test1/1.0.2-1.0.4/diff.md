# Comparing `tmp/n2t-hardware-tester-test1-1.0.2.tar.gz` & `tmp/n2t-hardware-tester-test1-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n2t-hardware-tester-test1-1.0.2.tar", last modified: Tue Jul  4 09:50:32 2023, max compression
+gzip compressed data, was "n2t-hardware-tester-test1-1.0.4.tar", last modified: Fri Jul  7 12:04:53 2023, max compression
```

## Comparing `n2t-hardware-tester-test1-1.0.2.tar` & `n2t-hardware-tester-test1-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.982057 n2t-hardware-tester-test1-1.0.2/
--rw-rw-rw-   0        0        0       72 2023-07-04 09:50:32.982057 n2t-hardware-tester-test1-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.922362 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.924714 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/authutil/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/authutil/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/authutil/auth_util.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.927705 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/__init__.py
--rw-rw-rw-   0        0        0     3767 2023-07-04 09:46:17.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.935797 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/
--rw-rw-rw-   0        0        0      556 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h1.yml
--rw-rw-rw-   0        0        0      286 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h2.yml
--rw-rw-rw-   0        0        0      374 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h3.yml
--rw-rw-rw-   0        0        0      183 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h4.yml
--rw-rw-rw-   0        0        0      341 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h5.yml
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.938785 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/configuration/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/configuration/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.940796 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/fetcher/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/fetcher/__init__.py
--rw-rw-rw-   0        0        0     6051 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/fetcher/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.943795 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/grader/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/grader/__init__.py
--rw-rw-rw-   0        0        0     6615 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/grader/grader.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.946980 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/homeworktester/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/homeworktester/__init__.py
--rw-rw-rw-   0        0        0     4720 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/homeworktester/homework_tester.py
--rw-rw-rw-   0        0        0      129 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/homeworktester/test_result.py
--rw-rw-rw-   0        0        0       87 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/main.py
--rw-rw-rw-   0        0        0     1281 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/n2tconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.973775 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/
--rw-rw-rw-   0        0        0       72 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1302 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-04 09:50:32.000000 n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 09:50:32.983090 n2t-hardware-tester-test1-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      604 2023-07-04 09:50:18.000000 n2t-hardware-tester-test1-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.975786 n2t-hardware-tester-test1-1.0.2/test/
--rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.977858 n2t-hardware-tester-test1-1.0.2/test/configuration/
--rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.2/test/configuration/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-07-04 09:45:18.000000 n2t-hardware-tester-test1-1.0.2/test/configuration/configuration_test.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:50:32.980161 n2t-hardware-tester-test1-1.0.2/test/homeworktester/
--rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.2/test/homeworktester/__init__.py
--rw-rw-rw-   0        0        0     2810 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.2/test/homeworktester/single_homework_test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.142663 n2t-hardware-tester-test1-1.0.4/
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:04:53.142663 n2t-hardware-tester-test1-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.070432 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.075098 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/authutil/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/authutil/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/authutil/auth_util.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.085099 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/__init__.py
+-rw-rw-rw-   0        0        0     6329 2023-07-06 13:15:27.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.096157 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/
+-rw-rw-rw-   0        0        0      556 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h1.yml
+-rw-rw-rw-   0        0        0      286 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h2.yml
+-rw-rw-rw-   0        0        0      374 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h3.yml
+-rw-rw-rw-   0        0        0      183 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h4.yml
+-rw-rw-rw-   0        0        0      341 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h5.yml
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.100781 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/configuration/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.104785 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/fetcher/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/fetcher/__init__.py
+-rw-rw-rw-   0        0        0     6051 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/fetcher/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.107785 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/grader/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/grader/__init__.py
+-rw-rw-rw-   0        0        0     6615 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/grader/grader.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.114130 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/homeworktester/
+-rw-rw-rw-   0        0        0        0 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/homeworktester/__init__.py
+-rw-rw-rw-   0        0        0     4720 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/homeworktester/homework_tester.py
+-rw-rw-rw-   0        0        0      129 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/homeworktester/test_result.py
+-rw-rw-rw-   0        0        0       87 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/main.py
+-rw-rw-rw-   0        0        0     1461 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/n2tconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.132389 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/
+-rw-rw-rw-   0        0        0       72 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1302 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-07 12:04:52.000000 n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:04:53.143680 n2t-hardware-tester-test1-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      604 2023-07-06 13:17:06.000000 n2t-hardware-tester-test1-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.133383 n2t-hardware-tester-test1-1.0.4/test/
+-rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.137383 n2t-hardware-tester-test1-1.0.4/test/configuration/
+-rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.4/test/configuration/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-07-06 13:15:15.000000 n2t-hardware-tester-test1-1.0.4/test/configuration/configuration_test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:04:53.140648 n2t-hardware-tester-test1-1.0.4/test/homeworktester/
+-rw-rw-rw-   0        0        0        0 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.4/test/homeworktester/__init__.py
+-rw-rw-rw-   0        0        0     2810 2023-07-03 07:32:08.000000 n2t-hardware-tester-test1-1.0.4/test/homeworktester/single_homework_test.py
```

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/authutil/auth_util.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/authutil/auth_util.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/cmdi/data/h1.yml` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/cmdi/data/h1.yml`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/configuration/configuration.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/fetcher/fetcher.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/fetcher/fetcher.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/grader/grader.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/grader/grader.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/homeworktester/homework_tester.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/homeworktester/homework_tester.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester/n2tconfig.py` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester/n2tconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 GOOGLE_API_CREDENTIALS: str = os.getenv("n2t_google_api_credentials")  # type: ignore
 GOOGLE_API_TOKENS_PATH: str = os.getenv("n2t_google_api_tokens_path")  # type: ignore
 DOWNLOAD_FOLDER: str = os.getenv("n2t_homework_files_download_folder")  # type: ignore
 
 env_variables_for_student = [N2T_WORK_AREA_PATH]
 env_variables_for_lecturer = [N2T_WORK_AREA_PATH, GOOGLE_API_CREDENTIALS, GOOGLE_API_TOKENS_PATH, DOWNLOAD_FOLDER]
 
+env_variable_names = ['n2t_work_area_path', 'n2t_google_api_credentials', 'n2t_google_api_tokens_path', 'n2t_homework_files_download_folder']
+
 env_variable_description = {
-    N2T_WORK_AREA_PATH: """Path of nand2tetris directory which contains tools and project folder for the course, 
+    "n2t_work_area_path": """Path of nand2tetris directory which contains tools and project folder for the course, 
     for example -> C:/Users/StudentName/nand2tetris
     """,
-    GOOGLE_API_CREDENTIALS: "path of google classroom api Credentials file for google authentication, must be downloaded from google cloud console",
-    GOOGLE_API_TOKENS_PATH: "path of google classroom api token path. token file is not necessary, will be downloaded automatically after login",
-    DOWNLOAD_FOLDER: "path of download folder, where student assignment attachments will be downloaded",
+    'n2t_google_api_credentials': "path of google classroom api Credentials file for google authentication, must be downloaded from google cloud console",
+    'n2t_google_api_tokens_path': "path of google classroom api token path. token file is not necessary, will be downloaded automatically after login",
+    'n2t_homework_files_download_folder': "path of download folder, where student assignment attachments will be downloaded",
 }
```

### Comparing `n2t-hardware-tester-test1-1.0.2/n2t_hardware_tester_test1.egg-info/SOURCES.txt` & `n2t-hardware-tester-test1-1.0.4/n2t_hardware_tester_test1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/setup.py` & `n2t-hardware-tester-test1-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="n2t-hardware-tester-test1",
-    version="1.0.2",
+    version="1.0.4",
     packages=find_packages(),
     install_requires=[
         "pytest",
         "PyYAML~=6.0",
         "requests",
         "typer",
         "google-api-python-client",
```

### Comparing `n2t-hardware-tester-test1-1.0.2/test/configuration/configuration_test.py` & `n2t-hardware-tester-test1-1.0.4/test/configuration/configuration_test.py`

 * *Files identical despite different names*

### Comparing `n2t-hardware-tester-test1-1.0.2/test/homeworktester/single_homework_test.py` & `n2t-hardware-tester-test1-1.0.4/test/homeworktester/single_homework_test.py`

 * *Files identical despite different names*

