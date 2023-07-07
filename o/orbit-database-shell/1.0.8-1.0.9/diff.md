# Comparing `tmp/orbit_database_shell-1.0.8.tar.gz` & `tmp/orbit_database_shell-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database_shell-1.0.8.tar", max compression
+gzip compressed data, was "orbit_database_shell-1.0.9.tar", max compression
```

## Comparing `orbit_database_shell-1.0.8.tar` & `orbit_database_shell-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/LICENSE.md
--rw-r--r--   0        0        0     2272 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/README.md
--rwxr-xr-x   0        0        0        0 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/orbit_database_shell/__init__.py
--rwxr-xr-x   0        0        0     1887 2023-06-29 22:19:46.643208 orbit_database_shell-1.0.8/orbit_database_shell/__main__.py
--rwxr-xr-x   0        0        0    24788 2023-06-28 13:28:56.984810 orbit_database_shell-1.0.8/orbit_database_shell/odb_actions.py
--rwxr-xr-x   0        0        0     4169 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/orbit_database_shell/odb_completers.py
--rw-r--r--   0        0        0     1988 2023-06-23 14:54:20.350769 orbit_database_shell-1.0.8/orbit_database_shell/odb_decorators.py
--rwxr-xr-x   0        0        0     7071 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.8/orbit_database_shell/odb_grammar.py
--rwxr-xr-x   0        0        0    46376 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.8/orbit_database_shell/odb_help.py
--rw-r--r--   0        0        0     1313 2023-06-29 22:19:46.643208 orbit_database_shell-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 orbit_database_shell-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0     2272 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.9/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.9/orbit_database_shell/__init__.py
+-rwxr-xr-x   0        0        0     1940 2023-07-07 15:18:06.802519 orbit_database_shell-1.0.9/orbit_database_shell/__main__.py
+-rwxr-xr-x   0        0        0    24579 2023-07-03 15:10:05.194599 orbit_database_shell-1.0.9/orbit_database_shell/odb_actions.py
+-rwxr-xr-x   0        0        0     4169 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.9/orbit_database_shell/odb_completers.py
+-rw-r--r--   0        0        0     1988 2023-06-23 14:54:20.350769 orbit_database_shell-1.0.9/orbit_database_shell/odb_decorators.py
+-rwxr-xr-x   0        0        0     7087 2023-07-03 12:04:57.383324 orbit_database_shell-1.0.9/orbit_database_shell/odb_grammar.py
+-rwxr-xr-x   0        0        0    46376 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.9/orbit_database_shell/odb_help.py
+-rw-r--r--   0        0        0     1310 2023-07-07 15:18:06.802519 orbit_database_shell-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3686 1970-01-01 00:00:00.000000 orbit_database_shell-1.0.9/PKG-INFO
```

### Comparing `orbit_database_shell-1.0.8/LICENSE.md` & `orbit_database_shell-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.8/README.md` & `orbit_database_shell-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/__main__.py` & `orbit_database_shell-1.0.9/orbit_database_shell/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from orbit_database_shell.odb_decorators import banner
 
 __author__ = 'Gareth Bult'
 __banner__ = 'Orbit-DB'
 __copyright__ = 'Copyright 2023, Mad Penguin Consulting Ltd'
 __credits__ = ['Gareth Bult']
 __license__ = 'MIT'
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __maintainer__ = 'Gareth Bult'
 __email__ = 'gareth@madpenguin.uk'
 __status__ = 'Development'
 
 
 def main ():
