# Comparing `tmp/cubicweb-card-1.4.0.tar.gz` & `tmp/cubicweb-card-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-card-1.4.0.tar", last modified: Thu Nov 24 02:12:33 2022, max compression
+gzip compressed data, was "cubicweb-card-2.0.0.tar", last modified: Fri Jul  7 13:11:43 2023, max compression
```

## Comparing `cubicweb-card-1.4.0.tar` & `cubicweb-card-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      388 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      891 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.121128 cubicweb-card-1.4.0/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.121128 cubicweb-card-1.4.0/cubicweb_card/data/
--rw-rw-rw-   0 root         (0) root         (0)       44 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/data/cubes.card.css
--rw-rw-rw-   0 root         (0) root         (0)      786 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/cubicweb_card/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     1196 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     1358 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/cubicweb_card/migration/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/migration/0.5.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/cubicweb_card/views/
--rw-rw-rw-   0 root         (0) root         (0)     5277 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/views/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      720 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/cubicweb_card/views/urlrewrite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.121128 cubicweb-card-1.4.0/cubicweb_card.egg-info/
--rw-r--r--   0 root         (0) root         (0)      891 2022-11-24 02:12:32.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      827 2022-11-24 02:12:33.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:12:32.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-11-24 02:12:32.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:12:32.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2022-11-24 02:12:32.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-24 02:12:33.000000 cubicweb-card-1.4.0/cubicweb_card.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2471 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:12:33.125129 cubicweb-card-1.4.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/test/test_card.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/test/unittest_card.py
--rw-rw-rw-   0 root         (0) root         (0)     4294 2022-11-24 02:12:21.000000 cubicweb-card-1.4.0/test/unittest_entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.429242 cubicweb-card-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-07 13:11:43.425242 cubicweb-card-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.409241 cubicweb-card-2.0.0/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.417241 cubicweb-card-2.0.0/cubicweb_card/data/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/data/cubes.card.css
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.417241 cubicweb-card-2.0.0/cubicweb_card/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.421242 cubicweb-card-2.0.0/cubicweb_card/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/migration/0.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.421242 cubicweb-card-2.0.0/cubicweb_card/views/
+-rw-rw-rw-   0 root         (0) root         (0)     5207 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/views/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/cubicweb_card/views/urlrewrite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.413241 cubicweb-card-2.0.0/cubicweb_card.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      827 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-07 13:11:43.000000 cubicweb-card-2.0.0/cubicweb_card.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 13:11:43.429242 cubicweb-card-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.425242 cubicweb-card-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 13:11:43.425242 cubicweb-card-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/test/test_card.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/test/unittest_card.py
+-rw-rw-rw-   0 root         (0) root         (0)     4000 2023-07-07 13:10:36.000000 cubicweb-card-2.0.0/test/unittest_entities.py
```

### Comparing `cubicweb-card-1.4.0/PKG-INFO` & `cubicweb-card-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-card
-Version: 1.4.0
+Version: 2.0.0
 Summary: card/wiki component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-card
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 This cube models cards that are like wiki pages.
 
@@ -18,9 +17,7 @@
 or html.
 
 To create a new card, just create a link like '/card/YOUR_WIKI_ID' and follow it
 in your browser. Such a link can be written using the native HTML editor
 (fckeditor) or the dedicated restructured text "card" directive, as follows ::
 
   :card:`free_software/logilab:free software at Logilab`
-
-
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card/entities.py` & `cubicweb-card-2.0.0/cubicweb_card/entities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """this contains the cube-specific entities' classes"""
 
 from cubicweb.entities import AnyEntity, fetch_config
 
 
 class Card(AnyEntity):
     """customized class for Card entities"""
-    __regid__ = 'Card'
-    rest_attr = 'wikiid'
 
-    fetch_attrs, cw_fetch_order = fetch_config(['title'])
+    __regid__ = "Card"
+    rest_attr = "wikiid"
+
+    fetch_attrs, cw_fetch_order = fetch_config(["title"])
 
     def dc_title(self):
         if self.wikiid:
