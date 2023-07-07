# Comparing `tmp/when-2.0.0.tar.gz` & `tmp/when-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "when-2.0.0.tar", last modified: Thu Feb 23 00:32:07 2023, max compression
+gzip compressed data, was "when-3.0.0.tar", last modified: Fri Jul  7 09:31:37 2023, max compression
```

## Comparing `when-2.0.0.tar` & `when-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.322404 when-2.0.0/
--rw-r--r--   0 david      (501) staff       (20)     1071 2023-02-11 08:57:18.000000 when-2.0.0/LICENSE
--rw-r--r--   0 david      (501) staff       (20)       35 2023-02-11 08:57:18.000000 when-2.0.0/MANIFEST.in
--rw-r--r--   0 david      (501) staff       (20)     5097 2023-02-23 00:32:07.322668 when-2.0.0/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     4046 2023-02-11 08:57:18.000000 when-2.0.0/README.rst
--rw-r--r--   0 david      (501) staff       (20)      421 2023-02-23 00:32:07.323987 when-2.0.0/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)     1577 2023-02-23 00:31:18.000000 when-2.0.0/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.306883 when-2.0.0/src/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.313830 when-2.0.0/src/when/
--rw-r--r--   0 david      (501) staff       (20)      276 2023-02-11 08:57:18.000000 when-2.0.0/src/when/__init__.py
--rwxr-xr-x   0 david      (501) staff       (20)      167 2023-02-11 08:57:18.000000 when-2.0.0/src/when/__main__.py
--rw-r--r--   0 david      (501) staff       (20)     4283 2023-02-11 08:57:18.000000 when-2.0.0/src/when/core.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.320409 when-2.0.0/src/when/db/
--rw-r--r--   0 david      (501) staff       (20)        0 2023-02-11 08:57:18.000000 when-2.0.0/src/when/db/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     4316 2023-02-11 08:57:18.000000 when-2.0.0/src/when/db/client.py
--rw-r--r--   0 david      (501) staff       (20)     4786 2023-02-11 08:57:18.000000 when-2.0.0/src/when/db/make.py
--rw-r--r--   0 david      (501) staff       (20)     1477 2023-02-11 08:57:18.000000 when-2.0.0/src/when/lunar.py
--rwxr-xr-x   0 david      (501) staff       (20)     8199 2023-02-12 05:00:48.000000 when-2.0.0/src/when/main.py
--rw-r--r--   0 david      (501) staff       (20)    15938 2023-02-11 08:57:18.000000 when-2.0.0/src/when/timezones.py
--rw-r--r--   0 david      (501) staff       (20)     2591 2023-02-11 08:57:18.000000 when-2.0.0/src/when/utils.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.318407 when-2.0.0/src/when.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     5097 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      493 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       44 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/entry_points.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2021-09-04 13:50:47.000000 when-2.0.0/src/when.egg-info/not-zip-safe
--rw-r--r--   0 david      (501) staff       (20)       32 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)        5 2023-02-23 00:32:07.000000 when-2.0.0/src/when.egg-info/top_level.txt
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-02-23 00:32:07.321360 when-2.0.0/tests/
--rw-r--r--   0 david      (501) staff       (20)     4238 2023-02-12 05:01:13.000000 when-2.0.0/tests/test_when.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.263886 when-3.0.0/
+-rw-r--r--   0 david      (501) staff       (20)     1071 2023-02-11 08:57:18.000000 when-3.0.0/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)       35 2023-02-11 08:57:18.000000 when-3.0.0/MANIFEST.in
+-rw-r--r--   0 david      (501) staff       (20)     4277 2023-07-07 09:31:37.264243 when-3.0.0/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     3189 2023-07-06 12:00:52.000000 when-3.0.0/README.rst
+-rw-r--r--   0 david      (501) staff       (20)       31 2023-07-05 22:47:35.000000 when-3.0.0/pyproject.toml
+-rw-r--r--   0 david      (501) staff       (20)      421 2023-07-07 09:31:37.266070 when-3.0.0/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)     1624 2023-07-06 02:56:50.000000 when-3.0.0/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.245646 when-3.0.0/src/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.254630 when-3.0.0/src/when/
+-rw-r--r--   0 david      (501) staff       (20)      313 2023-07-05 23:08:42.000000 when-3.0.0/src/when/__init__.py
+-rwxr-xr-x   0 david      (501) staff       (20)      158 2023-03-19 08:36:59.000000 when-3.0.0/src/when/__main__.py
+-rwxr-xr-x   0 david      (501) staff       (20)     5429 2023-07-06 09:03:13.000000 when-3.0.0/src/when/cli.py
+-rw-r--r--   0 david      (501) staff       (20)    15647 2023-07-06 09:04:45.000000 when-3.0.0/src/when/config.py
+-rw-r--r--   0 david      (501) staff       (20)    10513 2023-07-06 11:27:14.000000 when-3.0.0/src/when/core.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.261804 when-3.0.0/src/when/db/
+-rw-r--r--   0 david      (501) staff       (20)        0 2023-02-11 08:57:18.000000 when-3.0.0/src/when/db/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     4269 2023-07-05 22:47:45.000000 when-3.0.0/src/when/db/client.py
+-rw-r--r--   0 david      (501) staff       (20)     4708 2023-07-05 22:47:45.000000 when-3.0.0/src/when/db/make.py
+-rw-r--r--   0 david      (501) staff       (20)    15883 2023-07-05 22:47:45.000000 when-3.0.0/src/when/timezones.py
+-rw-r--r--   0 david      (501) staff       (20)     2124 2023-07-06 11:29:31.000000 when-3.0.0/src/when/utils.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.259649 when-3.0.0/src/when.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     4277 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      508 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)       44 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/entry_points.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2021-09-04 13:50:47.000000 when-3.0.0/src/when.egg-info/not-zip-safe
+-rw-r--r--   0 david      (501) staff       (20)       45 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)        5 2023-07-07 09:31:37.000000 when-3.0.0/src/when.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-07 09:31:37.263018 when-3.0.0/tests/
+-rw-r--r--   0 david      (501) staff       (20)     4163 2023-07-05 22:58:08.000000 when-3.0.0/tests/test_when.py
```

### Comparing `when-2.0.0/LICENSE` & `when-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `when-2.0.0/setup.py` & `when-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from setuptools import setup, find_packages
 import os
 import sys
 
 
-with open('README.rst') as fp:
+with open("README.rst") as fp:
     long_description = fp.read()
 
 
 local_ctx = {}
-with open('src/when/__init__.py') as fp:
+with open("src/when/__init__.py") as fp:
     exec(fp.read(), {}, local_ctx)
 
 
 setup(
-    name='when',
-    version=local_ctx['VERSION'],
-    description=local_ctx['__doc__'],
-    license='MIT',
+    name="when",
+    version=local_ctx["VERSION"],
+    description=local_ctx["__doc__"],
+    license="MIT",
     long_description=long_description,
-    long_description_content_type='text/x-rst',
-    author='David Krauth',
-    author_email='dakrauth@gmail.com',
-    url='https://github.com/dakrauth/when',
-    python_requires='>=3.7,<4',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
+    long_description_content_type="text/x-rst",
+    author="David Krauth",
+    author_email="dakrauth@gmail.com",
+    url="https://github.com/dakrauth/when",
+    python_requires=">=3.8,<4",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     include_package_data=True,
-    entry_points={'console_scripts': ['when = when.__main__:main',]},
-    install_requires=['python-dateutil>=2.8.0', 'requests'],
+    entry_points={"console_scripts": ["when = when.__main__:main",]},
+    install_requires=[
+        "python-dateutil>=2.8.0",
+        "toml>=0.10.2",
+        "requests",
+    ],
     classifiers=[
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: POSIX',
-        'Operating System :: Unix',
-        'Operating System :: MacOS :: MacOS X',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: System :: Software Distribution',
-        'Topic :: Utilities',
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: System :: Software Distribution",
+        "Topic :: Utilities",
     ],
     zip_safe=False,
 )
```

