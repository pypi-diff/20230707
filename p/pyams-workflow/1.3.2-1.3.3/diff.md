# Comparing `tmp/pyams_workflow-1.3.2.tar.gz` & `tmp/pyams_workflow-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_workflow-1.3.2.tar", last modified: Mon Feb 20 09:38:48 2023, max compression
+gzip compressed data, was "dist/pyams_workflow-1.3.3.tar", last modified: Fri Jul  7 21:49:11 2023, max compression
```

## Comparing `pyams_workflow-1.3.2.tar` & `pyams_workflow-1.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3019 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1274 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2571 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13226 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    26701 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/include.py
--rw-rw-rw-   0 root         (0) root         (0)    21162 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5556 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po
--rw-rw-rw-   0 root         (0) root         (0)     5733 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/locales/pyams_workflow.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    14340 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/versions.py
--rw-rw-rw-   0 root         (0) root         (0)    13568 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5561 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/history.py
--rw-rw-rw-   0 root         (0) root         (0)     5124 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/transition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      572 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/transitions.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-02-20 09:38:21.000000 pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3019 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1120 2023-02-20 09:38:48.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      268 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-20 09:38:47.000000 pyams_workflow-1.3.2/src/pyams_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1386 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2571 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13230 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    26701 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    21258 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po
+-rw-rw-rw-   0 root         (0) root         (0)     5733 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/locales/pyams_workflow.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    14456 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/versions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13568 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5561 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     5124 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/transition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      572 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/transitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-07-07 21:48:53.000000 pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      268 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-07 21:49:11.000000 pyams_workflow-1.3.3/src/pyams_workflow.egg-info/top_level.txt
```

### Comparing `pyams_workflow-1.3.2/LICENSE` & `pyams_workflow-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/PKG-INFO` & `pyams_workflow-1.3.3/src/pyams_workflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams_workflow
-Version: 1.3.2
+Name: pyams-workflow
+Version: 1.3.3
 Summary: PyAMS workflow management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS workflow
 Platform: UNKNOWN
@@ -48,14 +48,19 @@
 Please note however that this package doesn't provide any management interface, so can probably
 be reused easily outside of Pyramid.
 
 
 Changelog
 =========
 
+1.3.3
+-----
+ - updated default view permission
+ - automatically get last version if specified version ID is -1
+
 1.3.2
 -----
  - updated base transition form renderer
 
 1.3.1
 -----
  - added helper class to handle publication info of "hidden" contents
```

### Comparing `pyams_workflow-1.3.2/docs/HISTORY.rst` & `pyams_workflow-1.3.3/docs/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+1.3.3
+-----
+ - updated default view permission
+ - automatically get last version if specified version ID is -1
+
 1.3.2
 -----
  - updated base transition form renderer
 
 1.3.1
 -----
  - added helper class to handle publication info of "hidden" contents
```

### Comparing `pyams_workflow-1.3.2/docs/README.rst` & `pyams_workflow-1.3.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/setup.py` & `pyams_workflow-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.3.2'
+version = '1.3.3'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/__init__.py` & `pyams_workflow-1.3.3/src/pyams_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/content.py` & `pyams_workflow-1.3.3/src/pyams_workflow/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from zope.container.contained import Contained
 from zope.dublincore.interfaces import IZopeDublinCore
 from zope.interface import implementer
 from zope.schema.fieldproperty import FieldProperty
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
 from pyams_security.interfaces import ISecurityManager
-from pyams_security.interfaces.base import VIEW_PERMISSION
+from pyams_security.interfaces.base import PUBLIC_PERMISSION
 from pyams_utils.adapter import adapter_config, get_annotation_adapter
 from pyams_utils.date import SH_DATE_FORMAT, format_date, format_datetime
 from pyams_utils.factory import factory_config, get_object_factory
 from pyams_utils.registry import get_utility
 from pyams_utils.request import check_request
 from pyams_utils.timezone import GMT, gmtime, tztime
 from pyams_utils.traversing import get_parent
@@ -240,15 +240,15 @@
             if not wf_name:
                 return True
             # check workflow?
             if content.view_permission and \
                not request.has_permission(content.view_permission, context=self.__parent__):
                 return False
         else:
-            if not request.has_permission(VIEW_PERMISSION, context=self.__parent__):
+            if not request.has_permission(PUBLIC_PERMISSION, context=self.__parent__):
                 return False
         return self.is_published(check_parent)
 
 
 @adapter_config(required=IWorkflowPublicationSupport,
                 provides=IWorkflowPublicationInfo)
 def workflow_content_publication_info_factory(context):
