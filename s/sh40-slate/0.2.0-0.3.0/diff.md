# Comparing `tmp/sh40_slate-0.2.0.tar.gz` & `tmp/sh40_slate-0.3.0.tar.gz`

## Comparing `sh40_slate-0.2.0.tar` & `sh40_slate-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/__about__.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/__init__.py
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/color.py
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/color_info.py
--rw-r--r--   0        0        0    11061 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/core.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/event.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/key_names.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/screen.py
--rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/span.py
--rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_color.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_core.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_event.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_screen.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_span.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_terminal.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/LICENSE
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/README.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/__about__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/__init__.py
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/color.py
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/color_info.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/core.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/event.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/key_names.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/screen.py
+-rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/span.py
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/slate/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_color.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_core.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_event.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_screen.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_span.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/tests/test_terminal.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/LICENSE
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/README.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 sh40_slate-0.3.0/PKG-INFO
```

### Comparing `sh40_slate-0.2.0/slate/color.py` & `sh40_slate-0.3.0/slate/color.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/slate/color_info.py` & `sh40_slate-0.3.0/slate/color_info.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/slate/core.py` & `sh40_slate-0.3.0/slate/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         stream: The stream to write the query to. Uses `sys.stdout` by default.
 
     Return:
         A hexadecimal triplet with the format `rrggbb`. Note that it doesn't include
         a leading hash.
     """
 
-    if not stream.isatty():
+    if not sys.stdin.isatty():
         return DEFAULT_COLOR_DEFAULTS[layer]
 
     stream.flush()
     stream.write(f"\x1b]{layer};?\007")
     stream.flush()
 
     reply = getch()
@@ -154,14 +154,18 @@
     """Gets the maximum supported color system supported by the shell environment.
 
     Returns:
         The highest-supported color system in the terminal. If `$NO_COLOR` is set,
         `ColorSpace.NO_COLOR` will always be returned.
     """
 
+    shell_sys = os.getenv("SLATE_COLORSYS")
+    if shell_sys is not None:
+        return ColorSpace(shell_sys.lower())
+
     if os.getenv("NO_COLOR") is not None:
         return ColorSpace.NO_COLOR
 
     term = os.getenv("TERM", "")
     color_term = os.getenv("COLORTERM", "").strip().lower()
 
     if color_term == "":
@@ -351,14 +355,17 @@
         raw: If set, the returned string will not be converted to its canonical name,
             e.g. '\\x1b[D' -> 'left' or '\\x01' -> 'ctrl-a'.
 
     Returns:
         The longest sequence of characters that could be read from the stream.
     """
 
+    if not stream.isatty():
+        return ""
+
     if os.name == "nt":
         key = _getch_nt()
 
         if raw:
             return key
 
         return NT_KEY_NAMES.get(key, key)
```

### Comparing `sh40_slate-0.2.0/slate/event.py` & `sh40_slate-0.3.0/slate/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 """The basic Event class used by the rest of the library."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Callable
+from typing import Any, Callable, Union
+
+EventCallback = Union[Callable[[], Any], Callable[[Any], Any]]
+
+__all__ = [
+    "Event",
+    "EventCallback",
+    "CallbackError",
+]
 
 
 class CallbackError(Exception):
     """Raised when something went wrong with an event's callback"""
 
 
 @dataclass
@@ -17,22 +25,22 @@
     Construct an event and store it in a variable to have a reference for it. Then, you
     can `+=` callback handlers onto it, and call the event object with data to notify
     all of the callbacks.
     """
 
     name: str
 
-    _listeners: list[Callable[[Any], Any]] = field(default_factory=list)
+    _listeners: list[EventCallback] = field(default_factory=list)
 
     def __bool__(self) -> bool:
         """Returns whether this event has any listeners."""
 
         return len(self._listeners) > 0
 
-    def __iadd__(self, callback: Any) -> Event:
+    def __iadd__(self, callback: EventCallback) -> Event:
         if not callable(callback):
             raise ValueError(f"Invalid type for callback: {callback}")
 
         self._listeners.append(callback)
 
         return self
```

### Comparing `sh40_slate-0.2.0/slate/key_names.py` & `sh40_slate-0.3.0/slate/key_names.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/slate/screen.py` & `sh40_slate-0.3.0/slate/screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,18 @@
         changes = 0
 
         for span in spans:
             for char in span.get_characters(always_include_sequence=True):
                 if self.width <= x or x < 0 or self.height <= y or y < 0:
                     break
 
+                if char == "\n":
+                    y += 1
+                    continue
+
                 next_x, next_y = x + 1, y
 
                 if next_x >= self.width:
                     next_y += 1
                     next_x = 0
 
                 if force_overwrite or self._cells[y][x] != char:
```

### Comparing `sh40_slate-0.2.0/slate/span.py` & `sh40_slate-0.3.0/slate/span.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
         for fld in fields(self):
             if not (fld.name in SETTERS and getattr(self, fld.name)):
                 continue
 
             sequences += SETTERS[fld.name] + ";"
 
-        if sequences == ";":
+        if sequences == "":
             return ""
 
         return f"\x1b[{sequences.strip(';')}m"
 
     @property
     def attrs(self) -> dict[str, bool | str]:
         """Returns a copy of the attributes that define this span."""
@@ -472,14 +472,16 @@
 
         length = len(self.text)
 
         x, y = origin
 
         if not _is_block(self.text):
             baseline_offset = SVG_RECT_BASELINE_OFFSET * font_size
+        else:
+            baseline_offset = 0
 
         x = round(x, 2)
         y = round(y, 2)
 
         svg = (
             "<rect"
             + f" x='{x}'"
@@ -495,14 +497,15 @@
                 f"{key}:{value}" for key, value in self.get_svg_styles().items()
             )
 
         svg += (
             "<text  dy='-0.25em'"
             + f" x='{x}'"
             + f" y='{y + font_size}'"
+            + f" fill='{foreground.hex}'"
             + (f" styles='{styles}'" if inline_styles else "")
             + (f" class='{cls}'" if cls is not None else "")
             + f">{_escape_html(self.text)}</text>"
         )
 
         return svg
```

### Comparing `sh40_slate-0.2.0/slate/terminal.py` & `sh40_slate-0.3.0/slate/terminal.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_color.py` & `sh40_slate-0.3.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_core.py` & `sh40_slate-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_event.py` & `sh40_slate-0.3.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_screen.py` & `sh40_slate-0.3.0/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_span.py` & `sh40_slate-0.3.0/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/tests/test_terminal.py` & `sh40_slate-0.3.0/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/.gitignore` & `sh40_slate-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/LICENSE` & `sh40_slate-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/pyproject.toml` & `sh40_slate-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.2.0/PKG-INFO` & `sh40_slate-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-slate
-Version: 0.2.0
+Version: 0.3.0
 Summary: A lightweight set of tools for interfacing with the terminal.
 Project-URL: Documentation, https://github.com/shade40/slate#readme
 Project-URL: Issues, https://github.com/shade40/slate/issues
 Project-URL: Source, https://github.com/shade40/slate
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