-            return self.wikiid.split('/')[-1]
+            return self.wikiid.split("/")[-1]
         else:
             return self.title
 
-    def dc_description(self, format='text/plain'):
-        return self.printable_value('synopsis', format=format)
+    def dc_description(self, format="text/plain"):
+        return self.printable_value("synopsis", format=format)
 
     def rest_path(self):
         if self.wikiid:
-            return '%s/%s' % (str(self.e_schema).lower(),
-                              self._cw.url_quote(self.wikiid, safe='/'))
+            return "{}/{}".format(
+                str(self.e_schema).lower(),
+                self._cw.url_quote(self.wikiid, safe="/"),
+            )
         else:
-            return super(Card, self).rest_path()
+            return super().rest_path()
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card/i18n/en.po` & `cubicweb-card-2.0.0/cubicweb_card/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-card-1.4.0/cubicweb_card/i18n/fr.po` & `cubicweb-card-2.0.0/cubicweb_card/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-card-1.4.0/cubicweb_card/site_cubicweb.py` & `cubicweb-card-2.0.0/cubicweb_card/site_cubicweb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from docutils import nodes, utils
 from docutils.parsers.rst.roles import register_canonical_role, set_classes
 
 
-def card_reference_role(role, rawtext, text, lineno, inliner,
-                        options={}, content=[]):
+def card_reference_role(role, rawtext, text, lineno, inliner, options={}, content=[]):
     text = text.strip()
     try:
-        wikiid, rest = text.split(u':', 1)
+        wikiid, rest = text.split(":", 1)
     except Exception:
         wikiid, rest = text, text
     context = inliner.document.settings.context
-    ref = context._cw.build_url('card/' + wikiid)
-    rset = context._cw.execute('Card C WHERE C wikiid %(w)s', {'w': wikiid})
+    ref = context._cw.build_url("card/" + wikiid)
+    rset = context._cw.execute("Card C WHERE C wikiid %(w)s", {"w": wikiid})
     set_classes(options)
     if not rset:
-        options['classes'] = ['doesnotexist']
+        options["classes"] = ["doesnotexist"]
     else:
-        options.pop('classes', None)
-    return [nodes.reference(rawtext, utils.unescape(rest), refuri=ref,
-                            **options)], []
+        options.pop("classes", None)
+    return [nodes.reference(rawtext, utils.unescape(rest), refuri=ref, **options)], []
 
 
-register_canonical_role('card', card_reference_role)
+register_canonical_role("card", card_reference_role)
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card/views/__init__.py` & `cubicweb-card-2.0.0/cubicweb_card/views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,135 +15,141 @@
 from logilab.common.decorators import cachedproperty
 
 from cubicweb.predicates import is_instance, match_form_params
 from cubicweb_web.views import uicfg, primary, baseviews
 from cubicweb_web.views.autoform import AutomaticEntityForm
 from cubicweb_web.views.ibreadcrumbs import IBreadCrumbsAdapter
 
-uicfg.primaryview_section.tag_attribute(('Card', 'title'), 'hidden')
-uicfg.primaryview_section.tag_attribute(('Card', 'synopsis'), 'hidden')
-uicfg.primaryview_section.tag_attribute(('Card', 'wikiid'), 'hidden')
+uicfg.primaryview_section.tag_attribute(("Card", "title"), "hidden")
+uicfg.primaryview_section.tag_attribute(("Card", "synopsis"), "hidden")
+uicfg.primaryview_section.tag_attribute(("Card", "wikiid"), "hidden")
 
 
 class CardPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Card')
+    __select__ = is_instance("Card")
     show_attr_label = False
 
     def render_entity_title(self, entity):
-        self.w(u'<h1>%s</h1>' % xml_escape(entity.title))
+        self.w(f"<h1>{xml_escape(entity.title)}</h1>")
         if entity.synopsis:
-            self.w(u'<div class="summary">%s</div>'
-                   % entity.printable_value('synopsis'))
+            self.w(f"<div class=\"summary\">{entity.printable_value('synopsis')}</div>")
 
 
 class CardInlinedView(CardPrimaryView):
     """hide card title and summary"""
