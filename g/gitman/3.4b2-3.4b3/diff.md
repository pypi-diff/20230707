# Comparing `tmp/gitman-3.4b2.tar.gz` & `tmp/gitman-3.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitman-3.4b2.tar", max compression
+gzip compressed data, was "gitman-3.4b3.tar", max compression
```

## Comparing `gitman-3.4b2.tar` & `gitman-3.4b3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1088 2018-09-08 18:50:46.000000 gitman-3.4b2/LICENSE.md
--rw-r--r--   0        0        0     4079 2022-12-09 14:37:00.211987 gitman-3.4b2/README.md
--rw-r--r--   0        0        0      330 2022-11-09 19:43:21.865006 gitman-3.4b2/gitman/__init__.py
--rw-r--r--   0        0        0      589 2022-01-13 13:52:14.257310 gitman-3.4b2/gitman/__main__.py
--rw-r--r--   0        0        0    10303 2022-03-26 16:18:59.643140 gitman-3.4b2/gitman/cli.py
--rw-r--r--   0        0        0    11816 2023-03-22 11:55:52.337212 gitman-3.4b2/gitman/commands.py
--rw-r--r--   0        0        0     5395 2022-01-13 13:52:14.485313 gitman-3.4b2/gitman/common.py
--rw-r--r--   0        0        0      256 2021-02-12 02:33:38.716395 gitman-3.4b2/gitman/decorators.py
--rw-r--r--   0        0        0      726 2022-01-13 13:52:14.274203 gitman-3.4b2/gitman/exceptions.py
--rw-r--r--   0        0        0     8466 2022-03-26 01:35:15.876172 gitman-3.4b2/gitman/git.py
--rw-r--r--   0        0        0      241 2022-01-13 13:52:14.262983 gitman-3.4b2/gitman/hook-gitman.py
--rw-r--r--   0        0        0      127 2022-03-12 20:29:22.054396 gitman-3.4b2/gitman/models/__init__.py
--rw-r--r--   0        0        0    15330 2023-03-22 12:30:59.495494 gitman-3.4b2/gitman/models/config.py
--rw-r--r--   0        0        0      521 2020-11-18 21:15:23.000000 gitman-3.4b2/gitman/models/group.py
--rw-r--r--   0        0        0    11031 2022-03-26 13:15:44.714470 gitman-3.4b2/gitman/models/source.py
--rw-r--r--   0        0        0     3528 2022-03-26 16:18:59.081925 gitman-3.4b2/gitman/plugin.py
--rw-r--r--   0        0        0      740 2022-03-13 19:05:54.837062 gitman-3.4b2/gitman/settings.py
--rw-r--r--   0        0        0     4372 2022-03-12 19:36:19.514873 gitman-3.4b2/gitman/shell.py
--rw-r--r--   0        0        0       34 2017-01-09 13:05:30.000000 gitman-3.4b2/gitman/tests/__init__.py
--rw-r--r--   0        0        0      847 2022-01-13 13:52:14.475774 gitman-3.4b2/gitman/tests/conftest.py
--rw-r--r--   0        0        0      318 2021-06-02 20:53:11.405192 gitman-3.4b2/gitman/tests/files/gdm-custom.yml
--rw-r--r--   0        0        0      158 2018-11-20 14:52:53.000000 gitman-3.4b2/gitman/tests/files/gdm-default.yml
--rw-r--r--   0        0        0      755 2023-03-21 22:24:57.996859 gitman-3.4b2/gitman/tests/files/gitman.yml
--rw-r--r--   0        0        0      765 2023-01-25 17:38:54.328440 gitman-3.4b2/gitman/tests/files/subdir/gitman.yml
--rw-r--r--   0        0        0      778 2023-01-25 17:38:54.328826 gitman-3.4b2/gitman/tests/files/subdir/subsubdir/gitman.yml
--rw-r--r--   0        0        0      808 2023-01-25 17:38:54.329319 gitman-3.4b2/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml
--rw-r--r--   0        0        0    14014 2022-01-13 13:52:14.996788 gitman-3.4b2/gitman/tests/test_cli.py
--rw-r--r--   0        0        0     1118 2019-01-21 21:57:40.000000 gitman-3.4b2/gitman/tests/test_commands.py
--rw-r--r--   0        0        0     3047 2022-01-13 13:52:14.645994 gitman-3.4b2/gitman/tests/test_common.py
--rw-r--r--   0        0        0     9227 2022-03-26 01:35:15.876837 gitman-3.4b2/gitman/tests/test_git.py
--rw-r--r--   0        0        0     4553 2023-03-22 12:20:02.699527 gitman-3.4b2/gitman/tests/test_models_config.py
--rw-r--r--   0        0        0      263 2022-01-13 13:52:14.610271 gitman-3.4b2/gitman/tests/test_models_group.py
--rw-r--r--   0        0        0     5419 2022-03-26 01:35:15.877476 gitman-3.4b2/gitman/tests/test_models_source.py
--rw-r--r--   0        0        0     4181 2022-01-13 13:52:14.861539 gitman-3.4b2/gitman/tests/test_plugin.py
--rw-r--r--   0        0        0     3600 2022-01-13 13:52:14.795247 gitman-3.4b2/gitman/tests/test_shell.py
--rw-r--r--   0        0        0      344 2022-01-13 13:52:14.734256 gitman-3.4b2/gitman/tests/utils.py
--rw-r--r--   0        0        0     2096 2023-03-22 12:33:44.874777 gitman-3.4b2/pyproject.toml
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 gitman-3.4b2/setup.py
--rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 gitman-3.4b2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2018-09-08 18:50:46.000000 gitman-3.4b3/LICENSE.md
+-rw-r--r--   0        0        0     4079 2022-12-09 14:37:00.211987 gitman-3.4b3/README.md
+-rw-r--r--   0        0        0      330 2022-11-09 19:43:21.865006 gitman-3.4b3/gitman/__init__.py
+-rw-r--r--   0        0        0      589 2022-01-13 13:52:14.257310 gitman-3.4b3/gitman/__main__.py
+-rw-r--r--   0        0        0    10303 2022-03-26 16:18:59.643140 gitman-3.4b3/gitman/cli.py
+-rw-r--r--   0        0        0    11816 2023-03-22 11:55:52.337212 gitman-3.4b3/gitman/commands.py
+-rw-r--r--   0        0        0     5395 2022-01-13 13:52:14.485313 gitman-3.4b3/gitman/common.py
+-rw-r--r--   0        0        0      256 2021-02-12 02:33:38.716395 gitman-3.4b3/gitman/decorators.py
+-rw-r--r--   0        0        0      726 2022-01-13 13:52:14.274203 gitman-3.4b3/gitman/exceptions.py
+-rw-r--r--   0        0        0     8466 2022-03-26 01:35:15.876172 gitman-3.4b3/gitman/git.py
+-rw-r--r--   0        0        0      241 2022-01-13 13:52:14.262983 gitman-3.4b3/gitman/hook-gitman.py
+-rw-r--r--   0        0        0      127 2022-03-12 20:29:22.054396 gitman-3.4b3/gitman/models/__init__.py
+-rw-r--r--   0        0        0    15401 2023-03-22 19:48:37.552933 gitman-3.4b3/gitman/models/config.py
+-rw-r--r--   0        0        0      521 2020-11-18 21:15:23.000000 gitman-3.4b3/gitman/models/group.py
+-rw-r--r--   0        0        0    11031 2022-03-26 13:15:44.714470 gitman-3.4b3/gitman/models/source.py
+-rw-r--r--   0        0        0     3528 2022-03-26 16:18:59.081925 gitman-3.4b3/gitman/plugin.py
+-rw-r--r--   0        0        0      740 2022-03-13 19:05:54.837062 gitman-3.4b3/gitman/settings.py
+-rw-r--r--   0        0        0     4372 2022-03-12 19:36:19.514873 gitman-3.4b3/gitman/shell.py
+-rw-r--r--   0        0        0       34 2017-01-09 13:05:30.000000 gitman-3.4b3/gitman/tests/__init__.py
+-rw-r--r--   0        0        0      847 2022-01-13 13:52:14.475774 gitman-3.4b3/gitman/tests/conftest.py
+-rw-r--r--   0        0        0      318 2021-06-02 20:53:11.405192 gitman-3.4b3/gitman/tests/files/gdm-custom.yml
+-rw-r--r--   0        0        0      158 2018-11-20 14:52:53.000000 gitman-3.4b3/gitman/tests/files/gdm-default.yml
+-rw-r--r--   0        0        0      755 2023-03-21 22:24:57.996859 gitman-3.4b3/gitman/tests/files/gitman.yml
+-rw-r--r--   0        0        0      765 2023-01-25 17:38:54.328440 gitman-3.4b3/gitman/tests/files/subdir/gitman.yml
+-rw-r--r--   0        0        0      778 2023-01-25 17:38:54.328826 gitman-3.4b3/gitman/tests/files/subdir/subsubdir/gitman.yml
+-rw-r--r--   0        0        0      808 2023-01-25 17:38:54.329319 gitman-3.4b3/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml
+-rw-r--r--   0        0        0    14014 2022-01-13 13:52:14.996788 gitman-3.4b3/gitman/tests/test_cli.py
+-rw-r--r--   0        0        0     1118 2019-01-21 21:57:40.000000 gitman-3.4b3/gitman/tests/test_commands.py
+-rw-r--r--   0        0        0     3047 2022-01-13 13:52:14.645994 gitman-3.4b3/gitman/tests/test_common.py
+-rw-r--r--   0        0        0     9227 2022-03-26 01:35:15.876837 gitman-3.4b3/gitman/tests/test_git.py
+-rw-r--r--   0        0        0     4849 2023-03-22 19:43:36.218224 gitman-3.4b3/gitman/tests/test_models_config.py
+-rw-r--r--   0        0        0      263 2022-01-13 13:52:14.610271 gitman-3.4b3/gitman/tests/test_models_group.py
+-rw-r--r--   0        0        0     5419 2022-03-26 01:35:15.877476 gitman-3.4b3/gitman/tests/test_models_source.py
+-rw-r--r--   0        0        0     4181 2022-01-13 13:52:14.861539 gitman-3.4b3/gitman/tests/test_plugin.py
+-rw-r--r--   0        0        0     3600 2022-01-13 13:52:14.795247 gitman-3.4b3/gitman/tests/test_shell.py
+-rw-r--r--   0        0        0      344 2022-01-13 13:52:14.734256 gitman-3.4b3/gitman/tests/utils.py
+-rw-r--r--   0        0        0     2096 2023-03-22 19:45:39.592580 gitman-3.4b3/pyproject.toml
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 gitman-3.4b3/setup.py
+-rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 gitman-3.4b3/PKG-INFO
```

### Comparing `gitman-3.4b2/LICENSE.md` & `gitman-3.4b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/README.md` & `gitman-3.4b3/README.md`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/__main__.py` & `gitman-3.4b3/gitman/__main__.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/cli.py` & `gitman-3.4b3/gitman/cli.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/commands.py` & `gitman-3.4b3/gitman/commands.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/common.py` & `gitman-3.4b3/gitman/common.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/exceptions.py` & `gitman-3.4b3/gitman/exceptions.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/git.py` & `gitman-3.4b3/gitman/git.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/models/config.py` & `gitman-3.4b3/gitman/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,29 +360,29 @@
         return sources + extras
 
     def _get_sources_filter(
         self, *names: str, sources: List[Source], skip_default_group: bool
     ) -> List[str]:
         """Get a filtered subset of sources."""
         names_list = list(names)
-
         if not names_list and not skip_default_group:
             names_list.append(self.default_group)
 
         # Add sources from groups
         groups_filter = [group for group in self.groups if group.name in names_list]
         sources_filter = [member for group in groups_filter for member in group.members]
 
         # Add independent sources
         sources_filter.extend(
             [source.name for source in sources if source.name in names_list]
         )
 
+        # Fall back to all sources if allowed
         if not sources_filter:
-            if names:
+            if names and names_list != ["all"]:
                 log.warn(f"No dependencies match: {' '.join(names)}")
             else:
                 sources_filter = [source.name for source in sources if source.name]
 
         return list(set(sources_filter))
```

