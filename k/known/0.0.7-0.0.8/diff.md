# Comparing `tmp/known-0.0.7.tar.gz` & `tmp/known-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known-0.0.7.tar", last modified: Fri Jul  7 20:33:30 2023, max compression
+gzip compressed data, was "known-0.0.8.tar", last modified: Fri Jul  7 20:49:50 2023, max compression
```

## Comparing `known-0.0.7.tar` & `known-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.405554 known-0.0.7/
--rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-07 20:33:30.405554 known-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.374308 known-0.0.7/module/
-drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.389934 known-0.0.7/module/known/
--rw-rw-rw-   0        0        0      555 2023-07-07 20:29:17.000000 known-0.0.7/module/known/__init__.py
--rw-rw-rw-   0        0        0    26159 2023-07-07 20:24:17.000000 known-0.0.7/module/known/basic.py
--rw-rw-rw-   0        0        0     5330 2023-07-07 20:30:42.000000 known-0.0.7/module/known/imgu.py
--rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.7/module/known/mailer.py
--rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.7/module/known/store.py
-drwxrwxrwx   0        0        0        0 2023-07-07 20:33:30.405554 known-0.0.7/module/known.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 20:33:30.000000 known-0.0.7/module/known.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 20:33:30.405554 known-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-07 20:29:24.000000 known-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.420099 known-0.0.8/
+-rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-07 20:49:50.420099 known-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.404453 known-0.0.8/module/
+drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.404453 known-0.0.8/module/known/
+-rw-rw-rw-   0        0        0      453 2023-07-07 20:48:30.000000 known-0.0.8/module/known/__init__.py
+-rw-rw-rw-   0        0        0    26381 2023-07-07 20:43:11.000000 known-0.0.8/module/known/basic.py
+-rw-rw-rw-   0        0        0     4988 2023-07-07 20:47:33.000000 known-0.0.8/module/known/imgu.py
+-rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.8/module/known/mailer.py
+-rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.8/module/known/store.py
+drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.420099 known-0.0.8/module/known.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 20:49:50.420099 known-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-07 20:48:08.000000 known-0.0.8/setup.py
```

### Comparing `known-0.0.7/LICENSE` & `known-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `known-0.0.7/module/known/basic.py` & `known-0.0.8/module/known/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,98 +530,14 @@
         return inst
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 class BaseConvert:
-    r""" Number System Conversion """
-
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
-
-        :returns:       represented number as a list of ordinals in base-n number system
-
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
-
-        :param num:     iterable of base-n digits
-        :param base:    base-n number system
-
-        :returns:       represented number as a integer in base-10 number system
-
-        .. seealso::
-            :func:`~known.basic.int2base`
-        """
-        res = 0
-        for i,n in enumerate(num): res+=(base**i)*n
-        return int(res)
-
-
-    SYM_BIN = { f'{i}':i for i in range(2) }
-    SYM_OCT = { f'{i}':i for i in range(8) }
-    SYM_DEC = { f'{i}':i for i in range(10) }
-    SYM_HEX = {**SYM_DEC , **{ s:(i+10) for i,s in enumerate(('A', 'B', 'C', 'D', 'E', 'F'))}}
-    
-    @staticmethod
-    def n_syms(n): return { f'{i}':i for i in range(n) }
-
-    @staticmethod
-    def to_base_10(syms:dict, num:str):
-        b = len(syms)
-        l = [ syms[n] for n in num[::-1] ]
-        return __class__.base2int(l, b)
-
-    @staticmethod
-    def from_base_10(syms:dict, num:int, joiner=''):
-        base = len(syms)
-        print(f'----{num=} {type(num)}, {base=}, {type(base)}')
-        ndig = 1 + (0 if num==0 else floor(log(num, base))) # __class__.ndigs(num, base)
-        ss = tuple(syms.keys())
-        S = [ ss[i]  for i in __class__.int2base(num, base, ndig) ]
-        return joiner.join(S[::-1])
-
-
-    @staticmethod
-    def int2hex(num:int, joiner=''): return __class__.from_base_10(__class__.SYM_HEX, num, joiner)
-        
-
-
-
-class BaseConverter:
     r""" Number System Conversion 
     
     A number is abstract concept that has many representations using sets of symbols
 
     A base-n number system uses a set of n digits to represent any number
     This is called the representation of the number
 
@@ -660,14 +576,17 @@
         #repr_to = np.dot(digits_to , mult_to)
         #assert repr_to==repr_from
         if reversed: digits_to = digits_to[::-1]
         return tuple(digits_to)
 
 
     @staticmethod
+    def ndigits(num:int, base:int): return ceil(log(num,base))
+
+    @staticmethod
     def int2base(num:int, base:int, digs:int) -> list:
         r""" 
         Convert base-10 integer to a base-n list of fixed no. of digits 
 
         :param num:     base-10 number to be represented
         :param base:    base-n number system
         :param digs:    no of digits in the output
@@ -728,7 +647,94 @@
         return joiner.join(S[::-1])
 
 
     @staticmethod
     def int2hex(num:int, joiner=''): return __class__.from_base_10(__class__.SYM_HEX, num, joiner)
         
 
+
+
+# ARCHIVE
+
+# class BaseConvert:
+#     r""" Number System Conversion """
+
+
+#     @staticmethod
+#     def ndigs(num:int, base:int) -> int:
+#         r""" 
+#         Returns the number of digits required to represent a base-10 number in the given base.
+
+#         :param num:     base-10 number to be represented
+#         :param base:    base-n number system
+#         """
+#         return 1 + (0 if num==0 else floor(log(num, base)))
+
+#     @staticmethod
+#     def int2base(num:int, base:int, digs:int) -> list:
+#         r""" 
+#         Convert base-10 integer to a base-n list of fixed no. of digits 
+
+#         :param num:     base-10 number to be represented
+#         :param base:    base-n number system
+#         :param digs:    no of digits in the output
+
+#         :returns:       represented number as a list of ordinals in base-n number system
+
+#         .. seealso::
+#             :func:`~known.basic.base2int`
+#         """
+#         if not digs: digs=__class__.ndigs(num, base)
+#         res = [ 0 for _ in range(digs) ]
+#         q = num
+#         for i in range(digs): # <-- do not use enumerate plz
+#             res[i]=q%base
+#             q = floor(q/base)
+#         return res
+
+#     @staticmethod
+#     def base2int(num:Iterable, base:int) -> int:
+#         """ 
+#         Convert an iterbale of digits in base-n system to base-10 integer
+
+#         :param num:     iterable of base-n digits
+#         :param base:    base-n number system
+
+#         :returns:       represented number as a integer in base-10 number system
+
+#         .. seealso::
+#             :func:`~known.basic.int2base`
+#         """
+#         res = 0
+#         for i,n in enumerate(num): res+=(base**i)*n
+#         return int(res)
+
+
+#     SYM_BIN = { f'{i}':i for i in range(2) }
+#     SYM_OCT = { f'{i}':i for i in range(8) }
+#     SYM_DEC = { f'{i}':i for i in range(10) }
+#     SYM_HEX = {**SYM_DEC , **{ s:(i+10) for i,s in enumerate(('A', 'B', 'C', 'D', 'E', 'F'))}}
+    
+#     @staticmethod
+#     def n_syms(n): return { f'{i}':i for i in range(n) }
+
+#     @staticmethod
+#     def to_base_10(syms:dict, num:str):
+#         b = len(syms)
+#         l = [ syms[n] for n in num[::-1] ]
+#         return __class__.base2int(l, b)
+
+#     @staticmethod
+#     def from_base_10(syms:dict, num:int, joiner=''):
+#         base = len(syms)
+#         print(f'----{num=} {type(num)}, {base=}, {type(base)}')
+#         ndig = 1 + (0 if num==0 else floor(log(num, base))) # __class__.ndigs(num, base)
+#         ss = tuple(syms.keys())
+#         S = [ ss[i]  for i in __class__.int2base(num, base, ndig) ]
+#         return joiner.join(S[::-1])
+
+
+#     @staticmethod
+#     def int2hex(num:int, joiner=''): return __class__.from_base_10(__class__.SYM_HEX, num, joiner)
+        
+
+
```

