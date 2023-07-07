# Comparing `tmp/django-titofisto-0.2.2.tar.gz` & `tmp/django_titofisto-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-titofisto-0.2.2.tar", max compression
+gzip compressed data, was "django_titofisto-1.0.0.tar", max compression
```

## Comparing `django-titofisto-0.2.2.tar` & `django_titofisto-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1518 2022-02-03 09:09:26.019725 django-titofisto-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0    11373 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/LICENSE
--rw-r--r--   0        0        0     3003 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/README.rst
--rw-r--r--   0        0        0      817 2022-02-03 09:09:37.259701 django-titofisto-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       38 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/__init__.py
--rw-r--r--   0        0        0      315 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/settings.py
--rw-r--r--   0        0        0     1544 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/storage.py
--rw-r--r--   0        0        0      701 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/test_settings.py
--rw-r--r--   0        0        0      165 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/test_urls.py
--rw-r--r--   0        0        0     6179 2022-02-03 09:08:37.359830 django-titofisto-0.2.2/titofisto/tests.py
--rw-r--r--   0        0        0      142 2021-12-07 10:10:52.592509 django-titofisto-0.2.2/titofisto/urls.py
--rw-r--r--   0        0        0     1623 2022-02-03 09:08:37.359830 django-titofisto-0.2.2/titofisto/views.py
--rw-r--r--   0        0        0     3764 2022-02-03 09:10:26.196059 django-titofisto-0.2.2/setup.py
--rw-r--r--   0        0        0     3783 2022-02-03 09:10:26.196326 django-titofisto-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1737 2023-07-07 19:37:58.513308 django_titofisto-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11373 2021-12-07 10:10:52.592509 django_titofisto-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4519 2023-07-07 20:07:12.751646 django_titofisto-1.0.0/README.rst
+-rw-r--r--   0        0        0      863 2023-07-07 20:16:42.207155 django_titofisto-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2021-12-07 10:10:52.592509 django_titofisto-1.0.0/titofisto/__init__.py
+-rw-r--r--   0        0        0      472 2023-07-07 19:50:59.996547 django_titofisto-1.0.0/titofisto/settings.py
+-rw-r--r--   0        0        0     1672 2023-07-07 17:40:15.939074 django_titofisto-1.0.0/titofisto/storage.py
+-rw-r--r--   0        0        0      733 2023-07-07 19:51:17.780528 django_titofisto-1.0.0/titofisto/test_settings.py
+-rw-r--r--   0        0        0      165 2023-07-07 17:48:02.146669 django_titofisto-1.0.0/titofisto/test_urls.py
+-rw-r--r--   0        0        0     7870 2023-07-07 20:12:59.283346 django_titofisto-1.0.0/titofisto/tests.py
+-rw-r--r--   0        0        0      460 2023-07-07 18:57:09.038691 django_titofisto-1.0.0/titofisto/urls.py
+-rw-r--r--   0        0        0     3948 2023-07-07 20:11:36.535417 django_titofisto-1.0.0/titofisto/views.py
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 django_titofisto-1.0.0/PKG-INFO
```

### Comparing `django-titofisto-0.2.2/CHANGELOG.md` & `django_titofisto-1.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.0] - 2023-07-07
+### Added
+- Time-constrained upload slot handling
+
+### Changed
+- Use Django's Signer for token generation and verification
+
 ## [0.2.2] - 2022-02-03
 ### Fixed
 - Non-existing files in the public namespace erroneously raised interal server errors.
 
 ## [0.2.1] – 2021-12-07
 ### Changed
 - Allow Django 4.0
