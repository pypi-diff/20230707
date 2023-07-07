# Comparing `tmp/tuidbtv-0.1.6.tar.gz` & `tmp/tuidbtv-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.6.tar", max compression
+gzip compressed data, was "tuidbtv-0.1.7.tar", max compression
```

## Comparing `tuidbtv-0.1.6.tar` & `tuidbtv-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.6/LICENSE
--rw-r--r--   0        0        0      917 2023-07-03 17:12:50.724469 tuidbtv-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.6/tuidbtv/__init__.py
--rw-r--r--   0        0        0     3236 2023-07-03 17:12:50.729461 tuidbtv-0.1.6/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.6/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.6/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.6/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.6/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.6/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.6/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3117 2023-07-03 17:12:50.738495 tuidbtv-0.1.6/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.6/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.6/tuidbtv/default.css
--rw-r--r--   0        0        0      102 2023-07-03 17:12:50.745498 tuidbtv-0.1.6/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.6/tuidbtv/suggesters/__init__.py
--rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.6/tuidbtv/suggesters/SuggesterDict.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.6/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.6/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.6/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.6/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.6/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.6/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5706 2023-07-03 17:12:50.756478 tuidbtv-0.1.6/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1860 2023-07-03 17:12:50.754491 tuidbtv-0.1.6/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.7/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-07 20:07:56.685489 tuidbtv-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.7/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-07 20:07:13.436703 tuidbtv-0.1.7/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.7/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.7/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.7/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.7/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.7/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.7/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3303 2023-07-03 18:28:32.471479 tuidbtv-0.1.7/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.7/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.7/tuidbtv/default.css
+-rw-r--r--   0        0        0      276 2023-07-07 20:07:13.437708 tuidbtv-0.1.7/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.7/tuidbtv/suggesters/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.7/tuidbtv/suggesters/SuggesterDict.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.7/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.7/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.7/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.7/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.7/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.7/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     5706 2023-07-03 17:12:50.756478 tuidbtv-0.1.7/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.7/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.7/PKG-INFO
```

### Comparing `tuidbtv-0.1.6/LICENSE` & `tuidbtv-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/pyproject.toml` & `tuidbtv-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.6"
+version = "0.1.7"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.6/README.md` & `tuidbtv-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.1.7/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.1.7/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.1.7/tuidbtv/controllers/MySQLController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.1.7/tuidbtv/controllers/PostgresController.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,18 +33,26 @@
             data.insert(0, header_data)
             return data
         except Exception as e:
             self.connection.rollback()
             raise e
 
     def getSchemaNames(self):
-        return self.executeQuery("SELECT distinct table_schema FROM information_schema.tables")
+        data = sorted(self.executeQuery("SELECT distinct table_schema FROM information_schema.tables"))
+        try:
+            return sorted(data)
+        except:
+            return data
 
     def getTableNamesBySchema(self, schemaName):
-        return self.executeQuery(f"SELECT table_name FROM information_schema.tables WHERE table_schema='{schemaName}'")
+        data = self.executeQuery(f"SELECT table_name FROM information_schema.tables WHERE table_schema='{schemaName}'")
+        try:
+            return sorted(data)
+        except:
+            return data
 
     def getTablePreview(self, schemaName, tableName):
         data = self.executeQuery(f"SELECT * FROM {schemaName}.{tableName} limit 100")
         cutted_data = []
         for row in data:
             cutted_data.append(
                 tuple(
```

### Comparing `tuidbtv-0.1.6/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.1.7/tuidbtv/controllers/SQLLiteController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/default.css` & `tuidbtv-0.1.7/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/suggesters/SuggesterDict.py` & `tuidbtv-0.1.7/tuidbtv/suggesters/SuggesterDict.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.1.7/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.1.7/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.1.7/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.1.7/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.1.7/tuidbtv/widgets/SelectConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.6/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.1.7/tuidbtv/widgets/SQLEditor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from textual import on
 from textual.app import ComposeResult
 from textual.widget import Widget
 from textual.widgets import Input, Button, DataTable
 
+from tuidbtv.enums_and_variables import SQL_ABC
 from tuidbtv.suggesters.SuggesterDict import SuggesterDict
 from tuidbtv.widgets.PopUpScreen import PopUpScreen
 
-sql_abc = ["select", "from", "where", "join", "right join", "left join", "inner join",
-           "like", "insert", "into", "update", "order", "group", "by", "as", "on"]
-
 
 class SQLEditor(Widget):
+
+    def __init__(self, additional_suggestions: list[str] = []):
+        super().__init__()
+        self.suggestions = additional_suggestions
+
     def compose(self) -> ComposeResult:
-        yield Input(suggester=SuggesterDict([] + sql_abc, case_sensitive=False), id="new_request_input")
+        yield Input(suggester=SuggesterDict(self.suggestions + SQL_ABC, case_sensitive=False), id="new_request_input")
         yield Button("Run", id="execute_editor_button")
         yield DataTable(id="editor_table")
 
     @on(Button.Pressed)
     def execute_editor_query(self, event: Button.Pressed):
         if event.button.id == "execute_editor_button":
             query_text = self.query_one("#new_request_input", expect_type=Input).value
@@ -29,17 +32,17 @@
                 table.add_rows(data[1:])
             except Exception as e:
                 self.app.push_screen(PopUpScreen(e.__str__()))
 
     def add_completions(self, new_completions: list[str]):
         request_field = self.query_one("#new_request_input", expect_type=Input)
         try:
-            request_field.suggester.add_suggestions(new_completions)
+            request_field.suggester.add_suggestions([] + new_completions)
         except:
             pass
 
     def clean_completions(self):
         input = self.query_one("#new_request_input", expect_type=Input)
         try:
-            input.suggester.set_suggestions([] + sql_abc)
+            input.suggester.set_suggestions([] + SQL_ABC)
         except:
             pass
```

### Comparing `tuidbtv-0.1.6/PKG-INFO` & `tuidbtv-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.6
+Version: 0.1.7
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

