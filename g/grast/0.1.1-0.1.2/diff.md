# Comparing `tmp/grast-0.1.1.tar.gz` & `tmp/grast-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grast-0.1.1.tar", max compression
+gzip compressed data, was "grast-0.1.2.tar", max compression
```

## Comparing `grast-0.1.1.tar` & `grast-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-06-21 18:51:11.258738 grast-0.1.1/LICENSE
--rw-r--r--   0        0        0     1085 2023-07-06 23:22:25.846685 grast-0.1.1/README.md
--rw-r--r--   0        0        0      251 2023-07-06 17:37:36.352013 grast-0.1.1/grast/__init__.py
--rw-r--r--   0        0        0      670 2023-07-06 20:53:48.549457 grast-0.1.1/grast/cfg.py
--rw-r--r--   0        0        0       61 2023-06-27 14:58:24.953384 grast-0.1.1/grast/delta/__init__.py
--rw-r--r--   0        0        0     1455 2023-06-28 16:17:40.542993 grast-0.1.1/grast/delta/algebra.py
--rw-r--r--   0        0        0     1457 2023-07-06 16:06:53.066349 grast-0.1.1/grast/delta/delta.py
--rw-r--r--   0        0        0     3802 2023-07-06 21:06:38.305396 grast-0.1.1/grast/dual.py
--rw-r--r--   0        0        0     1761 2023-07-06 20:54:30.529316 grast-0.1.1/grast/forward.py
--rw-r--r--   0        0        0     1931 2023-07-06 18:08:44.604282 grast-0.1.1/grast/grad.py
--rw-r--r--   0        0        0        0 2023-07-06 22:22:43.359015 grast-0.1.1/grast/py.typed
--rw-r--r--   0        0        0      104 2023-06-27 17:20:32.718485 grast-0.1.1/grast/real/__init__.py
--rw-r--r--   0        0        0     2508 2023-07-06 21:06:38.302824 grast-0.1.1/grast/real/algebra.py
--rw-r--r--   0        0        0      205 2023-07-06 16:06:53.066615 grast-0.1.1/grast/real/binary.py
--rw-r--r--   0        0        0     1794 2023-07-06 21:06:38.291252 grast-0.1.1/grast/real/real.py
--rw-r--r--   0        0        0      300 2023-07-06 20:52:52.224748 grast-0.1.1/grast/real/unary.py
--rw-r--r--   0        0        0       40 2023-06-27 14:57:38.125311 grast-0.1.1/grast/utils/__init__.py
--rw-r--r--   0        0        0      268 2023-07-06 17:06:45.598423 grast-0.1.1/grast/utils/to_string/__init__.py
--rw-r--r--   0        0        0     1012 2023-07-06 17:05:01.049867 grast-0.1.1/grast/utils/to_string/delta_str.py
--rw-r--r--   0        0        0     1910 2023-07-06 17:09:50.774859 grast-0.1.1/grast/utils/to_string/real_str.py
--rw-r--r--   0        0        0     1146 2023-07-06 17:10:35.634522 grast-0.1.1/grast/utils/to_string/utils.py
--rw-r--r--   0        0        0      385 2023-07-06 22:20:17.933124 grast-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 grast-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-21 18:51:11.258738 grast-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1167 2023-07-07 05:13:14.466735 grast-0.1.2/README.md
+-rw-r--r--   0        0        0      251 2023-07-06 17:37:36.352013 grast-0.1.2/grast/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-06 20:53:48.549457 grast-0.1.2/grast/cfg.py
+-rw-r--r--   0        0        0       61 2023-06-27 14:58:24.953384 grast-0.1.2/grast/delta/__init__.py
+-rw-r--r--   0        0        0     1455 2023-06-28 16:17:40.542993 grast-0.1.2/grast/delta/algebra.py
+-rw-r--r--   0        0        0     1457 2023-07-06 16:06:53.066349 grast-0.1.2/grast/delta/delta.py
+-rw-r--r--   0        0        0     3915 2023-07-07 05:10:47.050835 grast-0.1.2/grast/dual.py
+-rw-r--r--   0        0        0     1761 2023-07-06 20:54:30.529316 grast-0.1.2/grast/forward.py
+-rw-r--r--   0        0        0     1931 2023-07-06 18:08:44.604282 grast-0.1.2/grast/grad.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:22:43.359015 grast-0.1.2/grast/py.typed
+-rw-r--r--   0        0        0      104 2023-06-27 17:20:32.718485 grast-0.1.2/grast/real/__init__.py
+-rw-r--r--   0        0        0     2508 2023-07-06 21:06:38.302824 grast-0.1.2/grast/real/algebra.py
+-rw-r--r--   0        0        0      205 2023-07-06 16:06:53.066615 grast-0.1.2/grast/real/binary.py
+-rw-r--r--   0        0        0     1794 2023-07-06 21:06:38.291252 grast-0.1.2/grast/real/real.py
+-rw-r--r--   0        0        0      300 2023-07-06 20:52:52.224748 grast-0.1.2/grast/real/unary.py
+-rw-r--r--   0        0        0       40 2023-06-27 14:57:38.125311 grast-0.1.2/grast/utils/__init__.py
+-rw-r--r--   0        0        0      268 2023-07-06 17:06:45.598423 grast-0.1.2/grast/utils/to_string/__init__.py
+-rw-r--r--   0        0        0     1012 2023-07-06 17:05:01.049867 grast-0.1.2/grast/utils/to_string/delta_str.py
+-rw-r--r--   0        0        0     1910 2023-07-06 17:09:50.774859 grast-0.1.2/grast/utils/to_string/real_str.py
+-rw-r--r--   0        0        0     1146 2023-07-06 17:10:35.634522 grast-0.1.2/grast/utils/to_string/utils.py
+-rw-r--r--   0        0        0      503 2023-07-07 05:12:06.395381 grast-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 grast-0.1.2/PKG-INFO
```

### Comparing `grast-0.1.1/LICENSE` & `grast-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/README.md` & `grast-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # grast
 