@@ -37,7 +44,8 @@
 [0.1.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.0
 [0.1.1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.1
 [0.1.2]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.2
 [0.1.2.post1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.2.post1
 [0.2.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.0
 [0.2.1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.1
 [0.2.2]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.2
+[0.3.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.3.0
```

### Comparing `django-titofisto-0.2.2/LICENSE` & `django_titofisto-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-titofisto-0.2.2/README.rst` & `django_titofisto-1.0.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Django Time-Token File Storage
 ==============================
 
 This is a simple extension to Django's `FileSystemStorage` that adds a URL
 parameter carrying a shared token, which is only valid for a defined period
 of time.
 
+Additionally, a like-wise time-constrained file upload slot mechanism is
+available.
+
 Functionality
 -------------
 
+File storage with token-secured URLs
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 This is a drop-in replacement for the Django `FileSystemStorage`, usable if
 media files are served by Django itself. It does currently not work if media
 files are served from an independent web server.
 
 The storage and its accompanying view do the following:
 
 * When a URL to a storage file is generated, a HMAC-based token is generated
@@ -19,22 +25,34 @@
   parameters to the URL
 * Upon retrieval of the file through the accompanying view, the requested
   file name and the passed timestamp are used to recalculate the HMAC-based
   token
 * Only if the tokens match, and a configured timeout has not passed, is the
   file served
 
-The HMAC-based token ensures that the token is invalidated when:
+The signature-based token ensures that the token is invalidated when:
 
 * The filename changes
 * The timestamp changes
 * The mtime of the file changes
 * The `SECRET_KEY` changes
 
-The HMAC is salted with the `SECRET_KEY`.
+Time-constrained uplaod slot
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The upload slot mechanism can be used to generically handle file uploads
+by clients that can not upload files with a regular request. One example
+for this is a client using GraphQL to talk to Django, because GraphQL
+does not support file uploads and rather suggests to do uplaods
+out-of-band.
+
+With Titofisto's upload slot mechanism, calling code can request a secure
+URL which it can hand out to a client. When the client POSTs its file
+to the endpoint, a previously provided callback is called to handle the
+uploaded file.
 
 Installation
 ------------
 
 To add `django-titofisto`_ to a project, first add it as dependency to your
 project, e.g. using `poetry`_::
 
@@ -63,25 +81,51 @@
 
 Provide public media files
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Sometimes, there might be media files, for example favicons,
 you want to be accessible without any authentication. Per default,
 `django-titofisto` will serve all files stored in the directory `public` without a token.
-You can disable or configure this behavior using these settings:
+You can disable or configure this behavior using these settings::
 
   TITOFISTO_USE_PUBLIC_NAMESPACE = True # optional, this is the default
   TITOFISTO_PUBLIC_NAMESPACE = "public/" # optional, this is the default
 
+Use the time-constrained upload slot
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To enable the file upload mechanism, a setting must be set, because the
+default `upload/` prefix could potentially shadow expected media file
+URLs::
+
+  TITOFISTO_ENABLE_UPLOAD = True
+  TITOFISTO_UPLOAD_NAMESPACE = "titofisto/upload/"
+
+A simplified example for using the upload slot mechanism is::
+
+  from titofisto.views import TitofistoUploadView
+
+  def handle_file(request, pk):
+      instance = MyModel.objects.get(pk=pk)
+      instance.photo = request.FILES["photo"]
+      instance.save()
+
+  # This gets an uplaod URL to pass on to the client
+  # On upload, the handler above will be called, with 15 as positional argument
+  upload_url = TitofistoUploadView.get_upload_slot(
+      "mymodule.handle_file",
+      (15,)
+  )
+
 Credits
 -------
 
 `django-titofisto` was developed for the `AlekSIS`_ school information system by
-its team.
+its team::
 
-  Copyright © 2021 Dominik George <dominik.george@teckids.org>
+  Copyright © 2021, 2023 Dominik George <dominik.george@teckids.org>
   Copyright © 2021 Jonathan Weth <dev@jonathanweth.de>
 
 .. _django-titofisto: https://edugit.org/AlekSIS/libs/django-titofisto
 .. _poetry: https://python-poetry.org/
 .. _Django's cache framework: https://docs.djangoproject.com/en/3.2/topics/cache/
 .. _AlekSIS: https://aleksis.org/
```

### Comparing `django-titofisto-0.2.2/pyproject.toml` & `django_titofisto-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-titofisto"
-version = "0.2.2"
+version = "1.0.0"
 description = "Django Time-Token File Storage"
 authors = ["Dominik George <dominik.george@teckids.org>", "Jonathan Weth <dev@jonathanweth.de>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://edugit.org/AlekSIS/libs/django-titofisto"
 keywords = ["django", "storage", "media", "secure"]
 classifiers = [
@@ -17,14 +17,16 @@
     { include = "titofisto" },
 ]
 include = ["LICENSE", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Django = ">2.2,<5.0"
+shortuuid = "^1.0.11"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
 freezegun = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django-titofisto-0.2.2/titofisto/storage.py` & `django_titofisto-1.0.0/titofisto/storage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import hmac
 from datetime import datetime
-from typing import Optional
 
-from django.conf import settings
 from django.core.files.storage import FileSystemStorage
+from django.core.signing import TimestampSigner
 
-from .settings import PARAM, USE_PUBLIC_NAMESPACE, PUBLIC_NAMESPACE
+from .settings import PARAM, TIMEOUT, USE_PUBLIC_NAMESPACE, PUBLIC_NAMESPACE
 
 
 class TitofistoStorage(FileSystemStorage):
     """Time-token secured variant of the base filesystem storage."""
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._signer = TimestampSigner()
+
     def url(self, name: str) -> str:
         """Compute URL for requested storage file."""
         # Get regular URL from base FileSystemStorage
         raw_url = super().url(name)
 
         if USE_PUBLIC_NAMESPACE:
             # Public files are accessible without a token
@@ -24,23 +26,22 @@
         # Get token and timestamp
         token = self.get_token(name)
 
         # Generate full, token-secured URL
         full_url = f"{raw_url}?{PARAM}={token}"
         return full_url
 
-    def get_token(self, name: str, ts: Optional[int] = None) -> str:
-        """Get a token for a filename."""
-        # Determine parts of the HMAC from the file
+    def get_token_message(self, name: str) -> str:
+        """Determine parts of the MAC from the file."""
         if self.exists(name):
             mtime = self.get_modified_time(name).isoformat()
         else:
             mtime = datetime.now().isoformat()
-        if ts is None:
-            ts = int(datetime.now().strftime("%s"))
-        full_msg = f"{name}//{mtime}@{ts}"
-
-        # Calculate a HMAC with the parts
-        token = hmac.new(
-            bytes(settings.SECRET_KEY, "utf-8"), msg=bytes(full_msg, "utf-8"), digestmod="sha256"
-        ).hexdigest() + hex(ts)[2:]
-        return token
+        return f"{name}//{mtime}"
+
+    def get_token(self, name: str) -> str:
+        """Get a token for a filename."""
+        return ":".join(self._signer.sign(self.get_token_message(name)).split(":")[-2:])
+
+    def verify_token(self, name: str, token: str):
+        """Verify a token for validity and timeout."""
+        return self._signer.unsign(":".join((self.get_token_message(name), token)), max_age=TIMEOUT)
```

### Comparing `django-titofisto-0.2.2/titofisto/test_settings.py` & `django_titofisto-1.0.0/titofisto/test_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 
 WSGI_APPLICATION = "titofisto_example.wsgi.application"
 
 USE_TZ = True
 
 MEDIA_ROOT = mkdtemp()
 MEDIA_URL = "/media/"
+
+TITOFISTO_ENABLE_UPLOAD = True
```

### Comparing `django-titofisto-0.2.2/titofisto/tests.py` & `django_titofisto-1.0.0/titofisto/tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 from io import BytesIO
 from pathlib import Path
 from unittest import TestCase
 
 from freezegun import freeze_time
 
 from django.conf import settings
+from django.core.files.uploadedfile import SimpleUploadedFile
+from django.http import HttpRequest, HttpResponse
 from django.test import Client
 
 from .storage import TitofistoStorage
+from .views import TitofistoUploadView
 
+test_file_1 = b"The quick brown fox jumps over the lazy dog"
+test_file_1_name = "quickfox.dat"
 
-class TitofistoTestCase(TestCase):
+
+class TitofistoMediaTestCase(TestCase):
     def setUp(self):
         self.storage = TitofistoStorage()
 
         self.test_file_1 = b"The quick brown fox jumps over the lazy dog"
         self.test_file_1_name = "quickfox.dat"
         self.storage.save(self.test_file_1_name, BytesIO(self.test_file_1))
 
@@ -33,116 +39,84 @@
 
     def tearDown(self):
         self.storage.delete(self.test_file_1_name)
         self.storage.delete(self.test_file_2_name)
 
     def test_token_deterministic(self):
         """The generated token is deterministic for a single, unchanged file"""
-        ts = int(datetime.now().strftime("%s"))
-
-        token_1 = self.storage.get_token(self.test_file_1_name, ts)
-        token_2 = self.storage.get_token(self.test_file_1_name, ts)
+        with freeze_time():
+            token_1 = self.storage.get_token(self.test_file_1_name)
+            token_2 = self.storage.get_token(self.test_file_1_name)
 
         self.assertEqual(token_1, token_2)
 
     def test_token_file_dependent(self):
         """The generated token is different for different files"""
-        ts = int(datetime.now().strftime("%s"))
-
-        token_1 = self.storage.get_token(self.test_file_1_name, ts)
-        token_2 = self.storage.get_token(self.test_file_2_name, ts)
+        with freeze_time():
+            token_1 = self.storage.get_token(self.test_file_1_name)
+            token_2 = self.storage.get_token(self.test_file_2_name)
 
         self.assertNotEqual(token_1, token_2)
 
     def test_token_ts_dependent(self):
         """The generated token is different for different timestamps"""
-        ts_1 = int(datetime.now().strftime("%s"))
-        ts_2 = ts_1 + 5
-
-        token_1 = self.storage.get_token(self.test_file_1_name, ts_1)
-        token_2 = self.storage.get_token(self.test_file_2_name, ts_2)
+        with freeze_time():
+            token_1 = self.storage.get_token(self.test_file_1_name)
+        with freeze_time():
+            token_2 = self.storage.get_token(self.test_file_2_name)
 
         self.assertNotEqual(token_1, token_2)
 
     def test_get_valid_token(self):
         """A file can be retrieved with a valid token"""
         token = self.storage.get_token(self.test_file_1_name)
 
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}={token}"
-        )
+        url = f"{settings.MEDIA_URL}{self.test_file_1_name}?" f"{self.param}={token}"
         res = self.client.get(url)
 
         self.assertEqual(res.status_code, 200)
         self.assertEqual(list(res.streaming_content)[0], self.test_file_1)
 
     def test_get_invalid_token(self):
         """A file can not be retrieved with an invalid token"""
         token = self.storage.get_token(self.test_file_1_name)
 
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}=a{token}"
-        )
-        res = self.client.get(url)
-
-        self.assertEqual(res.status_code, 404)
-
-    def test_get_invalid_ts(self):
-        """A file can not be retrieved with an invalid timestamp"""
-        token = self.storage.get_token(self.test_file_1_name)
-
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}={token}a"
-        )
+        url = f"{settings.MEDIA_URL}{self.test_file_1_name}?" f"{self.param}=a{token}"
         res = self.client.get(url)
 
         self.assertEqual(res.status_code, 404)
 
     def test_get_close_to_timeout(self):
         """A file can still be retrieved close to the timeout"""
         now = datetime.now()
-        token = self.storage.get_token(self.test_file_1_name, int(now.strftime("%s")))
-
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}={token}"
-        )
         with freeze_time(now + timedelta(seconds=self.timeout - 1)):
