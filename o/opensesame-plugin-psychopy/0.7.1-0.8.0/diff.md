# Comparing `tmp/opensesame_plugin_psychopy-0.7.1.tar.gz` & `tmp/opensesame_plugin_psychopy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_plugin_psychopy-0.7.1.tar", max compression
+gzip compressed data, was "opensesame_plugin_psychopy-0.8.0.tar", max compression
```

## Comparing `opensesame_plugin_psychopy-0.7.1.tar` & `opensesame_plugin_psychopy-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,83 @@
--rw-r--r--   0        0        0      146 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/__init__.py
--rw-r--r--   0        0        0     1991 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/__init__.py
--rw-r--r--   0        0        0      935 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.png
--rw-r--r--   0        0        0     1883 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.py
--rw-r--r--   0        0        0     2154 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim_large.png
--rw-r--r--   0        0        0     1692 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/__init__.py
--rw-r--r--   0        0        0     6273 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_basestim.py
--rw-r--r--   0        0        0      889 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.png
--rw-r--r--   0        0        0     1644 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.py
--rw-r--r--   0        0        0     2095 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim_large.png
--rw-r--r--   0        0        0      506 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1084 2023-03-21 19:17:22.055327 opensesame_plugin_psychopy-0.7.1/readme.md
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 opensesame_plugin_psychopy-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/__init__.py
+-rw-r--r--   0        0        0     1991 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/__init__.py
+-rw-r--r--   0        0        0     3348 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ar.qm
+-rw-r--r--   0        0        0     7135 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ar.ts
+-rw-r--r--   0        0        0     3466 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/bn.qm
+-rw-r--r--   0        0        0     7744 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/bn.ts
+-rw-r--r--   0        0        0     3600 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/de.qm
+-rw-r--r--   0        0        0     6899 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/de.ts
+-rw-r--r--   0        0        0     3570 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/es.qm
+-rw-r--r--   0        0        0     6888 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/es.ts
+-rw-r--r--   0        0        0     3832 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/fr.qm
+-rw-r--r--   0        0        0     7030 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/fr.ts
+-rw-r--r--   0        0        0     3358 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/he.qm
+-rw-r--r--   0        0        0     7147 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/he.ts
+-rw-r--r--   0        0        0     3534 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/hi.qm
+-rw-r--r--   0        0        0     7758 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/hi.ts
+-rw-r--r--   0        0        0     3662 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/id.qm
+-rw-r--r--   0        0        0     6934 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/id.ts
+-rw-r--r--   0        0        0     3720 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/it.qm
+-rw-r--r--   0        0        0     6969 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/it.ts
+-rw-r--r--   0        0        0     2848 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ja.qm
+-rw-r--r--   0        0        0     6929 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ja.ts
+-rw-r--r--   0        0        0     2884 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ko.qm
+-rw-r--r--   0        0        0     6877 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ko.ts
+-rw-r--r--   0        0        0     3624 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/nl.qm
+-rw-r--r--   0        0        0     6916 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/nl.ts
+-rw-r--r--   0        0        0     3522 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/pt.qm
+-rw-r--r--   0        0        0     6875 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/pt.ts
+-rw-r--r--   0        0        0     3540 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ru.qm
+-rw-r--r--   0        0        0     7352 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/ru.ts
+-rw-r--r--   0        0        0     3524 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/tr.qm
+-rw-r--r--   0        0        0     6917 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/tr.ts
+-rw-r--r--   0        0        0     6808 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/translatables.ts
+-rw-r--r--   0        0        0     2740 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/yue.qm
+-rw-r--r--   0        0        0     6739 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/yue.ts
+-rw-r--r--   0        0        0     2728 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/zh.qm
+-rw-r--r--   0        0        0     6749 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/locale/zh.ts
+-rw-r--r--   0        0        0      935 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.png
+-rw-r--r--   0        0        0     1850 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.py
+-rw-r--r--   0        0        0     2154 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim_large.png
+-rw-r--r--   0        0        0     1683 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/__init__.py
+-rw-r--r--   0        0        0     2581 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ar.qm
+-rw-r--r--   0        0        0     5749 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ar.ts
+-rw-r--r--   0        0        0     2901 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/bn.qm
+-rw-r--r--   0        0        0     6479 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/bn.ts
+-rw-r--r--   0        0        0     2891 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/de.qm
+-rw-r--r--   0        0        0     5616 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/de.ts
+-rw-r--r--   0        0        0     2885 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/es.qm
+-rw-r--r--   0        0        0     5618 2023-07-07 13:04:51.677068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/es.ts
+-rw-r--r--   0        0        0     3151 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/fr.qm
+-rw-r--r--   0        0        0     5762 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/fr.ts
+-rw-r--r--   0        0        0     2699 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/he.qm
+-rw-r--r--   0        0        0     5847 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/he.ts
+-rw-r--r--   0        0        0     2871 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/hi.qm
+-rw-r--r--   0        0        0     6408 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/hi.ts
+-rw-r--r--   0        0        0     2943 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/id.qm
+-rw-r--r--   0        0        0     5648 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/id.ts
+-rw-r--r--   0        0        0     3023 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/it.qm
+-rw-r--r--   0        0        0     5695 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/it.ts
+-rw-r--r--   0        0        0     2335 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ja.qm
+-rw-r--r--   0        0        0     5746 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ja.ts
+-rw-r--r--   0        0        0     2371 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ko.qm
+-rw-r--r--   0        0        0     5694 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ko.ts
+-rw-r--r--   0        0        0     2911 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/nl.qm
+-rw-r--r--   0        0        0     5633 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/nl.ts
+-rw-r--r--   0        0        0     2951 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/pt.qm
+-rw-r--r--   0        0        0     5672 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/pt.ts
+-rw-r--r--   0        0        0     2829 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ru.qm
+-rw-r--r--   0        0        0     5998 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/ru.ts
+-rw-r--r--   0        0        0     2811 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/tr.qm
+-rw-r--r--   0        0        0     5622 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/tr.ts
+-rw-r--r--   0        0        0     5525 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/translatables.ts
+-rw-r--r--   0        0        0     2221 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/yue.qm
+-rw-r--r--   0        0        0     5545 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/yue.ts
+-rw-r--r--   0        0        0     2203 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/zh.qm
+-rw-r--r--   0        0        0     5542 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/locale/zh.ts
+-rw-r--r--   0        0        0     6601 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_basestim.py
+-rw-r--r--   0        0        0      889 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.png
+-rw-r--r--   0        0        0     1647 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.py
+-rw-r--r--   0        0        0     2095 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim_large.png
+-rw-r--r--   0        0        0      535 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1084 2023-07-07 13:04:51.681068 opensesame_plugin_psychopy-0.8.0/readme.md
+-rw-r--r--   0        0        0     1847 1970-01-01 00:00:00.000000 opensesame_plugin_psychopy-0.8.0/PKG-INFO
```

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/__init__.py` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/__init__.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.png` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.py` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,39 +18,39 @@
     PsychopyBasestim
 
 
 class PsychopyGratingstim(PsychopyBasestim):
 
     def reset(self):
         super().reset()