-    __regid__ = 'inlined'
-    title = _('inlined view')
+
+    __regid__ = "inlined"
+    title = _("inlined view")
     main_related_section = False
 
     def render_entity_title(self, entity):
-        self.w(u'<div class="summary">%s</div>'
-               % entity.printable_value('synopsis'))
+        self.w(f"<div class=\"summary\">{entity.printable_value('synopsis')}</div>")
 
     def content_navigation_components(self, context):
         pass
 
 
 class CardDoesNotExistView(baseviews.NoResultView):
-    __select__ = (baseviews.NoResultView.__select__ &
-                  match_form_params('wikiid'))
+    __select__ = baseviews.NoResultView.__select__ & match_form_params("wikiid")
 
     def call(self, **kwargs):
-        super(CardDoesNotExistView, self).call(**kwargs)
-        etype = self._cw.vreg['etypes'].etype_class('Card')
-        ctx = {'url': etype.cw_create_url(self._cw,
-                                          wikiid=self._cw.form['wikiid']),
-               'message': xml_escape(self._cw._('This card does not exist yet.')),
-               'invite': xml_escape(self._cw._('Create it?')),
-               'notice': ''}
-        if not self._cw.vreg.schema['Card'].has_perm(self._cw, 'add'):
-            ctx['notice'] = xml_escape(self._cw._(' (You may need to log in first.)'))
-        self.w(u'<div class="section">%(message)s '
-               u'<a href="%(url)s">%(invite)s</a>%(notice)s</div>' % ctx)
+        super().call(**kwargs)
+        etype = self._cw.vreg["etypes"].etype_class("Card")
+        ctx = {
+            "url": etype.cw_create_url(self._cw, wikiid=self._cw.form["wikiid"]),
+            "message": xml_escape(self._cw._("This card does not exist yet.")),
+            "invite": xml_escape(self._cw._("Create it?")),
+            "notice": "",
+        }
+        if not self._cw.vreg.schema["Card"].has_perm(self._cw, "add"):
+            ctx["notice"] = xml_escape(self._cw._(" (You may need to log in first.)"))
+        self.w(
+            '<div class="section">%(message)s '
+            '<a href="%(url)s">%(invite)s</a>%(notice)s</div>' % ctx
+        )
         self._cw.status_out = 404
 
 
 class CardBreadCrumbsAdapter(IBreadCrumbsAdapter):
-
-    __select__ = IBreadCrumbsAdapter.__select__ & is_instance('Card')
+    __select__ = IBreadCrumbsAdapter.__select__ & is_instance("Card")
 
     @cachedproperty
     def dirname(self):
         if self.entity.wikiid:
-            return '/'.join(self.entity.wikiid.split('/')[:-1])
+            return "/".join(self.entity.wikiid.split("/")[:-1])
 
     def card_from_wikiid(self, path):
         """Return the Card given its ``wikiid`` path or None"""
         rset = self._cw.execute("Card C WHERE C wikiid %(id)s", {"id": path})
         if rset:
             return rset.get_entity(0, 0)
 
     def parent_entity(self):
         if not self.dirname:
             # card is at root: return whatever super returns
-            parent = super(CardBreadCrumbsAdapter, self).parent_entity()
+            parent = super().parent_entity()
         else:
             parent = self.card_from_wikiid(self.dirname)
         return parent
 
     def breadcrumbs(self, view=None, recurs=None):
         """Virtual hierarchy of wiki pages following a directory-like
         structure.
         """
         if self.parent_entity() or not self.dirname:
             # parent Card exists or the current Card is at the root (i.e. its
             # wikiid has no /)
-            return super(CardBreadCrumbsAdapter, self).breadcrumbs(view, recurs)
+            return super().breadcrumbs(view, recurs)
         else:
             # parent card does not exist: build the (reversed) path by
             # iterating on the directory structure
             path = [self.entity]
-            dirs = self.dirname.split('/')
+            dirs = self.dirname.split("/")
             while dirs:
-                card = self.card_from_wikiid('/'.join(dirs))
+                card = self.card_from_wikiid("/".join(dirs))
                 p = [dirs.pop()]
                 if card:
