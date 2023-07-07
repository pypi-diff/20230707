# Comparing `tmp/tui_typer_tutor-1.0.1.tar.gz` & `tmp/tui_typer_tutor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_typer_tutor-1.0.1.tar", max compression
+gzip compressed data, was "tui_typer_tutor-1.1.0.tar", max compression
```

## Comparing `tui_typer_tutor-1.0.1.tar` & `tui_typer_tutor-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-06-24 01:02:07.591613 tui_typer_tutor-1.0.1/LICENSE
--rw-r--r--   0        0        0     1709 2023-06-28 01:28:44.476366 tui_typer_tutor-1.0.1/docs/README.md
--rw-r--r--   0        0        0     1565 2023-06-28 01:28:40.135432 tui_typer_tutor-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-28 01:28:40.128121 tui_typer_tutor-1.0.1/tui_typer_tutor/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 09:58:56.713475 tui_typer_tutor-1.0.1/tui_typer_tutor/app/__init__.py
--rw-r--r--   0        0        0      659 2023-06-28 01:18:02.055916 tui_typer_tutor-1.0.1/tui_typer_tutor/app/ttt.py
--rw-r--r--   0        0        0       51 2023-06-26 01:07:36.370648 tui_typer_tutor-1.0.1/tui_typer_tutor/constants/__init__.py
--rw-r--r--   0        0        0     1208 2023-06-27 12:45:23.879196 tui_typer_tutor-1.0.1/tui_typer_tutor/constants/display_to_textual.py
--rw-r--r--   0        0        0        0 2023-06-25 00:11:43.547397 tui_typer_tutor-1.0.1/tui_typer_tutor/core/__init__.py
--rw-r--r--   0        0        0      554 2023-06-27 12:42:22.407622 tui_typer_tutor-1.0.1/tui_typer_tutor/core/config.py
--rw-r--r--   0        0        0     1856 2023-06-27 02:07:23.253288 tui_typer_tutor-1.0.1/tui_typer_tutor/core/metrics.py
--rw-r--r--   0        0        0       46 2023-06-25 23:10:12.527578 tui_typer_tutor-1.0.1/tui_typer_tutor/core/scrolled_labels.py
--rw-r--r--   0        0        0      537 2023-06-28 01:17:23.376603 tui_typer_tutor-1.0.1/tui_typer_tutor/core/seed_data.py
--rw-r--r--   0        0        0      155 2023-06-26 01:46:19.175089 tui_typer_tutor-1.0.1/tui_typer_tutor/core/seed_data.txt
--rw-r--r--   0        0        0     2010 2023-06-27 12:45:17.269183 tui_typer_tutor-1.0.1/tui_typer_tutor/core/typing.py
--rw-r--r--   0        0        0      844 2023-06-27 12:51:26.782478 tui_typer_tutor-1.0.1/tui_typer_tutor/core/uninstall.py
--rw-r--r--   0        0        0        0 2023-06-24 09:59:11.688594 tui_typer_tutor-1.0.1/tui_typer_tutor/screens/__init__.py
--rw-r--r--   0        0        0     1135 2023-06-28 01:18:02.056168 tui_typer_tutor-1.0.1/tui_typer_tutor/screens/help.py
--rw-r--r--   0        0        0     4225 2023-06-28 01:18:02.056517 tui_typer_tutor-1.0.1/tui_typer_tutor/screens/main.py
--rw-r--r--   0        0        0     1196 2023-06-27 12:51:26.782624 tui_typer_tutor-1.0.1/tui_typer_tutor/scripts.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 tui_typer_tutor-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-24 01:02:07.591613 tui_typer_tutor-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2780 2023-07-07 09:55:11.938058 tui_typer_tutor-1.1.0/docs/README.md
+-rw-r--r--   0        0        0     1527 2023-07-07 09:55:06.667130 tui_typer_tutor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-07-07 09:55:06.660826 tui_typer_tutor-1.1.0/tui_typer_tutor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 09:58:56.713475 tui_typer_tutor-1.1.0/tui_typer_tutor/app/__init__.py
+-rw-r--r--   0        0        0      659 2023-06-28 01:18:02.055916 tui_typer_tutor-1.1.0/tui_typer_tutor/app/ttt.py
+-rw-r--r--   0        0        0       51 2023-06-26 01:07:36.370648 tui_typer_tutor-1.1.0/tui_typer_tutor/constants/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-01 23:10:42.700299 tui_typer_tutor-1.1.0/tui_typer_tutor/constants/display_to_textual.py
+-rw-r--r--   0        0        0        0 2023-06-25 00:11:43.547397 tui_typer_tutor-1.1.0/tui_typer_tutor/core/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-27 12:42:22.407622 tui_typer_tutor-1.1.0/tui_typer_tutor/core/config.py
+-rw-r--r--   0        0        0     1824 2023-06-29 12:13:08.507232 tui_typer_tutor-1.1.0/tui_typer_tutor/core/metrics.py
+-rw-r--r--   0        0        0       46 2023-06-25 23:10:12.527578 tui_typer_tutor-1.1.0/tui_typer_tutor/core/scrolled_labels.py
+-rw-r--r--   0        0        0      537 2023-06-28 01:17:23.376603 tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.py
+-rw-r--r--   0        0        0      322 2023-07-01 23:10:42.700361 tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.txt
+-rw-r--r--   0        0        0     2010 2023-06-27 12:45:17.269183 tui_typer_tutor-1.1.0/tui_typer_tutor/core/typing.py
+-rw-r--r--   0        0        0      844 2023-06-27 12:51:26.782478 tui_typer_tutor-1.1.0/tui_typer_tutor/core/uninstall.py
+-rw-r--r--   0        0        0        0 2023-06-24 09:59:11.688594 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/__init__.py
+-rw-r--r--   0        0        0     1135 2023-06-28 01:18:02.056168 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/help.py
+-rw-r--r--   0        0        0     4455 2023-07-01 23:06:03.898939 tui_typer_tutor-1.1.0/tui_typer_tutor/screens/main.py
+-rw-r--r--   0        0        0     1082 2023-06-29 12:08:41.177093 tui_typer_tutor-1.1.0/tui_typer_tutor/scripts.py
+-rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 tui_typer_tutor-1.1.0/PKG-INFO
```

### Comparing `tui_typer_tutor-1.0.1/LICENSE` & `tui_typer_tutor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/docs/README.md` & `tui_typer_tutor-1.1.0/docs/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,65 @@
 # tui-typer-tutor
 
