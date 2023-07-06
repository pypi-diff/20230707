# Comparing `tmp/shelchemy-0.220906.5.tar.gz` & `tmp/shelchemy-1.230706.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelchemy-0.220906.5.tar", max compression
+gzip compressed data, was "shelchemy-1.230706.1.tar", max compression
```

## Comparing `shelchemy-0.220906.5.tar` & `shelchemy-1.230706.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-0.220906.5/LICENSE
--rw-r--r--   0        0        0     1348 2023-04-08 03:46:59.633950 shelchemy-0.220906.5/README.md
--rw-r--r--   0        0        0     1034 2023-04-08 03:47:00.789966 shelchemy-0.220906.5/pyproject.toml
--rw-r--r--   0        0        0       34 2022-08-23 03:49:07.000000 shelchemy-0.220906.5/src/shelchemy/__init__.py
--rw-r--r--   0        0        0     8257 2023-04-08 02:56:56.417591 shelchemy-0.220906.5/src/shelchemy/cache.py
--rw-r--r--   0        0        0     1758 2022-09-06 20:21:46.000000 shelchemy-0.220906.5/src/shelchemy/lazy.py
--rw-r--r--   0        0        0     5340 2023-01-31 13:59:11.645687 shelchemy-0.220906.5/src/shelchemy/locker.py
--rw-r--r--   0        0        0     2097 2023-01-12 19:31:50.000000 shelchemy-0.220906.5/src/shelchemy/scheduler.py
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 shelchemy-0.220906.5/setup.py
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 shelchemy-0.220906.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-1.230706.1/LICENSE
+-rw-r--r--   0        0        0     1348 2023-07-06 23:39:02.187317 shelchemy-1.230706.1/README.md
+-rw-r--r--   0        0        0     1036 2023-07-06 23:39:11.599322 shelchemy-1.230706.1/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-06 23:38:55.083313 shelchemy-1.230706.1/src/shelchemy/__init__.py
+-rw-r--r--   0        0        0     8274 2023-07-06 23:38:55.179313 shelchemy-1.230706.1/src/shelchemy/cache.py
+-rw-r--r--   0        0        0     1758 2022-09-06 20:21:46.000000 shelchemy-1.230706.1/src/shelchemy/lazy.py
+-rw-r--r--   0        0        0     5350 2023-04-14 21:34:25.807393 shelchemy-1.230706.1/src/shelchemy/locker.py
+-rw-r--r--   0        0        0     2097 2023-01-12 19:31:50.000000 shelchemy-1.230706.1/src/shelchemy/scheduler.py
+-rw-r--r--   0        0        0      333 2023-07-06 23:38:55.087313 shelchemy-1.230706.1/src/shelchemy/sqla.py
+-rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 shelchemy-1.230706.1/setup.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 shelchemy-1.230706.1/PKG-INFO
```

### Comparing `shelchemy-0.220906.5/LICENSE` & `shelchemy-1.230706.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shelchemy-0.220906.5/README.md` & `shelchemy-1.230706.1/README.md`

 * *Files identical despite different names*

### Comparing `shelchemy-0.220906.5/pyproject.toml` & `shelchemy-1.230706.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "shelchemy"
-version = "0.220906.5"
-description = "Shelve-like dict using sqlachemy as backend, and lazy scheduler for resuming tasks"
+version = "1.230706.1"
+description = "Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "shelchemy", from = "src" }
 ]
 
@@ -35,8 +35,7 @@
 click = "8.0.4"
 lz4 = "^4.0.2"
 safeserializer = "^0.230202.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `shelchemy-0.220906.5/src/shelchemy/cache.py` & `shelchemy-1.230706.1/src/shelchemy/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,58 +21,45 @@
 #  time spent here.
 
 from contextlib import contextmanager
 from hashlib import md5
 from pickle import dumps
 from typing import TypeVar
 
-from sqlalchemy import Column, String, create_engine, LargeBinary
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 
-VT = TypeVar("VT")
-Base = declarative_base()
-memory = "sqlite+pysqlite:///:memory:"
-
+from shelchemy import memory
+from shelchemy.sqla import Base, Content
 
