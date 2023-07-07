# Comparing `tmp/viper_lib-0.5.6.tar.gz` & `tmp/viper_lib-0.5.7.tar.gz`

## Comparing `viper_lib-0.5.6.tar` & `viper_lib-0.5.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper.pth
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 viper_lib-0.5.6/token.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/__init__.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/better_threading.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/exceptions.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/format.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/frozendict.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/interactive.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/pickle_utils.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/warnings.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/abc/__init__.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/abc/connection.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/abc/flux.py
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/abc/io.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/building/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/building/module_tools.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/compress/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/compress/flux.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/debugging/__init__.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/debugging/chrono.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/debugging/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/meta/__init__.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/meta/decorators.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/meta/iterable.py
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/meta/procedural.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.6/Viper/meta/utils.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.6/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.6/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper.pth
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 viper_lib-0.5.7/token.txt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/__init__.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/better_threading.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/exceptions.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/format.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/frozendict.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/interactive.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/pickle_utils.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/warnings.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/abc/__init__.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/abc/connection.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/abc/flux.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/abc/io.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/building/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/building/module_tools.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/compress/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/compress/flux.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/debugging/__init__.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/debugging/chrono.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/debugging/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/meta/__init__.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/meta/decorators.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/meta/iterable.py
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/meta/procedural.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.7/Viper/meta/utils.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.7/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.7/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.7/PKG-INFO
```

### Comparing `viper_lib-0.5.6/Viper/better_threading.py` & `viper_lib-0.5.7/Viper/better_threading.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/format.py` & `viper_lib-0.5.7/Viper/format.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/frozendict.py` & `viper_lib-0.5.7/Viper/frozendict.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/interactive.py` & `viper_lib-0.5.7/Viper/interactive.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/pickle_utils.py` & `viper_lib-0.5.7/Viper/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/warnings.py` & `viper_lib-0.5.7/Viper/warnings.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/abc/connection.py` & `viper_lib-0.5.7/Viper/abc/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -151,21 +151,14 @@
         Sends all of data to the other side of the connection. Blocks if necessary.
         If given, will start sending the message from offset instead of the beginning of the buffer.
         If given, will send at most size bytes (sends all bytes available otherwise).
         Raises ConnectionError on failure.
         """
         raise NotImplementedError()
     
-    @abstractmethod
-    async def asend(self, data : bytes | bytearray | memoryview, offset : int = 0, size : Optional[int] = None, /):
-        """
-        Asynchronous version of send.
-        """
-        raise NotImplementedError()
-
 
 
 
 
 class Receiver(ConnectionBase):
 
     """
@@ -176,66 +169,38 @@
     def recv(self) -> bytes:
         """
         Receives a message of bytes from the other side. Blocks until the next message arrives.
         The size of the message is the size of the buffer passed to send() by the other side.
         Raises ConnectionError on failure.
         """
         raise NotImplementedError()
-    
-    @abstractmethod
-    async def arecv(self) -> bytes:
-        """
-        Asynchronous version of recv.
-        """
-        raise NotImplementedError()
-    
+        
     @abstractmethod
     def recv_into(self, buffer : bytearray | memoryview, offset : int = 0, /) -> int:
         """
         Receives the next message in the given buffer and returns the size of the message.
         If given, will only start writing at offset position in the buffer.
         If the buffer doesn't have enough space to write the message, raises BufferTooSmall. An empty bytearray can also be given, and will be allocated with the corresponding size.
         """
         raise NotImplementedError()
     
     @abstractmethod
-    async def arecv_into(self, buffer : bytearray | memoryview, offset : int = 0, /) -> int:
-        """
-        Asynchronous version of recv_into.
-        """
-        raise NotImplementedError()
-    
-    @abstractmethod
     def poll(self, timeout : float = 0.0, /) -> bool:
         """
         Waits at most timeout and returns True when a message has been received. Returns False if the timeout has been reached and no message was received.
         By default, the timeout is 0. You can set an infinite timeout.
         """
         raise NotImplementedError()
     
-    @abstractmethod
-    async def apoll(self, timeout : float = 0.0, /) -> bool:
-        """
-        Asynchronous version of poll.
-        """
-        raise NotImplementedError()
-
     def __iter__(self) -> Iterator[bytes]:
         """
         Iterates over all the messages received.
         """
         while not self.closed:
             yield self.recv()
-    
-    async def __aiter__(self) -> AsyncIterator[bytes]:
-        """
-        Asynchronously iterates over all the messages received.
-        """
-        while not self.closed:
-            yield await self.arecv()
 
 
 
 
 
 class Connection(Sender, Receiver):
```

### Comparing `viper_lib-0.5.6/Viper/abc/flux.py` & `viper_lib-0.5.7/Viper/abc/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/abc/io.py` & `viper_lib-0.5.7/Viper/abc/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,30 +171,14 @@
         """
         Implements iter(self). Yields successive lines.
         """
         line = True
         while line:
             line = self.readline()
             yield line
-    
-    @abstractmethod
-    async def aread(self, size : int = -1, /) -> bytes:
-        """
-        Asynchronous version of read.
-        Should wait only if read would block.
-        Should also handle its own loop is necessary. (See async_utils.SelectorLoop/ProactorLoop for more info)
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    async def areadinto(self, buffer : bytearray | memoryview, /) -> int:
-        """
-        Same as aread, but reads data into pre-allocated buffer (of a given size) and returns the number of bytes read.
-        """
-        raise NotImplementedError()
 
 
 
 
 
 class BytesWriter(BytesIOBase):
     
@@ -256,23 +240,14 @@
                 raise TypeError("Expected iterable of bytes, bytearray or memoriview, got " + repr(type(line).__name__))
             ni = self.write(line)
             n += ni
             if ni < len(line):
                 break
         return n
     
-    @abstractmethod
-    async def awrite(self, data : bytes | bytearray | memoryview, /) -> int:
-        """
-        Asynchronous version of write.
-        Should wait only if write would block.
-        Should also handle its own loop is necessary. (See async_utils.SelectorLoop/ProactorLoop for more info)
-        """
-        raise NotImplementedError()
-
 
 
 
 
 class BytesIO(BytesReader, BytesWriter):
 
     """
```

### Comparing `viper_lib-0.5.6/Viper/building/module_tools.py` & `viper_lib-0.5.7/Viper/building/module_tools.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/compress/flux.py` & `viper_lib-0.5.7/Viper/compress/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/debugging/chrono.py` & `viper_lib-0.5.7/Viper/debugging/chrono.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/debugging/utils.py` & `viper_lib-0.5.7/Viper/debugging/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/meta/decorators.py` & `viper_lib-0.5.7/Viper/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/meta/iterable.py` & `viper_lib-0.5.7/Viper/meta/iterable.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/meta/procedural.py` & `viper_lib-0.5.7/Viper/meta/procedural.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/Viper/meta/utils.py` & `viper_lib-0.5.7/Viper/meta/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/.gitignore` & `viper_lib-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/LICENSE` & `viper_lib-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/README.md` & `viper_lib-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.6/pyproject.toml` & `viper_lib-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "viper_lib"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin.n7@gmail.com" },
 ]
 description = "A Python library full of useful Python tools."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `viper_lib-0.5.6/PKG-INFO` & `viper_lib-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viper_lib
-Version: 0.5.6
+Version: 0.5.7
 Summary: A Python library full of useful Python tools.
 Project-URL: Repository, https://github.com/MrVoustache/Viper
 Project-URL: Bug Tracker, https://github.com/MrVoustache/Viper/issues
 Author-email: Vincent Raulin <vincent.raulin.n7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Vincent Raulin
```

