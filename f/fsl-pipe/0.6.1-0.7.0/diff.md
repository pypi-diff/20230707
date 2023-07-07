# Comparing `tmp/fsl-pipe-0.6.1.tar.gz` & `tmp/fsl-pipe-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsl-pipe-0.6.1.tar", last modified: Wed Mar 29 09:45:19 2023, max compression
+gzip compressed data, was "fsl-pipe-0.7.0.tar", last modified: Fri Jul  7 15:40:22 2023, max compression
```

## Comparing `fsl-pipe-0.6.1.tar` & `fsl-pipe-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:45:19.414594 fsl-pipe-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-29 09:39:12.000000 fsl-pipe-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2796 2023-03-29 09:45:19.414594 fsl-pipe-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2280 2023-03-28 13:22:26.000000 fsl-pipe-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-03-29 09:45:19.415594 fsl-pipe-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:45:19.412594 fsl-pipe-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:45:19.413594 fsl-pipe-0.6.1/src/fsl_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-03-29 09:39:12.000000 fsl-pipe-0.6.1/src/fsl_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/src/fsl_pipe/datalad.py
--rw-rw-rw-   0 root         (0) root         (0)    33185 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/src/fsl_pipe/job.py
--rw-rw-rw-   0 root         (0) root         (0)    36502 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/src/fsl_pipe/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-28 12:35:56.000000 fsl-pipe-0.6.1/src/fsl_pipe/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 09:45:19.414594 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2796 2023-03-29 09:45:19.000000 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-03-29 09:45:19.000000 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 09:45:19.000000 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-29 09:45:19.000000 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-29 09:45:19.000000 fsl-pipe-0.6.1/src/fsl_pipe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-29 09:39:12.000000 fsl-pipe-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2280 2023-04-17 12:08:35.000000 fsl-pipe-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-07-07 15:40:22.093599 fsl-pipe-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.089599 fsl-pipe-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.091600 fsl-pipe-0.7.0/src/fsl_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-07 13:58:51.000000 fsl-pipe-0.7.0/src/fsl_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/src/fsl_pipe/datalad.py
+-rw-rw-rw-   0 root         (0) root         (0)    33496 2023-07-07 12:21:17.000000 fsl-pipe-0.7.0/src/fsl_pipe/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    37846 2023-07-07 13:57:09.000000 fsl-pipe-0.7.0/src/fsl_pipe/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/src/fsl_pipe/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/top_level.txt
```

### Comparing `fsl-pipe-0.6.1/LICENSE` & `fsl-pipe-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.6.1/PKG-INFO` & `fsl-pipe-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fsl-pipe
-Version: 0.6.1
+Version: 0.7.0
 Summary: Declative pipelines based on Filetrees
 Home-page: https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe
 Author: Michiel Cottaar
 Author-email: michiel.cottaar@ndcn.ox.ac.uk
 Project-URL: Bug Tracker, https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues
 Project-URL: Documentation, https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![File-tree Documentation](https://img.shields.io/badge/Documentation-file--tree-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577070.svg)](https://doi.org/10.5281/zenodo.6577070)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577069.svg)](https://doi.org/10.5281/zenodo.6577069)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/pipelines/latest)
 [![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe/htmlcov)
 
 Declative pipelines based on Filetrees
 
 # Installation
 ```shell
```

### Comparing `fsl-pipe-0.6.1/README.md` & `fsl-pipe-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![File-tree Documentation](https://img.shields.io/badge/Documentation-file--tree-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577070.svg)](https://doi.org/10.5281/zenodo.6577070)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577069.svg)](https://doi.org/10.5281/zenodo.6577069)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/pipelines/latest)
 [![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe/htmlcov)
 
 Declative pipelines based on Filetrees
 
 # Installation
 ```shell
```

### Comparing `fsl-pipe-0.6.1/setup.cfg` & `fsl-pipe-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.1
+current_version = 0.7.0
 commit = True
 tag = True
 
 [bumpversion:file:src/fsl_pipe/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `fsl-pipe-0.6.1/src/fsl_pipe/datalad.py` & `fsl-pipe-0.7.0/src/fsl_pipe/datalad.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.6.1/src/fsl_pipe/job.py` & `fsl-pipe-0.7.0/src/fsl_pipe/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,16 @@
             local_submit = dict(self.submit_params)
             if 'logdir' not in local_submit:
                 local_submit['logdir'] = 'log'
             Path(local_submit['logdir']).mkdir(exist_ok=True, parents=True)
             if 'name' not in local_submit:
                 local_submit['name'] = self.job_name()
             cmd = func_to_cmd(self.function, (), self.kwargs, local_submit['logdir'], clean="on_success")
+            if len(wait_for) == 0:
+                wait_for = None
             self.job = submit(cmd, jobhold=wait_for, **local_submit)
             logger.debug(f"submitted {self} with job ID {self.job}")
         elif method == RunMethod.dask:
             import dask
             def dask_job(*other_jobs):
                 if any(a != 0 for a in other_jobs):
                     logger.debug(f"{self} skipped because dependencies failed")
@@ -412,14 +414,24 @@
 
         Steps:
         1. Creates output directory
         """
         for target in self.output_targets:
             target.filename.parent.mkdir(parents=True, exist_ok=True)
 
+    def expected(self, ):
+        """
+        Return true if this job is expected to be able to run.
+        """
+        for target in self.input_targets:
+            if not target.expected():
+                return False
+        return True
+
+
 class SingleJob(JobParent):
     """A single job within a larger pipeline."""
 
     def __init__(self, function: Callable, kwargs, submit_params, input_targets, output_targets, optionals, set_parameters=None, batch=None):
         """
         Create a single job that can be run locally or submitted.
```

### Comparing `fsl-pipe-0.6.1/src/fsl_pipe/pipeline.py` & `fsl-pipe-0.7.0/src/fsl_pipe/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
                             help="If set also overwrites dependencies of requested files.")
         parser.add_argument("-j", '--job-hold', default='',
                             help='Place a hold on the whole pipeline until job has completed.')
         parser.add_argument('--skip-missing', default='',
                             help='If set skip running any jobs depending on missing data. This replaces the default behaviour of raising an error if any required input data is missing.')
         parser.add_argument("-q", '--quiet', action='store_true', help="Suppresses the report on what will be run (might speed up starting up the pipeline substantially).")
         parser.add_argument("-b", "--batch", action="store_true", help="Batch jobs based on submit parameters and pipeline labels before running them.")
+        gui_help = "Start a GUI to select which output files should be produced by the pipeline."
+        try:
+            import fsl_pipe_gui
+        except ModuleNotFoundError:
+            gui_help = gui_help + " Missing requirement 'fsl-pipe-gui' to run the GUI. Please install this with `conda/pip install fsl-pipe-gui`."
+        parser.add_argument("-g", "--gui", action="store_true", help=gui_help)
         if datalad is not None:
             parser.add_argument("--datalad", action='store_true',
                                 help="run datalad get on all input data before running/submitting the jobs")
         for var, values in tree.placeholders.items():
             if not isinstance(var, str):
                 continue
             if '/' in var:
@@ -174,28 +180,31 @@
             - skip-missing: whether to skip jobs depending on missing data instead of raising an error
             - datalad (defaults to False): if true, run datalad get on all input data before running/submitting the jobs
             - {placeholder} (defaults to values in FileTree): sequence of strings overwriting the possible values for a particular placeholder
 
         :param tree: Definition of pipeline input/output files
         """
         from .job import RunMethod
+        for var in tree.placeholders:
+            if isinstance(var, str) and getattr(args, var, None) is not None:
+                tree.placeholders[var] = getattr(args, var)
+        if args.gui:
+            self.gui(tree, overwrite_dependencies=args.overwrite_dependencies, run_method=RunMethod[args.pipeline_method])
+            return
         templates = set.union(*[script.filter_templates(output=True, all_templates=tree.template_keys()) for script in self.scripts])
         requested_templates = getattr(
             args, 'templates', 
             None if len(self.default_output) == 0 else self.default_output
         )
         not_in_tree = [template for template in requested_templates if template not in tree.template_keys()]
         if len(not_in_tree) > 0:
             raise ValueError(f"Requested templates {not_in_tree} are not defined in the FileTree")
         unrecognised_templates = set(requested_templates).difference(templates)
         if len(unrecognised_templates) > 0:
             raise ValueError(f"Requested templates {unrecognised_templates} cannot be produced by this pipeline")
-        for var in tree.placeholders:
-            if isinstance(var, str) and getattr(args, var, None) is not None:
-                tree.placeholders[var] = getattr(args, var)
         concrete = self.generate_jobs(tree)
         torun = concrete.filter(requested_templates, overwrite=args.overwrite, overwrite_dependencies=args.overwrite_dependencies, skip_missing=args.skip_missing)
         if not args.quiet:
             torun.report()
         if getattr(args, "batch", False):
             use_label = any(job.batch is not None for job in concrete.jobs)
             torun = torun.batch(use_label=use_label)
@@ -222,14 +231,28 @@
             if tree is None:
                 raise ValueError("No reference FileTree for pipeline found")
 
         parser = self.default_parser(tree=tree, include_vars=include_vars, exclude_vars=exclude_vars)
         args = parser.parse_args(cli_arguments)
         self.run_cli(args, tree)
 
+    def gui(self, tree: FileTree, **kwargs):
+        """
+        Run the fsl-pipe-gui interface to select pipeline output.
+
+        :param tree: `file_tree.FileTree` object describing the directory structure for the input/output files.
+        :param overwrite_depencencies: set to True to overwrite dependencies
+        :param run_method: overrides the default method to run the jobs
+        """
+        try:
+            from fsl_pipe_gui import run_gui
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError("'fsl-pipe-gui' needs to be installed to run the graphical user interface. Please run `pip/conda install fsl-pipe-gui` and try again.")
+        run_gui(self, tree, **kwargs)
+
     def move_to_subtree(self, sub_tree=None, other_mappings=None):
         """
         Create a new pipeline that runs in a sub-tree of a larger tree rather than at the top level.
 
         :param sub_tree: name of the sub-tree in the FileTree
         :param other_mappings: other mappings between templates or placeholder names and their new values
         """
@@ -327,14 +350,16 @@
         self.configure(function.__annotations__)
 
         if kwargs is not None:
             self.configure(kwargs)
 
         if no_iter is None:
             no_iter = set()
+        elif isinstance(no_iter, str):
+            no_iter = [no_iter]
         self.explicit_no_iter = set(no_iter)
 
     def copy(self, ):
         """Create a copy of this PipedFunction for pipeline merging."""
         new_script = copy(self)
         new_script.all_kwargs = dict(self.all_kwargs)
         self.explicit_no_iter = set(self.explicit_no_iter)
@@ -605,15 +630,15 @@
 The actual filename is extracted from the FileTree based on the template key.
 This template key will by default match the keyword argument name, but can be overriden by calling `In` (e.g., `In("other_key")`).
 """
 Ref = Template()
 
 """Use to mark keyword arguments that represent placeholder values in the pipeline.
 
-Placeholder values are returned as :py:`PlaceholderValue` objects.
+Placeholder values are returned as :any:`PlaceholderValue` objects.
 """
 Var = PlaceHolder()
 
 
 def to_templates_dict(input_files=(), output_files=(), reference_files=()):
     """Convert a sequence of input/output/reference files into a template dictionary.
```

### Comparing `fsl-pipe-0.6.1/src/fsl_pipe.egg-info/PKG-INFO` & `fsl-pipe-0.7.0/src/fsl_pipe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fsl-pipe
-Version: 0.6.1
+Version: 0.7.0
 Summary: Declative pipelines based on Filetrees
 Home-page: https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe
 Author: Michiel Cottaar
 Author-email: michiel.cottaar@ndcn.ox.ac.uk
 Project-URL: Bug Tracker, https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues
 Project-URL: Documentation, https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![File-tree Documentation](https://img.shields.io/badge/Documentation-file--tree-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577070.svg)](https://doi.org/10.5281/zenodo.6577070)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577069.svg)](https://doi.org/10.5281/zenodo.6577069)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/pipelines/latest)
 [![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe/htmlcov)
 
 Declative pipelines based on Filetrees
 
 # Installation
 ```shell
```