### Comparing `when-2.0.0/src/when/db/client.py` & `when-3.0.0/src/when/db/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import sys
 import sqlite3
 import logging
 from collections import namedtuple
 from pathlib import Path
 
 from .. import utils
 
@@ -32,15 +31,15 @@
 SELECT c.id, c.name, c.ascii, c.co, c.sub, c.tz
 FROM city c
 WHERE
     c.id = :value OR
     {}
 """
 
-MISSING_DB = f"""
+MISSING_DB = """
 The when database is not currently available. You can generate it easily
 (assuming you have internet access) by issuing the following command:
 
     when --db
 
 For details, see:
 
@@ -51,15 +50,15 @@
 class City(namedtuple("City", ["id", "name", "ascii", "co", "sub", "tz"])):
     __slots__ = ()
     sub_number_re = re.compile(r"\d")
 
     def __str__(self):
         bits = [self.name, self.co]
         if not self.sub_number_re.search(self.sub):
-            bits.append(self.sub)
+            bits.insert(1, self.sub)
 
         return ", ".join(bits)
 
     def __repr__(self):
         return f"City({self.ascii},{self.sub},{self.co} {self.tz})"
 
 
@@ -142,17 +141,15 @@
             bits = [a.strip() for a in value.split(",")]
             nbits = len(bits)
             if nbits == 2:
                 value, co = bits
                 like_exprs = [f"({bit} AND c.co = :co)" for bit in like_exprs]
             elif nbits == 3:
                 value, sub, co = bits
-                like_exprs = [
-                    f"({bit} AND c.co = :co AND c.sub = :sub)" for bit in like_exprs
-                ]
+                like_exprs = [f"({bit} AND c.co = :co AND c.sub = :sub)" for bit in like_exprs]
             elif nbits > 4:
                 raise ValueError(f"Invalid search expression: {value}")
 
             like_exprs = " OR ".join(like_exprs)
             sql = SEARCH_QUERY.format(like_exprs)
             dct = {
                 "like": f"%{value}%",
```

### Comparing `when-2.0.0/src/when/db/make.py` & `when-3.0.0/src/when/db/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,19 +103,15 @@
                 mod,
             ) = line.rstrip().split("\t")
 
             pop = int(pop) if pop else 0
             if (
                 (fcode in skip)
                 or (fcode in skip_if and (pop < minimum_population))
-                or (
-                    fcode == "PPLA5"
-                    and name.startswith("Marseille")
-                    and name[-1].isdigit()
-                )
+                or (fcode == "PPLA5" and name.startswith("Marseille") and name[-1].isdigit())
             ):
                 skipped[fcode] += 1
                 continue
 
             fcodes[fcode] += 1
             sub = admin_1.get(f"{co}.{a1}", a1)
             data.append([int(gid), name, aname, co, sub, tz, int(pop)])
```

### Comparing `when-2.0.0/src/when/timezones.py` & `when-3.0.0/src/when/timezones.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     "YEKT": [("Asia/Yekaterinburg", "Yekaterinburg Time")],
     "YST": [("Asia/Yakutsk", "Yakutsk Standard Time")],
 }
 
 
 class Zones:
     def __init__(self, abbrs):
-        self.abbrs = {k.lower(): v for k,v in abbrs.items()}
+        self.abbrs = {k.lower(): v for k, v in abbrs.items()}
         self._cached = {}
         self.utc_offset_re = re.compile(r"^UTC[+±-]\d\d?(:\d\d)?$", re.IGNORECASE)
 
     def get(self, abbr):
         lower = abbr.lower()
         utc_offset_match = False
         if lower not in self.abbrs:
@@ -337,17 +337,15 @@
             values = []
             if utc_offset_match:
                 values.append((gettz(abbr), abbr.upper()))
             else:
                 for value, name in self.abbrs[lower]:
                     values.append(
                         (
-                            gettz(value)
-                            if isinstance(value, str)
-                            else tzoffset(name, value),
+                            gettz(value) if isinstance(value, str) else tzoffset(name, value),
                             name,
                         )
                     )
 
             self._cached[lower] = values
 
         return self._cached[lower]
```

### Comparing `when-2.0.0/src/when/utils.py` & `when-3.0.0/src/when/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,74 @@
 import os
 import re
 import sys
 import time
+import decimal
 from pathlib import Path
+from datetime import datetime
 
 import requests
-from dateutil.tz import tzfile, tzoffset, gettz
+from dateutil.tz import tzfile
 from dateutil.zoneinfo import get_zonefile_instance
 from dateutil.parser import parse as dt_parse
 
-from . import timezones
-from .lunar import LunarPhase
-
-MONTH_ABBRS = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
-WEEKDAY_ABBRS = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
-
 utc_offset_re = re.compile(r"\b(UTC([+-]\d\d?)(?::(\d\d))?)")
 
 
 def parse(value):
     dt, tokens = dt_parse(value, fuzzy_with_tokens=True)
     return dt
 
 
-def render_extras(zone):
-    extra = f" ({zone.name})"
-    if zone.city:
-        extra = f" ({zone.city})"
-
-    return extra
-
-
-def default_format(result, format):
-    zone = result.zone
-    fmt = format.replace("%C", f" ({zone.city})" if zone.city else "")
-
-    if "%Z" in fmt:
-        fmt = fmt.replace("%Z", result.zone.zone_name(result.dt))
+def datetime_from_timestamp(arg):
+    try:
+        value = decimal.Decimal(arg)
+    except decimal.InvalidOperation:
+        return None
+
+    value = float(value)
+    try:
+        dt = datetime.fromtimestamp(value)
+    except ValueError as err:
+        if "out of range" not in str(err):
+            raise
+        dt = datetime.fromtimestamp(value / 1000)
 
-    if "%O" in fmt:
-        lp = LunarPhase(result.dt)
-        fmt = fmt.replace("%O", f"[{lp.description}]")
-
-    return result.dt.strftime(fmt).strip()
-
-
-def rfc2822_format(result):
-    dt = result.dt
-    tt = dt.timetuple()
-    mo = MONTH_ABBRS[tt[1] - 1]
-    weekday = WEEKDAY_ABBRS[tt[6]]
+    return dt
 
-    return (
-        f"{weekday}, {tt[2]:02} {mo} {tt[0]:04} {tt[3]:02}:{tt[4]:02}:{tt[5]:02} "
-        f"{dt.strftime('%z')}{render_extras(result.zone)}"
-    )
 
+def parse_source_input(arg):
+    # arg = arg or datetime.now().isoformat()
+    if not isinstance(arg, str):
+        arg = " ".join(arg)
 
-def iso_format(result):
-    return f"{result.dt.isoformat()}{render_extras(result.zone)}"
+    value = datetime_from_timestamp(arg)
+    return value.isoformat() if value else arg.strip()
 
 
 def timer(func):
     colorize = "\033[0;37;43m{}\033[0;0m".format
 
     def inner(*args, **kwargs):
         start = time.time()
         result = func(*args, **kwargs)
         duration = time.time() - start
         print(colorize(f"⌛️ {func.__name__}: {duration}"), file=sys.stderr)
         return result
 
-    return inner if os.getenv("WHEN_TIMER") else func
+    return inner if os.getenv("WHENTIMER") else func
 
 
 @timer
 def fetch(url):
     r = requests.get(url)
     if r.ok:
         return r.content
-    else:
-        raise RuntimeError(f"{r.status_code}: {url}")
+
+    raise RuntimeError(f"{r.status_code}: {url}")
 
 
 def get_timezone_db_name(tz):
     filename = None
     if isinstance(tz, str):
         filename = tz
     elif isinstance(tz, tzfile):
@@ -92,16 +76,18 @@
 
     if filename is None:
         return
 
     if filename == "/etc/localtime":
         filename = str(Path(filename).resolve())
 
-    if "/zonename/" in filename:
-        return filename.rsplit("/zoneinfo/", 1)[1]
+    if "/zoneinfo/" in filename:
+        filename = filename.rpartition("/zoneinfo/")[-1]
+
+    return filename
 
 
 def all_zones():
     zi = get_zonefile_instance()
     return sorted(zi.zones)
```

### Comparing `when-2.0.0/tests/test_when.py` & `when-3.0.0/tests/test_when.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import os
-import sys
 import time
 from datetime import datetime
-from unittest.mock import patch
 from dateutil.tz import gettz
 
 from when.core import Formatter
-from when import utils
-from when.db import client
-from when.main import main as when_main
-from when.main import holidays
+from when.cli import main as when_main
+from when.core import holidays
 from when.timezones import zones
 
-#"NYC", 5128581
-#"DC", 4140963
+# "NYC", 5128581
+# "DC", 4140963
+
 
 def test_db_search_singleton(db):
     result = db.search("maastricht")
     assert len(result) == 1
     assert result[0].tz == "Europe/Amsterdam"
 
 
@@ -47,15 +44,15 @@
     assert result[0].dt == expect
 
 
 def test_iso_formatter(when):
     fmt = Formatter("iso")
     result = when.convert("Jan 10, 2023 4:30am", sources="New York City", targets="Seoul")
     assert len(result) == 1
-    assert fmt(result[0]).startswith("2023-01-10T18:30:00+09:00")
+    assert fmt(result[0]).startswith("2023-01-10T18:30:00+0900")
 
 
 def test_rfc_formatter(when):
     fmt = Formatter("rfc2822")
     result = when.convert("Jan 10, 2023 4:30am", sources="New York City", targets="Seoul")
     assert len(result) == 1
     value = fmt(result[0])
@@ -87,15 +84,15 @@
     try:
         os.environ["TZ"] = "EST"
         time.tzset()
         argv = "--source America/New_York --target Seoul Jan 10, 2023 4:30am".split()
         when_main(argv, when)
         captured = capsys.readouterr()
         output = captured.out
-        assert output.startswith("2023-01-10 18:30:00+0900 (Asia/Seoul) 010d02w")
+        assert output.startswith("2023-01-10 18:30:00+0900 (KST, Asia/Seoul) 010d02w (Seoul, KR)")
     finally:
         os.environ["TZ"] = orig_tz
         time.tzset()
 
 
 HOLIDAYS = """\
 New Year's Day.....Sun, Jan 01 2023 [🌓 First Quarter]
```