### Comparing `known-0.0.7/module/known/imgu.py` & `known-0.0.8/module/known/imgu.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,22 +60,14 @@
         hex = hex.upper()
         lenhex = len(hex)
         assert lenhex==6 or lenhex==8, f'expecting 6 or 8 chars but got {lenhex} :: {hex}'
         if lenhex==6: hex = 'FF' + hex # max alpha
         B,G,R,A = tuple(BaseConvert.int2base(num=BaseConvert.to_base_10(BaseConvert.SYM_HEX, hex), base=256, digs=4))
         return self.set_color_at(row,col,(R,G,B,A))
     
-
-    def get_hex_at(self, row:int, col:int):
-        r,g,b,a = self.get_color_at(row, col, normalize=False)
-        int_code = BaseConvert.base2int(num=(b,g,r,a), base=256)
-        print(f'{int_code=}, {type(int_code)}')
-        hex_code = BaseConvert.int2hex(int_code,joiner='')
-        print(f'{hex_code=}')
-        return hex_code
     
     @staticmethod
     def save(pix, path):  
         return cv2.imwrite(path, pix.i)
 
     @staticmethod
     def load(path):
```

### Comparing `known-0.0.7/module/known/mailer.py` & `known-0.0.8/module/known/mailer.py`

 * *Files identical despite different names*

### Comparing `known-0.0.7/module/known/store.py` & `known-0.0.8/module/known/store.py`

 * *Files identical despite different names*

### Comparing `known-0.0.7/setup.py` & `known-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name =                      'known',
-    version =                   '0.0.7',
+    version =                   '0.0.8',
     url =                       'https://github.com/Nelson-iitp/known',
     author =                    'Nelson.S',
     author_email =              'mail.nelsonsharma@gmail.com',
     description =               'Module :: known',
     packages =                  ['known'],
     classifiers=                ['License :: OSI Approved :: MIT License'],
     package_dir =               { '' : 'module'},
```