### Comparing `gitman-3.4b2/gitman/models/group.py` & `gitman-3.4b3/gitman/models/group.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/models/source.py` & `gitman-3.4b3/gitman/models/source.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/plugin.py` & `gitman-3.4b3/gitman/plugin.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/settings.py` & `gitman-3.4b3/gitman/settings.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/shell.py` & `gitman-3.4b3/gitman/shell.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/conftest.py` & `gitman-3.4b3/gitman/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/files/gitman.yml` & `gitman-3.4b3/gitman/tests/files/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/files/subdir/gitman.yml` & `gitman-3.4b3/gitman/tests/files/subdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/files/subdir/subsubdir/gitman.yml` & `gitman-3.4b3/gitman/tests/files/subdir/subsubdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml` & `gitman-3.4b3/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_cli.py` & `gitman-3.4b3/gitman/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_commands.py` & `gitman-3.4b3/gitman/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_common.py` & `gitman-3.4b3/gitman/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_git.py` & `gitman-3.4b3/gitman/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_models_config.py` & `gitman-3.4b3/gitman/tests/test_models_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,21 +68,31 @@
     def test_install_with_names(self):
         """Verify the dependency list can be filtered."""
         config = Config(FILES)
 
         count = config.install_dependencies("gitman_2", "gitman_3")
         assert 2 == count
 
