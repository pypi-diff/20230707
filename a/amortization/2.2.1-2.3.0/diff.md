# Comparing `tmp/amortization-2.2.1.tar.gz` & `tmp/amortization-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amortization-2.2.1.tar", max compression
+gzip compressed data, was "amortization-2.3.0.tar", max compression
```

## Comparing `amortization-2.2.1.tar` & `amortization-2.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2022-12-15 19:37:04.613231 amortization-2.2.1/LICENSE
--rw-r--r--   0        0        0     6010 2022-12-15 19:37:04.613231 amortization-2.2.1/README.md
--rw-r--r--   0        0        0        0 2022-12-15 19:37:04.613231 amortization-2.2.1/amortization/__init__.py
--rw-r--r--   0        0        0     2768 2022-12-15 19:37:04.613231 amortization-2.2.1/amortization/amortize.py
--rw-r--r--   0        0        0      556 2022-12-15 19:37:04.613231 amortization-2.2.1/amortization/amount.py
--rw-r--r--   0        0        0      595 2022-12-15 19:37:04.613231 amortization-2.2.1/amortization/period.py
--rw-r--r--   0        0        0     1044 2022-12-15 19:37:04.613231 amortization-2.2.1/amortization/schedule.py
--rw-r--r--   0        0        0     2208 2022-12-15 19:37:04.613231 amortization-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     7034 1970-01-01 00:00:00.000000 amortization-2.2.1/setup.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 amortization-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-06 22:22:56.640949 amortization-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6382 2023-07-06 22:22:56.644949 amortization-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/__init__.py
+-rw-r--r--   0        0        0     3523 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/amortize.py
+-rw-r--r--   0        0        0      850 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/amount.py
+-rw-r--r--   0        0        0      195 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/enums.py
+-rw-r--r--   0        0        0      893 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/period.py
+-rw-r--r--   0        0        0     1251 2023-07-06 22:22:56.644949 amortization-2.3.0/amortization/schedule.py
+-rw-r--r--   0        0        0     2160 2023-07-06 22:22:56.644949 amortization-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7553 1970-01-01 00:00:00.000000 amortization-2.3.0/PKG-INFO
```

### Comparing `amortization-2.2.1/LICENSE` & `amortization-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amortization-2.2.1/README.md` & `amortization-2.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         <td>Version</td>
         <td><img src='https://img.shields.io/pypi/v/amortization.svg?logo=pypi&style=for-the-badge' alt="Version"></td>
     </tr>
     <tr>
         <td>Github Actions</td>
         <td><img src='https://img.shields.io/github/actions/workflow/status/roniemartinez/amortization/python.yml?branch=master&label=actions&logo=github%20actions&style=for-the-badge' alt="Github Actions"></td>
         <td>Coverage</td>
-        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/amortization/branch?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
+        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/amortization/master?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
     </tr>
     <tr>
         <td>Supported versions</td>
         <td><img src='https://img.shields.io/pypi/pyversions/amortization.svg?logo=python&style=for-the-badge' alt="Python Versions"></td>
         <td>Wheel</td>
         <td><img src='https://img.shields.io/pypi/wheel/amortization.svg?style=for-the-badge' alt="Wheel"></td>
     </tr>
@@ -81,37 +81,40 @@
 )
 ```
 
 ### Command line
 
 ```bash
 amortize -h
-usage: amortize [-h] -P PRINCIPAL -r INTEREST_RATE [-s] (-n PERIOD | -a AMOUNT)
+usage: amortize [-h] -P PRINCIPAL -r INTEREST_RATE [-s] [-f {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}] (-n PERIOD | -a AMOUNT)
 
 Python library for calculating amortizations and generating amortization schedules
 
 options:
   -h, --help            show this help message and exit
   -s, --schedule        Generate amortization schedule
+  -f {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}, --frequency {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}
+                        Payment frequency
   -n PERIOD, --period PERIOD
                         Total number of periods
   -a AMOUNT, --amount AMOUNT
                         Amortization amount per period
 
 required arguments:
   -P PRINCIPAL, --principal PRINCIPAL
                         Principal amount
   -r INTEREST_RATE, --interest-rate INTEREST_RATE
-                        Interest rate per period
+                        Interest rate per year
 ```
 
 ```bash
-amortize -P 150000 -n 36 -r 0.1         # period
-amortize -P 150000 -n 36 -r 0.1 -s      # schedule
-amortize -P 150000 -a 4840.08 -r 0.1    # amount
+amortize -P 150000 -n 36 -r 0.1             # period
+amortize -P 150000 -n 36 -r 0.1 -s          # schedule
+amortize -P 150000 -a 4840.08 -r 0.1        # amount
+amortize -P 150000 -n 36 -r 0.1 -f weekly   # period (specify payment frequency)
 ```
 
 ```bash
 % amortize -P 150000 -n 36 -r 0.1 -s           
 Number        Amount    Interest    Principal     Balance
 --------  ----------  ----------  -----------  ----------
 1           4,840.08    1,250.00     3,590.08  146,409.92
