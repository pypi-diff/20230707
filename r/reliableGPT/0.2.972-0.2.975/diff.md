# Comparing `tmp/reliableGPT-0.2.972.tar.gz` & `tmp/reliableGPT-0.2.975.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.972.tar", last modified: Thu Jul  6 19:25:26 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.975.tar", last modified: Fri Jul  7 01:41:49 2023, max compression
```

## Comparing `reliableGPT-0.2.972.tar` & `reliableGPT-0.2.975.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.693442 reliableGPT-0.2.972/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.972/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-06 19:25:26.693321 reliableGPT-0.2.972/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.690391 reliableGPT-0.2.972/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.692875 reliableGPT-0.2.972/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-06 19:23:20.000000 reliableGPT-0.2.972/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    16639 2023-07-06 19:19:57.000000 reliableGPT-0.2.972/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.972/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7483 2023-07-06 13:49:42.000000 reliableGPT-0.2.972/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      375 2023-07-06 17:39:33.000000 reliableGPT-0.2.972/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4762 2023-07-06 19:20:43.000000 reliableGPT-0.2.972/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-06 19:25:26.693502 reliableGPT-0.2.972/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-06 19:25:18.000000 reliableGPT-0.2.972/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.763665 reliableGPT-0.2.975/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.975/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:41:49.763552 reliableGPT-0.2.975/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8271 2023-07-03 21:43:04.000000 reliableGPT-0.2.975/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.760801 reliableGPT-0.2.975/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      514 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.763203 reliableGPT-0.2.975/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/reliablegpt/APICallHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3284 2023-07-07 00:13:35.000000 reliableGPT-0.2.975/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/reliablegpt/CustomQueue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    18148 2023-07-07 01:39:23.000000 reliableGPT-0.2.975/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.975/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.975/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7483 2023-07-06 16:11:58.000000 reliableGPT-0.2.975/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      375 2023-07-06 16:14:08.000000 reliableGPT-0.2.975/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5167 2023-07-07 01:37:33.000000 reliableGPT-0.2.975/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-03 21:42:46.000000 reliableGPT-0.2.975/reliablegpt/reliableQuery.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-07 01:41:49.763701 reliableGPT-0.2.975/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-07 01:41:30.000000 reliableGPT-0.2.975/setup.py
```

### Comparing `reliableGPT-0.2.972/LICENSE` & `reliableGPT-0.2.975/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/README.md` & `reliableGPT-0.2.975/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.975/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.975/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/Alerting.py` & `reliableGPT-0.2.975/reliablegpt/Alerting.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,25 +58,27 @@
     else:
       self.user_emails.add(user_email)
     return
 
   def add_error(self, openai_error=None, error_description=None, error_type=None):
     if openai_error != None:
       openai_error = openai_error.error  # index into the error attribute of the class
-      if "type" in openai_error:
-        error_type = openai_error['type']
+    error_type = error_type  # defalt to being None
+    if openai_error != None and 'type' in openai_error:
+      error_type = openai_error['type']
     elif error_description and error_type:
       error_type = error_type
       openai_error = error_description
     now = datetime.datetime.now()
     curr_time = now.hour
 
     if curr_time == self.current_time_block:
       if error_type in self.unhandled_errors:
         self.unhandled_errors[error_type] += 1
+        print(f"Got unhandled error {self.unhandled_errors}")
       else:
         self.unhandled_errors[error_type] = 1
       if self.unhandled_errors[error_type] >= 5:
         self.unhandled_errors[error_type] = 0  # reset this to 0
         # cooldown for 15 minutes -> do this to prevent email spam.
         if self.set_cooldown and time.time() - self.cooldown_start_time > 900:
           self.send_alert(error_type, openai_error)
```

### Comparing `reliableGPT-0.2.972/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.975/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.975/reliablegpt/IndividualRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     self.user_email = user_email
     self.user_token = user_token
     self.save_request = logging_fn
     self.backup_openai_key = backup_openai_key
     self.print_verbose(f"INIT fallback strategy {self.fallback_strategy}")
     self.caching = caching
     self.max_threads = max_threads
+    self.print_verbose(f"INIT with threads {self.max_threads} {self.caching} {max_threads}")
     self.alerting = alerting
 
   def print_verbose(self, print_statement):
     if self.verbose:
       print(colored("Individual Request: " + print_statement, "blue"))
 
   ## Code that handles / wraps openai calls
@@ -74,40 +75,57 @@
         self.save_request(
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.request',
         )
       except:
         print("ReliableGPT error occured during saving request")
-      self.print_verbose(f"max threads: {self.max_threads}, caching: {self.caching}")
+      self.print_verbose(f"Cache check {self.max_threads} {self.caching}")
       if self.max_threads and self.caching:
+        self.print_verbose(f'current util: {active_count()/self.max_threads}')
         thread_utilization = active_count()/self.max_threads
         self.print_verbose(f"Thread utilization: {thread_utilization}")
         if thread_utilization > 0.8: # over 80% utilization of threads, start returning cached responses
           if "messages" in kwargs and self.caching:
             print(kwargs["messages"])
             input_prompt = "\n".join(message["content"]
                                     for message in kwargs["messages"])
             self.print_verbose(
               f"queue depth is higher than the threshold, start caching")
             result = self.try_cache_request(query=input_prompt)
             if self.alerting:
