# Comparing `tmp/NumFmt-0.0.0.post0.tar.gz` & `tmp/NumFmt-0.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NumFmt-0.0.0.post0.tar", last modified: Thu Jul  6 16:28:22 2023, max compression
+gzip compressed data, was "NumFmt-0.0.0.post1.tar", last modified: Fri Jul  7 15:02:16 2023, max compression
```

## Comparing `NumFmt-0.0.0.post0.tar` & `NumFmt-0.0.0.post1.tar`

### file list

```diff
@@ -1,35 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.202747 NumFmt-0.0.0.post0/
--rw-rw-rw-   0        0        0    17098 2023-02-03 14:53:10.000000 NumFmt-0.0.0.post0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.171740 NumFmt-0.0.0.post0/NumFmt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-07-06 16:28:22.000000 NumFmt-0.0.0.post0/NumFmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-07-06 16:28:22.000000 NumFmt-0.0.0.post0/NumFmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:28:22.000000 NumFmt-0.0.0.post0/NumFmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 16:28:22.000000 NumFmt-0.0.0.post0/NumFmt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2055 2023-07-06 16:28:22.202747 NumFmt-0.0.0.post0/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-07-06 16:26:31.000000 NumFmt-0.0.0.post0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.174741 NumFmt-0.0.0.post0/numfmt/
--rw-rw-rw-   0        0        0       25 2023-06-30 06:43:44.000000 NumFmt-0.0.0.post0/numfmt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.180741 NumFmt-0.0.0.post0/numfmt/intstr/
--rw-rw-rw-   0        0        0       34 2023-06-30 06:43:44.000000 NumFmt-0.0.0.post0/numfmt/intstr/__init__.py
--rw-rw-rw-   0        0        0     3313 2023-06-28 05:26:36.000000 NumFmt-0.0.0.post0/numfmt/intstr/math.py
--rw-rw-rw-   0        0        0     1276 2023-07-02 13:45:42.000000 NumFmt-0.0.0.post0/numfmt/intstr/standard.py
--rw-rw-rw-   0        0        0     1074 2023-06-28 11:26:37.000000 NumFmt-0.0.0.post0/numfmt/intstr/utils.py
--rw-rw-rw-   0        0        0      780 2023-06-22 15:42:36.000000 NumFmt-0.0.0.post0/numfmt/map.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.189746 NumFmt-0.0.0.post0/numfmt/scistr/
--rw-rw-rw-   0        0        0       70 2023-07-02 13:49:11.000000 NumFmt-0.0.0.post0/numfmt/scistr/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-07-02 13:45:42.000000 NumFmt-0.0.0.post0/numfmt/scistr/calc.py
--rw-rw-rw-   0        0        0      479 2023-07-02 13:41:12.000000 NumFmt-0.0.0.post0/numfmt/scistr/fracs.py
--rw-rw-rw-   0        0        0     3427 2023-07-02 13:41:12.000000 NumFmt-0.0.0.post0/numfmt/scistr/ieee754.py
--rw-rw-rw-   0        0        0      382 2023-07-02 13:48:57.000000 NumFmt-0.0.0.post0/numfmt/scistr/standard.py
--rw-rw-rw-   0        0        0      251 2023-07-02 13:45:42.000000 NumFmt-0.0.0.post0/numfmt/scistr/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:28:22.200748 NumFmt-0.0.0.post0/numfmt/utils/
--rw-rw-rw-   0        0        0     1074 2023-07-02 13:28:28.000000 NumFmt-0.0.0.post0/numfmt/utils/__init__.py
--rw-rw-rw-   0        0        0     4575 2023-02-13 20:23:34.000000 NumFmt-0.0.0.post0/numfmt/utils/bitwise.py
--rw-rw-rw-   0        0        0      555 2022-12-23 05:08:06.000000 NumFmt-0.0.0.post0/numfmt/utils/floatwise.py
--rw-rw-rw-   0        0        0        0 2023-07-02 13:46:47.000000 NumFmt-0.0.0.post0/numfmt/utils/ftools.py
--rw-rw-rw-   0        0        0     3102 2022-09-15 09:41:56.000000 NumFmt-0.0.0.post0/numfmt/utils/int.py
--rw-rw-rw-   0        0        0     6588 2022-09-15 13:39:20.000000 NumFmt-0.0.0.post0/numfmt/utils/int_str.py
--rw-rw-rw-   0        0        0     3310 2023-06-28 23:48:33.000000 NumFmt-0.0.0.post0/numfmt/utils/intwise.py
--rw-rw-rw-   0        0        0        0 2023-07-02 13:46:42.000000 NumFmt-0.0.0.post0/numfmt/utils/itools.py
--rw-rw-rw-   0        0        0       42 2023-07-06 16:28:22.203746 NumFmt-0.0.0.post0/setup.cfg
--rw-rw-rw-   0        0        0     1849 2023-07-06 16:28:11.000000 NumFmt-0.0.0.post0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.061273 NumFmt-0.0.0.post1/
+-rw-rw-rw-   0        0        0    17098 2023-02-03 14:53:10.000000 NumFmt-0.0.0.post1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.031179 NumFmt-0.0.0.post1/NumFmt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-07-07 15:02:15.000000 NumFmt-0.0.0.post1/NumFmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-07 15:02:15.000000 NumFmt-0.0.0.post1/NumFmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:02:15.000000 NumFmt-0.0.0.post1/NumFmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 15:02:15.000000 NumFmt-0.0.0.post1/NumFmt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2055 2023-07-07 15:02:16.060273 NumFmt-0.0.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-07-06 16:26:31.000000 NumFmt-0.0.0.post1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.035180 NumFmt-0.0.0.post1/numfmt/
+-rw-rw-rw-   0        0        0       25 2023-06-30 06:43:44.000000 NumFmt-0.0.0.post1/numfmt/__init__.py
+-rw-rw-rw-   0        0        0      922 2023-07-07 14:07:39.000000 NumFmt-0.0.0.post1/numfmt/charmaps.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.039180 NumFmt-0.0.0.post1/numfmt/intstr/
+-rw-rw-rw-   0        0        0      270 2023-07-07 14:55:15.000000 NumFmt-0.0.0.post1/numfmt/intstr/__init__.py
+-rw-rw-rw-   0        0        0     3511 2023-07-07 14:55:15.000000 NumFmt-0.0.0.post1/numfmt/intstr/calc.py
+-rw-rw-rw-   0        0        0     1385 2023-07-07 14:32:21.000000 NumFmt-0.0.0.post1/numfmt/intstr/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.055273 NumFmt-0.0.0.post1/numfmt/scistr/
+-rw-rw-rw-   0        0        0      171 2023-07-07 14:39:18.000000 NumFmt-0.0.0.post1/numfmt/scistr/__init__.py
+-rw-rw-rw-   0        0        0     2691 2023-07-07 14:35:01.000000 NumFmt-0.0.0.post1/numfmt/scistr/calc.py
+-rw-rw-rw-   0        0        0      479 2023-07-02 13:41:12.000000 NumFmt-0.0.0.post1/numfmt/scistr/fracs.py
+-rw-rw-rw-   0        0        0     3428 2023-07-07 14:35:01.000000 NumFmt-0.0.0.post1/numfmt/scistr/ieee754.py
+-rw-rw-rw-   0        0        0      378 2023-07-07 14:35:01.000000 NumFmt-0.0.0.post1/numfmt/scistr/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:02:16.059273 NumFmt-0.0.0.post1/numfmt/utils/
+-rw-rw-rw-   0        0        0      549 2023-07-07 14:19:47.000000 NumFmt-0.0.0.post1/numfmt/utils/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-07-07 14:19:47.000000 NumFmt-0.0.0.post1/numfmt/utils/ftools.py
+-rw-rw-rw-   0        0        0     1107 2023-07-07 14:37:09.000000 NumFmt-0.0.0.post1/numfmt/utils/itools.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:02:16.061273 NumFmt-0.0.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1849 2023-07-07 15:02:07.000000 NumFmt-0.0.0.post1/setup.py
```

### Comparing `NumFmt-0.0.0.post0/LICENSE` & `NumFmt-0.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `NumFmt-0.0.0.post0/NumFmt.egg-info/PKG-INFO` & `NumFmt-0.0.0.post1/NumFmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumFmt
-Version: 0.0.0.post0
+Version: 0.0.0.post1
 Summary: Format Numbers in Any Base and Charset
 Home-page: https://github.com/technikker/numfmt
 Author: technician
 Author-email: <mail@xxxxxxxx.com>
 License: MPL
 Project-URL: Source, https://github.com/technikker/numfmt
 Keywords: python,NumFmt,numfmt,number,format,formatter
```

