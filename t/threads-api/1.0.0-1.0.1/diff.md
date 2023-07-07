# Comparing `tmp/threads-api-1.0.0.tar.gz` & `tmp/threads-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.0.tar", last modified: Thu Jul  6 22:48:26 2023, max compression
+gzip compressed data, was "threads-api-1.0.1.tar", last modified: Fri Jul  7 21:30:13 2023, max compression
```

## Comparing `threads-api-1.0.0.tar` & `threads-api-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-06 22:48:26.073092 threads-api-1.0.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.0/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-06 22:48:26.073092 threads-api-1.0.0/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3145 2023-07-06 22:48:00.000000 threads-api-1.0.0/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.0/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-06 22:48:26.073092 threads-api-1.0.0/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      610 2023-07-06 22:47:29.000000 threads-api-1.0.0/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-06 22:48:26.073092 threads-api-1.0.0/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.0/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-06 22:48:26.073092 threads-api-1.0.0/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.0/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8528 2023-07-06 22:12:47.000000 threads-api-1.0.0/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-06 22:48:26.073092 threads-api-1.0.0/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.0/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-06 22:37:38.000000 threads-api-1.0.0/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-06 22:48:26.073092 threads-api-1.0.0/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-06 22:48:26.000000 threads-api-1.0.0/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-06 22:48:26.000000 threads-api-1.0.0/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-06 22:48:26.000000 threads-api-1.0.0/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-06 22:48:26.000000 threads-api-1.0.0/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-06 22:48:26.000000 threads-api-1.0.0/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-07 21:30:13.242602 threads-api-1.0.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9206 2023-07-07 21:26:44.000000 threads-api-1.0.1/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.1/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-07 21:30:13.242602 threads-api-1.0.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      610 2023-07-07 21:30:11.000000 threads-api-1.0.1/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.238602 threads-api-1.0.1/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.1/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.1/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.1/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.1/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.1/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-07 21:30:13.242602 threads-api-1.0.1/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      493 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-07 21:30:13.000000 threads-api-1.0.1/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.0/LICENSE` & `threads-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.0/setup.py` & `threads-api-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='threads-api',
-    version='1.0.0',
+    version='1.0.1',
     description='Unofficial Python client for Meta Threads API',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
     install_requires=[
         'aiohttp',
```

### Comparing `threads-api-1.0.0/threads_api/src/threads_api.py` & `threads-api-1.0.1/threads_api/src/threads_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -190,8 +190,159 @@
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
+        return threads
+    
+    async def get_user_profile_replies(self, username: str, user_id: str):
+        url = 'https://www.threads.net/api/graphql'
+        headers = {
+            'authority': 'www.threads.net',
+            'accept': '*/*',
+            'accept-language': 'en-US,en;q=0.9',
+            'content-type': 'application/x-www-form-urlencoded',
+            'origin': 'https://www.threads.net',
+            'referer': 'https://www.threads.net/@zuck/replies',
+            'sec-ch-prefers-color-scheme': 'light',
+            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': 'Windows',
+            'sec-ch-ua-platform-version': '15.0.0',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+            'viewport-width': '897',
+            'x-asbd-id': '129477',
+            'x-fb-friendly-name': 'BarcelonaProfileRepliesTabQuery',
+            'x-fb-lsd': 'tu2kTRKO1aZl9rMKmRuq9u',
+            'x-ig-app-id': '238260118697367',
+        }
+        payload = {
+            'av': '0',
+            '__user': '0',
+            '__a': '1',
+            '__req': '2',
+            '__hs': '19545.HYP:barcelona_web_pkg.2.1..0.0',
+            'dpr': '1',
+            '__ccg': 'EXCELLENT',
+            '__rev': '1007803729',
+            '__s': 'vg5z1u:dyq74i:zgf5h2',
+            '__hsi': '7253172656040290354',
+            '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE465o-cw5Mx62G3i0Bo7O2l0Fwqo31wnEfovwRwlE-U2zxe2Gew9O22362W2K0zK5o4q0GpovU1aUbodEGdwtU2ewbS1LwTwNwLw8O1pwr82gxC',
+            '__csr': 'gA-AlUx9k00lp25u17xS6UvwhUO3gMym8g4Ry82GwwAN0rx11dxW4E4-261wwI7Nw4i0g11l0MgeoJS1KF0Y3MV4m0aj0g8X6G7wt4a0wo-eEU',
+            '__comet_req': '29',
+            'lsd': 'tu2kTRKO1aZl9rMKmRuq9u',
+            'jazoest': '21972',
+            '__spin_r': '1007803729',
+            '__spin_b': 'trunk',
+            '__spin_t': '1688760858',
+            '__jssesw': '1',
+            'fb_api_caller_class': 'RelayModern',
+            'fb_api_req_friendly_name': 'BarcelonaProfileRepliesTabQuery',
+            'variables': '{"userID":"314216"}',
+            'server_timestamps': 'true',
+            'doc_id': '6307072669391286',
+        }
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, headers=headers, data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+
+        threads = data['data']['mediaData']['threads']
+        return threads
+    
+    async def get_post_id_from_url(self, post_url, options=None):
+        url = post_url
+        headers = {
+            "authority": "www.threads.net",
+            "accept": "*/*",
+            "accept-language": "ko",
+            "cache-control": "no-cache",
+            "origin": "https://www.threads.net",
+            "pragma": "no-cache",
+            "referer": post_url,
+            "x-asbd-id": "129477",
+            "x-fb-lsd": self.fbLSDToken,
+            "x-ig-app-id": "238260118697367",
+        }
+
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=headers) as response:
+                text = await response.text()
+
+        text = text.replace('\\s', "").replace('\\n', "")
+        post_id = re.search(r'"props":{"post_id":"(\d+)"},', text)
+        return post_id.group(1)
+
+    async def get_post(self, thread_id: str):
+        url = 'https://www.threads.net/api/graphql'
+        headers = {
+            'authority': 'www.threads.net',
+            'accept': '*/*',
+            'accept-language': 'en-US,en;q=0.9',
+            'content-type': 'application/x-www-form-urlencoded',
+            'origin': 'https://www.threads.net',
+            'referer': f'https://www.threads.net/t/{thread_id}',
+            'sec-ch-prefers-color-scheme': 'light',
+            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
+            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
+            'sec-ch-ua-platform-version': '"15.0.0"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+            'viewport-width': '897',
+            'x-asbd-id': '129477',
+            'x-fb-friendly-name': 'BarcelonaPostPageQuery',
+            'x-fb-lsd': 'bUryVn_O9_i_D9F7WOqEpA',
+            'x-ig-app-id': '238260118697367',
+        }
+
+        payload = {
+        'av': '0',
+        '__user': '0',
+        '__a': '1',
+        '__req': '1',
+        '__hs': '19545.HYP:barcelona_web_pkg.2.1..0.0',
+        'dpr': '1',
+        '__ccg': 'EXCELLENT',
+        '__rev': '1007805316',
+        '__s': 'tygnis:dyq74i:zuyk3e',
+        '__hsi': '7253177132820350526',
+        '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE5ufz81s8hwGwQw9m1YwBgao6C0Mo5W3S7Udo5qfK0EUjwGzE2swwwNwKwHw8Xxm16waCm7-0iK2S3qazo7u0zE2ZwrUdUcobU2cwmo6O0A8pw',
+        '__csr': 'hI_yaUBb9sE01kRm1syToiwHc0sW1czEgDc11wwG0Qk1Hw1Co40tixLOw',
+        '__comet_req': '29',
+        'lsd': 'bUryVn_O9_i_D9F7WOqEpA',
+        'jazoest': '21915',
+        '__spin_r': '1007805316',
+        '__spin_b': 'trunk',
+        '__spin_t': '1688761899',
+        '__jssesw': '1',
+        'fb_api_caller_class': 'RelayModern',
+        'fb_api_req_friendly_name': 'BarcelonaPostPageQuery',
+        'variables': '{"postID":"3141737961795561608"}',
+        'server_timestamps': 'true',
+        'doc_id': '6529829603744567',
+    }
+        
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, headers=headers, data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+
+        threads = data['data']['data']
         return threads
```