+    @pytest.mark.integration
+    def test_install_with_names_all(self):
+        """Verify all dependencies can be installed."""
+        config = Config(FILES)
+
+        count = config.install_dependencies("all")
+        assert 7 == count
+
+    @pytest.mark.integration
     def test_install_with_names_unknown(self):
         """Verify zero dependencies are installed with unknown dependency."""
         config = Config(FILES)
 
         count = config.install_dependencies("foobar")
         assert 0 == count
 
+    @pytest.mark.integration
     def test_install_with_depth_0(self):
         """Verify an install depth of 0 installs nothing."""
         config = Config(FILES)
 
         count = config.install_dependencies(depth=0)
         assert 0 == count
```

### Comparing `gitman-3.4b2/gitman/tests/test_models_source.py` & `gitman-3.4b3/gitman/tests/test_models_source.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_plugin.py` & `gitman-3.4b3/gitman/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/gitman/tests/test_shell.py` & `gitman-3.4b3/gitman/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `gitman-3.4b2/pyproject.toml` & `gitman-3.4b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "gitman"
-version = "3.4b2"
+version = "3.4b3"
 description = "A language-agnostic dependency manager using Git."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `gitman-3.4b2/setup.py` & `gitman-3.4b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'console_scripts': ['git-deps = gitman.plugin:main',
                      'gitman = gitman.cli:main']}
 
 setup_kwargs = {
     'name': 'gitman',
-    'version': '3.4b2',
+    'version': '3.4b3',
     'description': 'A language-agnostic dependency manager using Git.',
     'long_description': '## Overview\n\nGitman is a language-agnostic dependency manager using Git. It aims to serve as a submodules replacement and provides advanced options for managing versions of nested Git repositories.\n\n[![Demo](https://raw.githubusercontent.com/jacebrowning/gitman/main/docs/demo.gif)](https://asciinema.org/a/3DLos4HIU84P0AfFlZMYcgPus)\n\n[![Unix Build Status](https://img.shields.io/travis/com/jacebrowning/gitman/main.svg?label=unix)](https://travis-ci.com/jacebrowning/gitman)\n[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/gitman/main.svg?label=window)](https://ci.appveyor.com/project/jacebrowning/gitman)\n[![Coverage Status](https://img.shields.io/coveralls/jacebrowning/gitman/main.svg)](https://coveralls.io/r/jacebrowning/gitman)\n[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/gitman.svg)](https://scrutinizer-ci.com/g/jacebrowning/gitman/?branch=main)\n[![PyPI License](https://img.shields.io/pypi/l/gitman.svg)](https://pypi.org/project/gitman)\n[![PyPI Version](https://img.shields.io/pypi/v/gitman.svg)](https://pypi.org/project/gitman)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/gitman.svg?color=orange)](https://pypistats.org/packages/gitman)\n\n## Setup\n\n### Requirements\n\n- Python 3.8+\n- Git 2.8+ (with [stored credentials](http://gitman.readthedocs.io/en/latest/setup/git/))\n\n### Installation\n\nInstall this tool globally with [pipx](https://pipxproject.github.io/pipx/) (or pip):\n\n```sh\n$ pipx install gitman\n```\nor add it to your [Poetry](https://python-poetry.org/docs/) project:\n\n```sh\n$ poetry add gitman\n```\n\n### Configuration\n\nGenerate a sample config file:\n\n```sh\n$ gitman init\n```\n\nor manually create one (`gitman.yml` or `.gitman.yml`) in the root of your working tree:\n\n```yaml\nlocation: vendor/gitman\n\nsources:\n  - repo: "https://github.com/kstenerud/iOS-Universal-Framework"\n    name: framework\n    rev: Mk5-end-of-life\n  - repo: "https://github.com/jonreid/XcodeCoverage"\n    name: coverage\n    links:\n      - target: Tools/XcodeCoverage\n  - repo: "https://github.com/dxa4481/truffleHog"\n    name: trufflehog\n    rev: master\n    scripts:\n      - chmod a+x truffleHog/truffleHog.py\n  - repo: "https://github.com/FortAwesome/Font-Awesome"\n    name: fontawesome\n    rev: master\n    sparse_paths:\n      - "webfonts/*"\n  - repo: "https://github.com/google/material-design-icons"\n    name: material-design-icons\n    rev: master\n\ngroups:\n  - name: code\n    members:\n      - framework\n      - trufflehog\n  - name: resources\n    members:\n      - fontawesome\n      - material-design-icons\n\ndefault_group: code\n```\n\nIgnore the dependency storage location:\n\n```sh\n$ echo vendor/gitman >> .gitignore\n```\n\n## Usage\n\nSee the available commands:\n\n```sh\n$ gitman --help\n```\n\n### Updating Dependencies\n\nGet the latest versions of all dependencies:\n\n```sh\n$ gitman update\n```\n\nwhich will essentially:\n\n1. Create a working tree at `<root>`/`<location>`/`<name>`\n2. Fetch from `repo` and checkout the specified `rev`\n3. Symbolically link each `<location>`/`<name>` from `<root>`/`<link>` (if specified)\n4. Repeat for all nested working trees containing a config file\n5. Record the actual commit SHAs that were checked out (with `--lock` option)\n6. Run optional post-install scripts for each dependency\n\nwhere `rev` can be:\n\n- all or part of a commit SHA: `123def`\n- a tag: `v1.0`\n- a branch: `main`\n- a `rev-parse` date: `\'main@{2015-06-18 10:30:59}\'`\n\nAlternatively, get the latest versions of specific dependencies:\n\n```sh\n$ gitman update framework\n```\n\nor named groups:\n\n```sh\n$ gitman update resources\n```\n\n### Restoring Previous Versions\n\nDisplay the versions that are currently installed:\n\n```sh\n$ gitman list\n```\n\nReinstall these specific versions at a later time:\n\n```sh\n$ gitman install\n```\n\n### Deleting Dependencies\n\nRemove all installed dependencies:\n\n```sh\n$ gitman uninstall\n```\n\n## Resources\n\n- [Source code](https://github.com/jacebrowning/gitman)\n- [Issue tracker](https://github.com/jacebrowning/gitman/issues)\n- [Release history](https://github.com/jacebrowning/gitman/blob/main/CHANGELOG.md)\n',
     'author': 'Jace Browning',
     'author_email': 'jacebrowning@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/gitman',
```

### Comparing `gitman-3.4b2/PKG-INFO` & `gitman-3.4b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitman
-Version: 3.4b2
+Version: 3.4b3
 Summary: A language-agnostic dependency manager using Git.
 Home-page: https://pypi.org/project/gitman
 License: MIT
 Keywords: git,version control,build systems,dependency management,submodules
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
```

