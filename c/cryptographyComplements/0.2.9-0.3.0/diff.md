# Comparing `tmp/cryptographyComplements-0.2.9.tar.gz` & `tmp/cryptographyComplements-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.9.tar", last modified: Fri Apr 21 00:20:29 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.3.0.tar", last modified: Fri Jul  7 00:56:12 2023, max compression
```

## Comparing `cryptographyComplements-0.2.9.tar` & `cryptographyComplements-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.354103 cryptographyComplements-0.2.9/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-21 00:20:29.354103 cryptographyComplements-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.9/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.349404 cryptographyComplements-0.2.9/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.9/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.9/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    10528 2023-04-21 00:19:12.000000 cryptographyComplements-0.2.9/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     3307 2023-04-20 23:46:09.000000 cryptographyComplements-0.2.9/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     3292 2023-04-20 23:48:10.000000 cryptographyComplements-0.2.9/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.353103 cryptographyComplements-0.2.9/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-21 00:20:29.000000 cryptographyComplements-0.2.9/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 00:20:29.355322 cryptographyComplements-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-21 00:20:24.000000 cryptographyComplements-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.693138 cryptographyComplements-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-07-07 00:56:12.691128 cryptographyComplements-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.684551 cryptographyComplements-0.3.0/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.0/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.0/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    16189 2023-07-07 00:40:25.000000 cryptographyComplements-0.3.0/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2182 2023-07-06 23:56:59.000000 cryptographyComplements-0.3.0/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     2451 2023-07-07 00:05:14.000000 cryptographyComplements-0.3.0/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.688474 cryptographyComplements-0.3.0/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-07 00:56:12.000000 cryptographyComplements-0.3.0/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 00:56:12.694135 cryptographyComplements-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-06-23 18:35:31.000000 cryptographyComplements-0.3.0/setup.py
```

### Comparing `cryptographyComplements-0.2.9/LICENSE` & `cryptographyComplements-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.9/PKG-INFO` & `cryptographyComplements-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.9/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.3.0/cryptographyComplements/mathFunctions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,136 @@
-"In this script you can find all the mathematical functions relative to Number Theory and Group Theory."
+"In this script you can find all the mathematical functions relative to Number Theory."
 from cryptographyComplements.tools import Numbers # required class, because contains functions used by some of them below
+import math
 
-def EulerTotientFunction(number: int):
+def EulerTotientFunction(n: int) -> int:
     "Calculate, from a given number, the Euler Totient function."
-    if not isinstance(number, int):
+    
+    if n <= 1:
+        if n == 1:
+            return 1
         return None
+    
+    factorization = FactorizationMethods.TrialDivision(n, n)
+
+    relativePrime = n
+
+    used = []
 
-    result = int(number)
-    p = 2
-    while p * p <= number:
-        if number % p == 0:
-            while number % p == 0:
-                number //= p
-            result -= result // p
-        p += 1
-    if number > 1:
-        result -= result // number
-    return result
+    for prime in factorization:
+        if prime in used:
+            continue
 
-def EuclideanAlgorithm(a: int, b: int):
+        relativePrime *= ((prime-1)/prime)
+        
+        used.append(prime)
+
+
+    return int(relativePrime)
+
+def EuclideanAlgorithm(a: int, b: int) -> int:
     "Given two numbers, a and b, calculate their Great Common Divisor."
-    if a % 1 != 0 or b % 1 != 0:
-        return None
 
-    a, b = int(a), int(b)
+    q = math.floor(a/b)
+    r = a-(b*q)
+
+    if r == 0:
+        return b
+
+    q2 = math.floor(b/r)
+    r2 = b-(q2*r)
+
+    if r2 == 0:
+        return q2
+
+    previous = [q, r, q2, r2]
 
     while True:
-        r = a % b
-        if r != 0:
-            a, b, remainder = b, r, r # remainder = r needs to be kept, because if r = 0, then it will be stored back.
-        else:
-            return remainder
+        q = math.floor(previous[1]/previous[3])
+        r = previous[1]-(q*previous[3])
 
-def ExtendedEuclideanAlgorithm(a: int, b: int):
-    "Given two numbers, a and b, calculate their Great Common Divisor and the coefficients of Bézout's identity"
+        if r == 0:
+            return previous[3]
+        
+        previous.pop(0)
+        previous.pop(0)
+        previous.append(q)
+        previous.append(r)
 
