# Comparing `tmp/cryptographyComplements-0.3.0.1.tar.gz` & `tmp/cryptographyComplements-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.3.0.1.tar", last modified: Fri Jul  7 01:01:09 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.3.1.tar", last modified: Fri Jul  7 17:46:00 2023, max compression
```

## Comparing `cryptographyComplements-0.3.0.1.tar` & `cryptographyComplements-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.301591 cryptographyComplements-0.3.0.1/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.0.1/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      581 2023-07-07 01:01:09.298635 cryptographyComplements-0.3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.292191 cryptographyComplements-0.3.0.1/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    16189 2023-07-07 00:40:25.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2182 2023-07-06 23:56:59.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2451 2023-07-07 00:05:14.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.296220 cryptographyComplements-0.3.0.1/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-07-07 01:01:09.000000 cryptographyComplements-0.3.0.1/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 01:01:09.302591 cryptographyComplements-0.3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-07-07 01:01:03.000000 cryptographyComplements-0.3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.724180 cryptographyComplements-0.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-07-07 17:46:00.723181 cryptographyComplements-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.705494 cryptographyComplements-0.3.1/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.1/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.1/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    15770 2023-07-07 17:41:22.000000 cryptographyComplements-0.3.1/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2182 2023-07-07 10:34:30.000000 cryptographyComplements-0.3.1/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3002 2023-07-07 17:40:51.000000 cryptographyComplements-0.3.1/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:46:00.720162 cryptographyComplements-0.3.1/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-07 17:46:00.000000 cryptographyComplements-0.3.1/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:46:00.725181 cryptographyComplements-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-07-07 17:45:45.000000 cryptographyComplements-0.3.1/setup.py
```

### Comparing `cryptographyComplements-0.3.0.1/LICENSE` & `cryptographyComplements-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0.1/PKG-INFO` & `cryptographyComplements-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.3.0.1
+Version: 0.3.1
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.3.0.1/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.3.1/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0.1/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.3.1/cryptographyComplements/mathFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,32 +376,14 @@
             b = math.sqrt(a**2 - n)
 
             if b % 1 == 0:
                 return (int(a-b), int(a+b))
             
         return True
 
-
-def lcm(n1: int, n2: int) -> int:
-    "Calculate the least common multiple for two numbers n1 and n2."
-
-    gcd = EuclideanAlgorithm(n1, n2)
-
-    return abs(n1) * (abs(n2)/gcd)
-
-def lcm_list(numbers: list) -> int:
-    "Calculate the least common multiple for a list of integer numbers."
-
-    lcmN = numbers[0]
-    for i in range(1, len(numbers)):
-
-        lcmN = lcm(lcmN, numbers[i])
-
-    return int(lcmN)
-
 def CarmichaelFunction(n: int) -> int:
     "Calculate the Carmichael function for n."
 
     factorization = FactorizationMethods.TrialDivision(n, n)
 
     powers = {}
 
@@ -418,15 +400,15 @@
 
         if prime == 2 and powers[prime] >= 3:
             phis.append((EulerTotientFunction(pow(prime, powers[prime]))*(1/2)))
 
         else:
             phis.append(EulerTotientFunction(pow(prime, powers[prime])))
 
-    return lcm_list(phis)
+    return Numbers.lcm_list(phis)
 
 def BertrandPostulate(n: int) -> int:
     "From a given integer n > 1 find the first prime number that verifies the inequality: n < p < 2n."
 
     from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
 
     if n <= 1:
```

### Comparing `cryptographyComplements-0.3.0.1/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.3.1/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0.1/cryptographyComplements/tools.py` & `cryptographyComplements-0.3.1/cryptographyComplements/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,32 @@
                 result += int(i)
 
             except ValueError:
                 continue
 
         return result
     
+    def lcm(n1: int, n2: int) -> int:
+        "Calculate the least common multiple for two numbers n1 and n2."
+        from cryptographyComplements.mathFunctions import EuclideanAlgorithm
+
+        gcd = EuclideanAlgorithm(n1, n2)
+
+        return abs(n1) * (abs(n2)/gcd)
+
+    def lcm_list(numbers: list) -> int:
+        "Calculate the least common multiple for a list of integer numbers."
+
+        lcmN = numbers[0]
+        for i in range(1, len(numbers)):
+
+            lcmN = Numbers.lcm(lcmN, numbers[i])
+
+        return int(lcmN)
+
 
 class stopwatch:
     "Create as many stopwatch as you need."
     def start() -> float:
         "Start a stopwatch. \nNote: The stopwatch needs to be saved into a variable."
         import time
         return time.time()
```

### Comparing `cryptographyComplements-0.3.0.1/setup.py` & `cryptographyComplements-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import decimal
 
 setup(
     name='cryptographyComplements',
-    version='0.3.0.1',
+    version='0.3.1',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