+            token = self.storage.get_token(self.test_file_1_name)
+            url = f"{settings.MEDIA_URL}{self.test_file_1_name}?" f"{self.param}={token}"
             res = self.client.get(url)
 
         self.assertEqual(res.status_code, 200)
         self.assertEqual(list(res.streaming_content)[0], self.test_file_1)
 
     def test_get_after_timeout(self):
         """A file can not be retrieved after the timeout"""
         now = datetime.now()
-        token = self.storage.get_token(self.test_file_1_name, int(now.strftime("%s")))
-
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}={token}"
-        )
+        with freeze_time(now):
+            token = self.storage.get_token(self.test_file_1_name)
+            url = f"{settings.MEDIA_URL}{self.test_file_1_name}?" f"{self.param}={token}"
         with freeze_time(now + timedelta(seconds=self.timeout + 1)):
             res = self.client.get(url)
 
         self.assertEqual(res.status_code, 404)
 
     def test_get_after_mtime_change(self):
         """A file can not be retrieved with the same token after its mtime changes"""
         now = datetime.now()
-        token = self.storage.get_token(self.test_file_1_name, int(now.strftime("%s")))
-
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_1_name}?"
-            f"{self.param}={token}"
-        )
         with freeze_time(now + timedelta(seconds=10)):
