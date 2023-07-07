# Comparing `tmp/pygrab-1.0.0.tar.gz` & `tmp/pygrab-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.0.0.tar", last modified: Tue Jul  4 21:18:28 2023, max compression
+gzip compressed data, was "pygrab-1.1.0.tar", last modified: Fri Jul  7 03:52:02 2023, max compression
```

## Comparing `pygrab-1.0.0.tar` & `pygrab-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.639000 pygrab-1.0.0/
--rw-rw-rw-   0        0        0      262 2023-07-04 21:18:28.630000 pygrab-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.555000 pygrab-1.0.0/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.0.0/pygrab/__init__.py
--rw-rw-rw-   0        0        0    11177 2023-07-04 21:13:44.000000 pygrab-1.0.0/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:18:28.620000 pygrab-1.0.0/pygrab.egg-info/
--rw-rw-rw-   0        0        0      262 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 21:18:28.000000 pygrab-1.0.0/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 21:18:28.637000 pygrab-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-04 21:16:14.000000 pygrab-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:52:02.059000 pygrab-1.1.0/
+-rw-rw-rw-   0        0        0      183 2023-07-07 03:52:02.050000 pygrab-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 03:52:01.983000 pygrab-1.1.0/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.0/pygrab/__init__.py
+-rw-rw-rw-   0        0        0    11748 2023-07-07 03:46:29.000000 pygrab-1.1.0/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:52:02.040000 pygrab-1.1.0/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:52:02.057000 pygrab-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-07 03:48:49.000000 pygrab-1.1.0/setup.py
```

### Comparing `pygrab-1.0.0/pygrab/pygrab.py` & `pygrab-1.1.0/pygrab/pygrab.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     
                 cls.PROXY_LIST.append(lst[i].split(':'))
         raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
 
 
 
 
-def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs) -> str: 
+def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs): 
     """
     Gets the content at the specified URL.
 
     Parameters:
     url (str): The URL to get.
     use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
     retries (int, optional): The number of times to retry the request if it fails. Defaults to 5.
@@ -103,15 +103,28 @@
     """
     local_file_starts = ['./', 'C:', '/'] 
     url_file_starts = ['http', 'ftp:', 'mailto:']
     if any([url.startswith(i) for i in local_file_starts]):
         raise ValueError ("Url must start with http. use get_local() for local requests.")
     elif any([url.startswith(i) for i in url_file_starts]):        
         if enable_js:
-            return __grab_enable_js(url)
+            try:
+                res = __grab_enable_js(url)
+            except RuntimeError as err:
+                if "This event loop is already running" in str(err):
+                    raise RuntimeError("enable_js=True unsupported in jupiter environment.")
+                else:
+                    raise RuntimeError(err)
+            
+            resp = _requests.models.Response()
+            resp.status_code = 200
+            resp.headers = {'header_key': 'NaN'}  # replace with your actual headers
+            resp._content = str(res).encode("utf-8")  # replace with your actual HTML content
+            resp.request = _requests.models.PreparedRequest()
+            return resp
         else:
             session = _requests.Session()
             retry = _requests.packages.urllib3.util.retry.Retry(total=retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
             adapter = _requests.adapters.HTTPAdapter(max_retries=retry)
             session.mount('http://', adapter)
             session.mount('https://', adapter)
             
@@ -124,15 +137,15 @@
                     'https': f'https://{temp_prox[0]}:{temp_prox[1]}'
                 }
                 try:
                     return session.get(url, *args, **kwargs, proxies=proxies)
                 except Exception as err:
                     raise Exception(f'{err}\n\nThere seems to have been an error with the proxy IP. Please note that free proxies may not be reliable.')
 
-            return str(session.get(url, *args, **kwargs).text)
+            return session.get(url, *args, **kwargs)
     raise Exception(f"Invalid url: {url}")
     
 def get_async(urls, use_proxy=False, retries=5, enable_js=False, time_rest=0, *args, **kwargs) -> list:
     """
     Gets multiple URLs asynchronously.
 
     This function sends HTTP requests to a list of URLs in separate threads, allowing for concurrent HTTP requests.
@@ -168,35 +181,32 @@
     return result
 
 def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8'):
     with open(filename, local_read_type, encoding=encoding) as f:
         data = f.read()
     return data
 
-def download(url: str, name:str=None, use_proxy=False, retries=5) -> None:
+def download(url: str, local_filename:str=None, use_proxy=False, retries=5) -> None:
     if '.' not in url:
         raise Exception("Argument 'url' needs a filepath extention")
     
 
-    if name is not None:
-        if '.' not in name:
-            if '.' in url:
-                name += '.' + url.split('.')[-1]
-        elif name.split('.')[-1] != url.split('.')[-1]:
-            raise Exception ("File extentions for 'url' and 'name' must match.")
+    if local_filename is not None:
+        if '.' not in local_filename:
+            raise ValueError("Argument 'local_filename' must have file extention.")
     elif '/' in url:
-        name = url.split('/')[-1]
+        local_filename = url.split('/')[-1]
     else:
-        name=url
+        local_filename=url
         
 
     response = get(url, use_proxy=use_proxy, retries=retries)
 
     if response.status_code == 200:
-        with open(name, 'wb') as f:
+        with open(local_filename, 'wb') as f:
             f.write(response.content)
     else:
         raise Exception(f"Error fetching url. Status code - {response.status_code}")
 
 def download_async(urls:list, names:list=None, use_proxy=False, retries=5, time_rest=0) -> None:
     if names is not None:
         if len(urls) != len(names):
@@ -274,15 +284,15 @@
     ProxyList.update_proxies()
 
 def __grab_thread_wrapper(url:str, payload:list, args, kwargs, use_proxy=False, retries=5, enable_js=False):
     res = get(url, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)
     payload.append(res)
 
 def __grab_enable_js(url):
-    return _asyncio.get_event_loop().run_until_complete(__grab_enable_js_async(url)) 
+    return _asyncio.get_event_loop().run_until_complete(__grab_enable_js_async(url))
 
 async def __grab_enable_js_async(url):
     browser = await _launch()
     page = await browser.newPage()
     await page.goto(url, waitUntil='networkidle0')
     html = await page.content()    
     await browser.close()
```

