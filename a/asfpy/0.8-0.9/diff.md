# Comparing `tmp/asfpy-0.8.tar.gz` & `tmp/asfpy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asfpy-0.8.tar", last modified: Sat Aug 10 16:41:02 2019, max compression
+gzip compressed data, was "dist/asfpy-0.9.tar", last modified: Mon Aug 12 15:19:43 2019, max compression
```

## Comparing `asfpy-0.8.tar` & `asfpy-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-10 16:41:02.000000 asfpy-0.8/
--rw-r--r--   0 vaps      (1000) vaps      (1000)       38 2019-08-10 16:41:02.000000 asfpy-0.8/setup.cfg
-drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy/
--rw-rw-r--   0 vaps      (1000) vaps      (1000)       66 2019-08-05 17:51:12.000000 asfpy-0.8/asfpy/__init__.py
--rw-rw-r--   0 vaps      (1000) vaps      (1000)     4606 2019-03-07 20:41:18.000000 asfpy-0.8/asfpy/daemon.py
--rw-rw-r--   0 vaps      (1000) vaps      (1000)    11039 2019-08-06 14:23:18.000000 asfpy-0.8/asfpy/ldap.py
--rw-r--r--   0 vaps      (1000) vaps      (1000)     4065 2019-08-05 17:36:22.000000 asfpy-0.8/asfpy/justone.py
--rw-rw-r--   0 vaps      (1000) vaps      (1000)     3203 2019-08-05 17:50:42.000000 asfpy-0.8/asfpy/messaging.py
--rw-rw-r--   0 vaps      (1000) vaps      (1000)     1766 2019-08-10 16:41:00.000000 asfpy-0.8/setup.py
-drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/
--rw-r--r--   0 vaps      (1000) vaps      (1000)      275 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/SOURCES.txt
--rw-r--r--   0 vaps      (1000) vaps      (1000)        1 2019-08-05 18:09:13.000000 asfpy-0.8/asfpy.egg-info/not-zip-safe
--rw-r--r--   0 vaps      (1000) vaps      (1000)       23 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/requires.txt
--rw-r--r--   0 vaps      (1000) vaps      (1000)      471 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/PKG-INFO
--rw-r--r--   0 vaps      (1000) vaps      (1000)        1 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/dependency_links.txt
--rw-r--r--   0 vaps      (1000) vaps      (1000)        6 2019-08-10 16:41:02.000000 asfpy-0.8/asfpy.egg-info/top_level.txt
--rw-r--r--   0 vaps      (1000) vaps      (1000)      471 2019-08-10 16:41:02.000000 asfpy-0.8/PKG-INFO
--rw-r--r--   0 vaps      (1000) vaps      (1000)       63 2019-08-05 17:36:22.000000 asfpy-0.8/README.rst
+drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-12 15:19:43.000000 asfpy-0.9/
+-rw-r--r--   0 vaps      (1000) vaps      (1000)       38 2019-08-12 15:19:43.000000 asfpy-0.9/setup.cfg
+drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-12 15:19:43.000000 asfpy-0.9/asfpy/
+-rw-rw-r--   0 vaps      (1000) vaps      (1000)       66 2019-08-05 17:51:12.000000 asfpy-0.9/asfpy/__init__.py
+-rw-rw-r--   0 vaps      (1000) vaps      (1000)     4606 2019-03-07 20:41:18.000000 asfpy-0.9/asfpy/daemon.py
+-rw-rw-r--   0 vaps      (1000) vaps      (1000)    14307 2019-08-12 15:18:28.000000 asfpy-0.9/asfpy/ldap.py
+-rw-r--r--   0 vaps      (1000) vaps      (1000)     4065 2019-08-05 17:36:22.000000 asfpy-0.9/asfpy/justone.py
+-rw-rw-r--   0 vaps      (1000) vaps      (1000)     3203 2019-08-05 17:50:42.000000 asfpy-0.9/asfpy/messaging.py
+-rw-rw-r--   0 vaps      (1000) vaps      (1000)     1766 2019-08-12 15:19:21.000000 asfpy-0.9/setup.py
+drwxr-xr-x   0 vaps      (1000) vaps      (1000)        0 2019-08-12 15:19:43.000000 asfpy-0.9/asfpy.egg-info/
+-rw-r--r--   0 vaps      (1000) vaps      (1000)      275 2019-08-12 15:19:42.000000 asfpy-0.9/asfpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vaps      (1000) vaps      (1000)        1 2019-08-05 18:09:13.000000 asfpy-0.9/asfpy.egg-info/not-zip-safe
+-rw-r--r--   0 vaps      (1000) vaps      (1000)       23 2019-08-12 15:19:42.000000 asfpy-0.9/asfpy.egg-info/requires.txt
+-rw-r--r--   0 vaps      (1000) vaps      (1000)      471 2019-08-12 15:19:42.000000 asfpy-0.9/asfpy.egg-info/PKG-INFO
+-rw-r--r--   0 vaps      (1000) vaps      (1000)        1 2019-08-12 15:19:42.000000 asfpy-0.9/asfpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vaps      (1000) vaps      (1000)        6 2019-08-12 15:19:42.000000 asfpy-0.9/asfpy.egg-info/top_level.txt
+-rw-r--r--   0 vaps      (1000) vaps      (1000)      471 2019-08-12 15:19:43.000000 asfpy-0.9/PKG-INFO
+-rw-r--r--   0 vaps      (1000) vaps      (1000)       63 2019-08-05 17:36:22.000000 asfpy-0.9/README.rst
```

### Comparing `asfpy-0.8/asfpy/daemon.py` & `asfpy-0.9/asfpy/daemon.py`

 * *Files identical despite different names*

### Comparing `asfpy-0.8/asfpy/justone.py` & `asfpy-0.9/asfpy/justone.py`

 * *Files identical despite different names*

### Comparing `asfpy-0.8/asfpy/messaging.py` & `asfpy-0.9/asfpy/messaging.py`

 * *Files identical despite different names*

### Comparing `asfpy-0.8/setup.py` & `asfpy-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 def main():
       setuptools.setup(name='asfpy',
-            version='0.8',
+            version='0.9',
             description='ASF Common Python Methods',
             long_description="This is a common set of functions used by the ASF Infrastructure team such as libraries for sending email, ldap management and generic process daemonization.",
             long_description_content_type = "text/plain",
             url='https://svn.apache.org/repos/infra/infrastructure/trunk/projects/asfpy/',
             author='ASF Infrastructure',
             author_email='users@infra.apache.org',
             license='Apache',
```

