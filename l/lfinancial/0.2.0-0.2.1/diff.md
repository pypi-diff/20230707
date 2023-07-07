# Comparing `tmp/lfinancial-0.2.0.tar.gz` & `tmp/lfinancial-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.0.tar", last modified: Thu Jul  6 09:22:29 2023, max compression
+gzip compressed data, was "lfinancial-0.2.1.tar", last modified: Fri Jul  7 15:08:03 2023, max compression
```

## Comparing `lfinancial-0.2.0.tar` & `lfinancial-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-06 09:22:11.000000 lfinancial-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 09:22:29.607624 lfinancial-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-06 09:22:11.000000 lfinancial-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/phone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:22:29.607624 lfinancial-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 09:22:11.000000 lfinancial-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 09:22:11.000000 lfinancial-0.2.0/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-07 15:07:42.000000 lfinancial-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 15:08:03.055751 lfinancial-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 15:07:42.000000 lfinancial-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-07 15:07:42.000000 lfinancial-0.2.1/lfinancial/generators/phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 15:08:03.000000 lfinancial-0.2.1/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:08:03.059751 lfinancial-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 15:07:42.000000 lfinancial-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:08:03.055751 lfinancial-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 15:07:42.000000 lfinancial-0.2.1/tests/test_document.py
```

### Comparing `lfinancial-0.2.0/LICENSE.txt` & `lfinancial-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/PKG-INFO` & `lfinancial-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -75,8 +75,11 @@
 # MA
 
 f.email()
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
+
+f.currency()
+# CNY
 ```
```

### Comparing `lfinancial-0.2.0/README.md` & `lfinancial-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,8 +63,11 @@
 # MA
 
 f.email()
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
+
+f.currency()
+# CNY
 ```
```

### Comparing `lfinancial-0.2.0/lfinancial/factory.py` & `lfinancial-0.2.1/lfinancial/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from lfinancial.generators.bank import BankGenerator
 from lfinancial.generators.contry import CountryGenerator
+from lfinancial.generators.currency import CurrencyGenerator
 from lfinancial.generators.document import IDCodeGenerator
 from lfinancial.generators.mail import EmailGenerator
 from lfinancial.generators.name import NameGenerator
 from lfinancial.generators.phone import PhoneGenerator
 
 
 class GeneratorFactory:
@@ -20,14 +21,15 @@
             "cn_name": NameGenerator(),
             "kana_name": NameGenerator(),
             "cellphone": PhoneGenerator(),
             "area_code": PhoneGenerator(),
             "high_risk": CountryGenerator(),
             "email": EmailGenerator(),
             "bank": BankGenerator(),
+            "currency": CurrencyGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.2.0/lfinancial/financial.py` & `lfinancial-0.2.1/lfinancial/financial.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
     def email(self, suffix=None):
         return self.__generate("email", suffix)
 
     def bank(self, country=None):
         return self.__generate("bank", country)
 
+    def currency(self, country=None):
+        return self.__generate("currency", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -68,7 +71,8 @@
     print(f.kana_name())
     print(f.cn_name())
     print(f.cellphone())
     print(f.area_code())
     print(f.high_risk_country())
     print(f.email())
     print(f.bank())
+    print(f.currency())
```

### Comparing `lfinancial-0.2.0/lfinancial/generators/bank.py` & `lfinancial-0.2.1/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/const.py` & `lfinancial-0.2.1/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/contry.py` & `lfinancial-0.2.1/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/document.py` & `lfinancial-0.2.1/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/mail.py` & `lfinancial-0.2.1/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/name.py` & `lfinancial-0.2.1/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial/generators/phone.py` & `lfinancial-0.2.1/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.0/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.1/lfinancial.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -75,8 +75,11 @@
 # MA
 
 f.email()
 # q0o58mkgq3@gmail.com
 
 f.bank()
 # BANK OF CHINA (HONG KONG) LIMITED
+
+f.currency()
+# CNY
 ```
```

### Comparing `lfinancial-0.2.0/setup.py` & `lfinancial-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.0',
+    version='0.2.1',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