-class Content(Base):
-    __tablename__ = "content"
-    id = Column(String(40), primary_key=True)
-    blob = Column(LargeBinary(length=(2**32) - 1))
+VT = TypeVar("VT")
 
 
 def check(key):
     if not isinstance(key, str):
         try:
             dump = dumps(key, protocol=5)
         except Exception as e:
             print(e)
             raise WrongKeyType(f"Key must be string or serializable (pickable), not {type(key)}.", key)
         key = dump
     return md5(key.encode()).hexdigest() if len(key) not in [32, 40] else key
 
 
-@contextmanager
-def sopen(url=memory, ondup="overwrite", autopack=True, safepack=False, stablepack=False, debug=False):
-    engine = create_engine(url, echo=debug)
-    Base.metadata.create_all(engine)
-    with Session(engine, autoflush=False) as session:
-        yield Cache(session, ondup, autopack, safepack, stablepack, debug)
-
-
 class Cache:
     r"""
     Dict-like persistence based on SQLAlchemy
 
     string or serializable (pickle) keys only
 
     When len(key) not in [32, 40], key is internally hashed to a MD5 hexdigest
 
     Usage:
 
+    >>> from shelchemy import sopen
     >>> d = Cache("sqlite+pysqlite:////tmp/sqla-test.db")
     >>> d["x"] = 5
     >>> d["x"]
     5
     >>> for k, v in d.items():
     ...     print(k, v)
     9dd4e461268c8034f5c8564e155c67a6 5
@@ -100,68 +87,85 @@
     {'9dd4e461268c8034f5c8564e155c67a6': b'asd'}
     True
     True
     True
     False
     """
 
-    def __init__(self, session=memory, ondup="overwrite", autopack=True, safepack=False, stablepack=False, debug=False):
+    def __init__(
+        self, session=memory, ondup="overwrite", autopack=True, safepack=False, stablepack=False, debug=False, _engine=None
+    ):
         if isinstance(session, str):
 
             @contextmanager
             def sessionctx():
                 engine = create_engine(url=session, echo=debug)
-                Base.metadata.create_all(engine)
+                self._engine = engine
                 session_ = Session(engine, autoflush=False)
                 yield session_
                 session_.close()
 
         else:
+            if _engine is None:
+                raise Exception(f"Missing `_engine` for external non string session.")
+            self._engine = _engine
 
             @contextmanager
             def sessionctx():
                 yield session
 
         self.sessionctx = sessionctx
         self.ondup = ondup
         self.autopack = autopack
         self.safepack = safepack
         self.stablepack = stablepack
 
+    def ensure_build(self, query__f):
+        with self.sessionctx() as session:
+            try:
+                return query__f(session)
+            except Exception as e:
+                try:
+                    Base.metadata.create_all(self._engine)
+                except:
+                    raise e from None
+        return query__f(session)
+
     def __contains__(self, key):
         key = check(key)
-        with self.sessionctx() as session:
-            return session.query(Content).filter_by(id=key).first() is not None
+        return self.ensure_build(lambda session: session.query(Content).filter_by(id=key).first() is not None)
 
     def __iter__(self):
-        with self.sessionctx() as session:
-            return (c.id for c in session.query(Content).all())
+        return self.ensure_build(lambda session: (c.id for c in session.query(Content).all()))
 
     def __setitem__(self, key: str, value, packing=True):
         key = check(key)
         if self.autopack and packing:
             try:
                 from safeserializer.compression import pack
             except ModuleNotFoundError:
                 raise Exception(
                     "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
                 )
             value = pack(value, ensure_determinism=self.stablepack, unsafe_fallback=not self.safepack)
         elif isinstance(value, str):
             value = value.encode()
-        with self.sessionctx() as session:
+
+        def f(session):
             if self.ondup == "overwrite":
                 session.query(Content).filter_by(id=key).delete()
             if self.ondup == "stop" or session.query(Content).filter_by(id=key).first() is None:
                 content = Content(id=key, blob=value)
                 session.add(content)
             session.commit()
 
+        self.ensure_build(f)
+
     def update(self, dic, packing=True):
