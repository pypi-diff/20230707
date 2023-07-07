# Comparing `tmp/signe-0.1.4.tar.gz` & `tmp/signe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.4.tar", last modified: Fri Jul  7 10:36:52 2023, max compression
+gzip compressed data, was "signe-0.1.5.tar", last modified: Fri Jul  7 13:35:33 2023, max compression
```

## Comparing `signe-0.1.4.tar` & `signe-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.850564 signe-0.1.4/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      469 2023-07-07 10:36:52.849566 signe-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 10:36:52.851561 signe-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.811675 signe-0.1.4/signe/
--rw-rw-rw-   0        0        0      164 2023-07-07 10:36:39.000000 signe-0.1.4/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.844579 signe-0.1.4/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.4/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/consts.py
--rw-rw-rw-   0        0        0     4518 2023-07-07 10:35:17.000000 signe-0.1.4/signe/core/effect.py
--rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.847573 signe-0.1.4/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.4/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.4/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.4/signe/types.py
--rw-rw-rw-   0        0        0     3358 2023-07-07 10:35:17.000000 signe-0.1.4/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.821650 signe-0.1.4/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.173878 signe-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-07 13:35:33.171883 signe-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:35:33.173878 signe-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.146950 signe-0.1.5/signe/
+-rw-rw-rw-   0        0        0      164 2023-07-07 13:35:16.000000 signe-0.1.5/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.166896 signe-0.1.5/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.5/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/consts.py
+-rw-rw-rw-   0        0        0     5778 2023-07-07 13:26:40.000000 signe-0.1.5/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.5/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.170885 signe-0.1.5/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.5/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.5/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.5/signe/types.py
+-rw-rw-rw-   0        0        0     3355 2023-07-07 13:26:40.000000 signe-0.1.5/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:33.156924 signe-0.1.5/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-07 13:35:33.000000 signe-0.1.5/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.4/LICENSE` & `signe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/README.md` & `signe-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/setup.py` & `signe-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/signe/core/collections.py` & `signe-0.1.5/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/signe/core/effect.py` & `signe-0.1.5/signe/core/effect.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, TypeVar, Set, Callable, Optional, Generic
+from typing import TYPE_CHECKING, Any, TypeVar, Set, Callable, Optional, Generic, cast
 from .consts import EffectState
+from itertools import chain
 
 if TYPE_CHECKING:
     from .runtime import Executor
     from .signal import Signal
 
 T = TypeVar("T")
 
@@ -27,62 +28,100 @@
         self.id = Effect._g_id
         self.__executor = executor
         self.value: Optional[T] = None
         self.fn = fn
         self._age = 0
         self._state = EffectState.CURRENT
         self.__dep_signals: Set[Signal] = set()
-        self.__dep_effects: Set[Effect] = set()
+
+        """
+        When one effect is triggered by another effect, 
+        the former belongs to a pre dependency 
+        and the latter belongs to a next dependency.
+
+        @effect
+        def a():
+            return 1
+
+        @effect
+        def b():
+            return a()
+
+        a is pre dep effect
+        b is next dep effect
+
+        b should be push to next dep of a
+        a should be push to pre dep of b
+        """
+        self.__pre_dep_effects: Set[Effect] = set()
+        self.__next_dep_effects: Set[Effect] = set()
+
         self._sub_effects: list[Effect] = []
 
         self._cleanup_callbacks: list[Callable] = []
 
         self._debug_trigger = debug_trigger
 
         self.__run_fn()
-        self.__init_no_deps = (len(self.__dep_effects) + len(self.__dep_signals)) <= 0
+        self.__init_no_deps = (
+            len(self.__pre_dep_effects)
+            + len(self.__next_dep_effects)
+            + len(self.__dep_signals)
+        ) <= 0
+
+    def __get_all_dep_effects(self):
+        return chain(self.__pre_dep_effects, self.__next_dep_effects)
+
+    def _get_pre_dep_effects(self):
+        return list(self.__pre_dep_effects)
+
+    def _get_next_dep_effects(self):
+        return list(self.__next_dep_effects)
 
     def _add_sub_effect(self, effect: Effect):
         self._sub_effects.append(effect)
 
     def add_dep_signal(self, signal: Signal):
         self.__dep_signals.add(signal)
 
-    def add_dep_effect(self, effect: Effect):
-        self.__dep_effects.add(effect)
+    def add_pre_dep_effect(self, effect: Effect):
+        self.__pre_dep_effects.add(effect)
+
+    def add_next_dep_effect(self, effect: Effect):
+        self.__next_dep_effects.add(effect)
 
     def getValue(self):
         if not self.__init_no_deps:
             tick = self.__executor.current_execution_scheduler.tick
             current_effect = self.__executor.effect_running_stack.get_current()
 
             if current_effect:
                 if self._age == tick:
                     if self._state == EffectState.RUNNING:
                         raise Exception("circular running")
 
                     self.update()
 
-                self.__dep_effects.add(current_effect)
-                current_effect.add_dep_effect(self)
+                self.add_next_dep_effect(current_effect)
+                current_effect.add_pre_dep_effect(self)
 
-        return self.value
+        return cast(T, self.value)
 
     def _push_scheduler(self):
         tick = self.__executor.current_execution_scheduler.tick
 
         if self._age >= tick:
             return
 
         self._age = tick
         self._state = EffectState.STALE
 
         self.__executor.current_execution_scheduler.add_effect(self)
 
-        for effect in self.__dep_effects:
+        for effect in self.__get_all_dep_effects():
             effect._push_scheduler()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.getValue()
 
     def update(self):
         if self._state != EffectState.STALE:
@@ -114,26 +153,31 @@
 
             self._state = EffectState.CURRENT
 
         finally:
             self.__executor.effect_running_stack.reset_current()
 
     def cleanup_dep_effect(self, effect: Effect):
-        self.__dep_effects.remove(effect)
+        if effect in self.__pre_dep_effects:
+            self.__pre_dep_effects.remove(effect)
+
+        if effect in self.__next_dep_effects:
+            self.__next_dep_effects.remove(effect)
 
     def cleanup_deps(self):
         for s in self.__dep_signals:
             s.cleanup_dep_effect(self)
 
         self.__dep_signals.clear()
 
-        for effect in self.__dep_effects:
+        for effect in self.__get_all_dep_effects():
             effect.cleanup_dep_effect(self)
 
-        self.__dep_effects.clear()
+        self.__pre_dep_effects.clear()
+        self.__next_dep_effects.clear()
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, self.__class__):
             return self.__hash__() == __value.__hash__()
```

### Comparing `signe-0.1.4/signe/core/runtime.py` & `signe-0.1.5/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/signe/core/signal.py` & `signe-0.1.5/signe/core/signal.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/signe/reactive/proxy.py` & `signe-0.1.5/signe/reactive/proxy.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.4/signe/utils.py` & `signe-0.1.5/signe/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def createSignal(value: T, comp: TSignalOptionInitComp[T] = None):
     s = Signal(exec, value, SignalOption(comp))
 
     return s.getValue, s.setValue
 
 
-def effect(fn: Callable[[], None]):
+def effect(fn: Callable[[], T]):
     return Effect(exec, fn)
 
 
 class computed(Generic[T]):
     def __init__(
         self, fn: Callable[[], T], debug_trigger: Optional[Callable] = None
     ) -> None:
```

