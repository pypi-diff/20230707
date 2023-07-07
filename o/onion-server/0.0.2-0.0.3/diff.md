# Comparing `tmp/onion-server-0.0.2.tar.gz` & `tmp/onion-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion-server-0.0.2.tar", last modified: Thu Jul  6 14:23:42 2023, max compression
+gzip compressed data, was "onion-server-0.0.3.tar", last modified: Fri Jul  7 15:28:03 2023, max compression
```

## Comparing `onion-server-0.0.2.tar` & `onion-server-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:23:42.703410 onion-server-0.0.2/
--rwxr-xr-x   0 root         (0) root         (0)      306 2023-07-06 13:46:22.000000 onion-server-0.0.2/CHANGELOG.md
--rwxr-xr-x   0 root         (0) root         (0)     1065 2023-06-13 01:15:27.000000 onion-server-0.0.2/LICENCE.txt
--rwxr-xr-x   0 root         (0) root         (0)       31 2023-06-13 01:16:12.000000 onion-server-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-06 14:23:42.691411 onion-server-0.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1364 2023-07-06 14:19:56.000000 onion-server-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-06 14:21:43.000000 onion-server-0.0.2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:23:42.691411 onion-server-0.0.2/onion_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    16920 2023-07-06 13:46:05.000000 onion-server-0.0.2/onion_server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:23:42.703410 onion-server-0.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1220 2023-07-06 14:20:43.000000 onion-server-0.0.2/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-07 15:28:03.637230 onion-server-0.0.3/
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      448 2023-07-07 15:17:56.000000 onion-server-0.0.3/CHANGELOG.md
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-06-13 01:15:27.000000 onion-server-0.0.3/LICENCE.txt
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)       31 2023-06-13 01:16:12.000000 onion-server-0.0.3/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3095 2023-07-07 15:28:03.637230 onion-server-0.0.3/PKG-INFO
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     2088 2023-07-07 15:25:19.000000 onion-server-0.0.3/README.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      265 2023-07-07 15:16:27.000000 onion-server-0.0.3/__init__.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-07 15:28:03.637230 onion-server-0.0.3/onion_server.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3095 2023-07-07 15:28:00.000000 onion-server-0.0.3/onion_server.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      301 2023-07-07 15:28:01.000000 onion-server-0.0.3/onion_server.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-07 15:28:00.000000 onion-server-0.0.3/onion_server.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       44 2023-07-07 15:28:00.000000 onion-server-0.0.3/onion_server.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-07-07 15:28:00.000000 onion-server-0.0.3/onion_server.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       13 2023-07-07 15:28:00.000000 onion-server-0.0.3/onion_server.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    19206 2023-07-07 15:15:08.000000 onion-server-0.0.3/onion_server.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-07 15:28:03.637230 onion-server-0.0.3/setup.cfg
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1254 2023-07-07 15:20:01.000000 onion-server-0.0.3/setup.py
```

### Comparing `onion-server-0.0.2/LICENCE.txt` & `onion-server-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `onion-server-0.0.2/PKG-INFO` & `onion-server-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onion-server
-Version: 0.0.2
-Summary: Dot-Onion Services Manager Client
+Version: 0.0.3
+Summary: Dot-Onion (domain.onion) DeepWeb and Hidden Services Server Manager
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: tor,hosting,onion,hidden,services,server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -15,35 +15,58 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ## **Onion-Server - Dot-Onion and hidden services manager and client**
 
 ---
 
-Onion-Server provides a client for fast and easy Hidden services management. Helps in controlling services in one session.
+Onion-Server provides a client for fast and easy hidden services management. Used for managing services in one session. Services include (.onion) deep web hosting on a local machine.
 <br>
 
 ### **Installation**
 
 ```bash
-sudo su
 python -m pip install onion-server
 ```
 
-<br>
-
 ### **OS Support**
 
 - Linux
 
+### **Requirements**
+
+onion-server requires tor services. Tor can be download using **apt**
+
+```bash
+$ apt install tor
+```
+
+<br>
+<br>
+
+## **USAGE**
+
 ---
 
+**Running Onion-Server**
+
+```bash
+$ sudo onion
+# or
+$ sudo python -m onion_server
+```
+
+To run onion-server, type **sudo onion** or **sudo python -m onion_server** in the terminal and run.
+
+<br>
 <br>
 
-## **Usage**
+## **COMMANDS**
+
+---
 
 ### **server**
 
 ```bash
 $ server.<command>
 ```
 
@@ -96,35 +119,64 @@
 ```
 
 **online** - set web service online  
 **offline** - set web service offline
 
 <br>
 