### Comparing `NumFmt-0.0.0.post0/PKG-INFO` & `NumFmt-0.0.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NumFmt
-Version: 0.0.0.post0
+Version: 0.0.0.post1
 Summary: Format Numbers in Any Base and Charset
 Home-page: https://github.com/technikker/numfmt
 Author: technician
 Author-email: <mail@xxxxxxxx.com>
 License: MPL
 Project-URL: Source, https://github.com/technikker/numfmt
 Keywords: python,NumFmt,numfmt,number,format,formatter
```

### Comparing `NumFmt-0.0.0.post0/README.rst` & `NumFmt-0.0.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `NumFmt-0.0.0.post0/numfmt/intstr/math.py` & `NumFmt-0.0.0.post1/numfmt/intstr/calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import typing as _tp
-from .utils import *
+from itertools import accumulate
+from ..utils.itools import concat, last  # need this as a utility function for importers
+from ..utils import exponential, conditional_negate
+
+
+T = _tp.TypeVar('T')
+I = _tp.TypeVar('I')
+S = _tp.TypeVar('S')
 
 
 DIGITS_1_R = _tp.Tuple[bool, _tp.Iterable[I]]
 DIGITS_0_R = _tp.Callable[[I, ], DIGITS_1_R]
 
 
 # You can extend your answer to include base 1. if b == 1: return n * [1]
@@ -79,65 +86,63 @@
 
 
 def number_le(
 		base: int = 10,
 ) -> NUMBER_0_R:
 	def f(_sign: NUMBER_1_0, _digits: NUMBER_1_1) -> I:
 		"""digits are passed in big endian order"""
-		sign = -bool(_sign) | 1  # either 1 or -1
 		div = 0
-		for pos, mod in zip(exp(base), _digits):
+		for pos, mod in zip(exponential(base), _digits):
 			# div += mod * (base ** i)  # reverse divmod
 			div += mod * pos  # reverse divmod
-		return div * sign
+			yield conditional_negate(_sign, div)
 
 	return f
 
 
 def number_le_comp(
 		base: int = 10,
 ) -> NUMBER_0_R:
 	"""base complimented"""
 	def f(_sign: NUMBER_1_0, _digits: NUMBER_1_1) -> I:
 		"""digits are passed in little endian order"""
-		return sum(
+		return accumulate(
 			mod * pos
 			for pos, mod in zip(
-				exp(base),
+				exponential(base),
 				concat(_digits, (-bool(_sign), )),
 			)
 		)
 
 	return f
 
 
 def number_be(
 		base: int = 10,
 ) -> NUMBER_0_R:
 	def f(_sign: NUMBER_1_0, _digits: NUMBER_1_1) -> I:
 		"""digits are passed in big endian order"""
-		sign = -bool(_sign) | 1  # either 1 or -1
 		div = 0
 		for mod in _digits:
 			div = base * div + mod  # reverse divmod
-		return div * sign
+			yield conditional_negate(_sign, div)
 
 	return f
 
 
 def number_be_comp(
 		base: int = 10,
 ) -> NUMBER_0_R:
 	"""base complimented"""
 	def f(_sign: NUMBER_1_0, _digits: NUMBER_1_1) -> I:
 		"""digits are passed in big endian order"""
 		div = -bool(_sign)
 		for mod in _digits:
 			div = base * div + mod  # reverse divmod
-		return div
+			yield div
 
 	return f
 
 
 def digits(
 		base: int = 10,
 		endian: int = False,
```

