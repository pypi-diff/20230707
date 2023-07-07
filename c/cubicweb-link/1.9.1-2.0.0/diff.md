# Comparing `tmp/cubicweb-link-1.9.1.tar.gz` & `tmp/cubicweb-link-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-link-1.9.1.tar", last modified: Fri Nov 22 14:42:56 2019, max compression
+gzip compressed data, was "cubicweb-link-2.0.0.tar", last modified: Fri Jul  7 12:59:19 2023, max compression
```

## Comparing `cubicweb-link-1.9.1.tar` & `cubicweb-link-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      277 2019-11-22 09:14:44.000000 cubicweb-link-1.9.1/MANIFEST.in
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      531 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       88 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/README
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       20 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/__init__.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      593 2019-11-22 14:41:47.000000 cubicweb-link-1.9.1/cubicweb_link/__pkginfo__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      288 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/data/icon_link.gif
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      488 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/entities.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      923 2019-11-20 12:43:51.000000 cubicweb-link-1.9.1/cubicweb_link/hooks.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link/i18n/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1464 2019-11-20 12:43:51.000000 cubicweb-link-1.9.1/cubicweb_link/i18n/en.po
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1684 2019-11-20 12:43:51.000000 cubicweb-link-1.9.1/cubicweb_link/i18n/fr.po
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link/migration/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       32 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/migration/1.7.0_Any.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       66 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/migration/postcreate.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      479 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/schema.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       48 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/uiprops.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2802 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/cubicweb_link/views.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      531 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      695 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       39 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       17 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       14 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/cubicweb_link.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2606 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/test/
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 14:42:56.000000 cubicweb-link-1.9.1/test/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        5 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/test/data/bootstrap_cubes
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      311 2019-03-05 13:46:12.000000 cubicweb-link-1.9.1/test/test_link.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     3067 2019-11-20 12:43:51.000000 cubicweb-link-1.9.1/test/unittest_link.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      507 2019-11-22 09:10:20.000000 cubicweb-link-1.9.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.754998 cubicweb-link-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-07 12:59:19.750998 cubicweb-link-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.714998 cubicweb-link-2.0.0/cubicweb_link/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.722998 cubicweb-link-2.0.0/cubicweb_link/data/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/data/icon_link.gif
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.726998 cubicweb-link-2.0.0/cubicweb_link/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.730998 cubicweb-link-2.0.0/cubicweb_link/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/migration/1.7.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/cubicweb_link/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.722998 cubicweb-link-2.0.0/cubicweb_link.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-07 12:59:19.000000 cubicweb-link-2.0.0/cubicweb_link.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 12:59:19.754998 cubicweb-link-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.730998 cubicweb-link-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:59:19.746998 cubicweb-link-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/test/test_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/test/unittest_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2023-07-07 12:58:08.000000 cubicweb-link-2.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-link-1.9.1/cubicweb_link/hooks.py` & `cubicweb-link-2.0.0/cubicweb_link/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from cubicweb.predicates import is_instance
 from cubicweb.sobjects.notification import ContentAddedView
 from cubicweb.server.hook import Hook
 
 
 class LinkAddedView(ContentAddedView):
     """get notified from new links"""
-    __select__ = is_instance('Link')
-    content_attr = 'description'
+
+    __select__ = is_instance("Link")
+    content_attr = "description"
 
 
 class NoDuplicateHook(Hook):