+### **config**
+
+```bash
+$ config.<command>
+```
+
+**del** - delete config file  
+**create** - create the config file
+
+<br>
+
 ### **Others**
 
 ```bash
 $ <command>
 ```
 
 **reset** - reset server  
 **scan** - update all running services on the server  
 **status** - display server services status  
+**help** - display help message  
+**update** - update onion-server  
 **exit** - quit server
+
+<br>
+
+---
+
+<br>
+
+> **NOTICE:** In case of any error or information email me. eirasmx@pm.me
 
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 13 JUNE 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
 
 > **0.0.2** -- [ 06 JULY 2023 ]  
 > [ ADDED ]  
-> [+] Config file delete
-> [+] Config file create
-> [+] Server reset
+> [+] Config file delete  
+> [+] Config file create  
+> [+] Server reset  
 > [+] Server restart
 >
 > [ FIXED ]  
 > [+] Hostname unchanged after error
+
+> **0.0.3** -- [ 07 JULY 2023 ]  
+> [ NOTICE ]  
+> [+] Readme Update
+>
+> [ ADDED ]  
+> [+] Help Command  
+> [+] Update Command
```

### Comparing `onion-server-0.0.2/onion_server.egg-info/PKG-INFO` & `onion-server-0.0.3/onion_server.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onion-server
-Version: 0.0.2
-Summary: Dot-Onion Services Manager Client
+Version: 0.0.3
+Summary: Dot-Onion (domain.onion) DeepWeb and Hidden Services Server Manager
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: tor,hosting,onion,hidden,services,server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -15,35 +15,58 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ## **Onion-Server - Dot-Onion and hidden services manager and client**
 
 ---
 
-Onion-Server provides a client for fast and easy Hidden services management. Helps in controlling services in one session.
+Onion-Server provides a client for fast and easy hidden services management. Used for managing services in one session. Services include (.onion) deep web hosting on a local machine.
 <br>
 
 ### **Installation**
 
 ```bash
-sudo su
 python -m pip install onion-server
 ```
 
-<br>
-
 ### **OS Support**
 
 - Linux
 
+### **Requirements**
+
+onion-server requires tor services. Tor can be download using **apt**
+
+```bash
+$ apt install tor
+```
+
+<br>
+<br>
+
+## **USAGE**
+
 ---
 
+**Running Onion-Server**
+
+```bash
+$ sudo onion
+# or
+$ sudo python -m onion_server
+```
+
+To run onion-server, type **sudo onion** or **sudo python -m onion_server** in the terminal and run.
+
+<br>
 <br>
 
-## **Usage**
+## **COMMANDS**
+
+---
 
 ### **server**
 
 ```bash
 $ server.<command>
 ```
 
@@ -96,35 +119,64 @@
 ```
 
 **online** - set web service online  
 **offline** - set web service offline
 
 <br>
 
+### **config**
+
+```bash
+$ config.<command>
+```
+
+**del** - delete config file  
+**create** - create the config file
+
+<br>
+
 ### **Others**
 
 ```bash
 $ <command>
 ```
 
 **reset** - reset server  
 **scan** - update all running services on the server  
 **status** - display server services status  
+**help** - display help message  
+**update** - update onion-server  
 **exit** - quit server
+
+<br>
+
+---
+
+<br>
+
+> **NOTICE:** In case of any error or information email me. eirasmx@pm.me
 
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 13 JUNE 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
 
 > **0.0.2** -- [ 06 JULY 2023 ]  
 > [ ADDED ]  
-> [+] Config file delete
-> [+] Config file create
-> [+] Server reset
+> [+] Config file delete  
+> [+] Config file create  
+> [+] Server reset  
 > [+] Server restart
 >
 > [ FIXED ]  
 > [+] Hostname unchanged after error
+
+> **0.0.3** -- [ 07 JULY 2023 ]  
+> [ NOTICE ]  
+> [+] Readme Update
+>
+> [ ADDED ]  
+> [+] Help Command  
+> [+] Update Command
```

### Comparing `onion-server-0.0.2/onion_server.py` & `onion-server-0.0.3/onion_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -292,25 +292,99 @@
             
         elif action == 'scan':
             update_server()
 
         elif cmd == 'reboot' or cmd == 'restart':
             make_process_stop()
             return 'reboot'
+    
+    def _help():
+        COMMAND_R = f'{Fore.BLUE}<command>{Style.RESET_ALL}'
+        PATH = f'{Fore.BLUE}<path>{Style.RESET_ALL}'
+        RESET = Style.RESET_ALL
+        YELLOW = Fore.YELLOW
+        CLI_MARK = f'{Fore.GREEN + Style.BRIGHT}${Style.RESET_ALL}'
 