+              # save_exception
               self.alerting.add_error(error_type="Thread Utilization > 85%", error_description="Your thread utilization is over 85%. We've started responding with cached results, to prevent requests from dropping. Please increase capacity (allocate more threads/servers) to prevent result quality from dropping.")
             if result == None: # cache miss!
               pass
             else:
               self.print_verbose(f"returns cached result: {result}")
+              self.save_request(
+                user_email=self.user_email,
+                posthog_event='reliableGPT.recovered_request_cache',
+                graceful_string = self.graceful_string,
+                result=result,
+                posthog_metadata={
+                  'error': 'High Thread Utilization',
+                  'recovered_response': result,
+                },
+                errors=['High Thread Utilization'],
+                function_name=str(self.model_function),
+                kwargs=kwargs
+              )
               return result
-      print("received request")
+      # print("received request")
+      # Run user request
       result = self.model_function(*args, **kwargs)
       if "messages" in kwargs and self.caching:
         print(kwargs["messages"])
         input_prompt = "\n".join(message["content"]
                                  for message in kwargs["messages"])
         extracted_result = result['choices'][0]['message']['content']
+        self.print_verbose(f'This is extracted result {extracted_result}')
         self.add_cache(
           input_prompt, extracted_result
         )  # [TODO] turn this into a threaded call, reduce latency.
       self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
       self.print_verbose("catches the error")
@@ -152,16 +170,18 @@
             querystring = {
                 "customer_id": customer_id,
                 "instance_id": instance_id, 
                 "user_email": user_email, 
                 "input_prompt": query,
             }
             response = requests.get(url, params=querystring)
-            print(f"cached response: {response}")
-            return response.json()["response"]
+            self.print_verbose(f"cached response: {response.json()}")
+            extracted_result = response.json()["response"]
+            results = {"choices":[{"message":{"content": extracted_result}}]}
+            return results
     except:
       traceback.print_exc()
       pass
     self.print_verbose(f"cache miss!")
     return None
 
   def fallback_request(self, args, kwargs, fallback_strategy):
@@ -366,14 +386,27 @@
           print(kwargs["messages"])
           input_prompt = "\n".join(message["content"]
                                    for message in kwargs["messages"])
           cached_response = self.try_cache_request(query=input_prompt)
           if cached_response == None:
             pass
           else:
+            self.save_request(
+              user_email=self.user_email,
+              posthog_event='reliableGPT.recovered_request_cache',
+              graceful_string = self.graceful_string,
+              result=cached_response,
+              posthog_metadata={
+                'error': 'High Thread Utilization',
+                'recovered_response': cached_response,
+              },
+              errors=['High Thread Utilization'],
+              function_name=str(self.model_function),
+              kwargs=kwargs
+            )
             return cached_response
         print("returns graceful string")
         self.save_request(
           user_email=self.user_email,
           graceful_string=self.graceful_string,
           posthog_event='reliableGPT.recovered_request_exception',
           result=result,
```

### Comparing `reliableGPT-0.2.972/reliablegpt/Model.py` & `reliableGPT-0.2.975/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.975/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.975/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.972/reliablegpt/main.py` & `reliableGPT-0.2.975/reliablegpt/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # # Prod Imports
-# from reliablegpt.IndividualRequest import IndividualRequest
-# from reliablegpt.RateLimitHandler import RateLimitHandler
-# from reliablegpt.Model import Model
-# from reliablegpt.Alerting import Alerting
-# from reliablegpt.reliableQuery import reliable_query
+from reliablegpt.IndividualRequest import IndividualRequest
+from reliablegpt.RateLimitHandler import RateLimitHandler
+from reliablegpt.Model import Model
+from reliablegpt.alerting import Alerting
+from reliablegpt.reliableQuery import reliable_query
 import requests
 
 # # Dev Imports
-from IndividualRequest import IndividualRequest
-from Model import Model
-from Alerting import Alerting
+# from IndividualRequest import IndividualRequest
+# from Model import Model
+# from Alerting import Alerting
 
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -58,14 +58,21 @@
       # Log handled and unahndled exceptions in R-GPT servers
       if posthog_event == 'reliableGPT.recovered_request':
         original_error = ""
         if 'error' in posthog_metadata:
           original_error = posthog_metadata['error']
         save_exception(type = 'handled', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
 
+      # Log handled and unahndled exceptions in R-GPT servers
+      if posthog_event == 'reliableGPT.recovered_request_cache':
+        original_error = ""
+        if 'error' in posthog_metadata:
+          original_error = posthog_metadata['error']
+        save_exception(type = 'handled cache', user_email=user_email, result=result, original_error=original_error, function_name=function_name, kwargs=kwargs)
+
       # Log unhandled exceptions in R-GPT servers
       if posthog_event == 'reliableGPT.recovered_request_exception':
         original_error = ""
         error2 = ""
         if 'error' in posthog_metadata:
           original_error = posthog_metadata['error']
         if 'error2' in posthog_metadata:
```

### Comparing `reliableGPT-0.2.972/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.975/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