+![.github/assets/demo.gif](https://raw.githubusercontent.com/KyleKing/tui-typer-tutor/main/.github/assets/demo.gif)
+
+Uncomplicated terminal typing practice.
+
 Fork of `kraanzu/termtyper` with a focus on special characters. Inspired by `climech/typing-practice` and `justinsgithub/terminal-typing-tutor`.
 
-## Installation and Usage
+## Installation
+
+[Install with `pipx`](https://pypi.org/project/pipx/)
+
+```sh
+pipx install tui-typer-tutor
+```
+
+## Usage
+
+Launch a typing session with the default text:
+
+```sh
+ttt
+```
+
+Or specify custom files with:
+
+```sh
+ttt --seed-file='./any-file.txt'
+```
+
+To uninstall run:
+
+```sh
+ttt --uninstall && pipx uninstall tui-typer-tutor
+```
+
+### Keys
+
+This app supports a few unicode characters when found in the seed file:
+
+- tab: `→`
+- shift+tab: `←`
+- enter/return: `⏎`
+- escape: `␛`
+
+[All supported characters are documented here](https://github.com/KyleKing/tui-typer-tutor/blob/main/tui_typer_tutor/constants/display_to_textual.py). `Ctrl` key combinations aren't yet supported and appear as an unknown character.
+
+### Seed File
+
+The algorithm for generating the expected text is:
+
+1. Load each line of the seed file
+1. Reorder randomly (keeping each line of text together)
+1. Join without a delimeter keeping any leading white space per line
+
+The default seed file is here: [./tui_typer_tutor/core/seed_data.txt](https://github.com/KyleKing/tui-typer-tutor/blob/main/tui_typer_tutor/core/seed_data.txt)
 
-1. `pipx install tui-typer-tutor`
-1. Launch a typing session with the default text: `ttt`
-1. Specify custom files with: `ttt --seed-file='./any-file.txt'`
-1. To uninstall run: `ttt --uninstall && pipx uninstall tui-typer-tutor`
+Ideas for better seed text generation are welcome!
 
 ## Project Status
 
 See the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tui_typer_tutor-1.0.1/pyproject.toml` & `tui_typer_tutor-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.0.1"
+version = "1.1.0"
 version_files = ["pyproject.toml:^version", "tui_typer_tutor/__init__.py:^__version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 1 - Planning",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.11",
 ] # https://pypi.org/classifiers/
-description = "Fork of kraanzu/termtyper with a focus on special characters. Inspired by climech/typing-practice."
+description = "Uncomplicated terminal typing practice."
 documentation = "https://tui-typer-tutor.kyleking.me"
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "tui_typer_tutor"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/tui-typer-tutor"
-version = "1.0.1"
+version = "1.1.0"
 
 [tool.poetry.dependencies]
 python = "^3.11.2"
+arguably = ">=1.2.5"
 bidict = ">=0.22.1"
 corallium = ">=0.2.2"
 platformdirs = ">=3.8.0"
 pydantic = ">=1.10.9"
 textual = ">=0.28.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/app/ttt.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/app/ttt.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/constants/display_to_textual.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/constants/display_to_textual.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     '^': 'circumflex_accent',
     '_': 'underscore',
     '`': 'grave_accent',
     '{': 'left_curly_bracket',
     '|': 'vertical_line',
     '}': 'right_curly_bracket',
     '~': 'tilde',
+    '←': 'shift+tab',
+    '→': 'tab',
     '⏎': 'enter',
     '␛': 'escape',
 }
 
 DISPLAY_TO_TEXTUAL = bidict({
     **_special_keys,
     **dict(zip(ascii_letters, ascii_letters, strict=True)),
```

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/core/config.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/core/config.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/core/metrics.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/core/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,18 @@
         """Initialize Metrics based on the filename."""
         return cls(filename=filename, session_start=utcnow())
 
     def end_session(self, keys: Keys) -> 'SessionMetrics':  # noqa: RBT002
         """Update the typed counters based on `Keys`."""
         self.session_end = utcnow()
         for key in keys.typed_all:
-            if key.expected:
-                if key.was_correct:
-                    self.typed_correct += 1
-                else:
-                    self.typed_incorrect += 1
+            if key.was_correct:
+                self.typed_correct += 1
+            elif key.expected:
+                self.typed_incorrect += 1
         return self
 
 
 @beartype
 def append_csv(metrics: SessionMetrics) -> None:
     """Write metrics to the global CSV."""
     csv_path = get_cache_dir() / 'metrics.csv'
```

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/core/seed_data.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/core/seed_data.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/core/typing.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/core/typing.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/core/uninstall.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/core/uninstall.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/screens/help.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/screens/help.py`

 * *Files identical despite different names*

### Comparing `tui_typer_tutor-1.0.1/tui_typer_tutor/screens/main.py` & `tui_typer_tutor-1.1.0/tui_typer_tutor/screens/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     BINDINGS: ClassVar[list[Binding]] = [  # type: ignore[assignment]
         Binding('ctrl+q', 'save_and_quit', 'Save and Quit'),
     ]
 
     keys: Keys
     metrics: SessionMetrics
+    width: int = 0
 
     def action_save_and_quit(self) -> None:
         """Save and quit."""
         append_csv(self.metrics.end_session(self.keys))
         # TODO: Print out or display a success message on completion!
         sys.exit(0)
 
@@ -95,26 +96,32 @@
         cont = self.query_one('#text-container', Horizontal)
         for key in self.keys.expected:  # FYI: Mounts all expected keys and crops
             cont.mount(Label(key.text, classes='text'))
 
     @beartype
     def on_key(self, event: Key) -> None:  # noqa: CAC001
         """Capture all key presses and show in the typed input."""
+        if event.key in {'ctrl+q', 'ctrl+backslash'}:
+            return  # ignore bound keys
+
         try:
             on_keypress(event.key, self.keys)
         except AtEndOfExpectedError:
             self.action_save_and_quit()
 
-        width = len(self.keys.typed)
         if self.keys.last_was_delete:
+            if self.width:
+                self.width -= 1
             with suppress(NoMatches):
                 self.query('Label.typed').last().remove()
-        elif width:
+                self.query_one('#typed-unknown', Label).update('')
+        else:
+            self.width += 1
             cursor_width = MAX_CHARS - CHAR_OFFSET
-            if width >= cursor_width:
+            if self.width >= cursor_width:
                 self.query('Label.typed').first().remove()
                 self.query('Label.text').first().remove()
             # Choose the class
             color_class = 'success'
             display_text = self.keys.typed[-1].text
             if not self.keys.typed[-1].was_correct:
                 color_class = 'error'
```

