# Comparing `tmp/tuidbtv-0.1.7.tar.gz` & `tmp/tuidbtv-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.7.tar", max compression
+gzip compressed data, was "tuidbtv-0.1.8.tar", max compression
```

## Comparing `tuidbtv-0.1.7.tar` & `tuidbtv-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.7/LICENSE
--rw-r--r--   0        0        0      917 2023-07-07 20:07:56.685489 tuidbtv-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.7/tuidbtv/__init__.py
--rw-r--r--   0        0        0     4687 2023-07-07 20:07:13.436703 tuidbtv-0.1.7/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.7/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.7/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.7/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.7/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.7/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.7/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3303 2023-07-03 18:28:32.471479 tuidbtv-0.1.7/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.7/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.7/tuidbtv/default.css
--rw-r--r--   0        0        0      276 2023-07-07 20:07:13.437708 tuidbtv-0.1.7/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.7/tuidbtv/suggesters/__init__.py
--rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.7/tuidbtv/suggesters/SuggesterDict.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.7/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.7/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.7/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.7/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.7/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.7/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5706 2023-07-03 17:12:50.756478 tuidbtv-0.1.7/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.7/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.8/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-07 21:53:09.681354 tuidbtv-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.8/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     4677 2023-07-07 21:38:37.857844 tuidbtv-0.1.8/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.8/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.8/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.8/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.8/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.8/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.8/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3303 2023-07-03 18:28:32.471479 tuidbtv-0.1.8/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.8/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.8/tuidbtv/default.css
+-rw-r--r--   0        0        0      276 2023-07-07 20:07:13.437708 tuidbtv-0.1.8/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.8/tuidbtv/suggesters/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.8/tuidbtv/suggesters/SuggesterDict.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.8/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.8/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.8/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.8/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.8/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.8/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     5781 2023-07-07 21:46:01.271982 tuidbtv-0.1.8/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.8/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.8/PKG-INFO
```

### Comparing `tuidbtv-0.1.7/LICENSE` & `tuidbtv-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/pyproject.toml` & `tuidbtv-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.7"
+version = "0.1.8"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.7/README.md` & `tuidbtv-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/__main__.py` & `tuidbtv-0.1.8/tuidbtv/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     yield DataTable(id="preview_data_table")
                 with TabPane("editor", id="editor_tab"):
                     yield SQLEditor()
                 with TabPane(" + ", id="add_new_tab_pane"):
                     yield Markdown()
         yield Footer()
 
-    def openConnectionSelectScreen(self, can_quit=False):
+    def openConnectionSelectScreen(self, _firstRun = False):
         def select_connection(db_controller):
             self.dbController = db_controller
             tree = self.query_one(Tree)
             tree.clear()
             tree.root.expand()
             self.suggestions = []
             for schemaName in self.dbController.getSchemaNames():
@@ -62,33 +62,33 @@
                     schema.add_leaf(tableName[0])
                     self.suggestions.append(tableName[0])
                     self.suggestions.append(f"{schemaName[0]}.{tableName[0]}")
             for editor in self.query(SQLEditor).nodes:
                 editor.clean_completions()
                 editor.add_completions(self.suggestions)
 
-        self.push_screen(SelectConnection(_can_quit=can_quit), select_connection)
+        self.push_screen(SelectConnection(firstRun=_firstRun), select_connection)
 
     def on_mount(self) -> None:
-        self.openConnectionSelectScreen(can_quit=False)
+        self.openConnectionSelectScreen(_firstRun=True)
 
     def on_tree_node_selected(self, event: Tree.NodeSelected):
         if not event.node.allow_expand:
             table = self.query_one("#preview_data_table")
             table.clear(columns=True)
             tableData = self.dbController.getTablePreview(event.node.parent.label, event.node.label)
             table.add_columns(*tableData[0])
             table.zebra_stripes = True
             table.add_rows(tableData[1:])
 
     def action_quit_window(self):
         self.push_screen(QuitScreen())
 
     def action_select_connection_window(self):