-    """ Before adding/updating a link, check that the URL is not already in the
+    """Before adding/updating a link, check that the URL is not already in the
     database.
     """
 
     __regid__ = "link_no_duplicate_hook"
     __select_ = Hook.__select__ & is_instance("Link")
     events = ("before_add_entity", "before_update_entity")
```

### Comparing `cubicweb-link-1.9.1/cubicweb_link/i18n/en.po` & `cubicweb-link-2.0.0/cubicweb_link/i18n/en.po`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 msgid "New Link"
 msgstr "New link"
 
 msgid "This Link"
 msgstr "This link"
 
-
-msgid "This URL is already existing"
-msgstr ""
-
 msgid "a link to an external internet resource"
 msgstr ""
 
 # subject and object forms for each relation type
 # (no object form for final or symetric relation types)
 msgctxt "Link"
 msgid "description"
```

### Comparing `cubicweb-link-1.9.1/cubicweb_link/i18n/fr.po` & `cubicweb-link-2.0.0/cubicweb_link/i18n/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 msgid "New Link"
 msgstr "Nouveau lien"
 
 msgid "This Link"
 msgstr "Ce lien"
 
-
-msgid "This URL is already existing"
-msgstr "Cette URL existe déjà"
-
 msgid "a link to an external internet resource"
 msgstr "un lien vers une ressource internet externe"
 
 # subject and object forms for each relation type
 # (no object form for final or symetric relation types)
 msgctxt "Link"
 msgid "description"
```

### Comparing `cubicweb-link-1.9.1/cubicweb_link/views.py` & `cubicweb-link-2.0.0/cubicweb_link/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,80 +6,86 @@
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb import _
 from cubicweb.predicates import is_instance, one_line_rset
-from cubicweb.view import EntityView
-from cubicweb.web import formwidgets
-from cubicweb.web import action
-from cubicweb.web.views import uicfg, primary, baseviews, xbel
+from cubicweb_web.view import EntityView
+from cubicweb_web import formwidgets
+from cubicweb_web import action
+from cubicweb_web.views import uicfg, primary, baseviews, xbel
 
 
-for attr in ('title', 'url'):
-    uicfg.primaryview_section.tag_attribute(('Link', attr), 'hidden')
-
-uicfg.autoform_field_kwargs.tag_attribute(('Link', 'url'),
-                                          {'widget': formwidgets.TextInput})
+for attr in ("title", "url"):
+    uicfg.primaryview_section.tag_attribute(("Link", attr), "hidden")
+
+uicfg.autoform_field_kwargs.tag_attribute(
+    ("Link", "url"), {"widget": formwidgets.TextInput}
+)
 
 
 class LinkPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Link')
+    __select__ = is_instance("Link")
     show_attr_label = False
 
     def render_entity_title(self, entity):
-        title = u'<a href="%s">%s</a>' % (xml_escape(entity.url),
-                                          xml_escape(entity.title))
-        self.w(u'<h1><span class="etype">%s</span> %s</h1>'
-               % (entity.dc_type().capitalize(), title))
+        title = f'<a href="{xml_escape(entity.url)}">{xml_escape(entity.title)}</a>'
+        self.w(
+            '<h1><span class="etype">%s</span> %s</h1>'
+            % (entity.dc_type().capitalize(), title)
+        )
 
 
 class LinkOneLineView(baseviews.OneLineView):
-    __select__ = is_instance('Link')
+    __select__ = is_instance("Link")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
-        descr = entity.printable_value('description', format='text/plain')
+        descr = entity.printable_value("description", format="text/plain")
         descr = descr and descr.splitlines()[0]
-        values = {'title': xml_escape(entity.title),
-                  'url': xml_escape(entity.absolute_url()),
-                  'description': xml_escape(descr),
-                  }
-        self.w(u'<a href="%(url)s" title="%(description)s">%(title)s</a>'
-               % values)
-        self.w(u'&nbsp;[<a href="%s">%s</a>]'
-               % (xml_escape(entity.url),
-                  self._cw._('follow')))
+        values = {
+            "title": xml_escape(entity.title),
+            "url": xml_escape(entity.absolute_url()),
+            "description": xml_escape(descr),
+        }
+        self.w(
+            f"<a href=\"{values['url']}\" title=\"{values['description']}\">{values['title']}</a>"
+        )
+        self.w(
+            f"&nbsp;[<a href=\"{xml_escape(entity.url)}\">{self._cw._('follow')}</a>]"
+        )
 
 
 class LinkView(EntityView):
-    __regid__ = 'link'
-    __select__ = is_instance('Link')
-    title = _('link')
+    __regid__ = "link"
+    __select__ = is_instance("Link")
+    title = _("link")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
-        values = {'title': xml_escape(entity.title),
-                  'url': xml_escape(entity.url),
-                  'description': xml_escape(entity.printable_value('description')),
-                  }
-        self.w(u'<a href="%(url)s" title="%(description)s">%(title)s</a>'
-               % values)
+        values = {
+            "title": xml_escape(entity.title),
+            "url": xml_escape(entity.url),
+            "description": xml_escape(entity.printable_value("description")),
+        }
+        self.w(
+            f"<a href=\"{values['url']}\" title=\"{values['description']}\">{values['title']}</a>"
+        )
 
 
 class XbelItemLinkView(xbel.XbelItemView):
-    __select__ = is_instance('Link')
+    __select__ = is_instance("Link")
 
     def url(self, entity):
         return entity.url
 
 
 class LinkFollowAction(action.Action):
-    __select__ = one_line_rset() & is_instance('Link')
-    __regid__ = 'follow'
+    __select__ = one_line_rset() & is_instance("Link")
+    __regid__ = "follow"
 
-    title = _('follow')
-    category = 'mainactions'
+    title = _("follow")
+    category = "mainactions"
 
     def url(self):
         return self.cw_rset.get_entity(self.cw_row or 0, self.cw_col or 0).url
```

### Comparing `cubicweb-link-1.9.1/cubicweb_link.egg-info/SOURCES.txt` & `cubicweb-link-2.0.0/cubicweb_link.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
-README
+README.rst
+__pkginfo__.py
 setup.py
 tox.ini
 cubicweb_link/__init__.py
 cubicweb_link/__pkginfo__.py
 cubicweb_link/entities.py
 cubicweb_link/hooks.py
 cubicweb_link/schema.py
```

### Comparing `cubicweb-link-1.9.1/setup.py` & `cubicweb-link-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2016 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a cubicweb-link.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -27,56 +27,55 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_link', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_link", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'link=cubicweb_link',
+        "cubicweb.cubes": [
+            "link=cubicweb_link",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-link-1.9.1/test/unittest_link.py` & `cubicweb-link-2.0.0/test/unittest_link.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,59 @@
-# -*- coding: utf-8 -*-
-from cubicweb import ValidationError
-from cubicweb.devtools.testlib import CubicWebTC
-from cubicweb.web.views import uicfg, actions
+from cubicweb_web.devtools.testlib import WebCWTC
+from cubicweb_web.views import uicfg, actions
 
 from cubicweb_link import views
 
 afs = uicfg.autoform_section
 
 
-class LinkTC(CubicWebTC):
-
+class LinkTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
-            cnx.create_entity('Link', title=u"vous êtes perdu ?", url=u"http://www.perdu.com")
+            cnx.create_entity(
+                "Link", title="vous êtes perdu ?", url="http://www.perdu.com"
+            )
             cnx.commit()
 
     def test_possible_actions(self):
         with self.admin_access.web_request() as req:
-            rset = req.execute('Any X WHERE X is Link')
+            rset = req.execute("Any X WHERE X is Link")
             allactions = self.pactionsdict(req, rset)
-            self.assertEqual(allactions['mainactions'],
-                             [actions.ModifyAction,
-                              views.LinkFollowAction])
-            self.assertEqual(allactions['moreactions'],
-                             [actions.ManagePermissionsAction,
-                              actions.AddRelatedActions,
-                              actions.DeleteAction,
-                              actions.CopyAction,
-                              ])
+            self.assertEqual(
+                allactions["mainactions"],
+                [actions.ModifyAction, views.LinkFollowAction],
+            )
+            self.assertEqual(
+                allactions["moreactions"],
+                [
+                    actions.ManagePermissionsAction,
+                    actions.AddRelatedActions,
+                    actions.DeleteAction,
+                    actions.CopyAction,
+                ],
+            )
 
     def test_relations_by_category(self):
         def rbc(iterable):
             return [(rschema.type, x) for rschema, tschemas, x in iterable]
+
         with self.admin_access.web_request() as req:
-            e = self.vreg["etypes"].etype_class('Link')(req)
-            self.assertEqual(rbc(afs.relations_by_section(e, 'main', 'attributes', 'update')),
-                             [('title', 'subject'), ('url', 'subject'),
-                              ('description', 'subject')])
+            e = self.vreg["etypes"].etype_class("Link")(req)
+            self.assertEqual(
+                rbc(afs.relations_by_section(e, "main", "attributes", "update")),
+                [("title", "subject"), ("url", "subject"), ("description", "subject")],
+            )
         with self.admin_access.repo_cnx() as cnx:
-            self.create_user(cnx, u'toto')
-        with self.new_access(u'toto').web_request() as req:
+            self.create_user(cnx, "toto")
+        with self.new_access("toto").web_request() as req:
             # create a new instance with the new connection
-            e = self.vreg["etypes"].etype_class('Link')(req)
-            self.assertEqual(rbc(afs.relations_by_section(e, 'main', 'attributes', 'update')),
-                             [('title', 'subject'), ('url', 'subject'),
-                              ('description', 'subject')])
-
-    def test_noduplicates(self):
-        """ Check that links cannot be duplicated """
-        with self.admin_access.repo_cnx() as cnx:
-
-            # the link is already in the DB.
-            with self.assertRaises(ValidationError):
-                cnx.create_entity(
-                    "Link",
-                    title=u"vous êtes perdu ?",
-                    url=u"http://www.perdu.com",
-                )
-
-            # create a new link with a typo (thus not in the db)
-            # and assert that no error is raised
-            perdu_link = cnx.create_entity(
-                "Link",
-                title=u"vous êtes perdu ?",
-                url=u"http://www.perd.com",
+            e = self.vreg["etypes"].etype_class("Link")(req)
+            self.assertEqual(
+                rbc(afs.relations_by_section(e, "main", "attributes", "update")),
+                [("title", "subject"), ("url", "subject"), ("description", "subject")],
             )
 
-            # fix the url, and assert the ValidationError is raised
-            with self.assertRaises(ValidationError):
-                perdu_link.cw_set(url=u"http://www.perdu.com")
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     from unittest import main
+
     main()
```

