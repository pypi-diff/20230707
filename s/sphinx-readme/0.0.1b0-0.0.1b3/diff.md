# Comparing `tmp/sphinx-readme-0.0.1b0.tar.gz` & `tmp/sphinx-readme-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1b0.tar", last modified: Wed Jun  7 16:15:52 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.1b3.tar", last modified: Fri Jul  7 10:56:43 2023, max compression
```

## Comparing `sphinx-readme-0.0.1b0.tar` & `sphinx-readme-0.0.1b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:15:52.810943 sphinx-readme-0.0.1b0/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b0/LICENSE
--rw-rw-rw-   0        0        0     6931 2023-06-07 16:15:52.810943 sphinx-readme-0.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     6189 2023-06-07 16:15:20.000000 sphinx-readme-0.0.1b0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-07 16:15:52.822567 sphinx-readme-0.0.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-06-07 14:46:55.000000 sphinx-readme-0.0.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:15:52.779701 sphinx-readme-0.0.1b0/sphinx_readme/
--rw-rw-rw-   0        0        0     1370 2023-06-07 14:46:55.000000 sphinx-readme-0.0.1b0/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:15:52.810943 sphinx-readme-0.0.1b0/sphinx_readme/config/
--rw-rw-rw-   0        0        0       94 2023-06-07 13:34:42.000000 sphinx-readme-0.0.1b0/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     5423 2023-06-07 13:34:42.000000 sphinx-readme-0.0.1b0/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0     4755 2023-06-07 14:08:34.000000 sphinx-readme-0.0.1b0/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    14740 2023-06-07 14:16:52.000000 sphinx-readme-0.0.1b0/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     3327 2023-06-07 14:08:34.000000 sphinx-readme-0.0.1b0/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:15:52.810943 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     6931 2023-06-07 16:15:52.000000 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-06-07 16:15:52.000000 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:15:52.000000 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 16:15:52.000000 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 16:15:52.000000 sphinx-readme-0.0.1b0/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 10:56:43.111156 sphinx-readme-0.0.1b3/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b3/LICENSE
+-rw-rw-rw-   0        0        0     8602 2023-07-07 10:56:43.111156 sphinx-readme-0.0.1b3/PKG-INFO
+-rw-rw-rw-   0        0        0     7811 2023-07-07 10:56:06.000000 sphinx-readme-0.0.1b3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:56:43.111156 sphinx-readme-0.0.1b3/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:56:43.095537 sphinx-readme-0.0.1b3/sphinx_readme/
+-rw-rw-rw-   0        0        0     1598 2023-07-07 10:50:48.000000 sphinx-readme-0.0.1b3/sphinx_readme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:56:43.111156 sphinx-readme-0.0.1b3/sphinx_readme/config/
+-rw-rw-rw-   0        0        0      136 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b3/sphinx_readme/config/__init__.py
+-rw-rw-rw-   0        0        0     6890 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b3/sphinx_readme/config/linkcode.py
+-rw-rw-rw-   0        0        0     8198 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b3/sphinx_readme/config/main.py
+-rw-rw-rw-   0        0        0    20906 2023-07-07 10:19:59.000000 sphinx-readme-0.0.1b3/sphinx_readme/parser.py
+-rw-rw-rw-   0        0        0     4878 2023-07-07 10:50:47.000000 sphinx-readme-0.0.1b3/sphinx_readme/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:56:43.111156 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     8602 2023-07-07 10:56:43.000000 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-07 10:56:43.000000 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:56:43.000000 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 10:56:43.000000 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 10:56:43.000000 sphinx-readme-0.0.1b3/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1b0/LICENSE` & `sphinx-readme-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b0/setup.py` & `sphinx-readme-0.0.1b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,24 +15,24 @@
         if line.startswith("__version__ ="):
             return line.split(" = ")[-1].strip('"')
 
 
 setup(
     name="sphinx-readme",
     version=get_version(),
-    description="Generate Pretty README.rst for GitHub, PyPi, GitLab",
+    description="Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket",
     long_description=read(LONG_DESCRIPTION_SRC),
     long_description_content_type="text/x-rst; charset=UTF-8",
     author="Adam Korn",
     author_email='hello@dailykitten.net',
     license="MIT License",
     packages=find_packages(),
     keywords=[
-        "sphinx", "sphinx-extension", "sphinx-contrib", "reStructuredText", "rst",
-        "reST-parser", "rst-parser", "README.rst", "README", "autodoc"
+        "sphinx", "docutils", "sphinx-extension", "sphinx-contrib", "reStructuredText", "rst",
+        "reST", "parser", "rst-parser", "README.rst", "README", "autodoc", "linkcode"
     ],
     url="https://github.com/tdkorn/sphinx-readme",
     download_url="https://github.com/TDKorn/sphinx-readme/tarball/main",
     classifiers=[
         "Framework :: Sphinx :: Extension",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `sphinx-readme-0.0.1b0/sphinx_readme/__init__.py` & `sphinx-readme-0.0.1b3/sphinx_readme/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import sphinx
 from pathlib import Path
 from typing import Dict, Any
-from docutils.nodes import Node
+from docutils.nodes import document
 from sphinx.application import Sphinx
+from sphinx.environment import BuildEnvironment
 from sphinx_readme.utils import get_conf_val, set_conf_val
+from sphinx_readme.config import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1b0"
+__version__ = "v0.0.1b3"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
+    app.connect('env-check-consistency', parse_titles)
     app.connect('doctree-resolved', parse_references)
     app.connect('build-finished', resolve_readme)
 
     app.add_config_value("readme_inline_markup", True, True)
     app.add_config_value("readme_raw_directive", True, True)
     app.add_config_value("readme_include_directive", True, True)
     app.add_config_value("readme_replace_attrs", True, True)
-    app.add_config_value("readme_out_dir", Path(app.srcdir).parent.parent, True)
-    app.add_config_value("readme_linkcode_blob", 'head', True)
-    app.add_config_value("readme_default_admonition_icon", "ℹ", True)
+    app.add_config_value("readme_out_dir", get_repo_dir(), True)
+    app.add_config_value("readme_blob", 'head', True)
+    app.add_config_value("readme_default_admonition_icon", "📄", True)
 
     set_conf_val(app, 'READMEParser', READMEParser(app))
 
-    app.setup_extension('sphinx.ext.linkcode')
-
     return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
 
 
-def parse_references(app: Sphinx, doctree: Node, docname: str):
+def parse_titles(app: Sphinx, env: BuildEnvironment):
+    readme = get_conf_val(app, 'READMEParser')
+    readme.parse_titles(env)
+
+
+def parse_references(app: Sphinx, doctree: document, docname: str):
     readme = get_conf_val(app, 'READMEParser')
-    readme.parse(doctree, docname)
+    readme.parse(app, doctree, docname)
 
 
 def resolve_readme(app: Sphinx, exception):
     readme = get_conf_val(app, 'READMEParser')
     readme.resolve()
```

### Comparing `sphinx-readme-0.0.1b0/sphinx_readme/parser.py` & `sphinx-readme-0.0.1b3/sphinx_readme/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,195 @@
-import os
 import re
+from copy import copy
 from pathlib import Path
+from collections import defaultdict
 from typing import Dict, List, Tuple, Set
 
 from docutils import nodes
-from docutils.nodes import Node
+from docutils.nodes import Node, document
+
+from sphinx import addnodes
 from sphinx.application import Sphinx
+from sphinx.testing import restructuredtext
+from sphinx.transforms import SphinxTransformer
+from sphinx.environment import BuildEnvironment
 
 from sphinx_readme.config import READMEConfig
-from sphinx_readme.utils import get_all_variants
+from sphinx_readme.utils import get_all_variants, escape_rst, format_rst
 
 
 class READMEParser:
 
     def __init__(self, app: Sphinx):
         self.config = READMEConfig(app)
         self.logger = self.config.logger
         self.ref_map = self.config.ref_map
-        self.sources = self.config.readme_sources
+        self.sources = self.config.source_files
+        self.toctrees = defaultdict(list)
         self.admonitions = {}
+        self.titles = {}
 
-    def parse(self, doctree: Node, docname: str):
-        for node in list(doctree.findall(nodes.inline)):
-            if 'doc' in node['classes']:
-                self.ref_map['doc'].append(self.get_cross_ref_target(node))
+    def parse(self, app: Sphinx, doctree: document, docname: str):
+        # If a source has ``only`` directives, its doctree will have missing/extra content
+        # Replace the ``only`` directives, then generate a new doctree if needed
+        doctree = self.get_doctree(app, doctree, docname)
 
-            elif 'std-ref' in node['classes']:
-                self.ref_map['ref'].append(self.get_cross_ref_target(node))
+        inline_nodes = list(doctree.findall(nodes.inline))
+        literal_nodes = list(doctree.findall(nodes.literal))
 
-            elif 'viewcode-link' in node['classes'] or 'linkcode-link' in node['classes']:
-                if node.parent.get('internal') is False:
-                    self.parse_linkcode_node(node)
+        self.parse_autodoc_nodes(literal_nodes, docname)
+
+        if self.config.docs_url_type == "code":
+            self.parse_linkcode_nodes(inline_nodes)
 
-        if self.config.replace_attrs and self.config.docs_url_type == 'html':
-            for node in list(doctree.findall(nodes.reference)):
-                if ":attr:" in node.parent.rawsource:
-                    self.parse_attr_node(node)
+        for node in list(doctree.findall(addnodes.toctree)):
+            self.parse_toctree(node, doctree)
 
-        if doctree.get('source') in self.config.readme_sources:
+        if doctree.get('source') in self.sources:
+            self.parse_xref_nodes(inline_nodes)
             self.parse_admonitions(doctree)
 
-    def parse_linkcode_node(self, node: Node):
-        grandparent = node.parent.parent
-        is_method = grandparent.get("_toc_name", "").endswith("()")
+    def get_doctree(self, app: Sphinx, doctree: document, docname: str) -> document:
+        # Return original doctree if file is not a readme source
+        if (src := doctree.get('source')) not in self.sources:
+            return doctree
 
-        try:
-            qualified_name = grandparent.get("ids")[0]
-        except IndexError:
-            qualified_name = grandparent.get("module", "") + grandparent.get("fullname", "")
+        # Parse ``only`` directives to get true source rst of README version
+        parsed_rst = self.config.read_rst(src, replace_only=True)
+        raw_rst = self.sources[src]
 
-        if self.config.docs_url_type == "code":
-            target = node.parent.get("refuri")
-        else:
-            target = self.get_internal_target(node, qualified_name)
+        # Return original doctree if file had no ``only`` directives
+        if parsed_rst == raw_rst:
+            return doctree
 
-        self.add_variants(qualified_name, target, is_method)
+        self.sources[src] = parsed_rst
 
-    def parse_attr_node(self, node: Node):
+        # Use temp docname to avoid duplicate warnings
+        docname = docname + "_readme"
+
+        # Generate new doctree from parsed rst using Sphinx application
+        doctree = restructuredtext.parse(app, parsed_rst, docname)
+
+        # Resolve references in the doctree
         try:
-            child = node.children[0]
-        except (AttributeError, IndexError) as e:
-            return
+            backup = copy(app.env.temp_data)
+            app.env.temp_data['docname'] = docname
 
-        if not isinstance(child, nodes.literal):
-            return
+            transformer = SphinxTransformer(doctree)
+            transformer.set_environment(app.env)
+            transformer.add_transforms(app.registry.get_post_transforms())
+            transformer.apply_transforms()
+
+        finally:
+            app.env.temp_data = backup
+
+        # Replace temp source with actual source
+        doctree['source'] = src
+        return doctree
+
+    def parse_xref_nodes(self, inline_nodes: List[nodes.inline]):
+        for node in inline_nodes:
+            if 'doc' in node['classes']:
+                self.ref_map['doc'].append(self._parse_xref(node))
+
+            elif 'std-ref' in node['classes']:
+                self.ref_map['ref'].append(self._parse_xref(node))
+
+    def _parse_xref(self, node: nodes.inline) -> Dict:
+        """Helper function to parse target info of a ``:ref:`` or ``:doc:`` xref"""
+        return {
+            'text': node.children[0].astext(),
+            "refuri": self.config.html_baseurl + "/" + node.parent.get('refuri', '')
+        }
+
+    def parse_autodoc_nodes(self, literal_nodes: List[nodes.literal], docname: str):
+        for node in literal_nodes:
+            if 'py' not in node['classes']:
+                continue
+
+            if not isinstance(node.parent, nodes.reference):
+                continue
+
+            if node.parent.get('internal') is False:
+                # External links are xrefs from intersphinx
+                self.parse_intersphinx_node(node)
+
+            elif 'py-mod' in node['classes']:
+                # Parse :mod: xrefs regardless of docs_url_type
+                self.parse_module_node(node, docname)
+
+            elif self.config.docs_url_type == "html":
+                # Only parse remaining py xrefs if linking to html
+                self.parse_autodoc_node(node, docname)
+
+    def parse_intersphinx_node(self, node: nodes.literal):
+        pattern = r":(mod|class|meth|func|attr):`~?\.?[.\w]+`"
+        match = re.match(pattern, node.rawsource)
+        target = node.parent.get('refuri')
 
-        if 'py-attr' not in child.get('classes', []):
+        if not all((match, target)):
             return
 
-        refuri = node.get("refuri", '').lstrip('./')
-        qualified_name = node.get("reftitle")
+        is_method = match.group(1) == "meth"
+        qualified_name = target.split("#")[-1].split("-")[-1]
+        self.add_variants(qualified_name, target, is_method)
 
-        if not all((refuri, qualified_name)):
+    def parse_module_node(self, node: Node, docname: str):
+        qualified_name = node.parent.get("reftitle", "")
+
+        if self.config.docs_url_type == 'code':
+            # Ex. sphinx_readme.parser -> sphinx_readme/parser.py
+            refuri = qualified_name.replace('.', '/') + '.py'
+        else:
+            refuri = self._parse_refuri(node, docname)
+
+        if not all((qualified_name, refuri)):
             return
 
-        target = self.config.docs_url + "/" + refuri
+        target = f"{self.config.docs_url}/{refuri}"
         self.add_variants(qualified_name, target)
 
-    def parse_admonitions(self, doctree: Node):
-        admonitions = {'generic': [], 'specific': []}
-        src = doctree.get('source')
+    def parse_autodoc_node(self, node: nodes.literal, docname: str):
+        qualified_name = node.parent.get("reftitle")
+        refuri = self._parse_refuri(node, docname)
 
-        for admonition in list(doctree.findall(nodes.Admonition)):
-            info = {
-                'body': admonition.rawsource
-            }
-            if isinstance(admonition, nodes.admonition):
-                # Generic Admonition (using admonition directive)
-                info.update({
-                    'class': admonition.get('classes')[0],
-                    'title': admonition.children[0].rawsource
-                })
-                admonitions['generic'].append(info)
-            else:
-                # Specific Admonition (for example, .. note::)
-                info.update({
-                    'class': admonition.tagname,
-                    'title': admonition.tagname.title(),
-                })
-                admonitions['specific'].append(info)
+        if not all((refuri, qualified_name)):
+            return
 
-        self.admonitions[src] = admonitions
+        is_method = 'py-meth' in node['classes']
+        target = f"{self.config.docs_url}/{refuri}"
+        self.add_variants(qualified_name, target, is_method)
 
-    def get_cross_ref_target(self, node: Node) -> Dict:
-        """Helper function to parse target info of a :ref: or :doc: cross-reference"""
-        return {
-            'text': str(node.children[0]),
-            "refuri": self.config.docs_url + "/" + node.parent.get('refuri', '')
-        }
+    def _parse_refuri(self, node: Node, docname: str):
+        if 'refuri' in node.parent:
+            # Ex. ../parser.html#sphinx_readme.parser.READMEParser
+            return node.parent["refuri"].lstrip("./")
+
+        elif 'refid' in node.parent:
+            # Ex. sphinx_readme.parser.READMEParser
+            return f"{docname}.html#{node.parent['refid']}"
+
+    def parse_linkcode_nodes(self, inline_nodes: List[nodes.inline]):
+        for node in inline_nodes:
+            if 'viewcode-link' in node['classes'] or 'linkcode-link' in node['classes']:
+                if node.parent.get('internal') is False:
+                    # Only parse links to external source code
+                    self.parse_linkcode_node(node)
+
+    def parse_linkcode_node(self, node: nodes.inline):
+        grandparent = node.parent.parent
+        is_method = grandparent.get("_toc_name", "").endswith("()")
+
+        try:
+            qualified_name = grandparent.get("ids")[0]
+        except IndexError:
+            qualified_name = grandparent.get("module", "") + grandparent.get("fullname", "")
 
-    def get_internal_target(self, node: Node, qualified_name: str):
-        """Helper function to parse an internal target from a linkcode node"""
-        rst_source = os.path.basename(node.parent.document.get("source"))
-        html_file = rst_source.split(".rst")[0] + ".html"
-        return f"{self.config.docs_url}/{html_file}#{qualified_name}"
+        target = node.parent.get("refuri")
+        self.add_variants(qualified_name, target, is_method)
 
     def add_variants(self, qualified_name, target, is_method: bool = False):
         short_ref = qualified_name.split('.')[-1]
         variants = get_all_variants(qualified_name)
 
         for variant in variants:
             if variant in self.ref_map:
@@ -135,20 +207,72 @@
                 replace = f"``{replace}``"
 
             self.ref_map[variant].update({
                 'target': target,
                 'replace': replace
             })
 
+    def parse_titles(self, env: BuildEnvironment):
+        for fname, title_node in env.titles.items():
+            parts = []
+
+            for child in title_node.children:
+                text = child.astext()
+                if isinstance(child, nodes.literal):
+                    parts.append(f"``{text}``")
+                else:
+                    parts.append(text)
+
+            self.titles[fname] = ' '.join(parts)
+
+    def parse_toctree(self, toctree: Node, doctree: addnodes.document):
+        src = doctree.get('source')
+        toc = {
+            'caption': toctree.get('caption'),
+            'entries': []
+        }
+        for _, entry in toctree.get('entries', []):
+            toc['entries'].append({
+                'entry': entry,
+                'title': self.titles.get(entry),
+            })
+        self.toctrees[src].append(toc)
+
+    def parse_admonitions(self, doctree: Node):
+        admonitions = {'generic': [], 'specific': []}
+        src = doctree.get('source')
+
+        for admonition in list(doctree.findall(nodes.Admonition)):
+            info = {
+                'body': admonition.rawsource
+            }
+            if isinstance(admonition, nodes.admonition):
+                # Generic Admonition (using admonition directive)
+                info.update({
+                    'class': admonition.get('classes')[0],
+                    'title': admonition.children[0].rawsource
+                })
+                admonitions['generic'].append(info)
+            else:
+                # Specific Admonition (for example, .. note::)
+                info.update({
+                    'class': admonition.tagname,
+                    'title': admonition.tagname.title(),
+                })
+                admonitions['specific'].append(info)
+
+        self.admonitions[src] = admonitions
+
     def resolve(self):
         for src, rst in self.sources.items():
             # Replace everything using data from ``parse()``
             rst = self.replace_admonitions(src, rst)
             rst = self.replace_rst_images(src, rst)
-            rst = self.replace_only_directives(rst)
+            rst = self.replace_toctrees(src, rst)
+            rst = self.replace_rst_rubrics(rst)
 
             for role in ('ref', 'doc'):
                 rst = self.replace_cross_refs(rst, role)
 
             # Use ref_map to generate autodoc substitution definitions
             rst, autodoc_refs = self.replace_autodoc_refs(rst)
             header_vals = self.get_header_vals(autodoc_refs)
@@ -184,87 +308,127 @@
                                 title=admonition['title'],
                                 text=admonition['body'],
                                 icon=icon),
                             string=rst
                         )
         return rst
 
