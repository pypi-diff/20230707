# Comparing `tmp/edx-i18n-tools-0.9.2.tar.gz` & `tmp/edx-i18n-tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-i18n-tools-0.9.2.tar", last modified: Mon Oct 17 18:57:03 2022, max compression
+gzip compressed data, was "edx-i18n-tools-1.0.0.tar", last modified: Fri Jul  7 13:15:28 2023, max compression
```

## Comparing `edx-i18n-tools-0.9.2.tar` & `edx-i18n-tools-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-17 18:57:03.000000 edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/i18n/
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/branch_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/changed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3989 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8968 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     7956 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1431 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5573 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/segment.py
--rw-r--r--   0 runner    (1001) docker     (121)     5490 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/transifex.py
--rw-r--r--   0 runner    (1001) docker     (121)     9864 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/i18n/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-17 18:57:03.775804 edx-i18n-tools-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2199 2022-10-17 18:56:59.000000 edx-i18n-tools-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5721 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.820283 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/branch_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/changed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8965 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10143 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7953 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1431 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/segment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5532 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9864 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2199 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/setup.py
```

### Comparing `edx-i18n-tools-0.9.2/LICENSE.txt` & `edx-i18n-tools-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/NOTICE.txt` & `edx-i18n-tools-1.0.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/PKG-INFO` & `edx-i18n-tools-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 0.9.2
+Version: 1.0.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-i18n-tools-0.9.2/README.rst` & `edx-i18n-tools-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/PKG-INFO` & `edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 0.9.2
+Version: 1.0.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-i18n-tools-0.9.2/edx_i18n_tools.egg-info/SOURCES.txt` & `edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/__init__.py` & `edx-i18n-tools-1.0.0/i18n/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tool to be used by other IDAs for internationalization.
 """
 import argparse
 import sys
 
 from . import config
 
-__version__ = '0.9.2'
+__version__ = '1.0.0'
 
 
 class Runner:
     """
     Runner class for internationalization.
     """
     def __init__(self):
```

### Comparing `edx-i18n-tools-0.9.2/i18n/branch_cleanup.py` & `edx-i18n-tools-1.0.0/i18n/branch_cleanup.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/changed.py` & `edx-i18n-tools-1.0.0/i18n/changed.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/config.py` & `edx-i18n-tools-1.0.0/i18n/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return locale_dir / BASE_CONFIG_FILENAME
 
     def read_config(self, filename):
         """
         Returns data found in config file (as dict), or raises exception if file not found
         """
         if not os.path.exists(filename):
-            raise Exception(f"Configuration file cannot be found: {filename}")
+            raise Exception(f"Configuration file cannot be found: {filename}")  # pylint: disable=broad-exception-raised
         with open(filename, encoding='UTF-8') as stream:
             return yaml.safe_load(stream)
 
     def __getattr__(self, name):
         if name in self.DEFAULTS:
             return self._config.get(name, self.DEFAULTS[name])
         raise AttributeError(f"Configuration has no such setting: {name!r}")
```

### Comparing `edx-i18n-tools-0.9.2/i18n/converter.py` & `edx-i18n-tools-1.0.0/i18n/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         """Extracts tags from string.
 
            returns (string, list) where
            string: string has tags replaced by indices (<BR>... => <0>, <1>, <2>, etc.)
            list: list of the removed tags ('<BR>', '<I>', '</I>')
         """
         counter = itertools.count(0)
-        count = lambda m: f'<{next(counter)}>'
+        count = lambda m: f'<{next(counter)}>'  # pylint: disable=unnecessary-lambda-assignment
         tags = self.tag_pattern.findall(string)
         tags = [''.join(tag) for tag in tags]
         (new, nfound) = self.tag_pattern.subn(count, string)
         if len(tags) != nfound:
-            raise Exception('tags dont match:' + string)
+            raise Exception('tags dont match:' + string)  # pylint: disable=broad-exception-raised
         return (new, tags)
 
     def retag_string(self, string, tags):
         """substitutes each tag back into string, into occurrences of <0>, <1> etc"""
         for i, tag in enumerate(tags):
             bracketed = f'<{i}>'
             string = re.sub(bracketed, tag, string, 1)
```

### Comparing `edx-i18n-tools-0.9.2/i18n/dummy.py` & `edx-i18n-tools-1.0.0/i18n/dummy.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 see http://www.loc.gov/standards/iso639-2/php/code_list.php
 
 Django will not localize in languages that django itself has not been
 localized for. So we are using a well-known language (default='eo').
 Django languages are listed in django.conf.global_settings.LANGUAGES
 
 po files can be generated with this:
-django-admin.py makemessages --all --extension html -l en
+django-admin makemessages --all --extension html -l en
 
 Usage:
 
 $ ./dummy.py
 
 generates output conf/locale/$DUMMY_LOCALE/LC_MESSAGES,
 where $DUMMY_LOCALE is the dummy_locale value set in the i18n config
```

### Comparing `edx-i18n-tools-0.9.2/i18n/execute.py` & `edx-i18n-tools-1.0.0/i18n/execute.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/extract.py` & `edx-i18n-tools-1.0.0/i18n/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This task extracts all English strings from all source code
 and produces three human-readable files:
    conf/locale/en/LC_MESSAGES/django-partial.po
    conf/locale/en/LC_MESSAGES/djangojs-partial.po
    conf/locale/en/LC_MESSAGES/mako.po
 
 This task will clobber any existing django.po file.
-This is because django-admin.py makemessages hardcodes this filename
+This is because django-admin makemessages hardcodes this filename
 and it cannot be overridden.
 
 """
 
 from datetime import datetime
 import importlib
 import os