-                    p = card.cw_adapt_to('IBreadCrumbs').breadcrumbs(view, recurs)
+                    p = card.cw_adapt_to("IBreadCrumbs").breadcrumbs(view, recurs)
                 path.extend(p)
             if not card:
                 # last path entry is not a card
-                path.append((self._cw.build_url(str(self.entity.e_schema)),
-                             self._cw._('Card_plural')))
+                path.append(
+                    (
+                        self._cw.build_url(str(self.entity.e_schema)),
+                        self._cw._("Card_plural"),
+                    )
+                )
             path.reverse()
             return path
 
 
 try:
     from cubicweb_seo.views import SitemapRule
 
     class CardSitemapRule(SitemapRule):
-        __regid__ = 'card'
-        query = 'Any X WHERE X is Card'
+        __regid__ = "card"
+        query = "Any X WHERE X is Card"
         priority = 1.0
+
 except ImportError:
     pass
 
 
 def registration_callback(vreg):
     vreg.register(CardPrimaryView)
     vreg.register(CardInlinedView)
     vreg.register(CardDoesNotExistView)
     vreg.register(CardBreadCrumbsAdapter)
 
     loaded_cubes = vreg.config.cubes()
 
-    if 'seo' in loaded_cubes:
+    if "seo" in loaded_cubes:
         vreg.register(CardSitemapRule)
 
-    if 'preview' in loaded_cubes:
+    if "preview" in loaded_cubes:
         from cubicweb_preview.views.forms import PreviewFormMixin
 
         class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
-            preview_mode = 'inline'
-            __select__ = AutomaticEntityForm.__select__ & is_instance('Card')
+            preview_mode = "inline"
+            __select__ = AutomaticEntityForm.__select__ & is_instance("Card")
+
         vreg.register(PreviewAutomaticEntityForm)
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card/views/urlrewrite.py` & `cubicweb-card-2.0.0/cubicweb_card/views/urlrewrite.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,10 +13,15 @@
     """handle path with the form::
 
         card/<wikiid>   -> view wiki page, wikiid can contain /
 
     Fall back to the `card` controller in any cases. The latter will handle
     both existent and non-existent cards.
     """
+
     priority = 10
-    rules = [(rgx('/card/(?P<wikiid>.+)'),
-              rgx_action(controller='card', formgroups=('wikiid', )))]
+    rules = [
+        (
+            rgx("/card/(?P<wikiid>.+)"),
+            rgx_action(controller="card", formgroups=("wikiid",)),
+        )
+    ]
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card.egg-info/PKG-INFO` & `cubicweb-card-2.0.0/cubicweb_card.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-card
-Version: 1.4.0
+Version: 2.0.0
 Summary: card/wiki component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-card
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 This cube models cards that are like wiki pages.
 
@@ -18,9 +17,7 @@
 or html.
 
 To create a new card, just create a link like '/card/YOUR_WIKI_ID' and follow it
 in your browser. Such a link can be written using the native HTML editor
 (fckeditor) or the dedicated restructured text "card" directive, as follows ::
 
   :card:`free_software/logilab:free software at Logilab`
-
-
```

### Comparing `cubicweb-card-1.4.0/cubicweb_card.egg-info/SOURCES.txt` & `cubicweb-card-2.0.0/cubicweb_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-card-1.4.0/setup.py` & `cubicweb-card-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,58 +21,57 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_card', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_card", "__pkginfo__.py")
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
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-dependency_links = __pkginfo__.get('dependency_links', ())
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
-            'card=cubicweb_card',
+        "cubicweb.cubes": [
+            "card=cubicweb_card",
+        ],
+        "cubicweb.i18ncube": [
+            "card=cubicweb_card.i18n",
         ],
