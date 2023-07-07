# Comparing `tmp/ectool-1.1.1.tar.gz` & `tmp/ectool-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.1.tar", last modified: Fri Jul  7 07:21:03 2023, max compression
+gzip compressed data, was "ectool-1.1.2.tar", last modified: Fri Jul  7 12:46:39 2023, max compression
```

## Comparing `ectool-1.1.1.tar` & `ectool-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.383125 ectool-1.1.1/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2018 2023-07-07 07:21:03.383125 ectool-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-07-07 07:20:11.000000 ectool-1.1.1/README.md
--rw-rw-rw-   0        0        0      113 2023-07-07 07:21:03.384125 ectool-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     7947 2023-07-07 07:18:53.000000 ectool-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.360127 ectool-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.374126 ectool-1.1.1/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.1/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15521 2023-07-07 06:53:51.000000 ectool-1.1.1/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.1/src/ectool/ecag.py
--rw-rw-rw-   0        0        0     4947 2023-07-07 07:19:15.000000 ectool-1.1.1/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.1/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.1/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3790 2023-07-07 06:32:49.000000 ectool-1.1.1/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.382125 ectool-1.1.1/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.693385 ectool-1.1.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2023 2023-07-07 12:46:39.694386 ectool-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2023-07-07 12:05:42.000000 ectool-1.1.2/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-07 12:46:39.694386 ectool-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-07 12:36:57.000000 ectool-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.672386 ectool-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.685387 ectool-1.1.2/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.2/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15985 2023-07-07 10:38:19.000000 ectool-1.1.2/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.2/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     5048 2023-07-07 12:41:03.000000 ectool-1.1.2/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.2/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.2/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3896 2023-07-07 12:43:56.000000 ectool-1.1.2/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:46:39.692387 ectool-1.1.2/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 12:46:39.000000 ectool-1.1.2/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.1/LICENSE` & `ectool-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.1/PKG-INFO` & `ectool-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -35,18 +35,18 @@
 2. EC718, EC616的刷机
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
-# 无镜像,或者系统默认镜像
-pip install -U ectool
 # 清华镜像
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+# 无镜像,或者系统默认镜像
+pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
@@ -59,12 +59,12 @@
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 支持只刷AP
 
 ## 参考链接
 
 * 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
-* beanio走的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
+* beanio做的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
 
 ## 开源协议
 
 MIT
```

### Comparing `ectool-1.1.1/README.md` & `ectool-1.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 2. EC718, EC616的刷机
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
-# 无镜像,或者系统默认镜像
-pip install -U ectool
 # 清华镜像
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+# 无镜像,或者系统默认镜像
+pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
@@ -33,12 +33,12 @@
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 支持只刷AP
 
 ## 参考链接
 
 * 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
-* beanio走的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
+* beanio做的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
 
 ## 开源协议
 
 MIT
```

### Comparing `ectool-1.1.1/setup.py` & `ectool-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.1.1",  # Required
+    version="1.1.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.1.1/src/ectool/ecaction.py` & `ectool-1.1.2/src/ectool/ecaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
 
 import os, struct, sys, json, shutil, logging, hashlib, time
 from serial import Serial
 import serial.tools.list_ports
-import zlib
+import zlib, platform
 
 from ectool.ecstruct import *
 from ectool.ecconst import *
 
 COM_DEBUG = False
 COM_DEBUG_FILE = False
 
+is_win32 = platform.platform().upper() == "WINDOWS"
+
 def com_write(burncom, data) :
     if COM_DEBUG :
         logging.debug(" == COM WRITE: " + data.hex().upper())
     if COM_DEBUG_FILE :
         with open("COM.txt", "a+") as f :
             f.write("-->({0}) {1}\n".format(len(data), data.hex().upper()))
-    burncom.write(data)
+    if is_win32 or len(data) <= 64 :
+        burncom.write(data)
+    else :
+        remain = len(data)
+        offset = 0
+        while remain > 0 :
+            if remain > 64 :
+                burncom.write(data[offset:offset+64])
+                offset += 64
+                remain -= 64
+                time.sleep(0.001)
+            else :
+                burncom.write(data[offset:])
+                break
 
 def com_read(burncom, slen) :
     if slen < 1 :
         return None
     recv = burncom.read(slen)
     if COM_DEBUG :
         if recv :
```

### Comparing `ectool-1.1.1/src/ectool/ecag.py` & `ectool-1.1.2/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.1/src/ectool/eccli.py` & `ectool-1.1.2/src/ectool/eccli.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logger = None
 
 def ecburn_auto_select() :
     for item in serial.tools.list_ports.comports():
         if not item.pid or not item.location :
             continue
         if item.vid == 0x17D1 and item.pid == 0x0001 :
