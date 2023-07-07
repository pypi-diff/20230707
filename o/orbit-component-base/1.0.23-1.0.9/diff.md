# Comparing `tmp/orbit_component_base-1.0.23.tar.gz` & `tmp/orbit_component_base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-1.0.23.tar", max compression
+gzip compressed data, was "orbit_component_base-1.0.9.tar", max compression
```

## Comparing `orbit_component_base-1.0.23.tar` & `orbit_component_base-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/README.md
--rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      206 2023-05-30 15:19:46.404293 orbit_component_base-1.0.23/orbit_component_base/cli/cli_base.py
--rw-r--r--   0        0        0     4646 2023-06-30 16:41:46.932914 orbit_component_base-1.0.23/orbit_component_base/cli/group_permissions.py
--rw-r--r--   0        0        0     3163 2023-06-30 17:15:55.107897 orbit_component_base-1.0.23/orbit_component_base/cli/permissions.py
--rw-r--r--   0        0        0     1691 2023-06-10 13:38:38.437638 orbit_component_base-1.0.23/orbit_component_base/cli/sessions.py
--rw-r--r--   0        0        0     2036 2023-07-06 10:49:46.366571 orbit_component_base-1.0.23/orbit_component_base/cli/users.py
--rw-r--r--   0        0        0     5263 2023-07-04 13:24:35.768682 orbit_component_base-1.0.23/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1963 2023-07-06 14:47:23.251031 orbit_component_base-1.0.23/orbit_component_base/schema/OrbitGroupPermissions.py
--rw-r--r--   0        0        0     1613 2023-06-23 14:35:03.647017 orbit_component_base-1.0.23/orbit_component_base/schema/OrbitPermissions.py
--rw-r--r--   0        0        0     1342 2023-06-22 12:00:55.061359 orbit_component_base-1.0.23/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0     1413 2023-07-04 16:43:44.101536 orbit_component_base-1.0.23/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     4716 2023-07-06 11:29:22.423366 orbit_component_base-1.0.23/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6555 2023-06-22 11:38:34.572765 orbit_component_base-1.0.23/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     7350 2023-06-30 15:29:25.195966 orbit_component_base-1.0.23/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1264 2023-07-06 11:29:07.067710 orbit_component_base-1.0.23/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     4248 2023-07-06 15:25:45.092402 orbit_component_base-1.0.23/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.23/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8909 2023-07-06 11:50:45.939350 orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-06-23 14:40:36.048032 orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6554 2023-07-06 11:18:34.457497 orbit_component_base-1.0.23/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2836 2023-07-06 10:31:16.650083 orbit_component_base-1.0.23/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.23/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.23/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.23/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0     6489 2023-06-23 12:53:38.130760 orbit_component_base-1.0.23/orbit_component_base/src/orbit_shells.py
--rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.23/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.23/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2023-07-07 15:11:12.699352 orbit_component_base-1.0.23/orbit_component_base/version.py
--rw-r--r--   0        0        0     1411 2023-07-07 15:11:12.699352 orbit_component_base-1.0.23/pyproject.toml
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 orbit_component_base-1.0.23/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitUsers.py
+-rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py
+-rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       22 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1394 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 orbit_component_base-1.0.9/PKG-INFO
```

### Comparing `orbit_component_base-1.0.23/LICENSE.md` & `orbit_component_base-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from orbit_component_base.src.orbit_orm import BaseTable, BaseCollection
 from orbit_database import SerialiserType, Doc
 from datetime import datetime
-from loguru import logger as log
 
 
 class SessionsTable (BaseTable):
+
     norm_table_name = 'sessions'
     norm_auditing = True
     norm_codec = SerialiserType.UJSON
     norm_ensure = [
         {'index_name': 'by_when'   , 'duplicates': True , 'func': '{when:14.6f}'},
-        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}'},
+        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}', 'force': True},
         {'index_name': 'by_ns'     , 'duplicates': True,  'func': '{ns}'},
     ]
 
     def from_sid (self, sid, transaction=None):
         self.set(self.norm_tb.seek_one('by_sid', Doc({'sid': sid}), txn=transaction))
         return self
 
     @property
     def when (self):
         return datetime.utcfromtimestamp(self._when).strftime('%Y-%m-%d %H:%M:%S')
 
 
 class SessionsCollection (BaseCollection):
