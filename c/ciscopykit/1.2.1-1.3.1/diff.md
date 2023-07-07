# Comparing `tmp/ciscopykit-1.2.1.tar.gz` & `tmp/ciscopykit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.2.1.tar", last modified: Thu Jul  6 18:08:20 2023, max compression
+gzip compressed data, was "ciscopykit-1.3.1.tar", last modified: Fri Jul  7 15:30:29 2023, max compression
```

## Comparing `ciscopykit-1.2.1.tar` & `ciscopykit-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 18:08:20.000000 ciscopykit-1.2.1/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:08:20.770057 ciscopykit-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-06 18:08:01.000000 ciscopykit-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/switch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/l2_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/l3_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 15:30:29.000000 ciscopykit-1.3.1/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:30:29.081513 ciscopykit-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-07 15:30:11.000000 ciscopykit-1.3.1/setup.py
```

### Comparing `ciscopykit-1.2.1/LICENSE.md` & `ciscopykit-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/PKG-INFO` & `ciscopykit-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.2.1
+Version: 1.3.1
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.2.1/README.md` & `ciscopykit-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/ciscopykit/app.py` & `ciscopykit-1.3.1/ciscopykit/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,7 +27,8 @@
     for interface in active_interfaces:
         print(interface)
 
 
 if __name__ == "__main__":
     main()
 
+#  python app.py --model "Cisco 3750" --ports "GigabitEthernet1/0/1,GigabitEthernet1/0/2,VLAN10,VLAN20" --active-ports "GigabitEthernet1/0/1,GigabitEthernet1/0/2" --routing-protocol "OSPF" --ip-dict "{'VLAN10': '10.0.0.1/24', 'VLAN20': '20.0.0.1/24', 'Gi0/0':'10.10.11.1/30'}" --hostname "LA_SW1" --subnet "10.0.0.0/16"
```

### Comparing `ciscopykit-1.2.1/ciscopykit/device.py` & `ciscopykit-1.3.1/ciscopykit/device.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/ciscopykit/entry_point.py` & `ciscopykit-1.3.1/ciscopykit/entry_point.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/ciscopykit/interface.py` & `ciscopykit-1.3.1/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/ciscopykit/templates/generate_router_config.py` & `ciscopykit-1.3.1/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.2.1/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-1.3.1/ciscopykit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.2.1
+Version: 1.3.1
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.2.1/setup.py` & `ciscopykit-1.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.2.1',
+    version='1.3.1',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
@@ -23,14 +23,16 @@
 
     ],
     install_requires=[
         'click',
         'networkx',
         'matplotlib',
         'ipaddress',
+        'argeparse'
     ],
     entry_points={
         'console_scripts': [
             'ciscopykit = ciscopykit.entry_point:main',
+            'switch = ciscopykit.switch.app:main'
         ],
     },
 )
```

