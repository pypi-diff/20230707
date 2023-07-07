# Comparing `tmp/psy_taliro-1.0.0b8.tar.gz` & `tmp/psy_taliro-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psy_taliro-1.0.0b8.tar", max compression
+gzip compressed data, was "psy_taliro-1.0.0b9.tar", max compression
```

## Comparing `psy_taliro-1.0.0b8.tar` & `psy_taliro-1.0.0b9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1520 2023-05-09 16:22:40.594155 psy_taliro-1.0.0b8/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-21 00:24:23.401552 psy_taliro-1.0.0b8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 23:38:32.004447 psy_taliro-1.0.0b8/src/staliro/__init__.py
--rw-r--r--   0        0        0      786 2023-06-12 23:38:32.004833 psy_taliro-1.0.0b8/src/staliro/core/__init__.py
--rw-r--r--   0        0        0     7484 2023-06-12 23:38:32.004952 psy_taliro-1.0.0b8/src/staliro/core/cost.py
--rw-r--r--   0        0        0     1508 2023-06-12 23:38:32.005305 psy_taliro-1.0.0b8/src/staliro/core/interval.py
--rw-r--r--   0        0        0     1602 2023-06-12 23:38:32.005461 psy_taliro-1.0.0b8/src/staliro/core/layout.py
--rw-r--r--   0        0        0     3215 2023-06-12 23:38:32.005576 psy_taliro-1.0.0b8/src/staliro/core/model.py
--rw-r--r--   0        0        0     2087 2023-06-12 23:38:32.005727 psy_taliro-1.0.0b8/src/staliro/core/optimizer.py
--rw-r--r--   0        0        0     5087 2023-06-12 23:38:32.005906 psy_taliro-1.0.0b8/src/staliro/core/result.py
--rw-r--r--   0        0        0     1733 2023-06-12 23:38:32.006035 psy_taliro-1.0.0b8/src/staliro/core/sample.py
--rw-r--r--   0        0        0     8058 2023-06-12 23:38:32.006184 psy_taliro-1.0.0b8/src/staliro/core/scenario.py
--rw-r--r--   0        0        0      763 2023-06-12 23:38:32.006343 psy_taliro-1.0.0b8/src/staliro/core/signal.py
--rw-r--r--   0        0        0     1222 2023-06-12 23:38:32.006459 psy_taliro-1.0.0b8/src/staliro/core/specification.py
--rw-r--r--   0        0        0     5133 2023-06-12 23:38:32.006577 psy_taliro-1.0.0b8/src/staliro/models.py
--rw-r--r--   0        0        0     5430 2023-06-12 23:38:32.006693 psy_taliro-1.0.0b8/src/staliro/optimizers.py
--rw-r--r--   0        0        0     5180 2023-06-12 23:38:32.006871 psy_taliro-1.0.0b8/src/staliro/options.py
--rw-r--r--   0        0        0      155 2023-05-09 16:22:40.597460 psy_taliro-1.0.0b8/src/staliro/parser/__init__.py
--rw-r--r--   0        0        0     1317 2023-05-09 16:22:40.597538 psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlLexer.g4
--rw-r--r--   0        0        0      791 2023-05-09 16:22:40.597591 psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlParser.g4
--rw-r--r--   0        0        0     3431 2023-05-16 00:14:46.061497 psy_taliro-1.0.0b8/src/staliro/parser/parser.py
--rw-r--r--   0        0        0    12212 2023-05-09 16:22:40.597746 psy_taliro-1.0.0b8/src/staliro/parser/stlLexer.py
--rw-r--r--   0        0        0    32028 2023-05-09 16:22:40.597877 psy_taliro-1.0.0b8/src/staliro/parser/stlParser.py
--rw-r--r--   0        0        0     3986 2023-05-09 16:22:40.597963 psy_taliro-1.0.0b8/src/staliro/parser/stlParserListener.py
--rw-r--r--   0        0        0     6496 2023-05-09 16:22:40.598018 psy_taliro-1.0.0b8/src/staliro/parser/stlParserVisitor.py
--rw-r--r--   0        0        0     8586 2023-05-09 16:22:40.598105 psy_taliro-1.0.0b8/src/staliro/parser/stlTptlParserVisitorTranslator.py
--rw-r--r--   0        0        0        0 2023-05-09 16:22:40.598128 psy_taliro-1.0.0b8/src/staliro/py.typed
--rw-r--r--   0        0        0     4547 2023-06-12 23:38:32.007007 psy_taliro-1.0.0b8/src/staliro/signals.py
--rw-r--r--   0        0        0    10272 2023-06-12 23:38:32.007174 psy_taliro-1.0.0b8/src/staliro/specifications.py
--rw-r--r--   0        0        0     4168 2023-06-12 23:38:32.007310 psy_taliro-1.0.0b8/src/staliro/staliro.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 psy_taliro-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-07-06 18:05:07.729803 psy_taliro-1.0.0b9/LICENSE
+-rw-r--r--   0        0        0     2192 2023-07-07 18:31:03.198203 psy_taliro-1.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 18:05:07.732943 psy_taliro-1.0.0b9/src/staliro/__init__.py
+-rw-r--r--   0        0        0      786 2023-07-06 18:05:07.733069 psy_taliro-1.0.0b9/src/staliro/core/__init__.py
+-rw-r--r--   0        0        0     7484 2023-07-06 18:05:07.733165 psy_taliro-1.0.0b9/src/staliro/core/cost.py
+-rw-r--r--   0        0        0     1508 2023-07-06 18:05:07.733243 psy_taliro-1.0.0b9/src/staliro/core/interval.py
+-rw-r--r--   0        0        0     1602 2023-07-06 18:05:07.733306 psy_taliro-1.0.0b9/src/staliro/core/layout.py
+-rw-r--r--   0        0        0     3215 2023-07-06 18:05:07.733393 psy_taliro-1.0.0b9/src/staliro/core/model.py
+-rw-r--r--   0        0        0     2087 2023-07-06 18:05:07.733472 psy_taliro-1.0.0b9/src/staliro/core/optimizer.py
+-rw-r--r--   0        0        0     5087 2023-07-06 18:05:07.733553 psy_taliro-1.0.0b9/src/staliro/core/result.py
+-rw-r--r--   0        0        0     1733 2023-07-06 18:05:07.733629 psy_taliro-1.0.0b9/src/staliro/core/sample.py
+-rw-r--r--   0        0        0     8058 2023-07-06 18:05:07.733721 psy_taliro-1.0.0b9/src/staliro/core/scenario.py
+-rw-r--r--   0        0        0      763 2023-07-06 18:05:07.733788 psy_taliro-1.0.0b9/src/staliro/core/signal.py
+-rw-r--r--   0        0        0     1222 2023-07-06 18:05:07.733859 psy_taliro-1.0.0b9/src/staliro/core/specification.py
+-rw-r--r--   0        0        0     5133 2023-07-06 18:05:07.733942 psy_taliro-1.0.0b9/src/staliro/models.py
+-rw-r--r--   0        0        0     5430 2023-07-06 18:05:07.734042 psy_taliro-1.0.0b9/src/staliro/optimizers.py
+-rw-r--r--   0        0        0     5180 2023-07-06 18:05:07.734142 psy_taliro-1.0.0b9/src/staliro/options.py
+-rw-r--r--   0        0        0      155 2023-07-06 18:05:07.734233 psy_taliro-1.0.0b9/src/staliro/parser/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-06 18:05:07.734347 psy_taliro-1.0.0b9/src/staliro/parser/grammar/stlLexer.g4
+-rw-r--r--   0        0        0      791 2023-07-06 18:05:07.734418 psy_taliro-1.0.0b9/src/staliro/parser/grammar/stlParser.g4
+-rw-r--r--   0        0        0     3431 2023-07-06 18:05:07.734495 psy_taliro-1.0.0b9/src/staliro/parser/parser.py
+-rw-r--r--   0        0        0    12212 2023-07-06 18:05:07.734610 psy_taliro-1.0.0b9/src/staliro/parser/stlLexer.py
+-rw-r--r--   0        0        0    32028 2023-07-06 18:05:07.734803 psy_taliro-1.0.0b9/src/staliro/parser/stlParser.py
+-rw-r--r--   0        0        0     3986 2023-07-06 18:05:07.734928 psy_taliro-1.0.0b9/src/staliro/parser/stlParserListener.py
+-rw-r--r--   0        0        0     6496 2023-07-06 18:05:07.734990 psy_taliro-1.0.0b9/src/staliro/parser/stlParserVisitor.py
+-rw-r--r--   0        0        0     8586 2023-07-06 18:05:07.735080 psy_taliro-1.0.0b9/src/staliro/parser/stlTptlParserVisitorTranslator.py
+-rw-r--r--   0        0        0        0 2023-07-06 18:05:07.735103 psy_taliro-1.0.0b9/src/staliro/py.typed
+-rw-r--r--   0        0        0     4547 2023-07-06 18:05:07.735193 psy_taliro-1.0.0b9/src/staliro/signals.py
+-rw-r--r--   0        0        0    10387 2023-07-07 18:30:35.104870 psy_taliro-1.0.0b9/src/staliro/specifications.py
+-rw-r--r--   0        0        0     4168 2023-07-06 18:05:07.735374 psy_taliro-1.0.0b9/src/staliro/staliro.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 psy_taliro-1.0.0b9/PKG-INFO
```

### Comparing `psy_taliro-1.0.0b8/LICENSE` & `psy_taliro-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/__init__.py` & `psy_taliro-1.0.0b9/src/staliro/core/__init__.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/cost.py` & `psy_taliro-1.0.0b9/src/staliro/core/cost.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/interval.py` & `psy_taliro-1.0.0b9/src/staliro/core/interval.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/layout.py` & `psy_taliro-1.0.0b9/src/staliro/core/layout.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/model.py` & `psy_taliro-1.0.0b9/src/staliro/core/model.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/optimizer.py` & `psy_taliro-1.0.0b9/src/staliro/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/result.py` & `psy_taliro-1.0.0b9/src/staliro/core/result.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/sample.py` & `psy_taliro-1.0.0b9/src/staliro/core/sample.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/scenario.py` & `psy_taliro-1.0.0b9/src/staliro/core/scenario.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/signal.py` & `psy_taliro-1.0.0b9/src/staliro/core/signal.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/core/specification.py` & `psy_taliro-1.0.0b9/src/staliro/core/specification.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/models.py` & `psy_taliro-1.0.0b9/src/staliro/models.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/optimizers.py` & `psy_taliro-1.0.0b9/src/staliro/optimizers.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/options.py` & `psy_taliro-1.0.0b9/src/staliro/options.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlLexer.g4` & `psy_taliro-1.0.0b9/src/staliro/parser/grammar/stlLexer.g4`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/grammar/stlParser.g4` & `psy_taliro-1.0.0b9/src/staliro/parser/grammar/stlParser.g4`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/parser.py` & `psy_taliro-1.0.0b9/src/staliro/parser/parser.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/stlLexer.py` & `psy_taliro-1.0.0b9/src/staliro/parser/stlLexer.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/stlParser.py` & `psy_taliro-1.0.0b9/src/staliro/parser/stlParser.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/stlParserListener.py` & `psy_taliro-1.0.0b9/src/staliro/parser/stlParserListener.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/stlParserVisitor.py` & `psy_taliro-1.0.0b9/src/staliro/parser/stlParserVisitor.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/parser/stlTptlParserVisitorTranslator.py` & `psy_taliro-1.0.0b9/src/staliro/parser/stlTptlParserVisitorTranslator.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/signals.py` & `psy_taliro-1.0.0b9/src/staliro/signals.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/src/staliro/specifications.py` & `psy_taliro-1.0.0b9/src/staliro/specifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from math import inf
+from sys import platform
 from typing import TYPE_CHECKING, Any, Dict, Iterable, NewType, Optional, Sequence, Tuple, TypeVar
 
 import numpy as np
 from attrs import field, frozen
 from numpy.typing import NDArray
 
 try:
-    from rtamt import Language, Semantics, STLDenseTimeSpecification, STLDiscreteTimeSpecification
+    from rtamt import Language, Semantics, StlDenseTimeSpecification, StlDiscreteTimeSpecification
 except ImportError:
     _has_rtamt = False
 else:
     _has_rtamt = True
 
 from .core import Specification, SpecificationError
 
@@ -90,17 +91,20 @@
     Attributes:
         phi: The specification requirement
         predicates: A set of Predicate(s) used in the requirement
     """
 
     def __init__(self, phi: str, column_map: PredicateColumnMap):
         if not _can_parse:
-            raise RuntimeError(
-                "TLTK specifications require parsing functionality. Please refer to the documentation for how to enable parsing."
-            )
+            if platform == "linux":
+                raise RuntimeError(
+                    "TLTK specifications require parsing functionality. Please refer to the documentation for how to enable parsing."
+                )
+            else:
+                raise RuntimeError("TLTK specification is only available on Linux")
 
         tltk_obj = parse(phi, list(column_map.keys()))
 
         if tltk_obj is None:
             raise SpecificationError("could not parse formula")
 
         self.tltk_obj = tltk_obj
@@ -123,81 +127,81 @@
 
     Attributes:
         phi: The specification requirement
         predicates: A set of Predicate(s) used in the requirement
     """
 
     def __init__(self, phi: str, column_map: PredicateColumnMap):
