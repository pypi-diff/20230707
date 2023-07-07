# Comparing `tmp/sphinx-readme-0.0.1b4.tar.gz` & `tmp/sphinx-readme-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1b4.tar", last modified: Fri Jul  7 11:11:42 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.1b5.tar", last modified: Fri Jul  7 11:54:23 2023, max compression
```

## Comparing `sphinx-readme-0.0.1b4.tar` & `sphinx-readme-0.0.1b5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:11:42.283894 sphinx-readme-0.0.1b4/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b4/LICENSE
--rw-rw-rw-   0        0        0     8606 2023-07-07 11:11:42.283894 sphinx-readme-0.0.1b4/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2023-07-07 11:11:16.000000 sphinx-readme-0.0.1b4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-07 11:11:42.283894 sphinx-readme-0.0.1b4/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-07 11:05:51.000000 sphinx-readme-0.0.1b4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:11:42.252649 sphinx-readme-0.0.1b4/sphinx_readme/
--rw-rw-rw-   0        0        0     1598 2023-07-07 11:06:11.000000 sphinx-readme-0.0.1b4/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:11:42.283894 sphinx-readme-0.0.1b4/sphinx_readme/config/
--rw-rw-rw-   0        0        0      136 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b4/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     6890 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b4/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0     8198 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b4/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    20933 2023-07-07 11:05:51.000000 sphinx-readme-0.0.1b4/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     4878 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b4/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:11:42.283894 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     8606 2023-07-07 11:11:42.000000 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-07 11:11:42.000000 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:11:42.000000 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 11:11:42.000000 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 11:11:42.000000 sphinx-readme-0.0.1b4/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b5/LICENSE
+-rw-rw-rw-   0        0        0     8624 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/PKG-INFO
+-rw-rw-rw-   0        0        0     7833 2023-07-07 11:54:04.000000 sphinx-readme-0.0.1b5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-07 11:49:24.000000 sphinx-readme-0.0.1b5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.524503 sphinx-readme-0.0.1b5/sphinx_readme/
+-rw-rw-rw-   0        0        0     1598 2023-07-07 11:50:39.000000 sphinx-readme-0.0.1b5/sphinx_readme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/sphinx_readme/config/
+-rw-rw-rw-   0        0        0      136 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/__init__.py
+-rw-rw-rw-   0        0        0     6890 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/linkcode.py
+-rw-rw-rw-   0        0        0     8198 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b5/sphinx_readme/config/main.py
+-rw-rw-rw-   0        0        0    21021 2023-07-07 11:49:24.000000 sphinx-readme-0.0.1b5/sphinx_readme/parser.py
+-rw-rw-rw-   0        0        0     4878 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b5/sphinx_readme/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:54:23.555747 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     8624 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 11:54:23.000000 sphinx-readme-0.0.1b5/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1b4/LICENSE` & `sphinx-readme-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b4/PKG-INFO` & `sphinx-readme-0.0.1b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: ⚠
 .. |caution| replace:: ⚠
 .. |danger| replace:: ☢
 .. |error| replace:: ❌
 .. |hint| replace:: 🧠
 .. |important| replace:: ‼
 .. |note| replace:: 📝
@@ -45,22 +45,25 @@
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/logo.png?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
    :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+   :align: center
    :width: 25%
 
+
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme/
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -72,16 +75,14 @@
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
     :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 
 
 |
-|
-
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
    :header: |default| What's Sphinx README?
@@ -98,15 +99,15 @@
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
 
 
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/demo/demo.gif?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
    :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
```

### Comparing `sphinx-readme-0.0.1b4/README.rst` & `sphinx-readme-0.0.1b5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: ⚠
 .. |caution| replace:: ⚠
 .. |danger| replace:: ☢
 .. |error| replace:: ❌
 .. |hint| replace:: 🧠
 .. |important| replace:: ‼
 .. |note| replace:: 📝
@@ -27,22 +27,25 @@
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/logo.png?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
    :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+   :align: center
    :width: 25%
 
+
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme/
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -54,16 +57,14 @@
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
     :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 
 
 |
-|
-
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
    :header: |default| What's Sphinx README?
@@ -80,15 +81,15 @@
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
 
 
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/demo/demo.gif?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
    :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
```

### Comparing `sphinx-readme-0.0.1b4/setup.py` & `sphinx-readme-0.0.1b5/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme/__init__.py` & `sphinx-readme-0.0.1b5/sphinx_readme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_readme.utils import get_conf_val, set_conf_val
 from sphinx_readme.config import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1b4"
