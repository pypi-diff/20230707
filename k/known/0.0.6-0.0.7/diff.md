# Comparing `tmp/known-0.0.6.tar.gz` & `tmp/known-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known-0.0.6.tar", last modified: Sat Jul  1 21:58:40 2023, max compression
+gzip compressed data, was "known-0.0.7.tar", last modified: Fri Jul  7 20:33:30 2023, max compression
```

## Comparing `known-0.0.6.tar` & `known-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.519152 known-0.0.6/
--rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-01 21:58:40.518158 known-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.494175 known-0.0.6/module/
-drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.503153 known-0.0.6/module/known/
--rw-rw-rw-   0        0        0      555 2023-07-01 21:52:09.000000 known-0.0.6/module/known/__init__.py
--rw-rw-rw-   0        0        0    21804 2023-07-01 21:41:03.000000 known-0.0.6/module/known/basic.py
--rw-rw-rw-   0        0        0     6166 2023-07-01 21:51:03.000000 known-0.0.6/module/known/imgu.py
--rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.6/module/known/mailer.py
--rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.6/module/known/store.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.516149 known-0.0.6/module/known.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 21:58:40.519152 known-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-01 21:49:59.000000 known-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.405554 known-0.0.7/
+-rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-07 20:33:30.405554 known-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.374308 known-0.0.7/module/
+drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.389934 known-0.0.7/module/known/
+-rw-rw-rw-   0        0        0      555 2023-07-07 20:29:17.000000 known-0.0.7/module/known/__init__.py
+-rw-rw-rw-   0        0        0    26159 2023-07-07 20:24:17.000000 known-0.0.7/module/known/basic.py
+-rw-rw-rw-   0        0        0     5330 2023-07-07 20:30:42.000000 known-0.0.7/module/known/imgu.py
+-rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.7/module/known/mailer.py
+-rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.7/module/known/store.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.405554 known-0.0.7/module/known.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 20:33:30.405554 known-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-07 20:29:24.000000 known-0.0.7/setup.py
```

### Comparing `known-0.0.6/LICENSE` & `known-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `known-0.0.6/module/known/__init__.py` & `known-0.0.7/module/known/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 .. code-block:: console
 
    >>> import known
    >>> known.__version___
 
 :py:mod:`known/__init__.py`
 """
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 #print(f'known.{__version__}')
 
 
 # from .basic import *
 # from .imgu import *
 # from .mailer import *
 # from .store import *
```

### Comparing `known-0.0.6/module/known/basic.py` & `known-0.0.7/module/known/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'onehot', 'onecold', 'dict_sort', 
 ]
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 import datetime
 from typing import Any, Union, Iterable #, BinaryIO, cast, Dict, Optional, Type, Tuple, IO
 import numpy as np
 from numpy import ndarray
