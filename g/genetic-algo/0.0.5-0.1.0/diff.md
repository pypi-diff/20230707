# Comparing `tmp/genetic-algo-0.0.5.tar.gz` & `tmp/genetic-algo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.0.5.tar", last modified: Mon Jul  3 14:17:48 2023, max compression
+gzip compressed data, was "genetic-algo-0.1.0.tar", last modified: Fri Jul  7 10:21:50 2023, max compression
```

## Comparing `genetic-algo-0.0.5.tar` & `genetic-algo-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.094955 genetic-algo-0.0.5/
--rw-rw-rw-   0        0        0      115 2023-07-03 14:17:47.000000 genetic-algo-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-07-03 14:17:48.093960 genetic-algo-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.0.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.5/build.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.078955 genetic-algo-0.0.5/genetic_algo/
--rw-rw-rw-   0        0        0     8921 2023-07-03 14:16:05.000000 genetic-algo-0.0.5/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     5957 2023-07-03 14:16:25.000000 genetic-algo-0.0.5/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    15386 2023-07-03 14:16:58.000000 genetic-algo-0.0.5/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     4843 2023-07-03 14:17:21.000000 genetic-algo-0.0.5/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.092983 genetic-algo-0.0.5/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-07-03 14:17:47.000000 genetic-algo-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:17:48.094955 genetic-algo-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-07-03 14:17:45.000000 genetic-algo-0.0.5/setup.py
--rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.5/test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.543813 genetic-algo-0.1.0/
+-rw-rw-rw-   0        0        0      115 2023-07-07 10:21:48.000000 genetic-algo-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2040 2023-07-07 10:21:50.542807 genetic-algo-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.528807 genetic-algo-0.1.0/genetic_algo/
+-rw-rw-rw-   0        0        0     9646 2023-07-07 10:19:44.000000 genetic-algo-0.1.0/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     6092 2023-07-07 10:20:42.000000 genetic-algo-0.1.0/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    15837 2023-07-07 10:18:26.000000 genetic-algo-0.1.0/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4930 2023-07-07 10:21:09.000000 genetic-algo-0.1.0/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.541836 genetic-algo-0.1.0/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-07-07 10:21:48.000000 genetic-algo-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:21:50.543813 genetic-algo-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-07-07 10:21:27.000000 genetic-algo-0.1.0/setup.py
+-rw-rw-rw-   0        0        0     2842 2023-07-07 10:15:25.000000 genetic-algo-0.1.0/test.py
```

### Comparing `genetic-algo-0.0.5/PKG-INFO` & `genetic-algo-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.5
+Version: 0.1.0
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.5/README.md` & `genetic-algo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.5/build.py` & `genetic-algo-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.5/genetic_algo/attributes.py` & `genetic-algo-0.1.0/genetic_algo/attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     "FloatAttribute"
 ]
 
 @represent
 class Arguments:
     """A class to represent a fitness function."""
 
+    __slots__ = "args", "kwargs"
+
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
         Calls the fitness function on the solution.
 
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments.
         """
@@ -71,14 +73,16 @@
     EXCLUDED: Iterable[Any] = []
 
     arguments = Arguments()
 
     __modifiers__ = Modifiers()
     __modifiers__.properties = True
 
+    __slots__ = "_value", "name"
+
     def __init__(self, value: _V, name: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param value: The value of the attribute.
         :param name: The name of the attribute.
         """
@@ -179,30 +183,35 @@
     """A class to represent an attribute of a solution."""
 
     BASE: Type[Number] = float
 
     FLOOR: Number = None
     ROOF: Number = None
     STEP: Optional[Number] = None
+    PRECISION: Optional[Number] = None
+
+    __slots__ = ()
 
     @classmethod
     def generate(
             cls,
             base: Optional[Type[Number]] = None,
             floor: Optional[Number] = None,
             roof: Optional[Number] = None,
-            step: Optional[Number] = None
+            step: Optional[Number] = None,
+            precision: Optional[Number] = None
     ) -> Number:
         """
         Generates the random attribute value.
 
         :param base: The type of the number.
         :param floor: The floor limit value.
         :param roof: The roof limit value.
         :param step: The step size.
+        :param precision: The precision size.
 
         :return: The attribute value.
         """
 
         if base is None:
             base = cls.BASE
         # end if
