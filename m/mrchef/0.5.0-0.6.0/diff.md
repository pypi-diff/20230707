# Comparing `tmp/mrchef-0.5.0.tar.gz` & `tmp/mrchef-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrchef-0.5.0.tar", max compression
+gzip compressed data, was "mrchef-0.6.0.tar", max compression
```

## Comparing `mrchef-0.5.0.tar` & `mrchef-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-17 06:23:46.499987 mrchef-0.5.0/LICENSE
--rw-r--r--   0        0        0     5000 2023-05-17 06:23:46.499987 mrchef-0.5.0/README.md
--rw-r--r--   0        0        0       55 2023-05-17 06:23:46.499987 mrchef-0.5.0/mrchef/__init__.py
--rw-r--r--   0        0        0      177 2023-05-17 06:23:46.499987 mrchef-0.5.0/mrchef/__main__.py
--rw-r--r--   0        0        0     4857 2023-05-17 06:23:46.499987 mrchef-0.5.0/mrchef/cli.py
--rw-r--r--   0        0        0    25176 2023-05-17 06:23:46.500987 mrchef-0.5.0/mrchef/lib.py
--rw-r--r--   0        0        0      964 2023-05-17 06:23:46.500987 mrchef-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 mrchef-0.5.0/setup.py
--rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 mrchef-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 05:52:08.782651 mrchef-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5291 2023-07-07 05:52:08.783651 mrchef-0.6.0/README.md
+-rw-r--r--   0        0        0       55 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/__main__.py
+-rw-r--r--   0        0        0     4857 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/cli.py
+-rw-r--r--   0        0        0    25292 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/lib.py
+-rw-r--r--   0        0        0      985 2023-07-07 05:52:08.784651 mrchef-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 mrchef-0.6.0/setup.py
+-rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 mrchef-0.6.0/PKG-INFO
```

### Comparing `mrchef-0.5.0/LICENSE` & `mrchef-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrchef-0.5.0/README.md` & `mrchef-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,19 @@
 understand how to use them. Ready to replace git submodules?
 
 Keep in mind this if using nix:
 
 -   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541
     or https://github.com/NixOS/nix/issues/5119 are fixed.
 