-        self.openConnectionSelectScreen(can_quit=True)
+        self.openConnectionSelectScreen()
 
     def action_add_new_tab(self):
         tab_pane = self.query_one(TabbedContent)
         add_new_tab_pane = self.query("#add_new_tab_pane").filter("TabPane").first()
         self.tabs_count += 1
         new_tab_id = f"editor_tab{self.tabs_count}"
         tab_pane.add_pane(
```

### Comparing `tuidbtv-0.1.7/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.1.8/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.1.8/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.1.8/tuidbtv/controllers/MySQLController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.1.8/tuidbtv/controllers/PostgresController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.1.8/tuidbtv/controllers/SQLLiteController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/default.css` & `tuidbtv-0.1.8/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/suggesters/SuggesterDict.py` & `tuidbtv-0.1.8/tuidbtv/suggesters/SuggesterDict.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.1.8/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.1.8/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.1.8/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.1.8/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.1.8/tuidbtv/widgets/SelectConnection.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 from tuidbtv.controllers.ControllerFactory import ControllerFactory
 from tuidbtv.widgets.NewConnection import NewConnection
 from tuidbtv.widgets.PopUpScreen import PopUpScreen
 
 
 class SelectConnection(ModalScreen):
     highlighted_index = 0
-    can_quit = True
+    firstRun = True
 
-    def __init__(self, _can_quit=True):
+    def __init__(self, firstRun = False):
         super().__init__()
-        self.can_quit = _can_quit
+        self.firstRun = firstRun
 
     def compose(self) -> ComposeResult:
         yield Grid(
             OptionList(id="select_connection_list"),
             Vertical(
+                Button.success("Connect", id="connect_button", disabled=True),
                 Button("New Connection", variant="primary", id="new_connection_button"),
                 Button("Test connection", id="test_connection_button", disabled=True),
                 Button("Edit connection", id="edit_connection_button", disabled=True),
                 Button.error("Delete Connection", id="delete_connection_button", disabled=True),
             ),
-            Button.warning("Cancel", id="cancel_select_connection_button", disabled=not self.can_quit),
-            Placeholder(),
-            Button.success("Connect", id="connect_button", disabled=True),
+            Button.warning("Quit" if self.firstRun else "Cancel", id="cancel_select_connection_button"),
             id="select_connection_dialog"
         )
 
     def on_mount(self):
         optionList: OptionList = self.queryConnectionsList()
         for connection in ConfigParser.readConnectionList():
             optionList.add_option(connection["connectionName"])
@@ -60,24 +59,27 @@
                     if connection['connectionName'] == selectedOption:
                         try:
                             controller = ControllerFactory.getController(connection)
                             self.dismiss(controller)
                         except:
                             self.app.push_screen(PopUpScreen("Some errors happened while trying to connect :c"))
             case "cancel_select_connection_button":
-                self.app.pop_screen()
+                if self.firstRun:
+                    self.app.exit()
+                else:
+                    self.app.pop_screen()
             case "delete_connection_button":
                 selectedConnection: OptionList = self.queryConnectionsList()
                 selectedOption = selectedConnection.get_option_at_index(self.highlighted_index).prompt.__str__()
                 selectedConnection.remove_option_at_index(self.highlighted_index)
                 ConfigParser.removeConnectionByName(selectedOption)
                 if selectedConnection.option_count == 0:
                     self.query_one("#connect_button").disabled = True
                     self.query_one("#test_connection_button").disabled = True
-                    # self.query_one("#edit_connection_button").disabled = True
+                    self.query_one("#edit_connection_button").disabled = True
                     self.query_one("#delete_connection_button").disabled = True
 
             case "test_connection_button":
                 try:
                     selectedConnection: OptionList = self.queryConnectionsList()
                     selectedOption = selectedConnection.get_option_at_index(self.highlighted_index).prompt.__str__()
                     for connection in ConfigParser.readConnectionList():
```

### Comparing `tuidbtv-0.1.7/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.1.8/tuidbtv/widgets/SQLEditor.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.7/PKG-INFO` & `tuidbtv-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.7
+Version: 0.1.8
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

