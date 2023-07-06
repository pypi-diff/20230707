# Comparing `tmp/hosh-3.230705.1.tar.gz` & `tmp/hosh-3.230705.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosh-3.230705.1.tar", max compression
+gzip compressed data, was "hosh-3.230705.2.tar", max compression
```

## Comparing `hosh-3.230705.1.tar` & `hosh-3.230705.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-3.230705.1/LICENSE
--rw-r--r--   0        0        0     9771 2023-07-05 21:21:04.153737 hosh-3.230705.1/README.md
--rw-r--r--   0        0        0      776 2023-07-05 21:21:10.973739 hosh-3.230705.1/pyproject.toml
--rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-3.230705.1/src/hosh/__init__.py
--rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-3.230705.1/src/hosh/_internals_appearance.py
--rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-3.230705.1/src/hosh/config.py
--rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/groups.py
--rw-r--r--   0        0        0    39941 2023-07-05 21:11:26.169527 hosh-3.230705.1/src/hosh/hosh_.py
--rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-3.230705.1/src/hosh/misc/__init__.py
--rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-3.230705.1/src/hosh/misc/colors.py
--rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/core.py
--rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/encoding/__init__.py
--rw-r--r--   0        0        0     9099 2023-04-17 16:49:34.360852 hosh-3.230705.1/src/hosh/misc/encoding/base.py
--rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/encoding/base777.py
--rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-3.230705.1/src/hosh/misc/exception.py
--rw-r--r--   0        0        0     1559 2023-04-22 00:24:44.334832 hosh-3.230705.1/src/hosh/misc/helper.py
--rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-3.230705.1/src/hosh/misc/identity.py
--rw-r--r--   0        0        0     4988 2023-05-04 17:05:47.757107 hosh-3.230705.1/src/hosh/misc/math.py
--rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-3.230705.1/src/hosh/misc/root.py
--rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-3.230705.1/src/hosh/theme.py
--rw-r--r--   0        0        0    10787 1970-01-01 00:00:00.000000 hosh-3.230705.1/setup.py
--rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 hosh-3.230705.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-3.230705.2/LICENSE
+-rw-r--r--   0        0        0     9771 2023-07-06 23:03:36.170467 hosh-3.230705.2/README.md
+-rw-r--r--   0        0        0      776 2023-07-06 23:03:39.974468 hosh-3.230705.2/pyproject.toml
+-rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-3.230705.2/src/hosh/__init__.py
+-rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-3.230705.2/src/hosh/_internals_appearance.py
+-rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-3.230705.2/src/hosh/config.py
+-rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-3.230705.2/src/hosh/groups.py
+-rw-r--r--   0        0        0    39936 2023-07-06 23:00:29.730380 hosh-3.230705.2/src/hosh/hosh_.py
+-rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-3.230705.2/src/hosh/misc/__init__.py
+-rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-3.230705.2/src/hosh/misc/colors.py
+-rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-3.230705.2/src/hosh/misc/core.py
+-rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-3.230705.2/src/hosh/misc/encoding/__init__.py
+-rw-r--r--   0        0        0     9099 2023-04-17 16:49:34.360852 hosh-3.230705.2/src/hosh/misc/encoding/base.py
+-rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-3.230705.2/src/hosh/misc/encoding/base777.py
+-rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-3.230705.2/src/hosh/misc/exception.py
+-rw-r--r--   0        0        0     1559 2023-04-22 00:24:44.334832 hosh-3.230705.2/src/hosh/misc/helper.py
+-rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-3.230705.2/src/hosh/misc/identity.py
+-rw-r--r--   0        0        0     4988 2023-05-04 17:05:47.757107 hosh-3.230705.2/src/hosh/misc/math.py
+-rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-3.230705.2/src/hosh/misc/root.py
+-rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-3.230705.2/src/hosh/theme.py
+-rw-r--r--   0        0        0    10787 1970-01-01 00:00:00.000000 hosh-3.230705.2/setup.py
+-rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 hosh-3.230705.2/PKG-INFO
```

### Comparing `hosh-3.230705.1/LICENSE` & `hosh-3.230705.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/README.md` & `hosh-3.230705.2/README.md`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/pyproject.toml` & `hosh-3.230705.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hosh"
-version = "3.230705.1"
+version = "3.230705.2"
 description = "Predictable Operable HaSH-based identifiers"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "hosh", from = "src" },
 ]
```

### Comparing `hosh-3.230705.1/src/hosh/__init__.py` & `hosh-3.230705.2/src/hosh/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/_internals_appearance.py` & `hosh-3.230705.2/src/hosh/_internals_appearance.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/config.py` & `hosh-3.230705.2/src/hosh/config.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/groups.py` & `hosh-3.230705.2/src/hosh/groups.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/hosh_.py` & `hosh-3.230705.2/src/hosh/hosh_.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,15 +895,15 @@
         =======
             List if hoshes
 
         >>> from hosh import Hosh
         >>> a = Hosh(b"a")
         >>> a[-1].rev == a
         True
-        >>> a[0, 1][0] == a
+        >>> a[0, 1] == a
         True
         >>> a[0:, 1][0] == a
         True
         >>> a[:1, 1][0] == a
         True
         >>> a[0:1, 1][0] == a
         True