+__version__ = "v0.0.1b5"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     app.connect('env-check-consistency', parse_titles)
     app.connect('doctree-resolved', parse_references)
     app.connect('build-finished', resolve_readme)
```

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme/config/linkcode.py` & `sphinx-readme-0.0.1b5/sphinx_readme/config/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme/config/main.py` & `sphinx-readme-0.0.1b5/sphinx_readme/config/main.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme/parser.py` & `sphinx-readme-0.0.1b5/sphinx_readme/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,46 +367,47 @@
            value of :confval:`readme_docs_url_type`
 
         :param rst_src: absolute path of the rst file being parsed
         :param rst: the content of the rst file being parsed
         """
         src_dir = self.config.src_dir
         repo_dir = self.config.repo_dir
+        relpath_to_src_dir = src_dir.relative_to(repo_dir)
         rst_src_dir = Path(rst_src).parent
         blob_url = self.config.blob_url
 
-        # These image paths are relative to the rst source file
-        # .. image:: image.png || .. image:: images/image.png || .. image:: ../images/image.png
-        relative = r"\.\. image:: ([^/][./\w-]+\.\w{3,4})"
-        img_paths = re.findall(relative, rst)
+        # Find the targets of all image directives
+        img_pattern = r"\.\. image:: ([./\w-]+\.\w{3,4})"
+        img_paths = re.findall(img_pattern, rst)
 
         for img_path in img_paths:
-            # Find absolute path of the image
-            abs_img_path = (rst_src_dir / Path(img_path)).resolve()
-
-            # Find path of image relative to the output directory
-            rel_img_path = abs_img_path.relative_to(repo_dir).as_posix()
+            if img_path.startswith("/"):
+                # These image paths are "absolute" (relative to src_dir)
+                # .. image:: /path/to/image.ext
+                path_to_img = (relpath_to_src_dir / Path(img_path)).as_posix()
+
+            else:
+                # These image paths are relative to the rst source file
+                # .. image:: image.png || .. image:: images/image.png || .. image:: ../images/image.png
+                abs_img_path = (rst_src_dir / Path(img_path)).resolve()
+
+                # Find path of image relative to the repo directory
+                path_to_img = abs_img_path.relative_to(repo_dir).as_posix()
+
+            # Use raw url for gifs
+            if img_path.endswith("gif"):
+                blob_url = blob_url.replace("blob", "raw")
 
             # Sub that hoe in!!!
             rst = re.sub(
                 pattern=rf"\.\. image:: {img_path}",
-                repl=fr".. image:: {blob_url}/{rel_img_path}?raw=True",
+                repl=fr".. image:: {blob_url}/{path_to_img}?raw=True",
                 string=rst
             )
-
-        # These image paths are "absolute" (relative to src_dir)
-        # .. image:: /path/to/image.ext
-        relpath_to_src_dir = src_dir.relative_to(repo_dir).as_posix()
-
-        # Replace all image paths starting with "/"
-        return re.sub(
-            pattern=r"\.\. image:: (/[\w/-]+\.\w{3,4})",
-            repl=fr".. image:: {blob_url}/{relpath_to_src_dir}\1?raw=True",
-            string=rst
-        )
+        return rst
 
     def replace_rst_rubrics(self, rst: str):
         heading_chars = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         rubric_pattern = r'\.\. rubric:: (.+?)(?=\n)'
 
         if heading := self.config.rubric_heading:
             if heading in heading_chars:
```

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme/utils.py` & `sphinx-readme-0.0.1b5/sphinx_readme/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b4/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.0.1b5/sphinx_readme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/sphinx_readme/parser.py#L124-L134
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/sphinx_readme/parser.py#L124-L134
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: ⚠
 .. |caution| replace:: ⚠
 .. |danger| replace:: ☢
 .. |error| replace:: ❌
 .. |hint| replace:: 🧠
 .. |important| replace:: ‼
 .. |note| replace:: 📝
@@ -45,22 +45,25 @@
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/logo.png?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b5/docs/source/_static/logo.png?raw=True
    :alt: Sphinx README: Generate reStructuredText files that render beautifully on GitHub, PyPi, GitLab, BitBucket
+   :align: center
    :width: 25%
 
+
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme/
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -72,16 +75,14 @@
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
     :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 
 
 |
-|
-
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
    :header: |default| What's Sphinx README?
@@ -98,15 +99,15 @@
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 
 
 
 
-.. image:: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b4/docs/source/_static/demo/demo.gif?raw=True
+.. image:: https://github.com/TDKorn/sphinx-readme/raw/v0.0.1b5/docs/source/_static/demo/demo.gif?raw=True
    :alt: Demonstration of sphinx-readme extension output on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
```

