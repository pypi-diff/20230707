# Comparing `tmp/city_score-0.1.1.tar.gz` & `tmp/city_score-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "city_score-0.1.1.tar", last modified: Wed Jul  5 21:33:57 2023, max compression
+gzip compressed data, was "city_score-0.1.2.tar", last modified: Thu Jul  6 23:07:55 2023, max compression
```

## Comparing `city_score-0.1.1.tar` & `city_score-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.294854 city_score-0.1.1/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1071 2023-07-04 20:59:48.000000 city_score-0.1.1/LICENSE
--rw-r--r--   0 jacobbudin   (501) staff       (20)     5154 2023-07-05 21:33:57.294729 city_score-0.1.1/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)     3040 2023-07-04 20:59:48.000000 city_score-0.1.1/README.md
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1217 2023-07-05 21:19:40.000000 city_score-0.1.1/pyproject.toml
--rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-07-05 21:33:57.294890 city_score-0.1.1/setup.cfg
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.291664 city_score-0.1.1/src/
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.293224 city_score-0.1.1/src/city_score/
--rw-r--r--   0 jacobbudin   (501) staff       (20)       27 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)       22 2023-07-05 21:33:46.000000 city_score-0.1.1/src/city_score/__version__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1683 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/app.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)      155 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/cache.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1739 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/city.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1478 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/decorators.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2663 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/printers.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1499 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/source.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.294551 city_score-0.1.1/src/city_score/sources/
--rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/__init__.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1108 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/core.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1509 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/peopleforbikes.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2786 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/snowpak.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     1269 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/yelp.py
--rw-r--r--   0 jacobbudin   (501) staff       (20)     2048 2023-07-04 20:59:48.000000 city_score-0.1.1/src/city_score/sources/zillow.py
-drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-05 21:33:57.293801 city_score-0.1.1/src/city_score.egg-info/
--rw-r--r--   0 jacobbudin   (501) staff       (20)     5154 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/PKG-INFO
--rw-r--r--   0 jacobbudin   (501) staff       (20)      633 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/SOURCES.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/dependency_links.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       75 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/requires.txt
--rw-r--r--   0 jacobbudin   (501) staff       (20)       11 2023-07-05 21:33:57.000000 city_score-0.1.1/src/city_score.egg-info/top_level.txt
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-06 23:07:55.672851 city_score-0.1.2/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1071 2023-07-04 20:59:48.000000 city_score-0.1.2/LICENSE
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     5196 2023-07-06 23:07:55.672709 city_score-0.1.2/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     3083 2023-07-06 23:05:12.000000 city_score-0.1.2/README.md
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1217 2023-07-05 21:19:40.000000 city_score-0.1.2/pyproject.toml
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       38 2023-07-06 23:07:55.672884 city_score-0.1.2/setup.cfg
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-06 23:07:55.669211 city_score-0.1.2/src/
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-06 23:07:55.671116 city_score-0.1.2/src/city_score/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       27 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       22 2023-07-06 23:07:03.000000 city_score-0.1.2/src/city_score/__version__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1683 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/app.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      155 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/cache.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1739 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/city.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1478 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/decorators.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2663 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/printers.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1499 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/source.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-06 23:07:55.672497 city_score-0.1.2/src/city_score/sources/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        0 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/__init__.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1108 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/core.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1509 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/peopleforbikes.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2786 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/snowpak.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     1269 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/yelp.py
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     2048 2023-07-04 20:59:48.000000 city_score-0.1.2/src/city_score/sources/zillow.py
+drwxr-xr-x   0 jacobbudin   (501) staff       (20)        0 2023-07-06 23:07:55.671778 city_score-0.1.2/src/city_score.egg-info/
+-rw-r--r--   0 jacobbudin   (501) staff       (20)     5196 2023-07-06 23:07:55.000000 city_score-0.1.2/src/city_score.egg-info/PKG-INFO
+-rw-r--r--   0 jacobbudin   (501) staff       (20)      633 2023-07-06 23:07:55.000000 city_score-0.1.2/src/city_score.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)        1 2023-07-06 23:07:55.000000 city_score-0.1.2/src/city_score.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       75 2023-07-06 23:07:55.000000 city_score-0.1.2/src/city_score.egg-info/requires.txt
+-rw-r--r--   0 jacobbudin   (501) staff       (20)       11 2023-07-06 23:07:55.000000 city_score-0.1.2/src/city_score.egg-info/top_level.txt
```

### Comparing `city_score-0.1.1/LICENSE` & `city_score-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/PKG-INFO` & `city_score-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city_score
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line application for scoring US cities and towns.
 Maintainer-email: Jacob Budin <self@jacobbudin.com>
 License: The MIT License
         
         Copyright (c) 2023 Jacob Budin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -106,14 +106,15 @@
 1. Download City Score from PyPI:
     ```
     $ python3 -m pip install city_score
     ```
 2. Create a script (`myscore.py`) like this:
     ```python
     from city_score import run
+    from city_score.sources.core import *
     from city_score.sources.peopleforbikes import *
     from city_score.sources.zillow import *
 
     sources = (
         PeopleForBikes,
         Zillow,
     )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: city_score Version: 0.1.1 Summary: A command-line
+Metadata-Version: 2.1 Name: city_score Version: 0.1.2 Summary: A command-line
 application for scoring US cities and towns. Maintainer-email: Jacob Budin
 jacobbudin.com> License: The MIT License Copyright (c) 2023 Jacob Budin
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -44,19 +44,20 @@
 allow users to easily add and remix data - Outputs prettified to the console or
 to CSV, HTML, JSON, JSONL ## Design City Score uses a three-step process: 1.
 Qualification: criteria identify cities that meet your minimum standard. 2.
 Scoring: scorers score facets of your choosing at various weights. 3.
 Generation: dimensions appear in the final output. ## Quick start 1. Download
 City Score from PyPI: ``` $ python3 -m pip install city_score ``` 2. Create a
 script (`myscore.py`) like this: ```python from city_score import run from
