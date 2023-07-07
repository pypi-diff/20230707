# Comparing `tmp/fs_code-0.3.tar.gz` & `tmp/fs_code-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_code-0.3.tar", max compression
+gzip compressed data, was "fs_code-0.3.1.tar", max compression
```

## Comparing `fs_code-0.3.tar` & `fs_code-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-07-03 19:04:20.909507 fs_code-0.3/LICENSE
--rw-r--r--   0        0        0     1657 2023-07-03 19:04:20.909507 fs_code-0.3/README.md
--rw-r--r--   0        0        0     2283 2023-07-03 19:04:20.910507 fs_code-0.3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/__init__.py
--rw-r--r--   0        0        0     3932 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/_core.py
--rw-r--r--   0        0        0     4015 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitfs/__init__.py
--rw-r--r--   0        0        0      723 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitfs/opener.py
--rw-r--r--   0        0        0     4566 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/githubfs/__init__.py
--rw-r--r--   0        0        0     2402 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/githubfs/opener.py
--rw-r--r--   0        0        0     4855 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitlabfs/__init__.py
--rw-r--r--   0        0        0     2697 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitlabfs/opener.py
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 fs_code-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-07 15:19:13.645573 fs_code-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1657 2023-07-07 15:19:13.645573 fs_code-0.3.1/README.md
+-rw-r--r--   0        0        0     2285 2023-07-07 15:19:13.647573 fs_code-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/__init__.py
+-rw-r--r--   0        0        0     4647 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/_core.py
+-rw-r--r--   0        0        0     3953 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/gitfs/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/gitfs/opener.py
+-rw-r--r--   0        0        0     4566 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/githubfs/__init__.py
+-rw-r--r--   0        0        0     2402 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/githubfs/opener.py
+-rw-r--r--   0        0        0     4855 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/gitlabfs/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-07 15:19:13.647573 fs_code-0.3.1/src/codefs/gitlabfs/opener.py
+-rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 fs_code-0.3.1/PKG-INFO
```

### Comparing `fs_code-0.3/LICENSE` & `fs_code-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/README.md` & `fs_code-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/pyproject.toml` & `fs_code-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fs-code"
-version = "0.3"
+version = "0.3.1"
 description = "PyFilesystems for GitLab, GitHub, and Git"
 license = "MIT"
 authors = [
     "Max Ludwig <mail@danjou.dev>",
 ]
 readme = "README.md"
 homepage = "https://danjou.gitlab.io/fs-code"
```

### Comparing `fs_code-0.3/src/codefs/_core.py` & `fs_code-0.3.1/src/codefs/_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from pathlib import PurePosixPath
-from typing import TypeVar, Callable, Generic, Mapping, List, Tuple, Protocol, Union
+from typing import TypeVar, Callable, Generic, Mapping, List, Tuple, Protocol, Union, Iterator, Collection, Optional
 
 from fs.base import FS
 from fs.errors import ResourceNotFound
+from fs.info import Info
 from fs.memoryfs import MemoryFS
 from fs.mountfs import MountFS
 from fs.path import abspath, normpath
 from fs.subfs import SubFS
 from fs.wrap import read_only, WrapReadOnly
 from schema import And, Use  # type: ignore
 
@@ -72,21 +73,30 @@
                 self.mount(mount_point, read_only(RefFS(self.archive_fetcher(repo))))
         except Exception as e:
             logging.exception("failed to mount repo")
             raise ResourceNotFound(path, e)
         fs, path = super()._delegate(path)
         return fs, path
 
-    def listdir(self, path: str) -> List[str]:
+    def _mount_repos(self, path: str) -> None:
         if _is_root(path):
             repos: Mapping[str, Repository] = self.repos_fetcher.get_repos()
             for name, repo in repos.items():
                 self.mount(name, read_only(RefFS(self.archive_fetcher(repo))))
+
+    def listdir(self, path: str) -> List[str]:
+        self._mount_repos(path)
         return super().listdir(path)
 
+    def scandir(
+        self, path: str, namespaces: Optional[Collection[str]] = None, page: Optional[Tuple[int, int]] = None
+    ) -> Iterator[Info]:
+        self._mount_repos(path)
+        return super().scandir(path, namespaces, page)
+
 
 class RefFS(MountFS):
     def __init__(self, fetch_archive: AbstractArchiveFetcher) -> None:
         super().__init__()
         self.fetch_archive = fetch_archive
 
     def _reset(self) -> None:
@@ -108,14 +118,21 @@
         return fs, path
 
     def listdir(self, path: str) -> List[str]:
         if _is_root(path):
             return [self.fetch_archive.DEFAULT_BRANCH]
         return super().listdir(path)
 
+    def scandir(
+        self, path: str, namespaces: Optional[Collection[str]] = None, page: Optional[Tuple[int, int]] = None
+    ) -> Iterator[Info]:
+        if _is_root(path):
+            return iter([Info(dict(basic=dict(name=self.fetch_archive.DEFAULT_BRANCH, is_dir=True)))])
+        return super().scandir(path, namespaces, page)
+
 
 def Str() -> And:
     return And(str, len, error="must be non-empty string")
 
 
 def Float() -> Use:
     return Use(float)
```

### Comparing `fs_code-0.3/src/codefs/gitfs/__init__.py` & `fs_code-0.3.1/src/codefs/gitfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 """
 import logging
 from contextlib import closing
 from io import BytesIO
 from typing import Mapping, Optional, Tuple
 
 from dulwich import porcelain
-from dulwich.client import FetchPackResult, GitClient
+from dulwich.client import GitClient
 from dulwich.porcelain import NoneStream
 from dulwich.refs import LOCAL_BRANCH_PREFIX, LOCAL_TAG_PREFIX
-from dulwich.repo import MemoryRepo, Repo
+from dulwich.repo import Repo
 from fs.base import FS
-from fs.memoryfs import MemoryFS
 from fs.subfs import SubFS
 from fs.tarfs import ReadTarFS
 from fs.tempfs import TempFS
 from fs.wrap import read_only, WrapReadOnly
 
 from codefs._core import RefFS, AbstractArchiveFetcher
```

### Comparing `fs_code-0.3/src/codefs/gitfs/opener.py` & `fs_code-0.3.1/src/codefs/gitfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/src/codefs/githubfs/__init__.py` & `fs_code-0.3.1/src/codefs/githubfs/__init__.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/src/codefs/githubfs/opener.py` & `fs_code-0.3.1/src/codefs/githubfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/src/codefs/gitlabfs/__init__.py` & `fs_code-0.3.1/src/codefs/gitlabfs/__init__.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/src/codefs/gitlabfs/opener.py` & `fs_code-0.3.1/src/codefs/gitlabfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.3/PKG-INFO` & `fs_code-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-code
-Version: 0.3
+Version: 0.3.1
 Summary: PyFilesystems for GitLab, GitHub, and Git
 Home-page: https://danjou.gitlab.io/fs-code
 License: MIT
 Author: Max Ludwig
 Author-email: mail@danjou.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