@@ -215,14 +224,18 @@
             roof = cls.ROOF
         # end if
 
         if step is None:
             step = cls.STEP
         # end if
 
+        if precision is None:
+            precision = cls.PRECISION
+        # end if
+
         if issubclass(base, int):
             floor = int(floor)
             roof = int(roof)
 
             if step is None:
                 return random.randint(floor, roof)
 
@@ -233,25 +246,32 @@
                 raise ValueError(
                     f"{cls} 'step' must be an int when "
                     f"'base' is an int, not {step}."
                 )
             # end if
 
         elif issubclass(base, float):
-            if step is None:
+            if step is None and precision is not None:
+                return round(random.uniform(floor, roof), precision)
+
+            elif step is None:
                 return random.uniform(floor, roof)
 
             elif isinstance(step, (int, float)):
+                if precision is None:
+                    precision = len(str(step - int(step))) - 1
+                # end if
+
                 values = [floor]
 
                 while values[-1] <= roof:
                     values.append(values[-1] + step)
                 # end while
 
-                return random.choice(values)
+                return round(random.choice(values), precision)
 
             else:
                 raise ValueError(
                     f"{cls} 'step' must be an int or a float when "
                     f"'base' is an int, not {step}."
                 )
             # end if
@@ -269,34 +289,42 @@
     """A class to represent an attribute of a solution."""
 
     BASE = int
 
     FLOOR = 0
     ROOF = 100
     STEP = 1
+    PRECISION = 0
+
+    __slots__ = ()
 # end IntegerAttribute
 
 class FloatAttribute(NumericAttribute[float]):
     """A class to represent an attribute of a solution."""
 
     BASE = float
 
     FLOOR = 0.0
     ROOF = 1.0
     STEP = 0.01
+    PRECISION = 8
+
+    __slots__ = ()
 # end FloatAttribute
 
 class StringAttribute(Attribute[str]):
     """A class to represent an attribute of a solution."""
 
     SOURCE: Iterable[str] = string.ascii_lowercase
     SEPARATOR: str = ""
 
     LENGTH: int = 10
 
+    __slots__ = ()
+
     @classmethod
     def generate(
             cls,
             source: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None
     ) -> str:
@@ -349,14 +377,16 @@
         return separator.join(random.choices(list(source), k=length))
     # end generate
 # end StringAttribute
 
 class BooleanAttribute(Attribute[bool]):
     """A class to represent an attribute of a solution."""
 
+    __slots__ = ()
+
     @classmethod
     def generate(cls) -> bool:
         """
         Generates the random attribute value.
 
         :return: The attribute value.
         """
```

### Comparing `genetic-algo-0.0.5/genetic_algo/driver.py` & `genetic-algo-0.1.0/genetic_algo/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     "DriverDefinition"
 ]
 
 @represent
 class DriverDefinition:
     """A class to contain the definition values of a driver object."""
 
+    __slots__ = "fitness_limit", "max_generations", "min_improvement", "min_count"
+
     def __init__(
             self,
             fitness_limit: float,
             max_generations: int,
             min_improvement: float,
             min_count: Optional[int] = None
     ) -> None:
@@ -34,15 +36,15 @@
 
         if min_count is None:
             min_count = 1
         # end if
 
         self.fitness_limit = fitness_limit
         self.max_generations = max_generations
-        self.count_limit = min_count
+        self.min_count = min_count
 
         self.min_improvement = scale(
             min_improvement, size=1, name="minimum improvement"
         )
     # end __init__
 
     def copy(self) -> Self:
@@ -60,14 +62,16 @@
     # end copy
 # end DriverDefinition
 
 @represent
 class Driver:
     """A class to represent a driver for genetic algorithm environments."""
 
