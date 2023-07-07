# Comparing `tmp/pygrab-1.1.0.tar.gz` & `tmp/pygrab-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.1.0.tar", last modified: Fri Jul  7 03:52:02 2023, max compression
+gzip compressed data, was "pygrab-1.1.1.tar", last modified: Fri Jul  7 04:44:07 2023, max compression
```

## Comparing `pygrab-1.1.0.tar` & `pygrab-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:52:02.059000 pygrab-1.1.0/
--rw-rw-rw-   0        0        0      183 2023-07-07 03:52:02.050000 pygrab-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 03:52:01.983000 pygrab-1.1.0/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.0/pygrab/__init__.py
--rw-rw-rw-   0        0        0    11748 2023-07-07 03:46:29.000000 pygrab-1.1.0/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:52:02.040000 pygrab-1.1.0/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 03:52:01.000000 pygrab-1.1.0/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 03:52:02.057000 pygrab-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-07 03:48:49.000000 pygrab-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.913000 pygrab-1.1.1/
+-rw-rw-rw-   0        0        0      183 2023-07-07 04:44:07.905000 pygrab-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.840000 pygrab-1.1.1/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.1/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.1/pygrab/proxylist.py
+-rw-rw-rw-   0        0        0    15788 2023-07-07 04:40:22.000000 pygrab-1.1.1/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.895000 pygrab-1.1.1/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 04:44:07.911000 pygrab-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-07 04:43:39.000000 pygrab-1.1.1/setup.py
```

### Comparing `pygrab-1.1.0/pygrab/pygrab.py` & `pygrab-1.1.1/pygrab/pygrab.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,55 @@
-# Author: Anish Kanthamneni
-import requests as _requests
-from pyppeteer import launch as _launch
-from random import choice as _choice
-import asyncio as _asyncio
+"""
+This module implements the primary developer interface for pygrab.
 
-class ProxyList():
-    PROXY_LIST = []
-    
-    @classmethod
-    def is_empty(cls):
-        return cls.PROXY_LIST == []
-    
-    @classmethod
-    def get_random(cls):
-        
-        high_quality = []
-        
-        for ip in cls.PROXY_LIST:
-            if ip[4] == 'Transparent':
-                continue
-            elif int(ip[-1]) < 550:
-                continue
-            high_quality.append(ip)
-        
-        if high_quality != []:
-            x = _choice(high_quality)
-            print (x)
-            print (f'length: {len(cls.PROXY_LIST)}')
-            return x
-        return _choice(cls.PROXY_LIST)
-    
-    @classmethod
-    def update_proxies(cls):
-        while (cls.PROXY_LIST != []): cls.PROXY_LIST.pop(0)
-        cls.gen_proxies()
-    
-    @classmethod
-    async def grab_proxies_async(cls):
-        browser = await _launch()
-        page = await browser.newPage()
-        await page.goto('https://proxyscrape.com/free-proxy-list', waitUntil='networkidle0')
-        html = await page.content()    
-        await browser.close()
-        return html
-    
-    @classmethod
-    def gen_proxies(cls):
-        def parse(row):
-            row = row.split('</td><td>')
-            row[-1] = row[4].split('>')[-1].replace('ms', '')
-            row[4] = row[4].split('<')[0]
-            return row
-        try:
-            raw_html = _asyncio.get_event_loop().run_until_complete(cls.grab_proxies_async())
-            html = raw_html.split('</thead>')[1]
-            html = html.split('<tr><td>')
-            html.pop(0)
-            cls.PROXY_LIST = [parse(i) for i in html]
-            
-        except Exception as err:
-            raise Exception(f'{err}\n\n{raw_html}\n\nThere seems to have been an error with finding a proxy IP. Please note that free proxies may not be reliable.')
+The main responsibilities of the :class:pygrab <pygrab> class revolve 
+predominantly around the developer's perspective. pygrab delegates the 
+majority of its heavy-duty tasks to smaller, specialized auxiliary 
+modules and functions, ensuring an intuitive and seamless experience 
+in handling various types of web requests, including asynchronous tasks, 
+Javascript-enabled sites, and local requests.
 
-    @classmethod
-    def set_proxies(cls, lst):
-        if len(lst) == 0: 
-            cls.PROXY_LIST = []
-            return
-        
-        if type(lst[0]) == list:
-            lst[0], lst[1] = str(lst[0]), str(lst[1])
-            for i in range (len(cls.PROXY_LIST)):
-                if ('.' not in lst[i][0]):
-                    raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
-                cls.PROXY_LIST.append(lst[i])
-        elif type(lst[0]) == str:
-            for i in range (len(cls.PROXY_LIST)):
-                if '://' in lst[0]:
-                    lst[0] = lst[0].split('://')[1]
-                if ('.' not in lst[i] or ':' not in lst[i]):
-                    raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
-                    
-                cls.PROXY_LIST.append(lst[i].split(':'))
-        raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
+"""
 
 
+from proxylist import ProxyList
+import requests as _requests
+from pyppeteer import launch as _launch
+import asyncio as _asyncio
+import time as _time
+
 
 
 def get(url: str, use_proxy=False, retries=5, enable_js=False, *args, **kwargs): 
     """
     Gets the content at the specified URL.
 
     Parameters:
-    url (str): The URL to get.
-    use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
-    retries (int, optional): The number of times to retry the request if it fails. Defaults to 5.
-    encoding (str, optional): The encoding to use when reading the response. Defaults to 'utf-8'.
-    *args: Variable length argument list passed to requests.get.
-    **kwargs: Arbitrary keyword arguments passed to requests.get.
+        url (str): The URL to get.
+        use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
+        retries (int, optional): The number of times to retry the request if it fails. Defaults to 5.
+        encoding (str, optional): The encoding to use when reading the response. Defaults to 'utf-8'.
+        *args: Variable length argument list passed to requests.get.
+        **kwargs: Arbitrary keyword arguments passed to requests.get.
 
     Returns:
-    requests.Response: The response from the server.
+        requests.Response: The response from the server.
+
+    Raises:
+        TypeError: If any of the arguments are not of the desired data type.
     """
