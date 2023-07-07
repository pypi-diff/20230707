# Comparing `tmp/signe-0.1.3.tar.gz` & `tmp/signe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.3.tar", last modified: Thu Jul  6 05:26:27 2023, max compression
+gzip compressed data, was "signe-0.1.4.tar", last modified: Fri Jul  7 10:36:52 2023, max compression
```

## Comparing `signe-0.1.3.tar` & `signe-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.996710 signe-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      469 2023-07-06 05:26:26.995712 signe-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 05:26:26.997229 signe-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.969414 signe-0.1.3/signe/
--rw-rw-rw-   0        0        0      164 2023-07-06 05:26:07.000000 signe-0.1.3/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.989725 signe-0.1.3/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.3/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/consts.py
--rw-rw-rw-   0        0        0     4309 2023-06-26 14:25:04.000000 signe-0.1.3/signe/core/effect.py
--rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.993719 signe-0.1.3/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.3/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.3/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.3/signe/types.py
--rw-rw-rw-   0        0        0     3062 2023-07-06 05:25:51.000000 signe-0.1.3/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.978713 signe-0.1.3/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.850564 signe-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-07 10:36:52.849566 signe-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:36:52.851561 signe-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.811675 signe-0.1.4/signe/
+-rw-rw-rw-   0        0        0      164 2023-07-07 10:36:39.000000 signe-0.1.4/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.844579 signe-0.1.4/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.4/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/consts.py
+-rw-rw-rw-   0        0        0     4518 2023-07-07 10:35:17.000000 signe-0.1.4/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.4/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.847573 signe-0.1.4/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.4/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.4/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.4/signe/types.py
+-rw-rw-rw-   0        0        0     3358 2023-07-07 10:35:17.000000 signe-0.1.4/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:36:52.821650 signe-0.1.4/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-07 10:36:52.000000 signe-0.1.4/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.3/LICENSE` & `signe-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/README.md` & `signe-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/setup.py` & `signe-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/signe/core/collections.py` & `signe-0.1.4/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/signe/core/effect.py` & `signe-0.1.4/signe/core/effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,35 @@
     def __init__(self, level=0) -> None:
         self.level = level
 
 
 class Effect(Generic[T]):
     _g_id = 0
 
-    def __init__(self, executor: Executor, fn: Callable[[], T]) -> None:
+    def __init__(
+        self,
+        executor: Executor,
+        fn: Callable[[], T],
+        debug_trigger: Optional[Callable] = None,
+    ) -> None:
         Effect._g_id += 1
         self.id = Effect._g_id
         self.__executor = executor
         self.value: Optional[T] = None
         self.fn = fn
         self._age = 0
         self._state = EffectState.CURRENT
         self.__dep_signals: Set[Signal] = set()
         self.__dep_effects: Set[Effect] = set()
         self._sub_effects: list[Effect] = []
 
         self._cleanup_callbacks: list[Callable] = []
 
+        self._debug_trigger = debug_trigger
+
         self.__run_fn()
         self.__init_no_deps = (len(self.__dep_effects) + len(self.__dep_signals)) <= 0
 
     def _add_sub_effect(self, effect: Effect):
         self._sub_effects.append(effect)
 
     def add_dep_signal(self, signal: Signal):
@@ -98,14 +105,16 @@
             self.__executor.effect_running_stack.set_current(self)
 
             self._state = EffectState.RUNNING
 
             self.cleanup_deps()
 
             self.value = self.fn()
+            if self._debug_trigger:
+                self._debug_trigger()
 
             self._state = EffectState.CURRENT
 
         finally:
             self.__executor.effect_running_stack.reset_current()
 
     def cleanup_dep_effect(self, effect: Effect):
```

### Comparing `signe-0.1.3/signe/core/runtime.py` & `signe-0.1.4/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/signe/core/signal.py` & `signe-0.1.4/signe/core/signal.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/signe/reactive/proxy.py` & `signe-0.1.4/signe/reactive/proxy.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.3/signe/utils.py` & `signe-0.1.4/signe/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,35 @@
 
 
 def effect(fn: Callable[[], None]):
     return Effect(exec, fn)
 
 
 class computed(Generic[T]):
-    def __init__(self, fn: Callable[[], T]) -> None:
+    def __init__(
+        self, fn: Callable[[], T], debug_trigger: Optional[Callable] = None
+    ) -> None:
         self.fn = fn
 
         def getter():
-            effect = Effect(exec, fn)
+            effect = Effect(exec, fn, debug_trigger)
             self.getter = effect
             return effect.getValue()
 
         self.getter = getter
 
+    @staticmethod
+    def debug_trigger(debug_trigger: Optional[Callable] = None):
+        def warp(
+            fn: Callable[[], T],
+        ):
+            return computed(fn, debug_trigger)
+
+        return warp
+
     def __call__(self, *args: Any, **kwds: Any) -> T:
         return self.getter()  # type: ignore
 
 
 def batch(fn: Callable[[], None]):
     if isinstance(exec.current_execution_scheduler, BatchExecutionScheduler):
         fn()
```

