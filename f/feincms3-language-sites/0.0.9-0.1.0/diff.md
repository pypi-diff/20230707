# Comparing `tmp/feincms3_language_sites-0.0.9.tar.gz` & `tmp/feincms3_language_sites-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feincms3_language_sites-0.0.9.tar", last modified: Thu Mar  3 14:03:41 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `feincms3_language_sites-0.0.9.tar` & `feincms3_language_sites-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,38 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.044394 feincms3_language_sites-0.0.9/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-03-03 12:26:38.000000 feincms3_language_sites-0.0.9/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      211 2022-03-03 12:26:38.000000 feincms3_language_sites-0.0.9/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4526 2022-03-03 14:03:41.044394 feincms3_language_sites-0.0.9/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3444 2022-03-03 13:40:02.000000 feincms3_language_sites-0.0.9/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.040394 feincms3_language_sites-0.0.9/feincms3_language_sites/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2022-03-03 14:03:26.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1088 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/checks.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.040394 feincms3_language_sites-0.0.9/feincms3_language_sites/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.040394 feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.040394 feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      880 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1170 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1740 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/middleware.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4120 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/models.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.044394 feincms3_language_sites-0.0.9/feincms3_language_sites/templatetags/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-03-03 13:51:21.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/templatetags/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      662 2022-03-03 14:01:02.000000 feincms3_language_sites-0.0.9/feincms3_language_sites/templatetags/feincms3_language_sites.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-03 14:03:41.040394 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4526 2022-03-03 14:03:40.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      696 2022-03-03 14:03:41.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-03-03 14:03:40.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-03-03 12:27:44.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       59 2022-03-03 14:03:40.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       24 2022-03-03 14:03:41.000000 feincms3_language_sites-0.0.9/feincms3_language_sites.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1374 2022-03-03 14:03:41.044394 feincms3_language_sites-0.0.9/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-03-03 12:26:38.000000 feincms3_language_sites-0.0.9/setup.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/.editorconfig
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tox.ini
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/checks.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/middleware.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/models.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/templatetags/__init__.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/feincms3_language_sites/templatetags/feincms3_language_sites.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/.gitignore
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/admin.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/application_urls.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/models.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/settings.py
+-rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/test_feincms3.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/urls.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/views.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/404.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/base.html
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/snippet.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/pages/standard.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/pages/with-sidebar.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/renderer/html.html
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/testapp/article_detail.html
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/tests/testapp/templates/testapp/article_list.html
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/README.rst
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 feincms3_language_sites-0.1.0/PKG-INFO
```

### Comparing `feincms3_language_sites-0.0.9/LICENSE` & `feincms3_language_sites-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_language_sites-0.0.9/PKG-INFO` & `feincms3_language_sites-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
-Name: feincms3_language_sites
-Version: 0.0.9
+Name: feincms3-language-sites
+Version: 0.1.0
 Summary: Multisite support for feincms3
-Home-page: https://github.com/matthiask/feincms3-language-sites/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
+Project-URL: Homepage, https://github.com/matthiask/feincms3-language-sites/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
-Platform: OS Independent
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Dist: django>=3.2
+Requires-Dist: feincms3>=0.92
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Requires-Dist: feincms3[all]; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 =======================
 feincms3-language-sites
 =======================
 
 .. image:: https://github.com/matthiask/feincms3-language-sites/workflows/Tests/badge.svg
     :target: https://github.com/matthiask/feincms3-language-sites/
@@ -90,20 +92,21 @@
     }
 
 Sites are checked in the order they are declared (since dictionaries are
 guaranteed to preserve the ordering of keys since Python 3.7).
 
 The keys of the ``SITES`` dictionary have to be equal to all language codes in
 ``LANGUAGES``. The ``host`` is required and should only consist of the host and
-an optional port, nothing else. The ``host_re`` is automatically derived from
-``host`` if it isn't given explicitly and is matched against
-``request.get_host()`` to find the current site. If no ``host_re`` matches the
-``site_middleware`` automatically raises a ``DisallowedHost`` exception (which
-produces the same error as Django if the request doesn't match
-``ALLOWED_HOSTS``).
+an optional port, nothing else. If ``host_re`` is given the
+``request.get_host()`` return value is matched against the ``host_re`` regular
+expression, otherwise the ``host`` has to match exactly.
+
+The ``site_middleware`` automatically raises a ``DisallowedHost`` exception if
+no site matches the current request (which produces the same error as Django if
+the request doesn't match ``ALLOWED_HOSTS``).
 
 
 Utilities
 =========
 
 * ``feincms3_language_sites.models.site_for_host``
 * ``feincms3_language_sites.models.reverse_language_site_app``
@@ -113,9 +116,7 @@
 Notes
 =====
 
 Note that ``Page.objects.active()`` only returns pages in the current language.
 If you want to generate translation links (e.g. using ``...|translations`` in a
 template) you do not want to use the ``.active()`` queryset method but build
 something yourself which runs ``.filter(is_active=True)``.
-
-
```

### Comparing `feincms3_language_sites-0.0.9/README.rst` & `feincms3_language_sites-0.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -62,20 +62,21 @@
     }
 
 Sites are checked in the order they are declared (since dictionaries are
 guaranteed to preserve the ordering of keys since Python 3.7).
 
 The keys of the ``SITES`` dictionary have to be equal to all language codes in
 ``LANGUAGES``. The ``host`` is required and should only consist of the host and
