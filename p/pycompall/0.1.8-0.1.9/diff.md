# Comparing `tmp/pycompall-0.1.8.tar.gz` & `tmp/pycompall-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.8.tar", last modified: Thu Jul  6 09:39:33 2023, max compression
+gzip compressed data, was "pycompall-0.1.9.tar", last modified: Fri Jul  7 05:51:43 2023, max compression
```

## Comparing `pycompall-0.1.8.tar` & `pycompall-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.332432 pycompall-0.1.8/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.8/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.8/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:39:33.328432 pycompall-0.1.8/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.8/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.8/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.8/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4832 2023-07-06 09:39:26.000000 pycompall-0.1.8/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.8/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:39:33.332432 pycompall-0.1.8/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:39:32.000000 pycompall-0.1.8/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 09:22:05.000000 pycompall-0.1.8/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.9/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.9/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-07 05:51:43.376844 pycompall-0.1.9/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.9/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.9/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.9/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     6214 2023-07-07 05:46:21.000000 pycompall-0.1.9/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1379 2023-07-07 05:51:18.000000 pycompall-0.1.9/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-07 05:51:43.376844 pycompall-0.1.9/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-07 05:51:40.000000 pycompall-0.1.9/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     8978 2023-07-07 05:50:44.000000 pycompall-0.1.9/test/test_compile.py
```

### Comparing `pycompall-0.1.8/app/application.py` & `pycompall-0.1.9/app/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,130 @@
 from compileall import compile_file
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 
+PathPatterns = Tuple[str, ...]
 
-def compile_command(path: Path, recursive: bool = False, in_place: bool = False, create_empty_init: bool = False, exclude_patterns: Tuple[str] = tuple()):
-    click.echo(exclude_patterns)
-    if patterns_match_path(exclude_patterns, path):
+
+def compile_command(
+        path: Path,
+        recursive: bool = False,
+        in_place: bool = False,
+        create_empty_init: bool = False,
+        exclude_files: PathPatterns = tuple(),
+        exclude_dirs: PathPatterns = tuple()
+):
+    if is_matching_file(path, exclude_files):
         click.echo(f'Skipping file \'{path}\'')
         return
 
+    if is_matching_dir(path, exclude_dirs):
+        click.echo(f'Skipping directory \'{path}\'')
+        return
+
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
             f'--create-empty-init flag can only be used when path supplied is a directory, but got {path}.')
 
     _clear_pycache_dir(path, missing_ok=True)
-    compileall(path, recursive, exclude_patterns=exclude_patterns)
+    compileall(
+        path,
+        recursive,
+        exclude_files=exclude_files,
+        exclude_dirs=exclude_dirs
+    )
 
     if (in_place):
-        replace_py_with_pyc(path, recursive, exclude_patterns=exclude_patterns)
+        replace_py_with_pyc(path, recursive,
+                            exclude_files=exclude_files,
+                            exclude_dirs=exclude_dirs)
 
     if (create_empty_init):
         _create_init_file(dir=path)
 
 
-def compileall(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
+def compileall(path: Path, is_recursive: bool, exclude_files: PathPatterns, exclude_dirs: PathPatterns):
     """
     Simple wrapper around python compileall package to compile .py to .pyc files.
 
     Note that created .pyc files are under the __pycache__ directory.
     """
     assert (path.exists())
-    if (path.is_dir()):
-        if (not is_recursive):
-            for file in path.glob('*.py'):
-                compileall(file, is_recursive=is_recursive,
-                           exclude_patterns=exclude_patterns)
-            return
+    if (path.is_dir() and not is_recursive):
+        for file in path.glob('*.py'):
+            compileall(file, is_recursive=is_recursive,
+                       exclude_files=exclude_files,
+                       exclude_dirs=exclude_dirs)
+        return
 
+    if (path.is_dir() and is_recursive):
         for file in path.iterdir():
             compileall(file, is_recursive=is_recursive,
-                       exclude_patterns=exclude_patterns)
+                       exclude_files=exclude_files,
+                       exclude_dirs=exclude_dirs)
+        return
 
-    elif (path.is_file() and path.suffix == '.py'):
-        if patterns_match_path(exclude_patterns, path):
+    if (path.is_file() and path.suffix == '.py'):
+        if is_matching_file(path, exclude_files):
             click.echo(f'Skipping file \'{path}\'')
             return
 
         click.echo(f'Compiling file \'{path}\'')
         compile_file(path, quiet=1)
 
 
-def replace_py_with_pyc(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
+def replace_py_with_pyc(path: Path, is_recursive: bool, exclude_files: PathPatterns, exclude_dirs: PathPatterns):
     """Replace .py with .pyc files """
     assert (path.exists())
 
     if (path.is_dir()):
         _replace_py_with_pyc_dir(
-            path, is_recursive, exclude_patterns=exclude_patterns)
+            path, is_recursive,
+            exclude_files=exclude_files,
+            exclude_dirs=exclude_dirs)
+
     elif (path.is_file()):
         assert (path.suffix == '.py')
