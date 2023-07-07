# Comparing `tmp/txredisapi-1.4.7.tar.gz` & `tmp/txredisapi-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/txredisapi-1.4.7.tar", last modified: Tue Dec  3 07:50:20 2019, max compression
+gzip compressed data, was "txredisapi-1.4.9.tar", last modified: Sat Mar 18 09:11:20 2023, max compression
```

## Comparing `txredisapi-1.4.7.tar` & `txredisapi-1.4.9.tar`

### file list

```diff
@@ -1,12 +1,40 @@
-drwxr-xr-x   0 ilya      (1000) ilya      (1000)        0 2019-12-03 07:50:20.000000 txredisapi-1.4.7/
--rw-r--r--   0 ilya      (1000) ilya      (1000)      824 2019-12-03 07:50:20.000000 txredisapi-1.4.7/PKG-INFO
--rw-r--r--   0 ilya      (1000) ilya      (1000)    20912 2019-12-03 07:49:43.000000 txredisapi-1.4.7/README.md
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       69 2019-12-03 07:50:20.000000 txredisapi-1.4.7/setup.cfg
--rw-r--r--   0 ilya      (1000) ilya      (1000)     1666 2019-12-03 07:46:36.000000 txredisapi-1.4.7/setup.py
-drwxr-xr-x   0 ilya      (1000) ilya      (1000)        0 2019-12-03 07:50:20.000000 txredisapi-1.4.7/txredisapi.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      824 2019-12-03 07:50:19.000000 txredisapi-1.4.7/txredisapi.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      211 2019-12-03 07:50:19.000000 txredisapi-1.4.7/txredisapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2019-12-03 07:50:19.000000 txredisapi-1.4.7/txredisapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2019-12-03 07:50:19.000000 txredisapi-1.4.7/txredisapi.egg-info/requires.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       11 2019-12-03 07:50:19.000000 txredisapi-1.4.7/txredisapi.egg-info/top_level.txt
--rw-r--r--   0 ilya      (1000) ilya      (1000)    93268 2019-12-03 07:46:40.000000 txredisapi-1.4.7/txredisapi.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-03-18 09:11:20.303538 txredisapi-1.4.9/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    11358 2023-03-02 20:42:50.000000 txredisapi-1.4.9/LICENSE
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    22090 2023-03-18 09:11:20.303538 txredisapi-1.4.9/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    21040 2023-03-18 08:47:38.000000 txredisapi-1.4.9/README.md
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       69 2023-03-18 09:11:20.303538 txredisapi-1.4.9/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     1959 2023-03-18 09:10:55.000000 txredisapi-1.4.9/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-03-18 09:11:20.303538 txredisapi-1.4.9/tests/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     3783 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_basics.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     5885 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_bitops.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     1634 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_blocking.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     1524 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_cancel.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     8333 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_connection.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     1767 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_connection_charset.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     4649 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_hash_ops.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2913 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_hyperloglog.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2236 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_implicit_pipelining.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2302 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_list_ops.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     3619 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_multibulk.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2610 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_number_conversions.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     5181 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_operations.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     5720 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_pipelining.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     3333 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_protocol.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     1045 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_publish.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2575 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_scan.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7443 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_scripting.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    12779 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_sentinel.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     6163 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_sets.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     2319 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_sort.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    12905 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_sortedsets.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     5362 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_subscriber.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     4393 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_transactions.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     3066 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_unix_connection.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     5244 2023-03-02 20:42:50.000000 txredisapi-1.4.9/tests/test_watch.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-03-18 09:11:20.303538 txredisapi-1.4.9/txredisapi.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    22090 2023-03-18 09:11:20.000000 txredisapi-1.4.9/txredisapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      852 2023-03-18 09:11:20.000000 txredisapi-1.4.9/txredisapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-03-18 09:11:20.000000 txredisapi-1.4.9/txredisapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       12 2023-03-18 09:11:20.000000 txredisapi-1.4.9/txredisapi.egg-info/requires.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       11 2023-03-18 09:11:20.000000 txredisapi-1.4.9/txredisapi.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)    94343 2023-03-18 09:10:55.000000 txredisapi-1.4.9/txredisapi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `txredisapi-1.4.7/README.md` & `txredisapi-1.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 - poolsize: how many connections to make. [default: 10]
 - reconnect: auto-reconnect if connection is lost. [default: True]
 - charset: string encoding. Do not decode/encode strings if None.
   [default: utf-8]
 - hosts (for sharded): list of ``host:port`` pairs. [default: None]
 - paths (for sharded): list of ``pathnames``. [default: None]
 - password: password for the redis server. [default: None]
+- ssl_context_factory: Either a boolean indicating wether to use SSL/TLS or a specific `ClientContextFactory`. [default: False]
 
 
 ### Connection Handlers ###
 
 All connection methods return a connection handler object at some point.
 
 Normal connections (not lazy) return a deferred, which is fired with the
```