-an optional port, nothing else. The ``host_re`` is automatically derived from
-``host`` if it isn't given explicitly and is matched against
-``request.get_host()`` to find the current site. If no ``host_re`` matches the
-``site_middleware`` automatically raises a ``DisallowedHost`` exception (which
-produces the same error as Django if the request doesn't match
-``ALLOWED_HOSTS``).
+an optional port, nothing else. If ``host_re`` is given the
+``request.get_host()`` return value is matched against the ``host_re`` regular
+expression, otherwise the ``host`` has to match exactly.
+
+The ``site_middleware`` automatically raises a ``DisallowedHost`` exception if
+no site matches the current request (which produces the same error as Django if
+the request doesn't match ``ALLOWED_HOSTS``).
 
 
 Utilities
 =========
 
 * ``feincms3_language_sites.models.site_for_host``
 * ``feincms3_language_sites.models.reverse_language_site_app``
```

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/checks.py` & `feincms3_language_sites-0.1.0/feincms3_language_sites/checks.py`

 * *Files identical despite different names*

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/LC_MESSAGES/django.mo` & `feincms3_language_sites-0.1.0/feincms3_language_sites/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/locale/de/LC_MESSAGES/django.po` & `feincms3_language_sites-0.1.0/feincms3_language_sites/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/middleware.py` & `feincms3_language_sites-0.1.0/feincms3_language_sites/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.conf import settings
 from django.core.exceptions import DisallowedHost, ImproperlyConfigured
 from django.http import HttpResponsePermanentRedirect
 from django.utils import translation
 
 
 def site_middleware(get_response):
-    from .models import site_for_host
+    from feincms3_language_sites.models import site_for_host
 
     def middleware(request):
         request.site = site_for_host(request.get_host())
         if request.site is None:
             raise DisallowedHost("No configuration found for %r" % request.get_host())
 
         translation.activate(request.site["language_code"])
```

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/models.py` & `feincms3_language_sites-0.1.0/feincms3_language_sites/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from django.core.validators import RegexValidator
 from django.db import models
 from django.utils.translation import get_language, gettext_lazy as _
 from feincms3 import applications, pages
 from feincms3.applications import apps_urlconf, reverse_app
 from feincms3.mixins import LanguageAndTranslationOfMixin
 
-import feincms3_language_sites.checks  # noqa
+import feincms3_language_sites.checks  # noqa: F401
+
+
+def _protocol():
+    return "https:" if settings.SECURE_SSL_REDIRECT else "http:"
 
 
 def site_for_host(host):
     for language_code, site in settings.SITES.items():
         site.setdefault("language_code", language_code)
         if "host_re" in site:
             if re.search(site["host_re"], host):
@@ -34,34 +38,37 @@
     if not urlconf_map or any(
         module for module in urlconf_map.values() if module not in sys.modules
     ):
         fields = ("path", "page_type", "app_namespace", "language_code")
         apps = {code: [] for code, name in settings.LANGUAGES}
         for app in (
             applications._APPS_MODEL._default_manager.filter(is_active=True)
-            .with_tree_fields(False)
+            .without_tree_fields()
             .exclude(app_namespace="")
             .values_list(*fields)
             .order_by(*fields)
         ):
+            # Skip apps with languages not in LANGUAGES
+            if app[-1] not in apps:
+                continue
             apps[app[-1]].append(app)
 
         urlconf_map = {
             code: apps_urlconf(apps=site_apps) for code, site_apps in apps.items()
         }
         cache.set(CACHE_KEY, urlconf_map, timeout=CACHE_TIMEOUT)
     return urlconf_map
 
 
 def reverse_language_site_app(*args, **kwargs):
     language_code = get_language()
     kwargs["urlconf"] = apps_urlconfs()[language_code]
     url = reverse_app(*args, **kwargs, languages=[language_code])
     host = settings.SITES[language_code]["host"]
-    return f"//{host}{url}"
+    return f"{_protocol()}//{host}{url}"
 
 
 class AbstractPageQuerySet(pages.AbstractPageQuerySet):
     def active(self, *, language_code=None):
         return self.filter(
             is_active=True, language_code=language_code or get_language()
         )
@@ -119,8 +126,8 @@
     @property
     def site(self):
         return settings.SITES[self.language_code]
 
     def get_absolute_url(self):
         host = self.site["host"]
         url = super().get_absolute_url()
-        return f"//{host}{url}"
+        return f"{_protocol()}//{host}{url}"
```

### Comparing `feincms3_language_sites-0.0.9/feincms3_language_sites/templatetags/feincms3_language_sites.py` & `feincms3_language_sites-0.1.0/feincms3_language_sites/templatetags/feincms3_language_sites.py`

 * *Files identical despite different names*