-city_score.sources.peopleforbikes import * from city_score.sources.zillow
-import * sources = ( PeopleForBikes, Zillow, ) criteria = ( minimum_bike_score
-(25), minimum_population(60000), maximum_median_home_price(1000000),
-prohibited_states(('TX', 'FL', 'CO', )), ) scorers = ( median_home_price_scorer
-(lower=350000, upper=800000), bike_score_scorer(lower=40, upper=80, weight=2),
-) dimensions = ( population, median_home_price, median_rent, bike_score, ) run
-(sources, criteria, scorers, dimensions) ``` 3. Run your script: ``` $ python3
-myscore.py --sort=score --scale-scores ``` ## Data sources - ð²
-PeopleForBikes provides a score for biking infrastructure. - ð Snowpak
-provides the name and location of most ski resorts. - ð Yelp provides data
-on many points of interest, including businesses. - ð¡ Zillow provides
-estimates for home and rent prices. ## License MIT License
+city_score.sources.core import * from city_score.sources.peopleforbikes import
+* from city_score.sources.zillow import * sources = ( PeopleForBikes, Zillow, )
+criteria = ( minimum_bike_score(25), minimum_population(60000),
+maximum_median_home_price(1000000), prohibited_states(('TX', 'FL', 'CO', )), )
+scorers = ( median_home_price_scorer(lower=350000, upper=800000),
+bike_score_scorer(lower=40, upper=80, weight=2), ) dimensions = ( population,
+median_home_price, median_rent, bike_score, ) run(sources, criteria, scorers,
+dimensions) ``` 3. Run your script: ``` $ python3 myscore.py --sort=score --
+scale-scores ``` ## Data sources - ð² PeopleForBikes provides a score for
+biking infrastructure. - ð Snowpak provides the name and location of most
+ski resorts. - ð Yelp provides data on many points of interest, including
+businesses. - ð¡ Zillow provides estimates for home and rent prices. ##
+License MIT License
```

### Comparing `city_score-0.1.1/README.md` & `city_score-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 1. Download City Score from PyPI:
     ```
     $ python3 -m pip install city_score
     ```
 2. Create a script (`myscore.py`) like this:
     ```python
     from city_score import run
+    from city_score.sources.core import *
     from city_score.sources.peopleforbikes import *
     from city_score.sources.zillow import *
 
     sources = (
         PeopleForBikes,
         Zillow,
     )
@@ -104,8 +105,8 @@
 ## Data sources
 - 🚲 PeopleForBikes provides a score for biking infrastructure.
 - 🏂 Snowpak provides the name and location of most ski resorts.
 - 🍕 Yelp provides data on many points of interest, including businesses.
 - 🏡 Zillow provides estimates for home and rent prices.
 
 ## License
-MIT License
+MIT License
```