+            token = self.storage.get_token(self.test_file_1_name)
+            url = f"{settings.MEDIA_URL}{self.test_file_1_name}?" f"{self.param}={token}"
             Path(self.storage.path(self.test_file_1_name)).touch()
         res = self.client.get(url)
 
         self.assertEqual(res.status_code, 404)
 
     def test_url(self):
         """The URL for a file should contain a token."""
@@ -155,18 +129,80 @@
         """The URL for a file in the public namespace doesn't contain a token."""
         url = self.storage.url(self.test_file_3_name)
         self.assertNotIn(self.param, url)
 
     def test_public_files_view(self):
         """A file in the public namespace can be acessed without a token."""
         self.storage.url(self.test_file_3_name)
-        url = (
-            f"{settings.MEDIA_URL}{self.test_file_3_name}"
-        )
+        url = f"{settings.MEDIA_URL}{self.test_file_3_name}"
         res = self.client.get(url)
         self.assertEqual(res.status_code, 200)
 
     def test_404_not_found(self):
         """A 404 is returned for non-existent files."""
-        url = (f"{settings.MEDIA_URL}public/some_not_existing_file.txt")
+        url = f"{settings.MEDIA_URL}public/some_not_existing_file.txt"
         res = self.client.get(url)
         self.assertEqual(res.status_code, 404)