-        self.var.tex = u'sin'
-        self.var.mask = u'gauss'
+        self.var.tex = "'sin'"
+        self.var.mask = "'gauss'"
         self.var.xsize = 100
         self.var.ysize = 100
         self.var.sf = 0.05
         self.var.phase = 0
-        self.var.objectname = u'gratingstim'
+        self.var.objectname = 'gratingstim'
 
     @property
     def _stimclass(self):
         from psychopy.visual import GratingStim
         return GratingStim
 
     def _prepare_bytecode(self, c):
-        bytecode = psychopy_basestim._prepare_bytecode(self, c)
+        bytecode = super()._prepare_bytecode(c)
         bytecode.update({
-            u'xsize': c(u'xsize'),
-            u'ysize': c(u'ysize'),
-            u'sf': c(u'sf'),
-            u'tex': c(u'tex'),
-            u'mask': c(u'mask'),
-            u'phase': c(u'phase')
+            'xsize': c('xsize'),
+            'ysize': c('ysize'),
+            'sf': c('sf'),
+            'tex': c('tex'),
+            'mask': c('mask'),
+            'phase': c('phase')
         })
         return bytecode
 
     def _update_attributes(self, f):
         super()._update_attributes(f)
-        self._stim.sf = f(u'sf')
-        self._stim.tex = f(u'tex')
-        self._stim.mask = f(u'mask')
-        self._stim.phase = f(u'phase')
-        self._stim.size = f(u'xsize'), f(u'ysize')
+        self._stim.sf = f('sf')
+        self._stim.tex = f('tex')
+        self._stim.mask = f('mask')
+        self._stim.phase = f('phase')
+        self._stim.size = f('xsize'), f('ysize')
```

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim_large.png` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_gratingstim/psychopy_gratingstim_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/__init__.py` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+"""A PsychoPy TextStim, mainly for use with coroutines"""
+
 category = 'Visual stimuli'
-description = 'A PsychoPy TextStim, mainly for use with coroutines'
 controls = [
   {'label': 'Update every',
    'type': 'spinbox',
    'suffix': ' ms',
    'info': '-1 = no updating',
    'min_val': -1,
    'max_val': 10000,
```

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_basestim.py` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_basestim.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,87 +10,96 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with psychopy_textstim.  If not, see <http://www.gnu.org/licenses/>.
 """
 from libopensesame.py3compat import *
-from libopensesame.exceptions import MissingDependency, OSException
+from libopensesame.exceptions import MissingDependency, OSException, \
+    PythonSyntaxError, PythonError
 from libopensesame.item import Item
 
 
 class PsychopyBasestim(Item):
 
     def reset(self):
         self.var.framerate = -1
-        self.var.interpretation = u'opensesame'
+        self.var.interpretation = 'python'
         self.var.xpos = 0
         self.var.ypos = 0
         self.var.ori = 0
-        self.var.color = u'white'
+        self.var.color = "'white'"
         self.var.contrast = 1
         self.var.opacity = 1
-        self.var.script = u''
+        self.var.script = ''
         self.var.order = 0
 
     def coroutine(self, coroutines=None):
         try:
             from psychopy.visual import Window
         except ImportError as e:
             raise MissingDependency('Failed to import PsychoPy')
         # Check whether the PsychoPy window is available
-        if not hasattr(self.experiment, u'window') or \
+        if not hasattr(self.experiment, 'window') or \
                 not isinstance(self.experiment.window, Window):
             raise OSException('No PsychoPy window available. Have you '
                               'selected the psychopy backend?')
         self._stim = self._stimclass(self.experiment.window)
         # Make sure that the window is flipped after every cycle
         if coroutines is not None and \
                 self.winflip not in coroutines.post_cycle_functions:
             coroutines.post_cycle_functions.append(self.winflip)
             self.experiment._psychopystim_needflip = False
         # Add all gratings to the grating queue, which is drawn in order
         # before the window flip. We sort the queue to control the drawing
         # order/ depth/ z-index of the stimuli.
-        if not hasattr(self.experiment, u'_psychopystim_queue'):
+        if not hasattr(self.experiment, '_psychopystim_queue'):
             self.experiment._psychopystim_queue = []
         if self not in self.experiment._psychopystim_queue:
             self.experiment._psychopystim_queue.append(self)
             self.experiment._psychopystim_queue.sort(
                 key=lambda item: item.var.order)
         # Register the grating in the Python workspace
         self.python_workspace[self.var.objectname] = self._stim
         alive = True
         last_update = None
         # The function to evaluate values depends on whether they are
         # Python-style values, which are evaluated in the workspace, or
         # OpenSesame-style values, which are evaluated by the syntax module
         # when the variable is retrieved.
-        if self.var.interpretation == u'python':
+        if self.var.interpretation == 'python':
             # A compile function that gets a statement, converts it to a str,
             # and then byte-compiles it to a code object. We cannot use
             # python_workspace._compile(), because this assumes exec
             # statements.
-            def c(stm): return compile(
-                (u'#-*- coding:%s -*-\n' % self.experiment.encoding +
-                 safe_decode(self.var.get(stm, _eval=False)))
-                .encode(self.experiment.encoding),
-                u'<string>', u'eval')
+            def c(stm):
+                script = safe_decode(self.var.get(stm, _eval=False))
+                try:
+                    return compile(script, '<string>', 'eval')  # __ignore_traceback__
+                except SyntaxError as e:
+                    raise PythonSyntaxError(
+                        f'Syntax error in Python expression',
+                        line_nr=e.lineno)
             # The compile function is then applied to all statements so that
             # they are precompiled. This is done in another function so that it
             # can be overridden.
             bytecode = self._prepare_bytecode(c)
             # And the evalutation function just evals the bytecode
-            def f(stm): return self.python_workspace._eval(bytecode[stm])
+            def f(stm):
+                try:
+                    return self.python_workspace._eval(bytecode[stm])
+                except Exception as e:
+                    raise PythonError(
+                        'Error while evaluating Python expression')
         else:
             # If the statements are OpenSesame-style, all the work is done by
             # the var store
             def f(stm): return self.var.get(stm)
         # If a custom Python script is provided, it's byte-compiled
-        script = self.var.get(u'script', _eval=False).strip()
+        script = self.var.get('script', _eval=False).strip()
         script = None if not script else self.python_workspace._compile(script)
         self.is_active = False
         yield  # Preparation done
 
         # Run, PsychoPy, run!
         self.is_active = True
         while alive:
@@ -111,28 +120,28 @@
 
     @property
     def _stimclass(self):
         raise NotImplementedError()
 
     def _prepare_bytecode(self, c):
         return {
-            u'color': c(u'color'),
-            u'contrast': c(u'contrast'),
-            u'opacity': c(u'opacity'),
-            u'xpos': c(u'xpos'),
-            u'ypos': c(u'ypos'),
-            u'ori': c(u'ori')
+            'color': c('color'),
+            'contrast': c('contrast'),
+            'opacity': c('opacity'),
+            'xpos': c('xpos'),
+            'ypos': c('ypos'),
+            'ori': c('ori')
         }
 
     def _update_attributes(self, f):
-        self._stim.color = f(u'color')
-        self._stim.contrast = f(u'contrast')
-        self._stim.opacity = f(u'opacity')
-        self._stim.pos = f(u'xpos'), f(u'ypos')
-        self._stim.ori = f(u'ori')
+        self._stim.color = f('color')
+        self._stim.contrast = f('contrast')
+        self._stim.opacity = f('opacity')
+        self._stim.pos = f('xpos'), f('ypos')
+        self._stim.ori = f('ori')
 
     def winflip(self):
         if not self.experiment._psychopystim_needflip:
             return
         for item_ in self.experiment._psychopystim_queue:
             if item_.is_active:
                 item_._stim.draw()
```

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.png` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.py` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,30 @@
     PsychopyBasestim
 
 
 class PsychopyTextstim(PsychopyBasestim):
 
     def reset(self):
         super().reset()