### Comparing `NumFmt-0.0.0.post0/numfmt/intstr/standard.py` & `NumFmt-0.0.0.post1/numfmt/intstr/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import typing as _tp
-from enum import Enum
 from itertools import islice
-from .utils import *
-from .math import *
-from ..map import *
+from ..utils.itools import concat, ireversed
+from ..charmaps import Charsets, DEFAULT_SIGNS
+from .calc import digits_le
+
+
+T = _tp.TypeVar('T')
+I = _tp.TypeVar('I')
+S = _tp.TypeVar('S')
 
 
 def pad_back(
 		padding: int = 1
 ):
-	def f(seq):
-		return tuple(concat(seq, (0 for _ in range(padding - len(seq)))))
+	# def f(seq):
+	# 	return tuple(concat(seq, (0 for _ in range(padding - len(seq)))))
 
 	def g(it):
 		i = 0
 		for i, x in enumerate(it, 1):
 			yield x
 		yield from (0 for _ in range(padding - i))
 
@@ -57,15 +61,15 @@
 	def encode(x: int) -> str:
 		neg, digs = _digits(x)
 		return "".join(
 			concat(
 				signs[neg][0],
 				map(
 					charset.__getitem__,
-					ireversed2(islice(_pad_back(digs), limit)),
+					ireversed(islice(_pad_back(digs), limit)),
 				),
 			)
 		)
 
 	return encode