-        if not _has_rtamt:
-            raise RuntimeError("RTAMT must be installed to use RTAMTDiscrete specification")
-
         if "time" in column_map:
             raise SpecificationError("'time' cannot be used as a predicate name for RTAMT")
 
-        self.rtamt_obj = STLDiscreteTimeSpecification(Semantics.STANDARD, language=Language.PYTHON)
-
-        self.rtamt_obj.spec = phi
+        self.phi = phi
         self.column_map = column_map
 
-        for name in column_map:
-            self.rtamt_obj.declare_var(name, "float")
-
     def evaluate(self, states: Sequence[Sequence[float]], times: Sequence[float]) -> float:
+        if not _has_rtamt:
+            raise RuntimeError("RTAMT must be installed to use RTAMTDiscrete specification")
+
         times_, states_ = _parse_times_states(times, states)
 
         if times_.size < 2:
             raise RuntimeError("timestamps must have at least two samples to evaluate")
 
-        self.rtamt_obj.reset()
+        spec = StlDiscreteTimeSpecification()
+
+        for name in self.column_map:
+            spec.declare_var(name, "float")
 
         period = times[1] - times[0]
-        self.rtamt_obj.set_sampling_period(round(period, 2), "s", 0.1)
 
-        self.rtamt_obj.parse()
+        spec.set_sampling_period(round(period, 2), "s", 0.1)
+        spec.spec = self.phi
+        spec.parse()
+
         traces = {"time": list(times)}
 
         for name, column in self.column_map.items():
             traces[name] = list(states[column])
 