+
+
+def _upload_cb_test_1(request) -> HttpResponse:
+    file = request.FILES["file"]
+    assert file.name == test_file_1_name
+    assert file.read() == test_file_1
+
+    return HttpResponse(status=418)
+
+
+def _upload_cb_test_2(request, p1, p2, foo) -> HttpResponse:
+    assert p1 == "pos1"
+    assert p2 == "pos2"
+    assert foo == "bar"
+
+    file = request.FILES["file"]
+    assert file.name == test_file_1_name
+    assert file.read() == test_file_1
+
+    return HttpResponse(status=420)
+
+
+class TitofistoUploadTestCase(TestCase):
+    def setUp(self):
+        self.client = Client()
+
+    def test_upload_valid_slot_no_args(self):
+        upload_url = TitofistoUploadView.get_upload_slot("titofisto.tests._upload_cb_test_1")
+        res = self.client.post(
+            upload_url, data={"file": SimpleUploadedFile(test_file_1_name, test_file_1)}
+        )
+
+        assert res.status_code == 418
+
+    def test_upload_valid_slot_with_args(self):
+        upload_url = TitofistoUploadView.get_upload_slot(
+            "titofisto.tests._upload_cb_test_2", ("pos1", "pos2"), {"foo": "bar"}
+        )
+        res = self.client.post(
+            upload_url, data={"file": SimpleUploadedFile(test_file_1_name, test_file_1)}
+        )
+
+        assert res.status_code == 420
+
+    def test_upload_invalid_slot(self):
+        upload_url = TitofistoUploadView.get_upload_slot("titofisto.tests._upload_cb_test_1")
+        upload_url_mangled = upload_url[:-1] + "a/"
+        res = self.client.post(
+            upload_url_mangled, data={"file": SimpleUploadedFile(test_file_1_name, test_file_1)}
+        )
+
+        assert res.status_code == 404
+
+    def test_upload_valid_slot_twice(self):
+        upload_url = TitofistoUploadView.get_upload_slot("titofisto.tests._upload_cb_test_1")
+        res1 = self.client.post(
+            upload_url, data={"file": SimpleUploadedFile(test_file_1_name, test_file_1)}
+        )
+        res2 = self.client.post(
+            upload_url, data={"file": SimpleUploadedFile(test_file_1_name, test_file_1)}
+        )
+
+        assert res1.status_code == 418
+        assert res2.status_code == 404
```

### Comparing `django-titofisto-0.2.2/PKG-INFO` & `django_titofisto-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: django-titofisto
-Version: 0.2.2
+Version: 1.0.0
 Summary: Django Time-Token File Storage
 Home-page: https://edugit.org/AlekSIS/libs/django-titofisto
 License: Apache-2.0
 Keywords: django,storage,media,secure
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>2.2,<5.0)
+Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
 Project-URL: Repository, https://edugit.org/AlekSIS/libs/django-titofisto
 Description-Content-Type: text/x-rst
 
 Django Time-Token File Storage
 ==============================
 
 This is a simple extension to Django's `FileSystemStorage` that adds a URL
 parameter carrying a shared token, which is only valid for a defined period
 of time.
 
