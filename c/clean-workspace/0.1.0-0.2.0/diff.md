# Comparing `tmp/clean_workspace-0.1.0.tar.gz` & `tmp/clean_workspace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_workspace-0.1.0.tar", max compression
+gzip compressed data, was "clean_workspace-0.2.0.tar", max compression
```

## Comparing `clean_workspace-0.1.0.tar` & `clean_workspace-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2022-10-06 13:37:49.000000 clean_workspace-0.1.0/LICENSE
--rw-r--r--   0        0        0     1464 2023-05-04 15:07:13.848181 clean_workspace-0.1.0/README.md
--rw-r--r--   0        0        0     6847 2023-06-09 23:11:53.340390 clean_workspace-0.1.0/clean_workspace/__init__.py
--rw-r--r--   0        0        0      655 2023-04-05 15:56:02.526260 clean_workspace-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 clean_workspace-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-07 14:11:37.204209 clean_workspace-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1945 2023-07-07 14:11:37.204505 clean_workspace-0.2.0/README.md
+-rw-r--r--   0        0        0     7639 2023-07-07 14:11:37.205823 clean_workspace-0.2.0/clean_workspace/__init__.py
+-rw-r--r--   0        0        0      762 2023-07-07 14:13:03.605335 clean_workspace-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 clean_workspace-0.2.0/PKG-INFO
```

### Comparing `clean_workspace-0.1.0/LICENSE` & `clean_workspace-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_workspace-0.1.0/README.md` & `clean_workspace-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Clean Workspace: Archive Web Browser Tabs
 
 I've been experimenting with how to make my mornings more productive. One glitch I've found in my mind is I can easily
 get distracted by open tabs on my browser, especially if I'm trying to write or read something which I want to give
-my full attention to. I've found that if I close all my tabs, I can focus better on the task at hand. However, I don't
+my full attention to. I've found that if I close all my tabs (similar idea to [shrinking context size](http://mikebian.co/improve-motivation-and-focus-with-small-contexts/)), I can focus better on the task at hand. However, I don't
 want to lose any interesting tabs so I never actually do that.
 
 This is simple utility to automate this process. It will close all your tabs (in both Safari & Chrome), and send them to [todoist](https://mikebian.co/todoist) (and output) them to the terminal.
 
 We'll see if this actually helps!
 
 ## Installation
@@ -30,11 +30,18 @@
 osascript <<EOT
 set dialogResult to display dialog "What were you working on yesterday?" buttons {"OK"} default button "OK" giving up after 300 default answer ""
 return text returned of dialogResult
 EOT
 )
 ```
 
+Here's a [full example](https://github.com/iloveitaly/dotfiles/blob/648010ec9a9c8f1fb0aa70be138994689f3bbfb3/.config/focus/initial_wake.sh#L42-L53) of using this with [hyper-focus](https://www.raycast.com/iloveitaly/hyper-focus).
+
 ## Inspiration
 
 - https://gist.github.com/aleks-mariusz/cc27b21f2c5b91fbd285
 - https://github.com/tominsam/shelf-python/blob/f357d9b147fa651034b71501edabf65f59d5befa/extractors/ComAppleSafari.py#L11
+
+## TODO
+
+- [ ] Indicate in python config that this is macOS only in poetry config?
+- [ ] move blacklist files into example area of repo
```

### Comparing `clean_workspace-0.1.0/clean_workspace/__init__.py` & `clean_workspace-0.2.0/clean_workspace/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import plistlib
 import sys
 import typing as t
+import click
 
-from ScriptingBridge import SBApplication
 import chrome_bookmarks
+from ScriptingBridge import SBApplication
+
 
 def todoist_client():
     # extract todoist api key from environment without throwing an exception
     todoist_api_key = os.environ.get("TODOIST_API_KEY", None)
 
     if not todoist_api_key:
         print("todoist api key not found in environment")
@@ -17,17 +19,19 @@
     print("todoist api key found, adding to todoist")
 
     from todoist_api_python.api import TodoistAPI
 
     api = TodoistAPI(todoist_api_key)
     return api
 
+
 def export_to_todoist(task_content, description):
     # TODO should also support .env here as well
     import dotenv
+
     dotenv.load_dotenv(".envrc")
 
     api = todoist_client()
     if not api:
         return
 
     import datetime
@@ -36,41 +40,41 @@
     project = None
     projects = api.get_projects()
     project_matches = [project for project in projects if project.name == project_name]
 
     if len(project_matches) == 1:
         project = project_matches[0]
 