#### html2text {}

```diff
@@ -18,19 +18,20 @@
 allow users to easily add and remix data - Outputs prettified to the console or
 to CSV, HTML, JSON, JSONL ## Design City Score uses a three-step process: 1.
 Qualification: criteria identify cities that meet your minimum standard. 2.
 Scoring: scorers score facets of your choosing at various weights. 3.
 Generation: dimensions appear in the final output. ## Quick start 1. Download
 City Score from PyPI: ``` $ python3 -m pip install city_score ``` 2. Create a
 script (`myscore.py`) like this: ```python from city_score import run from
-city_score.sources.peopleforbikes import * from city_score.sources.zillow
-import * sources = ( PeopleForBikes, Zillow, ) criteria = ( minimum_bike_score
-(25), minimum_population(60000), maximum_median_home_price(1000000),
-prohibited_states(('TX', 'FL', 'CO', )), ) scorers = ( median_home_price_scorer
-(lower=350000, upper=800000), bike_score_scorer(lower=40, upper=80, weight=2),
-) dimensions = ( population, median_home_price, median_rent, bike_score, ) run
-(sources, criteria, scorers, dimensions) ``` 3. Run your script: ``` $ python3
-myscore.py --sort=score --scale-scores ``` ## Data sources - ð²
-PeopleForBikes provides a score for biking infrastructure. - ð Snowpak
-provides the name and location of most ski resorts. - ð Yelp provides data
-on many points of interest, including businesses. - ð¡ Zillow provides
-estimates for home and rent prices. ## License MIT License
+city_score.sources.core import * from city_score.sources.peopleforbikes import
+* from city_score.sources.zillow import * sources = ( PeopleForBikes, Zillow, )
+criteria = ( minimum_bike_score(25), minimum_population(60000),
+maximum_median_home_price(1000000), prohibited_states(('TX', 'FL', 'CO', )), )
+scorers = ( median_home_price_scorer(lower=350000, upper=800000),
+bike_score_scorer(lower=40, upper=80, weight=2), ) dimensions = ( population,
+median_home_price, median_rent, bike_score, ) run(sources, criteria, scorers,
+dimensions) ``` 3. Run your script: ``` $ python3 myscore.py --sort=score --
+scale-scores ``` ## Data sources - ð² PeopleForBikes provides a score for
+biking infrastructure. - ð Snowpak provides the name and location of most
+ski resorts. - ð Yelp provides data on many points of interest, including
+businesses. - ð¡ Zillow provides estimates for home and rent prices. ##
+License MIT License
```

### Comparing `city_score-0.1.1/pyproject.toml` & `city_score-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/app.py` & `city_score-0.1.2/src/city_score/app.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/city.py` & `city_score-0.1.2/src/city_score/city.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/decorators.py` & `city_score-0.1.2/src/city_score/decorators.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/printers.py` & `city_score-0.1.2/src/city_score/printers.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/source.py` & `city_score-0.1.2/src/city_score/source.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/sources/core.py` & `city_score-0.1.2/src/city_score/sources/core.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/sources/peopleforbikes.py` & `city_score-0.1.2/src/city_score/sources/peopleforbikes.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/sources/snowpak.py` & `city_score-0.1.2/src/city_score/sources/snowpak.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/sources/yelp.py` & `city_score-0.1.2/src/city_score/sources/yelp.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score/sources/zillow.py` & `city_score-0.1.2/src/city_score/sources/zillow.py`

 * *Files identical despite different names*

### Comparing `city_score-0.1.1/src/city_score.egg-info/PKG-INFO` & `city_score-0.1.2/src/city_score.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city-score
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line application for scoring US cities and towns.
 Maintainer-email: Jacob Budin <self@jacobbudin.com>
 License: The MIT License
         
         Copyright (c) 2023 Jacob Budin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -106,14 +106,15 @@
 1. Download City Score from PyPI:
     ```
     $ python3 -m pip install city_score
     ```
 2. Create a script (`myscore.py`) like this:
     ```python
     from city_score import run
+    from city_score.sources.core import *
     from city_score.sources.peopleforbikes import *
     from city_score.sources.zillow import *
 
     sources = (
         PeopleForBikes,
         Zillow,
     )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: city-score Version: 0.1.1 Summary: A command-line
+Metadata-Version: 2.1 Name: city-score Version: 0.1.2 Summary: A command-line
 application for scoring US cities and towns. Maintainer-email: Jacob Budin
 jacobbudin.com> License: The MIT License Copyright (c) 2023 Jacob Budin
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -44,19 +44,20 @@
 allow users to easily add and remix data - Outputs prettified to the console or
 to CSV, HTML, JSON, JSONL ## Design City Score uses a three-step process: 1.
 Qualification: criteria identify cities that meet your minimum standard. 2.
 Scoring: scorers score facets of your choosing at various weights. 3.
 Generation: dimensions appear in the final output. ## Quick start 1. Download
 City Score from PyPI: ``` $ python3 -m pip install city_score ``` 2. Create a
 script (`myscore.py`) like this: ```python from city_score import run from