+    __slots__ = "definition", "environment"
+
     def __init__(
             self,
             definition: DriverDefinition,
             environment: Environment
     ) -> None:
         """
         Defines the class attributes.
@@ -152,16 +156,16 @@
 
         :return: The value to stop the process.
         """
 
         return (
             (not generation.solutions) or
             (
-                isinstance(self.definition.count_limit, int) and
-                (self.definition.count_limit >= len(generation.solutions))
+                    isinstance(self.definition.min_count, int) and
+                    (self.definition.min_count >= len(generation.solutions))
             )
         )
     # end finish
 
     def stop(self, generation: Generation, previous: Optional[Generation] = None) -> bool:
         """
         Checks the value to stop the process.
```

### Comparing `genetic-algo-0.0.5/genetic_algo/environment.py` & `genetic-algo-0.1.0/genetic_algo/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     "scale"
 ]
 
 @represent
 class Generation:
     """A class to represent a generation of solutions."""
 
+    __slots__ = "solutions",
+
     def __init__(self, solutions: Iterable[Solution]) -> None:
         """
         Defines the class attributes.
 
         :param solutions: The solutions of the generation.
         """
 
@@ -105,14 +107,19 @@
     # end if
 # end scale
 
 @represent
 class EnvironmentDefinition:
     """A class to define the attributes of an environment."""
 
+    __slots__ = (
+        "size", "ascending", "successors", "continuers", "padding",
+        "eliminations", "parents", "mutations", "repetitions"
+    )
+
     def __init__(
             self,
             size: int,
             ascending: bool,
             successors: Optional[Union[int, float]] = None,
             continuers: Optional[Union[int, float]] = None,
             eliminations: Optional[Union[int, float]] = None,
@@ -137,14 +144,18 @@
 
         self.size = size
 
         self.ascending = ascending
         self.repetitions = repetitions
         self.padding = padding
 
+        if eliminations is None:
+            eliminations = 0
+        # end if
+
         self.successors = scale(successors, size=size, name="successors")
         self.continuers = scale(continuers, size=size, name="continuers")
         self.eliminations = scale(eliminations, size=size, name="eliminations")
         self.parents = scale(parents, size=size, name="parents")
         self.mutations = scale(mutations, size=1, name="mutations")
     # end __init__
 
@@ -168,14 +179,16 @@
     # end copy
 # end EnvironmentDefinition
 
 @represent
 class Fitness:
     """A class to represent a fitness function."""
 
+    __slots__ = ()
+
     def __call__(self, solution: Solution) -> float:
         """
         Calls the fitness function on the solution.
 
         :param solution: The solution object.
 
         :return: The fitness value.
@@ -196,14 +209,16 @@
     # end call
 # end Fitness
 
 @represent
 class History:
     """A class to represent an environment history."""
 
+    __slots__ = "generations",
+
     def __init__(self, generations: Optional[Iterable[Generation]] = None) -> None:
         """
         Defines the class attributes.
 
         :param generations: The generations to add to the history.
         """
 
@@ -223,14 +238,19 @@
 
 @represent
 class Environment:
     """A class to represent an environment."""
 
     OPTIMIZE = False
 
+    __slots__ = (
+        "definition", "template", "fitness",
+        "generation", "history", "optimize"
+    )
+
     def __init__(
             self,
             definition: EnvironmentDefinition,
             template: Template,
             fitness: Fitness,
             generation: Optional[Type[Generation]] = None,
             history: Optional[History] = None,
```

### Comparing `genetic-algo-0.0.5/genetic_algo/solution.py` & `genetic-algo-0.1.0/genetic_algo/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     "same_solution"
 ]
 
 @represent
 class Solution:
     """A class to represent a solution of a problem."""
 
+    __slots__ = "attributes", "fitness"
+
     def __init__(self, attributes: Iterable[Attribute]) -> None:
         """
         Defines the class attributes.
 
         :param attributes: The attributes of the solution.
         """
 