```

### Comparing `NumFmt-0.0.0.post0/numfmt/intstr/utils.py` & `NumFmt-0.0.0.post1/numfmt/utils/itools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 import typing as _tp
+from itertools import tee
 
 
 T = _tp.TypeVar('T')
 I = _tp.TypeVar('I')
 S = _tp.TypeVar('S')
 
 
-# todo some of these fns can be i[ter]tools2?
 def concat(*its: _tp.Iterable[T]) -> _tp.Generator[T, None, None]:
 	"""joins iterables together"""
 	for it in its:
 		yield from it
 
 
-def ireversed(it: _tp.Iterable[T]) -> _tp.List[T]:
-	"""reverses an iterable that does not implement 'reversed'
-	doesn't work on infinite iterables"""
-	r = []
-	for x in it:
-		r.insert(0, x)
-	return r
+def strcat(it):
+	return "".join(it)
 
 
-def ireversed2(it: _tp.Iterable[T]) -> _tp.Iterable[T]:
+def ireversed(it: _tp.Iterable[T]) -> _tp.Iterable[T]:
 	"""reverses an iterable that does not implement 'reversed'
 	doesn't work on infinite iterables"""
 	return reversed(tuple(it))
 
 
-def first(it):
-	return next(iter(it))
-
-
-def strcat(it):
-	return "".join(it)
-
+def ireversed2(it: _tp.Iterable[T]) -> _tp.List[T]:
+	"""reverses an iterable that does not implement 'reversed'
+	doesn't work on infinite iterables"""
+	r = []
+	for x in it:
+		r.insert(0, x)
+	return r
 
-def chars(start: str, length: int) -> _tp.Sequence[str]:
-	start = ord(start)
-	return tuple((chr(i) for i in range(start, start + length)))
 
+def first(it, default=None):
+	return next(iter(it), default)
 
-def exp(base, start=1):
-	p = start
-	while True:
-		yield p
-		p *= base
 
+def last(it, default=None):
+	r = default
+	for r in it:
+		pass
+	return r
 
-def undivmod(base):
-	def f(div, mod):
-		return base * div + mod
 
-	return f
+# try to import from itertools, if this fails, define here
+try:
+	from itertools import pairwise
+except ImportError:
+	def pairwise(iterable):
+		# pairwise('ABCDEFG') --> AB BC CD DE EF FG
+		a, b = tee(iterable)
+		next(b, None)
+		return zip(a, b)
```

### Comparing `NumFmt-0.0.0.post0/numfmt/scistr/calc.py` & `NumFmt-0.0.0.post1/numfmt/scistr/calc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import typing as _tp
+# import typing as _tp
 import itertools
 import math