@@ -31,14 +31,21 @@
 
 
 EDX_MARKER = "edX translation file"
 LOG = logging.getLogger(__name__)
 DEVNULL = open(os.devnull, 'wb')    # pylint: disable=consider-using-with
 
 
+def file_exists(path_name):
+    """
+    Returns True if the file exists and is not empty.
+    """
+    return os.path.exists(path_name) and os.path.getsize(path_name) > 0
+
+
 class Extract(Runner):
     """
     Class used to extract source files
     """
 
     def base(self, path1, *paths):
         """Return a relative path from config.BASE_DIR to path1 / paths[0] / ... """
@@ -114,15 +121,15 @@
                 verbosity=babel_verbosity,
                 config=babel_underscore_cfg,
                 output=self.base(configuration.source_messages_dir, 'underscore.po'),
             )
 
             execute(babel_underscore_cmd, working_directory=configuration.root_dir, stderr=stderr)
 
-        makemessages = f"django-admin.py makemessages -l en -v{args.verbose}"
+        makemessages = f"django-admin makemessages -l en -v{args.verbose}"
         ignores = " ".join(f'--ignore="{d}/*"' for d in configuration.ignore_dirs)
         if ignores:
             makemessages += " " + ignores
 
         # Extract strings from django source files (*.py, *.html, *.txt).
         make_django_cmd = makemessages + ' -d django'
         execute(make_django_cmd, working_directory=configuration.root_dir, stderr=stderr)
@@ -159,37 +166,49 @@
             )
             execute(babel_cmd, working_directory=app_dir, stderr=stderr)
 
         # Segment the generated files.
         segmented_files = segment_pofiles(configuration, configuration.source_locale)
         files_to_clean.update(segmented_files)
 
+        # Add partial files to the list of files to clean.
+        files_to_clean.update(('django_partial', 'djangojs_partial'))
+
         # Finish each file.
         for filename in files_to_clean:
-            LOG.info('Cleaning %s', filename)
-            pofile = polib.pofile(self.source_msgs_dir.joinpath(filename))
-            # replace default headers with edX headers
-            fix_header(pofile)
-            # replace default metadata with edX metadata
-            fix_metadata(pofile)
-            # remove key strings which belong in messages.po
-            strip_key_strings(pofile)
-            pofile.save()
+            clean_pofile(self.source_msgs_dir.joinpath(filename))
 
         # Restore the saved .po files.
         self.rename_source_file('django-saved.po', 'django.po')
         self.rename_source_file('djangojs-saved.po', 'djangojs.po')
 
 
+def clean_pofile(path_name):
+    """
+    Perform header fix, metadata fix, and key string removal on a single pofile
+    """
+    if not file_exists(path_name):
+        return
+    LOG.info('Cleaning %s', os.path.basename(path_name))
+    profile = polib.pofile(path_name)
+    # replace default headers with edX headers
+    fix_header(profile)
+    # replace default metadata with edX metadata
+    fix_metadata(profile)
+    # remove key strings which belong in messages.po
+    strip_key_strings(profile)
+    profile.save()
+
+
 def fix_header(pofile):
     """
     Replace default headers with edX headers
     """
 