-        robustness = self.rtamt_obj.evaluate(traces)
+        robustness = spec.evaluate(traces)
         return robustness[0][1]
 
 
 class RTAMTDense(StlSpecification):
     """STL logic specification that uses RTAMT dense-time semantics to compute robustness.
 
     Attributes:
         phi: The specification requirement
         predicates: A set of Predicate(s) used in the requirement
     """
 
     def __init__(self, phi: str, column_map: PredicateColumnMap):
-        if not _has_rtamt:
-            raise RuntimeError("RTAMT must be installed to use RTAMTDense specification")
-
-        self.rtamt_obj = STLDenseTimeSpecification(Semantics.STANDARD, language=Language.PYTHON)
+        self.phi = phi
         self.column_map = column_map
-        self.rtamt_obj.spec = phi
-
-        for name in column_map:
-            self.rtamt_obj.declare_var(name, "float")
 
     def evaluate(self, states: Sequence[Sequence[float]], times: Sequence[float]) -> float:
+        if not _has_rtamt:
+            raise RuntimeError("RTAMT must be installed to use RTAMTDense specification")
+
         times_, states_ = _parse_times_states(times, states)
+        spec = StlDenseTimeSpecification()
 
-        self.rtamt_obj.reset()
-        self.rtamt_obj.parse()
+        for name in self.column_map:
+            spec.declare_var(name, "float")
+
+        spec.spec = self.phi
+        spec.parse()
 
         map_items = self.column_map.items()
         traces = [
             (name, np.array([times_.tolist(), states_[column]]).T.tolist())
             for name, column in map_items
         ]
 
