# Comparing `tmp/ordotools-0.0.5.tar.gz` & `tmp/ordotools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ordotools-0.0.5.tar", last modified: Fri Jul  7 18:26:48 2023, max compression
+gzip compressed data, was "ordotools-0.0.6.tar", last modified: Fri Jul  7 19:37:28 2023, max compression
```

## Comparing `ordotools-0.0.5.tar` & `ordotools-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.261293 ordotools-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-07-07 18:26:48.261293 ordotools-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-07-07 18:26:36.000000 ordotools-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.249293 ordotools-0.0.5/ordotools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.249293 ordotools-0.0.5/ordotools/ordotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-07-07 18:26:48.000000 ordotools-0.0.5/ordotools/ordotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 18:26:48.000000 ordotools-0.0.5/ordotools/ordotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:26:48.000000 ordotools-0.0.5/ordotools/ordotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:26:48.000000 ordotools-0.0.5/ordotools/ordotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 18:26:48.000000 ordotools-0.0.5/ordotools/ordotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.253293 ordotools-0.0.5/ordotools/sanctoral/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.253293 ordotools-0.0.5/ordotools/sanctoral/country/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/country/australiae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/country/nameofcountry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.253293 ordotools-0.0.5/ordotools/sanctoral/diocese/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/bathurstensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/lismorensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/maitlandensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/melbournensis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/nameofdiocese.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/rockhamptonensis.py
--rw-r--r--   0 runner    (1001) docker     (123)   193907 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/sanctoral/diocese/roman.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:48.261293 ordotools-0.0.5/ordotools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/OLD_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    93647 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/feast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/liturgical_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/parts.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-07-07 18:26:36.000000 ordotools-0.0.5/ordotools/tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:26:48.261293 ordotools-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-07 18:26:36.000000 ordotools-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 19:37:28.179049 ordotools-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-07 19:37:17.000000 ordotools-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/ordotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:37:28.000000 ordotools-0.0.6/ordotools/ordotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/sanctoral/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.175048 ordotools-0.0.6/ordotools/sanctoral/country/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/australiae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/country/nameofcountry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/ordotools/sanctoral/diocese/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/bathurstensis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/lismorensis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/maitlandensis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/melbournensis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/nameofdiocese.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/rockhamptonensis.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193907 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/sanctoral/diocese/roman.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/ordotools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/OLD_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93647 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/feast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/liturgical_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-07-07 19:37:17.000000 ordotools-0.0.6/ordotools/tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 19:37:17.000000 ordotools-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:37:28.179049 ordotools-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 19:37:17.000000 ordotools-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:37:28.179049 ordotools-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-07 19:37:17.000000 ordotools-0.0.6/tests/test.py
```

### Comparing `ordotools-0.0.5/ordotools/ordotools.egg-info/SOURCES.txt` & `ordotools-0.0.6/ordotools/ordotools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+pyproject.toml
 setup.py
 ordotools/ordotools.egg-info/PKG-INFO
 ordotools/ordotools.egg-info/SOURCES.txt
 ordotools/ordotools.egg-info/dependency_links.txt
 ordotools/ordotools.egg-info/requires.txt
 ordotools/ordotools.egg-info/top_level.txt
 ordotools/sanctoral/__init__.py
@@ -24,8 +25,9 @@
 ordotools/tools/feast.py
 ordotools/tools/helpers.py
 ordotools/tools/liturgical_dates.py
 ordotools/tools/logger.py
 ordotools/tools/outputs.py
 ordotools/tools/parts.py
 ordotools/tools/settings.py
-ordotools/tools/temporal.py
+ordotools/tools/temporal.py
+tests/test.py
```

### Comparing `ordotools-0.0.5/ordotools/sanctoral/country/australiae.py` & `ordotools-0.0.6/ordotools/sanctoral/country/australiae.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/country/nameofcountry.py` & `ordotools-0.0.6/ordotools/sanctoral/country/nameofcountry.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/bathurstensis.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/bathurstensis.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/lismorensis.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/lismorensis.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/maitlandensis.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/maitlandensis.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/melbournensis.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/melbournensis.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/nameofdiocese.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/nameofdiocese.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/rockhamptonensis.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/rockhamptonensis.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/sanctoral/diocese/roman.py` & `ordotools-0.0.6/ordotools/sanctoral/diocese/roman.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/OLD_temporal.py` & `ordotools-0.0.6/ordotools/tools/OLD_temporal.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/algorithm.py` & `ordotools-0.0.6/ordotools/tools/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from importlib import import_module
 
 from tools.feast import Feast
 
-from tools.helpers import FIRST_ADVENT
-from tools.helpers import LAST_ADVENT
-from tools.helpers import LENT_BEGINS
-from tools.helpers import LENT_ENDS
+from tools.helpers import LiturgicalYearMarks
 from tools.helpers import days
 from tools.helpers import ladys_office
 from tools.helpers import leap_year
 
 from tools.liturgical_dates import integer_to_roman
 
 from tools.temporal import Temporal
@@ -20,14 +17,18 @@
 class LiturgicalCalendar:
 
     def __init__(self, year, diocese, country=""):
         self.year = year
         self.diocese = diocese
         self.transfers = None
         self.temporal = Temporal(self.year).return_temporal()