+    def replace_toctrees(self, rst_src: str, rst: str) -> str:
+        if self.config.docs_url_type == 'html':
+            base_url = self.config.docs_url
+        else:
+            base_url = self.config.html_baseurl
+
+        pattern = r".. toctree::\n+?(?:\s+:\w+:\s*?\w*?\n\s+)*?(?:\s+\w+\n)+?(?=\n+\S+?)"
+        toctrees = re.findall(pattern, rst)
+
+        for toctree, info in zip(toctrees, self.toctrees[rst_src]):
+            substitutions = []
+            repl = ""
+
+            if info['caption']:
+                repl += f"**{info['caption']}**\n\n"
+
+            for entry in info['entries']:
+                # Replace each entry with a link to html docs
+                target = f"{base_url}/{entry['entry']}.html"
+
+                if "`" in entry['title']:
+                    # Inline markup in links must be inserted with substitutions
+                    sub = entry['title'].replace('`', '')
+                    substitutions.extend([
+                        f".. |{sub}| replace:: {entry['title']}",
+                        f".. _{sub}: {target}"
+                    ])
+                    repl += f"* |{sub}|_\n"
+
+                else:
+                    # Replace with a normal link otherwise
+                    repl += f"* `{entry['title']} <{target}>`_\n"
+
+            if substitutions:
+                repl += '\n\n' + '\n'.join(substitutions) + '\n\n'
+
+            # Replace toctree directive with links and substitution defs
+            rst = rst.replace(toctree, repl)
+
+        return rst
+
     def replace_rst_images(self, rst_src: str, rst: str) -> str:
-        """Resolves filepaths of ``image`` directives to be relative to the ``readme_out_dir``
+        """Replaces filepaths in ``image`` directives with repository links
+
+        :Example:
+            :rst:`.. image:: /_static/logo.png`
+
+            would be replaced with
 
-            ".. image:: /blah/blah.png"
-            ".. image:: /blah.png"
-            ".. image:: blah.png"
-            ".. image:: blah/blah.png"
-            ".. image:: ../blah/blah.png"
+            :rst:`.. image:: https://github.com/tdkorn/sphinx-readme/blob/docs/docs/source/_static/logo.png`
 
-        :param rst_src: filename of the rst file being parsed
+        .. note:: Your repository will be used as the image source regardless of the
+           value of :confval:`readme_docs_url_type`
+
+        :param rst_src: absolute path of the rst file being parsed
         :param rst: the content of the rst file being parsed
-        :return: the rst file content with correct image directives
         """
-        src_dir_path = Path(self.config.src_dir)
-        out_dir_path = Path(self.config.out_dir)
-        rst_src_dir_path = Path(rst_src).parent
+        src_dir = self.config.src_dir
+        repo_dir = self.config.repo_dir
+        rst_src_dir = Path(rst_src).parent
+        blob_url = self.config.blob_url
 
         # These image paths are relative to the rst source file
         # .. image:: image.png || .. image:: images/image.png || .. image:: ../images/image.png
-        relative = r".. image:: ([\w\.]+[\w/]+\.\w{3,4})"
+        relative = r"\.\. image:: ([^/][./\w-]+\.\w{3,4})"
         img_paths = re.findall(relative, rst)
 
         for img_path in img_paths:
             # Find absolute path of the image
-            abs_img_path = (rst_src_dir_path / Path(img_path)).resolve()
+            abs_img_path = (rst_src_dir / Path(img_path)).resolve()
 
             # Find path of image relative to the output directory
-            rel_img_path = abs_img_path.relative_to(out_dir_path).as_posix()
+            rel_img_path = abs_img_path.relative_to(repo_dir).as_posix()
 
             # Sub that hoe in!!!
             rst = re.sub(
-                pattern=rf".. image:: {img_path}",
-                repl=fr".. image:: {rel_img_path}",
+                pattern=rf"\.\. image:: {img_path}",
+                repl=fr".. image:: {blob_url}/{rel_img_path}",
                 string=rst
             )
 
         # These image paths are "absolute" (relative to src_dir)
         # .. image:: /path/to/image.ext
-        relpath_to_src_dir = src_dir_path.relative_to(out_dir_path).as_posix()
+        relpath_to_src_dir = src_dir.relative_to(repo_dir).as_posix()
 
         # Replace all image paths starting with "/"
         return re.sub(
-            pattern=r".. image:: (/[\w/]+\.\w{3,4})",
-            repl=fr".. image:: {relpath_to_src_dir}\1",
+            pattern=r"\.\. image:: (/[\w/-]+\.\w{3,4})",
+            repl=fr".. image:: {blob_url}/{relpath_to_src_dir}\1",
             string=rst
         )
 
-    def replace_only_directives(self, rst: str) -> str:
-        # Match all ``only`` directives
-        pattern = r"\.\. only:: ([\w\s]+?)\n+?((?:^[ ]+[\w\W]+?\n)+?)(?=\n+?\S+?)"
-        directives = re.findall(pattern, rst, re.M)
-
-        for expression, content in directives:
-            # Match each block exactly
-            pattern = rf"\.\. only:: {expression}\n+?{content}"
-
-            if 'readme' in expression:
-                # Remove preceding indent (3 spaces) from each line
-                text = '\n\n'.join(line[3:] for line in content.split('\n\n'))
-
-                # Replace directive with content
-                rst = re.sub(pattern, rf"{text}", rst, re.M)
-
-            else:
-                # Remove directive
-                rst = re.sub(pattern, '', rst, re.M)
-
-        return rst
+    def replace_rst_rubrics(self, rst: str):
+        heading_chars = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
+        rubric_pattern = r'\.\. rubric:: (.+?)(?=\n)'
+
+        if heading := self.config.rubric_heading:
+            if heading in heading_chars:
+                return re.sub(
+                    pattern=rubric_pattern,
+                    repl=lambda m: f"{m.group(1)}\n{heading * len(m.group(1))}",
+                    string=rst
+                )
+        return re.sub(
+            pattern=rubric_pattern,
+            repl=lambda m: format_rst("bold", m.group(1)),
+            string=rst
+        )
 
     def replace_cross_refs(self, rst: str, ref_role: str) -> str:
         # Find all :ref_role:`ref_id` cross-refs
         cross_refs = re.findall(
-            pattern=fr":{ref_role}:`(.+)`",
+            pattern=fr"(?:\s*?):{ref_role}:`([^`]+)`(?=\s*?)",
             string=rst
         )
         # Match these ids up with target data in the ref_map
         cross_ref_map = dict(zip(cross_refs, self.ref_map[ref_role]))
 
         # Replace cross-refs with `text <link>`_ format
         for ref_id, target in cross_ref_map.items():
@@ -277,20 +441,20 @@
 
     def replace_autodoc_refs(self, rst: str) -> Tuple[str, Set]:
         """
         :param rst:
         :return:
         """
         # :role:`{~.}{module|class}{.}target` where {} is optional
-        pattern = r":(?:class|meth|func):`([~\.\w]+)`"
+        pattern = r":(?:mod|class|meth|func):`([~\.\w]+)`"
 
         if self.config.replace_attrs:
             if self.config.docs_url_type == 'html':
                 # If linking to HTML docs, we can generate cross-refs for attributes
-                pattern = r":(?:class|meth|func|attr):`([~\.\w]+)`"
+                pattern = r":(?:mod|class|meth|func|attr):`([~\.\w]+)`"
             else:
                 # If linking to source code, just replace :attr:`~.attribute` with ``attribute``
                 rst = self.replace_autodoc_attrs(rst)
 
         # To render on GitHub/PyPi/etc., we use Sphinx substitutions instead of cross-refs
         # Syntax is |.{ref}|_ or |.`{ref}`|_
         if self.config.inline_markup:
@@ -314,15 +478,15 @@
         long_ref = r" :attr:`\.?([\.\w]+)`"
         repl = r" ``\1``"
 
         rst = re.sub(short_ref, repl, rst)
         rst = re.sub(long_ref, repl, rst)
         return rst
 
-    def get_header_vals(self, autodoc_refs: Dict) -> List[str]:
+    def get_header_vals(self, autodoc_refs: Set) -> List[str]:
         header = []
 
         for ref in autodoc_refs:
             info = self.ref_map[ref]
 
             # Check for empty REFERENCE_MAPPING
             if not any(info.values()):
@@ -339,53 +503,50 @@
         if not self.config.raw_directive:
             for _type, icon in self.config.icon_map.items():
                 header.append(f'.. |{_type}| replace:: {icon}')
 
         return header
 
     def get_admonition_regex(self, admonition, admonition_type):
-        # Parse rawsource body to have same whitespace formatting as the rst file
-        lines = (line.replace('\n', '\n   ') for line in admonition['body'].split('\n\n'))
-        body = '\n\n   '.join(lines)
-        title = admonition['title']
-
-        for char in ("*", "+", ".", "?"):
-            body = body.replace(char, rf"\{char}")
-            title = title.replace(char, rf"\{char}")
+        body = escape_rst(admonition['body'])
+        title = escape_rst(admonition['title'])
+
+        # Account for arbitrary whitespace before each line of directive content
+        lines = (line.replace('\n', '\n\s+') for line in body.split('\n\n'))
+        body = '\n\n\s+'.join(lines)
 
         if admonition_type == 'specific':
             # For example, .. note:: This is a note
-            pattern = fr"\.\. {admonition['class']}::\n?\n?\s+"
+            pattern = fr"\.\. {admonition['class']}::\n*?\s+"
 
         else:
-            # Any admonition that uses generic .. admonition:: directive
+            # Generic admonition directives with/without class option
             pattern = rf"\.\. admonition::\s+{title}" + r"\n"
 
             if cls := admonition['class']:
                 if 'admonition-' not in cls:
                     pattern += rf"\s+:class: {cls}" + r"\n"
 
-            pattern += r"\n" + rf"\s+"
+            pattern += r"\n*?\s+"
 
         if not self.config.raw_directive:
             # csv-table template body uses match group
             pattern += rf"({body})"
         else:
             # raw html template body uses string formatting
             pattern += rf"{body}"
 
-        pattern += r"\n*?(\S+|$)"
+        pattern += r"(?=[\n\S]+?)"
         return pattern
 
     def get_admonition_icon(self, admonition: dict):
         icon = self.config.icon_map.get(admonition['class'])
 
         # Raw directive allows for using icon directly
         if self.config.raw_directive:
             return icon if icon else self.config.default_admonition_icon
 
         if icon:  # Without raw directive, must use substitution
             return f"|{admonition['class']}|"
 
         # Use default icon if admonition class isn't in icon map
         return "|default|"
-
```