-        'cubicweb.i18ncube': [
-            'card=cubicweb_card.i18n',
-        ]
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-card-1.4.0/test/unittest_card.py` & `cubicweb-card-2.0.0/test/unittest_card.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 "Card unit test"
 import re
 import unittest
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC, MAILBOX
-from cubicweb.ext.rest import rest_publish
+from cubicweb.devtools.testlib import MAILBOX
+from cubicweb_web.devtools.testlib import WebCWTC
+from cubicweb_web.ext.rest import rest_publish
 
 
-class CardTests(CubicWebTC):
-
+class CardTests(WebCWTC):
     def test_notifications(self):
         with self.admin_access.client_cnx() as cnx:
             cnx.create_entity(
-                'Card', title=u'sample card',
-                synopsis=u'this is a sample card')
+                "Card", title="sample card", synopsis="this is a sample card"
+            )
             self.assertEqual(len(MAILBOX), 0)
             cnx.commit()
         self.assertEqual(len(MAILBOX), 1)
-        self.assertEqual(re.sub(r'#\d+', '#EID', MAILBOX[0].subject),
-                         'New Card #EID (admin)')
+        self.assertEqual(
+            re.sub(r"#\d+", "#EID", MAILBOX[0].subject), "New Card #EID (admin)"
+        )
 
 
-class RestTC(CubicWebTC):
+class RestTC(WebCWTC):
     def context(self, cnx):
         return cnx.execute('CWUser X WHERE X login "admin"').get_entity(0, 0)
 
     def test_card_role_create(self):
         with self.admin_access.client_cnx() as cnx:
             self.assertEqual(
-                rest_publish(self.context(cnx), ':card:`index`'),
+                rest_publish(self.context(cnx), ":card:`index`"),
                 f'<p><a class="doesnotexist reference" '
-                f'href="{BASE_URL}card/index">index</a></p>\n')
+                f'href="{BASE_URL}card/index">index</a></p>\n',
+            )
 
     def test_card_role_create_subpage(self):
         with self.admin_access.client_cnx() as cnx:
             self.assertEqual(
-                rest_publish(self.context(cnx), ':card:`foo/bar`'),
+                rest_publish(self.context(cnx), ":card:`foo/bar`"),
                 f'<p><a class="doesnotexist reference" '
-                f'href="{BASE_URL}card/foo/bar">foo/bar</a></p>\n')  # noqa
+                f'href="{BASE_URL}card/foo/bar">foo/bar</a></p>\n',
+            )  # noqa
 
     def test_card_role_link(self):
         with self.admin_access.client_cnx() as cnx:
-            cnx.create_entity('Card', wikiid=u'index',
-                              title=u'Site index page', synopsis=u'yo')
+            cnx.create_entity(
+                "Card", wikiid="index", title="Site index page", synopsis="yo"
+            )
             self.assertEqual(
-                rest_publish(self.context(cnx), ':card:`index`'),
+                rest_publish(self.context(cnx), ":card:`index`"),
                 f'<p><a class="reference" '
-                f'href="{BASE_URL}card/index">index</a></p>\n')
+                f'href="{BASE_URL}card/index">index</a></p>\n',
+            )
 
     def test_nocard_create(self):
-        with self.admin_access.web_request('card/foobar') as req:
+        with self.admin_access.web_request("card/foobar") as req:
             content = self.app_handle_request(req)
-            create_url = req.build_url('add/Card?wikiid=foobar')
-            self.assertIn(' href="{0}"'.format(create_url).encode('utf-8'), content)
+            create_url = req.build_url("add/Card?wikiid=foobar")
+            self.assertIn(f' href="{create_url}"'.encode(), content)
             self.assertEqual(req.status_out, 404)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-card-1.4.0/test/unittest_entities.py` & `cubicweb-card-2.0.0/test/unittest_entities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2013-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2013-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -13,81 +13,79 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """test on entities"""
 
 import unittest
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class DCTitleTC(CubicWebTC):
+class DCTitleTC(WebCWTC):
     def test_nowikiid(self):
         with self.admin_access.client_cnx() as cnx:
-            venus = cnx.create_entity('Card', title=u"Venus",
-                                      content=u"a planet")
-            self.assertEqual(venus.dc_title(), 'Venus')
+            venus = cnx.create_entity("Card", title="Venus", content="a planet")
+            self.assertEqual(venus.dc_title(), "Venus")
 
     def test_wikiid(self):
         with self.admin_access.client_cnx() as cnx:
             venus = cnx.create_entity(
-                'Card', title=u"Venus",
-                content=u"a planet", wikiid=u'Planet_Venus')
-            self.assertEqual(venus.dc_title(), 'Planet_Venus')
+                "Card", title="Venus", content="a planet", wikiid="Planet_Venus"
+            )
+            self.assertEqual(venus.dc_title(), "Planet_Venus")
 
 
-class BreadCrumbsTC(CubicWebTC):
+class BreadCrumbsTC(WebCWTC):
     def test_onecard_nowikiid(self):
         with self.admin_access.web_request() as req:
-            venus = req.create_entity('Card', title=u"Venus",
-                                      content=u"a planet")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
+            venus = req.create_entity("Card", title="Venus", content="a planet")
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
             self.assertListEqual([venus], breadcrumbs)
 
     def test_onecard(self):
         with self.admin_access.web_request() as req:
-            venus = req.create_entity('Card', title=u"Venus",
-                                      content=u"a planet", wikiid=u"Venus")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
+            venus = req.create_entity(
+                "Card", title="Venus", content="a planet", wikiid="Venus"
+            )
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
             self.assertListEqual([venus], breadcrumbs)
 
     def test_twocards(self):
         """Planet and Planet/Venus"""
         with self.admin_access.web_request() as req:
-            planet = req.create_entity('Card', title=u"Planet",
-                                       wikiid=u"Planet")
-            venus = req.create_entity('Card', title=u"Venus",
-                                      wikiid=u"Planet/Venus")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
+            planet = req.create_entity("Card", title="Planet", wikiid="Planet")
+            venus = req.create_entity("Card", title="Venus", wikiid="Planet/Venus")
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
             self.assertListEqual([planet, venus], breadcrumbs)
 
     def test_onecardnested(self):
         """Planet/Venus without Planet"""
         with self.admin_access.web_request() as req:
-            venus = req.create_entity('Card', title=u"Venus",
-                                      wikiid=u"Planet/Venus")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
-            self.assertListEqual(['Planet', venus], breadcrumbs[1:])
+            venus = req.create_entity("Card", title="Venus", wikiid="Planet/Venus")
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
+            self.assertListEqual(["Planet", venus], breadcrumbs[1:])
 
     def test_treecards_oneinexistent(self):
         """Astronomy and Astronomy/Planet/Venus (no Astronomy/Planet)"""
         with self.admin_access.web_request() as req:
-            astro = req.create_entity('Card', title=u"Astronomy",
-                                      wikiid=u"Astronomy")
-            venus = req.create_entity('Card', title=u"Venus",
-                                      wikiid=u"Astronomy/Planet/Venus")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
-            self.assertListEqual([astro, 'Planet', venus], breadcrumbs)
+            astro = req.create_entity("Card", title="Astronomy", wikiid="Astronomy")
+            venus = req.create_entity(
+                "Card", title="Venus", wikiid="Astronomy/Planet/Venus"
+            )
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
+            self.assertListEqual([astro, "Planet", venus], breadcrumbs)
 
     def test_treecards_oneinexistent2(self):
         """Astronomy/Planet and Astronomy/Planet/Venus (no Astronomy)"""
         with self.admin_access.web_request() as req:
-            planet = req.create_entity('Card', title=u"Planets",
-                                       wikiid=u"Astronomy/Planet")
-            venus = req.create_entity('Card', title=u"Venus",
-                                      wikiid=u"Astronomy/Planet/Venus")
-            breadcrumbs = venus.cw_adapt_to('IBreadCrumbs').breadcrumbs()
-            self.assertListEqual(['Astronomy', planet, venus], breadcrumbs[1:])
+            planet = req.create_entity(
+                "Card", title="Planets", wikiid="Astronomy/Planet"
+            )
+            venus = req.create_entity(
+                "Card", title="Venus", wikiid="Astronomy/Planet/Venus"
+            )
+            breadcrumbs = venus.cw_adapt_to("IBreadCrumbs").breadcrumbs()
+            self.assertListEqual(["Astronomy", planet, venus], breadcrumbs[1:])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

