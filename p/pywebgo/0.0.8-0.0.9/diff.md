# Comparing `tmp/pywebgo-0.0.8.tar.gz` & `tmp/pywebgo-0.0.9.tar.gz`

## Comparing `pywebgo-0.0.8.tar` & `pywebgo-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.8/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.8/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.9/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    15299 2020-02-02 00:00:00.000000 pywebgo-0.0.9/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.9/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.9/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.9/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.9/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.9/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.9/PKG-INFO
```

### Comparing `pywebgo-0.0.8/.github/workflows/python-publish.yml` & `pywebgo-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/src/pywebgo/controller.py` & `pywebgo-0.0.9/src/pywebgo/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     - :class:`list` urls --> non-linked web pages to traverse through
     - :class:`bool` teardown --> closes the browser after execution if true
     - :class:`float` wait --> time delay for executing each action
     - :class:`ElementsHandler` elem_handler --> instance of ElementsHandler class to manage elements
     - :class:`DataHandler` data_handler --> instance of DataHandler class to manage data associated with the elements
     """
 
-    def __init__(self, urls: list, teardown: bool = True, wait: float = 0,
+    def __init__(self, urls: list, timeout: float, teardown: bool = True, wait: float = 0,
                  options: list = None, retry_attempts: int = 1, detach: bool = False):
         """
         Initialize a new instance of the WebController class.
 
         :param urls: non-linked web pages to traverse through
+        :param timeout: timeout for each operation during execution
         :param teardown: closes the browser after execution if true
         :param wait: time delay for executing each action
         """
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_experimental_option("excludeSwitches", ["disable-popup-blocking"])
         chrome_options.add_experimental_option("detach", detach)
         if options:
@@ -44,14 +45,15 @@
                 chrome_options.add_argument(option)
 
         super(WebController, self).__init__(chrome_options=chrome_options)
 
         # ---- Private Variables ----- #
         self.urls = urls
         self.wait = wait
+        self.timeout = timeout
         self.teardown = teardown
         self.retry_attempts = retry_attempts
         self.elem_handler = ElementsHandler()
         self.data_handler = DataHandler()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
@@ -114,40 +116,41 @@
             if this_action == 'send-keys':
                 web_element.send_keys(element['keys'])
                 return
             if this_action == 'select':
                 Select(web_element).select_by_visible_text(element['keys'])
             self.perform_action_chains(this_action, web_element)
 
-    def execute_operations(self, timeout: float = 20) -> None:
+    def execute_operations(self) -> None:
         """
         Execute all the operations associated with the current WebController object.
 
-        :param timeout: time before throwing exception if the element is not found
         """
         # Load the first url
         start_url = self.urls[0]
         self.load_page(start_url)
         for element in self.elem_handler.elements:
             index = self.elem_handler.elements.index(element)
             # Switch window if the element is located in a different window
             self.switch_window(element)
             # Call the custom function if it exists
             if callable(element['custom']):
                 element['custom'](self, element)
                 continue
-            web_element = self.get_element(element, self.retry_attempts, timeout)
+            web_element = self.get_element(element,
+                                           self.retry_attempts,
+                                           self.timeout)
             self.elem_handler.store_web_element(web_element)
             self.retrieve_data(web_element, element)
             self.execute_actions(web_element, element)
             self.load_next_page(index)
             # Handle alert if appears after any action
             self.handle_alert(element, web_element)
 
-    def get_active_element(self, timeout):
+    def get_active_element(self, timeout: float):
         """
         Switch to and return the active web element object.
 
         :param timeout: time before throwing exception if the element is not found
         :return: active web element
         """
         active_element = self.switch_to.active_element
@@ -189,17 +192,20 @@
         :param url: URL of a web page
         :return: requested HTML of a web page
         """
         if url:
             self.load_page(url)
         return self.page_source
 
-    def handle_alert(self, element, web_element) -> None:
+    def handle_alert(self, element: dict, web_element: WebElement) -> None:
         """
         Handle any alert that may be present on the page.
+
+        :param element: a dictionary containing WebElement specifications
+        :param web_element: element to perform action on after handling alert
         """
         try:
             alert = self.switch_to.alert
             alert.accept()
             # Retry the last operation
             self.execute_actions(web_element, element)
         except (NoAlertPresentException, NoSuchWindowException):
@@ -343,32 +349,31 @@
         if isinstance(element, WebElement):
             wait.until(expected_conditions.visibility_of(element))
         else:
             identifiers = utils.get_element_identifiers(element)
             (strategy, locator) = (identifiers['strategy'], identifiers['locator'])
             wait.until(expected_conditions.visibility_of_element_located((strategy, locator)))
 
-    def element_exists(self, element, retry=0, timeout=0) -> bool:
+    def element_exists(self, element: dict, retry: int, timeout: float) -> bool:
         """
         Check if an element exists.
 
         :param element: dictionary containing element specifications
         :param retry: the number of retry attempts to find an element
         :param timeout: wait time before throwing an exception
         :return: bool flag to assert the existence of an element
         """
         try:
             self.get_element(element, retry, timeout)
             return True
         except NoSuchElementException:
             return False
 
-    def run_controller(self, elements: list, timeout: float = 20) -> None:
+    def run_controller(self, elements: list) -> None:
         """
         Runs the controller to initiate the execution of the operations.
 
-        :param timeout:
         :param elements: elements to interact with
         """
         self.create_elements(elements)
         self.elem_handler.sort_elements_by_rank()
-        self.execute_operations(timeout=timeout)
+        self.execute_operations()
```

### Comparing `pywebgo-0.0.8/src/pywebgo/data.py` & `pywebgo-0.0.9/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/src/pywebgo/elements.py` & `pywebgo-0.0.9/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/src/pywebgo/utils.py` & `pywebgo-0.0.9/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/.gitignore` & `pywebgo-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/LICENSE` & `pywebgo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.8/pyproject.toml` & `pywebgo-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.8/PKG-INFO` & `pywebgo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.8
+Version: 0.0.9
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