-        robustness = self.rtamt_obj.evaluate(*traces)
+        robustness = spec.evaluate(*traces)
         return robustness[0][1]
 
 
 @frozen(slots=True)
 class TaliroPredicate:
     name: str = field(kw_only=True)
     A: NDArray[np.float_] = field(kw_only=True)
@@ -232,15 +236,19 @@
     Attributes:
         phi: The specification requirement
         predicates: A set of Predicate(s) used in the requirement
     """
 
     def __init__(self, phi: str, predicate_map: Iterable[TaliroPredicate]):
         if not _has_tptaliro:
-            raise RuntimeError("Py-TaLiRo must be installed to use TP-TaLiRo specification")
+            if platform == "linux":
+                raise RuntimeError("Py-TaLiRo must be installed to use TP-TaLiRo specification")
+            else:
+                raise RuntimeError("Py-TaLiRo is only available on Linux")
+
         if not _can_translate:
             raise RuntimeError("TP-TaLiRo specifications require translation functionality.")
 
         # translate STL to TPTL; else, assume valid TPTL
         try:
             self.spec = translate(phi, TemporalLogic.STL, TemporalLogic.TPTL)
         except SpecificationSyntaxError:
```

### Comparing `psy_taliro-1.0.0b8/src/staliro/staliro.py` & `psy_taliro-1.0.0b9/src/staliro/staliro.py`

 * *Files identical despite different names*

### Comparing `psy_taliro-1.0.0b8/PKG-INFO` & `psy_taliro-1.0.0b9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psy-taliro
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: System-level verification library using STL
 License: BSD-3-Clause
 Author: Quinn Thibeault
 Author-email: qthibeau@asu.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -14,12 +14,12 @@
 Provides-Extra: pytaliro
 Provides-Extra: rtamt
 Provides-Extra: tltk
 Requires-Dist: antlr4-python3-runtime (>=4.7)
 Requires-Dist: attrs (>=21.0.0,<22.0.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.21.5,<2.0.0)
-Requires-Dist: py-taliro (>=0.2.1,<0.3.0) ; extra == "pytaliro"
+Requires-Dist: py-taliro (>=0.2.1,<0.3.0) ; (sys_platform == "linux") and (extra == "pytaliro")
 Requires-Dist: rtamt (>=0.3.5,<0.4.0) ; extra == "rtamt"
 Requires-Dist: scipy (>=1.6.2,<2.0.0)
 Requires-Dist: tltk-mtl (>=0.0.27,<0.0.28) ; (sys_platform == "linux") and (extra == "tltk")
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
```