```

### Comparing `amortization-2.2.1/pyproject.toml` & `amortization-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amortization"
-version = "2.2.1"
+version = "2.3.0"
 repository = "https://github.com/roniemartinez/amortization"
 description = "Python library for calculating amortizations and generating amortization schedules"
 authors = ["Ronie Martinez <ronmarti18@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "amortization"
@@ -12,40 +12,39 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Topic :: Office/Business :: Financial :: Accounting",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.urls]
 "Donate" = "https://www.buymeacoffee.com/roniemartinez"
 
 [tool.poetry.scripts]
 amortize = "amortization.amortize:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7.8"
-black = "^22.12"
-isort = "^5.11.2"
-mypy = "^0.991"
+black = "^23.3"
+isort = "^5.11.5"
+mypy = "^1.4"
 pyproject-flake8 = "^5.0.4"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 types-tabulate = "^0.9.0"
 
 [tool.isort]
 line_length = 120
 multi_line_output = 3
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `amortization-2.2.1/PKG-INFO` & `amortization-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 Metadata-Version: 2.1
 Name: amortization
-Version: 2.2.1
+Version: 2.3.0
 Summary: Python library for calculating amortizations and generating amortization schedules
 Home-page: https://github.com/roniemartinez/amortization
 License: MIT
 Keywords: amortization
 Author: Ronie Martinez
 Author-email: ronmarti18@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Donate, https://www.buymeacoffee.com/roniemartinez
 Project-URL: Repository, https://github.com/roniemartinez/amortization
@@ -38,15 +31,15 @@
         <td>Version</td>
         <td><img src='https://img.shields.io/pypi/v/amortization.svg?logo=pypi&style=for-the-badge' alt="Version"></td>
     </tr>
     <tr>
         <td>Github Actions</td>
         <td><img src='https://img.shields.io/github/actions/workflow/status/roniemartinez/amortization/python.yml?branch=master&label=actions&logo=github%20actions&style=for-the-badge' alt="Github Actions"></td>
         <td>Coverage</td>
-        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/amortization/branch?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
+        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/amortization/master?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
     </tr>
     <tr>
         <td>Supported versions</td>
         <td><img src='https://img.shields.io/pypi/pyversions/amortization.svg?logo=python&style=for-the-badge' alt="Python Versions"></td>
         <td>Wheel</td>
         <td><img src='https://img.shields.io/pypi/wheel/amortization.svg?style=for-the-badge' alt="Wheel"></td>
     </tr>
@@ -114,37 +107,40 @@
 )
 ```
 
 ### Command line
 
 ```bash
 amortize -h
-usage: amortize [-h] -P PRINCIPAL -r INTEREST_RATE [-s] (-n PERIOD | -a AMOUNT)
+usage: amortize [-h] -P PRINCIPAL -r INTEREST_RATE [-s] [-f {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}] (-n PERIOD | -a AMOUNT)
 
 Python library for calculating amortizations and generating amortization schedules
 
 options:
   -h, --help            show this help message and exit
   -s, --schedule        Generate amortization schedule
+  -f {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}, --frequency {daily,biweekly,weekly,semimonthly,monthly,quarterly,semiyearly,yearly}
+                        Payment frequency
   -n PERIOD, --period PERIOD
                         Total number of periods
   -a AMOUNT, --amount AMOUNT
                         Amortization amount per period
 
 required arguments:
   -P PRINCIPAL, --principal PRINCIPAL
                         Principal amount
   -r INTEREST_RATE, --interest-rate INTEREST_RATE
-                        Interest rate per period
+                        Interest rate per year
 ```
 
 ```bash
-amortize -P 150000 -n 36 -r 0.1         # period
-amortize -P 150000 -n 36 -r 0.1 -s      # schedule
-amortize -P 150000 -a 4840.08 -r 0.1    # amount
+amortize -P 150000 -n 36 -r 0.1             # period
+amortize -P 150000 -n 36 -r 0.1 -s          # schedule
+amortize -P 150000 -a 4840.08 -r 0.1        # amount
+amortize -P 150000 -n 36 -r 0.1 -f weekly   # period (specify payment frequency)
 ```
 
 ```bash
 % amortize -P 150000 -n 36 -r 0.1 -s           
 Number        Amount    Interest    Principal     Balance
 --------  ----------  ----------  -----------  ----------
 1           4,840.08    1,250.00     3,590.08  146,409.92
```