+-   Most mrchef-based derivations will benefit a lot from pre-filtering the sources
+    before the build. Typically, by just including `./mrchef.toml`,
+    `./.mrchef.freezer.toml` and `./kitchen/` (if it exists and the kitchen is named
+    like that), you will have all you need to build.
+
 ## Who
 
 Created and maintained by [Moduon Team](https://www.moduon.team/).
 
 Original idea by [Jairo Llopis](https://www.recallstack.icu/).
 
 ## Where
```

### Comparing `mrchef-0.5.0/mrchef/cli.py` & `mrchef-0.6.0/mrchef/cli.py`

 * *Files identical despite different names*

### Comparing `mrchef-0.5.0/mrchef/lib.py` & `mrchef-0.6.0/mrchef/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from shutil import rmtree
 from textwrap import dedent
 from typing import Optional
 
 import coloredlogs
 import requests
 import tomlkit
+from git_find_repos import find_repos
 from plumbum import local
 from plumbum.commands.processes import ProcessExecutionError
 
 CONFIG_FILE = "mrchef.toml"
 FREEZER_FILE = ".mrchef.freezer.toml"
 
 logger = getLogger("mrchef")
@@ -209,15 +210,15 @@
 
     def hot_meals(self) -> dict[str, Meal]:
         """Get info from the hot meals found in the kitchen."""
         result = {}
         if not self.kitchen.is_dir():
             return result
         self._cache_spices()
-        for meal_path in self.kitchen.glob("**/.git/.."):
+        for meal_path in map(Path, find_repos(self.kitchen)):
             meal_path = meal_path.resolve()
             if not git_is_repo(meal_path):
                 continue
             key = str(meal_path.relative_to(self.kitchen))
             branch = git_branch(meal_path)
             url = self.config_user.get(key, {}).get("url") or git_origin(meal_path)
             remote_head = git_remote_head(meal_path, url, branch)
@@ -390,15 +391,17 @@
         for name, meal in sorted(self.hot_meals().items()):
             assert meal.rev
             new_freezer["meals"][name] = {
                 "rev": meal.rev,
             }
             for spice_url in meal.spices:
                 spice_content = self._get_spice_content(spice_url)
-                new_freezer["spices"][spice_url] = spice_content
+                new_freezer["spices"][spice_url] = tomlkit.api.string(
+                    spice_content, multiline=True
+                )
                 for patch_id in git_get_patch_ids_map(meal.path, spice_content):
                     new_freezer["patch2spice"][patch_id] = spice_url
         with self.freezer_file.open("w") as fd:
             fd.write("# MrChef's freezer. MANUAL CHANGES WILL BE OVERRIDDEN.\n")
             tomlkit.dump(new_freezer, fd)
         # Because maybe we detected hot patches in the mean time
         self.update_user_config()
```

### Comparing `mrchef-0.5.0/pyproject.toml` & `mrchef-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mrchef"
-version = "0.5.0"
+version = "0.6.0"
 description = "Metarepo Chef"
 authors = ["Moduon <info@moduon.team>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/moduon/mrchef"
 
 [tool.poetry.scripts]
@@ -12,14 +12,15 @@
 mrchef = "mrchef.__main__:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 coloredlogs = ">=15.0.1"
 decorator = ">=5.1.1"
 git-autoshare = ">=1.0.0-beta.6"
+git-find-repos = ">=2.1.0"
 mergedeep = ">=1.3.4"
 plumbum = ">=1.7.2"
 requests = ">=2.27.1"
 tomlkit = ">=0.10.0"
 xdg = ">=5.1.1"
 
 [tool.poetry.group.dev.dependencies]
@@ -29,14 +30,12 @@
 [tool.pydocstyle]
 convention = "google"
 ignore_decorators = "handle_error"
 
 [tool.pytest.ini_options]
 addopts = "-n auto -ra"
 testpaths = ["tests"]
-markers = [
-    "impure: tests that depend on network access or external sources"
-]
+markers = ["impure: tests that depend on network access or external sources"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mrchef-0.5.0/setup.py` & `mrchef-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['coloredlogs>=15.0.1',
  'decorator>=5.1.1',
  'git-autoshare>=1.0.0-beta.6',
+ 'git-find-repos>=2.1.0',
  'mergedeep>=1.3.4',
  'plumbum>=1.7.2',
  'requests>=2.27.1',
  'tomlkit>=0.10.0',
  'xdg>=5.1.1']
 
 entry_points = \
 {'console_scripts': ['mrchef = mrchef.__main__:run']}
 
 setup_kwargs = {
     'name': 'mrchef',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Metarepo Chef',
-    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n-   Code is 100% reproducible.\n-   Full freeze-warmup-freeze coding cycle.\n-   Upstream patching supported.\n-   Downstream patching supported.\n-   Mixed and multi-patching repo supported.\n-   Automated updates.\n-   Automatic disk space economization with [git-autoshare][].\n-   Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n-   Use separate repos and glue them together through packaging. But what if some code\n    you need isn't properly packaged? What if some dependencies need more than 1 patch\n    to work?\n-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n    some parts are open source and you need to upstream or review changes?\n-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n    that requires that every time you do a `git checkout`... or almost any git\n    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_\n    of headaches when you move files around and perform basically any operation. And\n    what if you need to merge 2 upstream patches?\n-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,\n    you need even more deep knowledge than with submodules to be able to review or\n    publish patches. And again, how to merge more than one patch?\n-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't\n    ready for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n-   _Buffet_ is the main git repository that contains all the instructions to build it.\n-   The _config file_ is a file named `mrchef.toml` that stands in the root of your\n    _buffet_ and configures what Mr. Chef should do.\n-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the\n    _meals_. It's configured inside the _config file_.\n-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n-   A _spice_ is a patch that is added to a _meal_.\n-   The _freezer_ is where we store the gory details needed to make the kitchen 100%\n    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n    _kitchen_, ready to cook!\n-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n    up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nInstall it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\nGo read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into\naggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to\nunderstand how to use them. Ready to replace git submodules?\n\nKeep in mind this if using nix:\n\n-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541\n    or https://github.com/NixOS/nix/issues/5119 are fixed.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
+    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n-   Code is 100% reproducible.\n-   Full freeze-warmup-freeze coding cycle.\n-   Upstream patching supported.\n-   Downstream patching supported.\n-   Mixed and multi-patching repo supported.\n-   Automated updates.\n-   Automatic disk space economization with [git-autoshare][].\n-   Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n-   Use separate repos and glue them together through packaging. But what if some code\n    you need isn't properly packaged? What if some dependencies need more than 1 patch\n    to work?\n-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n    some parts are open source and you need to upstream or review changes?\n-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n    that requires that every time you do a `git checkout`... or almost any git\n    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_\n    of headaches when you move files around and perform basically any operation. And\n    what if you need to merge 2 upstream patches?\n-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,\n    you need even more deep knowledge than with submodules to be able to review or\n    publish patches. And again, how to merge more than one patch?\n-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't\n    ready for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n-   _Buffet_ is the main git repository that contains all the instructions to build it.\n-   The _config file_ is a file named `mrchef.toml` that stands in the root of your\n    _buffet_ and configures what Mr. Chef should do.\n-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the\n    _meals_. It's configured inside the _config file_.\n-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n-   A _spice_ is a patch that is added to a _meal_.\n-   The _freezer_ is where we store the gory details needed to make the kitchen 100%\n    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n    _kitchen_, ready to cook!\n-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n    up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nInstall it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\nGo read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into\naggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to\nunderstand how to use them. Ready to replace git submodules?\n\nKeep in mind this if using nix:\n\n-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541\n    or https://github.com/NixOS/nix/issues/5119 are fixed.\n\n-   Most mrchef-based derivations will benefit a lot from pre-filtering the sources\n    before the build. Typically, by just including `./mrchef.toml`,\n    `./.mrchef.freezer.toml` and `./kitchen/` (if it exists and the kitchen is named\n    like that), you will have all you need to build.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
     'author': 'Moduon',
     'author_email': 'info@moduon.team',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/moduon/mrchef',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mrchef-0.5.0/PKG-INFO` & `mrchef-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrchef
-Version: 0.5.0
+Version: 0.6.0
 Summary: Metarepo Chef
 Home-page: https://gitlab.com/moduon/mrchef
 License: GPL-3.0-or-later
 Author: Moduon
 Author-email: info@moduon.team
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1)
 Requires-Dist: decorator (>=5.1.1)
 Requires-Dist: git-autoshare (>=1.0.0-beta.6)
+Requires-Dist: git-find-repos (>=2.1.0)
 Requires-Dist: mergedeep (>=1.3.4)
 Requires-Dist: plumbum (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: tomlkit (>=0.10.0)
 Requires-Dist: xdg (>=5.1.1)
 Project-URL: Repository, https://gitlab.com/moduon/mrchef
 Description-Content-Type: text/markdown
@@ -165,14 +166,19 @@
 understand how to use them. Ready to replace git submodules?
 
 Keep in mind this if using nix:
 
 -   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541
     or https://github.com/NixOS/nix/issues/5119 are fixed.
 
+-   Most mrchef-based derivations will benefit a lot from pre-filtering the sources
+    before the build. Typically, by just including `./mrchef.toml`,
+    `./.mrchef.freezer.toml` and `./kitchen/` (if it exists and the kitchen is named
+    like that), you will have all you need to build.
+
 ## Who
 
 Created and maintained by [Moduon Team](https://www.moduon.team/).
 
 Original idea by [Jairo Llopis](https://www.recallstack.icu/).
 
 ## Where
```

