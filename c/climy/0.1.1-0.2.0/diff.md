# Comparing `tmp/climy-0.1.1.tar.gz` & `tmp/climy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climy-0.1.1.tar", max compression
+gzip compressed data, was "climy-0.2.0.tar", max compression
```

## Comparing `climy-0.1.1.tar` & `climy-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.1.1/LICENSE
--rw-r--r--   0        0        0     1236 2023-06-29 12:11:02.677187 climy-0.1.1/README.md
--rw-r--r--   0        0        0      136 2023-06-29 11:45:06.580415 climy-0.1.1/climy/__init__.py
--rw-r--r--   0        0        0     1107 2023-06-29 11:45:06.584415 climy-0.1.1/climy/application.py
--rw-r--r--   0        0        0     5217 2023-06-30 12:47:51.074491 climy-0.1.1/climy/command.py
--rw-r--r--   0        0        0       25 2023-06-16 10:11:53.677630 climy-0.1.1/climy/manager.py
--rw-r--r--   0        0        0      922 2023-06-29 11:45:06.596415 climy-0.1.1/climy/option.py
--rw-r--r--   0        0        0      394 2023-06-30 12:49:10.576289 climy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 climy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3690 2023-07-07 10:22:12.926676 climy-0.2.0/README.md
+-rw-r--r--   0        0        0      154 2023-07-07 11:58:11.921355 climy-0.2.0/climy/__init__.py
+-rw-r--r--   0        0        0     1107 2023-06-29 11:45:06.584415 climy-0.2.0/climy/application.py
+-rw-r--r--   0        0        0     5484 2023-07-07 11:57:29.664408 climy-0.2.0/climy/command.py
+-rw-r--r--   0        0        0     5594 2023-07-07 11:13:50.001324 climy-0.2.0/climy/console.py
+-rw-r--r--   0        0        0       25 2023-06-16 10:11:53.677630 climy-0.2.0/climy/manager.py
+-rw-r--r--   0        0        0      922 2023-06-29 11:45:06.596415 climy-0.2.0/climy/option.py
+-rw-r--r--   0        0        0      394 2023-07-07 12:02:50.271392 climy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 climy-0.2.0/PKG-INFO
```

### Comparing `climy-0.1.1/LICENSE` & `climy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climy-0.1.1/climy/application.py` & `climy-0.2.0/climy/application.py`

 * *Files identical despite different names*

### Comparing `climy-0.1.1/climy/command.py` & `climy-0.2.0/climy/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from climy.option import Option
 
 
+class Handler:
+    def __init__(self, command: 'Command'):
+        self.command = command
+
+    def run(self):
+        ...
+
+
 class Command:
     def __init__(
             self,
             name: str,
             description: str,
             title: str = '',
-            handler: callable = None
+            handler=None
     ):
         self.commands: dict[str, Command] = {}
         self.options: dict[str, Option] = {}
         self.options_short: dict[str, str] = {}
         self.options_required: set[str] = set()
         self.name = name
         self.title = title
@@ -101,15 +109,19 @@
                     option.value = True
                 else:
                     option.value = pair.pop(1) if len(pair) > 1 else None
         if self.options_required:
             print(f'\033[1;35mSome options are required: [{", ".join(self.options_required)}]')
             return
         if self.handler:
-            self.handler(comm=self)
+            if issubclass(self.handler, Handler):
+                handler = self.handler(command=self)
+                handler.run()
+            else:
+                self.handler(comm=self)
 
     def generate_help(self, text: str = ''):
         text += "\033[1mUsage:\033[0m\r\n  {name} <command> [options] [arguments]".format(name=self.get_name())
         if self.options:
             text += self.generate_help_options_session()
         if self.commands:
             text += "\r\n\r\n\033[1mCommands:\033[0m\r\n  {opt}".format(opt=self.generate_help_commands_session())
```

### Comparing `climy-0.1.1/climy/option.py` & `climy-0.2.0/climy/option.py`

 * *Files identical despite different names*

