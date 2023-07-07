# Comparing `tmp/gitmopy-0.4.0.tar.gz` & `tmp/gitmopy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.4.0.tar", max compression
+gzip compressed data, was "gitmopy-0.4.1.tar", max compression
```

## Comparing `gitmopy-0.4.0.tar` & `gitmopy-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.4.0/LICENSE
--rw-r--r--   0        0        0     7978 2023-06-30 23:12:55.485417 gitmopy-0.4.0/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.4.0/gitmopy/__init__.py
--rw-r--r--   0        0        0    15715 2023-06-30 23:12:55.486562 gitmopy-0.4.0/gitmopy/cli.py
--rw-r--r--   0        0        0     8580 2023-06-30 23:12:55.487270 gitmopy-0.4.0/gitmopy/constants.py
--rw-r--r--   0        0        0     6899 2023-06-30 23:12:55.488544 gitmopy-0.4.0/gitmopy/git.py
--rw-r--r--   0        0        0     3218 2023-06-30 23:12:55.489041 gitmopy-0.4.0/gitmopy/history.py
--rw-r--r--   0        0        0     8690 2023-06-30 23:12:55.489763 gitmopy-0.4.0/gitmopy/prompt.py
--rw-r--r--   0        0        0     7413 2023-06-30 23:12:55.490210 gitmopy-0.4.0/gitmopy/utils.py
--rw-r--r--   0        0        0      578 2023-06-30 23:12:55.490739 gitmopy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 gitmopy-0.4.0/setup.py
--rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 gitmopy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7978 2023-07-07 18:31:52.869588 gitmopy-0.4.1/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.4.1/gitmopy/__init__.py
+-rw-r--r--   0        0        0    15714 2023-07-07 18:31:01.609331 gitmopy-0.4.1/gitmopy/cli.py
+-rw-r--r--   0        0        0     8580 2023-06-30 23:12:55.487270 gitmopy-0.4.1/gitmopy/constants.py
+-rw-r--r--   0        0        0     6899 2023-06-30 23:12:55.488544 gitmopy-0.4.1/gitmopy/git.py
+-rw-r--r--   0        0        0     3218 2023-06-30 23:12:55.489041 gitmopy-0.4.1/gitmopy/history.py
+-rw-r--r--   0        0        0     8690 2023-06-30 23:12:55.489763 gitmopy-0.4.1/gitmopy/prompt.py
+-rw-r--r--   0        0        0     7413 2023-06-30 23:12:55.490210 gitmopy-0.4.1/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-07-07 18:31:40.403560 gitmopy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 gitmopy-0.4.1/setup.py
+-rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 gitmopy-0.4.1/PKG-INFO
```

### Comparing `gitmopy-0.4.0/LICENSE` & `gitmopy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/README.md` & `gitmopy-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version      : 0.4.0
+  version      : 0.4.1
   app path     : /Users/victor/.gitmopy
   history      : /Users/victor/.gitmopy/history.json
   config       : /Users/victor/.gitmopy/config.yaml
   custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml
 
 Current configuration:
   skip_scope      : False
```

### Comparing `gitmopy-0.4.0/gitmopy/cli.py` & `gitmopy-0.4.1/gitmopy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
                 break
 
         if not dry:
             # no staged files and user does not want to add: abort
             if not status["staged"] and not add:
                 print(
                     col(
-                        +"\nNo staged files. Stage files yourself or use [b]--add[/b]"
+                        "\nNo staged files. Stage files yourself or use [b]--add[/b]"
                         + " to add all unstaged files.\n",
                         "y",
                     )
                 )
                 raise typer.Exit(1)
             if remote and not push:
                 print(col("\nIgnoring --remote flag because --push is not set\n", "y"))
```

### Comparing `gitmopy-0.4.0/gitmopy/constants.py` & `gitmopy-0.4.1/gitmopy/constants.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/gitmopy/git.py` & `gitmopy-0.4.1/gitmopy/git.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/gitmopy/history.py` & `gitmopy-0.4.1/gitmopy/history.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/gitmopy/prompt.py` & `gitmopy-0.4.1/gitmopy/prompt.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/gitmopy/utils.py` & `gitmopy-0.4.1/gitmopy/utils.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.4.0/pyproject.toml` & `gitmopy-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.4.0"
+version = "0.4.1"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.4.0/setup.py` & `gitmopy-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'A python command-line for gitmoji',
-    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji convention: [gitmoji.dev/](https://gitmoji.dev/)\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\nUse your own emojis by editing the "custom emojis" file listed by `gitmopy info`!\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version      : 0.4.0\n  app path     : /Users/victor/.gitmopy\n  history      : /Users/victor/.gitmopy/history.json\n  config       : /Users/victor/.gitmopy/config.yaml\n  custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * [typer.tiangolo.com/tutorial/testing/](https://typer.tiangolo.com/tutorial/testing/)\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
+    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji convention: [gitmoji.dev/](https://gitmoji.dev/)\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\nUse your own emojis by editing the "custom emojis" file listed by `gitmopy info`!\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version      : 0.4.1\n  app path     : /Users/victor/.gitmopy\n  history      : /Users/victor/.gitmopy/history.json\n  config       : /Users/victor/.gitmopy/config.yaml\n  custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * [typer.tiangolo.com/tutorial/testing/](https://typer.tiangolo.com/tutorial/testing/)\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gitmopy-0.4.0/PKG-INFO` & `gitmopy-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -105,15 +105,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version      : 0.4.0
+  version      : 0.4.1
   app path     : /Users/victor/.gitmopy
   history      : /Users/victor/.gitmopy/history.json
   config       : /Users/victor/.gitmopy/config.yaml
   custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml
 
 Current configuration:
   skip_scope      : False
```