@@ -126,14 +128,16 @@
 @represent
 class Template(Generic[_S]):
     """A class to represent a template for solution attributes."""
 
     SOLUTION: _S = Solution
     ATTRIBUTES: Attributes = []
 
+    __slots__ = "solution", "attributes"
+
     def __init__(
             self,
             solution: Optional[Type[_S]] = None,
             attributes: Optional[Attributes] = None
     ) -> None:
         """
         Defines the class attributes.
```

### Comparing `genetic-algo-0.0.5/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-0.1.0/genetic_algo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.5
+Version: 0.1.0
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.5/pyproject.toml` & `genetic-algo-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.0.5'
+version = '0.1.0'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.0.5/setup.py` & `genetic-algo-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.0.5',
+        version='0.1.0',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.0.5/test.py` & `genetic-algo-0.1.0/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 # test.py
 
-from genetic_algo.attributes import IntegerAttribute
+from genetic_algo.attributes import FloatAttribute
 from genetic_algo.solution import Template, Solution
 from genetic_algo.driver import DriverDefinition, Driver
 from genetic_algo.environment import (
     Environment, EnvironmentDefinition, Fitness, History
 )
 
-class Parameter(IntegerAttribute):
+class Parameter(FloatAttribute):
     """A class to represent an attribute of a solution."""
 
-    FLOOR = -20
-    ROOF = 20
-    STEP = 1
+    FLOOR = -5
+    ROOF = 5
+    STEP = 0.1
 
     EXCLUDED = [0]
 # end Parameter
 
 class CombinationSolution(Solution):
     """A class to represent a solution of a problem."""
 # end CombinationSolution
 
 class FormulaTemplate(Template):
     """A class to represent a template for solution attributes."""
 
     SOLUTION = CombinationSolution
-    ATTRIBUTES = [Parameter, Parameter]
+    ATTRIBUTES = [Parameter, Parameter, Parameter]
 # end FormulaTemplate
 
 class MeanAbsoluteError(Fitness):
     """A class to represent a fitness function."""
 
-    variables = list(map(lambda x: x / 100, range(-1000, 1000)))
+    variables = list(range(-1000, 1000))
 
     def call(self, solution: CombinationSolution) -> float:
         """
         Calls the fitness function on the solution.
 
         :param solution: The solution object.
 
         :return: The fitness value.
         """
 
         # a * x ^ 2 + b * x + c = 0
-        # x ^ 2 - 4 * x + 4 = 0
+        # Finds a function with the minima of 1.
 
-        return sum(
-            abs(
-                (
-                    solution.attributes[0].value * (value ** 2) +
-                    solution.attributes[1].value * value
-                ) - solution.attributes[1].value
-            )
-            for value in self.variables
-        ) / len(self.variables)
+        return round(
+            sum(
+                abs(
+                    (
+                        (
+                            solution.attributes[0].value * (value ** 2) +
+                            solution.attributes[1].value * value +
+                            solution.attributes[2].value
+                        ) - 1
+                    ) / (value if value != 0 else 1)
+                )
+                for value in self.variables
+            ) / len(self.variables), 5
+        )
     # end call
 # end MeanAbsoluteError
 
 def main() -> None:
     """The main function to run the test."""
 
     environment_definition = EnvironmentDefinition(
         size=100,
         ascending=False,
         repetitions=False,
         padding=True,
         parents=2,
-        eliminations=60,
-        successors=30,
-        continuers=10,
+        eliminations=0.05,
+        successors=0.5,
+        continuers=0.05,
         mutations=0.01
     )
 
     template = FormulaTemplate()
     fitness = MeanAbsoluteError()
     history = History()
 
@@ -80,15 +85,15 @@
         definition=environment_definition,
         template=template,
         fitness=fitness,
         history=history
     )
 
     deriver_definition = DriverDefinition(
-        fitness_limit=5,
+        fitness_limit=1,
         max_generations=100,
         min_improvement=0.001,
         min_count=1
     )
 
     driver = Driver(
         definition=deriver_definition,
```