+
     table_class = SessionsTable
     table_strip = ['address', 'sid', 'user_id']
-    table_methods = ['get_ids']
-    
+
     def flush (self, nsp):
         limit = Doc({'ns': nsp})
         for result in self.filter(index_name='by_ns', lower=limit, upper=limit):
             result.doc.delete()
         return self
 
     def disconnect (self):
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_app.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 from aiohttp import web
 from aiohttp.web_runner import GracefulExit
 from argparse import ArgumentParser
-from asyncio import sleep, create_task
+from asyncio import sleep
 from loguru import logger as log
 from multiprocessing import freeze_support, set_start_method
 from socketio import AsyncServer
 from ssl import create_default_context, Purpose
-from asyncinotify import Inotify, Mask
-import os
-import sys
+from sys import argv, exit
 #
 # These can be overridden
 #
 from orbit_component_base.src.orbit_router import OrbitRouter
 from orbit_component_base.src.orbit_config import OrbitConfig
 from orbit_component_base.src.orbit_database import OrbitDatabase
 from orbit_component_base.src.orbit_logger import OrbitLogger
@@ -43,65 +41,47 @@
 
     def __init__ (self, app=None):
         if app:
             self.APPLICATION = app
         self._router = None
 
     async def startup (self, app=None):
-        log.debug(f'Orbit Application {self.APPLICATION} Starting up')
         if world.conf.sio_debug:
             self.SERVER_PARAMS['logger'] = self.LOGGER()
         sio = world.sio = AsyncServer(**self.SERVER_PARAMS)
         odb = self.MAINDB().open()
         
         for plugin in Plugins('Plugin'):
             plugin = plugin.Plugin(odb=odb).open().register(sio)
             sio.attach(app, socketio_path=plugin.ns)
             self._router.add_namespace(plugin.NAMESPACE)
-        
-        if world.args.dev:
-            log.debug('Starting file watched, will auto-restart on changes ...')
-            create_task(self.watch_files())
-        
-    async def watch_files (self):
-        with Inotify() as inotify:
-            base = os.environ.get('PYENV_VIRTUAL_ENV') + f'/lib/python{sys.version_info.major}.{sys.version_info.minor}/site-packages'
-            inotify.add_watch(base, Mask.MODIFY | Mask.CREATE | Mask.DELETE | Mask.MOVE)
-            for path, _, _ in os.walk(base):
-                name = path.split('/')[-1]
-                if name.startswith('orbit_'):
-                    inotify.add_watch(path, Mask.MODIFY | Mask.CREATE | Mask.DELETE | Mask.MOVE)
-            async for event in inotify:
-                log.warning('<< Detected a filesystem change, waiting for 3s >>')
-                await sleep(3)
-                log.warning('<< Initiating a program restart >>')
-                os.execv(sys.executable, ['python'] + sys.argv)
 
     async def shutdown(self, app=None):
         await sleep(1)
         raise GracefulExit()
 
     def run (self):
         set_start_method('spawn')
         freeze_support()
+       
+        world.conf = self.CONFIG(self.APPLICATION).open()       
 
-        parser = ArgumentParser()        
+        parser = ArgumentParser()
         for plugin in Plugins('Args'):
             plugin.Args(parser=parser).setup()
-        world.args = parser.parse_args()
-        world.conf = self.CONFIG(self.APPLICATION).open()
-               
+        world.args = parser.parse_args()        
+
         if not world.args.run:
-            odb = self.MAINDB().open(auditing=False)
+            odb = self.MAINDB().open()
             for plugin in Plugins('Plugin'):
                 plugin = plugin.Plugin(odb=odb).open(nql=False)
             for plugin in Plugins('Args'):
                 plugin.Args(parser=parser).open(odb, world.args).process()
             print('Please add "run" if you wish to launch the application')
