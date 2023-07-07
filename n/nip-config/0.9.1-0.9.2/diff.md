# Comparing `tmp/nip-config-0.9.1.tar.gz` & `tmp/nip-config-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nip-config-0.9.1.tar", last modified: Fri Apr 28 08:29:03 2023, max compression
+gzip compressed data, was "nip-config-0.9.2.tar", last modified: Fri Apr 28 09:52:48 2023, max compression
```

## Comparing `nip-config-0.9.1.tar` & `nip-config-0.9.2.tar`

### file list

```diff
@@ -1,29 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.155334 nip-config-0.9.1/
--rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      740 2023-04-28 08:29:03.155334 nip-config-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.141738 nip-config-0.9.1/nip/
--rw-rw-rw-   0        0        0      137 2023-04-28 07:36:18.000000 nip-config-0.9.1/nip/__init__.py
--rw-rw-rw-   0        0        0     5869 2023-04-28 07:37:49.000000 nip-config-0.9.1/nip/constructor.py
--rw-rw-rw-   0        0        0     3078 2023-04-28 08:21:33.000000 nip-config-0.9.1/nip/convertor.py
--rw-rw-rw-   0        0        0     1576 2023-04-28 08:28:10.000000 nip-config-0.9.1/nip/directives.py
--rw-rw-rw-   0        0        0      807 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/dumper.py
--rw-rw-rw-   0        0        0    19040 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/elements.py
--rw-rw-rw-   0        0        0     1632 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/iter_parser.py
--rw-rw-rw-   0        0        0     8749 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/main.py
--rw-rw-rw-   0        0        0     2453 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/non_seq_constructor.py
--rw-rw-rw-   0        0        0     1603 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/parser.py
--rw-rw-rw-   0        0        0     2478 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/stream.py
--rw-rw-rw-   0        0        0     6848 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/tokens.py
--rw-rw-rw-   0        0        0     1462 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.152953 nip-config-0.9.1/nip_config.egg-info/
--rw-rw-rw-   0        0        0      740 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      841 2023-04-28 08:29:03.157369 nip-config-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.153988 nip-config-0.9.1/tests/
--rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.9.1/tests/test_multi.py
--rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.9.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:52:48.170049 nip-config-0.9.2/
+-rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-04-28 09:52:48.171092 nip-config-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 09:52:48.143244 nip-config-0.9.2/nip/
+-rw-rw-rw-   0        0        0      137 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/__init__.py
+-rw-rw-rw-   0        0        0     5869 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/constructor.py
+-rw-rw-rw-   0        0        0     3079 2023-04-28 09:40:53.000000 nip-config-0.9.2/nip/convertor.py
+-rw-rw-rw-   0        0        0     1449 2023-04-28 08:47:20.000000 nip-config-0.9.2/nip/directives.py
+-rw-rw-rw-   0        0        0      807 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/dumper.py
+-rw-rw-rw-   0        0        0    18267 2023-04-28 09:31:58.000000 nip-config-0.9.2/nip/elements.py
+-rw-rw-rw-   0        0        0     1632 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/iter_parser.py
+-rw-rw-rw-   0        0        0     8749 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:52:48.154237 nip-config-0.9.2/nip/nip/
+-rw-rw-rw-   0        0        0      137 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/__init__.py
+-rw-rw-rw-   0        0        0     5869 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/constructor.py
+-rw-rw-rw-   0        0        0     3079 2023-04-28 09:40:53.000000 nip-config-0.9.2/nip/nip/convertor.py
+-rw-rw-rw-   0        0        0     1449 2023-04-28 08:47:20.000000 nip-config-0.9.2/nip/nip/directives.py
+-rw-rw-rw-   0        0        0      807 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/dumper.py
+-rw-rw-rw-   0        0        0    18267 2023-04-28 09:31:58.000000 nip-config-0.9.2/nip/nip/elements.py
+-rw-rw-rw-   0        0        0     1632 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/iter_parser.py
+-rw-rw-rw-   0        0        0     8749 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/main.py
+-rw-rw-rw-   0        0        0     2453 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/non_seq_constructor.py
+-rw-rw-rw-   0        0        0     1600 2023-04-28 09:06:04.000000 nip-config-0.9.2/nip/nip/parser.py
+-rw-rw-rw-   0        0        0     2478 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/stream.py
+-rw-rw-rw-   0        0        0     6848 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/tokens.py
+-rw-rw-rw-   0        0        0     1462 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/nip/utils.py
+-rw-rw-rw-   0        0        0     2453 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/non_seq_constructor.py
+-rw-rw-rw-   0        0        0     1600 2023-04-28 09:06:04.000000 nip-config-0.9.2/nip/parser.py
+-rw-rw-rw-   0        0        0     2478 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/stream.py
+-rw-rw-rw-   0        0        0       19 2023-04-28 09:06:50.000000 nip-config-0.9.2/nip/test.py
+-rw-rw-rw-   0        0        0     6848 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/tokens.py
+-rw-rw-rw-   0        0        0     1462 2023-04-28 08:29:58.000000 nip-config-0.9.2/nip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:52:48.167731 nip-config-0.9.2/nip_config.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-04-28 09:52:48.000000 nip-config-0.9.2/nip_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-04-28 09:52:48.000000 nip-config-0.9.2/nip_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:52:48.000000 nip-config-0.9.2/nip_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 09:52:48.000000 nip-config-0.9.2/nip_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 09:52:48.000000 nip-config-0.9.2/nip_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2023-04-28 09:52:48.177123 nip-config-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:52:48.170049 nip-config-0.9.2/tests/
+-rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.9.2/tests/test_multi.py
+-rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.9.2/tests/test_utils.py
```

### Comparing `nip-config-0.9.1/LICENSE` & `nip-config-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/PKG-INFO` & `nip-config-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.9.1
+Version: 0.9.2
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nip-config-0.9.1/README.md` & `nip-config-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/constructor.py` & `nip-config-0.9.2/nip/constructor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/convertor.py` & `nip-config-0.9.2/nip/convertor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Dict, Optional, Callable, Union
 
