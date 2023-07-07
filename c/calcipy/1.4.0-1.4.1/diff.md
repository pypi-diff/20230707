# Comparing `tmp/calcipy-1.4.0.tar.gz` & `tmp/calcipy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.4.0.tar", max compression
+gzip compressed data, was "calcipy-1.4.1.tar", max compression
```

## Comparing `calcipy-1.4.0.tar` & `calcipy-1.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.4.0/LICENSE
--rw-r--r--   0        0        0      167 2023-06-25 19:59:53.761206 calcipy-1.4.0/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.4.0/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.4.0/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.4.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.4.0/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.4.0/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.4.0/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.4.0/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.4.0/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.4.0/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.4.0/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.4.0/calcipy/file_search.py
--rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.4.0/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.4.0/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.4.0/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.4.0/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6441 2023-06-25 19:20:04.315707 calcipy-1.4.0/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1418 2023-06-23 11:18:02.014243 calcipy-1.4.0/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.4.0/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.4.0/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.4.0/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.4.0/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.4.0/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.4.0/calcipy/tasks/executable_utils.py
--rw-r--r--   0        0        0     4191 2023-06-25 19:43:32.342494 calcipy-1.4.0/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.4.0/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.4.0/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.4.0/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.4.0/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.4.0/calcipy/tasks/test.py
--rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.4.0/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-06-25 20:00:00.310899 calcipy-1.4.0/docs/README.md
--rw-r--r--   0        0        0     6579 2023-06-25 19:59:53.799463 calcipy-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    11265 1970-01-01 00:00:00.000000 calcipy-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.4.1/LICENSE
+-rw-r--r--   0        0        0      167 2023-07-07 10:08:33.703053 calcipy-1.4.1/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.4.1/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.4.1/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.4.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.4.1/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.4.1/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.4.1/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.4.1/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.4.1/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.4.1/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.4.1/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.4.1/calcipy/file_search.py
+-rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.4.1/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.4.1/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.4.1/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.4.1/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6444 2023-07-07 09:54:44.784397 calcipy-1.4.1/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1418 2023-06-23 11:18:02.014243 calcipy-1.4.1/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.4.1/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.4.1/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.4.1/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.4.1/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.4.1/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.4.1/calcipy/tasks/executable_utils.py
+-rw-r--r--   0        0        0     4191 2023-06-25 19:43:32.342494 calcipy-1.4.1/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.4.1/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.4.1/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.4.1/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.4.1/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.4.1/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.4.1/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     7709 2023-07-07 10:08:16.231213 calcipy-1.4.1/docs/README.md
+-rw-r--r--   0        0        0     6579 2023-07-07 10:08:33.742868 calcipy-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12323 1970-01-01 00:00:00.000000 calcipy-1.4.1/PKG-INFO
```

### Comparing `calcipy-1.4.0/LICENSE` & `calcipy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/can_skip.py` & `calcipy-1.4.1/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.4.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/cli.py` & `calcipy-1.4.1/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/code_tag_collector/_collector.py` & `calcipy-1.4.1/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.4.1/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.4.1/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/file_search.py` & `calcipy-1.4.1/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/invoke_helpers.py` & `calcipy-1.4.1/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/md_writer/_writer.py` & `calcipy-1.4.1/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/noxfile/_noxfile.py` & `calcipy-1.4.1/calcipy/noxfile/_noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     from nox_poetry import session as nox_session  # type: ignore[no-redef]
 
 
 @lru_cache(maxsize=1)
 @beartype
 def _get_pythons() -> List[str]:
     """Get python versions from the `.tool-versions` file."""
-    return [str(ver) for ver in get_tool_versions()['python']]
+    return [*{str(ver) for ver in get_tool_versions()['python']}]
 
 
 @beartype
 def _retrieve_keys(source: Dict, keys: List[str]) -> Dict:  # type: ignore[type-arg]
     """Retrieve nested dictionary keys unless not found."""
     result = source
     for key in keys:
