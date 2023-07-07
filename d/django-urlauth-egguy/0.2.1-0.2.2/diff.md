# Comparing `tmp/django_urlauth_egguy-0.2.1.tar.gz` & `tmp/django_urlauth_egguy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_urlauth_egguy-0.2.1.tar", max compression
+gzip compressed data, was "django_urlauth_egguy-0.2.2.tar", max compression
```

## Comparing `django_urlauth_egguy-0.2.1.tar` & `django_urlauth_egguy-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1484 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/LICENSE
--rw-r--r--   0        0        0      498 2023-07-06 05:03:08.515771 django_urlauth_egguy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/__init__.py
--rw-r--r--   0        0        0      197 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/admin.py
--rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/management/commands/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/management/commands/urlauth_cleanup.py
--rw-r--r--   0        0        0     1433 2023-07-06 04:45:25.609095 django_urlauth_egguy-0.2.1/urlauth/middleware.py
--rw-r--r--   0        0        0      768 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/migrations/__init__.py
--rw-r--r--   0        0        0     3359 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/models.py
--rw-r--r--   0        0        0       76 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/settings.py
--rw-r--r--   0        0        0      106 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/signals.py
--rw-r--r--   0        0        0     6329 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/tests.py
--rw-r--r--   0        0        0      760 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.1/urlauth/util.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 django_urlauth_egguy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1484 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.2/LICENSE
+-rw-r--r--   0        0        0      511 2023-07-07 07:32:16.738666 django_urlauth_egguy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.2/urlauth/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/admin.py
+-rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.2/urlauth/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.2/urlauth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1531 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/management/commands/urlauth_cleanup.py
+-rw-r--r--   0        0        0     1359 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/middleware.py
+-rw-r--r--   0        0        0      821 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-06 04:43:42.988766 django_urlauth_egguy-0.2.2/urlauth/migrations/__init__.py
+-rw-r--r--   0        0        0     3144 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/models.py
+-rw-r--r--   0        0        0       76 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/settings.py
+-rw-r--r--   0        0        0      106 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/signals.py
+-rw-r--r--   0        0        0     6029 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/tests.py
+-rw-r--r--   0        0        0      705 2023-07-07 07:28:44.960580 django_urlauth_egguy-0.2.2/urlauth/util.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 django_urlauth_egguy-0.2.2/PKG-INFO
```

### Comparing `django_urlauth_egguy-0.2.1/LICENSE` & `django_urlauth_egguy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_urlauth_egguy-0.2.1/urlauth/management/commands/urlauth_cleanup.py` & `django_urlauth_egguy-0.2.2/urlauth/management/commands/urlauth_cleanup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from datetime import datetime
 
 from django.core.management.base import BaseCommand
 from django.db import transaction
 from django.db.models.sql.subqueries import DeleteQuery
 
 from urlauth.models import AuthKey
 
+
 def truncate_queryset(qs):
     """
     Deletes all records matched by queryset using
 
         DELETE from table WHERE <condition>
 
     query without fetching PK values for all items in original queryset
@@ -34,21 +34,19 @@
         else:
             transaction.commit_unless_managed(using=qs.db)
     finally:
         if forced_managed:
             transaction.leave_transaction_management(using=qs.db)
 
 
-
-
 class Command(BaseCommand):
-    help = 'Remove expired keys from database'
+    help = "Remove expired keys from database"
 
     def handle(self, *args, **kwargs):
         qs = AuthKey.objects.filter(expired__lt=datetime.now())
         count = qs.count()
 
         # qs.delete() is grossly inefficient for larger querysets
         # and there can be a *LOT* of AuthKey's
         truncate_queryset(qs)
 
-        print('%d keys deleted' % count)
+        print("%d keys deleted" % count)
```

### Comparing `django_urlauth_egguy-0.2.1/urlauth/migrations/0001_initial.py` & `django_urlauth_egguy-0.2.2/urlauth/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 # Generated by Django 1.11.29 on 2020-09-16 09:49
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='AuthKey',
+            name="AuthKey",
             fields=[
-                ('id', models.CharField(max_length=40, primary_key=True, serialize=False)),
-                ('uid', models.PositiveIntegerField(null=True)),
-                ('expired', models.DateTimeField()),
-                ('created', models.DateTimeField(auto_now_add=True)),
-                ('onetime', models.BooleanField(default=True)),
-                ('data', models.TextField()),
+                (
+                    "id",
+                    models.CharField(max_length=40, primary_key=True, serialize=False),
+                ),
+                ("uid", models.PositiveIntegerField(null=True)),
+                ("expired", models.DateTimeField()),
+                ("created", models.DateTimeField(auto_now_add=True)),
+                ("onetime", models.BooleanField(default=True)),
+                ("data", models.TextField()),
             ],
         ),
     ]
```

### Comparing `django_urlauth_egguy-0.2.1/urlauth/models.py` & `django_urlauth_egguy-0.2.2/urlauth/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,24 @@
-from builtins import range
-from urlauth.settings import URLAUTH_AUTHKEY_NAME, URLAUTH_AUTHKEY_TIMEOUT
-import os
-from binascii import hexlify
+import json
 from datetime import datetime, timedelta
+from uuid import uuid4
 
-try:
-    from django.contrib.auth import get_user_model
-    #User = get_user_model()
-    get_user = lambda: get_user_model()
-except ImportError:
-    from django.contrib.auth.models import User
-    get_user = lambda: User
-
-from django.db import models
 from django.conf import settings
-try:
-    # load simple json compat from django
-    from django.utils import simplejson as json
-except ImportError:
-    import json
+from django.contrib.auth import get_user_model
+from django.db import models
 from django.db.utils import IntegrityError
-from uuid import uuid4
+
+from urlauth.settings import URLAUTH_AUTHKEY_NAME, URLAUTH_AUTHKEY_TIMEOUT
 
 
 class URLAuthError(Exception):
     pass
 
 
 class AuthKeyManager(models.Manager):
-
     def create_key(self, uid, expired=None, onetime=True, **kwargs):
         """
         Create AuthKey object and return its ID.
         :param uid: The uid of the user to automatically log
         :param expired: (default:  datetime.now() + timedelta(seconds=settings.URLAUTH_AUTHKEY_TIMEOUT)) datetime.now() + time delta to specify when the key must expire
         :param ontime: (default: True) Generate a one time key
         :param kwargs: others arguments
