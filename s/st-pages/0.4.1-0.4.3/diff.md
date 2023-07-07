# Comparing `tmp/st_pages-0.4.1.tar.gz` & `tmp/st_pages-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pages-0.4.1.tar", max compression
+gzip compressed data, was "st_pages-0.4.3.tar", max compression
```

## Comparing `st_pages-0.4.1.tar` & `st_pages-0.4.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-04-28 21:21:38.777100 st_pages-0.4.1/LICENSE
--rw-r--r--   0        0        0     4597 2023-04-28 21:21:38.777100 st_pages-0.4.1/README.md
--rw-r--r--   0        0        0     1012 2023-04-28 21:21:38.781100 st_pages-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    11017 2023-04-28 21:21:38.781100 st_pages-0.4.1/src/st_pages/__init__.py
--rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 st_pages-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-07 18:32:26.671736 st_pages-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4597 2023-07-07 18:32:26.671736 st_pages-0.4.3/README.md
+-rw-r--r--   0        0        0     1013 2023-07-07 18:32:26.675735 st_pages-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    11290 2023-07-07 18:32:26.675735 st_pages-0.4.3/src/st_pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 18:32:26.675735 st_pages-0.4.3/src/st_pages/py.typed
+-rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 st_pages-0.4.3/PKG-INFO
```

### Comparing `st_pages-0.4.1/LICENSE` & `st_pages-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pages-0.4.1/README.md` & `st_pages-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `st_pages-0.4.1/pyproject.toml` & `st_pages-0.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "st-pages"
-version = "0.4.1"
+version = "0.4.3"
+license = "MIT"
 description = "An experimental version of Streamlit Multi-Page Apps"
 authors = ["Zachary Blackwood <zachary@streamlit.io>"]
 readme = "README.md"
 packages = [{include = "st_pages", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9.7 || >3.9.7,<4.0"
@@ -20,18 +21,21 @@
 pytest-playwright = "^0.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.isort]
-profile = "black"
-line_length = 88
-skip = ["./.venv", "./direnv", ".env"]
+[tool.ruff]
+line-length = 88
+select = [
+    "E",
+    "F",
+    "I001",
+]
 
 [tool.black]
 exclude = '''
 (
   /(
       \.vscode
     | \.git
```

### Comparing `st_pages-0.4.1/src/st_pages/__init__.py` & `st_pages-0.4.3/src/st_pages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,51 +56,54 @@
     page title and favicon in the browser tab.
 
     All **kwargs are passed to st.set_page_config
     """
     pages = get_pages("")
     ctx = get_script_run_ctx()
 
-    if ctx is not None:
-        try:
-            current_page = pages[ctx.page_script_hash]
-        except KeyError:
-            try:
-                current_page = [
-                    p
-                    for p in pages.values()
-                    if p["relative_page_hash"] == ctx.page_script_hash
-                ][0]
-            except IndexError:
-                return
+    if ctx is None:
+        return
 
-        if "page_title" not in kwargs:
-            kwargs["page_title"] = current_page["page_name"]
+    try:
+        current_page = pages[ctx.page_script_hash]
+    except KeyError:
+        try:
+            current_page = [
+                p
+                for p in pages.values()
+                if p["relative_page_hash"] == ctx.page_script_hash
+            ][0]
+        except IndexError:
+            return
 
-        if "page_icon" not in kwargs:
-            kwargs["page_icon"] = current_page["icon"]
+    if "page_title" not in kwargs:
+        kwargs["page_title"] = current_page["page_name"]
 
-        page_title = current_page["page_name"]
-        page_icon = current_page["icon"]
+    if "page_icon" not in kwargs:
+        kwargs["page_icon"] = current_page["icon"]
 
-        try:
-            st.set_page_config(**kwargs)
-        except StreamlitAPIException:
-            pass
+    page_title = current_page["page_name"]
+    page_icon = current_page["icon"]
 
-        if add_icon:
-            st.title(f"{translate_icon(page_icon)} {page_title}")
-        else:
-            st.title(page_title)
+    try:
+        ctx._set_page_config_allowed = True
+        st.set_page_config(**kwargs)
+    except StreamlitAPIException:
+        pass
+
+    if add_icon:
+        st.title(f"{translate_icon(page_icon)} {page_title}")
+    else:
+        st.title(page_title)
 
-        if also_indent:
-            add_indentation()
+    if also_indent:
+        add_indentation()
 
-        if hidden_pages:
-            hide_pages(hidden_pages)
+    if hidden_pages:
+        hide_pages(hidden_pages)
 
 
 add_page_title = _gather_metrics("st_pages.add_page_title", _add_page_title)
 
 
 @cache_resource
 def get_icons() -> dict[str, str]:
@@ -141,14 +144,15 @@
     """
 
     path: str
     name: str | None = None
     icon: str | None = None
     is_section: bool = False
     in_section: bool = True
+    use_relative_hash: bool = False
 
     @property
     def page_path(self) -> Path:
         return Path(str(self.path))
 
     @property
     def page_name(self) -> str:
@@ -168,14 +172,16 @@
     def relative_page_hash(self) -> str:
         if self.is_section:
             return calc_md5(f"{self.page_path}_{self.page_name}")
         return calc_md5(str(self.page_path))
 
     @property
     def page_hash(self) -> str:
+        if self.use_relative_hash:
+            return self.relative_page_hash
         if self.is_section:
             return calc_md5(f"{self.page_path}_{self.page_name}")
         return calc_md5(str(self.page_path.absolute()))
 
     def to_dict(self) -> dict[str, str | bool]:
         return {
             "page_script_hash": self.page_hash,
@@ -220,16 +226,21 @@
     except IndexError:
         raise ValueError("Must pass at least one page to show_pages")
 
     for page in pages:
         if page.is_section:
             page.path = default_page
 
+    first_page_hash = list(current_pages.keys())[0]
+
     current_pages.clear()
-    for page in pages:
+    for idx, page in enumerate(pages):
+        if idx == 0:
+            if page.relative_page_hash == first_page_hash:
+                page.use_relative_hash = True
         current_pages[page.page_hash] = page.to_dict()
 
     _on_pages_changed.send()
 
 
 show_pages = _gather_metrics("st_pages.show_pages", _show_pages)
 
@@ -304,16 +315,17 @@
         elif is_indented and not val.get("in_section"):
             # Page is specifically unnested
             # Un-indent all pages until next section
             is_indented = False
         elif is_indented:
             # Unless specifically unnested, indent all pages that aren't section headers
             styling += f"""
-                div[data-testid=\"stSidebarNav\"] li:nth-child({idx + 1}) span:nth-child(1) {{
-                    margin-left: 1.5rem;
+                div[data-testid=\"stSidebarNav\"] li:nth-child({idx + 1})
+                    span:nth-child(1) {{
+                        margin-left: 1.5rem;
                 }}
             """
 
     styling = f"""
         <style>
             {styling}
         </style>
```

### Comparing `st_pages-0.4.1/PKG-INFO` & `st_pages-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: st-pages
-Version: 0.4.1
+Version: 0.4.3
 Summary: An experimental version of Streamlit Multi-Page Apps
+License: MIT
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: streamlit (>=1.10.0)
```

