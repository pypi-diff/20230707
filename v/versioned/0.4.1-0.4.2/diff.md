# Comparing `tmp/versioned-0.4.1.tar.gz` & `tmp/versioned-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.4.1.tar", last modified: Fri Jul  7 14:51:01 2023, max compression
+gzip compressed data, was "versioned-0.4.2.tar", last modified: Fri Jul  7 18:17:27 2023, max compression
```

## Comparing `versioned-0.4.1.tar` & `versioned-0.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.617604 versioned-0.4.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.4.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 14:51:01.617444 versioned-0.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.4.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     3784 2023-07-07 14:50:17.000000 versioned-0.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.4.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.4.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-07 14:51:01.617650 versioned-0.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.4.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.613399 versioned-0.4.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1091 2023-07-07 14:48:52.000000 versioned-0.4.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9626 2023-07-07 14:49:13.000000 versioned-0.4.1/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.615542 versioned-0.4.1/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.4.1/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-07 14:49:59.000000 versioned-0.4.1/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.4.1/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.4.1/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.4.1/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    16596 2023-07-07 14:48:27.000000 versioned-0.4.1/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.616220 versioned-0.4.1/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.4.1/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.4.1/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.616620 versioned-0.4.1/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.4.1/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.617219 versioned-0.4.1/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.4.1/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.4.1/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 14:51:01.616113 versioned-0.4.1/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 14:51:01.000000 versioned-0.4.1/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-07 14:51:01.000000 versioned-0.4.1/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-07 14:51:01.000000 versioned-0.4.1/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-07 14:51:01.000000 versioned-0.4.1/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-07 14:51:01.000000 versioned-0.4.1/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.539202 versioned-0.4.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.4.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.4.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.4.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 18:17:27.539063 versioned-0.4.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.4.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4015 2023-07-07 18:16:47.000000 versioned-0.4.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.4.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.4.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.4.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-07 18:17:27.539247 versioned-0.4.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.4.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.536214 versioned-0.4.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1091 2023-07-07 14:48:52.000000 versioned-0.4.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9626 2023-07-07 14:49:13.000000 versioned-0.4.2/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537205 versioned-0.4.2/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.4.2/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-07 18:16:04.000000 versioned-0.4.2/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.4.2/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.4.2/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.4.2/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16648 2023-07-07 18:15:44.000000 versioned-0.4.2/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537866 versioned-0.4.2/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.4.2/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.4.2/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.538277 versioned-0.4.2/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.4.2/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.538877 versioned-0.4.2/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.4.2/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.4.2/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 18:17:27.537762 versioned-0.4.2/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-07 18:17:27.000000 versioned-0.4.2/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.4.1/AUTHORS.rst` & `versioned-0.4.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/LICENSE.txt` & `versioned-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/PKG-INFO` & `versioned-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.4.1
+Version: 0.4.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.4.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.4.1/README.rst` & `versioned-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/release-history.rst` & `versioned-0.4.2/release-history.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.2 (2023-07-07)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that the ``purge_all`` method cannot delete DynamoDB items correctly when S3 doesn't have the artifacts.
+
+
 0.4.1 (2023-07-07)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - add ``versioned.api.Repository.connect_boto_session`` to public API. it can explicitly connect the S3 and DynamoDB API to the given boto session.
 - removed useless argument ``bsm`` in many APIs.
 - add ``versioned.api.Repository.purge_all`` to public API.
```

### Comparing `versioned-0.4.1/requirements-doc.txt` & `versioned-0.4.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/setup.py` & `versioned-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/tests/test_api.py` & `versioned-0.4.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/tests/test_core.py` & `versioned-0.4.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/bootstrap.py` & `versioned-0.4.2/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/core.py` & `versioned-0.4.2/versioned/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,10 +498,12 @@
 
     def purge_all(self):
         """
         Completely delete all artifacts and aliases in this Repository
         This operation is irreversible. It will remove all related S3 artifacts
         and DynamoDB items.
         """
-        for s3dir in self.s3dir_artifact_store.iterdir():
-            artifact_name = s3dir.basename
-            self.purge_artifact(name=artifact_name)
+        self.s3dir_artifact_store.delete()
+        Artifact = self._artifact_class
+        with Artifact.batch_write() as batch:
+            for item in Artifact.scan():
+                batch.delete(item)
```

### Comparing `versioned-0.4.1/versioned/dynamodb.py` & `versioned-0.4.2/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/paths.py` & `versioned-0.4.2/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/tests/mock_aws.py` & `versioned-0.4.2/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/vendor/hashes.py` & `versioned-0.4.2/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned/vendor/pytest_cov_helper.py` & `versioned-0.4.2/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.4.1/versioned.egg-info/PKG-INFO` & `versioned-0.4.2/versioned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.4.1
+Version: 0.4.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.4.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.4.1/versioned.egg-info/SOURCES.txt` & `versioned-0.4.2/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

