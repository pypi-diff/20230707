# Comparing `tmp/apache_airflow_providers_kettle-1.0.4.tar.gz` & `tmp/apache_airflow_providers_kettle-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_kettle-1.0.4.tar", last modified: Sun Jun 25 21:52:57 2023, max compression
+gzip compressed data, was "apache_airflow_providers_kettle-1.0.5.tar", last modified: Fri Jul  7 11:48:28 2023, max compression
```

## Comparing `apache_airflow_providers_kettle-1.0.4.tar` & `apache_airflow_providers_kettle-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/
--rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.4/LICENSE
--rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:00:40.000000 apache_airflow_providers_kettle-1.0.4/README.md
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/
--rw-rw-r--   0 bop       (1000) bop       (1000)      468 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/SOURCES.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/dependency_links.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/entry_points.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/requires.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-06-25 21:52:57.000000 apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/top_level.txt
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/kettle_provider/
--rw-rw-r--   0 bop       (1000) bop       (1000)      429 2023-06-25 21:52:42.000000 apache_airflow_providers_kettle-1.0.4/kettle_provider/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/kettle_provider/hooks/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.4/kettle_provider/hooks/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/kettle_provider/operators/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.4/kettle_provider/operators/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)     8598 2023-06-25 20:10:05.000000 apache_airflow_providers_kettle-1.0.4/kettle_provider/operators/kettle_operator.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/kettle_provider/sensors/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.4/kettle_provider/sensors/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-06-25 21:52:57.696189 apache_airflow_providers_kettle-1.0.4/setup.cfg
--rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-06-25 21:52:45.000000 apache_airflow_providers_kettle-1.0.4/setup.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/
+-rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.5/LICENSE
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4040 2023-07-07 11:47:10.000000 apache_airflow_providers_kettle-1.0.5/README.md
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/SOURCES.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/dependency_links.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/entry_points.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/requires.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/top_level.txt
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/
+-rw-rw-r--   0 bop       (1000) bop       (1000)      438 2023-07-07 11:46:20.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/hooks/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/hooks/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)     8600 2023-07-07 11:46:37.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/kettle_operator.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/sensors/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/sensors/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/setup.cfg
+-rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-07-07 11:46:11.000000 apache_airflow_providers_kettle-1.0.5/setup.py
```

### Comparing `apache_airflow_providers_kettle-1.0.4/LICENSE` & `apache_airflow_providers_kettle-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.4/apache_airflow_providers_kettle.egg-info/SOURCES.txt` & `apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.4/kettle_provider/operators/kettle_operator.py` & `apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/kettle_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             -level={self.loglevel} \
             -logfile={self.logfile} \
             -maxloglines={self.maxloglines} \
             -maxlogtimeout={self.maxlogtimeout} \
             -norep=Y '
         # Get additional parameters
         for k, v in self.params.items():
-            pdi_command.append(f'-param:{k}={v}')
+            pdi_command.append(f'-param:{k}={v} ')
         # Execute the command
         result = self.subprocess_hook.run_command(
             command=[bash_path, '-c', pdi_command],
             output_encoding=self.output_encoding,
             cwd=self.pdipath
         )
         if result.exit_code != 0:
@@ -170,15 +170,15 @@
             -level={self.loglevel} \
             -logfile={self.logfile} \
             -maxloglines={self.maxloglines} \
             -maxlogtimeout={self.maxlogtimeout} \
             -norep=Y '
         # Get additional parameters
         for k, v in self.params.items():
-            pdi_command.append(f'-param:{k}={v}')
+            pdi_command.append(f'-param:{k}={v} ')
         # Execute the command
         result = self.subprocess_hook.run_command(
             command=[bash_path, '-c', pdi_command],
             output_encoding=self.output_encoding,
             cwd=self.pdipath
         )
         if result.exit_code != 0:
```

### Comparing `apache_airflow_providers_kettle-1.0.4/setup.py` & `apache_airflow_providers_kettle-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 """Perform the package airflow-provider-kettle-operator setup."""
 setup(
     name="apache_airflow_providers_kettle",
     version=__version__,
     description="A simple Apache Airflow Kettle Operator that can invoke jobs and transformations for Linux based systems.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={"apache_airflow_provider": ["provider_info=kettle_provider.__init__:get_provider_info"]},
     license="Apache License 2.0",
     packages=find_packages(exclude=["*tests.*", "*tests"]),
-    install_requires=["apache-airflow>=2.3"],
+    install_requires=["apache-airflow>=2.0"],
     setup_requires=["setuptools", "wheel"],
     author="Robert Bryśkiewicz",
     author_email="bryskiewiczr@pm.me",
     url="",
     classifiers=[
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
```

