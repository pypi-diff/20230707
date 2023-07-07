# Comparing `tmp/versioned-0.3.2.tar.gz` & `tmp/versioned-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.3.2.tar", last modified: Thu Jul  6 16:53:41 2023, max compression
+gzip compressed data, was "versioned-0.3.3.tar", last modified: Thu Jul  6 19:44:58 2023, max compression
```

## Comparing `versioned-0.3.2.tar` & `versioned-0.3.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.151189 versioned-0.3.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.3.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.3.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.3.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 16:53:41.151031 versioned-0.3.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.3.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     3152 2023-07-06 16:52:53.000000 versioned-0.3.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.3.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.3.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 16:53:41.151232 versioned-0.3.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.3.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.146201 versioned-0.3.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1058 2023-07-06 16:52:28.000000 versioned-0.3.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    10092 2023-07-06 16:50:27.000000 versioned-0.3.2/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.148740 versioned-0.3.2/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.3.2/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 16:51:24.000000 versioned-0.3.2/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.3.2/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1864 2023-07-06 16:43:17.000000 versioned-0.3.2/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.3.2/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    16380 2023-07-06 16:48:54.000000 versioned-0.3.2/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149530 versioned-0.3.2/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.3.2/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.3.2/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149999 versioned-0.3.2/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.3.2/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.150810 versioned-0.3.2/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.3.2/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149397 versioned-0.3.2/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.566754 versioned-0.3.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.3.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.3.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.3.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 19:44:58.566590 versioned-0.3.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.3.3/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3403 2023-07-06 19:44:04.000000 versioned-0.3.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.3.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.3.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.3.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.3.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.3.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 19:44:58.566808 versioned-0.3.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.3.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.561744 versioned-0.3.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1058 2023-07-06 16:52:28.000000 versioned-0.3.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10269 2023-07-06 19:42:46.000000 versioned-0.3.3/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.564362 versioned-0.3.3/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.3.3/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 19:43:10.000000 versioned-0.3.3/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.3.3/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1864 2023-07-06 16:43:17.000000 versioned-0.3.3/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.3.3/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16826 2023-07-06 19:39:24.000000 versioned-0.3.3/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.565184 versioned-0.3.3/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.3.3/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.3.3/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.565646 versioned-0.3.3/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.3.3/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.566372 versioned-0.3.3/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.3.3/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.3.3/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 19:44:58.565043 versioned-0.3.3/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 19:44:58.000000 versioned-0.3.3/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 19:44:58.000000 versioned-0.3.3/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 19:44:58.000000 versioned-0.3.3/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 19:44:58.000000 versioned-0.3.3/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 19:44:58.000000 versioned-0.3.3/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.3.2/AUTHORS.rst` & `versioned-0.3.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/LICENSE.txt` & `versioned-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/PKG-INFO` & `versioned-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.3.2
+Version: 0.3.3
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.3.2/README.rst` & `versioned-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/release-history.rst` & `versioned-0.3.3/release-history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.3 (2023-07-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- allow user to set a file name extension for the artifact repository via ``versioned.api.Repository(..., suffix=".tar.gz")``.
+
+
 0.3.2 (2023-07-06)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - now the ``versioned.api.Repository`` takes explicit ``aws_region``, ``s3_bucket`` arguments in constructor.
 - add ``versioned.api.Repository.get_artifact_s3path`` to public API.
```

### Comparing `versioned-0.3.2/requirements-doc.txt` & `versioned-0.3.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/setup.py` & `versioned-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/tests/test_api.py` & `versioned-0.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/tests/test_core.py` & `versioned-0.3.3/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
     @classmethod
     def setup_class_post_hook(cls):
         context.attach_boto_session(cls.bsm.boto_ses)
         cls.repo = Repository(
             aws_region=cls.bsm.aws_region,
             s3_bucket=f"{cls.bsm.aws_account_id}-{cls.bsm.aws_region}-artifacts",
+            suffix=".txt",
         )
         cls.repo.bootstrap(cls.bsm)
 
     def _test(self):
         name = "deploy"
         alias = "LIVE"
 
@@ -65,15 +66,15 @@
         # rprint(artifact)
         # put artifact with the same content, S3 and Dynamodb should not changed
         artifact = self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v1")
 
         def _assert_artifact(artifact):
             assert artifact.name == name
             assert artifact.version == constants.LATEST_VERSION
-            assert artifact.s3uri.endswith(constants.LATEST_VERSION)
+            assert artifact.s3uri.endswith(constants.LATEST_VERSION + ".txt")
             assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         _assert_artifact(artifact)
 
         artifact = self.repo.get_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         _assert_artifact(artifact)
@@ -82,31 +83,35 @@
         # rprint(artifact_list)
         assert len(artifact_list) == 1
         _assert_artifact(artifact_list[0])
 
         artifact = self.repo.publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "1"
-        assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL))
-        assert artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL)
+        assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL) + ".txt")
+        assert (
+            artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL) + ".txt"
+        )
         assert artifact.s3path.metadata["foo"] == "bar"
         assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         # put artifact again
         artifact = self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v2")
         # rprint(artifact)
         assert artifact.version == constants.LATEST_VERSION
         assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
 
         artifact = self.repo.publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "2"
         s3path = S3Path(artifact.s3uri)