-        _replace_py_with_pyc_file(path, exclude_patterns=exclude_patterns)
+        _replace_py_with_pyc_file(path,
+                                  exclude_files=exclude_files,
+                                  exclude_dirs=exclude_dirs)
 
     _clear_pycache_dir(path, missing_ok=True)
 
 
-def _replace_py_with_pyc_dir(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
+def _replace_py_with_pyc_dir(path: Path, is_recursive: bool, exclude_files: PathPatterns, exclude_dirs: PathPatterns):
+    assert path.exists() and path.is_dir()
+
+    if (is_matching_dir(path, exclude_dirs)):
+        click.echo(f'Skipping directory \'{path}\'')
+        return
+
     for child in path.iterdir():
         if (child.is_dir() and is_recursive):
             _replace_py_with_pyc_dir(
-                child, is_recursive, exclude_patterns=exclude_patterns)
+                child, is_recursive,
+                exclude_files=exclude_files,
+                exclude_dirs=exclude_dirs)
             continue
 
         if (child.is_file() and child.suffix == '.py'):
-            _replace_py_with_pyc_file(child, exclude_patterns=exclude_patterns)
+            _replace_py_with_pyc_file(child,
+                                      exclude_files=exclude_files,
+                                      exclude_dirs=exclude_dirs)
             continue
 
 
-def _replace_py_with_pyc_file(python_file_path: Path, exclude_patterns: Tuple[str]):
+def _replace_py_with_pyc_file(python_file_path: Path, exclude_files: PathPatterns, exclude_dirs: PathPatterns):
     """Replace a .py file with its corresponding .pyc file in the __pycache__ directory."""
     assert (python_file_path.is_file() and python_file_path.suffix == '.py')
-    if patterns_match_path(exclude_patterns, python_file_path):
+
+    if is_matching_file(python_file_path, exclude_files):
+        click.echo(f'Skipping file \'{python_file_path}\'')
         return
 
     compiled_file = _get_pycache_pyc_from_py(python_file_path)
     if (compiled_file is None):
         raise FileNotFoundError(
             f'.pyc file does not exist for the file {python_file_path.as_posix()}')
     python_file_path.unlink()
@@ -105,14 +144,15 @@
     return compiled_file
 
 
 def _create_init_file(dir: Path) -> Path:
     """For a given directory, create an empty __init__.py file and return the resulting file as a Path object."""
     assert dir.is_dir()
     file = (dir / '__init__.py')
+    click.echo(f'Creating init file at {file.as_posix()}')
     file.touch()
     return file
 
 
 def _clear_pycache_dir(path: Path, missing_ok: bool) -> None:
     """Given a directory or file, delete the __pycache__ folder."""
     if (path.is_file()):
@@ -131,12 +171,20 @@
             rmtree(p, missing_ok=missing_ok)
         else:
             p.unlink(missing_ok=True)
 
     root.rmdir()
 
 
-def patterns_match_path(patterns: Tuple[str], path: Path):
+def is_matching_file(path: Path, patterns: PathPatterns):
+    return path.is_file() and path.suffix == '.py' and patterns_match_path(patterns, path)
+
+
+def is_matching_dir(path: Path, patterns: PathPatterns):
+    return path.is_dir() and patterns_match_path(patterns, path)
+
+
+def patterns_match_path(patterns: PathPatterns, path: Path):
     for pattern in patterns:
         if (path.match(pattern)):
             return True
     return False
```

### Comparing `pycompall-0.1.8/pycompall.py` & `pycompall-0.1.9/pycompall.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     pass
 
 
 @cli.command()
 @click.option('-recursive', '-r', is_flag=True, default=False, help='Recurse through subdirectories.')
 @click.option('--in-place', is_flag=True, default=False, help='Remove .py and replace them with compiled .pyc files.')
 @click.option('--create-empty-init', is_flag=True, default=False, help='Create an empty __init__.py file in the base directory path specified after compilation. Useful for interacting with tools such as colcon.')
-@click.option('--exclude', '-e', multiple=True, help='Exclude pattern(s) for files to be excluded during compilation and replacement.')
+@click.option('--exclude-files', multiple=True, help='Exclude pattern(s) for files to be excluded during compilation and replacement.')
+@click.option('--exclude-dirs', multiple=True, help='Exclude pattern(s) for directories to be excluded during compilation and replacement. If the direcoty is skipped and --create-empty-init is True, the __init__.py file will not be created.')
 @click.argument('paths', type=click.Path(exists=True), nargs=-1)
-def compile(paths, recursive, in_place, create_empty_init, exclude):
+def compile(paths, recursive, in_place, create_empty_init, exclude_files, exclude_dirs):
     for path in paths:
         compile_command(
             Path(path),
             recursive=recursive,
             in_place=in_place,
             create_empty_init=create_empty_init,
-            exclude_patterns=exclude
+            exclude_files=exclude_files,
+            exclude_dirs=exclude_dirs,
         )