+Additionally, a like-wise time-constrained file upload slot mechanism is
+available.
+
 Functionality
 -------------
 
+File storage with token-secured URLs
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 This is a drop-in replacement for the Django `FileSystemStorage`, usable if
 media files are served by Django itself. It does currently not work if media
 files are served from an independent web server.
 
 The storage and its accompanying view do the following:
 
 * When a URL to a storage file is generated, a HMAC-based token is generated
@@ -40,22 +49,34 @@
   parameters to the URL
 * Upon retrieval of the file through the accompanying view, the requested
   file name and the passed timestamp are used to recalculate the HMAC-based
   token
 * Only if the tokens match, and a configured timeout has not passed, is the
   file served
 
-The HMAC-based token ensures that the token is invalidated when:
+The signature-based token ensures that the token is invalidated when:
 
 * The filename changes
 * The timestamp changes
 * The mtime of the file changes
 * The `SECRET_KEY` changes
 
-The HMAC is salted with the `SECRET_KEY`.
+Time-constrained uplaod slot
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The upload slot mechanism can be used to generically handle file uploads
+by clients that can not upload files with a regular request. One example
+for this is a client using GraphQL to talk to Django, because GraphQL
+does not support file uploads and rather suggests to do uplaods
+out-of-band.
+
+With Titofisto's upload slot mechanism, calling code can request a secure
+URL which it can hand out to a client. When the client POSTs its file
+to the endpoint, a previously provided callback is called to handle the
+uploaded file.
 
 Installation
 ------------
 
 To add `django-titofisto`_ to a project, first add it as dependency to your
 project, e.g. using `poetry`_::
 
@@ -84,26 +105,52 @@
 
 Provide public media files
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Sometimes, there might be media files, for example favicons,
 you want to be accessible without any authentication. Per default,
 `django-titofisto` will serve all files stored in the directory `public` without a token.
-You can disable or configure this behavior using these settings:
+You can disable or configure this behavior using these settings::
 
   TITOFISTO_USE_PUBLIC_NAMESPACE = True # optional, this is the default
   TITOFISTO_PUBLIC_NAMESPACE = "public/" # optional, this is the default
 
+Use the time-constrained upload slot
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To enable the file upload mechanism, a setting must be set, because the
+default `upload/` prefix could potentially shadow expected media file
+URLs::
+
+  TITOFISTO_ENABLE_UPLOAD = True
+  TITOFISTO_UPLOAD_NAMESPACE = "titofisto/upload/"
+
+A simplified example for using the upload slot mechanism is::
+
+  from titofisto.views import TitofistoUploadView
+
+  def handle_file(request, pk):
+      instance = MyModel.objects.get(pk=pk)
+      instance.photo = request.FILES["photo"]
+      instance.save()
+
+  # This gets an uplaod URL to pass on to the client
+  # On upload, the handler above will be called, with 15 as positional argument
+  upload_url = TitofistoUploadView.get_upload_slot(
+      "mymodule.handle_file",
+      (15,)
+  )
+
 Credits
 -------
 
 `django-titofisto` was developed for the `AlekSIS`_ school information system by
-its team.
+its team::
 
-  Copyright © 2021 Dominik George <dominik.george@teckids.org>
+  Copyright © 2021, 2023 Dominik George <dominik.george@teckids.org>
   Copyright © 2021 Jonathan Weth <dev@jonathanweth.de>
 
 .. _django-titofisto: https://edugit.org/AlekSIS/libs/django-titofisto
 .. _poetry: https://python-poetry.org/
 .. _Django's cache framework: https://docs.djangoproject.com/en/3.2/topics/cache/
 .. _AlekSIS: https://aleksis.org/
```