```

### Comparing `calcipy-1.4.0/calcipy/scripts.py` & `calcipy-1.4.1/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/all_tasks.py` & `calcipy-1.4.1/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/cl.py` & `calcipy-1.4.1/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/defaults.py` & `calcipy-1.4.1/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/doc.py` & `calcipy-1.4.1/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/executable_utils.py` & `calcipy-1.4.1/calcipy/tasks/executable_utils.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/lint.py` & `calcipy-1.4.1/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/pack.py` & `calcipy-1.4.1/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/stale.py` & `calcipy-1.4.1/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/tags.py` & `calcipy-1.4.1/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/test.py` & `calcipy-1.4.1/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/calcipy/tasks/types.py` & `calcipy-1.4.1/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.4.0/docs/README.md` & `calcipy-1.4.1/docs/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -36,59 +36,101 @@
 ### Calcipy CLI
 
 Additionally, `calcipy` can be run as a CLI application without adding the package as a dependency.
 
 Quick Start:
 
 ```sh
-pipx install calcipy
+# For the CLI, only install a few of the extras which can be used from a few different CLI commands
+pipx install 'calcipy[flake8,lint,tags]'
 
 # Use 'tags' to create a CODE_TAG_SUMMARY of the specified directory
-calcipy tags --help
-calcipy tags --base-dir=~/path/to/my_project
+calcipy-tags tags --help
+calcipy-tags tags --base-dir=~/path/to/my_project
 
-# See additional documentation from the CLI help
-> calcipy
+# You can list all provided CLI commands with
+pipx list
+```
+
+```txt
+venvs are in ~/.local/pipx/venvs
+apps are exposed on your $PATH at ~/.local/bin
+   package calcipy 1.4.0, installed using Python 3.11.4
+    - calcipy
+    - calcipy-lint
+    - calcipy-pack
+    - calcipy-tags
+    - calcipy-types
+```
+
+Note: the CLI output below is compressed for readability, but you can try running each of these commands locally to see the most up-to-date documentation and the full set of options. The "Usage", "Core options", and "Global Task Options" are the same for each subsequent command, so they are excluded for brevity.
+
+```txt
+> calcipy-lint
+Usage: calcipy-lint [--core-opts] <subcommand> [--subcommand-opts] ...
+
+Core options:
+
+  --complete                         Print tab-completion candidates for given parse remainder.
+  --hide=STRING                      Set default value of run()'s 'hide' kwarg.
+  --print-completion-script=STRING   Print the tab-completion script for your preferred shell (bash|zsh|fish).
+  --prompt-for-sudo-password         Prompt user at start of session for the sudo.password config value.
+  --write-pyc                        Enable creation of .pyc files.
+  -d, --debug                        Enable debug output.
+  -D INT, --list-depth=INT           When listing tasks, only show the first INT levels.
+  -e, --echo                         Echo executed commands before running.
+  -f STRING, --config=STRING         Runtime configuration file to use.
+  -F STRING, --list-format=STRING    Change the display format used when listing tasks. Should be one of: flat (default), nested, json.
+  -h [STRING], --help[=STRING]       Show core or per-task help and exit.
+  -l [STRING], --list[=STRING]       List available tasks, optionally limited to a namespace.
+  -p, --pty                          Use a pty when executing shell commands.
+  -R, --dry                          Echo commands instead of running.
+  -T INT, --command-timeout=INT      Specify a global command execution timeout, in seconds.
+  -V, --version                      Show version and exit.
+  -w, --warn-only                    Warn, instead of failing, when shell commands fail.
 
 Subcommands:
 
-main                                     Main task pipeline.
-other                                    Run tasks that are otherwise not exercised in main.
-release                                  Release pipeline.
-cl.bump                                  Bumps project version based on commits & settings in pyproject.toml.
-cl.write                                 Write a Changelog file with the raw Git history.
-doc.build                                Build documentation with mkdocs.
-doc.deploy                               Deploy docs to the Github `gh-pages` branch.
-doc.watch                                Serve local documentation for local editing.
-lint.autopep8                            Run autopep8.
-lint.check (lint)                        Run ruff as check-only.
-lint.fix                                 Run ruff and apply fixes.
-lint.flake8                              Run ruff and apply fixes.
-lint.pre-commit                          Run pre-commit.
-lint.pylint                              Run ruff and apply fixes.
-lint.security                            Attempt to identify possible security vulnerabilities.
-lint.watch                               Run ruff as check-only.
-nox.noxfile (nox)                        Run nox from the local noxfile.
-pack.check-licenses                      Check licenses for compatibility with `licensecheck`.
-pack.lock                                Ensure poetry.lock is  up-to-date.
-pack.publish                             Build the distributed format(s) and publish.
-stale.check-for-stale-packages (stale)   Identify stale dependencies.
-tags.collect-code-tags (tags)            Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments.
-test.coverage                            Generate useful coverage outputs after running pytest.
-test.pytest (test)                       Run pytest with default arguments.
-test.step                                Run pytest optimized to stop on first error.
-test.watch                               Run pytest with polling and optimized to stop on first error.
-types.mypy                               Run mypy.
-types.pyright                            Run pyright.
+  lint.autopep8       Run autopep8.
+  lint.check (lint)   Run ruff as check-only.
+  lint.fix            Run ruff and apply fixes.
+  lint.flake8         Run flake8.
+  lint.pre-commit     Run pre-commit.
+  lint.pylint         Run pylint.
+  lint.security       Attempt to identify possible security vulnerabilities.
+  lint.watch          Run ruff as check-only.
 
 Global Task Options:
 
-working_dir   Set the cwd for the program. Example: "../run --working-dir .. lint test"
-*file_args    List of Paths available globally to all tasks. Will resolve paths with working_dir
-verbose       Globally configure logger verbosity (-vvv for most verbose)
+  *file_args             List of Paths available globally to all tasks. Will resolve paths with working_dir
+  --keep-going           Continue running tasks even on failure
+  --working_dir=STRING   Set the cwd for the program. Example: "../run --working-dir .. lint test"
+  -v,-vv,-vvv            Globally configure logger verbosity (-vvv for most verbose)
+
+> calcipy-pack
+
+Subcommands:
+
+  pack.check-licenses   Check licenses for compatibility with `licensecheck`.
+  pack.install-extras   Run poetry install with all extras.
+  pack.lock             Ensure poetry.lock is  up-to-date.
+  pack.publish          Build the distributed format(s) and publish.
+
+> calcipy-tags
+
+Subcommands:
+
+  tags.collect-code-tags (tags)   Create a `CODE_TAG_SUMMARY.md` with a table          for TODO- and FIXME-style code comments.
+
+> calcipy-types
+
+Subcommands:
+
+  types.mypy      Run mypy.
+  types.pyright   Run pyright.
 ```
 
 ### Calcipy Pre-Commit
 
 `calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:
 
 ```yaml