-from math import floor, log
+from math import floor, log, ceil
 import json, pickle
 from collections import UserDict
 #import pickle, pathlib, io
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 def now(year:bool=True, month:bool=True, day:bool=True, 
         hour:bool=True, minute:bool=True, second:bool=True, mirco:bool=True, 
@@ -104,67 +104,18 @@
     else:
         ks = K[S][::-1]
         vs = V[S][::-1]
         ss = S[::-1]
     
     return {k:v for k,v in zip(ks,vs)} if return_dict else (ks,vs,ss)
 
-#=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
-
-class BaseConvert:
-    r""" Number System Conversion """
-
-    @staticmethod
-    def ndigs(num:int, base:int) -> int:
-        r""" 
-        Returns the number of digits required to represent a base-10 number in the given base.
-
-        :param num:     base-10 number to be represented
-        :param base:    base-n number system
-        """
-        return 1 + (0 if num==0 else floor(log(num, base)))
-
-    @staticmethod
-    def int2base(num:int, base:int, digs:int) -> list:
-        r""" 
-        Convert base-10 integer to a base-n list of fixed no. of digits 
-
-        :param num:     base-10 number to be represented
-        :param base:    base-n number system
-        :param digs:    no of digits in the output
 
-        :returns:       represented number as a list of ordinals in base-n number system
 
-        .. seealso::
-            :func:`~known.basic.base2int`
-        """
-        if not digs: digs=__class__.ndigs(num, base)
-        res = [ 0 for _ in range(digs) ]
-        q = num
-        for i in range(digs): # <-- do not use enumerate plz
-            res[i]=q%base
-            q = floor(q/base)
-        return res
-
-    @staticmethod
-    def base2int(num:Iterable, base:int) -> int:
-        """ 
-        Convert an iterbale of digits in base-n system to base-10 integer
 
-        :param num:     iterable of base-n digits
-        :param base:    base-n number system
 
-        :returns:       represented number as a integer in base-10 number system
-
-        .. seealso::
-            :func:`~known.basic.int2base`
-        """
-        res = 0
-        for i,n in enumerate(num): res+=(base**i)*n
-        return res
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 class Symbols:
     r"""
     contains some special symbols described in the table below
 
@@ -576,37 +527,208 @@
         # Create a copy and avoid triggering descriptors
         inst.__dict__["data"] = self.__dict__["data"].copy()
         inst.__dict__["names"] = self.__dict__["names"].copy()
         return inst
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
+#=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
+
+class BaseConvert:
+    r""" Number System Conversion """
 
 
-# def pname(path:str, sep:str='.'): 
-#     r""" Path Name - retuns the path except file extension using ``path[0:path.rfind(sep)]`` 
+    @staticmethod
+    def ndigs(num:int, base:int) -> int:
+        r""" 
+        Returns the number of digits required to represent a base-10 number in the given base.
+
+        :param num:     base-10 number to be represented
+        :param base:    base-n number system
+        """
+        return 1 + (0 if num==0 else floor(log(num, base)))
+
+    @staticmethod
+    def int2base(num:int, base:int, digs:int) -> list:
+        r""" 
+        Convert base-10 integer to a base-n list of fixed no. of digits 
+
+        :param num:     base-10 number to be represented
+        :param base:    base-n number system
+        :param digs:    no of digits in the output
+
+        :returns:       represented number as a list of ordinals in base-n number system
+
+        .. seealso::
+            :func:`~known.basic.base2int`
+        """
+        if not digs: digs=__class__.ndigs(num, base)
+        res = [ 0 for _ in range(digs) ]
+        q = num
+        for i in range(digs): # <-- do not use enumerate plz
+            res[i]=q%base
+            q = floor(q/base)
+        return res
+
+    @staticmethod
+    def base2int(num:Iterable, base:int) -> int:
+        """ 
+        Convert an iterbale of digits in base-n system to base-10 integer
+
+        :param num:     iterable of base-n digits
+        :param base:    base-n number system
+
+        :returns:       represented number as a integer in base-10 number system
+
+        .. seealso::
+            :func:`~known.basic.int2base`
+        """
+        res = 0
+        for i,n in enumerate(num): res+=(base**i)*n
+        return int(res)
+
+
+    SYM_BIN = { f'{i}':i for i in range(2) }
+    SYM_OCT = { f'{i}':i for i in range(8) }
+    SYM_DEC = { f'{i}':i for i in range(10) }
+    SYM_HEX = {**SYM_DEC , **{ s:(i+10) for i,s in enumerate(('A', 'B', 'C', 'D', 'E', 'F'))}}
+    
+    @staticmethod
+    def n_syms(n): return { f'{i}':i for i in range(n) }
+
+    @staticmethod
+    def to_base_10(syms:dict, num:str):
+        b = len(syms)
+        l = [ syms[n] for n in num[::-1] ]
+        return __class__.base2int(l, b)
+
+    @staticmethod
+    def from_base_10(syms:dict, num:int, joiner=''):
+        base = len(syms)
+        print(f'----{num=} {type(num)}, {base=}, {type(base)}')
+        ndig = 1 + (0 if num==0 else floor(log(num, base))) # __class__.ndigs(num, base)
+        ss = tuple(syms.keys())
+        S = [ ss[i]  for i in __class__.int2base(num, base, ndig) ]
+        return joiner.join(S[::-1])
+
+
+    @staticmethod
+    def int2hex(num:int, joiner=''): return __class__.from_base_10(__class__.SYM_HEX, num, joiner)
+        
+
+
+
+class BaseConverter:
+    r""" Number System Conversion 
+    
+    A number is abstract concept that has many representations using sets of symbols
+
+    A base-n number system uses a set of n digits to represent any number
+    This is called the representation of the number
+
+    Given one representation, we only need to convert to another
+
+    """
+
+    DIGITS_DTYPE =  np.uint32
+    @staticmethod
+    def convert(digits, base_from, base_to, reversed=True):
+        r""" convers from one base to another 
+        
+        :param digits:      iterable of digits in base ```base_from```. NOTE: digits are Natural Numbers starting at 0. base 'b' will have digits between [0, b-1]
+        :param base_from:   int - the base to convert from
+        :param base_to:     int - the base to convert to
+        :param reversed:    bool - if True, digits are assumed in reverse (human readable left to right)
+                            e.g. if reversed is True then binary digits iterable [1,0,0] will represent [4] in decimal otherwise it will represent [1] in decimal
+        """
+
+        digits_from =  np.array(digits, dtype=__class__.DIGITS_DTYPE) # convert to int data-type
+        if reversed: digits_from = digits_from[::-1]
+        ndigits_from = len(digits_from)
+        mult_from = np.array([base_from**i for i in range(ndigits_from)], dtype=__class__.DIGITS_DTYPE)
+        repr_from = np.dot(digits_from , mult_from)
+
+        #ndc = base_from**ndigits_from
+        ndigits_to = ceil(log(repr_from,base_to))
+        digits_to =  np.zeros((ndigits_to,), dtype=__class__.DIGITS_DTYPE)
+        n = int(repr_from)
+        for d in range(ndigits_to):
+            digits_to[d] = n%base_to
+            n=n//base_to
+            #n = (n-digits_to[d])/base_to
+
+        #mult_to = np.array([base_to**i for i in range(ndigits_to)])
+        #repr_to = np.dot(digits_to , mult_to)
+        #assert repr_to==repr_from
+        if reversed: digits_to = digits_to[::-1]
+        return tuple(digits_to)
+
+
+    @staticmethod
+    def int2base(num:int, base:int, digs:int) -> list:
+        r""" 
+        Convert base-10 integer to a base-n list of fixed no. of digits 
+
+        :param num:     base-10 number to be represented
+        :param base:    base-n number system
+        :param digs:    no of digits in the output
+
+        :returns:       represented number as a list of ordinals in base-n number system
+
+        .. seealso::
+            :func:`~known.basic.base2int`
+        """
+        
+        ndigits = digs if digs else ceil(log(num,base)) 
+        digits =  np.zeros((ndigits,), dtype=__class__.DIGITS_DTYPE)
+        n = num
+        for d in range(ndigits):
+            digits[d] = n%base
+            n=n//base
+        return digits
+
+    @staticmethod
+    def base2int(num:Iterable, base:int) -> int:
+        """ 
+        Convert an iterbale of digits in base-n system to base-10 integer
+
+        :param num:     iterable of base-n digits
+        :param base:    base-n number system
+
+        :returns:       represented number as a integer in base-10 number system
+
+        .. seealso::
+            :func:`~known.basic.int2base`
+        """
+        res = 0
+        for i,n in enumerate(num): res+=(base**i)*n
+        return int(res)
+
+
+    SYM_BIN = { f'{i}':i for i in range(2) }
+    SYM_OCT = { f'{i}':i for i in range(8) }
+    SYM_DEC = { f'{i}':i for i in range(10) }
+    SYM_HEX = {**SYM_DEC , **{ s:(i+10) for i,s in enumerate(('A', 'B', 'C', 'D', 'E', 'F'))}}
     
-#     .. seealso::
-#         :func:`~known.basic.pext`
-#         :func:`~known.basic.psplit`
-#     """
-#     return path[0:path.rfind(sep)]
-
-# def pext(path:str, sep:str='.'): 
-#     r""" Path Extension - retuns the extension from a path using ``path[path.rfind(sep):]`` 
-
-#     .. seealso::
-#         :func:`~known.basic.pname`
-#         :func:`~known.basic.psplit`
-#     """
-#     return path[path.rfind(sep):]
-
-# def psplit(path:str, sep:str='.'): 
-#     r""" Path Split - splits the path into name and extension
+    @staticmethod
+    def n_syms(n): return { f'{i}':i for i in range(n) }
+
+    @staticmethod
+    def to_base_10(syms:dict, num:str):
+        b = len(syms)
+        l = [ syms[n] for n in num[::-1] ]
+        return __class__.base2int(l, b)
+
+    @staticmethod
+    def from_base_10(syms:dict, num:int, joiner=''):
+        base = len(syms)
+        print(f'----{num=} {type(num)}, {base=}, {type(base)}')
+        ndig = 1 + (0 if num==0 else floor(log(num, base))) # __class__.ndigs(num, base)
+        ss = tuple(syms.keys())
+        S = [ ss[i]  for i in __class__.int2base(num, base, ndig) ]
+        return joiner.join(S[::-1])
 
-#     :returns: 2-tuple (Name, Ext)
 
-#     .. note:: This is the same as using :func:`~known.basic.pname` and :func:`~known.basic.pext` together. 
-#         This may be used to create copies of a file by adding a suffix to its name witout changing the extension.
+    @staticmethod
+    def int2hex(num:int, joiner=''): return __class__.from_base_10(__class__.SYM_HEX, num, joiner)
+        
 
-#     """
-#     return (path[0:path.rfind(sep)], path[path.rfind(sep):])
```

### Comparing `known-0.0.6/module/known/mailer.py` & `known-0.0.7/module/known/mailer.py`

 * *Files identical despite different names*

### Comparing `known-0.0.6/module/known/store.py` & `known-0.0.7/module/known/store.py`

 * *Files identical despite different names*

### Comparing `known-0.0.6/setup.py` & `known-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name =                      'known',
-    version =                   '0.0.6',
+    version =                   '0.0.7',
     url =                       'https://github.com/Nelson-iitp/known',
     author =                    'Nelson.S',
     author_email =              'mail.nelsonsharma@gmail.com',
     description =               'Module :: known',
     packages =                  ['known'],
     classifiers=                ['License :: OSI Approved :: MIT License'],
     package_dir =               { '' : 'module'},
```

