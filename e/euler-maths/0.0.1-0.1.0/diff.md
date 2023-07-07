# Comparing `tmp/euler_maths-0.0.1.tar.gz` & `tmp/euler_maths-0.1.0.tar.gz`

## Comparing `euler_maths-0.0.1.tar` & `euler_maths-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 euler_maths-0.0.1/TODO
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 euler_maths-0.0.1/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 euler_maths-0.0.1/src/euler_maths/__init__.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 euler_maths-0.0.1/src/euler_maths/misc.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 euler_maths-0.0.1/src/euler_maths/prime.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 euler_maths-0.0.1/tests/speed_test.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 euler_maths-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 euler_maths-0.0.1/LICENSE
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 euler_maths-0.0.1/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 euler_maths-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 euler_maths-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 euler_maths-0.1.0/TODO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 euler_maths-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 euler_maths-0.1.0/src/euler_maths/__init__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 euler_maths-0.1.0/src/euler_maths/misc.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 euler_maths-0.1.0/src/euler_maths/prime.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 euler_maths-0.1.0/tests/speed_test.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 euler_maths-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 euler_maths-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 euler_maths-0.1.0/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 euler_maths-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 euler_maths-0.1.0/PKG-INFO
```

### Comparing `euler_maths-0.0.1/src/euler_maths/prime.py` & `euler_maths-0.1.0/src/euler_maths/prime.py`

 * *Files identical despite different names*

### Comparing `euler_maths-0.0.1/tests/speed_test.py` & `euler_maths-0.1.0/tests/speed_test.py`

 * *Files identical despite different names*

### Comparing `euler_maths-0.0.1/LICENSE` & `euler_maths-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `euler_maths-0.0.1/README.md` & `euler_maths-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Euler Maths
 
 ## Description
 
 A collection of useful functions for mathematical calculations, mostly concerned with prime numbers and basic algebra on natural numbers.
 
 ### Key features
-
 - Prime number sieve
 - Primality test
 - Prime factors sieve
 - Euler's totient function
 - Mobius function
 - Modular inverse
 
 ### Motivation
-
 The functions contained here are commonly used in solving [Project Euler](https://projecteuler.net/) problems.
 
 ![ProjectEulerProfile](https://projecteuler.net/profile/Luke943.png)
 
 *Note: These are NOT solutions to any particular problem.*
 
 ## Module Dependencies
@@ -34,20 +32,21 @@
 - `prime_factors(N)` - Returns array of unique prime factors for each number < N.
 - `is_prime(n)` - Determines if n is prime (utilising the Miller-Rabin test for large values).
 - `euler_totients(N)` - Returns an array with value of Euler's totient function for numbers <N.
 - `euler_totient(n, prime_factors)` - Calculates Euler's totient function of n given a list of its prime factors.
 - `mobius_array(N)` - Returns an array with value of the Mobius function for numbers <N.
 - `square_free(N)` - Counts of the number of square-free values <N.
 - `modular_inverse(a, n)` - Computes the inverse of a modulo n.
+- `isqrt2` - Integer square-root function compatible with Numba.
 
 ## Installation
 
-The package can be installed from TestPyPI by running:
+The package can be installed from PyPI by running:
 ```bash
-pip install --index-url https://test.pypi.org/simple/ euler_maths
+pip install euler-maths
 ```
 
 ## Usage
 
 Once installed, simply import the module and use the functions it provides.
 
 ```python
```

### Comparing `euler_maths-0.0.1/pyproject.toml` & `euler_maths-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "euler_maths"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Luke Hartley", email="luke.hartley05@gmail.com" },
 ]
 description = "A library of mathematical functions for Project Euler"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `euler_maths-0.0.1/PKG-INFO` & `euler_maths-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euler_maths
-Version: 0.0.1
+Version: 0.1.0
 Summary: A library of mathematical functions for Project Euler
 Project-URL: Homepage, https://github.com/Luke943/Euler-Maths
 Project-URL: Bug Tracker, https://github.com/Luke943/Euler-Maths/issues
 Author-email: Luke Hartley <luke.hartley05@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,24 +17,22 @@
 # Euler Maths
 
 ## Description
 
 A collection of useful functions for mathematical calculations, mostly concerned with prime numbers and basic algebra on natural numbers.
 
 ### Key features
-
 - Prime number sieve
 - Primality test
 - Prime factors sieve
 - Euler's totient function
 - Mobius function
 - Modular inverse
 
 ### Motivation
-
 The functions contained here are commonly used in solving [Project Euler](https://projecteuler.net/) problems.
 
 ![ProjectEulerProfile](https://projecteuler.net/profile/Luke943.png)
 
 *Note: These are NOT solutions to any particular problem.*
 
 ## Module Dependencies
@@ -50,20 +48,21 @@
 - `prime_factors(N)` - Returns array of unique prime factors for each number < N.
 - `is_prime(n)` - Determines if n is prime (utilising the Miller-Rabin test for large values).
 - `euler_totients(N)` - Returns an array with value of Euler's totient function for numbers <N.
 - `euler_totient(n, prime_factors)` - Calculates Euler's totient function of n given a list of its prime factors.
 - `mobius_array(N)` - Returns an array with value of the Mobius function for numbers <N.
 - `square_free(N)` - Counts of the number of square-free values <N.
 - `modular_inverse(a, n)` - Computes the inverse of a modulo n.
+- `isqrt2` - Integer square-root function compatible with Numba.
 
 ## Installation
 
-The package can be installed from TestPyPI by running:
+The package can be installed from PyPI by running:
 ```bash
-pip install --index-url https://test.pypi.org/simple/ euler_maths
+pip install euler-maths
 ```
 
 ## Usage
 
 Once installed, simply import the module and use the functions it provides.
 
 ```python
```