-            sys.exit(0)
+            exit()
   
         self._router = router = self.ROUTER()
         app = router.application()
         app.on_startup.append(self.startup)
         app.on_shutdown.append(self.shutdown)
         try:
             if world.conf.secure:
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def activate_user(self, user):
         user.update({'active': True, 'code': None}).save()
         return {'ok': True, 'validate': False}
 
     def activate_session (self, user_id, auth, session):
         SessionsTable().from_doc(Doc({
-            # 'user_id'   : user_id,
+            'user_id'   : user_id,
             'when'      : datetime.now().timestamp(),
             'vendor'    : auth.get('vendor', 'unknown'),
             'platform'  : auth.get('platform', 'unknown'),
             'language'  : auth.get('language', 'unknown'),
             'address'   : session['address'],
             'host_id'   : session['host_id'],
             'sid'       : self._sid,
@@ -93,15 +93,15 @@
             user_id = cipher.decrypt(b64decode(secret)).decode()
             user = UsersTable().from_key(host_id)
             if user.isValid:
                 if user._user_id == user_id:
                     if user._active or world.conf.authentication == 'autoenroll':
                         session['activated'] = True
                         session['perm'] = user._perm
-                        # log.debug(f'Save: {self._sid} / {self._ns} => {session}')
+                        log.debug(f'Save: {self._sid} / {self._ns} => {session}')
                         try:
                             await save_session(self._sid, session)
                             self.activate_session(user._user_id, auth, session)
                         except Exception as e:
                             log.error(e)
                             
                         return {'ok': True, 'validate': False}
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_config.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from orbit_component_base.src.orbit_shared import world
 from platform import system
 
 
 class OrbitConfig:
 
     BASE_authentication = 'autoenroll'
-    BASE_name = 'localhost'
-    BASE_network_host = '127.0.0.1'
-    BASE_network_port = '8445'
 
     @property
     def path (self):            return Path(self._conf.get('BASE', 'path')).expanduser()
 
     @property
     def code (self):            return Path(self._conf.get('BASE', 'code')).expanduser()
 
@@ -45,17 +42,14 @@
     @property
     def engineio_debug (self):  return self._conf.getboolean('NETWORK', 'engineio_debug')
 
     @property
     def vite_port (self):       return self._conf.getint('DEV', 'vite_port')
 
     @property
-    def debug (self):           return self._conf.getboolean('DEV', 'debug')
-
-    @property
     def make_keys (self):       return self._conf.get('TOOLS', 'make_keys')
 
     @property
     def database (self):        return self.mkpath('DATA', 'database')
 
     @property
     def tmp (self):             return self.mkpath('DATA', 'tmp')
@@ -122,33 +116,24 @@
         self._path.mkdir(parents=True, exist_ok=True)
         self._conf = ConfigParser()
         self._conf.read(self._file.as_posix())
         for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV']:
             if section not in self._conf.sections():
                 self._conf.add_section(section)
                 self._changed = True
-                
-        if system() == 'Darwin':
-            code_path = f'/Applications/{self._appl}.app/Contents/Resources/'
-        else:
-            if world.args.dev:
-                code_path = f'~/{self._appl}/server'
-            else:
-                code_path = f'/opt/{self._appl}'
-
+        code_path = f'/Applications/{self._appl}.app/Contents/Resources/' if system() == 'Darwin' else f'/opt/{self._appl}'
         self._option('BASE', 'path', f'~/.local/{self._appl}', 'base location for this application')
         self._option('BASE', 'code', code_path, "where the application's code is located")
         self._option('BASE', 'authentication', self.BASE_authentication, 'the default type of authentication (autoenroll/secure)')
-        self._option('SSL', 'name', self.BASE_name, 'the host name (CN) for our SSL certificate')
+        self._option('SSL', 'name', 'localhost', 'the host name (CN) for our SSL certificate')
         self._option('SSL', 'ssl', 'ssl', 'the folder to store SSL files in')
         self._option('SSL', 'secure', 'true', 'whether to use SSL or not')
-        self._option('NETWORK', 'host', self.BASE_network_host, 'the host to expose the server on, use "0.0.0.0" for a local network')
-        self._option('NETWORK', 'port', self.BASE_network_port, "the port to expose the server on")
+        self._option('NETWORK', 'host', '127.0.0.1', 'the host to expose the server on, use "0.0.0.0" for a local network')
+        self._option('NETWORK', 'port', '8445', "the port to expose the server on")
         self._option('DEV', 'vite_port', '5173', 'the port to run "vite" on')
-        self._option('DEV', 'debug', 'false', 'whether debugging is enabled or not')
         self._option('NETWORK', 'sio_debug', 'false', 'SIO debugging')
         self._option('NETWORK', 'engineio_debug', 'false', 'AIO debugging')
         self._option('DATA', 'database', 'orbit_database', 'the path name of the folder to store data in')
         self._option('DATA', 'tmp', 'tmp', 'the path name of a temporary folder')
         self._option('DATA', 'templates', 'templates', 'the path name of the folder to store templates in')
         self._option('DATA', 'web', 'web', 'the path name of the folder to store web assets for in production mode')
         self._option('DATA', 'logs', 'logs', 'the path name of the folder to store logs in')
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_database.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     PATH = 'default'
     FILE = None
     MAX_DATABASE_SIZE = 64
     COLLECTIONS = []
     CONFIG = {
         'map_size': 1024 * 1024 * 1024 * 64,
         'reindex': False,
+        'auditing': True,
         'writemap': True
     }
 
     @property
     def real_path (self):
         return self._floc
     
     def __init__ (self):
         self._path = self.PATH
         self._file = self.FILE
         self._config = self.CONFIG
         self._floc = None
        
-    def open(self, auditing=True):
-        self.CONFIG['auditing'] = auditing
+    def open(self):
         if self._path == 'default':
             path = world.conf.database
         elif path and self._file:
             path = Path(self._path) / self._file
         else:
             raise Exception(f'bad database specification: {self._path} / {self._file}')
         if not path.exists():
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 import functools
-import sys
 from loguru import logger as log
 from asyncio import sleep
 from time import time
 from os import times
-from orbit_component_base.schema.OrbitGroupPermissions import GroupPermissionsCollection
-from orbit_component_base.schema.OrbitUsers import UsersTable
-
-
-permissions = []
 
 
 async def run_and_log(func, args, kwargs):
     try:
         tstart = time()
         cstart = times()
         try:
@@ -40,65 +34,64 @@
                 log.log('RPC', f'{func.__name__} => {params.get("method")} :: real={real_time:.0f}ms, sys={sys_time:.0f}ms usr={usr_time:.0f}ms repeat@{1000/real_time:.0f}/sec')
                 return output
         log.log('RPC', f'{func.__name__} :: real={real_time:.0f}ms, sys={sys_time:.0f}ms usr={usr_time:.0f}ms repeat@{1000/real_time:.0f}/sec') ## :: {new_args}')
         return output
     except Exception as e:
         log.exception(e)
 
-def check_permission (session, nsp, name, args):
-    host_id = session.get('host_id')
-    user = UsersTable().from_key(host_id)
-    if not user.isValid:
-        return False
-    if 'admin' in user._groups:
-        return True
-    exec = args[3] if len(args) > 3 else 'default'
-    for group_id in (user._groups or []):
-        if GroupPermissionsCollection(args[1]).check(group_id, nsp, name, exec):
-            return True
-    log.debug(f'Permission denied, user={user.doc} namespace={nsp} name={name} exec={exec}')
-    return False
-
-def check_own_hostid (session, nsp, name, args):
-    # log.debug(f'[check host id] nsp={nsp} name={name} args={str(args)}')
-    if len(args) > 2 and 'host_id' in args[2]:
-        # log.success(f'Compare: {args[2].get("host_id")} || {session.get("host_id")}')
-        return args[2].get('host_id') == session.get('host_id')
-    return True
 
-def Sentry(fn=None, nsp=None, desc=None):
+def navGuard(func):
+    @functools.wraps(func)
+    async def wrapper(*args, **kwargs):
+        try:
+            retrying = False
+            while True:
+                try:
+                    session = await args[0].get_session(args[1])
+                except KeyError:
+                    log.warning('<< disconnected dead session >>')
+                    return {'ok': False, 'error': 'Server was restarted'}
+                except Exception as e:
+                    log.exception(e)
+                    raise
+                if not session.get('activated', False):
+                    if not retrying:
+                        log.debug(f'<< waiting for authentication >> {args[1]}')
+                        retrying = True
+                    await sleep(0.1)
+                    continue
+                return await run_and_log(func, args, kwargs)
+        except Exception as e:
+            log.exception(e)
+    return wrapper
+
+
+def apiSentry(permissions):
     def navGuard(func):
-        if fn:
-            f = list(sys._current_frames().values())[0]
-            permissions.append((f.f_back.f_globals["__package__"], nsp, func.__name__, desc))
         @functools.wraps(func)
         async def wrapper(*args, **kwargs):
             try:
                 retrying = False
                 while True:
                     try:
                         session = await args[0].get_session(args[1])
+                        if session.get('perm') not in permissions:
+                            error = f'insufficient permissions, wanted: {permissions}, got: {session.get("perm")}'
+                            log.error(error)
+                            return { 'ok': False, 'error': error }
                     except KeyError:
                         log.warning('<< disconnected dead session >>')
                         return {'ok': False, 'error': 'Server was restarted'}
                     except Exception as e:
                         log.exception(e)
                         raise
                     if not session.get('activated', False):
                         if not retrying:
                             log.debug(f'<< waiting for authentication >> {args[1]}')
                             retrying = True
                         await sleep(0.1)
                         continue
-                    try:
-                        if fn and not fn(session, nsp, func.__name__, args):
-                            log.error(error := f'you do not have permission to access this endpoint: {func.__name__}')
-                            return { 'ok': False, 'error': error }
-                        return await run_and_log(func, args, kwargs)
-                    except Exception as e:
-                        log.exception(e)
-                        log.error(f'Args: {str(args)}')
-                        return { 'ok': False, 'error': str(e) }
+                    return await run_and_log(func, args, kwargs)
             except Exception as e:
                 log.exception(e)
         return wrapper
     return navGuard
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,25 @@
         return self
 
     def register(self, method_name, method):
         if not method:
             log.error(f'[programming error] unable to find routine "{method_name}" to publish')
         else:
             self._methods[method_name] = method
-            # log.success(f'Register: {method_name} for {self._ns}')
+            log.success(f'Register: {method_name} for {self._ns}')
 
     def connect(self, sid):
-        # log.error(f'Connect: {sid} => {self._ns}')
         self._sessions[sid] = Session()
         self._sessions[sid].clear()
-        
-        # log.success(f'[connect] {self._sessions.keys()}')
 
     def disconnect(self, sid):
         if sid in self._sessions:
             del self._sessions[sid]
-        # log.success(f'[disconnect] {self._sessions.keys()}')
 
     def call(self, sid, params):
-        # log.success(f'[call] {self._sessions.keys()}')
         session = self._sessions[sid]
         model_name = params.get('model')
         label_name = params.get('label')
         if not model_name:
             return {'ok': False, 'error': f'no model for "{params}"'}
         if not label_name:
             return {'ok': False, 'error': f'no label for "{params}"'}
@@ -120,15 +115,15 @@
                     # 'dref': dref
                 }
             else:
                 if 'ids' in result:
                     # result['dref'] = dref
                     # session.invalid_list[model_name] |= set(old_set) - set(result['ids'])
                     return result
-                # log.debug("#3")
+                log.debug("#3")
                 return {
                     'ok': True,
                     'ids': [],
                     'data': [],
                     # 'dref': dref
                 }
 
@@ -166,15 +161,14 @@
         if docs:
             await self._input_buffer.enqueue(model, docs)
         
     async def update_next (self, model, docs):
         try:
             for sid, session in dict(self._sessions).items():
                 if model not in session.cache_ids:
-                    # log.warning(f'[not cached]')
                     continue
                 for doc in docs:
                     if doc._e != AuditEntry.DELETE.value:
                         session.cache_data[model].discard(doc._o if isinstance(doc, Doc) else doc)
                 for label in dict(session.cache_ids[model]):
                     params = dict(session.cache_params[model][label])
                     old_set = set(session.cache_ids[model].get(label, []))
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from socketio import AsyncNamespace
 from orbit_component_base.src.orbit_nql import NQL
 from orbit_component_base.src.orbit_auth import OrbitAuth
-from orbit_component_base.src.orbit_decorators import Sentry, check_own_hostid, check_permission
+from orbit_component_base.src.orbit_decorators import navGuard
 from orbit_component_base.schema.OrbitSessions import SessionsCollection
 from orbit_component_base.schema.OrbitSessions import SessionsTable
+from orbit_component_base.schema.OrbitVersions import VersionsCollection
 from loguru import logger as log
-from orbit_component_base.src.orbit_shared import world
 
 
 class PluginBase (AsyncNamespace):
 
     NAMESPACE = ''
     COLLECTIONS = []
 
     @property
     def ns (self):
         return f'/{self.NAMESPACE}'
 
     def __init__(self, *args, **kwargs):
-        # log.debug(f'Initialise namespace: {self.ns}')
+        log.debug(f'Initialise namespace: {self.ns}')
         kwargs['namespace'] = self.ns
         self._odb = kwargs.pop('odb')
         self._nql = None
         self._collections = []
         super().__init__(*args, **kwargs)
 
     def open (self, nql=True):
-        if world.conf.debug:
-            log.success(f'Open namespace: {self.ns}')
         if nql:
             self._nql = NQL(self.emit, self.ns).open()
         for cls in self.COLLECTIONS:
             cls().open(self._odb, self._nql)
         if nql:
             SessionsCollection().flush(self.ns)
         return self
@@ -44,39 +42,44 @@
         await self.save_session(sid, {
             'sid': sid,
             'address': environ['aiohttp.request'].transport.get_extra_info('peername')[0]
         })
         self._nql.connect(sid)
 
     async def on_disconnect(self, sid):
+        log.error(f"DISCONNECT={sid}")
         self._nql.disconnect(sid)
         SessionsTable().from_sid(sid).delete()
 
+    async def on_get_version (self, sid, product, version):
+        log.debug(f"NS={self.ns} product={product} version={version}")
+        return await VersionsCollection(sid=sid, session=await self.get_session(sid), ns=self.ns).get_version(product, version)
+
     async def on_auth_hello(self, sid, auth):
         return await OrbitAuth(sid, self.ns).hello(auth, self.get_session, self.save_session)
 
     async def on_auth_validate(self, sid, auth):
-        log.info(f'Validated access for session={sid} to namespace={self.NAMESPACE}')
+        log.info(f'Validate: {sid} / {self.NAMESPACE}')
         return await OrbitAuth(sid, self.ns).validate(auth, self.get_session, self.save_session)
 
     async def on_auth_confirm(self, sid, auth):
         return await OrbitAuth(sid, self.ns).confirm(auth, self.get_session, self.save_session)
 
-    @Sentry(check_own_hostid)
+    @navGuard
     async def on_call_nql(self, sid, params):
         return self._nql.call(sid, params)
 
-    @Sentry()
+    @navGuard
     async def on_drop_nql(self, sid, params):
         return self._nql.drop(sid, params)
 
-    @Sentry()
+    @navGuard
     async def on_dump_nql(self, sid):
         return self._nql.dump ()
-    
+
 
 class ArgsBase:
 
     def __init__ (self, parser=None, args=None):
         self._parser = parser
 
     def setup (self):
```

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_router.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.23/pyproject.toml` & `orbit_component_base-1.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "1.0.23"
+version = "1.0.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
@@ -22,24 +22,22 @@
 documentation = "https://gitlab.com/madpenguin/orbit-component-base"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-base"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-base/-/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <4"
-python-socketio = "^5"
-orbit-database = "^1.0"
-loguru = "^0.7"
-ujson = "^5.7"
-pycryptodome = "^3.18"
-tqdm = "^4"
-aiohttp = "^3"
-rich = "^13"
-asyncinotify = "^4"
+python = "^3.10"
+python-socketio = "^5.8.0"
+orbit-database = "^0.99.91"
+loguru = "^0.7.0"
+ujson = "^5.7.0"
+pycryptodome = "^3.18.0"
+tqdm = "^4.65.0"
+aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.3.1"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orbit_component_base-1.0.23/PKG-INFO` & `orbit_component_base-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 1.0.23
+Version: 1.0.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
-Requires-Python: >=3.10,<4
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: aiohttp (>=3,<4)
-Requires-Dist: asyncinotify (>=4,<5)
-Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: orbit-database (>=1.0,<2.0)
-Requires-Dist: pycryptodome (>=3.18,<4.0)
-Requires-Dist: python-socketio (>=5,<6)
-Requires-Dist: rich (>=13,<14)
-Requires-Dist: tqdm (>=4,<5)
-Requires-Dist: ujson (>=5.7,<6.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: python-socketio (>=5.8.0,<6.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-base
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-base
 Description-Content-Type: text/markdown
 
 # Orbit Component :: Base : Server
 
 #### This is the base compoent for the orbit framework back-end. It's required for all other components and for the framework itself, assuming you want the framework to do something useful.
```