-    if a % 1 != 0 or b % 1 != 0:
-        return None
-    a, b = int(a), int(b)
+def ExtendedEuclideanAlgorithm(a: int, b: int) -> tuple:
+    "Given two numbers, a and b, calculate their Great Common Divisor and the coefficients of Bézout's identity"
 
     x0, x1, y0, y1 = 1, 0, 0, 1
     while b != 0:
         r = a % b
         x = x0 - (a // b)*x1
         y = y0 - (a // b)*y1
         a, b, x0, x1, y0, y1 = b, r, x1, x, y1, y
 
     return a, x0, y0 # a is the GCD of a and b
 
-def calculateOrder(g:int, p:int):
-    "Given a number: g, and a prime number. Calculate the order of g in p."
-    k = 1
-    order = 0
-    while order != 1:
-        order = (g**k) % p
-        k += 1
-    
-    return int(k-1) # -1 needs to be added because +1 will be added even if the order is 1, because the iteration when order becomes 1 is not completed yet.
-
-def InverseModuloBruteforceAlgorithm(number: int, mod:int):
-    "Calculate by a given number and modulo the inverse modulo of them. It uses the bruteforce method so for larger numbers is not recommended."
+def MultiplicativeOrder(a: int, n: int) -> int:
+    "Calculate the multiplicative order of a in mod n. The function if n is relatively prime to a then it will return the Carmichael function, in any other case it will use the bruteforce algorithm."
 
-    if EuclideanAlgorithm(number, mod) != 1: # checks if exists an inverse modulo
-        return None
+    if EuclideanAlgorithm(a, n) == 1:
+        Carmichael = CarmichaelFunction(n)
+        return Carmichael
+    
+    k = 0
 
-    for i in range(mod):
-        if (number*i % mod) == 1:
-            return i
-        
-        i += 1
+    while pow(a, k, n) != 1:
+        k += 1
 
-def WillansFormula(n: int):
-    "From a given number in input calculate the Willans Formula. \nNote this formula can't be used for numbers > 7 because of Overflow Error."
-    from math import floor, cos, pi, factorial
-    return 1+ sum([
-        floor(pow(
-        n/sum([
-            floor(pow(cos(pi * (float(factorial(j-1)) + 1)/j), 2))
-            for j in range(1, i+1)
-        ]), 1/n))
-        for i in range(1, (2**n)+1)
-    ])
-
-def CollatzConjecture(n: int):
-    "From a given number in input, calculate the Collatz Conjecture. \n\nIt will return True if the number entered in input it's in a cyclic group and False if it the number in input gets to 1."
-    number = n
-    while True:
-        if n == 1:
-            return False
+    return k
 
-        n = 3*n + 1     
-        while n % 2 == 0:
-            n //= 2
-
-        if n == number:
-            print(f"Cyclic number found: {n}")
-            return True
 
 class DiscreteLogarithm:
-    "This class contains all the Discrete Logarithm algorithm to solve the Discrete Logarithm Problem: g^x = h (mod p)"
+    "This class contains all the Discrete Logarithm algorithms to solve the Discrete Logarithm Problem: g^x ≡ h (mod p) or g^X = h in Fp"
+
+    def BruteforceAlgorithm(g: int, h: int, p: int) -> int:
+        "Using the Bruteforce algorithm, solve the Discrete Logarithm Problem. \n\nThe functions search for all numbers up to p. If there isn't a solution or it's greater than p the algorithm will return None."
 
-    def BruteforceAlgorithm(g: int, h: int, p: int):
-        "Using the Bruteforce algorithm, solve the Discrete Logarithm Problem: g^x = h (mod p) \n\nThe functions search for all numbers up to p. If there isn't a solution or it's greater than p the algorithm will return None."
-        if not isinstance(g, int) or not isinstance(h, int) or not isinstance(p, int):
-            return None
-        
         for x in range(0, p+1):
 
-            if ((g**x) % p) == (h % p):
+            if pow(g, x, p) == (h % p):
                 return x
-            
+
         return None
 
-    def ShanksBabyStepGiantStepAlgorithm(g:int, h:int, p:int):
-        "Using the Shanks Baby-Step Giant-Step algorithm, solve the Discrete Logarithm Problem: g^x = h (mod p) \n\nThe functions returns None if there isn't a solution to the algorithm"
+    def ShanksBabyStepGiantStepAlgorithm(g:int, h:int, p:int) -> int:
+        "Using the Shanks Baby-Step Giant-Step algorithm, solve the Discrete Logarithm Problem: g^x ≡ h (mod p) \n\nThe function returns None if there isn't a solution to the Discrete Logarithm."
         
-        from math import floor, sqrt
-        from cryptographyComplements.mathFunctions import calculateOrder
-        n = floor(sqrt(calculateOrder(g, p))) + 1
+        import math
+        n = math.floor(math.sqrt(MultiplicativeOrder(g, p))) + 1
 
-        u = (g**(EulerTotientFunction(p)-n)) % p
+        u = pow(g, EulerTotientFunction(p)-n, p)
 
         l1, l2 = [], []
 
         for i in range(0, n+1):
-            l1.append((g**i) % p)
+            l1.append(pow(g, i, p))
 
         for j in range(0, n):
-            keep = (h*(u**j)) % p
-            l2.append((h*(u**j)) % p)
+            keep = (h*(pow(u, j))) % p
+            l2.append(keep)
             if keep in l1:
                 break
 
         try:
             value = l1.index(keep)
         except ValueError:
             return None
 
         value2 = l2.index(keep)
 
         x = value + (n * value2)
 
         return x
     
-def ChineseRemainderTheorem(congruences:list, modulo: list):
+def ChineseRemainderTheorem(congruences:list, modulo: list) -> int:
     "From a list of congruences and a list of modulos, tuples are accepted too, of the same lenght, calculate the Chinese Remainder Theorem. \n\nIf there is a solution it will be returned as a number, but if there isn't it will return None."
     try:
         for i in range(0, len(modulo)):
             if i == (len(modulo)-1):
                 break
 
             try:
@@ -166,145 +149,116 @@
 
     for i in modulo:
         moduloI = M/i
         totalM.append(moduloI)
 
     moduloInverses = []
     for i in range(0, len(congruences)):
-        moduloI = InverseModuloExtendedEuclideanAlgorithm(totalM[i], modulo[i])
+        moduloI = ExtendedEuclideanModularMultiplicativeInverse(totalM[i], modulo[i])
 
         if moduloI == None: # If there is no inverse modulo, then there isn't a solution for that congruence
             return None
 
-
         moduloInverses.append(moduloI)
 
     y = 0
     for i in range(0, len(congruences)):
-        y += (moduloInverses[i]* totalM[i] * congruences[i])
+        y += (moduloInverses[i] * totalM[i] * congruences[i])
 
     return int((y % M))
 
-
 class MersennePrime:
-    
-    def LucasNumbers(limit: int):
-        "Calculate the Lucas Numbers from a given number in limit: it defines when the algorithm stops."
+    "In this class you can find all the math functions about Mersenne numbers: 2^n - 1"
 
-        if not isinstance(limit, int) or limit < 0:
-            return None
+    def LucasNumbers(limit: int) -> list:
+        "Calculate the Lucas Numbers from a given number in limit: it defines at what number the algorithm stops."
 
-        sequence = [1, 3]
+        sequence = [2, 1, 3]
         x0, x1 = 1, 3
 
         for i in range(limit):
 
             x = x0 + x1
             x0 = x1
             x1 = x
 
             sequence.append(x)
 
         return sequence
-    
-    def LucasMethod(number: int):
-        "Use the Lucas Method to calculate a Mersenne prime number, and check if it's a prime number."
-        from cryptographyComplements.primalityTests import MersennePrimePrimalityTest
-        
-        return MersennePrimePrimalityTest.LucasPrimalityTest(number)
-
 
-    def LucasLehmerNumbers(limit: int):
+    def LucasLehmerNumbers(limit: int) -> list:
         "Calculate the Lucas-Lehmer Numbers from a given number in limit: it defines when the algorithm stops."
 
-        if not isinstance(limit, int) or limit < 0:
-            return None
-
         sequence = [4]
         x = 4
 
         for i in range(1, limit):
 
-            x = (x**2)-2
+            x = pow(x, 2) - 2
+
             sequence.append(x)
 
         return sequence
     
-
-    def LucasLehmerModuloNumbers(limit: int, modulo: int):
-        "This version of the Lucas-Lehmer numbers sequence uses the limit and the modulo too. The modulo needs to be added to reduce the computational time required. \n\nUse this if you don't care about the whole sequence of the numbers."
-
-        if not isinstance(limit, int) or limit < 0:
-            return None
+    def LucasLehmerModuloNumbers(limit: int, modulo: int) -> list:
+        "This version of the Lucas-Lehmer numbers sequence uses the limit and the modulo too. The modulo needs to be added to reduce the computational time required. \n\nUse this only for the Lucas-Lehmer primality test."
 
         sequence = [4]
         x = 4
 
         for i in range(1, limit):
 
-            x = (((x**2)-2) % modulo)
+            x = ((pow(x, 2)-2) % modulo)
             sequence.append(x)
 
         return sequence
-    
-    def LucasLehmerMethod(number: int):
-        "Use the Lucas-Lehmer Method to calculate a Mersenne prime number, and check if it's a prime number."
-
-        from cryptographyComplements.primalityTests import MersennePrimePrimalityTest
-        return MersennePrimePrimalityTest.LucasLehmerPrimalityTest(number)
-    
 
-def InverseModuloExtendedEuclideanAlgorithm(number: int, modulo: int):
-    "From a given number and a modulo in input, calculate the inverse modulo of the number. \n \nNote: The function will return None if there isn't a inverse modulo."
+def ExtendedEuclideanModularMultiplicativeInverse(a: int, m: int) -> int:
+    "Calculate the modular multiplicative inverse of the number an integer a modulo m. The functions uses the coefficients of the Bézout identity to calculate it. \n \nNote: The function will return None if there isn't a inverse modulo."
 
-    gcd, x, y = ExtendedEuclideanAlgorithm(number, modulo)
+    gcd, x, y = ExtendedEuclideanAlgorithm(a, m)
 
 
     if gcd != 1:
-
-        return None # There isn't an inverse modulo
+        return None # this happens only if there isn't an inverse modulo
     
-    return x % modulo
-
+    return x % m
 
-def FermatLittleTheorem(a:int, p:int) -> int:
-    "From a given integer and a prime number, calculate the Fermat Little Theorem."
-    return ((a**(p-1)) % p)
+def FermatLittleTheorem(a:int, n:int) -> int:
+    "From a given integer and a modulo, calculate the Fermat Little Theorem. \n\nNote: The function will return 1 if n is either a prime number or a carmichae number."
 
+    return pow(a, n-1, n)
 
-def MultiplicativePersistence(num: int):
+def MultiplicativePersistence(num: int) -> int:
     "From a given integer in input, calculate the multiplicative persistence. The function will return the number of steps required."
 
     result, steps = 1, 0
 
     for i in str(num):
         result = int(i) * result
 
     steps += 1
 
 
     while len(str(result)) != 1:
-        # print(result)
         num = result
         result = 1        
         for i in str(num):
 
             result *= int(i)
 
         steps += 1
 
     return steps
 
-
 def FermatEulerTheorem(a:int, n:int) -> int:
-    "From a given two given integers calculate Fermat-Euler Theorem. \n\nNote: a is the number and n is the modulo"
-    return (a**(EulerTotientFunction(n))) % n
-
+    "From a given two given integers calculate Fermat-Euler Theorem. \n\nNote: a is the number and n is the modulo. Moreover, the function will return 1 if and only if a and are coprime positive."
+    return pow(a, EulerTotientFunction(n), n)
 
-def EulerFormula(p: int, q: int) -> bool:
+def EulerFormulaForPQ(p: int, q: int) -> bool:
     "The Euler Formula from two given integers p and q returns True if the congruence a^((p-1)(q-1)/g) mod pq is congruent to 1 and False if it's not."
 
     if p == 2 or q == 2:
         return FermatEulerTheorem(p, q)
 
     g = EuclideanAlgorithm(p-1, q-1)
 
@@ -314,13 +268,281 @@
         return False
 
     if pow(a, (p-1)*(q-1)//g, p*q) != 1:
         return False
 
     return True
 
+def PrimeNumberTheorem(n: int) -> float:
+    "Calculate the Prime Number Theorem for n using n/ln(n). The value returned is an approximation."
+    if n <= 1:
+        return 0.0
+    return n / (math.log(n))
+
+from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
+class FactorizationMethods:
+    "This class contains factorization methods, including special purpose and general purpose ones."
+
+    def TrialDivision(n: int, maxN: int) -> list:
+        "This factorization method uses the trial division and it's a special purpose algorithm, so it's not recommended for numbers that could be possibly be prime, or for large composites.\n\nNote: maxN defines the maximum value for which will be searched primes that factorize n. It has been implemented to avoid large computations. \nIf you want to search up to n, just put maxN=n"
+
+        if MillerRabinPrimalityTest(n, 100):
+            return [n]        
+
+        primeFactors = []
+        keep = n
+
+        import math
+
+        # for i in range(2, n+1):
+        for i in range(2, maxN+1):
+
+            flag = False
+
+            if n / i % 1 == 0:
+
+                for prime in primeFactors:
+                    if i/prime % 1 == 0:
+                        flag = True
+                        break
+
+                if not flag:
+                    primeFactors.append(i)
+                    n /= i
+
+                    while n/i % 1 == 0:
+                        primeFactors.append(i)
+                        n /= i
+
+
+            if Numbers.listMultiplication(primeFactors) == keep:
+                break
+
+        return primeFactors
+
+    def PollardRhoFactorizationAlgorithm(n: int) -> int:
+        "The Pollard Rho factorization algorithm is a special purpose algorithm \n\n The algorithm returns a prime factor of n."
+
+        def gx(x, n):
+            return (x**2 + 1) % n
+
+        x = 2
+        y = 2
+        d = 1
+
+        while d == 1:
+            x = gx(x, n)
+            y = gx(gx(y, n), n)
+            
+            d = ExtendedEuclideanAlgorithm(abs(x-y), n)[0]
+
+        if d == n:
+            return None
+        
+        return d
+
+    def PollardFactorizationAlgorithm(n: int) -> int:
+        "The Pollard's p-1 algorithm is a factorization algorithm for special purpose \n\n The algorithm returns a prime factor of n."
+
+        a = 2
+        for j in range(2, n):
+            a = pow(a, j, n)
+            d = ExtendedEuclideanAlgorithm(a-1, n)[0]
+            if 1 < d < n:
+                return d
 
-def PrimeNumberTheorem(number: int) -> float:
-    "Given a number, calculate using the Natural Logarithm how much primes are below that number. \n\nNote: Value is an estimate."
-    import math
+    def FermatFactorizationAlgorithm(n: int) -> None|tuple|bool:
+        "The Fermat factorization algorithm is exponential and special purpose. \n\nIf n it's not odd, it will return None, in any other case it will return a nontrivial divisor of n or it will return True if n is prime."
+
+        if n % 2 == 0:
+            return None
+        
+        rad = math.ceil(math.sqrt(n))
+        maxN = math.ceil((n+9)/6)
+
+        steps = 1
+
+        if n % 4 == 1:
+            steps = 2
+            if rad % 2 == 0:
+                rad += 1
+
+        elif n % 3 == 2:
+            steps = 3
+
+            while rad % 3 != 0:
+                rad += 1
+
+        for a in range(rad, maxN+1, steps):
+            b = math.sqrt(a**2 - n)
+
+            if b % 1 == 0:
+                return (int(a-b), int(a+b))
+            
+        return True
+
+
+def lcm(n1: int, n2: int) -> int:
+    "Calculate the least common multiple for two numbers n1 and n2."
+
+    gcd = EuclideanAlgorithm(n1, n2)
+
+    return abs(n1) * (abs(n2)/gcd)
+
+def lcm_list(numbers: list) -> int:
+    "Calculate the least common multiple for a list of integer numbers."
+
+    lcmN = numbers[0]
+    for i in range(1, len(numbers)):
+
+        lcmN = lcm(lcmN, numbers[i])
+
+    return int(lcmN)
+
+def CarmichaelFunction(n: int) -> int:
+    "Calculate the Carmichael function for n."
+
+    factorization = FactorizationMethods.TrialDivision(n, n)
+
+    powers = {}
+
+    for prime in factorization:
+        try:
+            powers[prime] += 1
+
+        except KeyError:
+            powers[prime] = 1
+
+    phis = []
+
+    for prime in powers.keys():
+
+        if prime == 2 and powers[prime] >= 3:
+            phis.append((EulerTotientFunction(pow(prime, powers[prime]))*(1/2)))
+
+        else:
+            phis.append(EulerTotientFunction(pow(prime, powers[prime])))
+
+    return lcm_list(phis)
+
+def BertrandPostulate(n: int) -> int:
+    "From a given integer n > 1 find the first prime number that verifies the inequality: n < p < 2n."
+
+    from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
+
+    if n <= 1:
+        return None
+    
+    for i in range(n+1, 2*n):
+        
+        if MillerRabinPrimalityTest(i, 100):
+            return i
+        
+def SieveOfEratosthenes(n: int) -> list:
+    "Calculate all the prime numbers less than n using the Sieve of Eratosthenes."
+
+    nums = [i for i in range(2, n+1)]
+
+    maxN = math.ceil(math.sqrt(n))
+
+    for p in nums:
+
+        if p > maxN:
+            break
+
+        t = 2
+
+        while t*p <= n:
+            tp = p*t
+
+            try:
+                nums.remove(tp)
+
+            except ValueError:
+                pass
+
+            t+=1
+
+    return nums
+
+def MobiusFunction(n: int) -> int:
+    "From a given n, calculate the Möbius function."
+
+    if n == 1:
+        return 1
+    
+    factorization = FactorizationMethods.TrialDivision(n, n)
+
+    seen = []
+
+    for f in factorization:
+        if f in seen:
+            return 0
+
+        seen.append(f)
+    
+    if len(factorization) % 2 == 0:
+        return 1
+    
+    return -1
+
+
+class Conjectures:
+    "In this class you can find all the conjectures developed."
+
+    def CollatzConjecture(n: int) -> tuple:
+        "From a given number in input, calculate the Collatz Conjecture. \n\nIt will return at: Index 0: True if the number reaches 1, False if the number reaches the initial number given in input | Index 1: the number of steps taken | Index 2: The steps (numbers reached) |"
+        number = n
+        steps = []
+        while True:
+            if n == 1:
+                return (True, len(steps), steps)
+
+            n = 3*n + 1
+            steps.append(n)
+            while n % 2 == 0:
+                n //= 2
+                steps.append(n)
+
+            if n == number:
+                return (False, len(steps), steps)
+
+    def GoldbachConjecture(n: int) -> list:
+        "The Golbach conjecture states that for any even integer exists two primes p and q with their sum being n. \n\nThe function will use the Sieve of Eratosthenes to calculate all primes below n, and then it will return all the possible combinations."
+
+        if n % 2 == 1:
+            return None
+
+        primes = SieveOfEratosthenes(n)
+        sum = 0
+        Goldbach = []
+
+        for p in primes:
+            sum += p
+
+            for j in primes:
+
+                if sum + j == n:
+                    Goldbach.append((p, j))
+                
+            sum = 0
+
+        return Goldbach
+    
+    def TwinPrimeConjecture(x: int, y: int) -> list:
+        "Given an interval of the type: [x, y] check if there are twin primes in there. \n\nThe fuction will return the twin primes found."
+
+        from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
+
+        twinPrimes = []
+
+        if x % 2 == 0: 
+            x+= 1
+
+        for n in range(x, y+1, 2):
+
+            if MillerRabinPrimalityTest(n, 100) and MillerRabinPrimalityTest(n+2, 100):
+                twinPrimes.append((n, n+2))
+
+        return twinPrimes
+    
 
-    return number / (math.log(number))
```

### Comparing `cryptographyComplements-0.2.9/setup.py` & `cryptographyComplements-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from setuptools import setup, find_packages
+import decimal
 
 setup(
     name='cryptographyComplements',
-    version='0.2.9',
+    version='0.3.0',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
         'Source': 'https://github.com/Forzooo/cryptographyComplements',
         'Documentation': 'https://cryptographycomplements.readthedocs.io/'
     },
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
+    install_requires=[
+        'decimal',
+    ]
 
 )
```