-        with self.sessionctx() as session:
+        def f(session):
             for k, v in dic.items():
                 k = check(k)
                 if self.autopack and packing:
                     try:
                         from safeserializer.compression import pack
                     except ModuleNotFoundError:
                         raise Exception(
@@ -172,48 +176,54 @@
                     v = v.encode()
 
                 if self.ondup == "overwrite":
                     session.query(Content).filter_by(id=k).delete()
                 if self.ondup == "stop" or session.query(Content).filter_by(id=k).first() is None:
                     content = Content(id=k, blob=v)
                     session.add(content)
-
             session.commit()
 
+        self.ensure_build(f)
+
     def __getitem__(self, key, packing=True):
         key = check(key)
-        with self.sessionctx() as session:
+
+        def f(session):
             if ret := session.query(Content).get(key):
                 if ret is not None:
                     ret = ret.blob
                     if self.autopack and packing:
                         try:
                             from safeserializer.compression import unpack
                         except ModuleNotFoundError:
                             raise Exception(
                                 "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
                             )
                         ret = unpack(ret)
-        return ret
+            return ret
+
+        return self.ensure_build(f)
 
     def __delitem__(self, key):
         key = check(key)
-        with self.sessionctx() as session:
+
+        def f(session):
             session.query(Content).filter_by(id=key).delete()
             session.commit()
 
+        self.ensure_build(f)
+
     def __getattr__(self, key):
         key_ = check(key)
         if key_ in self:
             return self[key_]
         return self.__getattribute__(key)
 
     def __len__(self):
-        with self.sessionctx() as session:
-            return session.query(Content).count()
+        return self.ensure_build(lambda session: session.query(Content).count())
 
     def __repr__(self):
         return repr(self.asdict)
 
     def __str__(self):
         return repr(self)
```

### Comparing `shelchemy-0.220906.5/src/shelchemy/lazy.py` & `shelchemy-1.230706.1/src/shelchemy/lazy.py`

 * *Files identical despite different names*

### Comparing `shelchemy-0.220906.5/src/shelchemy/locker.py` & `shelchemy-1.230706.1/src/shelchemy/locker.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 def alive(val, timeout):
     try:
         return timeout is not None and datetime.now() < unpackb(val).datetime() + timedelta(seconds=timeout)
     except Exception as e:
         print(val)
         print(unpackb(val))
-        raise e
+        raise e from None
 
 
 def locker(iterable, dict__url=None, timeout=None, logstep=1):
     """
     Generator that skips already processed (or still being processed) items from 'iterable'
 
     Item processing is restarted if 'timeout' expires.
```

### Comparing `shelchemy-0.220906.5/src/shelchemy/scheduler.py` & `shelchemy-1.230706.1/src/shelchemy/scheduler.py`

 * *Files identical despite different names*

### Comparing `shelchemy-0.220906.5/setup.py` & `shelchemy-1.230706.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 ['SQLAlchemy>=1.4.39,<2.0.0', 'temporenc>=0.1.0,<0.2.0']
 
 extras_require = \
 {'full': ['lz4>=4.0.2,<5.0.0', 'safeserializer>=0.230202.1,<0.230203.0']}
 
 setup_kwargs = {
     'name': 'shelchemy',
-    'version': '0.220906.5',
-    'description': 'Shelve-like dict using sqlachemy as backend, and lazy scheduler for resuming tasks',
+    'version': '1.230706.1',
+    'description': 'Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks',
     'long_description': '![test](https://github.com/shelchemy/shelchemy/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/shelchemy/shelchemy/branch/main/graph/badge.svg)](https://codecov.io/gh/shelchemy/shelchemy)\n<a href="https://pypi.org/project/shelchemy">\n<img src="https://img.shields.io/github/v/release/shelchemy/shelchemy?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://shelchemy.github.io/shelchemy)\n[![Downloads](https://static.pepy.tech/badge/shelchemy)](https://pepy.tech/project/shelchemy)\n\n# shelchemy - Dict-like (shelve-like) storage wrapper for any DBMS (SQLAlchemy)\n \n\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install shelchemy\n```\n\n### from source\n```bash\ngit clone https://github.com/shelchemy/shelchemy\ncd shelchemy\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['shelchemy'] package_data = \ {'': ['*']} install_requires
 = \ ['SQLAlchemy>=1.4.39,<2.0.0', 'temporenc>=0.1.0,<0.2.0'] extras_require = \
 {'full': ['lz4>=4.0.2,<5.0.0', 'safeserializer>=0.230202.1,<0.230203.0']}
-setup_kwargs = { 'name': 'shelchemy', 'version': '0.220906.5', 'description':
-'Shelve-like dict using sqlachemy as backend, and lazy scheduler for resuming
-tasks', 'long_description': '![test](https://github.com/shelchemy/shelchemy/
-workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/shelchemy/
-shelchemy/branch/main/graph/badge.svg)](https://codecov.io/gh/shelchemy/
-shelchemy)\n\n[github]\n\n![Python version](https://img.shields.io/badge/
-python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/
-badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![API
-documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)]
-(https://shelchemy.github.io/shelchemy)\n[![Downloads](https://
-static.pepy.tech/badge/shelchemy)](https://pepy.tech/project/shelchemy)\n\n#
-shelchemy - Dict-like (shelve-like) storage wrapper for any DBMS (SQLAlchemy)\n
-\n\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv.
-\npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip
-install shelchemy\n```\n\n### from source\n```bash\ngit clone https://
-github.com/shelchemy/shelchemy\ncd shelchemy\npoetry install\n```\n\n###
-Examples\nSome usage examples.\n\n\n## Grants\nThis work was partially
-supported by Fapesp under supervision of\nProf. AndrÃ© C. P. L. F. de Carvalho
-at CEPID-CeMEAI (Grants 2013/07375-0 â 2019/01735-0).\n', 'author': 'davips',
-'author_email': 'dpsabc@gmail.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+setup_kwargs = { 'name': 'shelchemy', 'version': '1.230706.1', 'description':
+'Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for
+resuming tasks', 'long_description': '![test](https://github.com/shelchemy/
+shelchemy/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/
+shelchemy/shelchemy/branch/main/graph/badge.svg)](https://codecov.io/gh/
+shelchemy/shelchemy)\n\n[github]\n\n![Python version](https://img.shields.io/
+badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0)\n\n[![API documentation](https://img.shields.io/badge/doc-
+API%20%28auto%29-a0a0a0.svg)](https://shelchemy.github.io/shelchemy)\n[!
+[Downloads](https://static.pepy.tech/badge/shelchemy)](https://pepy.tech/
+project/shelchemy)\n\n# shelchemy - Dict-like (shelve-like) storage wrapper for
+any DBMS (SQLAlchemy)\n \n\n\n## Python installation\n### from
+package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/
+bin/activate\n\n# Install from PyPI\npip install shelchemy\n```\n\n### from
+source\n```bash\ngit clone https://github.com/shelchemy/shelchemy\ncd
+shelchemy\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n\n##
+Grants\nThis work was partially supported by Fapesp under supervision of\nProf.
+AndrÃ© C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 â 2019/
+01735-0).\n', 'author': 'davips', 'author_email': 'dpsabc@gmail.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'package_dir':
+package_dir, 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'extras_require': extras_require,
+'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `shelchemy-0.220906.5/PKG-INFO` & `shelchemy-1.230706.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shelchemy
-Version: 0.220906.5
-Summary: Shelve-like dict using sqlachemy as backend, and lazy scheduler for resuming tasks
+Version: 1.230706.1
+Summary: Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks
 License: GPL
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: shelchemy Version: 0.220906.5 Summary: Shelve-like
-dict using sqlachemy as backend, and lazy scheduler for resuming tasks License:
-GPL Author: davips Author-email: dpsabc@gmail.com Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Provides-Extra: full
+Metadata-Version: 2.1 Name: shelchemy Version: 1.230706.1 Summary: Shelve-like
+dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks
+License: GPL Author: davips Author-email: dpsabc@gmail.com Requires-Python:
+>=3.10,<4.0 Classifier: License :: Other/Proprietary License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: full
 Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0) Requires-Dist: lz4 (>=4.0.2,<5.0.0)
 ; extra == "full" Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ;
 extra == "full" Requires-Dist: temporenc (>=0.1.0,<0.2.0) Description-Content-
 Type: text/markdown ![test](https://github.com/shelchemy/shelchemy/workflows/
 test/badge.svg) [![codecov](https://codecov.io/gh/shelchemy/shelchemy/branch/
 main/graph/badge.svg)](https://codecov.io/gh/shelchemy/shelchemy) [github] !
 [Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
```