@@ -979,15 +979,15 @@
         if n <= 0:  # pragma: no cover
             raise Exception(f"Wrong value: n={n}  <=  0")
 
         if isinstance(idx := slc, int):
             if idx < n - 1:
                 return Hosh(f"{self.id}-{idx}".encode())
             if n == 1:
-                return [self]
+                return self
             if idx == n - 1:
                 return list(self.components(0, n, n))[idx]
             raise Exception(f"Wrong value: i={slc}  >  n={n}")  # pragma: no cover
 
         if not isinstance(slc, slice) or slc.step is not None:  # pragma: no cover
             raise Exception(f"Wrong syntax. Simple slice or index expected as first tuple item, not `{slc}`: hosh[i, n] or hosh[l:m, n]")
```

### Comparing `hosh-3.230705.1/src/hosh/misc/__init__.py` & `hosh-3.230705.2/src/hosh/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/colors.py` & `hosh-3.230705.2/src/hosh/misc/colors.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/core.py` & `hosh-3.230705.2/src/hosh/misc/core.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/encoding/__init__.py` & `hosh-3.230705.2/src/hosh/misc/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/encoding/base.py` & `hosh-3.230705.2/src/hosh/misc/encoding/base.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/encoding/base777.py` & `hosh-3.230705.2/src/hosh/misc/encoding/base777.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/exception.py` & `hosh-3.230705.2/src/hosh/misc/exception.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/helper.py` & `hosh-3.230705.2/src/hosh/misc/helper.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/identity.py` & `hosh-3.230705.2/src/hosh/misc/identity.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/math.py` & `hosh-3.230705.2/src/hosh/misc/math.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/misc/root.py` & `hosh-3.230705.2/src/hosh/misc/root.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/src/hosh/theme.py` & `hosh-3.230705.2/src/hosh/theme.py`

 * *Files identical despite different names*

### Comparing `hosh-3.230705.1/setup.py` & `hosh-3.230705.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'blake3>=0.3.3,<0.4.0',
  'bs4>=0.0.1,<0.0.2',
  'colored==1.4.2',
  'wheel>=0.40.0,<0.41.0']
 
 setup_kwargs = {
     'name': 'hosh',
-    'version': '3.230705.1',
+    'version': '3.230705.2',
     'description': 'Predictable Operable HaSH-based identifiers',
     'long_description': '![test](https://github.com/davips/hosh/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)\n<a href="https://pypi.org/project/hosh">\n<img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)\n\n# hosh - Identification based on group theory\n[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https://davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).\nA previous version, containing extra group theory content, is available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA first implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh` and serves as an advanced usage example.\n<br>\nA second (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/project/hoshmap).\nThe most recent rewritten version of a hosh-based dict (and the most robust, recommended, one) is available in the package [hdict](https://pypi.org/project/hdict).\n\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/hosh) \nand [GitHub repository](https://github.com/davips/hosh), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/hosh/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/hosh).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install hosh\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/hosh\ncd hosh\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom hosh import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n\n## Performance\nComputation time for the simple operations performed by `hosh` can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_6.png)\nThe package [hoshrust](https://pypi.org/project/hoshrust) was a faster implementation of an earlier version of `hosh`.\nAs the performance of the current `hosh` seems already very high (only ~2x slower than if it was implemented in native code in like _rust_), \nwe don\'t have plans for a new \'rust\' implementation in the near future.\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hosh', 'hosh.misc', 'hosh.misc.encoding'] package_data =
 \ {'': ['*']} install_requires = \ ['ansi2html>=1.6.0,<2.0.0',
 'blake3>=0.3.3,<0.4.0', 'bs4>=0.0.1,<0.0.2', 'colored==1.4.2',
 'wheel>=0.40.0,<0.41.0'] setup_kwargs = { 'name': 'hosh', 'version':
-'3.230705.1', 'description': 'Predictable Operable HaSH-based identifiers',
+'3.230705.2', 'description': 'Predictable Operable HaSH-based identifiers',
 'long_description': '![test](https://github.com/davips/hosh/workflows/test/
 badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/
 badge.svg)](https://codecov.io/gh/davips/hosh)\n\n[pypi]\n\n![Python version]
 (https://img.shields.io/badge/python-â¥3.8-blue.svg)\n[![license: GPL v3]
 (https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/
 zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https:/
```

### Comparing `hosh-3.230705.1/PKG-INFO` & `hosh-3.230705.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosh
-Version: 3.230705.1
+Version: 3.230705.2
 Summary: Predictable Operable HaSH-based identifiers
 License: GPL
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hosh Version: 3.230705.1 Summary: Predictable
+Metadata-Version: 2.1 Name: hosh Version: 3.230705.2 Summary: Predictable
 Operable HaSH-based identifiers License: GPL Author: davips Author-email:
 dpsabc@gmail.com Requires-Python: >=3.8 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: ansi2html
 (>=1.6.0,<2.0.0) Requires-Dist: blake3 (>=0.3.3,<0.4.0) Requires-Dist: bs4
```