-from .. import utils
+from ..intstr.calc import digits_be, number_be
+from ..utils.itools import strcat
+from ..utils import exponential
 from . import fracs
-from . import ieee754
-from ..intstr import math as intstr_math
 
 
 def sci_exp(base: int, x: float):
 	x = abs(x)
 	if x < 1:
 		if x == 0.0:
 			e = 0
@@ -43,43 +43,42 @@
 	yield div
 	while mod:
 		mod *= base
 		div, mod = divmod(mod, b)
 		yield div
 
 
-# todo should intstr be redone to work like this?
-def number_be(
+def number_be2(
 		base: int = 10,
 ):
 	def f(_digits):
 		"""digits are passed in big endian order"""
 		div = 0
 		for mod in _digits:
 			div = base * div + mod  # reverse divmod
 			yield div
 
 	return f
 
 
 def frac2(base, digits):
 	return zip(
-		number_be(base)(digits),
-		utils.exp(base),
+		number_be2(base)(digits),
+		exponential(base),
 	)
 
 
 def digits_frac(base: int):
 
 	def f(frac_digits, exp_digits) -> tuple:
 		sign, frac_digits = frac_digits
 		frac_digits = tuple(frac_digits)
 		# frac_max = base ** (len(frac_digits) - 1)
 		# frac_numerator = intstr.math.number_be(base)(sign, frac_digits)
-		exp = intstr_math.number_be(base)(*exp_digits)
+		exp = number_be(base)(*exp_digits)
 
 		# convert to fraction
 		frac = tuple(frac2(base, frac_digits))[-1]
 		frac = fracs.exp(frac, base, exp)
 
 		return sign, frac
 
@@ -98,15 +97,15 @@
 
 
 def sci_digits(base: int, figures: int = 6):
 
 	def f(sign, frac, exp):
 		# convert rebased fraction into str
 		frac_digits = (itertools.islice(sci_div(base, *frac), figures))
-		exp_digits = intstr_math.digits_be(base)(exp)
+		exp_digits = digits_be(base)(exp)
 		return (sign, frac_digits), exp_digits
 
 	return f
 
 
 def sci_str(base: int = None):
 	zero = str(0)
@@ -118,14 +117,14 @@
 		f_sign, f_digits = frac_digits
 		e_sign, e_digits = exp_digits
 
 		f_digits = iter(f_digits)
 		fs = signs[f_sign]
 		es = signs[e_sign]
 		fd_a = charmap(next(f_digits))
-		fd_b = utils.strcat(map(charmap, f_digits))
-		ed = utils.strcat(map(charmap, e_digits))
+		fd_b = strcat(map(charmap, f_digits))
+		ed = strcat(map(charmap, e_digits))
 		# e = f"e{exp_digits}"
 		# e = f" * {base}**{exp_digits}"
 		return f"{fs}{fd_a}.{fd_b if fd_b else zero}e{es}{ed}"
 
 	return f
```

### Comparing `NumFmt-0.0.0.post0/numfmt/scistr/ieee754.py` & `NumFmt-0.0.0.post1/numfmt/scistr/ieee754.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 import typing as _tp
 import enum
+from ..utils import bits
 from . import fracs
-from .utils import bits
 
 
 def float_to_bits(f: float) -> int:
 	s = struct.pack('>f', f)
 	i = struct.unpack('>L', s)[0]
 	return i
```

### Comparing `NumFmt-0.0.0.post0/setup.py` & `NumFmt-0.0.0.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 NAME = "NumFmt"
-VERSION = '0.0.0-0'
+VERSION = '0.0.0-1'
 DESCRIPTION = 'Format Numbers in Any Base and Charset'
 
 
 def read(fname):
 	return open(os.path.join(os.path.dirname(__file__), fname)).read()
```