```

### Comparing `pycompall-0.1.8/setup.py` & `pycompall-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.1.8',
+    version='0.1.9',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.1.8/test/test_compile.py` & `pycompall-0.1.9/test/test_compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,42 +81,42 @@
         dir, files = nested_py_file
         compile_command(files[0], recursive=False, in_place=False)
         expected_pycache_file = _get_pycache_pyc_from_py(files[0])
         unexpected_pycache_files = [
             _get_pycache_pyc_from_py(file) for file in files[1:]]
 
         assert files[0].exists()
-        assert expected_pycache_file.exists()
-        for i in range(1, len(files)):
-            assert files[i].exists()
-            assert unexpected_pycache_files[i - 1] is None or \
-                not unexpected_pycache_files[i - 1].exists()
+        assert expected_pycache_file is not None and expected_pycache_file.exists()
+        for file, unexpected_pycache_file in zip(files[1:], unexpected_pycache_files):
+            assert file.exists()
+            assert unexpected_pycache_file is None or \
+                not unexpected_pycache_file.exists()
 
     def test_compile_nested_by_dir_non_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (non-recursive), without replacing it."""
         dir, files = nested_py_file
         compile_command(dir, recursive=False, in_place=False)
         expected_pycache_files = [_get_pycache_pyc_from_py(
             file) for file in dir.glob('*.py')]
         for file in files:
             assert file.exists()
-        for file in expected_pycache_files:
-            assert file.exists()
+        for pycache_file in expected_pycache_files:
+            assert pycache_file is not None and pycache_file.exists()
 
     def test_compile_nested_by_dir_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (recursive), without replacing it."""
         dir, files = nested_py_file
         compile_command(dir, recursive=True, in_place=False)
         expected_pycache_files = [_get_pycache_pyc_from_py(
             file) for file in files]
 
         for file in files:
             assert file.exists()
-        for file in expected_pycache_files:
-            assert file.exists()
+        for pycache_file in expected_pycache_files:
+            assert pycache_file is not None and pycache_file.exists()
 
     def test_compile_nested_by_dir_non_recursive_in_place(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (non-recursive), replacing it."""
         dir, files = nested_py_file
         expected_compiled_files = list(dir.glob('*.py'))
         compile_command(dir, recursive=False, in_place=True)
 
@@ -144,37 +144,82 @@
             compile_command(file, create_empty_init=True)
 
     def test_create_empty_init(self, one_py_file: Tuple[Path, Path]):
         dir, file = one_py_file
         compile_command(dir, create_empty_init=True)
 
         assert file.exists()
-        assert _get_pycache_pyc_from_py(file).exists()
+        expected_pycache_file = _get_pycache_pyc_from_py(file)
+        assert expected_pycache_file is not None and expected_pycache_file.exists()
         assert (dir / '__init__.py').exists()
 
 
-class TestExcludePattern:
+class TestExcludeFilePattern:
     def test_exclude_all_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         pattern = '*.py'
         compile_command(dir, recursive=True, in_place=True,
-                        exclude_patterns=(pattern,))
+                        exclude_files=(pattern,))
         for file in files:
             if (file.match(pattern)):
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
             else:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
 
     def test_exclude_one_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         pattern = 'one.py'
         compile_command(dir, recursive=True, in_place=True,
-                        exclude_patterns=(pattern,))
+                        exclude_files=(pattern,))
         for file in files:
             if (file.match(pattern)):
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
             else:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
+
+
+class TestExcludeDirPattern:
+    def test_exclude_all_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
+        dir, files = nested_py_file
+        pattern = '*'
+        compile_command(dir, recursive=True, in_place=True, create_empty_init=True,
+                        exclude_dirs=(pattern,))
+        for file in files:
+            dir = file.parent
+            init_file = dir / '__init__.py'
+            assert not init_file.exists()
+            assert file.exists()
+            assert not file.with_suffix('.pyc').exists()
+
+    def test_exclude_one_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
+        dir, files = nested_py_file
+        print(dir)
+        pattern = 'two'
+        compile_command(dir, recursive=True, in_place=True, create_empty_init=True,
+                        exclude_dirs=(pattern,))
+        for file in files:
+            if 'two' in str(file):
+                assert file.exists()
+                assert not file.with_suffix('.pyc').exists()
+            else:
+                assert not file.exists()
+                assert file.with_suffix('.pyc').exists()
+
+        init_file = dir / '__init__.py'
+        assert init_file.exists()
+
+    def test_exclude_base_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
+        dir, files = nested_py_file
+        print(dir)
+        pattern = 'temp'
+        compile_command(dir, recursive=True, in_place=True,
+                        exclude_dirs=(pattern,))
+        for file in files:
+            assert file.exists()
+            assert not file.with_suffix('.pyc').exists()
+
+        init_file = dir / '__init__.py'
+        assert not init_file.exists()
```