-            return item.name
+            return item.device
     return None
 
 def cli_burn() :
     if not ecargs.file :
         logger.error("require -f/--file !!!")
         sys.exit(3)
     import ectool.unpkg as unpkg
@@ -34,26 +34,27 @@
     if not ecargs.port or ecargs.port == "auto" :
         ecargs.port = None
         logger.info("Searching for USB Boot COM, max wait 120s")
         logger.info("Pls Press BOOT button and poweron/reset the module/chip")
         for i in range(1200) :
             COM = ecburn_auto_select()
             if COM :
-                logger.info("Found " + COM)
+                logger.info("Found " + str(COM))
                 ecargs.port = COM
                 break
             time.sleep(0.1)
         if ecargs.port == None :
             logger.error("timeout for searching, exit")
             sys.exit(2)
             return
     logger.info("Select " + ecargs.port)
     COM = ecargs.port
 
-    burncom = serial.Serial(COM, baudrate=921600, timeout=1)
+    # burncom = serial.Serial(COM, baudrate=921600, exclusive=None, timeout=1, xonxoff=False, rtscts=False, dsrdtr=False)
+    burncom = serial.Serial(COM, baudrate=921600)
     burncom.dtr = 1
 
     logging.info("Go   Sync")
     if 0 != burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_DLBOOT, 2) :
         return -1
     logging.info("Done Sync")
     
@@ -104,16 +105,16 @@
     parser = argparse.ArgumentParser(description='A tool for EC modules, like EC618')
     parser.add_argument("action", choices=["burn", "unpack"], help="main action to perform")
     parser.add_argument("--file", "-f", help="file path")
     parser.add_argument("--burn_addr",  help="burn bin file to addr")
     parser.add_argument("--img_type", "-t", choices=["BL", "CP", "AP", "FF"], help="image type for bin file")
     parser.add_argument("--sysreset", help="reset the chip after burn success", const=True, nargs="?")
     parser.add_argument("--debug", "-d", const=True, nargs="?", help="debug mode")
-    parser.add_argument("--port", "-p", default="auto", nargs=1, help="COM port or path, like COM49, default is auto search")
-    parser.add_argument("--outdir", "-o", default="tmp", nargs=1, help="output dir for actoion like unpack/diff")
+    parser.add_argument("--port", "-p", default="auto", help="COM port or path, like COM49, default is auto search")
+    parser.add_argument("--outdir", "-o", default="tmp", help="output dir for actoion like unpack/diff")
     parser.add_argument("--allow-upload", const=True, nargs="?", help="diff action require upload binpkg/soc to remote server, add this option means you agree it")
     ecargs = parser.parse_args()
     if len(sys.argv) == 1 or not ecargs.action :
         parser.print_help()
         return
     if ecargs.debug :
         logging.basicConfig(level=logging.DEBUG)
```

### Comparing `ectool-1.1.1/src/ectool/ecconst.py` & `ectool-1.1.2/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.1/src/ectool/ecstruct.py` & `ectool-1.1.2/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.1/src/ectool/unpkg.py` & `ectool-1.1.2/src/ectool/unpkg.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # logging.basicConfig(level=logging.DEBUG)
 
 def binpkg_unpack(path_or_data, outpath_dir=None, ram=False, debug=False) :
     # logging.info("binpkg " + binpkg_path)
     # logging.info("output " + outpath_dir)
     if outpath_dir and not os.path.exists(outpath_dir) :
         os.makedirs(outpath_dir)
+    if ram :
+        outpath_dir = None
     jdata = {}
     if path_or_data.__class__.__name__ == "bytes" :
         fdata = path_or_data
     else:
         if str(path_or_data).endswith(".binpkg") :
             with open(path_or_data, "rb") as f :
                 fdata = f.read()
@@ -39,14 +41,16 @@
                                 f.write(tmpdata)
                         if ram :
                             jdata["script"]["data"] = tmpdata
                     elif str(fname) == "info.json" :
                         info_json = json.load(bio)
             if info_json and "script" in jdata :
                 jdata["script"]["burn_addr"] = int(info_json["download"]["script_addr"], 16)
+        else:
+            raise Exception("unkown file type")
     fsize = len(fdata)
 
     # 首先, 解析头部数据
     foffset = 0
     fhead = fdata[:52] 
     foffset += 52
     # 然后逐个文件解析出来
```

### Comparing `ectool-1.1.1/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.2/src/ectool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -35,18 +35,18 @@
 2. EC718, EC616的刷机
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
-# 无镜像,或者系统默认镜像
-pip install -U ectool
 # 清华镜像
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
+# 无镜像,或者系统默认镜像
+pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
@@ -59,12 +59,12 @@
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 支持只刷AP
 
 ## 参考链接
 
 * 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
-* beanio走的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
+* beanio做的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
 
 ## 开源协议
 
 MIT
```