```

### Comparing `calcipy-1.4.0/pyproject.toml` & `calcipy-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.4.0"
+version = "1.4.1"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,15 +26,15 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.4.0"
+version = "1.4.1"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # lint
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
```

### Comparing `calcipy-1.4.0/PKG-INFO` & `calcipy-1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -129,59 +129,101 @@
 ### Calcipy CLI
 
 Additionally, `calcipy` can be run as a CLI application without adding the package as a dependency.
 
 Quick Start:
 
 ```sh
-pipx install calcipy
+# For the CLI, only install a few of the extras which can be used from a few different CLI commands
+pipx install 'calcipy[flake8,lint,tags]'
 
 # Use 'tags' to create a CODE_TAG_SUMMARY of the specified directory
-calcipy tags --help
-calcipy tags --base-dir=~/path/to/my_project
+calcipy-tags tags --help
+calcipy-tags tags --base-dir=~/path/to/my_project
 
-# See additional documentation from the CLI help
-> calcipy
+# You can list all provided CLI commands with
+pipx list
+```
+
+```txt
+venvs are in ~/.local/pipx/venvs
+apps are exposed on your $PATH at ~/.local/bin
+   package calcipy 1.4.0, installed using Python 3.11.4
+    - calcipy
+    - calcipy-lint
+    - calcipy-pack
+    - calcipy-tags
+    - calcipy-types
+```
+
+Note: the CLI output below is compressed for readability, but you can try running each of these commands locally to see the most up-to-date documentation and the full set of options. The "Usage", "Core options", and "Global Task Options" are the same for each subsequent command, so they are excluded for brevity.
+
+```txt
+> calcipy-lint
+Usage: calcipy-lint [--core-opts] <subcommand> [--subcommand-opts] ...
+
+Core options:
+
+  --complete                         Print tab-completion candidates for given parse remainder.
+  --hide=STRING                      Set default value of run()'s 'hide' kwarg.
+  --print-completion-script=STRING   Print the tab-completion script for your preferred shell (bash|zsh|fish).
+  --prompt-for-sudo-password         Prompt user at start of session for the sudo.password config value.
+  --write-pyc                        Enable creation of .pyc files.
+  -d, --debug                        Enable debug output.
+  -D INT, --list-depth=INT           When listing tasks, only show the first INT levels.
+  -e, --echo                         Echo executed commands before running.
+  -f STRING, --config=STRING         Runtime configuration file to use.
+  -F STRING, --list-format=STRING    Change the display format used when listing tasks. Should be one of: flat (default), nested, json.
+  -h [STRING], --help[=STRING]       Show core or per-task help and exit.
+  -l [STRING], --list[=STRING]       List available tasks, optionally limited to a namespace.
+  -p, --pty                          Use a pty when executing shell commands.
+  -R, --dry                          Echo commands instead of running.
+  -T INT, --command-timeout=INT      Specify a global command execution timeout, in seconds.
+  -V, --version                      Show version and exit.
+  -w, --warn-only                    Warn, instead of failing, when shell commands fail.
 
 Subcommands:
 
-main                                     Main task pipeline.
-other                                    Run tasks that are otherwise not exercised in main.
-release                                  Release pipeline.
-cl.bump                                  Bumps project version based on commits & settings in pyproject.toml.
-cl.write                                 Write a Changelog file with the raw Git history.
-doc.build                                Build documentation with mkdocs.
-doc.deploy                               Deploy docs to the Github `gh-pages` branch.
-doc.watch                                Serve local documentation for local editing.
-lint.autopep8                            Run autopep8.
-lint.check (lint)                        Run ruff as check-only.
-lint.fix                                 Run ruff and apply fixes.
-lint.flake8                              Run ruff and apply fixes.
-lint.pre-commit                          Run pre-commit.
-lint.pylint                              Run ruff and apply fixes.
-lint.security                            Attempt to identify possible security vulnerabilities.
-lint.watch                               Run ruff as check-only.
-nox.noxfile (nox)                        Run nox from the local noxfile.
-pack.check-licenses                      Check licenses for compatibility with `licensecheck`.
-pack.lock                                Ensure poetry.lock is  up-to-date.
-pack.publish                             Build the distributed format(s) and publish.
-stale.check-for-stale-packages (stale)   Identify stale dependencies.
-tags.collect-code-tags (tags)            Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments.
-test.coverage                            Generate useful coverage outputs after running pytest.
-test.pytest (test)                       Run pytest with default arguments.
-test.step                                Run pytest optimized to stop on first error.
-test.watch                               Run pytest with polling and optimized to stop on first error.
-types.mypy                               Run mypy.
-types.pyright                            Run pyright.
+  lint.autopep8       Run autopep8.
+  lint.check (lint)   Run ruff as check-only.
+  lint.fix            Run ruff and apply fixes.
+  lint.flake8         Run flake8.
+  lint.pre-commit     Run pre-commit.
+  lint.pylint         Run pylint.
+  lint.security       Attempt to identify possible security vulnerabilities.
+  lint.watch          Run ruff as check-only.
 
 Global Task Options:
 
-working_dir   Set the cwd for the program. Example: "../run --working-dir .. lint test"
-*file_args    List of Paths available globally to all tasks. Will resolve paths with working_dir
-verbose       Globally configure logger verbosity (-vvv for most verbose)
+  *file_args             List of Paths available globally to all tasks. Will resolve paths with working_dir
+  --keep-going           Continue running tasks even on failure
+  --working_dir=STRING   Set the cwd for the program. Example: "../run --working-dir .. lint test"
+  -v,-vv,-vvv            Globally configure logger verbosity (-vvv for most verbose)
+
+> calcipy-pack
+
+Subcommands:
+
+  pack.check-licenses   Check licenses for compatibility with `licensecheck`.
+  pack.install-extras   Run poetry install with all extras.
+  pack.lock             Ensure poetry.lock is  up-to-date.
+  pack.publish          Build the distributed format(s) and publish.
+
+> calcipy-tags
+
+Subcommands:
+
+  tags.collect-code-tags (tags)   Create a `CODE_TAG_SUMMARY.md` with a table          for TODO- and FIXME-style code comments.
+
+> calcipy-types
+
+Subcommands:
+
+  types.mypy      Run mypy.
+  types.pyright   Run pyright.
 ```
 
 ### Calcipy Pre-Commit
 
 `calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:
 
 ```yaml
```

