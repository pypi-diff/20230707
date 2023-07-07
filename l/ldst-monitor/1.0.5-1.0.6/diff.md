# Comparing `tmp/ldst_monitor-1.0.5.tar.gz` & `tmp/ldst_monitor-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldst_monitor-1.0.5.tar", last modified: Fri Jul  7 03:54:56 2023, max compression
+gzip compressed data, was "ldst_monitor-1.0.6.tar", last modified: Fri Jul  7 06:12:08 2023, max compression
```

## Comparing `ldst_monitor-1.0.5.tar` & `ldst_monitor-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.953503 ldst_monitor-1.0.5/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:54:56.953141 ldst_monitor-1.0.5/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      488 2023-07-07 03:52:54.000000 ldst_monitor-1.0.5/pyproject.toml
--rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-07 03:54:56.953641 ldst_monitor-1.0.5/setup.cfg
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.940660 ldst_monitor-1.0.5/src/
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.945811 ldst_monitor-1.0.5/src/ldst_monitor/
--rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.5/src/ldst_monitor/__init__.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     1321 2023-07-06 14:55:29.000000 ldst_monitor-1.0.5/src/ldst_monitor/ding.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)      987 2023-07-06 14:55:51.000000 ldst_monitor-1.0.5/src/ldst_monitor/main.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     2653 2023-07-06 16:01:17.000000 ldst_monitor-1.0.5/src/ldst_monitor/monitor.py
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 03:54:56.951751 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      320 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/SOURCES.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/dependency_links.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)       23 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/requires.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)       13 2023-07-07 03:54:56.000000 ldst_monitor-1.0.5/src/ldst_monitor.egg-info/top_level.txt
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 06:12:08.484212 ldst_monitor-1.0.6/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 06:12:08.483882 ldst_monitor-1.0.6/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      488 2023-07-07 06:07:21.000000 ldst_monitor-1.0.6/pyproject.toml
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-07 06:12:08.484329 ldst_monitor-1.0.6/setup.cfg
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 06:12:08.472573 ldst_monitor-1.0.6/src/
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 06:12:08.476951 ldst_monitor-1.0.6/src/ldst_monitor/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.6/src/ldst_monitor/__init__.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     1344 2023-07-07 05:43:23.000000 ldst_monitor-1.0.6/src/ldst_monitor/ding.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     1649 2023-07-07 06:05:18.000000 ldst_monitor-1.0.6/src/ldst_monitor/main.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     2940 2023-07-07 05:42:23.000000 ldst_monitor-1.0.6/src/ldst_monitor/monitor.py
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-07 06:12:08.482669 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-07 06:12:08.000000 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      332 2023-07-07 06:12:08.000000 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-07 06:12:08.000000 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       23 2023-07-07 06:12:08.000000 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/requires.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       24 2023-07-07 06:12:08.000000 ldst_monitor-1.0.6/src/ldst_monitor.egg-info/top_level.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       41 2023-07-07 05:11:49.000000 ldst_monitor-1.0.6/src/main.py
```

### Comparing `ldst_monitor-1.0.5/src/ldst_monitor/ding.py` & `ldst_monitor-1.0.6/src/ldst_monitor/ding.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         hmac_code = hmac.new(secret_enc, string_to_sign_enc, digestmod=hashlib.sha256).digest()
         sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
         return f'{self.token}&timestamp={timestamp}&sign={sign}'
 
     #
     def send_text(self, message):
         url = self._sign()
+        print(message)
         data = {
             'msgtype': 'markdown',
             "markdown": {
                 "title": "Server notification",
                 "text": message
             }
         }
```

### Comparing `ldst_monitor-1.0.5/src/ldst_monitor/monitor.py` & `ldst_monitor-1.0.6/src/ldst_monitor/monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import os.path
 import subprocess
 import time
 
+import requests
+
 
 class Monitor:
     def __init__(self):
+        self.ip = None
         self.status = {
             "mysql": True,
             "nginx": True,
             "memcached": True,
             "php-fpm-74": True,
         }
+        self.failed_status = {
+
+        }
         self.check = {
             "last_check": 0.0,
             "failed_time": 0.0,
             "failed_send_time": 0.0,
             "success_send_time": 0.0
         }
 
+        self.get_ip()
+
     def mysql(self):
         process = subprocess.run(["pgrep", "-x", "mysqld"], capture_output=True)
         if process.returncode != 0:
             self.status.update({"mysql": False})
             process = subprocess.run(['/etc/init.d/mysqld', 'start'])
             print(process.stdout)
         else:
@@ -70,12 +78,17 @@
         if not os.path.exists(cache):
             os.makedirs(cache)
 
         self.check.update({"last_check": time.time()})
 
         if self.is_failed() and not self.check.get("failed_time"):
             self.check.update({"failed_time": time.time()})
+            self.failed_status.update(self.status.items())
+
+    def get_ip(self):
+        self.ip = requests.get('https://checkip.amazonaws.com').text.strip()
+        print(self.ip)
 
 
 if __name__ == "__main__":
     monitor = Monitor()
     monitor.run()
```

