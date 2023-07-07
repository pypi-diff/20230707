# Comparing `tmp/vja-2.0.0rc3.tar.gz` & `tmp/vja-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0rc3.tar", last modified: Mon Jun  5 19:00:43 2023, max compression
+gzip compressed data, was "vja-2.0.0rc4.tar", last modified: Mon Jun 12 19:51:42 2023, max compression
```

## Comparing `vja-2.0.0rc3.tar` & `vja-2.0.0rc4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-05 19:00:43.198216 vja-2.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 19:00:43.198216 vja-2.0.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-05 18:59:55.000000 vja-2.0.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.195471 vja-2.0.0rc3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)    10103 2023-06-05 18:59:55.000000 vja-2.0.0rc3/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17977 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     5756 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/project_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-05 18:59:55.000000 vja-2.0.0rc3/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:00:43.197301 vja-2.0.0rc3/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-05 19:00:43.000000 vja-2.0.0rc3/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:51:42.444196 vja-2.0.0rc4/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-12 19:51:42.444196 vja-2.0.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-12 19:51:42.445196 vja-2.0.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-12 19:50:59.000000 vja-2.0.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:51:42.442196 vja-2.0.0rc4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 19:50:59.000000 vja-2.0.0rc4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-12 19:50:59.000000 vja-2.0.0rc4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-12 19:50:59.000000 vja-2.0.0rc4/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-12 19:50:59.000000 vja-2.0.0rc4/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)    10103 2023-06-12 19:50:59.000000 vja-2.0.0rc4/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:51:42.443196 vja-2.0.0rc4/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17977 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5756 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/project_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10245 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-12 19:50:59.000000 vja-2.0.0rc4/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:51:42.444196 vja-2.0.0rc4/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 19:51:42.000000 vja-2.0.0rc4/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0rc3/PKG-INFO` & `vja-2.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc3/setup.py` & `vja-2.0.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/tests/conftest.py` & `vja-2.0.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/tests/test_basic.py` & `vja-2.0.0rc4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/tests/test_command.py` & `vja-2.0.0rc4/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/tests/test_query.py` & `vja-2.0.0rc4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/apiclient.py` & `vja-2.0.0rc4/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/authenticate.py` & `vja-2.0.0rc4/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/cli.py` & `vja-2.0.0rc4/vja/cli.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/config.py` & `vja-2.0.0rc4/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/filter.py` & `vja-2.0.0rc4/vja/filter.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/model.py` & `vja-2.0.0rc4/vja/model.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/output.py` & `vja-2.0.0rc4/vja/output.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/parse.py` & `vja-2.0.0rc4/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/project_service.py` & `vja-2.0.0rc4/vja/project_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/service_command.py` & `vja-2.0.0rc4/vja/service_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,16 +95,14 @@
         task_remote.update({'id': None})
         task_remote.update({'title': title})
         task_remote.update({'position': 0})
         task_remote.update({'kanban_position': 0})
         if is_clone_bucket:
             task_remote.update({'bucket_id': 0})
 
-        # make sure we do not send back the old reminder_dates
-        task_remote.pop("reminder_dates", None)
         logger.debug('put task: %s', task_remote)
         task_json = self._api_client.put_task(task_remote['project_id'], task_remote)
         task = self._task_service.task_from_json(task_json)
 
         for label in task_remote['labels']:
             self._api_client.add_label_to_task(task.id, label['id'])
         return task
@@ -120,16 +118,14 @@
             args.update({
                 'note': task_remote['description'] + '\n' + append_note if task_remote['description'] else append_note
             })
 
         payload = self._args_to_payload(args)
         logger.debug('update fields: %s', payload)
         task_remote.update(payload)
-        # make sure we do not send back the old reminder_dates
-        task_remote.pop("reminder_dates", None)
         logger.debug('post task: %s', task_remote)
         task_json = self._api_client.post_task(task_id, task_remote)
         task_new = self._task_service.task_from_json(task_json)
 
         label = self._label_from_name(label_name, is_force) if label_name else None
         if label:
             if task_new.has_label(label):
@@ -176,16 +172,14 @@
                 {'reminder': None})  # --reminder=""
         else:
             args.update(
                 {'reminder': [{'reminder': parse_date_arg_to_iso(reminder_arg)}]})
 
     def toggle_task_done(self, task_id):
         task_remote = self._api_client.get_task(task_id)
-        # make sure we do not send back the old reminder_dates
-        task_remote.pop("reminder_dates", None)
         task_remote.update({'done': not task_remote['done']})
         task_json = self._api_client.post_task(task_id, task_remote)
         return self._task_service.task_from_json(task_json)
 
     def defer_task(self, task_id, delay_by):
         timedelta = parse_date_arg_to_timedelta(delay_by)
         args = {}
@@ -206,16 +200,14 @@
             if reminder_date and is_absolute_reminder:
                 args.update({'reminder': datetime_to_isoformat(reminder_date + timedelta)})
                 self._update_reminder(args, task_remote)
 
         payload = self._args_to_payload(args)
         logger.debug('update fields: %s', payload)
         task_remote.update(payload)
-        # make sure we do not send back the old reminder_dates
-        task_remote.pop("reminder_dates", None)
         task_json = self._api_client.post_task(task_id, task_remote)
         return self._task_service.task_from_json(task_json)
 
     def _label_from_name(self, name, is_force):
         if not name:
             return None
         labels_remote = Label.from_json_array(self._api_client.get_labels())
```

### Comparing `vja-2.0.0rc3/vja/service_query.py` & `vja-2.0.0rc4/vja/service_query.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/task_service.py` & `vja-2.0.0rc4/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja/urgency.py` & `vja-2.0.0rc4/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc3/vja.egg-info/PKG-INFO` & `vja-2.0.0rc4/vja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc3/vja.egg-info/SOURCES.txt` & `vja-2.0.0rc4/vja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