-    # By default, django-admin.py makemessages creates this header:
+    # By default, django-admin makemessages creates this header:
     #
     #   SOME DESCRIPTIVE TITLE.
     #   Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
     #   This file is distributed under the same license as the PACKAGE package.
     #   FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 
     pofile.metadata_is_fuzzy = []   # remove [u'fuzzy']
@@ -216,36 +235,37 @@
 
 
 def fix_metadata(pofile):
     """
     Replace default metadata with edX metadata
     """
 
-    # By default, django-admin.py makemessages creates this metadata:
+    # By default, django-admin makemessages creates this metadata:
     #
     #   {u'PO-Revision-Date': u'YEAR-MO-DA HO:MI+ZONE',
     #   u'Language': u'',
     #   u'Content-Transfer-Encoding': u'8bit',
     #   u'Project-Id-Version': u'PACKAGE VERSION',
     #   u'Report-Msgid-Bugs-To': u'',
     #   u'Last-Translator': u'FULL NAME <EMAIL@ADDRESS>',
     #   u'Language-Team': u'LANGUAGE <LL@li.org>',
     #   u'POT-Creation-Date': u'2013-04-25 14:14-0400',
     #   u'Content-Type': u'text/plain; charset=UTF-8',
     #   u'MIME-Version': u'1.0'}
 
     fixes = {
-        'PO-Revision-Date': datetime.utcnow(),
         'Report-Msgid-Bugs-To': 'openedx-translation@googlegroups.com',
         'Project-Id-Version': '0.1a',
         'Language': 'en',
         'Last-Translator': '',
         'Language-Team': 'openedx-translation <openedx-translation@googlegroups.com>',
         'Plural-Forms': 'nplurals=2; plural=(n != 1);',
     }
+    pofile.metadata.pop('POT-Creation-Date', None)
+    pofile.metadata.pop('PO-Revision-Date', None)
     pofile.metadata.update(fixes)
 
 
 def strip_key_strings(pofile):
     """
     Removes all entries in PO which are key strings.
     These entries should appear only in messages.po, not in any other po files.
```

### Comparing `edx-i18n-tools-0.9.2/i18n/generate.py` & `edx-i18n-tools-1.0.0/i18n/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         # Dummy text is not required. Don't raise exception if files are missing.
         for locale in configuration.dummy_locales:
             merge_files(configuration, locale, fail_if_missing=False)
         # Merge the source locale, so we have the canonical .po files.
         if configuration.source_locale not in langs:
             merge_files(configuration, configuration.source_locale, fail_if_missing=args.strict)
 
-        compile_cmd = f'django-admin.py compilemessages -v{args.verbose}'
+        compile_cmd = f'django-admin compilemessages -v{args.verbose}'
         if args.verbose:
             stderr = None
         else:
             stderr = DEVNULL
         execute(compile_cmd, working_directory=configuration.root_dir, stderr=stderr)
 
         # Check for any mapped languages and copy directories around accordingly
```

### Comparing `edx-i18n-tools-0.9.2/i18n/main.py` & `edx-i18n-tools-1.0.0/i18n/main.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/segment.py` & `edx-i18n-tools-1.0.0/i18n/segment.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/i18n/transifex.py` & `edx-i18n-tools-1.0.0/i18n/transifex.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,14 @@
         elif args.command == "ltr":
             pull_all_ltr(self.configuration)
         elif args.command == "rtl":
             pull_all_rtl(self.configuration)
         elif args.command == "push_all":
             push_all()
         else:
-            raise Exception(f"unknown command ({args.command})")
+            raise Exception(f"unknown command ({args.command})")  # pylint: disable=broad-exception-raised
 
 
 main = Transifex()
 
 if __name__ == '__main__':
     main()
```

### Comparing `edx-i18n-tools-0.9.2/i18n/validate.py` & `edx-i18n-tools-1.0.0/i18n/validate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-0.9.2/setup.py` & `edx-i18n-tools-1.0.0/setup.py`

 * *Files identical despite different names*

