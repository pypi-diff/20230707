# Comparing `tmp/probability_calculator-0.2.0.tar.gz` & `tmp/probability_calculator-0.3.0.tar.gz`

## Comparing `probability_calculator-0.2.0.tar` & `probability_calculator-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/README_files/README_1_0.png
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/README_files/README_3_0.png
--rw-r--r--   0        0        0     5593 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/README_files/README_5_0.png
--rw-r--r--   0        0        0    25307 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/docs/README.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/src/probability_calculator/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/src/probability_calculator/density.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/src/probability_calculator/outcome.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/src/probability_calculator/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/.gitignore
--rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/LICENSE
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/README.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 probability_calculator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/.github/workflows/python-package-with-hatch.yml
+-rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/README_files/README_1_0.png
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/README_files/README_3_0.png
+-rw-r--r--   0        0        0    11437 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/README_files/README_5_0.png
+-rw-r--r--   0        0        0    48897 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/docs/README.ipynb
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/src/probability_calculator/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/src/probability_calculator/part.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/src/probability_calculator/random_variables.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/.gitignore
+-rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 probability_calculator-0.3.0/PKG-INFO
```

### Comparing `probability_calculator-0.2.0/src/probability_calculator/density.py` & `probability_calculator-0.3.0/src/probability_calculator/random_variables.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,109 @@
-import math
-from typing import Optional, List
-from .outcome import Outcome, ExportedOutcome, DiskreteOutcome
-from .plot import plotDensity
-
-
-class DiscreteDensity:
-    def __init__(self, outcomes: List[ExportedOutcome] = [], _outcomes: Optional[List[Outcome]] = None):
-        self._outcomes: List[Outcome] = _outcomes if _outcomes is not None else [
-        ]
-
-        for o in outcomes:
-            self._outcomes.append(
-                DiskreteOutcome(value=o["value"], prob=o["prob"])
-            )
-
-        self.simplify()
-
-    def plot(self):
-        """
-        plots the density with matplotlib
-        """
-        return plotDensity(self)
-
-    def simplify(self):
-        """
-        simplifies the list of outcomes by combining elements
-        """
-        outcomes = sorted(self._outcomes, key=lambda o: o.getValue())
-        newOutcomes: List[Outcome] = []
-        lastOutcome: Optional[Outcome] = None
-        for o in outcomes:
-            if lastOutcome is not None and isinstance(lastOutcome, DiskreteOutcome) and isinstance(o, DiskreteOutcome) and math.isclose(lastOutcome.getValue(), o.getValue()):
-                # two DiskreteOutcomes with the same value -> join together
-                lastOutcome.addProb(o.getProb())
-            else:
-                newOutcomes.append(o)
-                lastOutcome = o
-
-        self._outcomes = newOutcomes
-
-    def exportOutcomes(self):
-        outcomes: List[ExportedOutcome] = []
-        for o in self._outcomes:
-            outcomes.extend(o.export())
-
+import itertools
+from fractions import Fraction
+from typing import List, Literal
+from .part import Outcome, _Part
+import matplotlib.pyplot as plt
+
+
+class RandomVariable:
+    def __init__(self, outcomes: List[Outcome] = [], _parts: List[_Part] = []):
+        parts = []
+        for part in _parts:
+            parts.append(part)
+        for outcome in outcomes:
+            p = outcome["p"]
+            value = outcome["value"]
+            parts.append(_Part(
+                p,
+                value,
+                value**2,
+                value,
+                value
+            ))
+
+        self._parts = RandomVariable._simplifyParts(parts)
+
+    def outcomes(self):
+        outcomes: List[Outcome] = list(
+            itertools.chain(*[part.outcomes() for part in self._parts]))
         return outcomes
 
-    def __mul__(self, other):
-        outcomes = []
-        for o1 in self._outcomes:
-            for o2 in other._outcomes:
-                outcomes.append(o1+o2)
+    def __add__(self, other):
+        parts = []
+        for part1 in self._parts:
+            for part2 in other._parts:
+                parts.append(part1 + part2)
+        return RandomVariable(_parts=parts)
+
+    def __rmul__(self, other):
+        if not isinstance(other, int):
+            raise NotImplementedError
 
-        return DiscreteDensity(_outcomes=outcomes)
+        return self * other
 
-    def __pow__(self, other):
+    def __mul__(self, other):
         if isinstance(other, int):
-            if other == 1:
+            if other <= 0:
+                raise NotImplementedError
+            elif other == 1:
                 return self
-            elif other > 1:
-                return self * (self**(other-1))
+            else:
+                return self + self * (other - 1)
+        elif not isinstance(other, RandomVariable):
+            raise NotImplemented
+
+        parts = []
+        for part1 in self._parts:
+            for part2 in other._parts:
+                parts.append(part1 * part2)
+        return RandomVariable(_parts=parts)
+
+    def plot_outcomes(
+            self,
+            xscale: Literal["linear", "log"] = "linear",
+            yscale: Literal["linear", "log"] = "linear"):
+        outcomes = self.outcomes()
+        x = [o["value"] for o in outcomes]
+        y = [o["p"] for o in outcomes]
+        fig, ax = plt.subplots()
+        ax.set_xscale(xscale)
+        ax.set_yscale(yscale)
+        ax.plot(x, y, "o", ms=4, alpha=0.7)
+        if yscale == "linear":
+            ax.set_ylim(bottom=0)
+        plt.show()
+        plt.close()
+        return fig, ax
+
+    @staticmethod
+    def _simplifyParts(parts: List[_Part]):
+        sortedParts = sorted(parts, key=lambda part: part._min)
+        simplifiedParts = []
+
+        i = 0
+        while i < len(sortedParts):
+            part = sortedParts[i]
+            j = i + 1
+            while j < len(sortedParts):
+                nextPart = sortedParts[j]
+                if nextPart._min != part._min or nextPart._max != part._max:
+                    break
+
+                j += 1
+
+            selectedParts = sortedParts[i:j]
+            simplifiedParts.append(_Part.merge(selectedParts))
+            i = j
 
-        return NotImplemented
+        return simplifiedParts
 
 
-class Dice(DiscreteDensity):
+class FairDie(RandomVariable):
     def __init__(self, n):
         """
-        Generates a fair dice with n sides
+        Generates a fair die with n sides
         """
-        prob = 1./n
-        outcomes = []
-        for i in range(1, n+1):
-            outcomes.append({"value": i, "prob": prob})
+        p = Fraction(1, n)
+        outcomes = [Outcome(p=p, value=i) for i in range(1, n + 1)]
 
         super().__init__(outcomes)
```

### Comparing `probability_calculator-0.2.0/LICENSE` & `probability_calculator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `probability_calculator-0.2.0/pyproject.toml` & `probability_calculator-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "probability_calculator"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Hendrik Roehm", email="git@roehm.ws" },
 ]
 description = "Calculate with and analyze probability densities."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -12,14 +12,21 @@
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 3 - Alpha"
 ]
 
+
+dependencies = [
+  "matplotlib",
+  "scipy",
+  "autopep8",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/HendrikRoehm/probability_calculator"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

