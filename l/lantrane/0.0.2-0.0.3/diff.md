# Comparing `tmp/lantrane-0.0.2.tar.gz` & `tmp/lantrane-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantrane-0.0.2.tar", last modified: Thu Jul  6 02:54:26 2023, max compression
+gzip compressed data, was "lantrane-0.0.3.tar", last modified: Fri Jul  7 17:41:18 2023, max compression
```

## Comparing `lantrane-0.0.2.tar` & `lantrane-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/
--rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.2/LICENSE.md
--rw-rw-r--   0 ace       (1000) ace       (1000)     1127 2023-07-06 02:54:26.313043 lantrane-0.0.2/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      672 2023-07-06 01:14:46.000000 lantrane-0.0.2/README.md
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/lantrane/
--rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.2/lantrane/__init__.py
--rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-01 23:22:02.000000 lantrane-0.0.2/lantrane/data.py
--rw-rw-r--   0 ace       (1000) ace       (1000)     1218 2023-07-06 02:53:39.000000 lantrane-0.0.2/lantrane/lantrane.py
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/lantrane.egg-info/
--rw-rw-r--   0 ace       (1000) ace       (1000)     1127 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      216 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/SOURCES.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/dependency_links.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/top_level.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-06 02:54:26.313043 lantrane-0.0.2/setup.cfg
--rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-06 02:54:10.000000 lantrane-0.0.2/setup.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 17:41:18.730797 lantrane-0.0.3/
+-rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.3/LICENSE.md
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1199 2023-07-07 17:41:18.730797 lantrane-0.0.3/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      744 2023-07-07 17:40:46.000000 lantrane-0.0.3/README.md
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 17:41:18.730797 lantrane-0.0.3/lantrane/
+-rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.3/lantrane/__init__.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-01 23:22:02.000000 lantrane-0.0.3/lantrane/data.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1325 2023-07-07 17:41:01.000000 lantrane-0.0.3/lantrane/lantrane.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-07 17:41:18.730797 lantrane-0.0.3/lantrane.egg-info/
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1199 2023-07-07 17:41:18.000000 lantrane-0.0.3/lantrane.egg-info/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      216 2023-07-07 17:41:18.000000 lantrane-0.0.3/lantrane.egg-info/SOURCES.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-07 17:41:18.000000 lantrane-0.0.3/lantrane.egg-info/dependency_links.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-07 17:41:18.000000 lantrane-0.0.3/lantrane.egg-info/top_level.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-07 17:41:18.730797 lantrane-0.0.3/setup.cfg
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-07 17:39:45.000000 lantrane-0.0.3/setup.py
```

### Comparing `lantrane-0.0.2/LICENSE.md` & `lantrane-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.2/PKG-INFO` & `lantrane-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +19,21 @@
 
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
+import asyncio
 
-for data in Trane(args.ip, args.port).listen():
+async def read_async():
+	async for data in Trane(args.ip, args.port).listen():
 	print(data)
 
+asyncio.run(read_async())
 ```
 
 
 
 ## Distribution
 
 ```
```

### Comparing `lantrane-0.0.2/README.md` & `lantrane-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
+import asyncio
 
-for data in Trane(args.ip, args.port).listen():
+async def read_async():
+	async for data in Trane(args.ip, args.port).listen():
 	print(data)
 
+asyncio.run(read_async())
 ```
 
 
 
 ## Distribution
 
 ```
```

### Comparing `lantrane-0.0.2/lantrane/data.py` & `lantrane-0.0.3/lantrane/data.py`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.2/lantrane.egg-info/PKG-INFO` & `lantrane-0.0.3/lantrane.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +19,21 @@
 
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
+import asyncio
 
-for data in Trane(args.ip, args.port).listen():
+async def read_async():
+	async for data in Trane(args.ip, args.port).listen():
 	print(data)
 
+asyncio.run(read_async())
 ```
 
 
 
 ## Distribution
 
 ```
```

### Comparing `lantrane-0.0.2/setup.py` & `lantrane-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=[],      								  # Dependencies
      python_requires='>=3',                                   # Minimum Python version
      name='lantrane',                                  # Package name
-     version="0.0.2",                                     # Version
+     version="0.0.3",                                     # Version
      author="Adrian Edwards",                                 # Author name
      author_email="adrian@adriancedwards.com",                           # Author mail
      description="Python package for interacting with Trane thermostats locally.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/MoralCode/lantrane",       # Url to your Git Repo
     #  download_url = 'https://github.com/MoralCode/lantrane/archive/'+new_version+'.tar.gz',
```