-    actions = Actions().notice(banner)
+    actions = Actions().notice(banner + f'\n<magenta>     Version {__version__}</magenta>')
     print()
     folder = Path('~/.orbit').expanduser()
     folder.mkdir(exist_ok=True, parents=True)
     session = PromptSession(
         history=FileHistory(PosixPath(folder / 'shell_history')),
         complete_style=CompleteStyle.READLINE_LIKE,
         auto_suggest=AutoSuggestFromHistory(),
```

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/odb_actions.py` & `orbit_database_shell-1.0.9/orbit_database_shell/odb_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._limit = 10
         self._mode = False
         self._mysql = None
         Path.mkdir(self._home, exist_ok=True)
 
     def get_table(self, name):
         if name in list(self._db.tables(True)):
-            return self._db.table(name)
+            return self._db.table(name, auditing=True)
         else:
             self.error(f'no such table "{name}"')
             return None
 
     def complete(self, action, variables):
         if hasattr(self, f'do_{action}'):
             getattr(self, f'do_{action}')(variables)
@@ -78,15 +78,15 @@
 
     @property
     def tables(self):
         return [name for name in self._db.tables(self._mode)] if self._db else []
 
     def indexes(self, variables):
         table_name = variables.get('table')
-        return [name for name in self._db.table(table_name).indexes()] if self._db and table_name in self._db.tables(self._mode) else []
+        return [name for name in self.get_table(table_name).indexes()] if self._db and table_name in self.get_db.tables(self._mode) else []
 
     def fields(self, variables):
         return self._fields(variables.get('table'), variables.getall('fields'))
 
     def all_fields(self, table_name):
         return self._fields(table_name, [])
 
@@ -150,15 +150,15 @@
         else:
             table_names = [table_name]      
 
         start = datetime.now()
         for name in table_names:
             cursor.execute(f"select * from {name}")
             rows = cursor.fetchall()
-            table = self._db.table(name.replace('_', '-'))
+            table = self.get_table(name.replace('_', '-'))
             with WriteTransaction(self._db) as txn:
                 for row in tqdm(rows, colour="green"):
                     doc = Doc()
                     for i in range(len(row)):
                         if row[i]:
                             t = cursor.description[i][1]
                             if t == 6:
@@ -192,15 +192,15 @@
             print(f'Invalid: {cmd}')
         return
     
     @selected
     def do_load (self, vars):
         name = vars.get('table')
         path = vars.get('path')
-        table = self._db.table(name)
+        table = self.get_table(name)
         if table.records():
             return self.warning(f' <b>{name}</b> already has records!')
         if not Path(path).exists():
             return (f' <b>{path}</b> not found!')
         table.import_from_file(path)
 
     @selected
@@ -359,19 +359,15 @@
         """Display a list of indexes for the specified table\n"""
         table_name = vars.get('table')
         table = self.get_table(table_name)
         
         tab = self.richTable(['Table name', 'Index name', 'Entries', 'Dups', 'Key'])
         with ReadTransaction(self._db) as transaction:
             for index in table.indexes(txn=transaction.txn):
-                d = self._db.meta.fetch_index(table_name, index, transaction.txn)
-                conf = d['conf']
-                if not d or 'conf' not in d:
-                    self.error(f' Unable to locate metadata for {table_name}!')
-                    continue
+                conf = table[index]._conf
                 if conf.get('iwx'):
                     key = 'Full Text Index'
                 else:
                     key = conf.get('func', 'None')
                     if not key:
                         key = 'None'
                 text, key = key[:60], key[60:]
```

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/odb_completers.py` & `orbit_database_shell-1.0.9/orbit_database_shell/odb_completers.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/odb_decorators.py` & `orbit_database_shell-1.0.9/orbit_database_shell/odb_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/odb_grammar.py` & `orbit_database_shell-1.0.9/orbit_database_shell/odb_grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from prompt_toolkit.contrib.regular_languages.lexer import GrammarLexer
 from prompt_toolkit.lexers import SimpleLexer
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.styles import Style
 from orbit_database_shell.odb_completers import DatabaseCompleter, PathCompleter, TableCompleter, FieldCompleter, IndexCompleter, MyGrammarCompleter
 from orbit_database_shell.odb_completers import MySQLDBCompleter, MySQLTableCompleter
 
-commands = ['show', 'select', 'use', 'register', 'explain', 'clear', 'unique', 'analyse', 'dump', 'lexicon', 'match', 'help', 'delete', 'import', 'drop', 'fix', 'mode', 'create']
+commands = ['show', 'select', 'use', 'register', 'explain', 'clear', 'unique', 'analyse', 'dump', 'lexicon', 'match', 'help', 'delete', 'import', 'drop', 'fix', 'mode', 'create', 'load', 'save']
 show_commands = ['databases', 'tables', 'indexes']
 drop_commands = ['table', 'index']
 mode_commands = ['user', 'advanced']
 select_options = ['limit', 'index', 'where']
 index_options = ['doc']
 unique_options = ['index']
```

### Comparing `orbit_database_shell-1.0.8/orbit_database_shell/odb_help.py` & `orbit_database_shell-1.0.9/orbit_database_shell/odb_help.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.8/pyproject.toml` & `orbit_database_shell-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-database-shell"
-version = "1.0.8"
+version = "1.0.9"
 description = "Orbit-DB Shell"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -26,15 +26,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 prompt-toolkit = "*"
 Pygments = "^2.12.0"
 ujson = "^5.4.0"
 termcolor = "^1.1.0"
 python-snappy = "^0.6.1"
-loguru = ">=0.6.0"
+loguru = "^0.7"
 rich = "^13.3.4"
 mysql-connector-python = "^8.0.33"
 tqdm = "^4.65.0"
 orbit-database = ">=1.0.0"
 
 [tool.poetry.scripts]
 orbit_database_shell = 'orbit_database_shell.__main__:main'
```

### Comparing `orbit_database_shell-1.0.8/PKG-INFO` & `orbit_database_shell-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-database-shell
-Version: 1.0.8
+Version: 1.0.9
 Summary: Orbit-DB Shell
 Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: File Formats :: JSON
 Requires-Dist: Pygments (>=2.12.0,<3.0.0)
-Requires-Dist: loguru (>=0.6.0)
+Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
 Requires-Dist: orbit-database (>=1.0.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: orbit-database-shell Version: 1.0.8 Summary: Orbit-
+Metadata-Version: 2.1 Name: orbit-database-shell Version: 1.0.9 Summary: Orbit-
 DB Shell Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell Author: Gareth Bult Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console :: Curses Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: File Formats :: JSON Requires-Dist: Pygments
-(>=2.12.0,<3.0.0) Requires-Dist: loguru (>=0.6.0) Requires-Dist: mysql-
+(>=2.12.0,<3.0.0) Requires-Dist: loguru (>=0.7,<0.8) Requires-Dist: mysql-
 connector-python (>=8.0.33,<9.0.0) Requires-Dist: orbit-database (>=1.0.0)
 Requires-Dist: prompt-toolkit Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0) Requires-Dist: termcolor
 (>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: ujson
 (>=5.4.0,<6.0.0) Project-URL: Bug Tracker, https://gitlab.com/madpenguin/orbit-
 database-shell/-/issues Project-URL: Documentation, https://gitlab.com/
 madpenguin/orbit-database-shell Project-URL: Repository, https://gitlab.com/
```

