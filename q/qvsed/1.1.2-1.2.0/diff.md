# Comparing `tmp/qvsed-1.1.2.tar.gz` & `tmp/qvsed-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.1.2.tar", last modified: Fri Jul  7 11:23:00 2023, max compression
+gzip compressed data, was "qvsed-1.2.0.tar", last modified: Fri Jul  7 12:30:11 2023, max compression
```

## Comparing `qvsed-1.1.2.tar` & `qvsed-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.670728 qvsed-1.1.2/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 qvsed-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      710 2023-07-07 11:23:00.669717 qvsed-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.649248 qvsed-1.1.2/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.1.2/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.1.2/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.1.2/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.1.2/QVSED/config_default.py
--rw-rw-rw-   0        0        0     8334 2023-07-07 11:18:15.000000 qvsed-1.1.2/QVSED/qvsed.py
--rw-rw-rw-   0        0        0     4080 2023-07-07 11:19:56.000000 qvsed-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.664726 qvsed-1.1.2/qvsed.egg-info/
--rw-rw-rw-   0        0        0      710 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 11:23:00.671740 qvsed-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-07-07 11:22:20.000000 qvsed-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:30:11.546534 qvsed-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 qvsed-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1245 2023-07-07 12:30:11.546534 qvsed-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 12:30:11.521017 qvsed-1.2.0/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.2.0/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.2.0/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.2.0/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.2.0/QVSED/config_default.py
+-rw-rw-rw-   0        0        0     8332 2023-07-07 12:27:40.000000 qvsed-1.2.0/QVSED/qvsed.py
+-rw-rw-rw-   0        0        0     5751 2023-07-07 12:20:45.000000 qvsed-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 12:30:11.543920 qvsed-1.2.0/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1245 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 12:30:11.000000 qvsed-1.2.0/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:30:11.546534 qvsed-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2023-07-07 12:29:15.000000 qvsed-1.2.0/setup.py
```

### Comparing `qvsed-1.1.2/LICENSE.txt` & `qvsed-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.1.2/QVSED/QVSED.ui` & `qvsed-1.2.0/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.1.2/QVSED/qvsed.py` & `qvsed-1.2.0/QVSED/qvsed.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,16 +170,15 @@
                 self.echo_area_update(f"Error opening file: {str(e)}")
 
     def show_help(self):
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
         help_message = """QVSED - Qt-based Volatile Small Editor
 ========================================
-
-QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files, licensed under the GNU General Public License version 3 or later.
+QVSED is a stateless, volatile text editor with a minimalist approach, focusing solely on text editing without file metadata or prompts for potentially destructive actions.
 
 This is the Text Area, where the actual editing takes place. Type anything you want into here, and edit as you please.
 Down there, below the Text Area is the Echo Area, where messages and errors will be displayed.
 On the left of the QVSED window is the Action Deck, containing commands to clear the Text area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
 I hope you enjoy using QVSED! I enjoyed writing it, and it's a nice little venture into my first Qt project.
```

### Comparing `qvsed-1.1.2/README.md` & `qvsed-1.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # QVSED - Qt-based Volatile Small Editor
 
-QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files.
+QVSED is a volatile text editor. "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded. Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata. You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
+
+QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more. QVSED's editing style is text-based, not file-based like basically every other editor out there. Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
+
+QVSED can be used as a simple scratchpad or throwaway editor, as well as a general editing software application, since it won't prompt you if you do anything destructive, It stays out of your way on many occasions. Whether or not that's a good thing is up to you.
 
 QVSED is a PyQt5 rewrite of my older project, [ASMED (Another SMol EDitor)](https://github.com/That1M8Head/ASMED), which was written using Windows Forms, and was quite obviously only for Windows.
 
 QVSED aims to replace ASMED by offering cross-platform support and the advantages of a lightweight editor without the overhead of .NET.
 
 ## Installing
 
@@ -20,36 +24,41 @@
 
 QVSED is free software, licensed under the GNU General Public License version 3 or later.
 
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
+The Action Deck contains editing commands, the Text Area is a text area, and the Echo Area is where messages will be printed.
+
 ![QVSED screenshot, showing the help message](qsved_screenie.png)
 
 ## Action Deck
 
-### Key
+The Action Deck, positioned on the left side of the QVSED window, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
-+ `C` - `Ctrl` (Windows, Linux), `⌘` (macOS)
-+ `A` - `Alt` (Windows, Linux), `⌥` (macOS)
+The Action Deck is on the left rather than on the top like a traditional menu bar, so that the buttons can be bigger while still providing enough screen real estate for the Text Area.
 
-### Commands
-
-**Clear Text** - `C-n` - Clear the Text Area. Think of it like New File.
+### Key Prefixes
 
-**Open File** - `C-f` - Launch a file picker and load the chosen file's contents into the Text Area.
++ `C-` - `Ctrl` (Windows, Linux), `⌘` (macOS)
++ `A-` - `Alt` (Windows, Linux), `⌥` (macOS)
 
-**Save File** - `C-s` - Launch a file picker and save the contents of the Text Area to the chosen file name.
+When you see `<C-n>`, for instance, that means pressing `Ctrl+N` on Windows/Linux, or `⌘N` on macOS.
 
-**Full Screen** - `A-f` - Toggle full screen mode.
+This kind of notation was inspired by Emacs (though, QVSED uses `A-` instead of `M-` to be clearer).
 
-**Get Help** - `C-h` - Show a help message in the Text Area. This will overwrite your current work.
+### Commands
 
-**Quit QVSED**  - `A-q` - Quit QVSED on the spot with no confirmation dialog.
++ **Clear Text** - `<C-n>` - Clear the Text Area. Think of it like New File.
++ **Open File** - `<C-f>` - Launch a file picker and load the chosen file's contents into the Text Area.
++ **Save File** - `<C-s>` - Launch a file picker and save the contents of the Text Area to the chosen file name.
++ **Full Screen** - `<A-f>` - Toggle full screen mode.
++ **Get Help** - `<C-h>` - Show a help message in the Text Area. This will overwrite your current work.
++ **Quit QVSED**  - `<A-q>` - Quit QVSED on the spot with no confirmation dialog.
 
 ## Text Area
 
 The Text Area is where the actual text editing takes place.
 
 You can enter and delete text, scroll down and up, cut, copy, paste, all that standard Notepad stuff.
 
@@ -67,15 +76,15 @@
 
 When QVSED is started, it looks for a configuration file. If it can't find one, it creates one and populates it with defaults.
 
 On Windows, the configuration file will be stored at `C:\Users\<username>\AppData\Roaming\QVSED\config.py`, where `<username>` is your Windows username.
 
 On *nix systems, the configuration file will be stored at `~/.config/QVSED/config.py`, where `~` is your home directory (`/home/<username>`).
 
-The configuration file currently only supports two options to configure: `font_family` and `font_size`.
+At the moment, QVSED currently only supports two options to configure, `font_family` and `font_size`.
 
 ```python
 # The default QVSED config.
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 ```
```