+    if not (isinstance(url, str)):
+        raise TypeError("Argument 'url' must be a str")
+    elif not (isinstance(use_proxy, bool)):
+        raise TypeError("Argument 'use_proxy' must be a bool")
+    elif not (isinstance(retries, int)):
+        raise TypeError("Argument 'retries' must be a int")
+    elif not (isinstance(enable_js, bool)):
+        raise TypeError("Argument 'enable_js' must be a bool")
+
     local_file_starts = ['./', 'C:', '/'] 
     url_file_starts = ['http', 'ftp:', 'mailto:']
     if any([url.startswith(i) for i in local_file_starts]):
         raise ValueError ("Url must start with http. use get_local() for local requests.")
     elif any([url.startswith(i) for i in url_file_starts]):        
         if enable_js:
             try:
@@ -157,18 +102,30 @@
         retries (int, optional): The number of times to retry the HTTP request in case of failure. Defaults to 5.
         time_rest (int, optional): The time in seconds to wait between starting each thread. Defaults to 0.
         *args: Variable length argument list to pass to the get function.
         **kwargs: Arbitrary keyword arguments to pass to the get function.
 
     Returns:
         list: A list of responses from the grabbed URLs.
+    
+    Raises:
+        TypeError: If any of the arguments are not of the desired data type.
     """
-    # only import if async functionality is needed
-    import threading as _threading
-    import time as _time
+    if not (isinstance(urls, list)):
+        raise TypeError("Argument 'urls' must be a list")
+    elif not (isinstance(use_proxy, bool)):
+        raise TypeError("Argument 'use_proxy' must be a bool")
+    elif not (isinstance(retries, int)):
+        raise TypeError("Argument 'retries' must be a int")
+    elif not (isinstance(enable_js, bool)):
+        raise TypeError("Argument 'enable_js' must be a bool")
+    elif not (isinstance(time_rest, int) or isinstance(time_rest, float)):
+        raise TypeError("Argument 'time_rest' must be a int or float")
+
+    import threading as _threading # only import if async functionality is needed
     if type(urls) == str:
         return [get(urls, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)]
 
     result = []
     threads = []
     for url in urls:
         threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
@@ -177,21 +134,74 @@
     
     for thread in threads:
         thread.join()
         
     return result
 
 def get_local(filename:str, local_read_type:str='r', encoding:str='utf-8'):
+    """
+    Reads the contens of a file and returns it to the user.
+
+    This function reads the contens of a file and returns it to the user.
+
+    Parameters:
+        filename (str): The file to read from.
+        local_read_type (str, optional): The read type, 'r' or 'rb' for example.
+        encoding (str, optional): Encoding, 'utf-8 or 'ascii' for example.
+
+    Returns:
+        data: The contents of the file
+
+    Raises:
+        TypeError: If any of the arguments are not of the desired data type.
+    """
+        
+    if not (isinstance(filename, str)):
+        raise TypeError("Argument 'filename' must be a str")
+    if not (isinstance(local_read_type, str)):
+        raise TypeError("Argument 'local_read_type' must be a str")
+    if not (isinstance(encoding, str)):
+        raise TypeError("Argument 'encoding' must be a str")
+
+
     with open(filename, local_read_type, encoding=encoding) as f:
         data = f.read()
     return data
 
 def download(url: str, local_filename:str=None, use_proxy=False, retries=5) -> None:
+    """
+    Downloads a file from a given URL and saves it locally.
+
+    This function retrieves a file from a specified URL and saves it to a local directory. The file will be saved with the filename from the URL if no local filename is specified.
+
+    Parameters:
+        url (str): The URL of the file to be downloaded. Must include a file extension.
+        local_filename (str, optional): The name to be used when saving the file locally. If none is provided, the function uses the filename from the URL. Must include a file extension if provided.
+        use_proxy (bool, optional): If set to True, the function will use a proxy server for the download. Defaults to False.
+        retries (int, optional): The number of retry attempts for the download in case of failure. Defaults to 5.
+
+    Returns:
+        None
+
+    Raises:
+        TypeError: If any of the arguments are not of the desired data type.
+        ValueError: If 'url' does not contain a file extension or if there was an error fetching the URL.
+        ValueError: If 'local_filename' is specified but does not contain a file extension.
+    """
+    if not (isinstance(url, str)):
+        raise TypeError("Argument 'url' must be a str")
+    elif not (isinstance(local_filename, str) or local_filename is None):
+        raise TypeError("Argument 'local_filename' must be a str")
+    elif not (isinstance(use_proxy, bool)):
+        raise TypeError("Argument 'use_proxy' must be a bool")
+    elif not (isinstance(retries, int)):
+        raise TypeError("Argument 'retries' must be a int")
+    
     if '.' not in url:
-        raise Exception("Argument 'url' needs a filepath extention")
+        raise ValueError("Argument 'url' needs a filepath extention")
     
 
     if local_filename is not None:
         if '.' not in local_filename:
             raise ValueError("Argument 'local_filename' must have file extention.")
     elif '/' in url:
         local_filename = url.split('/')[-1]
@@ -203,27 +213,59 @@
 
     if response.status_code == 200:
         with open(local_filename, 'wb') as f:
             f.write(response.content)
     else:
         raise Exception(f"Error fetching url. Status code - {response.status_code}")
 
-def download_async(urls:list, names:list=None, use_proxy=False, retries=5, time_rest=0) -> None:
-    if names is not None:
-        if len(urls) != len(names):
-            raise Exception("Lists 'url' and 'name' must be of equal length.")
+def download_async(urls:list, local_filename:list=None, use_proxy=False, retries=5, time_rest=0) -> None:
+    """
+    Executes multiple file downloads asynchronously from a list of given URLs and saves them locally.
+
+    This function uses threading to download multiple files simultaneously. Each file is saved with a filename from the list of local filenames, if provided. If no local filename is provided, the function uses the filename from the corresponding URL.
+
+    Parameters:
+        urls (list of str): The URLs of the files to be downloaded. Each URL must include a file extension.
+        local_filename (list of str, optional): A list of names to be used when saving the files locally. If none is provided, the function uses the filename from each corresponding URL. Each filename must include a file extension if provided. Must be of same length as 'urls' if provided.
+        use_proxy (bool, optional): If set to True, the function will use a proxy server for the downloads. Defaults to False.
+        retries (int, optional): The number of retry attempts for the downloads in case of failure. Defaults to 5.
+        time_rest (int, optional): The amount of time to rest between the start of each download thread. Defaults to 0 seconds.
+
+    Returns:
+        None
+
+    Raises:
+        TypeError: If any of the arguments are not of the desired data type.
+        ValueError: If 'local_filename' is specified but does not match the length of 'urls' or if a URL does not contain a file extension.
+        ValueError: If a 'local_filename' is specified but does not contain a file extension.
+    """
+    if not (isinstance(urls, list)):
+        raise TypeError("Argument 'urls' must be a list")
+    elif not (isinstance(local_filename, list) or local_filename is None):
+        raise TypeError("Argument 'local_filename' must be a list")
+    elif not (isinstance(use_proxy, bool)):
+        raise TypeError("Argument 'use_proxy' must be a bool")
+    elif not (isinstance(retries, int)):
+        raise TypeError("Argument 'retries' must be a int")
+    elif not (isinstance(time_rest, int) or isinstance(time_rest, float)):
+        raise TypeError("Argument 'time_rest' must be a int or float")
+
+
+    if local_filename is not None:
+        if len(urls) != len(local_filename):
+            raise ValueError("Lists 'url' and 'name' must be of equal length.")
     else:
-        names = [None for _ in range(len(urls))]
+        local_filename = [None for _ in range(len(urls))]
 
     # only import if async functionality is needed
     import threading as _threading
     import time as _time
 
     threads = []
-    for url, name in zip(urls, names):
+    for url, name in zip(urls, local_filename):
         threads.append(_threading.Thread(target=download, args=[url, name, use_proxy, retries]))
         threads[-1].start()
         _time.sleep(time_rest)
     
     for thread in threads:
         thread.join()
     
@@ -235,14 +277,28 @@
     local_file_starts = ['./', 'C:', '/'] 
     if any([url.startswith(i) for i in local_file_starts]):
         raise ValueError("use post_local() for creation of local files.")
         
     return _requests.post(url, data=data, json=json, **kwargs)
 
 def post_local(filepath:str, data:str, local_save_type:str="w", encoding:str='utf-8') -> None:
+    """
+    Writes data to a local file.
+
+    This function is used to write or append data to a local file. It can be used in various scenarios such as saving request data, logging, or other local storage needs.
+
+    Parameters:
+        filepath (str): The path to the file where the data will be written. If the file does not exist, it will be created.
+        data (str): The data that will be written to the file.
+        local_save_type (str, optional): The mode in which the file is opened. Defaults to 'w' (write mode), and can also be set to 'a' (append mode) or any other valid file mode.
+        encoding (str, optional): The encoding to be used when opening the file. Defaults to 'utf-8'.
+
+    Returns:
+        None
+    """
     with open(filepath, local_save_type, encoding=encoding) as f:
         f.write(str(data))
 
 def put(url, data=None, **kwargs):
     return _requests.put(url, data=data, **kwargs)
 
 def patch(url, data=None, **kwargs):
```