-Automatic differentiation of generic fields for Python
+Lazy automatic differentiation for Python
 
 ## Install
 
+Requires python >= 3.10
+
 ```sh
 pip install grast
 ```
 
 ## Usage
 
 Create function R^n -> R
 ```py
 from grast import var
 
 x = var('x')
 y = var('y')
+z = var('z').freeze()  # do not compute derivative
 
-f = x/y + y**x
+h = x/y + y**x
+f = z * h + 3
 ```
 
 Get gradient
 ```py
 df = f.grad()
 df_dx = df['x']
 df_dy = df['y']
 ```
 
 Evaluate with specific arguments
 ```py
-args = dict(x=-3, y=5)
+args = dict(x=-3, y=5, z=2)
 f(args)
 df_dx(args)
 df_dy(args)
 ```
 
 View in symbolic format
 ```py
```

### Comparing `grast-0.1.1/grast/cfg.py` & `grast-0.1.2/grast/cfg.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/delta/algebra.py` & `grast-0.1.2/grast/delta/algebra.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/delta/delta.py` & `grast-0.1.2/grast/delta/delta.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/dual.py` & `grast-0.1.2/grast/dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         self,
         args: Args[T] | None = None,
         cfg: Cfg[T] | None = None,
     ) -> Args[T]:
         grad = self.grad()
         return {k: v(args, cfg=cfg) for k, v in grad.items()}
 
+    def freeze(self) -> Dual[T]:
+        return Dual(self.real, Zero())
+
     def __str__(self) -> str:
         return str(self.real)
 
     def __add__(self, other: Dual[T] | T) -> Dual[T]:
         other = wrap(other)
         a, b = self.tup
         c, d = other.tup
@@ -139,17 +142,17 @@
 
 def wrap(val: Dual[T] | T) -> Dual[T]:
     if isinstance(val, Dual):
         return val
     return const(val)
 
 
-def var(key: str) -> Dual[T]:
-    real: re.Var[T] = re.Var(key=key)
-    delta: OneHot[T] = OneHot(var=real)
+def var(key: str, requires_grad: bool = True) -> Dual:
+    real: re.Var = re.Var(key=key)
+    delta = OneHot(var=real) if requires_grad else Zero()
     return Dual(real, delta)
 
 
 def const(val: T) -> Dual[T]:
     real = re.Const(val=val)
     delta = Zero()
     return Dual(real, delta)
```

### Comparing `grast-0.1.1/grast/forward.py` & `grast-0.1.2/grast/forward.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/grad.py` & `grast-0.1.2/grast/grad.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/real/algebra.py` & `grast-0.1.2/grast/real/algebra.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/real/real.py` & `grast-0.1.2/grast/real/real.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/utils/to_string/delta_str.py` & `grast-0.1.2/grast/utils/to_string/delta_str.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/utils/to_string/real_str.py` & `grast-0.1.2/grast/utils/to_string/real_str.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/grast/utils/to_string/utils.py` & `grast-0.1.2/grast/utils/to_string/utils.py`

 * *Files identical despite different names*

### Comparing `grast-0.1.1/PKG-INFO` & `grast-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 Metadata-Version: 2.1
 Name: grast
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Lazy automatic differentiation for Python
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # grast
 
-Automatic differentiation of generic fields for Python
+Lazy automatic differentiation for Python
 
 ## Install
 
+Requires python >= 3.10
+
 ```sh
 pip install grast
 ```
 
 ## Usage
 
 Create function R^n -> R
 ```py
 from grast import var
 
 x = var('x')
 y = var('y')
+z = var('z').freeze()  # do not compute derivative
 
-f = x/y + y**x
+h = x/y + y**x
+f = z * h + 3
 ```
 
 Get gradient
 ```py
 df = f.grad()
 df_dx = df['x']
 df_dy = df['y']
 ```
 
 Evaluate with specific arguments
 ```py
-args = dict(x=-3, y=5)
+args = dict(x=-3, y=5, z=2)
 f(args)
 df_dx(args)
 df_dy(args)
 ```
 
 View in symbolic format
 ```py
```