```

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/doctests/README.rst` & `pyams_workflow-1.3.3/src/pyams_workflow/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/include.py` & `pyams_workflow-1.3.3/src/pyams_workflow/include.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/interfaces.py` & `pyams_workflow-1.3.3/src/pyams_workflow/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from zope.annotation import IAttributeAnnotatable
 from zope.interface import Attribute, Interface, Invalid, implementer, invariant
 from zope.interface.interfaces import IObjectEvent, ObjectEvent
 from zope.lifecycleevent import IObjectCreatedEvent, ObjectCreatedEvent
 from zope.schema import Bool, Choice, Datetime, Int, List, Object, Set, Text, TextLine
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
-from pyams_security.interfaces.base import VIEW_PERMISSION
+from pyams_security.interfaces.base import PUBLIC_PERMISSION
 from pyams_security.schema import PrincipalField
 
 
 from pyams_workflow import _
 
 
 #
@@ -403,16 +403,19 @@
 
 
 class IWorkflowVersions(Interface):
     """Interface to get information about versions of content in workflow"""
 
     last_version_id = Attribute("Last version ID")
 
-    def get_version(self, version_id):
-        """Get version matching given id"""
+    def get_version(self, version_id=None):
+        """Get version matching given id
+
+        If version ID is None or equals -1, method returns the last version.
+        """
 
     def get_versions(self, states=None, sort=False, reverse=False):
         """Get all versions of object known for this (optional) state"""
 
     def get_last_versions(self, count=1):
         """Get last versions of this object. Set count=0 to get all versions."""
 
@@ -452,15 +455,15 @@
                            description=_("Name of workflow utility managing this content"),
                            required=True,
                            vocabulary=WORKFLOWS_VOCABULARY)
 
     view_permission = Choice(title=_("View permission"),
                              description=_("This permission will be required to display content"),
                              vocabulary='PyAMS permissions',
-                             default=VIEW_PERMISSION,
+                             default=PUBLIC_PERMISSION,
                              required=False)
 
 
 DISPLAY_FIRST_VERSION = 'first'
 """Displayed publication date is the first publication date"""
 
 DISPLAY_CURRENT_VERSION = 'current'
```

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo` & `pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po` & `pyams_workflow-1.3.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/locales/pyams_workflow.pot` & `pyams_workflow-1.3.3/src/pyams_workflow/locales/pyams_workflow.pot`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/tests/__init__.py` & `pyams_workflow-1.3.3/src/pyams_workflow/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/tests/test_utilsdocs.py` & `pyams_workflow-1.3.3/src/pyams_workflow/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/tests/test_utilsdocstrings.py` & `pyams_workflow-1.3.3/src/pyams_workflow/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/versions.py` & `pyams_workflow-1.3.3/src/pyams_workflow/versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,17 +169,20 @@
     def __init__(self):
         super().__init__()
         self.last_version_id = 0
         self.state_by_version = PersistentMapping()
         self.versions_by_state = PersistentMapping()
         self.deleted = PersistentMapping()
 
-    def get_version(self, version_id):
-        """Get version with given ID"""
-        if version_id is None:
+    def get_version(self, version_id=None):
+        """Get version with given ID
+
+        If version ID is None or equals -1, method returns the last version.
+        """
+        if (version_id is None) or (version_id == -1):
             version_id = self.last_version_id
         try:
             return self[str(version_id)]
         except KeyError as ex:  # pylint: disable=invalid-name
             raise VersionError("Missing given version ID {0}".format(version_id)) from ex
 
     def get_versions(self, states=None, sort=False, reverse=False):
```

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/workflow.py` & `pyams_workflow-1.3.3/src/pyams_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/__init__.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/history.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/history.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/transition.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/transition.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/__init__.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/transitions.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/transitions.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow/zmi/viewlet/versions.py` & `pyams_workflow-1.3.3/src/pyams_workflow/zmi/viewlet/versions.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow.egg-info/PKG-INFO` & `pyams_workflow-1.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyams-workflow
-Version: 1.3.2
+Name: pyams_workflow
+Version: 1.3.3
 Summary: PyAMS workflow management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS workflow
 Platform: UNKNOWN
@@ -48,14 +48,19 @@
 Please note however that this package doesn't provide any management interface, so can probably
 be reused easily outside of Pyramid.
 
 
 Changelog
 =========
 
+1.3.3
+-----
+ - updated default view permission
+ - automatically get last version if specified version ID is -1
+
 1.3.2
 -----
  - updated base transition form renderer
 
 1.3.1
 -----
  - added helper class to handle publication info of "hidden" contents
```

### Comparing `pyams_workflow-1.3.2/src/pyams_workflow.egg-info/SOURCES.txt` & `pyams_workflow-1.3.3/src/pyams_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