-city_score.sources.peopleforbikes import * from city_score.sources.zillow
-import * sources = ( PeopleForBikes, Zillow, ) criteria = ( minimum_bike_score
-(25), minimum_population(60000), maximum_median_home_price(1000000),
-prohibited_states(('TX', 'FL', 'CO', )), ) scorers = ( median_home_price_scorer
-(lower=350000, upper=800000), bike_score_scorer(lower=40, upper=80, weight=2),
-) dimensions = ( population, median_home_price, median_rent, bike_score, ) run
-(sources, criteria, scorers, dimensions) ``` 3. Run your script: ``` $ python3
-myscore.py --sort=score --scale-scores ``` ## Data sources - ð²
-PeopleForBikes provides a score for biking infrastructure. - ð Snowpak
-provides the name and location of most ski resorts. - ð Yelp provides data
-on many points of interest, including businesses. - ð¡ Zillow provides
-estimates for home and rent prices. ## License MIT License
+city_score.sources.core import * from city_score.sources.peopleforbikes import
+* from city_score.sources.zillow import * sources = ( PeopleForBikes, Zillow, )
+criteria = ( minimum_bike_score(25), minimum_population(60000),
+maximum_median_home_price(1000000), prohibited_states(('TX', 'FL', 'CO', )), )
+scorers = ( median_home_price_scorer(lower=350000, upper=800000),
+bike_score_scorer(lower=40, upper=80, weight=2), ) dimensions = ( population,
+median_home_price, median_rent, bike_score, ) run(sources, criteria, scorers,
+dimensions) ``` 3. Run your script: ``` $ python3 myscore.py --sort=score --
+scale-scores ``` ## Data sources - ð² PeopleForBikes provides a score for
+biking infrastructure. - ð Snowpak provides the name and location of most
+ski resorts. - ð Yelp provides data on many points of interest, including
+businesses. - ð¡ Zillow provides estimates for home and rent prices. ##
+License MIT License
```

### Comparing `city_score-0.1.1/src/city_score.egg-info/SOURCES.txt` & `city_score-0.1.2/src/city_score.egg-info/SOURCES.txt`

 * *Files identical despite different names*