+        self.FIRST_ADVENT = LiturgicalYearMarks(self.year).first_advent
+        self.LAST_ADVENT = LiturgicalYearMarks(self.year).last_advent
+        self.LENT_BEGINS = LiturgicalYearMarks(self.year).lent_begins
+        self.LENT_ENDS = LiturgicalYearMarks(self.year).lent_ends
 
     def explode_octaves(self, feast: Feast) -> dict:
         """
         Generates "explodes" the octave for a feast.
         """
         octave = {}
         for x in range(7):
@@ -171,17 +172,17 @@
         Adds Office of the BVM to the compiled calendar.
         """
         # TODO: add Mass number according to season
         year = calendar.copy()
         office = ladys_office
         for feast in year.keys():
             if feast.strftime("%w") == str(6):
-                if LENT_BEGINS.date() <= feast.date() <= LENT_ENDS.date():
+                if self.LENT_BEGINS.date() <= feast.date() <= self.LENT_ENDS.date():
                     continue
-                elif FIRST_ADVENT.date() <= feast.date() <= LAST_ADVENT.date():
+                elif self.FIRST_ADVENT.date() <= feast.date() <= self.LAST_ADVENT.date():
                     continue
                 else:
                     if year[feast]["rank"][0] > 16:  # not a double
                         year[feast] = office  # TODO: add commemorations
                     else:
                         continue
         return year
```

### Comparing `ordotools-0.0.5/ordotools/tools/data.py` & `ordotools-0.0.6/ordotools/tools/data.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/feast.py` & `ordotools-0.0.6/ordotools/tools/feast.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/helpers.py` & `ordotools-0.0.6/ordotools/tools/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 from datetime import datetime
 from datetime import timedelta
 
-from tools.settings import YEAR
-
 import dateutil.easter
 
 import re
 
 
+class LiturgicalYearMarks:
+    def __init__(self, year):
+        self.christmas = datetime.strptime(str(self.year) + "-12-25", "%Y-%m-%d")
+        self.first_advent = self.christmas - findsunday(self.christmas) - timedelta(weeks=3)
+        self.last_advent = self.christmas - timedelta(days=1)
+        self.easter_season_start = easter(self.year) - timedelta(weeks=6, days=4)
+        self.lent_begins = easter(self.year) - timedelta(weeks=6, days=4)
+        self.lent_ends = easter(self.year) - timedelta(days=1)
+        self.easter = easter(self.year)
+        self.easter_season_end = easter(self.year) + timedelta(days=39)
+        self.pentecost_season_start = easter(self.year) + timedelta(days=49)
+        self.pentecost_season_end = self.first_advent - timedelta(days=1)
+
+
+
 def findsunday(date: datetime) -> timedelta:
     """
     return the distance betweent the date and
     the previous Sunday, as timedelta.days
     """
     return timedelta(days=int(date.strftime('%w')))
 
@@ -21,34 +34,14 @@
     return datetime(
         year=int(dateutil.easter.easter(year).strftime('%Y')),
         month=int(dateutil.easter.easter(year).strftime('%m')),
         day=int(dateutil.easter.easter(year).strftime('%d'))
     )
 
 
-CHRISTMAS = datetime.strptime(str(YEAR) + "-12-25", "%Y-%m-%d")
-
-FIRST_ADVENT = CHRISTMAS - findsunday(CHRISTMAS) - timedelta(weeks=3)
-
-LAST_ADVENT = CHRISTMAS - timedelta(days=1)
-
-EASTER_SEASON_START = easter(YEAR) - timedelta(weeks=6, days=4)
-
-LENT_BEGINS = easter(YEAR) - timedelta(weeks=6, days=4)
-
-LENT_ENDS = easter(YEAR) - timedelta(days=1)
-
-EASTER = easter(YEAR)
-
-EASTER_SEASON_END = easter(YEAR) + timedelta(days=39)
-
-PENTECOST_SEASON_START = easter(YEAR) + timedelta(days=49)
-
-PENTECOST_SEASON_END = FIRST_ADVENT - timedelta(days=1)
-
 ladys_office = {
     "feast": "De Sancta Maria in Sabbato",
     "rank": [21, "s"],
     "color": "white",
     "mass": {
         "int": "Salve sancta parens",
         "glo": True,
```

### Comparing `ordotools-0.0.5/ordotools/tools/liturgical_dates.py` & `ordotools-0.0.6/ordotools/tools/liturgical_dates.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/logger.py` & `ordotools-0.0.6/ordotools/tools/logger.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/outputs.py` & `ordotools-0.0.6/ordotools/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/parts.py` & `ordotools-0.0.6/ordotools/tools/parts.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/ordotools/tools/temporal.py` & `ordotools-0.0.6/ordotools/tools/temporal.py`

 * *Files identical despite different names*

### Comparing `ordotools-0.0.5/setup.py` & `ordotools-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="ordotools",
-    version="0.0.5",
+    version="0.0.6",
     description="A set of tools for producing a traditional Catholic Ordo, given a year and diocese",
     package_dir={"": "ordotools"},
     packages=find_packages(where="ordotools"),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/corei8/Ordo",
+    url="https://github.com/corei8/ordotools",
     author="corei8 (Fr. G.R.Barnes)",
     author_email="corei8.github@gmail.com",
     license="GNU",
-    # classifiers=[]
+    classifiers=[
+        "Programming Language :: Python :: 3"
+    ],
     install_requires=[
-        "dateutil"
+        "python-dateutil"
     ],
     python_requires=">=3.7",
 )
```

