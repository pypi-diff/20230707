# Comparing `tmp/pygenda-0.2.7.tar.gz` & `tmp/pygenda-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenda-0.2.7.tar", last modified: Fri Apr 28 10:30:07 2023, max compression
+gzip compressed data, was "pygenda-0.2.8.tar", last modified: Fri Jul  7 06:43:32 2023, max compression
```

## Comparing `pygenda-0.2.7.tar` & `pygenda-0.2.8.tar`

### file list

```diff
@@ -1,83 +1,59 @@
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.421058 pygenda-0.2.7/
--rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.2.7/COPYING
--rw-------   0 matt      (1000) users      (100)     1015 2023-04-28 10:30:07.420058 pygenda-0.2.7/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     6283 2023-04-28 10:14:02.000000 pygenda-0.2.7/README.md
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.407058 pygenda-0.2.7/csrc/
--rw-------   0 matt      (1000) users      (100)      773 2022-01-30 22:37:16.000000 pygenda-0.2.7/csrc/Makefile
--rw-------   0 matt      (1000) users      (100)     3027 2023-03-31 11:03:09.000000 pygenda-0.2.7/csrc/pygenda_clipboard.c
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.408058 pygenda-0.2.7/docs/
--rw-------   0 matt      (1000) users      (100)     3429 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/CalDAV.md
--rw-------   0 matt      (1000) users      (100)     3559 2023-04-23 17:43:29.000000 pygenda-0.2.7/docs/Development.md
--rw-------   0 matt      (1000) users      (100)     3066 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/Usage.md
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.409058 pygenda-0.2.7/docs/config-examples/
--rw-------   0 matt      (1000) users      (100)      497 2022-01-30 22:37:16.000000 pygenda-0.2.7/docs/config-examples/README.md
--rw-------   0 matt      (1000) users      (100)     2532 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/backgrounds.css
--rw-------   0 matt      (1000) users      (100)     6205 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/darkmode.css
--rw-------   0 matt      (1000) users      (100)     6023 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/config-examples/defaults.ini
--rw-------   0 matt      (1000) users      (100)     3459 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/config-examples/gemini.css
--rw-------   0 matt      (1000) users      (100)       41 2022-01-30 22:37:16.000000 pygenda-0.2.7/docs/config-examples/gemini.ini
--rw-------   0 matt      (1000) users      (100)      342 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/pygenda.desktop
--rw-------   0 matt      (1000) users      (100)    10433 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/known_issues.md
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.410058 pygenda-0.2.7/docs/screenshots/
--rw-------   0 matt      (1000) users      (100)    17045 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/todo_view.png
--rw-------   0 matt      (1000) users      (100)    16198 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/week_view.png
--rw-------   0 matt      (1000) users      (100)    23745 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/year_view.png
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.413058 pygenda-0.2.7/pygenda/
--rwx------   0 matt      (1000) users      (100)      823 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/__main__.py
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.415058 pygenda-0.2.7/pygenda/css/
--rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+loop+star.svg
--rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+loop.svg
--rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+star.svg
--rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc.svg
--rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/loop+star.svg
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/loop.svg
--rw-------   0 matt      (1000) users      (100)    15656 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/css/pygenda.css
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/star.svg
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/glade/
--rw-------   0 matt      (1000) users      (100)    44996 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/glade/dialog_event.glade
--rw-------   0 matt      (1000) users      (100)     5150 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/dialog_find.glade
--rw-------   0 matt      (1000) users      (100)     7963 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/dialog_todo.glade
--rw-------   0 matt      (1000) users      (100)    27159 2023-04-23 17:32:42.000000 pygenda-0.2.7/pygenda/glade/main.glade
--rw-------   0 matt      (1000) users      (100)     3892 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/view_week.glade
--rw-------   0 matt      (1000) users      (100)     5931 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/glade/view_year.glade
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/en_US/
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)      433 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)     1290 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/pygenda.po
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/fr/
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)     8312 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)    14232 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.po
--rw-------   0 matt      (1000) users      (100)     1104 2023-04-25 20:33:58.000000 pygenda-0.2.7/pygenda/mypy.ini
--rw-------   0 matt      (1000) users      (100)    58256 2023-04-23 17:43:29.000000 pygenda-0.2.7/pygenda/pygenda_calendar.py
--rw-------   0 matt      (1000) users      (100)     5450 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_config.py
--rw-------   0 matt      (1000) users      (100)     9869 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_entryprops.py
--rw-------   0 matt      (1000) users      (100)    62921 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_dialog_event.py
--rw-------   0 matt      (1000) users      (100)     3538 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_find.py
--rw-------   0 matt      (1000) users      (100)     5377 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_todo.py
--rw-------   0 matt      (1000) users      (100)     4146 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_entryinfo.py
--rw-------   0 matt      (1000) users      (100)    42037 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/pygenda_gui.py
--rw-------   0 matt      (1000) users      (100)    10419 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_util.py
--rw-------   0 matt      (1000) users      (100)      300 2023-04-28 10:14:24.000000 pygenda-0.2.7/pygenda/pygenda_version.py
--rw-------   0 matt      (1000) users      (100)    15418 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_view.py
--rw-------   0 matt      (1000) users      (100)    26915 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/pygenda_view_todo.py
--rw-------   0 matt      (1000) users      (100)    21063 2023-04-23 17:43:29.000000 pygenda-0.2.7/pygenda/pygenda_view_week.py
--rw-------   0 matt      (1000) users      (100)    27377 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_view_year.py
--rw-------   0 matt      (1000) users      (100)    22142 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_widgets.py
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.413058 pygenda-0.2.7/pygenda.egg-info/
--rw-------   0 matt      (1000) users      (100)     1015 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     2218 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/SOURCES.txt
--rw-------   0 matt      (1000) users      (100)        1 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/dependency_links.txt
--rw-------   0 matt      (1000) users      (100)       44 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/requires.txt
--rw-------   0 matt      (1000) users      (100)        8 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/top_level.txt
--rw-------   0 matt      (1000) users      (100)       38 2023-04-28 10:30:07.421058 pygenda-0.2.7/setup.cfg
--rwx------   0 matt      (1000) users      (100)     3745 2023-04-28 10:14:02.000000 pygenda-0.2.7/setup.py
-drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.418058 pygenda-0.2.7/test/
--rwx------   0 matt      (1000) users      (100)    15117 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/maketest_example.py
--rwx------   0 matt      (1000) users      (100)     1274 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/maketest_large.py
--rw-------   0 matt      (1000) users      (100)       83 2022-01-30 22:37:16.000000 pygenda-0.2.7/test/test00_empty.ics
--rw-------   0 matt      (1000) users      (100)     1500 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test01_small.ics
--rw-------   0 matt      (1000) users      (100)    12965 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test02_repeats.ics
--rw-------   0 matt      (1000) users      (100)     1241 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test03_errors.ics
--rwx------   0 matt      (1000) users      (100)   107588 2023-04-23 17:43:29.000000 pygenda-0.2.7/test/test_repeats.py
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.451005 pygenda-0.2.8/
+-rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.2.8/COPYING
+-rw-------   0 matt      (1000) users      (100)      275 2023-07-06 20:42:29.000000 pygenda-0.2.8/MANIFEST.in
+-rw-------   0 matt      (1000) users      (100)     1015 2023-07-07 06:43:32.450005 pygenda-0.2.8/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     6431 2023-07-06 20:42:29.000000 pygenda-0.2.8/README.md
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.444005 pygenda-0.2.8/csrc/
+-rw-------   0 matt      (1000) users      (100)      812 2023-07-06 20:42:29.000000 pygenda-0.2.8/csrc/CMakeLists.txt
+-rw-------   0 matt      (1000) users      (100)     3043 2023-07-06 20:42:29.000000 pygenda-0.2.8/csrc/pygenda_clipboard.c
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.446005 pygenda-0.2.8/pygenda/
+-rwx------   0 matt      (1000) users      (100)      823 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/__main__.py
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.447005 pygenda-0.2.8/pygenda/app/
+-rw-------   0 matt      (1000) users      (100)      369 2023-07-06 20:42:29.000000 pygenda-0.2.8/pygenda/app/pygenda.desktop
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.448005 pygenda-0.2.8/pygenda/css/
+-rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/disc+loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/disc+loop.svg
+-rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/disc+star.svg
+-rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/disc.svg
+-rw-------   0 matt      (1000) users      (100)     3688 2023-07-06 20:42:29.000000 pygenda-0.2.8/pygenda/css/gemini.css
+-rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/loop.svg
+-rw-------   0 matt      (1000) users      (100)    15656 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/css/pygenda.css
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.8/pygenda/css/star.svg
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.450005 pygenda-0.2.8/pygenda/glade/
+-rw-------   0 matt      (1000) users      (100)    41555 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/glade/dialog_event.glade
+-rw-------   0 matt      (1000) users      (100)     5150 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/glade/dialog_find.glade
+-rw-------   0 matt      (1000) users      (100)     7963 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/glade/dialog_todo.glade
+-rw-------   0 matt      (1000) users      (100)    27159 2023-07-05 21:01:57.000000 pygenda-0.2.8/pygenda/glade/main.glade
+-rw-------   0 matt      (1000) users      (100)     3892 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/glade/view_week.glade
+-rw-------   0 matt      (1000) users      (100)     5931 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/glade/view_year.glade
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.442005 pygenda-0.2.8/pygenda/locale/
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.442005 pygenda-0.2.8/pygenda/locale/en_US/
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.450005 pygenda-0.2.8/pygenda/locale/en_US/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)      433 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.442005 pygenda-0.2.8/pygenda/locale/fr/
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.450005 pygenda-0.2.8/pygenda/locale/fr/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)     8113 2023-07-06 20:42:29.000000 pygenda-0.2.8/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)    58845 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/pygenda_calendar.py
+-rw-------   0 matt      (1000) users      (100)     5450 2023-03-31 11:03:09.000000 pygenda-0.2.8/pygenda/pygenda_config.py
+-rw-------   0 matt      (1000) users      (100)     9909 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/pygenda_dialog_entryprops.py
+-rw-------   0 matt      (1000) users      (100)    64810 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/pygenda_dialog_event.py
+-rw-------   0 matt      (1000) users      (100)     3538 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_dialog_find.py
+-rw-------   0 matt      (1000) users      (100)     5366 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/pygenda_dialog_todo.py
+-rw-------   0 matt      (1000) users      (100)     4146 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_entryinfo.py
+-rw-------   0 matt      (1000) users      (100)    42247 2023-07-06 20:42:29.000000 pygenda-0.2.8/pygenda/pygenda_gui.py
+-rw-------   0 matt      (1000) users      (100)    10419 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_util.py
+-rw-------   0 matt      (1000) users      (100)      300 2023-07-06 20:45:07.000000 pygenda-0.2.8/pygenda/pygenda_version.py
+-rw-------   0 matt      (1000) users      (100)    15418 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_view.py
+-rw-------   0 matt      (1000) users      (100)    26915 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_view_todo.py
+-rw-------   0 matt      (1000) users      (100)    21071 2023-07-05 21:44:54.000000 pygenda-0.2.8/pygenda/pygenda_view_week.py
+-rw-------   0 matt      (1000) users      (100)    27377 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_view_year.py
+-rw-------   0 matt      (1000) users      (100)    22142 2023-06-10 21:22:42.000000 pygenda-0.2.8/pygenda/pygenda_widgets.py
+drwx------   0 matt      (1000) users      (100)        0 2023-07-07 06:43:32.446005 pygenda-0.2.8/pygenda.egg-info/
+-rw-------   0 matt      (1000) users      (100)     1015 2023-07-07 06:43:32.000000 pygenda-0.2.8/pygenda.egg-info/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     1197 2023-07-07 06:43:32.000000 pygenda-0.2.8/pygenda.egg-info/SOURCES.txt
+-rw-------   0 matt      (1000) users      (100)        1 2023-07-07 06:43:32.000000 pygenda-0.2.8/pygenda.egg-info/dependency_links.txt
+-rw-------   0 matt      (1000) users      (100)       54 2023-07-07 06:43:32.000000 pygenda-0.2.8/pygenda.egg-info/requires.txt
+-rw-------   0 matt      (1000) users      (100)        8 2023-07-07 06:43:32.000000 pygenda-0.2.8/pygenda.egg-info/top_level.txt
+-rw-------   0 matt      (1000) users      (100)       38 2023-07-07 06:43:32.451005 pygenda-0.2.8/setup.cfg
+-rwx------   0 matt      (1000) users      (100)     3871 2023-07-06 20:42:29.000000 pygenda-0.2.8/setup.py
```

### Comparing `pygenda-0.2.7/COPYING` & `pygenda-0.2.8/COPYING`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/PKG-INFO` & `pygenda-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.2.7
+Version: 0.2.8
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygenda-0.2.7/README.md` & `pygenda-0.2.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 **WARNING: This is in-development code, released for testing/feedback and
 as a preview for developers. The software is provided as-is, with no
 guarantees. You should back up any files or data used by Pygenda (e.g. iCal
 files or data stored on calendar servers).**
 
 There are currently **lots of missing/incomplete features** as well as
 **bugs**. For a list of known issues, see: [known_issues.md](docs/known_issues.md).
-If you find any new bugs, please send them to: pygenda@semiprime.com.
+If you find any new bugs, please send them to pygenda@semiprime.com,
+or raise them as issues on GitHub.
 
 *However*, it currently has Week, Year and Todo Views that are functional
 enough that the author is now using Pygenda as his main agenda, so
 maybe other people will also find it useful. Feedback is welcome at
 pygenda@semiprime.com – suggestions, questions about how to get something
 working, or just to say that you tried it out.
 
@@ -85,24 +86,24 @@
 
 For more complete settings, see "Configuration", below.
 
 Dependencies
 ------------
 Python3. Version >=3.5 (because Gemini's "Gemian" Linux provides Python 3.5).
 
-* Install on Debian/Gemian: `sudo apt install python3`
+* Install on Debian/Gemian: `sudo apt install python3 python3-pip`
 
 GTK+3
 
 * Install on Debian: `sudo apt install gtk+3`
 
-Python3 modules: PyGObject3 (for gi), icalendar, python-dateutil, tzlocal
+Python3 modules: PyGObject3 (for gi), icalendar, python-dateutil, tzlocal, num2words
 
-* Install on Debian: `sudo apt install python3-gi python3-icalendar python3-dateutil python3-tzlocal`
-* Or install them using pip3: `pip3 install pygobject icalendar python-dateutil tzlocal`
+* Install on Debian: `sudo apt install python3-gi python3-icalendar python3-dateutil python3-tzlocal python3-num2words`
+* Or install them using pip3: `pip3 install [--user] pygobject icalendar python-dateutil tzlocal num2words`
 
 Note: When I tested on Gemian on the Gemini, pip3 installed tzlocal
 version 2.1, which did not work (although versions 1 to 4 worked on a
 Linux laptop). If you get errors like "No such file or directory:
 'getprop'" at startup, try installing a different version of tzlocal
 with either apt or pip3 (v1.5.1 should work on Gemian with Python 3.5).
 
@@ -118,30 +119,30 @@
 
 More information: [docs/config-examples/README.md](docs/config-examples/README.md)
 
 Quick config on Gemini/other handhelds
 --------------------------------------
 If you're running Pygenda on a Gemini or similar PDA, the default font
 sizes will probably not be appropriate for the screen size. To fix
-this, use the custom CSS provided in docs/config-examples/gemini.css.
+this, use the custom CSS provided in pygenda/css/gemini.css.
 The easiest way to do this is to import the gemini.css file from your
 own ~/.config/pygenda/pygenda.css file, by adding the line:
 
 	@import "PATH_TO_GEMINI_CSS_FILE";
 
 You can then add your own custom CSS after this. (This way, if you
 git pull an update to the Pygenda source, then you'll automatically
 get any new css rules included in the new version.)
 
 The "startup/maximized" and "startup/fullscreen" options are also
 useful for devices with small screens. See "Configuration" above.
 
 Desktop/panel/menu launchers
 ----------------------------
-A sample `pygenda.desktop` file is provided in docs/config-examples/.
+A sample `pygenda.desktop` file is provided in pygenda/app/.
 This should help adding launch icons to the desktop menu/panels etc.
 For example, to add Pygenda to the desktop menu, copy (or create a
 link to) the pygenda.desktop file in the `/usr/share/applications/` or
 `~/.local/share/applications/` directory; to add a launcher to the
 LXQt panel, edit the `~/.config/lxqt/panel.conf` file and add a line
 in the [quicklaunch] section (& restart LXQt).
 
@@ -156,12 +157,16 @@
 but a CalDAV server is recommended for real use.
 
 For CalDAV configuration, see: [CalDAV.md](docs/CalDAV.md)
 
 The default ICS file is created in `~/.config/pygenda/pygenda.ics`
 but you can change this from the command line or config file.
 
+Contributing
+------------
+See: [Contributing.md](docs/Contributing.md)
+
 Alternatives
 ------------
 If you want to compare the "competition", the Gemian people also have
 an in-development agenda-like app designed for the Gemini/Cosmo.
 Details at https://gemian.thinkglobally.org/#Calendar
```