-        assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL))
-        assert artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL)
+        assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL) + ".txt")
+        assert (
+            artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL) + ".txt"
+        )
         assert artifact.get_content(bsm=self.bsm) == b"v2"
 
         artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 3
 
         # ======================================================================
         # Artifact
@@ -114,15 +119,17 @@
         # --- test raises error ---
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.put_alias(bsm=self.bsm, name=name, alias=alias, version=999)
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
-            self.repo.put_alias(bsm=self.bsm, name=name, alias=alias, secondary_version=999)
+            self.repo.put_alias(
+                bsm=self.bsm, name=name, alias=alias, secondary_version=999
+            )
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
             self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
@@ -181,15 +188,15 @@
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
             assert ali.version == constants.LATEST_VERSION
             assert ali.secondary_version is None
             assert ali.secondary_version_weight is None
-            assert ali.version_s3uri.endswith(constants.LATEST_VERSION)
+            assert ali.version_s3uri.endswith(constants.LATEST_VERSION + ".txt")
             assert ali.secondary_version_s3uri is None
             assert ali.get_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
         ali = self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
@@ -212,16 +219,16 @@
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
             assert ali.version == "1"
             assert ali.secondary_version == "2"
             assert ali.secondary_version_weight == 20
-            assert ali.version_s3uri.endswith(encode_version(1))
-            assert ali.secondary_version_s3uri.endswith(encode_version(2))
+            assert ali.version_s3uri.endswith(encode_version(1) + ".txt")
+            assert ali.secondary_version_s3uri.endswith(encode_version(2) + ".txt")
             assert ali.get_version_content(bsm=self.bsm) == b"v1"
             assert ali.get_secondary_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
         ali = self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
```

### Comparing `versioned-0.3.2/versioned/bootstrap.py` & `versioned-0.3.3/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned/core.py` & `versioned-0.3.3/versioned/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,31 +104,39 @@
         Get the content of the secondary artifact version of this alias.
         """
         return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
 
 @dataclasses.dataclass
 class Repository:
+    """
+    :param aws_region: the aws region of where the artifact store is.
+    :param s3_bucket: the s3 bucket name of the artifact store.
+    :param s3_prefix: the s3 prefix (folder path) of the artifact store.
+    :param dynamodb_table_name: the dynamodb table name of the artifact metadata store.
+    :param suffix: the file extension suffix of the artifact binary.
+    """
     aws_region: str = dataclasses.field()
     s3_bucket: str = dataclasses.field()
     s3_prefix: str = dataclasses.field(default=constants.S3_PREFIX)
     dynamodb_table_name: str = dataclasses.field(default=constants.DYNAMODB_TABLE_NAME)
+    suffix: str = dataclasses.field(default="")
 
     @property
     def s3dir_artifact_store(self) -> S3Path:
         """
         Return the s3dir of the artifact store folder.
         """
         return S3Path(self.s3_bucket).joinpath(self.s3_prefix).to_dir()
 
     def get_artifact_s3path(self, name: str, version: str) -> S3Path:
         return S3Path(self.s3_bucket).joinpath(
             self.s3_prefix,
             name,
-            dynamodb.encode_version(version),
+            f"{dynamodb.encode_version(version)}{self.suffix}",
         )
 
     def bootstrap(
         self,
         bsm: BotoSesManager,
         dynamodb_write_capacity_units: T.Optional[int] = None,
         dynamodb_read_capacity_units: T.Optional[int] = None,
```

### Comparing `versioned-0.3.2/versioned/dynamodb.py` & `versioned-0.3.3/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned/paths.py` & `versioned-0.3.3/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned/tests/mock_aws.py` & `versioned-0.3.3/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned/vendor/hashes.py` & `versioned-0.3.3/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned/vendor/pytest_cov_helper.py` & `versioned-0.3.3/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.2/versioned.egg-info/PKG-INFO` & `versioned-0.3.3/versioned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.3.2
+Version: 0.3.3
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.3.2/versioned.egg-info/SOURCES.txt` & `versioned-0.3.3/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