@@ -40,70 +26,80 @@
         """
 
         key = AuthKey()
         key.uid = uid
         if expired:
             key.expired = expired
         else:
-            key.expired = datetime.now() + timedelta(seconds=getattr(settings, "URLAUTH_AUTHKEY_TIMEOUT", URLAUTH_AUTHKEY_TIMEOUT))
+            key.expired = datetime.now() + timedelta(
+                seconds=getattr(
+                    settings, "URLAUTH_AUTHKEY_TIMEOUT", URLAUTH_AUTHKEY_TIMEOUT
+                )
+            )
 
         key.onetime = onetime
         key.data = json.dumps(kwargs)
 
         # Try 10 times to create AuthKey instance with unique PK
-        for x in range(10):
+        for _ in range(10):
             key.pk = uuid4()  # Use a unique identifier
             try:
                 key.save(force_insert=True)
             except IntegrityError:
                 key.pk = None
             else:
                 break
 
         if not key.pk:
-            raise URLAuthError('Could not create unique key')
+            raise URLAuthError("Could not create unique key")
 
         return key.id
 
     def wrap_url(self, url, uid, **kwargs):
         """
         Create new authorization key, append it to the url and return modified url.
         :param url: The url to wrap
         :param uid: id of the user to log
         :param kwargs: others params used byt create_key
         :return: An url wrapped with an unique key
         """
 
         key_id = self.create_key(uid, **kwargs)
-        clue = '?' in url and '&' or '?'
-        parts = url.rsplit('#', 1)
+        clue = "?" in url and "&" or "?"
+        parts = url.rsplit("#", 1)
         if len(parts) > 1:
             url, hash = parts
-            hash = '#%s' % hash
+            hash = "#%s" % hash
         else:
-            hash = ''
-        url = '%s%s%s=%s%s' % (url, clue, getattr(settings, "URLAUTH_AUTHKEY_NAME", URLAUTH_AUTHKEY_NAME), key_id, hash)
+            hash = ""
+        url = "{}{}{}={}{}".format(
+            url,
+            clue,
+            getattr(settings, "URLAUTH_AUTHKEY_NAME", URLAUTH_AUTHKEY_NAME),
+            key_id,
+            hash,
+        )
         return url
 
 
 class AuthKey(models.Model):
     id = models.CharField(max_length=40, primary_key=True)
     uid = models.PositiveIntegerField(null=True)
     expired = models.DateTimeField()
     created = models.DateTimeField(auto_now_add=True)
     onetime = models.BooleanField(blank=True, default=True)
     data = models.TextField()
 
     objects = AuthKeyManager()
 
-    def __unicode__(self):
-        return 'AuthKey #%s' % self.id
+    def __str__(self):
+        return "AuthKey #%s" % self.id
 
     @property
     def extra(self):
         return json.loads(self.data)
 
     def get_user(self):
         if self.uid:
-            return get_user().objects.get(pk=self.uid)
+            return get_user_model().objects.get(pk=self.uid)
         else:
             return None
```

### Comparing `django_urlauth_egguy-0.2.1/urlauth/tests.py` & `django_urlauth_egguy-0.2.2/urlauth/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,172 +1,176 @@
-from builtins import range
-from datetime import datetime, timedelta
 import cgi
+from datetime import datetime, timedelta
 
 from django.conf.urls import url
-from django.test import TestCase
+from django.contrib.auth import get_user_model
 from django.http import HttpResponse
-from django.conf import settings
-from urlauth.settings import URLAUTH_AUTHKEY_NAME
-
-try:
-    from django.contrib.auth import get_user_model
-    User = get_user_model()
-except ImportError:
-    from django.contrib.auth.models import User
+from django.test import TestCase
 
-from urlauth.util import load_key, InvalidKey
 from urlauth.models import AuthKey
+from urlauth.settings import URLAUTH_AUTHKEY_NAME
 from urlauth.signals import authkey_processed
+from urlauth.util import InvalidKey, load_key
+
+User = get_user_model()
 
 
 class UrlauthTestCase(TestCase):
-    urls = 'urlauth.tests'
-    test_url = '/urlauth_test_view/'
+    urls = "urlauth.tests"
+    test_url = "/urlauth_test_view/"
 
     # Helpers
     def setUp(self):
         """
         Create active and inactive users.
         """
 
         User.objects.all().delete()
-        self.user = User.objects.create_user('user', 'user@host.com', 'pass')
-        self.ban_user = User.objects.create_user('ban_user', 'ban_user@host.com',
-                                                 'pass')
+        self.user = User.objects.create_user("user", "user@host.com", "pass")
+        self.ban_user = User.objects.create_user(
+            "ban_user", "ban_user@host.com", "pass"
+        )
         self.ban_user.is_active = False
         self.ban_user.save()
 
     def process_url(self, url, **kwargs):
         """
         Add authkey to the ``url`` and then open that url with django test client.
 
         Returns:
             The ID of created ``AuthKey`` instance
         """
 
         url = AuthKey.objects.wrap_url(url, **kwargs)
-        path, args = url.split('?')[0], cgi.parse_qs(url.split('?')[1])
+        path, args = url.split("?")[0], cgi.parse_qs(url.split("?")[1])
         self.client.get(url, args)
         return args[URLAUTH_AUTHKEY_NAME][0]
 
     # Test cases
 
     def test_create_key(self):
         "Test the create_key function"
-        self.assertTrue(AuthKey.objects.create_key(uid=self.user.pk,
-                                                   expired=datetime.now()))
+        self.assertTrue(
+            AuthKey.objects.create_key(uid=self.user.pk, expired=datetime.now())
+        )
 
     def test_wrap_url(self):
         "Test the wrap_url function"
         expired = datetime.now()
 
         AuthKey.objects.all().delete()
-        clean_url = 'http://ya.ru'
+        clean_url = "http://ya.ru"
         url = AuthKey.objects.wrap_url(clean_url, uid=self.user.pk, expired=expired)
         key = AuthKey.objects.get()
-        self.assertEqual(url, '%s?%s=%s' % (clean_url,
-                                            URLAUTH_AUTHKEY_NAME, key.id))
+        self.assertEqual(
+            url, "{}?{}={}".format(clean_url, URLAUTH_AUTHKEY_NAME, key.id)
+        )
 
         AuthKey.objects.all().delete()
-        clean_url = 'http://ya.ru?foo=bar'
+        clean_url = "http://ya.ru?foo=bar"
         url = AuthKey.objects.wrap_url(clean_url, uid=self.user.pk, expired=expired)
         key = AuthKey.objects.get()
-        self.assertEqual(url, '%s&%s=%s' % (clean_url,
-                                            URLAUTH_AUTHKEY_NAME, key.id))
+        self.assertEqual(
+            url, "{}&{}={}".format(clean_url, URLAUTH_AUTHKEY_NAME, key.id)
+        )
 
         # Test url with hash
         AuthKey.objects.all().delete()
-        clean_url = 'http://ya.ru#hash'
+        clean_url = "http://ya.ru#hash"
         url = AuthKey.objects.wrap_url(clean_url, uid=self.user.pk, expired=expired)
         key = AuthKey.objects.get()
-        self.assertEqual(url, 'http://ya.ru?%s=%s#hash' % (URLAUTH_AUTHKEY_NAME,
-                                                           key.id))
+        self.assertEqual(
+            url, "http://ya.ru?{}={}#hash".format(URLAUTH_AUTHKEY_NAME, key.id)
+        )
 
         # Test url with hash and non-empty querystring
         AuthKey.objects.all().delete()
-        clean_url = 'http://ya.ru?foo=bar#hash'
+        clean_url = "http://ya.ru?foo=bar#hash"
         url = AuthKey.objects.wrap_url(clean_url, uid=self.user.pk, expired=expired)
         key = AuthKey.objects.get()
-        self.assertEqual(url, 'http://ya.ru?foo=bar&%s=%s#hash' % (URLAUTH_AUTHKEY_NAME,
-                                                                   key.id))
+        self.assertEqual(
+            url, "http://ya.ru?foo=bar&{}={}#hash".format(URLAUTH_AUTHKEY_NAME, key.id)
+        )
 
     def test_validate_key(self):
         "Test the validate_key function"
         expired = datetime.now() - timedelta(seconds=1)
-        key = AuthKey.objects.create_key(uid=self.user.pk, expired=expired, foo='bar')
+        key = AuthKey.objects.create_key(uid=self.user.pk, expired=expired, foo="bar")
         self.assertRaises(InvalidKey, lambda: load_key(key))
 
         expired = datetime.now() + timedelta(seconds=10)
         key = AuthKey.objects.create_key(uid=self.user.pk, expired=expired)
         self.assertTrue(load_key(key))
 
     def test_authentication(self):
         "Test the authentication middleware"
         expired = datetime.now() + timedelta(days=1)
         resp = self.client.get(self.test_url)
 
         # Guest is not authenticated
         self.client.logout()
-        self.assertFalse('_auth_user_id' in self.client.session)
+        self.assertFalse("_auth_user_id" in self.client.session)
 
         ## Simple authorization
         self.client.logout()
         self.process_url(self.test_url, uid=self.user.pk, expired=expired)
-        self.assertEqual(self.client.session['_auth_user_id'], self.user.pk)
+        # self.assertEqual(self.client.session, self.user.pk)
+
+        self.assertEqual(self.client.session["_auth_user_id"], str(self.user.pk))
 
         ## Baned user can't authorize
         self.client.logout()
         self.process_url(self.test_url, uid=self.ban_user.pk, expired=expired)
-        self.assertFalse('_auth_user_id' in self.client.session)
+        self.assertFalse("_auth_user_id" in self.client.session)
 
         ## Expired auth key does not work
         self.client.logout()
         expired = datetime.now() - timedelta(seconds=1)
         self.process_url(self.test_url, uid=self.user.pk, expired=expired)
-        self.assertFalse('_auth_user_id' in self.client.session)
+        self.assertFalse("_auth_user_id" in self.client.session)
 
     def test_signals(self):
         logs = []
 
-        handler = lambda **k: logs.append('X')
+        def handler(**k):
+            return logs.append("X")
 
         authkey_processed.connect(handler)
 
         self.assertEqual(0, len(logs))
         self.client.logout()
         expired = datetime.now() + timedelta(days=1)
         self.process_url(self.test_url, uid=self.user.pk, expired=expired)
         self.assertEqual(1, len(logs))
 
     def test_onetime_feature(self):
         self.client.logout()
         expired = datetime.now() + timedelta(days=1)
-        hash = self.process_url(self.test_url, uid=self.user.pk,
-                                expired=expired)
+        hash = self.process_url(self.test_url, uid=self.user.pk, expired=expired)
         self.assertFalse(AuthKey.objects.filter(id=hash).count())
 
         self.client.logout()
         expired = datetime.now() + timedelta(days=1)
-        hash = self.process_url(self.test_url, uid=self.user.pk,
-                                expired=expired, onetime=False)
+        hash = self.process_url(
+            self.test_url, uid=self.user.pk, expired=expired, onetime=False
+        )
         self.assertTrue(AuthKey.objects.filter(id=hash).count())
 
     def test_bulk(self):
         User.objects.all().delete()
         AuthKey.objects.all().delete()
         for x in range(100):
-            username = 'test%d' % x
-            User.objects.create_user(username, '%s@gmail.com' % username, username)
+            username = "test%d" % x
+            User.objects.create_user(username, "%s@gmail.com" % username, username)
         users = User.objects.all()
         for user in users:
-            obj = AuthKey.objects.wrap_url('/', uid=user.pk)
+            obj = AuthKey.objects.wrap_url("/", uid=user.pk)
         self.assertEqual(User.objects.count(), AuthKey.objects.count())
 
 
 def test_view(request):
-    return HttpResponse('')
+    return HttpResponse("")
 
 
 urlpatterns = [
-                       url('urlauth_test_view/', test_view, name='urlauth_test_view'),
-               ]
+    url("urlauth_test_view/", test_view, name="urlauth_test_view"),
+]
```

### Comparing `django_urlauth_egguy-0.2.1/PKG-INFO` & `django_urlauth_egguy-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-urlauth-egguy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django application for user authentication with key in hypertext link
 License: BSD
 Author: egguy
 Author-email: etienne.guilluy@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=1.11)
-Requires-Dist: future (>=0.18.2,<0.19.0)
```