-        self.var.text = ''
-        self.var.font_family = 'mono'
+        self.var.text = "'text'"
+        self.var.font_family = "'mono'"
         self.var.font_size = 18
         self.var.objectname = 'textstim'
         
     @property
     def _stimclass(self):
         from psychopy.visual import TextStim
         return TextStim
         
     def _prepare_bytecode(self, c):
         bytecode = super()._prepare_bytecode(c)
         bytecode.update({
-            'text'			: c('text'),
-            'font_family'	: c('font_family'),
-            'font_size'	: c('font_size'),
+            'text': c('text'),
+            'font_family': c('font_family'),
+            'font_size': c('font_size'),
             })
         return bytecode
         
     def _update_attributes(self, f):
         super()._update_attributes(f)
         self._stim.text = f('text')
         self._stim.font = f('font_family')
```

### Comparing `opensesame_plugin_psychopy-0.7.1/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim_large.png` & `opensesame_plugin_psychopy-0.8.0/opensesame_plugins/psychopy/psychopy_textstim/psychopy_textstim_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/readme.md` & `opensesame_plugin_psychopy-0.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_psychopy-0.7.1/PKG-INFO` & `opensesame_plugin_psychopy-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-psychopy
-Version: 0.7.1
+Version: 0.8.0
 Summary: PsychoPy plugins for OpenSesame
 Home-page: https://osdoc.cogsci.nl/
 License: COPYING
 Author: Sebastiaan Mathôt
 Author-email: s.mathot@cogsci.nl
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: opensesame-core (>3.99.99)
 Project-URL: Repository, https://github.com/open-cogsci/opensesame-plugin-psychopy
 Description-Content-Type: text/markdown
 
 # PsychoPy plugins for OpenSesame
 
 Copyright (2016-2023) Sebastiaan Mathôt
```