+        help_text = f'''
+{Style.BRIGHT}server{Style.RESET_ALL}
+
+{CLI_MARK} {YELLOW}server{Style.RESET_ALL}.{COMMAND_R}
+
+    {YELLOW}start{RESET}    - start server  
+    {YELLOW}stop{RESET}     - stop server  
+    {YELLOW}scan{RESET}     - scan server for unrecorded changes  
+    {YELLOW}reboot{RESET} | {YELLOW}restart{RESET} - restart or reboot server
+
+
+{Style.BRIGHT}tor{Style.RESET_ALL}
+
+{CLI_MARK} {YELLOW}tor{Style.RESET_ALL}.{COMMAND_R}
+
+    {YELLOW}start{RESET}    - start tor service  
+    {YELLOW}stop{RESET}     - stop tor service
+
+
+{Style.BRIGHT}http{Style.RESET_ALL}
+
+{CLI_MARK} {YELLOW}http{Style.RESET_ALL}.{COMMAND_R}
+
+    {YELLOW}start{RESET}    - start http service  
+    {YELLOW}stop{RESET}     - stop http service
+
+
+{Style.BRIGHT}web{Style.RESET_ALL}
+
+{CLI_MARK} {YELLOW}web{Style.RESET_ALL}.{COMMAND_R}
+
+    {YELLOW}info{RESET}     - display web services status  
+    {YELLOW}dir{RESET} [ path ]     - set new web files dir
+
+        {CLI_MARK} {YELLOW}web.dir{Style.RESET_ALL} {PATH}
+
+    {YELLOW}set{RESET} [ status ]   - set web status
+
+        {CLI_MARK} {YELLOW}web.set{Style.RESET_ALL} {COMMAND_R}
+
+    {YELLOW}online{RESET}   - set web service online  
+    {YELLOW}offline{RESET}  - set web service offline
+
+
+{Style.BRIGHT}config{Style.RESET_ALL}
+
+{CLI_MARK} {YELLOW}config{Style.RESET_ALL}.{COMMAND_R}
+
+    {YELLOW}del{RESET}      - delete config file  
+    {YELLOW}create{RESET}   - create the config file
+
+
+{Style.BRIGHT}Others{Style.RESET_ALL}
+
+{CLI_MARK} {COMMAND_R}
+
+    {YELLOW}reset{RESET}    - reset server  
+    {YELLOW}scan{RESET}     - update all running services on the server  
+    {YELLOW}status{RESET}   - display server services status  
+    {YELLOW}help{RESET}     - display this message
+    {YELLOW}update{RESET}   - update onion-server 
+    {YELLOW}exit{RESET}     - quit server'''
+        
+        print(help_text)
 
     def handle_cmd(cmd):
         if cmd == 'exit':
             make_process_stop()
             exit()
             
         elif cmd == 'reset':
             processes = [TOR_SERVICE, HTTP_SERVER]
             for i in range(2):
                 reset(processes[i-1])
+
+        elif cmd == 'update':
+            sp.run('python -m pip install onion-server --upgrade', shell=True)
         
         elif 'config' in cmd:
             command = cmd.split('.')
             action = command[1]
 
             if action == 'del' or action == 'remove' or action == 'delete':
                 sp.getoutput(f'rm -r {DIR_NAME}/config.ini')
@@ -351,14 +425,16 @@
                 if GET['http_server_status'] != False:
                     stop(HTTP_SERVER)
                 else:
                     print(f'\n  [{Fore.YELLOW + Style.BRIGHT} MESSAGE {Style.RESET_ALL}]  http already stopped!')
                     
         elif cmd == 'clear':
             sp.run('clear', shell=True)
+        elif cmd == 'help':
+            _help()
         elif 'server' in cmd:
             server_cmd(cmd)    
         elif cmd == 'status':
             CONFIG = settings.get('MAIN')
             http = CONFIG['http_server_status']
             tor = CONFIG['tor_service_status']
```

### Comparing `onion-server-0.0.2/setup.py` & `onion-server-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Dot-Onion Services Manager Client'
+VERSION = '0.0.3'
+DESCRIPTION = 'Dot-Onion (domain.onion) DeepWeb and Hidden Services Server Manager'
 KEYWORDS = ['tor', 'hosting', 'onion', 'hidden', 'services', 'server']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
     'License :: OSI Approved :: MIT License',
```