-from nip.elements import Element, Args, Tag, Value
-from nip.constructor import global_builders
+from .constructor import global_builders
 
 global_convertors = {}
 
 
 class Convertor:
     def __init__(self, load_globals: bool = True):
         self.convertors = {}
         if load_globals:
             self._load_globals()
 
-    def convert(self, obj: object) -> Element:
+    def convert(self, obj: object):
         class_name = type(obj).__name__
         if class_name in self.convertors:
             tag, convertor = self.convertors[class_name]
             return Tag(tag, self.convert(convertor(obj)))
 
         if hasattr(obj, "__nip__"):
             return Tag(class_name, self.convert(obj.__nip__()))
@@ -82,7 +81,10 @@
     def _(item: type):
         if not isinstance(item, type):
             raise ValueError("Expected class type to be wrapped.")
         global_convertors[class_name] = (tag, item)
         return item
 
     return _
+
+
+from .elements import Args, Tag, Value  # fixes cycle imports
```

### Comparing `nip-config-0.9.1/nip/dumper.py` & `nip-config-0.9.2/nip/dumper.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/elements.py` & `nip-config-0.9.2/nip/elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Contains all the elements of nip config files"""
 # from __future__ import annotations
 
 import logging
 
-import nip.constructor  # This import pattern because of cycle imports
-import nip.directives
-import nip.dumper
-import nip.non_seq_constructor as nsc
-import nip.parser
-import nip.stream
-import nip.tokens as tokens
-import nip.utils
+from .stream import Stream
+from .constructor import Constructor, ConstructorError, check_typing
+from .convertor import Convertor
+from .directives import call_directive
+from .dumper import Dumper, DumpError
+from .non_seq_constructor import preload_vars
+from .parser import Parser, ParserError
+from . import tokens
+from .utils import flatten, iterate_items
+
 
 from abc import abstractmethod, ABC
 from typing import Any, Union, Tuple, Dict
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -22,90 +24,90 @@
     """Base token for nip file"""
     def __init__(self, name: str = '', value: Any = None):
         self.name = name
         self.value = value
 
     @classmethod
     @abstractmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Element", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Element", None]:
         pass
 
     def __str__(self):
         return f"{self.__class__.__name__}('{self.name}', {self.value})"
 
     def __getitem__(self, item):
         return self.value[item]
 
     def __setitem__(self, key, value):
         self.value[key] = value
 
     def to_python(self):
         return self.value.to_python()
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         return self.value.construct(constructor)
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return self.value.dump(dumper)
 
     def __eq__(self, other):
         return self.name == other.name and self.value == other.value
 
     def flatten(self, delimiter='.') -> Dict:
-        return nip.utils.flatten(self.to_python(), delimiter)
+        return flatten(self.to_python(), delimiter)
 
 
 class Document(Element):  # ToDo: add multi document support
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> "Document":
+    def read(cls, stream: Stream, parser: "Parser") -> "Document":
         doc_name = cls._read_name(stream)
         content = RightValue.read(stream, parser)
         return Document(doc_name, content)
 
     @classmethod
-    def _read_name(cls, stream: "nip.stream.Stream"):
+    def _read_name(cls, stream: Stream):
         read_tokens = stream.peek(tokens.Operator('---'), tokens.Name) or \
                       stream.peek(tokens.Operator('---'))
         if read_tokens is not None:
             stream.step()
             if len(read_tokens) == 2:
                 return read_tokens[1].value
         return ''
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         string = "---"
         if self.name:
             string += " " + self.name + " "
         return string + self.value.dump(dumper)
 
 
 class RightValue(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Element:
+    def read(cls, stream: Stream, parser: "Parser") -> Element:
         value = Directive.read(stream, parser) or \
                 LinkCreation.read(stream, parser) or \
                 Link.read(stream, parser) or \
                 Class.read(stream, parser) or \
                 Tag.read(stream, parser) or \
                 Iter.read(stream, parser) or \
                 Args.read(stream, parser) or \
                 FString.read(stream, parser) or \
                 Nothing.read(stream, parser) or \
                 InlinePython.read(stream, parser) or \
                 Value.read(stream, parser)
 
         if value is None:
-            raise nip.parser.ParserError(stream, "Wrong right value")
+            raise ParserError(stream, "Wrong right value")
 
         return value
 
 
 class Value(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[None, "Value"]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union[None, "Value"]:
         tokens_list = [
             tokens.Number,
             tokens.Bool,
             tokens.String,
             tokens.List,
             tokens.TupleToken,
             tokens.Dict
@@ -117,212 +119,212 @@
                 return Value(read_tokens[0].name, read_tokens[0].value)
 
         return None
 
     def to_python(self):
         return self.value
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         return self.value
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         if isinstance(self.value, str):
             return f'"{self.value}"'
         return str(self.value)
 
     def __len__(self):
         return len(self.value)
 
 
 class LinkCreation(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[Element, None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union[Element, None]:
         read_tokens = stream.peek(tokens.Operator('&'), tokens.Name)
         if read_tokens is None:
             # if stream.peek(tokens.Operator('&')):  # mb: do it more certainly: peak operator
-            #     raise "nip.parser.Parser"Error(      # mb: firstly and then choose class to read)
+            #     raise "Parser"Error(      # mb: firstly and then choose class to read)
             #         stream, "Found variable creation operator '&' but name is not specified")
             return None
 
         name = read_tokens[1].value
         stream.step()
 
         value = RightValue.read(stream, parser)
         if name in parser.link_names:
-            raise nip.parser.ParserError(stream, f"Redefining of link '{name}'")
+            raise ParserError(stream, f"Redefining of link '{name}'")
         parser.link_names.append(name)
 
         return LinkCreation(name, value)
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         constructor.vars[self.name] = self.value.construct(constructor)
         return constructor.vars[self.name]
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"&{self.name} {self.value.dump(dumper)}"
 
 
 class Link(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[Element, None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union[Element, None]:
         read_tokens = stream.peek(tokens.Operator('*'), tokens.Name)
         if read_tokens is None:
             return None
 
         name = read_tokens[1].value
         stream.step()
 
         if name in parser.link_replacements:
             return parser.link_replacements[name]
 
         if parser.sequential_links and name not in parser.link_names:
-            nip.parser.ParserError(stream, "Link usage before assignment")
+            ParserError(stream, "Link usage before assignment")
 
         return Link(name)
 
     def to_python(self):
         return "nil"  # something that means that object is not constructed yet.
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         return constructor.vars[self.name]
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"*{self.name}"
 
 
 class Tag(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Tag", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Tag", None]:
         read_tokens = stream.peek(tokens.Operator('!'), tokens.Name)
         if read_tokens is None:
             return None
         name = read_tokens[1].value
         stream.step()
 
         value = RightValue.read(stream, parser)
 
         return Tag(name, value)
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         if isinstance(self.value, Args):
             args, kwargs = self.value.construct(constructor, always_pair=True)
         else:
             value = self.value.construct(constructor)
             if isinstance(value,  Nothing):  # mb: Add IS_NOTHING method
                 return constructor.builders[self.name]()
             else:
                 args, kwargs = [value], {}
 
         if self.name not in constructor.builders:
-            raise nip.constructor.ConstructorError(
+            raise ConstructorError(
                 self, args, kwargs, f"Constructor for Tag '{self.name}' is not registered.")
 
-        messages = nip.constructor.check_typing(constructor.builders[self.name], args, kwargs)
+        messages = check_typing(constructor.builders[self.name], args, kwargs)
         if len(messages) > 0:
             if constructor.strict_typing:
-                raise nip.constructor.ConstructorError(self, args, kwargs, "\n".join(messages))
+                raise ConstructorError(self, args, kwargs, "\n".join(messages))
             else:
                 _LOGGER.warning(f"Typing mismatch while constructing {self.name}:\n" +
                                 "\n".join(messages))
 
         try:  # Try to construct
             return constructor.builders[self.name](*args, **kwargs)
         except Exception as e:
-            raise nip.constructor.ConstructorError(self, args, kwargs, e)
+            raise ConstructorError(self, args, kwargs, e)
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"!{self.name} " + self.value.dump(dumper)
 
 
 class Class(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Class", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Class", None]:
         read_tokens = stream.peek(tokens.Operator('!&'), tokens.Name)
         if read_tokens is None:
             return None
         name = read_tokens[1].value
         stream.step()
 
         value = RightValue.read(stream, parser)
         if not isinstance(value, Nothing):
-            raise nip.parser.ParserError(stream, "Class should be created with nothing to the right.")
+            raise ParserError(stream, "Class should be created with nothing to the right.")
 
         return Class(name, value)
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         value = self.value.construct(constructor)
         assert isinstance(value, Nothing), "Unexpected right value while constructing Class"
 
         return constructor.builders[self.name]
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"!&{self.name} " + self.value.dump(dumper)
 
 
 class Args(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Args", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Args", None]:
         start_indent = stream.pos
         if start_indent <= parser.last_indent:
             return None
 
         args = []
         kwargs = {}  # mb: just dict with integer and string keys
         read_kwarg = False
         while stream and stream.pos == start_indent:
             parser.last_indent = start_indent
 
             item = cls._read_list_item(stream, parser)
             if item is not None:
                 if parser.strict and read_kwarg:
-                    raise nip.parser.ParserError(stream,
+                    raise ParserError(stream,
                                                  "Positional argument after keyword argument "
                                                  "is forbiddent in `strict` mode.")
                 args.append(item)
                 continue
 
             key, value = cls._read_dict_pair(stream, parser, kwargs.keys())
             if key is not None:
                 read_kwarg = True
                 kwargs[key] = value
                 continue
 
             break
 
         if stream.pos > start_indent:
-            raise nip.parser.ParserError(stream, "Unexpected indent")
+            raise ParserError(stream, "Unexpected indent")
 
         if not args and not kwargs:
             return None
         return Args("args", (args, kwargs))
 
     @classmethod
-    def _read_list_item(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") \
+    def _read_list_item(cls, stream: Stream, parser: "Parser") \
             -> Union[Element, None]:
         read_tokens = stream.peek(tokens.Operator('- '))
         if read_tokens is None:
             return None
         stream.step()
 
         value = RightValue.read(stream, parser)
 
         return value
 
     @classmethod
-    def _read_dict_pair(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser", kwargs_keys) \
+    def _read_dict_pair(cls, stream: Stream, parser: "Parser", kwargs_keys) \
             -> Union[Tuple[str, Element], Tuple[None, None]]:
         # mb: read String instead of Name for keys with spaces,
         # mb: but this leads to the case that
         read_tokens = stream.peek(tokens.Name, tokens.Operator(': '))
         if read_tokens is None:
             return None, None
 
         key = read_tokens[0].value
         if parser.strict and key in kwargs_keys:
-            raise nip.parser.ParserError(stream,
+            raise ParserError(stream,
                                          f"Dict key overwriting is forbidden in `strict` "
                                          f"mode. Overwritten key: '{key}'.")
         stream.step()
 
         value = RightValue.read(stream, parser)
 
         return key, value
@@ -340,21 +342,23 @@
     def __getitem__(self, item):
         try:
             return self.value[0][item]
         except TypeError:
             return self.value[1][item]
 
     def __setitem__(self, key, value):
+        convertor = Convertor()
         if isinstance(key, int):
-            self.value[0][key] = nip.convert(value)
+            self.value[0][key] = convertor.convert(value)
         else:
-            self.value[1][key] = nip.convert(value)
+            self.value[1][key] = convertor.convert(value)
 
     def append(self, value):
-        self.value[0].append(nip.convert(value))
+        convertor = Convertor()
+        self.value[0].append(convertor.convert(value))
 
     def __len__(self):
         return len(self.value[0]) + len(self.value[1])
 
     def __iter__(self):
         for item in self.value[0]:
             yield item
@@ -363,28 +367,28 @@
 
     def to_python(self):
         args = list(item.to_python() for item in self.value[0])
         kwargs = {key: value.to_python() for key, value in self.value[1].items()}
         assert args or kwargs, "Error converting Args node to python"  # This should never happen
         if args and kwargs:
             result = {}
-            result.update(nip.utils.iterate_items(args))
-            result.update(nip.utils.iterate_items(kwargs))
+            result.update(iterate_items(args))
+            result.update(iterate_items(kwargs))
             return result
         return args or kwargs
 
-    def construct(self, constructor: "nip.constructor.Constructor", always_pair=False):
+    def construct(self, constructor: Constructor, always_pair=False):
         args = list(item.construct(constructor) for item in self.value[0])
         kwargs = {key: value.construct(constructor) for key, value in self.value[1].items()}
         assert args or kwargs, "Error converting Args node to python"  # This should never happen
         if args and kwargs or always_pair:
             return args, kwargs
         return args or kwargs
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         dumped_args = '\n'.join([
             " "*dumper.indent + f"- {item.dump(dumper + dumper.default_shift)}"
             for item in self.value[0]
         ])
         string = ('\n' if dumped_args else '') + dumped_args
 
         dumped_kwargs = '\n'.join([
@@ -399,27 +403,27 @@
 class Iter(Element):
     def __init__(self, name: str = '', value: Any = None):
         super(Iter, self).__init__(name, value)
         self.return_index = -1
         # mb: name all the iterators and get the value from constructor rather then use this index
 
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Iter", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Iter", None]:
         read_tokens = stream.peek(tokens.Operator('@'), tokens.Name) or \
                       stream.peek(tokens.Operator('@'))
         if read_tokens is None:
             return None
         stream.step()
         value = RightValue.read(stream, parser)
         if isinstance(value, Value) and isinstance(value.value, list):
             value = value.value
         elif isinstance(value, Args) and len(value.value[1]) == 0:
             value = value
         else:
-            raise nip.parser.ParserError(stream, "List is expected as a value for Iterable node")
+            raise ParserError(stream, "List is expected as a value for Iterable node")
         if len(read_tokens) == 1:
             iterator = Iter('', value)
         else:
             iterator = Iter(read_tokens[1].value, value)
 
         parser.iterators.append(iterator)
         return iterator
@@ -427,114 +431,114 @@
     def to_python(self):
         if self.return_index == -1:
             raise iter(self.value)
         if isinstance(self.value[self.return_index], Element):
             return self.value[self.return_index].to_python()
         return self.value[self.return_index]
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         if self.return_index == -1:
             raise Exception("Iterator index was not specified by IterParser")
         if isinstance(self.value, list):
             return self.value[self.return_index]
         elif isinstance(self.value, Args):
             return self.value[self.return_index].construct(constructor)
         else:
-            raise nip.constructor.ConstructorError(self, (), {}, "Unexpected iter value type")
+            raise ConstructorError(self, (), {}, "Unexpected iter value type")
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         if self.return_index == -1:
-            raise nip.dumper.DumpError(
+            raise DumpError(
                 "Dumping an iterator but index was not specified by IterParser"
             )
         if isinstance(self.value, list):
             return str(self.value[self.return_index])
         elif isinstance(self.value, Args):
             return self.value[self.return_index].dump(dumper)
         else:
-            raise nip.dumper.DumpError("Unable to dump Iterable node: unexpected value type")
+            raise DumpError("Unable to dump Iterable node: unexpected value type")
 
 
 class InlinePython(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+    def read(cls, stream: Stream, parser: "Parser") -> \
             Union["InlinePython", None]:
         read_tokens = stream.peek(tokens.InlinePython)
         if read_tokens is None:
             return None
         stream.step()
         exec_string = read_tokens[0].value
         return InlinePython(value=exec_string)
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
-        nsc.preload_vars(self.value, constructor)
+    def construct(self, constructor: Constructor):
+        preload_vars(self.value, constructor)
         locals().update(constructor.vars)
         return eval(self.value)
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"`{self.value}`"
 
     def to_python(self):
         return f"`{self.value}`"
 
 
 class Nothing(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Nothing", None]:
+    def read(cls, stream: Stream, parser: "Parser") -> Union["Nothing", None]:
         if not stream:
             return Nothing()
 
         indent = stream.pos
         if stream.pos == 0 or (
                 stream.lines[stream.n][:stream.pos].isspace()
                 and indent <= parser.last_indent):
             return Nothing()
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
+    def construct(self, constructor: Constructor):
         return self
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return ""
 
     def to_python(self):
         return None
 
 
 class FString(Element):  # Includes f-string and r-string
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+    def read(cls, stream: Stream, parser: "Parser") -> \
             Union["FString", None]:
         read_tokens = stream.peek(tokens.PythonString)
         if read_tokens is None:
             return None
         stream.step()
         string, t = read_tokens[0].value
         if t == 'r':
             print("Warning: all strings in NIP are already python r-string. "
                   "You don't have to explicitly specify it.")
         return FString(value=string)
 
-    def construct(self, constructor: "nip.constructor.Constructor"):
-        nsc.preload_vars(f"f{self.value}", constructor)
+    def construct(self, constructor: Constructor):
+        preload_vars(f"f{self.value}", constructor)
         locals().update(constructor.vars)
         return eval(f"f{self.value}")
 
-    def dump(self, dumper: nip.dumper.Dumper):
+    def dump(self, dumper: Dumper):
         return f"f{self.value}"
 
     def to_python(self):
         return f"f{self.value}"
 
 
 class Directive(Element):
     @classmethod
-    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+    def read(cls, stream: Stream, parser: "Parser") -> \
             Union["FString", None]:
         read_tokens = stream.peek(tokens.Operator('!!'), tokens.Name)
         if read_tokens is None:
             return None
         name = read_tokens[1].value
         stream.step()
 
         value = RightValue.read(stream, parser)
 
-        return nip.directives.call_directive(name, value, stream)
+        return call_directive(name, value, stream)
```

### Comparing `nip-config-0.9.1/nip/iter_parser.py` & `nip-config-0.9.2/nip/iter_parser.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/main.py` & `nip-config-0.9.2/nip/main.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/non_seq_constructor.py` & `nip-config-0.9.2/nip/nip/non_seq_constructor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/parser.py` & `nip-config-0.9.2/nip/nip/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import nip.elements as elements
-
 from pathlib import Path
 from typing import Union
 
 from .stream import Stream
 
 
 class Parser:  # mb: we don't need Parser itself. its just storage for links and tags. Hm...
@@ -25,16 +23,17 @@
 
         return self.parse_string(string_representation)
 
     def __call__(self, path: Union[str, Path]):
         return self.parse(path)
 
     def parse_string(self, string):
+        from .elements import Document
         stream = Stream(string)  # mb: add stream to parser and log errors more convenient
-        tree = elements.Document.read(stream, self)
+        tree = Document.read(stream, self)
         if stream:
             raise ParserError(stream, "Wrong statement.")
         return tree
 
     def has_iterators(self) -> bool:
         return len(self.iterators) > 0
```

### Comparing `nip-config-0.9.1/nip/stream.py` & `nip-config-0.9.2/nip/nip/stream.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/tokens.py` & `nip-config-0.9.2/nip/nip/tokens.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip/utils.py` & `nip-config-0.9.2/nip/nip/utils.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.1/nip_config.egg-info/PKG-INFO` & `nip-config-0.9.2/nip_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.9.1
+Version: 0.9.2
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nip-config-0.9.1/setup.cfg` & `nip-config-0.9.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6970 2d63 6f6e 6669 670d 0a76   = nip-config..v
-00000020: 6572 7369 6f6e 203d 2030 2e39 2e31 0d0a  ersion = 0.9.1..
+00000020: 6572 7369 6f6e 203d 2030 2e39 2e32 0d0a  ersion = 0.9.2..
 00000030: 6175 7468 6f72 203d 2049 6c79 6120 5661  author = Ilya Va
 00000040: 7369 6c69 6576 0d0a 6175 7468 6f72 5f65  siliev..author_e
 00000050: 6d61 696c 203d 2073 7061 6972 6574 4062  mail = spairet@b
 00000060: 6b2e 7275 0d0a 6465 7363 7269 7074 696f  k.ru..descriptio
 00000070: 6e20 3d20 4164 7661 6e63 6564 2063 6f6e  n = Advanced con
 00000080: 6669 6773 2066 6f72 2070 7974 686f 6e0d  figs for python.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
```

### Comparing `nip-config-0.9.1/tests/test_utils.py` & `nip-config-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