### Comparing `txredisapi-1.4.7/txredisapi.py` & `txredisapi-1.4.9/txredisapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 import re
 import warnings
 import zlib
 import string
 import hashlib
 import random
 
-from twisted.internet import defer
+from typing import Optional, Union
+from twisted.internet import defer, ssl
 from twisted.internet import protocol
 from twisted.internet import reactor
 from twisted.internet.tcp import Connector
 from twisted.protocols import basic
 from twisted.protocols import policies
 from twisted.python import log
 from twisted.python.failure import Failure
@@ -2376,123 +2377,128 @@
 
     def __init__(self, isLazy=False, handler=ConnectionHandler):
         RedisFactory.__init__(self, None, None, 1, isLazy=isLazy,
                               handler=handler)
 
 
 def makeConnection(host, port, dbid, poolsize, reconnect, isLazy,
-                   charset, password, connectTimeout, replyTimeout,
+                   charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                    convertNumbers):
     uuid = "%s:%d" % (host, port)
     factory = RedisFactory(uuid, dbid, poolsize, isLazy, ConnectionHandler,
                            charset, password, replyTimeout, convertNumbers)
     factory.continueTrying = reconnect
     for x in range(poolsize):
-        reactor.connectTCP(host, port, factory, connectTimeout)
+        if ssl_context_factory is True:
+            ssl_context_factory = ssl.ClientContextFactory()
+        if ssl_context_factory:
+            reactor.connectSSL(host, port, factory, ssl_context_factory, connectTimeout)
+        else:
+            reactor.connectTCP(host, port, factory, connectTimeout)
 
     if isLazy:
         return factory.handler
     else:
         return factory.deferred
 
 
 def makeShardedConnection(hosts, dbid, poolsize, reconnect, isLazy,
-                          charset, password, connectTimeout, replyTimeout,
+                          charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                           convertNumbers):
     err = "Please use a list or tuple of host:port for sharded connections"
     if not isinstance(hosts, (list, tuple)):
         raise ValueError(err)
 
     connections = []
     for item in hosts:
         try:
             host, port = item.split(":")
             port = int(port)
         except:
             raise ValueError(err)
 
         c = makeConnection(host, port, dbid, poolsize, reconnect, isLazy,
-                           charset, password, connectTimeout, replyTimeout,
+                           charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                            convertNumbers)
         connections.append(c)
 
     if isLazy:
         return ShardedConnectionHandler(connections)
     else:
         deferred = defer.DeferredList(connections)
         ShardedConnectionHandler(deferred)
         return deferred
 
 
 def Connection(host="localhost", port=6379, dbid=None, reconnect=True,
-               charset="utf-8", password=None,
+               charset="utf-8", password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                connectTimeout=None, replyTimeout=None, convertNumbers=True):
     return makeConnection(host, port, dbid, 1, reconnect, False,
-                          charset, password, connectTimeout, replyTimeout,
+                          charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                           convertNumbers)
 
 
 def lazyConnection(host="localhost", port=6379, dbid=None, reconnect=True,
-                   charset="utf-8", password=None,
+                   charset="utf-8", password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                    connectTimeout=None, replyTimeout=None, convertNumbers=True):
     return makeConnection(host, port, dbid, 1, reconnect, True,
-                          charset, password, connectTimeout, replyTimeout,
+                          charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                           convertNumbers)
 
 
 def ConnectionPool(host="localhost", port=6379, dbid=None,
-                   poolsize=10, reconnect=True, charset="utf-8", password=None,
+                   poolsize=10, reconnect=True, charset="utf-8", password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                    connectTimeout=None, replyTimeout=None,
                    convertNumbers=True):
     return makeConnection(host, port, dbid, poolsize, reconnect, False,
-                          charset, password, connectTimeout, replyTimeout,
+                          charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                           convertNumbers)
 
 
 def lazyConnectionPool(host="localhost", port=6379, dbid=None,
                        poolsize=10, reconnect=True, charset="utf-8",
-                       password=None, connectTimeout=None, replyTimeout=None,
+                       password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False, connectTimeout=None, replyTimeout=None,
                        convertNumbers=True):
     return makeConnection(host, port, dbid, poolsize, reconnect, True,
-                          charset, password, connectTimeout, replyTimeout,
+                          charset, password, ssl_context_factory, connectTimeout, replyTimeout,
                           convertNumbers)
 
 
 def ShardedConnection(hosts, dbid=None, reconnect=True, charset="utf-8",
-                      password=None, connectTimeout=None, replyTimeout=None,
+                      password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False, connectTimeout=None, replyTimeout=None,
                       convertNumbers=True):
     return makeShardedConnection(hosts, dbid, 1, reconnect, False,
-                                 charset, password, connectTimeout,
+                                 charset, password, ssl_context_factory, connectTimeout,
                                  replyTimeout, convertNumbers)
 
 
 def lazyShardedConnection(hosts, dbid=None, reconnect=True, charset="utf-8",
-                          password=None,
+                          password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                           connectTimeout=None, replyTimeout=None,
                           convertNumbers=True):
     return makeShardedConnection(hosts, dbid, 1, reconnect, True,
-                                 charset, password, connectTimeout,
+                                 charset, password, ssl_context_factory, connectTimeout,
                                  replyTimeout, convertNumbers)
 
 
 def ShardedConnectionPool(hosts, dbid=None, poolsize=10, reconnect=True,
-                          charset="utf-8", password=None,
+                          charset="utf-8", password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                           connectTimeout=None, replyTimeout=None,
                           convertNumbers=True):
     return makeShardedConnection(hosts, dbid, poolsize, reconnect, False,
-                                 charset, password, connectTimeout,
+                                 charset, password, ssl_context_factory, connectTimeout,
                                  replyTimeout, convertNumbers)
 
 
 def lazyShardedConnectionPool(hosts, dbid=None, poolsize=10, reconnect=True,
-                              charset="utf-8", password=None,
+                              charset="utf-8", password=None, ssl_context_factory: Union[ssl.ClientContextFactory, bool]=False,
                               connectTimeout=None, replyTimeout=None,
                               convertNumbers=True):
     return makeShardedConnection(hosts, dbid, poolsize, reconnect, True,
-                                 charset, password, connectTimeout,
+                                 charset, password, ssl_context_factory, connectTimeout,
                                  replyTimeout, convertNumbers)
 
 
 def makeUnixConnection(path, dbid, poolsize, reconnect, isLazy,
                        charset, password, connectTimeout, replyTimeout,
                        convertNumbers):
     factory = RedisFactory(path, dbid, poolsize, isLazy, UnixConnectionHandler,
@@ -2790,20 +2796,20 @@
         factory = factory_class(sentinel_manager=self, service_name=service_name,
                                 is_master=False, uuid=None, dbid=dbid,
                                 poolsize=poolsize, **connection_kwargs)
         return self._connect_factory_and_return_handler(factory, poolsize)
 
 
 __all__ = [
-    Connection, lazyConnection,
-    ConnectionPool, lazyConnectionPool,
-    ShardedConnection, lazyShardedConnection,
-    ShardedConnectionPool, lazyShardedConnectionPool,
-    UnixConnection, lazyUnixConnection,
-    UnixConnectionPool, lazyUnixConnectionPool,
-    ShardedUnixConnection, lazyShardedUnixConnection,
-    ShardedUnixConnectionPool, lazyShardedUnixConnectionPool,
-    Sentinel, MasterNotFoundError
+    "Connection", "lazyConnection",
+    "ConnectionPool", "lazyConnectionPool",
+    "ShardedConnection", "lazyShardedConnection",
+    "ShardedConnectionPool", "lazyShardedConnectionPool",
+    "UnixConnection", "lazyUnixConnection",
+    "UnixConnectionPool", "lazyUnixConnectionPool",
+    "ShardedUnixConnection", "lazyShardedUnixConnection",
+    "ShardedUnixConnectionPool", "lazyShardedUnixConnectionPool",
+    "Sentinel", "MasterNotFoundError"
 ]
 
 __author__ = "Alexandre Fiori"
-__version__ = version = "1.4.7"
+__version__ = version = "1.4.9"
```