-
     # find a label called "web-archive" or create it
     label_name = os.environ.get("TODOIST_LABEL", "web-archive")
     labels = api.get_labels()
     label_matches = [label for label in labels if label.name == label_name]
 
     # assigning label for debugging
     if len(label_matches) == 0:
         # https://developer.todoist.com/rest/v1/#create-a-new-label
         print(f"could not find {label_name} label, creating it")
-        label = api.add_label(name=label_name)
+        api.add_label(name=label_name)
     else:
-        label = label_matches[0]
+        label_matches[0]
 
     # https://developer.todoist.com/rest/v2#create-a-new-task
-    response = api.add_task(
+    api.add_task(
         # set content to "web archive CURRENT_DAY" using format YYYY-MM-DD
         content="{}web archive {}".format(
             description, datetime.datetime.now().strftime("%Y-%m-%d")
         ),
         description=task_content,
         # date is serialized in the task description, no need for a due date
         due_string="no date",
         labels=[label_name],
         project_id=project.id if project else None,
     )
 
+
 def get_browser_urls() -> t.List[str]:
     browser_urls = []
     chrome = SBApplication.applicationWithBundleIdentifier_("com.google.Chrome")
 
     for window in chrome.windows():
         for tab in window.tabs():
             browser_urls.append((tab.URL(), tab.name()))
@@ -81,14 +85,15 @@
         for tab in window.tabs():
             browser_urls.append((tab.URL(), tab.name()))
             # it doesn't look possible to close out the tabs with SBApplication :/
             # instead we just close out the whole application below
 
     return browser_urls
 
+
 def get_bookmarks_urls() -> t.List[str]:
     raw_bookmark_urls = [bookmark.url for bookmark in chrome_bookmarks.urls]
 
     # read all safari bookmarks, don't include these in the printout
     with open(os.path.expanduser("~") + "/Library/Safari/Bookmarks.plist", "rb") as f:
         bookmarks_plist = plistlib.load(f)
 
@@ -99,36 +104,29 @@
 
         safari_bookmarks = [
             child
             for child in bookmarks_plist["Children"]
             if child["Title"] == "BookmarksBar"
         ][0]["Children"]
 
-        raw_safari_bookmark_urls = [bookmark["URLString"] for bookmark in safari_bookmarks]
+        raw_safari_bookmark_urls = [
+            bookmark["URLString"] for bookmark in safari_bookmarks
+        ]
 
         raw_bookmark_urls.extend(raw_safari_bookmark_urls)
 
     return [bookmark.split("#")[0] for bookmark in raw_bookmark_urls]
 
+
 def quit_browsers():
     os.system("osascript -e 'quit app \"Safari\"'")
     os.system("osascript -e 'quit app \"Chrome\"'")
 
-def main():
-    if not is_internet_connected():
-        print("internet is not connected")
-        return
-
-    # TODO maybe optionally collect via applescript input dialog? We'd need to develop a proper interface for the CLI at that point.
-    # get first CLI argument if it exists
-    if len(sys.argv) > 1 and sys.argv[1].strip():
-        tab_description = sys.argv[1].strip() + " "
-    else:
-        tab_description = ""
 
+def clean_workspace(tab_description, blacklist_domains, blacklist_urls):
     browser_urls = get_browser_urls()
 
     # if page is blank, there is no url or string does not contain http
     browser_urls = [x for x in browser_urls if x[0] is not None and "http" in x[0]]
 
     # remove duplicates
     browser_urls = list(set(browser_urls))
@@ -139,31 +137,34 @@
     # strip all anchors from the urls
     browser_urls = [(url.split("#")[0], name) for url, name in browser_urls]
 
     # TODO load these files from a home config file
 
     # user configurable blacklist for urls you don't want to archive
     url_blacklist = []
-    with open("blacklist_urls.txt", "r") as f:
+    with open(blacklist_urls, "r") as f:
         url_blacklist = f.read().splitlines()
 
     domain_blacklist = []
-    with open("blacklist_domains.txt", "r") as f:
+    with open(blacklist_domains, "r") as f:
         domain_blacklist = f.read().splitlines()
         # add a `www.` prefix to each domain in the blacklist and merge it with the existing list
         domain_blacklist = domain_blacklist + [
             "www." + domain for domain in domain_blacklist
         ]
 
     bookmark_urls = get_bookmarks_urls()
 
     # TODO output skipped domains
     # TODO support wildcard subdomains, *.sentry.io
+
     # filter all urls with blacklisted domains
-    browser_urls = [x for x in browser_urls if x[0].split("/")[2] not in domain_blacklist]
+    browser_urls = [
+        x for x in browser_urls if x[0].split("/")[2] not in domain_blacklist
+    ]
 
     # join url and name with "-" and print to stdout
     todoist_content = ""
     for url_with_name in browser_urls:
         if (
             # if the url is in the bookmark list of chrome or safari, skip it
             url_with_name[0] not in bookmark_urls
@@ -183,24 +184,61 @@
     print(f"\n{todoist_content}\n")
 
     # since we've archived all content we can now close out Safari & Chrome
     quit_browsers()
 
     export_to_todoist(todoist_content, tab_description)
 
-    archive_old_tasks()
+
+@click.command()
+@click.option("--blacklist-domains", type=click.Path(), default=None)
+@click.option("--blacklist-urls", type=click.Path(), default=None)
+@click.option("--tab-description", default="", help="Description for tab")
+def main(tab_description, blacklist_domains, blacklist_urls):
+    if not is_internet_connected():
+        print("internet is not connected")
+        return
+
+    home_dir = os.path.expanduser("~")
+
+    if blacklist_domains is None:
+        default_domains_path = os.path.join(
+            home_dir, ".config", "clean-workspace", "blacklist_domains.txt"
+        )
+        blacklist_domains = (
+            default_domains_path
+            if os.path.exists(default_domains_path)
+            else "blacklist_domains.txt"
+        )
+
+    if blacklist_urls is None:
+        default_urls_path = os.path.join(
+            home_dir, ".config", "clean-workspace", "blacklist_urls.txt"
+        )
+        blacklist_urls = (
+            default_urls_path
+            if os.path.exists(default_urls_path)
+            else "blacklist_urls.txt"
+        )
+
+    clean_workspace(tab_description, blacklist_domains, blacklist_urls)
+
 
 def archive_old_tasks():
     # find all old tasks (>1mo) and archive them
     # optionally only do this when there is not a custom name in the title
     pass
 
+
 def is_internet_connected():
     import socket
+
     s = socket.socket(socket.AF_INET)
     try:
-        s.connect(("google.com",80))
+        s.connect(("google.com", 80))
         return True
-    except socket.error as e: return False
+    except socket.error:
+        return False
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `clean_workspace-0.1.0/PKG-INFO` & `clean_workspace-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: clean-workspace
-Version: 0.1.0
+Version: 0.2.0
 Summary: Collect all browser URLs, output to terminal, and archive to todoist
+Home-page: https://github.com/iloveitaly/clean-workspace
 License: MIT
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chrome-bookmarks (>=2020.10.25,<2021.0.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: pyobjc-framework-ScriptingBridge (>=9.0.1,<10.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: todoist-api-python (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Clean Workspace: Archive Web Browser Tabs
 
 I've been experimenting with how to make my mornings more productive. One glitch I've found in my mind is I can easily
 get distracted by open tabs on my browser, especially if I'm trying to write or read something which I want to give
-my full attention to. I've found that if I close all my tabs, I can focus better on the task at hand. However, I don't
+my full attention to. I've found that if I close all my tabs (similar idea to [shrinking context size](http://mikebian.co/improve-motivation-and-focus-with-small-contexts/)), I can focus better on the task at hand. However, I don't
 want to lose any interesting tabs so I never actually do that.
 
 This is simple utility to automate this process. It will close all your tabs (in both Safari & Chrome), and send them to [todoist](https://mikebian.co/todoist) (and output) them to the terminal.
 
 We'll see if this actually helps!
 
 ## Installation
@@ -48,12 +50,19 @@
 osascript <<EOT
 set dialogResult to display dialog "What were you working on yesterday?" buttons {"OK"} default button "OK" giving up after 300 default answer ""
 return text returned of dialogResult
 EOT
 )
 ```
 
+Here's a [full example](https://github.com/iloveitaly/dotfiles/blob/648010ec9a9c8f1fb0aa70be138994689f3bbfb3/.config/focus/initial_wake.sh#L42-L53) of using this with [hyper-focus](https://www.raycast.com/iloveitaly/hyper-focus).
+
 ## Inspiration
 
 - https://gist.github.com/aleks-mariusz/cc27b21f2c5b91fbd285
 - https://github.com/tominsam/shelf-python/blob/f357d9b147fa651034b71501edabf65f59d5befa/extractors/ComAppleSafari.py#L11
 
+## TODO
+
+- [ ] Indicate in python config that this is macOS only in poetry config?
+- [ ] move blacklist files into example area of repo
+
```