### Comparing `pygenda-0.2.7/csrc/pygenda_clipboard.c` & `pygenda-0.2.8/csrc/pygenda_clipboard.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // pygenda_clipboard.c
 //
 // Small C library to interface Pygenda with GTK clipboard.
 // Allows Pygenda entries to be copied to the clipboard.
 // Note: Pasting is done in the Python code (pygenda_gui.py).
 //
-// Copyright (C) 2022 Matthew Lewis
+// Copyright (C) 2022,2023 Matthew Lewis
 //
 // This file is part of Pygenda.
 //
 // Pygenda is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, version 3.
 //
@@ -53,15 +53,15 @@
 // type_idx is set to enumerated value type
 void cb_get_fn(GtkClipboard* clipboard, GtkSelectionData* selection_data, guint type_idx, gpointer ptr) {
 	switch(type_idx) {
 	case DATA_TXT_PLAIN:
 		gtk_selection_data_set_text(selection_data, selectionStr[DATA_TXT_PLAIN], -1);
 		break;
 	case DATA_TXT_CALENDAR:
-		gtk_selection_data_set(selection_data, gdk_atom_intern("text/calendar", FALSE),8,selectionStr[type_idx], strlen(selectionStr[type_idx]));
+		gtk_selection_data_set(selection_data, gdk_atom_intern("text/calendar", FALSE), 8, (guchar*)selectionStr[type_idx], strlen(selectionStr[type_idx]));
 		break;
 	}
 }
 
 // Callback - called when data is no longer needed (e.g. something
 // else is copied)
 void cb_clear_fn(GtkClipboard* clipboard, gpointer ptr) {
```

### Comparing `pygenda-0.2.7/docs/config-examples/gemini.css` & `pygenda-0.2.8/pygenda/css/gemini.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 /*****************************
 gemini.css
 
 Example user CSS file for Planet Computers' Gemini PDA. Include from
 ~/.config/pygenda/pygenda.css or copy & adapt as desired. Should also
 be suitable for similar products such as the Cosmo Communicator.
+
+At some point this may be loaded automatically. However, that will
+depend on code to detect the device, which should be fine, but I'd
+prefer to wait until there's more than one device that gets regular
+testing before adding it!
 ******************************/
 
 /* Remove transition animations - they make Gemini feel slow */
 * {
 	transition-duration:0s;
 	transition-delay:0s;
 }
```

### Comparing `pygenda-0.2.7/pygenda/__main__.py` & `pygenda-0.2.8/pygenda/__main__.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/css/pygenda.css` & `pygenda-0.2.8/pygenda/css/pygenda.css`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/glade/dialog_event.glade` & `pygenda-0.2.8/pygenda/glade/dialog_event.glade`

 * *Files 2% similar despite different names*

#### Comparing `pygenda-0.2.7/pygenda/glade/dialog_event.glade` & `pygenda-0.2.8/pygenda/glade/dialog_event.glade`

```diff
@@ -392,28 +392,26 @@
                         <property name="can-focus">False</property>
                         <property name="halign">start</property>
                         <property name="active">0</property>
                         <items>
                           <item translatable="yes">None</item>
                           <item id="YEARLY" translatable="yes">Yearly</item>
                           <item id="MONTHLY" translatable="yes">Monthly</item>
-                          <item id="MONTHLY-MONTHDAY" translatable="yes">Monthly by day</item>
-                          <item id="MONTHLY-WEEKDAY" translatable="yes">Monthly by weekday</item>
                           <item id="WEEKLY" translatable="yes">Weekly</item>
                           <item id="DAILY" translatable="yes">Daily</item>
                         </items>
                         <signal name="changed" handler="reptype_changed" swapped="no"/>
                       </object>
                       <packing>
                         <property name="left-attach">1</property>
                         <property name="top-attach">0</property>
                       </packing>
                     </child>
                     <child>
-                      <object class="GtkRevealer" id="revealer_repeat_day_l">
+                      <object class="GtkRevealer" id="revealer_repeaton_l">
                         <property name="visible">True</property>
                         <property name="can-focus">False</property>
                         <child>
                           <object class="GtkLabel">
                             <property name="visible">True</property>
                             <property name="can-focus">False</property>
                             <property name="label" translatable="yes">Repeat on:</property>
@@ -426,99 +424,30 @@
                       </object>
                       <packing>
                         <property name="left-attach">0</property>
                         <property name="top-attach">1</property>
                       </packing>
                     </child>
                     <child>
-                      <object class="GtkBox">
+                      <object class="GtkRevealer" id="revealer_repeaton_month">
                         <property name="visible">True</property>
                         <property name="can-focus">False</property>
-                        <property name="orientation">vertical</property>
                         <child>
-                          <object class="GtkRevealer" id="revealer_repeat_monthday_e">
+                          <object class="GtkComboBoxText" id="combo_repeaton_month">
                             <property name="visible">True</property>
                             <property name="can-focus">False</property>
-                            <child>
-                              <object class="GtkComboBoxText" id="combo_bydaymonth">
-                                <property name="visible">True</property>
-                                <property name="can-focus">False</property>
-                                <property name="halign">start</property>
-                                <property name="active">0</property>
-                                <items>
-                                  <item id="-1" translatable="yes">Last day</item>
-                                  <item id="-2" translatable="yes">2nd last day</item>
-                                  <item id="-3" translatable="yes">3rd last day</item>
-                                  <item id="-4" translatable="yes">4th last day</item>
-                                  <item id="-5" translatable="yes">5th last day</item>
-                                  <item id="-6" translatable="yes">6th last day</item>
-                                  <item id="-7" translatable="yes">7th last day</item>
-                                </items>
-                              </object>
-                            </child>
+                            <property name="halign">start</property>
+                            <property name="active">0</property>
+                            <items>
+                              <item id="STD">Xth day of month</item>
+                              <item id="FROMEND">Xth to last day of month</item>
+                              <item id="WEEKDAY">Xth WEEKDAY of month</item>
+                              <item id="WEEKDAY_FROMEND">Xth to last WEEKDAY of month</item>
+                            </items>
                           </object>
-                          <packing>
-                            <property name="expand">False</property>
-                            <property name="fill">True</property>
-                            <property name="position">0</property>
-                          </packing>
-                        </child>
-                        <child>
-                          <object class="GtkRevealer" id="revealer_repeat_weekday_e">
-                            <property name="visible">True</property>
-                            <property name="can-focus">False</property>
-                            <child>
-                              <object class="GtkBox">
-                                <property name="visible">True</property>
-                                <property name="can-focus">False</property>
-                                <child>
-                                  <object class="GtkComboBoxText" id="combo_byday_ord">
-                                    <property name="visible">True</property>
-                                    <property name="can-focus">False</property>
-                                    <property name="halign">start</property>
-                                    <property name="active">0</property>
-                                    <items>
-                                      <item id="1" translatable="yes">1st</item>
-                                      <item id="2" translatable="yes">2nd</item>
-                                      <item id="3" translatable="yes">3rd</item>
-                                      <item id="4" translatable="yes">4th</item>
-                                      <item id="5" translatable="yes">5th</item>
-                                      <item id="-1" translatable="yes">Last</item>
-                                      <item id="-2" translatable="yes">2nd last</item>
-                                      <item id="-3" translatable="yes">3rd last</item>
-                                      <item id="-4" translatable="yes">4th last</item>
-                                      <item id="-5" translatable="yes">5th last</item>
-                                    </items>
-                                  </object>
-                                  <packing>
-                                    <property name="expand">False</property>
-                                    <property name="fill">True</property>
-                                    <property name="position">0</property>
-                                  </packing>
-                                </child>
-                                <child>
-                                  <object class="GtkComboBoxText" id="combo_byday_day">
-                                    <property name="visible">True</property>
-                                    <property name="can-focus">False</property>
-                                    <property name="halign">start</property>
-                                  </object>
-                                  <packing>
-                                    <property name="expand">False</property>
-                                    <property name="fill">True</property>
-                                    <property name="position">1</property>
-                                  </packing>
-                                </child>
-                              </object>
-                            </child>
-                          </object>
-                          <packing>
-                            <property name="expand">False</property>
-                            <property name="fill">True</property>
-                            <property name="position">1</property>
-                          </packing>
                         </child>
                       </object>
                       <packing>
                         <property name="left-attach">1</property>
                         <property name="top-attach">1</property>
                       </packing>
                     </child>
```

### Comparing `pygenda-0.2.7/pygenda/glade/dialog_find.glade` & `pygenda-0.2.8/pygenda/glade/dialog_find.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/glade/dialog_todo.glade` & `pygenda-0.2.8/pygenda/glade/dialog_todo.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/glade/main.glade` & `pygenda-0.2.8/pygenda/glade/main.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/glade/view_week.glade` & `pygenda-0.2.8/pygenda/glade/view_week.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/glade/view_year.glade` & `pygenda-0.2.8/pygenda/glade/view_year.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.mo` & `pygenda-0.2.8/pygenda/locale/fr/LC_MESSAGES/pygenda.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,69 +1,27 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-23 19:39+0200\n"
+"PO-Revision-Date: 2023-07-04 22:46+0200\n"
 "Last-Translator: Matthew Lewis <pygenda@semiprime.com>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid " (timezone: {:s})"
 msgstr " (fuseau horaire : {:s})"
 
 msgid "1 (Highest)"
 msgstr "1 (la plus haute)"
 
-msgid "1st"
-msgstr "1er"
-
-msgid "2nd"
-msgstr "2e"
-
-msgid "2nd last"
-msgstr "2e au dernier"
-
-msgid "2nd last day"
-msgstr "2e au dernier jour"
-
-msgid "3rd"
-msgstr "3e"
-
-msgid "3rd last"
-msgstr "3e au dernier"
-
-msgid "3rd last day"
-msgstr "3e au dernier jour"
-
-msgid "4th"
-msgstr "4e"
-
-msgid "4th last"
-msgstr "4e au dernier"
-
-msgid "4th last day"
-msgstr "4e au dernier jour"
-
-msgid "5th"
-msgstr "5e"
-
-msgid "5th last"
-msgstr "5e au dernier"
-
-msgid "5th last day"
-msgstr "5e au dernier jour"
-
-msgid "6th last day"
-msgstr "6e au dernier jour"
-
-msgid "7th last day"
-msgstr "7e au dernier jour"
+msgid "1st day of month"
+msgstr "1er du mois"
 
 msgid "9 (Lowest)"
 msgstr "9 (la plus basse)"
 
 msgid ":"
 msgstr " :"
 
@@ -131,14 +89,17 @@
 
 msgid "By month:"
 msgstr "Par mois :"
 
 msgid "By second:"
 msgstr "Par seconde :"
 
+msgid "By set position:"
+msgstr "Par position dans série :"
+
 msgid "By week number:"
 msgstr "Par numero de la semaine :"
 
 msgid "By year day:"
 msgstr "Par jour de l’année :"
 
 msgid "Cance_lled"
@@ -269,32 +230,26 @@
 
 msgid "In _progress"
 msgstr "En _cours"
 
 msgid "In progress"
 msgstr "En cours"
 
-msgid "Last"
-msgstr "Dernier"
+msgid "Last day of month"
+msgstr "Dernier jour du mois"
 
-msgid "Last day"
-msgstr "Dernier jour"
+msgid "Last {day:s} of month"
+msgstr "Dernier {day:s} du mois"
 
 msgid "Location:"
 msgstr "Lieu :"
 
 msgid "Monthly"
 msgstr "Mensuelle"
 
-msgid "Monthly by day"
-msgstr "Mensuelle par jour"
-
-msgid "Monthly by weekday"
-msgstr "Mensuelle par jour de la semaine"
-
 msgid "New Event"
 msgstr ""
 "Nouvel\n"
 "évènement"
 
 msgid "New To-do"
 msgstr "Nouvelle tâche"
@@ -337,14 +292,17 @@
 
 msgid "Set _Status"
 msgstr "_Statut"
 
 msgid "Show _Properties"
 msgstr "Afficher _propriétés"
 
+msgid "Source code & documentation: "
+msgstr "Code source et documentation : "
+
 msgid "Start date/time:"
 msgstr "Date/heure de commencement :"
 
 msgid "Start date:"
 msgstr "Date de commencement :"
 
 msgid "Start time:"
@@ -478,9 +436,21 @@
 
 msgid "year_view_accel"
 msgstr "a"
 
 msgid "ymdhm"
 msgstr "amjhm"
 
+msgid "{:s} to last day of month"
+msgstr "{:s} au dernier jour du mois"
+
+msgid "{ord:s} day of month"
+msgstr "{card:d} du mois"
+
+msgid "{ord:s} to last {day:s} of month"
+msgstr "{ord:s} au dernier {day:s} du mois"
+
+msgid "{ord:s} {day:s} of month"
+msgstr "{ord:s} {day:s} du mois"
+
 msgid "“{:s}”"
 msgstr "« {:s} »"
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_calendar.py` & `pygenda-0.2.8/pygenda/pygenda_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,67 +239,48 @@
     def update_entry(cls, en:Union[iEvent,iTodo], e_inf:EntryInfo) -> None:
         # Update entry using details from EntryInfo e_inf.
         clear_rep = False
         clear_norep = False
 
         if 'UID' not in en:
             en.add('UID', Calendar.gen_uid()) # Should be present
+
         # DateTime utcnow() function doesn't include TZ, so use now(tz.utc)
         utcnow =  dt_datetime.now(timezone.utc)
-        try:
-            en['DTSTAMP'].dt = utcnow
-        except KeyError:
-            # Entry had no DTSTAMP (note: DTSTAMP required by icalendar spec)
-            en.add('DTSTAMP', utcnow)
-        try:
-            en['LAST-MODIFIED'].dt = utcnow
-        except KeyError:
-            # Entry had no LAST-MODIFIED - add one
-            en.add('LAST-MODIFIED', utcnow)
-        try:
-            en['SUMMARY'] = e_inf.desc
-        except KeyError:
-            # Entry had no SUMMARY
-            en.add('SUMMARY', e_inf.desc)
-
-        if 'CATEGORIES' in en:
-            del(en['CATEGORIES'])
-        if e_inf.categories:
-            # Convert to list - to work around bug passing set to old icalendar
-            en.add('CATEGORIES', list(e_inf.categories))
-        if 'PRIORITY' in en:
-            del(en['PRIORITY'])
-        if e_inf.priority:
-            en.add('PRIORITY', e_inf.priority)
+        cls._update_entry(en, 'DTSTAMP', utcnow)
+        cls._update_entry(en, 'LAST-MODIFIED', utcnow)
+        cls._update_entry(en, 'SUMMARY', e_inf.desc)
+        cls._update_entry(en, 'PRIORITY', e_inf.priority)
+
+        # For Categories, we need to convert to a list,
+        # to work around bug passing set to old icalendar.
+        cls._update_entry(en, 'CATEGORIES', None if e_inf.categories is None else list(e_inf.categories))
 
         # DTSTART - delete & re-add so type (DATE vs. DATE-TIME) is correct
         # (Also, Q: if comparing DTSTARTs with different TZs, how does != work?)
         had_date = 'DTSTART' in en
         if had_date:
             del(en['DTSTART'])
         if e_inf.start_dt is not None:
             en.add('DTSTART', e_inf.start_dt)
 
         # Duration or Endtime - first delete existing
-        if 'DURATION' in en:
-            del(en['DURATION'])
-        if 'DTEND' in en:
-            del(en['DTEND'])
+        cls._clear_entry(en, 'DURATION')
+        cls._clear_entry(en, 'DTEND')
         # Then add new end time/duration (if needed)
         cls._event_add_end_dur_from_info(en, e_inf)
 
         # Repeats (including exception dates)
         if 'RRULE' in en:
             del(en['RRULE'])
             clear_rep = True
         elif had_date:
             # Previously had start time, but no repeats
             clear_norep = True
-        if 'EXDATE' in en:
-            del(en['EXDATE'])
+        cls._clear_entry(en, 'EXDATE')
         if e_inf.rep_type is not None and e_inf.rep_inter>0:
             cls._event_add_repeat_from_info(en, e_inf)
             clear_rep = True
         elif e_inf.start_dt is not None:
             # Now has start time, but no repeats
             clear_norep = True
 
@@ -321,14 +302,34 @@
         if e_inf.type==EntryInfo.TYPE_TODO or isinstance(en, iTodo):
             cls._todo_list = None
 
         cls.calConnector.update_entry(en) # Write to store
 
 
     @staticmethod
+    def _clear_entry(en:Union[iEvent,iTodo], elname:str) -> None:
+        # Helper function to delete an entry value if it exists.
+        if elname in en:
+            del(en[elname])
+
+
+    @staticmethod
+    def _update_entry(en:Union[iEvent,iTodo], elname:str, val) -> None:
+        # Helper function to update an entry value, or add if it doesn't
+        # exist. Use delete-and-recreate since seems more reliable
+        # (e.g. for datetimes, some combinations of modules lose the
+        # timezone marker if you do en[elname]=val).
+        # Note: if val is None, then existing entry is deleted.
+        if elname in en:
+            del(en[elname])
+        if val is not None:
+	        en.add(elname, val)
+
+
+    @staticmethod
     def _event_add_end_dur_from_info(ev:iEvent, e_inf:EntryInfo) -> None:
         # Adds end time or duration to an event from EntryInfo.
         # How it does this depends on whether event is timed or not
 
         # If entry is timed, check for an end-time/duration & add if present
         # Note: don't add both an end-time & duration - at most one
         if isinstance(e_inf.start_dt, dt_datetime):
@@ -397,24 +398,22 @@
                 del(ev['DTEND'])
                 ev.add('DTEND', end)
 
 
     @staticmethod
     def _entry_set_status_from_info(en:Union[iEvent,iTodo], e_inf:EntryInfo) -> None:
         # Set entry status (cancelled, tentative etc.) from e_inf.
-        if 'STATUS' in en:
-            del(en['STATUS'])
+        Calendar._clear_entry(en, 'STATUS')
         Calendar._add_status_entry(en, e_inf.status)
 
 
     @staticmethod
     def _event_set_location_from_info(ev:iEvent, e_inf:EntryInfo) -> None:
         # Set event location (text string) from e_inf.
-        if 'LOCATION' in ev:
-            del(ev['LOCATION'])
+        Calendar._clear_entry(ev, 'LOCATION')
         if e_inf.location:
             ev.add('LOCATION', e_inf.location)
 
 
     @staticmethod
     def _entry_set_alarms_from_info(en:Union[iEvent,iTodo], e_inf:EntryInfo) -> None:
         # Set entry alarms from e_inf
@@ -474,21 +473,20 @@
 
     @staticmethod
     def _add_status_entry(entry:Union[iEvent,iTodo], stat:Optional[str]) -> None:
         # Set entry STATUS to stat.
         # Assumes entry['STATUS'] does not exist.
         # Only allows spec'ed values.
         if stat=='COMPLETED':
-            if 'PERCENT-COMPLETE' in entry:
-                del(entry['PERCENT-COMPLETE']) # Automatically set to 100
+            # PERCENT-COMPLETE automatically set to 100, so can delete
+            Calendar._clear_entry(entry, 'PERCENT-COMPLETE')
         else:
             if 'PERCENT-COMPLETE' in entry and entry['PERCENT-COMPLETE']==100:
                 entry['PERCENT-COMPLETE'] = 99 # Stop it being == 100
-            if 'COMPLETED' in entry:
-                del(entry['COMPLETED'])
+            Calendar._clear_entry(entry, 'COMPLETED')
         if (isinstance(entry,iEvent) and stat in Calendar.STATUS_LIST_EVENT) or (
             isinstance(entry,iTodo) and stat in Calendar.STATUS_LIST_TODO):
                 entry.add('STATUS', stat)
 
 
     @classmethod
     def _update_entry_norep_list(cls) -> None:
@@ -503,15 +501,15 @@
     @classmethod
     def _update_entry_rep_list(cls) -> None:
         # Re-build _entry_rep_list, if it has been cleared (==None)
         # Possible optimisation: sort most -> least frequent
         # (so don't get last one inserting loads into array) 
         if cls._entry_rep_list is None:
             evs = cls.calConnector.cal.walk('VEVENT')
-            cls._entry_rep_list = [e for e in evs if 'RRULE' in e]
+            cls._entry_rep_list = [e for e in evs if 'RRULE' in e and e['RRULE'] is not None]
 
 
     @classmethod
     def occurrence_list(cls, start:dt_date, stop:dt_date, include_single:bool=True, include_repeated:bool=True) -> list:
         # Return list of occurences in range start <= . < stop.
         # Designed to be called by View classes to get events in range.
         # An "occurrence" is a pair: (event,datetime)
@@ -912,15 +910,19 @@
             raise RepeatUnsupportedError('Unsupported multiple days in BYDAY in RRULE')
         byday_rule = rrule_byday[0]
         try:
             self.byday_day = self.DAY_ABBR.index(byday_rule[-2:])
             self.byday_idx = int(byday_rule[:-2])
         except ValueError:
             raise RepeatUnsupportedError('Unsupported BYDAY {} in MONTHLY/YEARLY repeat'.format(byday_rule))
-        if (self.byday_idx==0 or abs(self.byday_idx)>4):
+        abs_byday = abs(self.byday_idx)
+        if abs_byday==0 or abs_byday>5:
+            print('Notice: Impossible BYDAY rule: {}'.format(byday_rule), file=stderr)
+            raise RepeatImpossibleError()
+        if (abs_byday==5):
             raise RepeatUnsupportedError('Unsupported BYDAY {} in MONTHLY/YEARLY repeat'.format(byday_rule))
         # Test to see if DTSTART matches RRULE
         if self.firstday_to_byweekdayinmonth(self.dtstart.replace(day=1)) != self.dtstart:
             raise RepeatUnsupportedError('Given start date does not match RRULE')
         self._isby_weekday_in_month = True
 
 
@@ -1144,14 +1146,18 @@
         return RepeatIter_simpledelta(self)
 
 
 # Exception used to indicate need to used fallback repeat calculation
 class RepeatUnsupportedError(Exception):
     pass
 
+# Exception used to indicate a repeat can never occur, e.g. 32nd day of Jan
+class RepeatImpossibleError(Exception):
+    pass
+
 
 class RepeatIter_simpledelta:
     # Iterator class for RepeatInfo where we can just use a simple delta.
 
     def __init__(self, rinfo:RepeatInfo):
         self.rinfo = rinfo
         self.dt = rinfo.start_in_rng
@@ -1330,14 +1336,16 @@
 def repeats_in_range(ev:iEvent, start:dt_date, stop:dt_date) -> list:
     # Given a repeating event ev, return list of occurrences from
     # dates start to stop. N.B. start/stop must be dates, not datetimes.
     if isinstance(start,dt_datetime) or isinstance(stop,dt_datetime):
         raise TypeError('Start/stop must be dates, not datetimes')
     try:
         r_info = RepeatInfo(ev, start, stop)
+    except RepeatImpossibleError:
+        return list() # empty list
     except RepeatUnsupportedError as err:
         # RepeatInfo doesn't handle this type of repeat.
         # Fall back to using rrule - more complete, but slower for simple repeats
         print('Notice: Fallback to unoptimised repeat for "{:s}" ({:s})'.format(ev['SUMMARY'],str(err)), file=stderr)
         return repeats_in_range_with_rrstr(ev, start, stop)
     ret = list(iter(r_info))
     # Uncomment the next two lines to test calculated values (slow!)
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_config.py` & `pygenda-0.2.8/pygenda/pygenda_config.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_dialog_entryprops.py` & `pygenda-0.2.8/pygenda/pygenda_dialog_entryprops.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         'BYWEEKNO': 'By week number:',
         'BYYEARDAY': 'By year day:',
         'BYMONTHDAY': 'By month day:',
         'BYDAY': 'By day:',
         'BYHOUR': 'By hour:',
         'BYMINUTE': 'By minute:',
         'BYSECOND': 'By second:',
+        'BYSETPOS': 'By set position:',
         'WKST': 'Week starts:',
         'UNTIL': 'Until:',
         'COUNT': 'Count:'
         }
     STATUS_MAP = {
         'IN-PROCESS': 'In progress',
         'NEEDS-ACTION': 'Action required'
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_dialog_event.py` & `pygenda-0.2.8/pygenda/pygenda_dialog_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 # Pygenda is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
+
+
 from gi import require_version as gi_require_version
 gi_require_version('Gtk', '3.0')
-from gi.repository import Gtk, Gdk, GLib, Gio
+from gi.repository import Gtk, Gdk
 
 from datetime import date as dt_date, time as dt_time, datetime as dt_datetime, timedelta
 from dateutil import rrule as du_rrule
 from dateutil.relativedelta import relativedelta
 from icalendar import Event as iEvent, vRecur
 from sys import stderr
-from typing import Optional, Tuple, List
+from typing import Optional, Union, Tuple, List
 
 # for internationalisation/localisation
-from locale import gettext as _
+from locale import gettext as _, getlocale
 from calendar import day_name, monthrange
+from num2words import num2words
 
 # pygenda components
 from .pygenda_config import Config
 from .pygenda_gui import GUI
 from .pygenda_widgets import WidgetDate, WidgetTime, WidgetDuration
 from .pygenda_calendar import Calendar, RepeatInfo
 from .pygenda_entryinfo import EntryInfo, AlarmInfo
@@ -83,38 +86,32 @@
     wid_allday_count = None # type: Gtk.SpinButton
     _tmdur_handler_time = 0
     _tmdur_handler_dur = 0
     _tmdur_handler_endtime = 0
 
     wid_rep_type = None # type: Gtk.ComboBox
     revs_repeat = None
-    revs_rep_monthdays = None
-    revs_rep_weekdays = None
-    revs_rep_monthweekdays = None
+    revs_repeaton_lab = None
+    revs_repeaton_month = None
     wid_rep_interval = None # type: Gtk.SpinButton
     wid_rep_forever = None # type: Gtk.CheckButton
-    wid_repbymonthday = None # type: Gtk.ComboBox
-    wid_repbyweekday_day = None # type: Gtk.ComboBox
-    wid_repbyweekday_ord = None # type: Gtk.ComboBox
+    wid_repeaton_month = None # type: Gtk.ComboBox
     wid_rep_occs = None # type: Gtk.SpinButton
     wid_rep_enddt = None # type: WidgetDate
     revs_rep_ends = None
     rep_occs_determines_end = True
     _rep_handler_date = 0
+    _rep_handler_date_repon = 0
     _rep_handler_time = 0
     _rep_handler_type = 0
-    _rep_handler_mday = 0
-    _rep_handler_wdayday = 0
-    _rep_handler_wdayord = 0
+    _rep_handler_repon_month = 0
     _rep_handler_inter = 0
     _rep_handler_occs = 0
     _rep_handler_enddt = 0
     _lab_rep_exceptions = None # type: Gtk.Label
-    repbymonthday_initialized = False
-    repbyweekday_initialized = False
     dur_determines_end = False
     exception_list = [] # type: List[dt_date]
 
     wid_alarmstack = None # type: Gtk.Stack
     wid_alarmset = None # type: Gtk.Switch
     _revealer_alarmlist = None # type: Gtk.Revealer
     wid_alarmlist = None # type: Gtk.TreeView
@@ -206,47 +203,37 @@
 
     @classmethod
     def _init_repeatfields(cls) -> None:
         # Initialise widgets etc in the Event dialog under the "Repeats" tab.
         # Called on app startup.
         cls.wid_rep_type = GUI._builder.get_object('combo_repeat_type')
         cls.revs_repeat = cls._revealers_from_ids('revealer_repeat_l','revealer_repeat_e')
-        cls.revs_rep_monthdays = cls._revealers_from_ids('revealer_repeat_monthday_e')
-        cls.revs_rep_weekdays = cls._revealers_from_ids('revealer_repeat_weekday_e')
-        cls.revs_rep_monthweekdays = cls._revealers_from_ids('revealer_repeat_day_l')
+        cls.revs_repeaton_lab = cls._revealers_from_ids('revealer_repeaton_l')
+        cls.revs_repeaton_month = cls._revealers_from_ids('revealer_repeaton_month')
 
         cls.wid_rep_interval = GUI._builder.get_object('repeat_interval')
         cls.wid_rep_forever = GUI._builder.get_object('repeat_forever')
-        cls.wid_repbymonthday = GUI._builder.get_object('combo_bydaymonth')
-        cls.wid_repbyweekday_day = GUI._builder.get_object('combo_byday_day')
-        cls.wid_repbyweekday_ord = GUI._builder.get_object('combo_byday_ord')
+        cls.wid_repeaton_month = GUI._builder.get_object('combo_repeaton_month')
 
         cls.wid_rep_occs = GUI._builder.get_object('repeat_occurrences')
         cls.wid_rep_enddt = WidgetDate()
         rbox = GUI._builder.get_object('revealer_repeat_until_e').get_child() # Should be a GtkBox
         rbox.add(cls.wid_rep_enddt)
         rbox.show_all()
         cls.revs_rep_ends = cls._revealers_from_ids('revealer_repeat_until_l', 'revealer_repeat_until_e')
 
         cls._rep_handler_date = cls.wid_date.connect('changed', cls._repend_changed,0)
+        cls._rep_handler_date_repon = cls.wid_date.connect('changed', cls._repon_changed)
         cls._rep_handler_time = cls.wid_time.connect('changed', cls._repend_changed,0)
         cls._rep_handler_type = cls.wid_rep_type.connect('changed', cls._repend_changed,0)
-        cls._rep_handler_mday = cls.wid_repbymonthday.connect('changed', cls._repend_changed,0)
-        cls._rep_handler_wdayday = cls.wid_repbyweekday_day.connect('changed', cls._repend_changed,0)
-        cls._rep_handler_wdayord = cls.wid_repbyweekday_ord.connect('changed', cls._repend_changed,0)
+        cls._rep_handler_repon_month = cls.wid_repeaton_month.connect('changed', cls._repend_changed,0)
         cls._rep_handler_inter = cls.wid_rep_interval.connect('changed', cls._repend_changed,0)
         cls._rep_handler_occs = cls.wid_rep_occs.connect('changed', cls._repend_changed,1)
         cls._rep_handler_enddt = cls.wid_rep_enddt.connect('changed', cls._repend_changed,2)
 
-        # For repeat on "1st Sat." etc, we fill ComboBox with local day names
-        day = Config.get_int('global','start_week_day')
-        for i in range(7):
-            cls.wid_repbyweekday_day.append(RepeatInfo.DAY_ABBR[day],day_name[day])
-            day = (day+1)%7
-
         # Get label used to display exception dates
         cls._lab_rep_exceptions = GUI._builder.get_object('lab_rep_exceptions')
 
         # We want default to be signal *blocked* - unblock when dialog active
         cls._block_rep_occend_signals()
 
 
@@ -367,48 +354,18 @@
     @classmethod
     def _reptype_changed(cls, wid:Gtk.ComboBox) -> bool:
         # Callback. Called when event repeat type is changed by user.
         # Reveals/hides relevant sub-options.
         # wid should be the repeat-type combobox
         st = wid.get_active()>0
         cls._do_multireveal(cls.revs_repeat, st)
-        monthday = (wid.get_active_id()=='MONTHLY-MONTHDAY')
-        weekday = (wid.get_active_id()=='MONTHLY-WEEKDAY') # Booleans
-        cls._do_multireveal(cls.revs_rep_monthdays, monthday)
-        cls._do_multireveal(cls.revs_rep_weekdays, weekday)
-        cls._do_multireveal(cls.revs_rep_monthweekdays, monthday or weekday)
-        if monthday and not cls.repbymonthday_initialized:
-            # First time shown showing monthday-repeats, so initialise based on start date
-            cls.repbymonthday_initialized = True
-            sdt = cls.get_date_start()
-            if sdt is None: # Fallback in case date is invalid
-                cls.wid_repbymonthday.set_active(0)
-            else:
-                idx = sdt.day - monthrange(sdt.year,sdt.month)[1] - 1
-                if -7 <= idx <= -2:
-                    cls.wid_repbymonthday.set_active_id(str(idx))
-                else:
-                    cls.wid_repbymonthday.set_active(0)
-        elif weekday and not cls.repbyweekday_initialized:
-            # First time shown showing weekday-repeats, so initialise based on start date
-            cls.repbyweekday_initialized = True
-            sdt = cls.get_date_start()
-            if sdt is None: # Fallback in case date is invalid
-                cls.wid_repbyweekday_ord.set_active(0)
-                cls.wid_repbyweekday_day.set_active(0)
-            else:
-                wkst = Config.get_int('global','start_week_day')
-                cls.wid_repbyweekday_day.set_active((sdt.weekday()-wkst)%7)
-                if sdt.day<=21:
-                    # Value will be, e.g. "1st", "2nd" (Tues of month)
-                    cls.wid_repbyweekday_ord.set_active_id(str(1+(sdt.day-1)//7))
-                else:
-                    # Want, e.g. "last" (Friday of month)
-                    rem = monthrange(sdt.year,sdt.month)[1]-sdt.day
-                    cls.wid_repbyweekday_ord.set_active_id(str(-1-(rem//7)))
+        r_monthly = (wid.get_active_id()=='MONTHLY') # Boolean
+        cls._do_multireveal(cls.revs_repeaton_lab, r_monthly)
+        cls._do_multireveal(cls.revs_repeaton_month, r_monthly)
+        # (We assume above that repeat-on combobox is already setup)
         cls._cancel_empty_desc_allowed()
         return True # don't propagate event
 
 
     @classmethod
     def _do_repeatforever_toggle(cls, wid:Gtk.Button) -> bool:
         # Callback. Called when repeat-forever state is changed by user.
@@ -487,36 +444,34 @@
     @classmethod
     def _block_rep_occend_signals(cls) -> None:
         # Function to disable "changed" signals from various widgets that
         # lead to either the end-date or repeat count being re-calculated
         # based on the new values. Generally, keep signals blocked except
         # when the dialog is being shown to the user.
         cls.wid_date.handler_block(cls._rep_handler_date)
+        cls.wid_date.handler_block(cls._rep_handler_date_repon)
         cls.wid_time.handler_block(cls._rep_handler_time)
         cls.wid_rep_type.handler_block(cls._rep_handler_type)
-        cls.wid_repbymonthday.handler_block(cls._rep_handler_mday)
-        cls.wid_repbyweekday_day.handler_block(cls._rep_handler_wdayday)
-        cls.wid_repbyweekday_ord.handler_block(cls._rep_handler_wdayord)
+        cls.wid_repeaton_month.handler_block(cls._rep_handler_repon_month)
         cls.wid_rep_interval.handler_block(cls._rep_handler_inter)
         cls.wid_rep_occs.handler_block(cls._rep_handler_occs)
         cls.wid_rep_enddt.handler_block(cls._rep_handler_enddt)
 
 
     @classmethod
     def _unblock_rep_occend_signals(cls) -> None:
         # Function to re-enable "changed" signals from various widgets that
         # lead to either the end-date or repeat count being re-calculated
         # based on the new values. Generally, unblock when the dialog is
         # being used and user can change these values.
         cls.wid_date.handler_unblock(cls._rep_handler_date)
+        cls.wid_date.handler_unblock(cls._rep_handler_date_repon)
         cls.wid_time.handler_unblock(cls._rep_handler_time)
         cls.wid_rep_type.handler_unblock(cls._rep_handler_type)
-        cls.wid_repbymonthday.handler_unblock(cls._rep_handler_mday)
-        cls.wid_repbyweekday_day.handler_unblock(cls._rep_handler_wdayday)
-        cls.wid_repbyweekday_ord.handler_unblock(cls._rep_handler_wdayord)
+        cls.wid_repeaton_month.handler_unblock(cls._rep_handler_repon_month)
         cls.wid_rep_interval.handler_unblock(cls._rep_handler_inter)
         cls.wid_rep_occs.handler_unblock(cls._rep_handler_occs)
         cls.wid_rep_enddt.handler_unblock(cls._rep_handler_enddt)
 
 
     @classmethod
     def _tmdur_changed(cls, wid:Gtk.Widget, el:int) -> bool:
@@ -580,98 +535,107 @@
         cls.wid_rep_occs.set_range(mn,mx)
 
 
     # Maps used to calculate repeats using dateutil.rrule class
     MAP_RTYPE_TO_RRULE = {
         'YEARLY': du_rrule.YEARLY,
         'MONTHLY': du_rrule.MONTHLY,
-        'MONTHLY-MONTHDAY': du_rrule.MONTHLY,
-        'MONTHLY-WEEKDAY': du_rrule.MONTHLY,
         'WEEKLY': du_rrule.WEEKLY,
         'DAILY': du_rrule.DAILY,
         'HOURLY': du_rrule.HOURLY,
         'MINUTELY': du_rrule.MINUTELY,
         'SECONDLY': du_rrule.SECONDLY
         }
 
-    MAP_RDAY_TO_RRULEDAY = {
-        'MO': du_rrule.MO,
-        'TU': du_rrule.TU,
-        'WE': du_rrule.WE,
-        'TH': du_rrule.TH,
-        'FR': du_rrule.FR,
-        'SA': du_rrule.SA,
-        'SU': du_rrule.SU
-        }
+    MAP_RDAY_TO_RRULEDAY = (
+        du_rrule.MO,
+        du_rrule.TU,
+        du_rrule.WE,
+        du_rrule.TH,
+        du_rrule.FR,
+        du_rrule.SA,
+        du_rrule.SU
+        )
 
     @classmethod
     def _sync_rep_occs_end(cls) -> None:
         # Function to recalculate repeat end-date or occurences count.
         # Called when widgets that might affect repeat counts are updated.
         if cls.wid_rep_forever.get_active():
             return
         rtype = cls.wid_rep_type.get_active_id()
         if rtype is None:
             return
         if cls.rep_occs_determines_end:
-            stdt = cls.get_date_start()
-            if stdt is not None:
-                span = (cls.get_repeat_occurrences()-1) * cls.get_repeat_interval()
-                if rtype=='YEARLY':
-                    if stdt.day==29 and stdt.month==2: # 29th Feb - leap day!
-                        cls._sync_rep_end_from_occ_rrule(rtype)
-                        return
-                    delta = relativedelta(years=span)
-                elif rtype=='MONTHLY':
-                    if cls.get_datetime_start().day>=29:
-                        cls._sync_rep_end_from_occ_rrule(rtype)
-                        return
-                    else:
-                        delta = relativedelta(months=span)
-                elif rtype=='WEEKLY':
-                    delta = timedelta(days=span*7)
-                elif rtype=='DAILY':
-                    delta = timedelta(days=span)
-                elif rtype=='HOURLY':
-                    delta = timedelta(hours=span)
-                elif rtype=='MINUTELY':
-                    delta = timedelta(minutes=span)
-                elif rtype=='SECONDLY':
-                    delta = timedelta(seconds=span)
-                elif rtype in ('MONTHLY-MONTHDAY','MONTHLY-WEEKDAY'):
+            cls._sync_rep_ends_from_occs(rtype)
+        else:
+            cls._sync_occs_from_rep_ends(rtype)
+
+
+    @classmethod
+    def _sync_rep_ends_from_occs(cls, rtype:str) -> None:
+        # Function to recalculate & update repeat End Date
+        # from Occurences count.
+        stdt = cls.get_date_start()
+        if stdt is not None:
+            span = (cls.get_repeat_occurrences()-1) * cls.get_repeat_interval()
+            if rtype=='YEARLY':
+                if stdt.day==29 and stdt.month==2: # 29th Feb - leap day!
                     cls._sync_rep_end_from_occ_rrule(rtype)
                     return
-                else:
-                    # !! Don't know how to sync
-                    print('Warning: Sync for {} not implemented'.format(rtype), file=stderr)
+                delta = relativedelta(years=span) # type:Union[relativedelta,timedelta]
+            elif rtype=='MONTHLY':
+                if stdt.day>=29 or cls.wid_repeaton_month.get_active()>0:
+                    cls._sync_rep_end_from_occ_rrule(rtype)
                     return
-                edt = stdt+delta
-                cls.wid_rep_enddt.set_date(edt)
-        else: # occurrences determined by end date - use dateutil:rrule to calc
-            try:
-                fr = cls.MAP_RTYPE_TO_RRULE[rtype]
-            except KeyError:
+                else:
+                    delta = relativedelta(months=span)
+            elif rtype=='WEEKLY':
+                delta = timedelta(days=span*7)
+            elif rtype=='DAILY':
+                delta = timedelta(days=span)
+            elif rtype=='HOURLY':
+                delta = timedelta(hours=span)
+            elif rtype=='MINUTELY':
+                delta = timedelta(minutes=span)
+            elif rtype=='SECONDLY':
+                delta = timedelta(seconds=span)
+            else:
                 # !! Don't know how to sync
                 print('Warning: Sync for {} not implemented'.format(rtype), file=stderr)
                 return
+            edt = stdt+delta
+            cls.wid_rep_enddt.set_date(edt)
+
+
+    @classmethod
+    def _sync_occs_from_rep_ends(cls, rtype:str) -> None:
+        # Function to recalculate & update repeat Occurences count
+        # from End Date.
+        # Uses dateutil:rrule to do calculation.
+        try:
+            fr = cls.MAP_RTYPE_TO_RRULE[rtype]
+        except KeyError:
+            # !! Don't know how to sync
+            print('Warning: Sync for {} not implemented'.format(rtype), file=stderr)
+            return
+        if rtype=='MONTHLY':
+            bymtdy,bywkdy = cls._get_monthly_bymonthday_byweekday()
+        else:
             bymtdy = None
             bywkdy = None
-            if rtype=='MONTHLY-MONTHDAY':
-                bymtdy = cls._get_cal_monthday_rep()
-            elif rtype=='MONTHLY-WEEKDAY':
-                bywkdy = cls._get_cal_weekday_rep()
-            dtst = cls.get_date_start() # Without time, because time breaks calc
-            interv = cls.get_repeat_interval()
-            rend = cls.wid_rep_enddt.get_date_or_none()
-            if dtst is not None and rend is not None:
-                rr = du_rrule.rrule(fr, dtstart=dtst, interval=interv, until=rend, byweekday=bywkdy, bymonthday=bymtdy)
-                c = rr.count()
-                if c>=0:
-                    cls._set_occs_min(0 if c==0 else 1) # possibly allow "0"
-                    cls.wid_rep_occs.set_value(c)
+        dtst = cls.get_date_start() # Without time, because time breaks calc
+        interv = cls.get_repeat_interval()
+        rend = cls.wid_rep_enddt.get_date_or_none()
+        if dtst is not None and rend is not None:
+            rr = du_rrule.rrule(fr, dtstart=dtst, interval=interv, until=rend, byweekday=bywkdy, bymonthday=bymtdy)
+            c = rr.count()
+            if c>=0:
+                cls._set_occs_min(0 if c==0 else 1) # possibly allow "0"
+                cls.wid_rep_occs.set_value(c)
 
 
     @classmethod
     def _sync_rep_end_from_occ_rrule(cls, rtype:str) -> None:
         # Function to synchronise End Date repeat field from Occurrences in
         # complex situations, e.g. leapday (29 Feb) or monthly late in month.
         # Use rrule class for these.
@@ -682,38 +646,79 @@
             print('Warning: Sync for {} not implemented'.format(rtype), file=stderr)
             return
         dtst = cls.get_datetime_start()
         if dtst is None:
             return
         interv = cls.get_repeat_interval()
         occs = cls.get_repeat_occurrences()
-        bymtdy = None
-        bywkdy = None
-        if rtype=='MONTHLY-MONTHDAY':
-            bymtdy = cls._get_cal_monthday_rep()
-        elif rtype=='MONTHLY-WEEKDAY':
-            bywkdy = cls._get_cal_weekday_rep()
+        if rtype=='MONTHLY':
+            bymtdy,bywkdy = cls._get_monthly_bymonthday_byweekday()
+        else:
+            bymtdy = None
+            bywkdy = None
         rr = du_rrule.rrule(fr, dtstart=dtst, interval=interv, count=occs, byweekday=bywkdy, bymonthday=bymtdy)
         edt = list(rr)[-1]
         cls.wid_rep_enddt.set_date(edt)
 
 
     @classmethod
-    def _get_cal_monthday_rep(cls) -> int:
-        # Return value for monthday repeats to pass to rrule
-        retd = int(cls.wid_repbymonthday.get_active_id())
-        return retd
+    def _get_monthly_bymonthday_byweekday(cls) -> Tuple:
+        # Return bymonthday & byweekday for monthday repeats to pass to rrule
+        repon = cls.wid_repeaton_month.get_active_id()
+        dtst = cls.get_date_start()
+        bymtdy = None
+        bywkdy = None
+        if dtst is not None:
+            if repon=='FROMEND':
+                bymtdy = dtst.day - monthrange(dtst.year,dtst.month)[1] - 1
+            elif repon=='WEEKDAY':
+                dayocc = (dtst.day+6)//7
+                bywkdy = cls.MAP_RDAY_TO_RRULEDAY[dtst.weekday()](dayocc)
+            elif repon=='WEEKDAY_FROMEND':
+                dayocc = (dtst.day-monthrange(dtst.year,dtst.month)[1]-1)//7
+                bywkdy = cls.MAP_RDAY_TO_RRULEDAY[dtst.weekday()](dayocc)
+        return bymtdy,bywkdy
+
+
+    @classmethod
+    def _repon_changed(cls, wid:Gtk.Widget) -> bool:
+        # Handler for signals from any widget that might result in the
+        # text of the repeat on field to change. Rewrites text.
+        cls._block_rep_occend_signals()
+        cls._repon_wid_datesync()
+        cls._unblock_rep_occend_signals()
+        return True # don't propagate event
 
 
     @classmethod
-    def _get_cal_weekday_rep(cls) -> du_rrule.weekday:
-        # Return rrule structure for weekday repeats.
-        # E.g. MO(-2) = "2nd last Monday"
-        rrwd = cls.MAP_RDAY_TO_RRULEDAY[cls.wid_repbyweekday_day.get_active_id()](int(cls.wid_repbyweekday_ord.get_active_id()))
-        return rrwd
+    def _repon_wid_datesync(cls) -> None:
+        # Rewrites text of repeat-on monthly widget to reflect start date.
+        # Note: Should be called with signals blocked, o/w get side-effects.
+        dt = cls.wid_date.get_date_or_none()
+        if dt is None:
+            return # invalid date (eg 31st Feb)
+        active = cls.wid_repeaton_month.get_active() # save current value
+        fromend = monthrange(dt.year,dt.month)[1] - dt.day
+        daynm = day_name[dt.weekday()]
+        lang = getlocale()[0]
+        cls.wid_repeaton_month.remove_all()
+        if dt.day==1:
+            cls.wid_repeaton_month.append('STD',_('1st day of month'))
+        else:
+            cls.wid_repeaton_month.append('STD',_('{ord:s} day of month').format(ord=num2words(dt.day,to='ordinal_num',lang=lang),card=dt.day))
+        if fromend == 0:
+            cls.wid_repeaton_month.append('FROMEND',_('Last day of month'))
+        else:
+            cls.wid_repeaton_month.append('FROMEND',_('{:s} to last day of month').format(num2words(fromend+1,to='ordinal_num',lang=lang)))
+        cls.wid_repeaton_month.append('WEEKDAY',_('{ord:s} {day:s} of month').format(ord=num2words((dt.day+6)//7,to='ordinal_num',lang=lang),day=daynm))
+        if fromend < 7:
+	        cls.wid_repeaton_month.append('WEEKDAY_FROMEND',_('Last {day:s} of month').format(day=daynm))
+        else:
+	        cls.wid_repeaton_month.append('WEEKDAY_FROMEND',_('{ord:s} to last {day:s} of month').format(ord=num2words(fromend//7+1,to='ordinal_num',lang=lang),day=daynm))
+        cls.wid_repeaton_month.set_active(active) # restore saved value
 
 
     @classmethod
     def new_event(cls, txt:str=None, date:dt_date=None) -> None:
         # Called to implement "new event" from GUI, e.g. menu
         cls.dialog.set_title(_('New Event'))
         cls._empty_desc_allowed = True # initially allowed, can switch to False
@@ -782,14 +787,15 @@
 
         # Two cases: new event or edit existing event
         if event is None:
             # Initialise decscription field
             cls._seed_text_only(txt)
         else: # existing entry - take values
             cls._seed_from_event(event)
+        cls._repon_wid_datesync() # Do this at end, so date used is correct
 
         cls._seed_rep_exception_list(event) # If event==None this clears exlist
 
 
     @classmethod
     def _set_fields_to_defaults(cls, date:Optional[dt_date]) -> None:
         # Set dialog fields to default values
@@ -808,16 +814,15 @@
         cls.wid_dur.set_duration(timedelta(0))
         cls.wid_endtime.set_time(tm9)
         cls.dur_determines_end = True
         cls.wid_allday_count.set_value(1)
 
         # Repeats tab
         cls.wid_rep_type.set_active(0) # Sends signal to hide fields
-        cls.repbymonthday_initialized = False # Init these later when we can
-        cls.repbyweekday_initialized = False  # choose appropriate values.
+        cls.wid_repeaton_month.set_active(0)
         cls.wid_rep_interval.set_value(1)
         cls.wid_rep_forever.set_active(True)
         cls.rep_occs_determines_end = True
         cls.wid_rep_occs.set_value(1)
         cls._set_occs_min(1)
         # No need to set wid_rep_enddt because it will be synced when revealed
 
@@ -843,15 +848,15 @@
             cls.wid_desc.set_position(len(txt))
             cls.wid_desc.handler_unblock(cls._wid_desc_changed_handler)
         cls.wid_desc.grab_focus_without_selecting()
 
 
     @classmethod
     def _seed_from_event(cls, event:iEvent) -> None:
-        # Called when dialog is opened for en existing event.
+        # Called when dialog is opened for an existing event.
         # Assume defaults already set before this is called.
 
         if 'SUMMARY' in event:
             cls.wid_desc.set_text(event['SUMMARY'])
         cls.wid_desc.grab_focus() # also selects text in field
 
         # Date & Time tab
@@ -873,15 +878,15 @@
             cls.wid_location.set_text(event['LOCATION'])
 
         cls._sync_rep_occs_end()
 
 
     @classmethod
     def _seed_date_timetab(cls, event:iEvent) -> None:
-        # Called when dialog is opened for en existing event.
+        # Called when dialog is opened for an existing event.
         # Seeds the date field and the time tab (inc. all-day events).
         dt = event['DTSTART'].dt
         dttm = None
         tm = None
         dur = None
         end_dttm = None
         if isinstance(dt,dt_datetime):
@@ -932,38 +937,30 @@
             # Set both fields in dialog. Values have been made to match above.
             cls.wid_dur.set_duration(dur)
             cls.wid_endtime.set_time(end_dttm.time())
 
 
     @classmethod
     def _seed_repeatstab(cls, rrule:vRecur) -> None:
-        # Called when dialog is opened for en existing event.
+        # Called when dialog is opened for an existing event.
         # Assumes that start date has already been set from event.
         rrfreq = rrule['FREQ'][0]
-        if rrfreq == 'MONTHLY' and 'BYDAY' in rrule:
-            cls.wid_rep_type.set_active_id('MONTHLY-WEEKDAY')
-            if len(rrule['BYDAY']) > 1:
-                raise EventPropertyBeyondEditDialog('Editing MONTHLY repeat with multiple \'BYDAY\' not (yet) supported')
-            byday = rrule['BYDAY'][0]
-            cls.repbyweekday_initialized = True
-            cls.wid_repbyweekday_ord.set_active_id(byday[1 if byday[0]=='+' else 0:-2])
-            cls.wid_repbyweekday_day.set_active_id(byday[-2:])
-        elif rrfreq == 'MONTHLY' and 'BYMONTHDAY' in rrule:
-            if len(rrule['BYMONTHDAY'])!=1:
-                raise EventPropertyBeyondEditDialog('Editing repeat with multiple \'BYMONTHDAY\' not (yet) supported')
-            cls.wid_rep_type.set_active_id('MONTHLY-MONTHDAY')
-            bymday = rrule['BYMONTHDAY'][0]
-            if not(-7 <= int(bymday) <= -1):
-                raise EventPropertyBeyondEditDialog('Editing repeat with BYMONTHDAY={} not (yet) supported'.format(bymday))
-            cls.wid_repbymonthday.set_active_id(str(bymday))
-            cls.repbymonthday_initialized = True
-        elif rrfreq in ('YEARLY','MONTHLY','WEEKLY','DAILY'):
+        if rrfreq in ('YEARLY','MONTHLY','WEEKLY','DAILY'):
             cls.wid_rep_type.set_active_id(rrfreq)
         else:
             raise EventPropertyBeyondEditDialog('Editing repeat freq \'{}\' not (yet) supported'.format(rrfreq))
+
+        if rrfreq == 'MONTHLY':
+            cls._seed_reptab_monthly(rrule)
+
+        if rrfreq == 'WEEKLY' and 'BYDAY' in rrule:
+            rr_byday = rrule['BYDAY']
+            if isinstance(rr_byday, list) and len(rr_byday)>1:
+                raise EventPropertyBeyondEditDialog('Editing WEEKLY repeat with multiple \'BYDAY\' not (yet) supported')
+
         cls.wid_rep_interval.set_value(int(rrule['INTERVAL'][0]) if 'INTERVAL' in rrule else 1)
         if 'COUNT' in rrule:
             cls.wid_rep_forever.set_active(False)
             c = rrule['COUNT'][0]
             cls.wid_rep_occs.set_value(c if c>=1 else 1)
             cls.rep_occs_determines_end = True
         elif 'UNTIL' in rrule:
@@ -971,18 +968,61 @@
             u = rrule['UNTIL'][0]
             if isinstance(u,dt_datetime):
                 u = u.date()
             dt_st = cls.get_date_start() # Won't be none, because seeded
             cls.wid_rep_enddt.set_date(u if u>dt_st else dt_st)
             cls.rep_occs_determines_end = False
 
-        if rrfreq == 'WEEKLY' and 'BYDAY' in rrule:
-            rr_byday = rrule['BYDAY']
-            if isinstance(rr_byday, list) and len(rr_byday)>1:
-                raise EventPropertyBeyondEditDialog('Editing WEEKLY repeat with multiple \'BYDAY\' not (yet) supported')
+
+    @classmethod
+    def _seed_reptab_monthly(cls, rrule:vRecur) -> None:
+        # Called when dialog is opened for a monthly repeating event
+        has_byday = 'BYDAY' in rrule
+        has_bymonthday = 'BYMONTHDAY' in rrule
+        if has_byday and has_bymonthday:
+            raise EventPropertyBeyondEditDialog('MONTHLY repeat has both BYDAY and BYMONTHDAY')
+        if has_byday:
+            byday = rrule['BYDAY']
+            if len(byday) > 1:
+                raise EventPropertyBeyondEditDialog('Editing MONTHLY repeat with multiple \'BYDAY\' not (yet) supported')
+            byday = byday[0]
+            byday_day = byday[-2:]
+            dt_st = cls.get_date_start() # Won't be none, because seeded
+            if RepeatInfo.DAY_ABBR[dt_st.weekday()]!= byday_day:
+                raise EventPropertyBeyondEditDialog('Repeat BYDAY does not match start date')
+            try:
+                byday_ord = int(byday[0:-2])
+            except ValueError:
+                raise EventPropertyBeyondEditDialog('Non-integer value for BYDAY')
+            if byday_ord > 0:
+                if byday_ord != (dt_st.day+6)//7:
+                    raise EventPropertyBeyondEditDialog('Repeat BYDAY does not match start date')
+                cls.wid_repeaton_month.set_active_id('WEEKDAY')
+            else: # byday_ord<0
+                if byday_ord != (dt_st.day-monthrange(dt_st.year,dt_st.month)[1]-1)//7:
+                    raise EventPropertyBeyondEditDialog('Repeat BYDAY does not match start date')
+                cls.wid_repeaton_month.set_active_id('WEEKDAY_FROMEND')
+        elif has_bymonthday:
+            bymday = rrule['BYMONTHDAY']
+            if len(bymday)!=1:
+                raise EventPropertyBeyondEditDialog('Editing MONTHLY repeat with multiple \'BYMONTHDAY\' not (yet) supported')
+            try:
+                bymday = int(bymday[0])
+            except ValueError:
+                raise EventPropertyBeyondEditDialog('Non-integer value for BYMONTHDAY')
+            dt_st = cls.get_date_start() # Won't be none, because seeded
+            if bymday>=0:
+                if dt_st.day != bymday:
+                    raise EventPropertyBeyondEditDialog('Repeat BYMONTHDAY does not match start date')
+                # No need to set repeaton value - default works
+            else: # bymday < 0
+                dt_st_fromend = dt_st.day - monthrange(dt_st.year,dt_st.month)[1] - 1
+                if dt_st_fromend != bymday:
+                    raise EventPropertyBeyondEditDialog('Repeat BYMONTHDAY does not match start date')
+                cls.wid_repeaton_month.set_active_id('FROMEND')
 
 
     @classmethod
     def _seed_rep_exception_list(cls, event:iEvent) -> None:
         # Sets & displays repeat exception list from event parameter.
         # Called from _seed_fields() when dialog is opened.
         cls._set_rep_exception_list(event)
@@ -1052,42 +1092,59 @@
             d = max(1,int(cls.wid_allday_count.get_value()))
             ei.set_end_dt(dt+timedelta(days=d))
         elif cls.dur_determines_end:
             ei.set_duration(cls.wid_dur.get_duration_or_none())
         else:
             ei.set_end_dt(cls.wid_endtime.get_time_or_none())
 
-        # repeat information
+        # Repeat information
+        cls._fillin_repeatinfo(ei)
+
+        # Alarm info
+        if cls.wid_alarmset.get_active():
+            for al in cls.alarmlist_model:
+                ei.add_alarm(al[0])
+
+        return ei
+
+
+    @classmethod
+    def _fillin_repeatinfo(cls, ei:EntryInfo) -> None:
+        # Add repeat info from dialog to ei
         reptype = cls.wid_rep_type.get_active_id()
         if reptype is not None:
             inter = cls.get_repeat_interval()
+            # Repeat type details, e.g. monthly, 2nd Monday of month
+            byday = None
+            bymonthday = None # type: Optional[str]
+            if reptype=='MONTHLY':
+                repon = cls.wid_repeaton_month.get_active_id()
+                dt = cls.get_date_start()
+                if dt is not None:
+                    if repon=='FROMEND':
+                        bymonthday = dt.day - monthrange(dt.year,dt.month)[1] - 1 # type: ignore
+                        bymonthday = str(bymonthday)
+                    elif repon=='WEEKDAY':
+                        dayocc = (dt.day+6)//7
+                        dayabbr = RepeatInfo.DAY_ABBR[dt.weekday()]
+                        byday = str(dayocc)+dayabbr # e.g. '2SU' - 2nd Sunday
+                    elif repon=='WEEKDAY_FROMEND':
+                        dayoccn = (dt.day-monthrange(dt.year,dt.month)[1]-1)//7
+                        dayabbr = RepeatInfo.DAY_ABBR[dt.weekday()]
+                        byday = str(dayoccn)+dayabbr # e.g. '-2MO' - 2nd last Monday
+            # If not "repeat forever", when repeats stop
             count = None
             until = None
-            byday = None
-            bymonthday = None
-            if reptype=='MONTHLY-WEEKDAY':
-                reptype = 'MONTHLY'
-                byday = cls.wid_repbyweekday_ord.get_active_id() + cls.wid_repbyweekday_day.get_active_id()
-            elif reptype=='MONTHLY-MONTHDAY':
-                reptype = 'MONTHLY'
-                bymonthday = cls.wid_repbymonthday.get_active_id()
             if not cls.wid_rep_forever.get_active():
                 if cls.rep_occs_determines_end:
                     count = cls.get_repeat_occurrences()
                 else:
                     until = cls.wid_rep_enddt.get_date_or_none()
             ei.set_repeat_info(reptype, interval=inter, count=count, until=until, bymonthday=bymonthday, byday=byday, except_list=cls._get_exceptions_list_for_type())
 
-        # Alarm info
-        if cls.wid_alarmset.get_active():
-            for al in cls.alarmlist_model:
-                ei.add_alarm(al[0])
-
-        return ei
-
 
     @classmethod
     def _get_exceptions_list_for_type(cls) -> Optional[list]:
         # Return exceptions list transformed to match event.
         # E.g. if a timed event, return timed exceptions.
         if len(cls.exception_list)==0:
             return None
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_dialog_find.py` & `pygenda-0.2.8/pygenda/pygenda_dialog_find.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_dialog_todo.py` & `pygenda-0.2.8/pygenda/pygenda_dialog_todo.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
 from gi import require_version as gi_require_version
 gi_require_version('Gtk', '3.0')
-from gi.repository import Gtk, Gdk, GLib, Gio
+from gi.repository import Gtk, Gdk
 
 from icalendar import Todo as iTodo
 from locale import gettext as _
 from typing import Optional, Tuple
 
 # pygenda components
 from .pygenda_gui import GUI
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_entryinfo.py` & `pygenda-0.2.8/pygenda/pygenda_entryinfo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_gui.py` & `pygenda-0.2.8/pygenda/pygenda_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
 from gi import require_version as gi_require_version
 gi_require_version('Gtk', '3.0')
-from gi.repository import Gtk, Gdk, GLib, Gio
+from gi.repository import Gtk, Gdk, GdkPixbuf, GLib, Gio
 
 from datetime import date as dt_date, time as dt_time, datetime as dt_datetime, timedelta
 from icalendar import Calendar as iCalendar, Event as iEvent, Todo as iTodo
 from importlib import import_module
 from os import path as ospath
 from sys import stderr
 import signal
@@ -472,15 +472,15 @@
             sb.connect('key-press-event', cls._spinbutton_keypress)
             sb.connect('focus-out-event', cls._focusout_unhighlight)
 
 
     @classmethod
     def _init_comboboxes(cls) -> None:
         # Connect ComboBox events to handlers for extra features.
-        for cb_id in ('combo_repeat_type','combo_bydaymonth','combo_byday_ord','combo_byday_day','combo_status','combo_todo_list','combo_todo_priority','combo_todo_status'):
+        for cb_id in ('combo_repeat_type','combo_repeaton_month','combo_status','combo_todo_list','combo_todo_priority','combo_todo_status'):
             cb = cls._builder.get_object(cb_id)
             cb.connect('key-press-event', cls._combobox_keypress)
 
 
     @classmethod
     def _init_entryboxes(cls) -> None:
         # Connect Entry textbox events to handlers for extra features.
@@ -943,15 +943,19 @@
     @classmethod
     def dialog_about(cls, *args) -> bool:
         # Display the "About Pygenda" dialog
         dialog = Gtk.AboutDialog(parent=cls._window)
         dialog.set_program_name('Pygenda')
         dialog.set_copyright(u'Copyright © 2022,2023 Matthew Lewis')
         dialog.set_license_type(Gtk.License.GPL_3_0_ONLY)
-        dialog.set_logo_icon_name('x-office-calendar')
+        github_url = 'https://github.com/semiprime/pygenda'
+        dialog.set_website(github_url)
+        dialog.set_website_label(_('Source code & documentation: ')+github_url)
+        logo = GdkPixbuf.Pixbuf.new(GdkPixbuf.Colorspace.RGB, True, 8, 1, 1)
+        dialog.set_logo(logo)
         dialog.set_authors(('Matthew Lewis',))
         dialog.set_version('version {:s}'.format(__version__))
         dialog.set_comments(_(u'A calendar/agenda application written in Python/GTK3. The UI is inspired by the Agenda apps on the Psion Series 3 and Series 5 PDAs.\nWARNING: This is in-development code, released for testing and feedback. There will be bugs; please report them to: pygenda@semiprime.com.'))
         dialog.show_all()
         dialog.run()
         dialog.destroy()
         return True # don't propagate event
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_util.py` & `pygenda-0.2.8/pygenda/pygenda_util.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_view.py` & `pygenda-0.2.8/pygenda/pygenda_view.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_view_todo.py` & `pygenda-0.2.8/pygenda/pygenda_view_todo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_view_week.py` & `pygenda-0.2.8/pygenda/pygenda_view_week.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             cls._scroll_to_cursor_in_day = dy # to be read in draw handler
         else:
             cls._scroll_to_cursor_in_day = None
         GUI.set_menu_elts(on_event=(ecount!=0)) # Enable/disable hide menu items
 
 
     @classmethod
-    def _pre_datecontent_draw(cls, wid:Gtk.Widget, _, day:int) -> bool:
+    def _pre_datecontent_draw(cls, wid:Gtk.Widget, cairo_ctx, day:int) -> bool:
         # Callback called on 'draw' event on date_content.
         # Called before drawing date content.
         # Used to scroll window when cursor has been moved (since we
         # need to have calculated the layout to know where to scoll to).
         if cls._scroll_to_cursor_in_day == day:
             cls.scroll_to_row(cls._day_rows[day], View._cursor_idx_in_date, cls._day_scroll[day])
             cls._scroll_to_cursor_in_day = None
```

### Comparing `pygenda-0.2.7/pygenda/pygenda_view_year.py` & `pygenda-0.2.8/pygenda/pygenda_view_year.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda/pygenda_widgets.py` & `pygenda-0.2.8/pygenda/pygenda_widgets.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.7/pygenda.egg-info/PKG-INFO` & `pygenda-0.2.8/pygenda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.2.7
+Version: 0.2.8
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygenda-0.2.7/setup.py` & `pygenda-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 #
 
+# Example usage:
+#   ./setup.py install [--user]
+#   ./setup.py develop [--user]
+#   ./setup.py sdist
+#   ./setup.py bdist_wheel --plat-name=[linux-x86_64|linux-aarch64]
+
+
 from setuptools import setup
 from setuptools.command.bdist_egg import bdist_egg
 from sys import platform
 import subprocess
 from os import path as ospath
 
 
@@ -36,14 +43,15 @@
 
     @staticmethod
     def make_clipboard_library():
         # Only know how to do this on Linux - needs fixing for other platforms
         if platform == 'linux':
             print("Compiling clipboard library...")
             cdir = '{:s}/csrc'.format(ospath.dirname(__file__))
+            subprocess.run(['cmake','.'], cwd=cdir)
             subprocess.run(['make','clean'], cwd=cdir)
             subprocess.run(['make'], cwd=cdir)
             print("Copying clipboard library...")
             subprocess.run(['make','cp'], cwd=cdir)
         else:
             print("Don't know how to build clipboard library on this platform.\nSkipping.")
 
@@ -65,23 +73,24 @@
     url = "https://github.com/semiprime/pygenda",
     author = "Matthew Lewis",
     author_email = "pygenda@semiprime.com",
     description = "An agenda application inspired by Agenda programs on Psion PDAs.",
     long_description = "Pygenda is a calendar/agenda application written in Python3/GTK3. The UI is inspired by the Agenda programs on the Psion Series 3 and Series 5 range of keyboard PDAs, with the aim of being suitable for devices such as Planet Computers' Gemini (running Linux).\n\nFor more information/latest source, see https://github.com/semiprime/pygenda",
     packages = ["pygenda"],
     cmdclass = {'bdist_egg': PygendaEggInstall}, # use custom install above
-    package_data={'': ['glade/*.glade', 'css/pygenda.css', 'css/*.svg', 'libpygenda_clipboard.so', 'locale/*/LC_MESSAGES/pygenda.mo', '../docs/*.md', '../docs/config-examples/*.md', '../docs/config-examples/*.ini', '../docs/config-examples/*.css', '../docs/config-examples/pygenda.desktop']},
+    package_data = {'': ['glade/*.glade', 'css/*.css', 'css/*.svg', 'libpygenda_clipboard.so', 'locale/*/LC_MESSAGES/pygenda.mo', 'app/pygenda.desktop']}, # files for bdists
     license = "GPLv3 only",
     python_requires = ">=3.5",
     setup_requires = ["pycairo"], # For PyGObject
     install_requires = [
         "PyGObject",
         "python-dateutil",
         "icalendar",
         "tzlocal",
+        "num2words",
     ],
     classifiers = [
         "Development Status :: 3 - Alpha",
         "Environment :: Handhelds/PDA's",
         "Environment :: X11 Applications :: GTK",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
```

