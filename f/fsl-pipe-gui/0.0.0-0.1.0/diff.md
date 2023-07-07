# Comparing `tmp/fsl-pipe-gui-0.0.0.tar.gz` & `tmp/fsl-pipe-gui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsl-pipe-gui-0.0.0.tar", last modified: Fri Jul  7 15:47:48 2023, max compression
+gzip compressed data, was "fsl-pipe-gui-0.1.0.tar", last modified: Fri Jul  7 16:51:11 2023, max compression
```

## Comparing `fsl-pipe-gui-0.0.0.tar` & `fsl-pipe-gui-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michielcottaar   (506) staff       (20)        0 2023-07-07 15:47:48.917257 fsl-pipe-gui-0.0.0/
--rw-r--r--   0 michielcottaar   (506) staff       (20)       18 2023-07-04 14:11:43.000000 fsl-pipe-gui-0.0.0/MANIFEST.in
--rw-r--r--   0 michielcottaar   (506) staff       (20)     2714 2023-07-07 15:47:48.917376 fsl-pipe-gui-0.0.0/PKG-INFO
--rw-r--r--   0 michielcottaar   (506) staff       (20)     2211 2023-07-04 14:11:43.000000 fsl-pipe-gui-0.0.0/README.md
--rw-r--r--   0 michielcottaar   (506) staff       (20)      396 2023-07-06 13:53:15.000000 fsl-pipe-gui-0.0.0/pyproject.toml
--rw-r--r--   0 michielcottaar   (506) staff       (20)     1006 2023-07-07 15:47:48.919119 fsl-pipe-gui-0.0.0/setup.cfg
-drwxr-xr-x   0 michielcottaar   (506) staff       (20)        0 2023-07-07 15:47:48.878142 fsl-pipe-gui-0.0.0/src/
-drwxr-xr-x   0 michielcottaar   (506) staff       (20)        0 2023-07-07 15:47:48.898928 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/
--rw-r--r--   0 michielcottaar   (506) staff       (20)      100 2023-07-06 12:41:53.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/__init__.py
--rw-r--r--   0 michielcottaar   (506) staff       (20)     3768 2023-07-07 13:19:11.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/all_panes.py
--rw-r--r--   0 michielcottaar   (506) staff       (20)     2133 2023-07-07 11:26:10.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/placeholder_tab.py
--rw-r--r--   0 michielcottaar   (506) staff       (20)     1546 2023-07-07 13:28:50.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/run.py
--rw-r--r--   0 michielcottaar   (506) staff       (20)     9895 2023-07-07 13:41:36.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/selector_tab.py
--rw-r--r--   0 michielcottaar   (506) staff       (20)     1199 2023-07-07 11:41:30.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/summary.py
-drwxr-xr-x   0 michielcottaar   (506) staff       (20)        0 2023-07-07 15:47:48.914491 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/
--rw-r--r--   0 michielcottaar   (506) staff       (20)     2714 2023-07-07 15:47:48.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/PKG-INFO
--rw-r--r--   0 michielcottaar   (506) staff       (20)      425 2023-07-07 15:47:48.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/SOURCES.txt
--rw-r--r--   0 michielcottaar   (506) staff       (20)        1 2023-07-07 15:47:48.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/dependency_links.txt
--rw-r--r--   0 michielcottaar   (506) staff       (20)       38 2023-07-07 15:47:48.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/requires.txt
--rw-r--r--   0 michielcottaar   (506) staff       (20)       13 2023-07-07 15:47:48.000000 fsl-pipe-gui-0.0.0/src/fsl_pipe_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:51:11.096946 fsl-pipe-gui-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-04 15:12:36.000000 fsl-pipe-gui-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-07-07 16:51:11.096946 fsl-pipe-gui-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-07 16:35:03.000000 fsl-pipe-gui-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-07-06 13:53:30.000000 fsl-pipe-gui-0.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-07-07 16:51:11.097946 fsl-pipe-gui-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:51:11.093946 fsl-pipe-gui-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:51:11.095946 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-07 16:46:35.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3872 2023-07-07 16:30:08.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/all_panes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2023-07-07 11:40:30.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/placeholder_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-07-07 13:52:45.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2023-07-07 16:30:08.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/selector_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-07 12:01:41.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:51:11.096946 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-07-07 16:51:11.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-07 16:51:11.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 16:51:11.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 16:51:11.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 16:51:11.000000 fsl-pipe-gui-0.1.0/src/fsl_pipe_gui.egg-info/top_level.txt
```

### Comparing `fsl-pipe-gui-0.0.0/README.md` & `fsl-pipe-gui-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,43 @@
+Metadata-Version: 2.1
+Name: fsl-pipe-gui
+Version: 0.1.0
+Summary: Terminal-based GUI for fsl-pipe
+Home-page: https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui
+Author: Michiel Cottaar
+Author-email: michiel.cottaar@ndcn.ox.ac.uk
+Project-URL: Bug Tracker, https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/issues
+Project-URL: Documentation, https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe-gui
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fsl-pipe-gui)](https://pypi.org/project/fsl-pipe-gui/)
-[![Documentation](https://img.shields.io/badge/Documentation-fsl-pipe-gui-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe-gui)
+[![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/pipelines/latest)
-[![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe-gui/htmlcov)
 
-terminal-based GUI for fsl-pipe
+Terminal-based GUI for fsl-pipe.
+It allows interactively choosing which subset of potential output files you want an fsl-pipe pipeline to produce.
 
 # Installation
 ```shell
-pip install git+https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui.git
+pip install fsl-pipe-gui
 ```
 
 Any bug reports and feature requests are very welcome (see [issue tracker](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/issues)).
 
-# Setting up local test environment
-First clone the repository:
-```shell
-pip install https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui.git
-```
-
-Then, we install the package in an interactive manner:
-```shell
-cd fsl-pipe-gui
-pip install -e .
-```
-
-Development tools can be installed using:
-```
-pip install -r requirements_dev.txt
-pre-commit install  # installs pre-commit hooks to keep the code clean
-```
-
-
-## Running tests
-Tests are run using the [pytest](https://docs.pytest.org) framework. They can be run from the project root as:
-```shell
-pytest src/tests
-```
-
-## Compiling documentation
-The documentation is build using [sphinx](https://www.sphinx-doc.org/en/master/). After installation (`pip install sphinx`) run:
-```shell
-cd doc
-sphinx-build source build
-open build/index.html
-```
-
-## Contributing
-[Merge requests](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/merge_requests) with any bug fixes or documentation updates are always welcome.
-
-For new features, please raise an [issue](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/issues) to allow for discussion before you spend the time implementing them.
-
-## Releasing new versions
-- Run `bump2version` (install using `pip install bump2version`)
-- Push to gitlab
-- Manually activate the "to_pypi" task in the [pipeline](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/pipelines/latest) to upload to pypi
+# Usage
+For any pipelines using the standard command line interface, the GUI will be available using the `-g/--gui` flag.
+Some pipelines might have customised this flag. Please check their documentation.
+
+When starting the GUI from your own custom python code, you will need:
+- a `file_tree` describing the paths of the input and output files (see [file-tree](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)).
+- a `pipeline` containing the recipes to produce the output from the input files (see [fsl-pipe](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)).
+The GUI can then be started using
+```python
+pipeline.gui(file_tree)
+```
+
+This GUI will consist of 3 parts, which will be presented to the user in sequence:
+1. An interactive table, where the default values for placeholders (e.g., subject or session id) can be overwritten.
+2. A visualisation of the `file_tree` on the left. For the template selected on the left, the matching filenames are shown on the right. If you want the pipeline to produce a specific file, simply click on the row to mark the checkbox. Files without a checkbox cannot be produced by this pipeline. If the checkbox has been replaced by an "M" then the file cannot be produced due to a missing input file. Filenames in blue already exist (but can be produced by the pipeline anyway if it has a checkbox).
+3. A summary of which files are requested and which jobs will actually be run. If the user confirms this summary then the pipeline will actually run.
```

### Comparing `fsl-pipe-gui-0.0.0/setup.cfg` & `fsl-pipe-gui-0.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [bumpversion]
-current_version = 0.0.0
+current_version = 0.1.0
 commit = True
 tag = True
 
 [bumpversion:file:src/fsl_pipe_gui/__init__.py]
-search = __version__ = '{current_version}'
-replace = __version__ = '{new_version}'
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
 
 [metadata]
 name = fsl-pipe-gui
 version = attr: fsl_pipe_gui.__version__
 author = Michiel Cottaar
 author_email = michiel.cottaar@ndcn.ox.ac.uk
-description = terminal-based GUI for fsl-pipe
+description = Terminal-based GUI for fsl-pipe
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui
 project_urls = 
 	Bug Tracker = https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-gui/-/issues
 	Documentation = https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe-gui
 classifiers =
```

### Comparing `fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/all_panes.py` & `fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/all_panes.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,25 @@
         self,
         pipeline: Pipeline,
         file_tree: FileTree,
         overwrite_dependencies=False,
         run_method=None,
     ):
         """Create new pipeline selector to be edited in GUI."""
+        self.file_tree = file_tree
         all_templates = file_tree.template_keys()
         templates = {
             elem
             for piped_function in pipeline.scripts
             for elem in set.union(
                 piped_function.filter_templates(False, all_templates),
                 piped_function.filter_templates(True, all_templates),
             )
         }
-        self.file_tree = file_tree.filter_templates(templates)
+        self.partial_tree = file_tree.filter_templates(templates)
         self.pipeline = pipeline
         self.full_job_list = self.pipeline.generate_jobs(self.file_tree)
         self.selected_files = set()
         self.all_jobs = ([], set())
 
         self._overwrite_dependencies = overwrite_dependencies
         if run_method is None:
@@ -71,14 +72,15 @@
     def get_file_targets(self, path) -> FileTarget:
         """Return file target corresponding to path."""
         return get_target(path, self.full_job_list.targets)
 
     def update_placeholders(self, **new_placeholders):
         """Update full job list for if placeholder values got changed."""
         self.file_tree.placeholders.update(**new_placeholders)
+        self.partial_tree.placeholders.update(**new_placeholders)
         self.full_job_list = self.pipeline.generate_jobs(self.file_tree)
         self.reset_all_jobs()
 
     def add_selected_file(self, file):
         """Add a specific file to the list to be produced."""
         self.selected_files.add(file)
         target = self.get_file_targets(file)
```

### Comparing `fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/placeholder_tab.py` & `fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/placeholder_tab.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/run.py` & `fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/run.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/selector_tab.py` & `fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/selector_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def compose(self) -> ComposeResult:
         """Create basic layout."""
         yield Header()
         self.template_renderer = TemplateRenderer(self.selector)
         yield Vertical(
             Horizontal(
-                TemplateTreeControl(self.file_tree, self.template_renderer),
+                TemplateTreeControl(self.selector.partial_tree, self.template_renderer),
                 self.template_renderer,
             ),
             Horizontal(
                 Button("Back", name="back"),
                 Button("Run pipeline", name="run"),
                 Select(
                     [(e.name, e) for e in RunMethod], value=self.selector.run_method
```

### Comparing `fsl-pipe-gui-0.0.0/src/fsl_pipe_gui/summary.py` & `fsl-pipe-gui-0.1.0/src/fsl_pipe_gui/summary.py`

 * *Files identical despite different names*

