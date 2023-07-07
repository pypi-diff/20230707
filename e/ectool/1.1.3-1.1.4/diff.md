# Comparing `tmp/ectool-1.1.3.tar.gz` & `tmp/ectool-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.3.tar", last modified: Fri Jul  7 13:09:54 2023, max compression
+gzip compressed data, was "ectool-1.1.4.tar", last modified: Fri Jul  7 14:48:04 2023, max compression
```

## Comparing `ectool-1.1.3.tar` & `ectool-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.592749 ectool-1.1.3/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     2023 2023-07-07 13:09:54.592749 ectool-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-07-07 12:05:42.000000 ectool-1.1.3/README.md
--rw-rw-rw-   0        0        0      113 2023-07-07 13:09:54.593750 ectool-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     7947 2023-07-07 13:08:09.000000 ectool-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.574748 ectool-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.585750 ectool-1.1.3/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.3/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15985 2023-07-07 10:38:19.000000 ectool-1.1.3/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.3/src/ectool/ecag.py
--rw-rw-rw-   0        0        0     5142 2023-07-07 13:07:09.000000 ectool-1.1.3/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.3/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.3/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3896 2023-07-07 12:43:56.000000 ectool-1.1.3/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:09:54.591749 ectool-1.1.3/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 13:09:54.000000 ectool-1.1.3/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.573512 ectool-1.1.4/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2293 2023-07-07 14:48:04.574509 ectool-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2023-07-07 14:04:47.000000 ectool-1.1.4/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-07 14:48:04.574509 ectool-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-07 14:46:57.000000 ectool-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.553510 ectool-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.566510 ectool-1.1.4/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.4/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15990 2023-07-07 14:41:24.000000 ectool-1.1.4/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.4/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     5148 2023-07-07 14:45:41.000000 ectool-1.1.4/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.4/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.4/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3912 2023-07-07 14:36:13.000000 ectool-1.1.4/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.572509 ectool-1.1.4/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2293 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.3/LICENSE` & `ectool-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.3/PKG-INFO` & `ectool-1.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -20,23 +20,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
- # 移芯工具箱
+# 移芯工具箱
 
-已支持:
-1. EC618的刷机
-2. binpkg格式解包
-
-将要支持
-1. binpkg格式的打包
-2. EC718, EC616的刷机
+支持移芯方案的刷机, 解包, windows/linux/macos 可用
+
+当前支持EC618系列, 例如Air780E/Air700E等模块
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
 # 清华镜像
@@ -48,21 +44,31 @@
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
 
+更多参数执行 `ectool -h` 获取说明
+
 ## TODO List
 
-* [ ] 完整的注释
-* [ ] 测试Linux下的兼容性
+* [x] EC618使用USB刷机
+* [x] binpkg解包
+* [x] 测试Linux下的兼容性
+* [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 支持只刷AP
+* [ ] 完整的注释
+* [ ] SoC日志解析
+
+## Linux刷机过程展示
+
+[![asciicast](https://asciinema.org/a/595464.svg)](https://asciinema.org/a/595464)
 
 ## 参考链接
 
 * 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
 * beanio做的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
 
 ## 开源协议
```

### Comparing `ectool-1.1.3/setup.py` & `ectool-1.1.4/setup.py`

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
-    version="1.1.3",  # Required
+    version="1.1.4",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.1.3/src/ectool/ecaction.py` & `ectool-1.1.4/src/ectool/ecaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ectool.ecstruct import *
 from ectool.ecconst import *
 
 COM_DEBUG = False
 COM_DEBUG_FILE = False
 
-is_win32 = platform.platform().upper() == "WINDOWS"
+is_win32 = platform.platform().upper().startswith("WIN")
 
 def com_write(burncom, data) :
     if COM_DEBUG :
         logging.debug(" == COM WRITE: " + data.hex().upper())
     if COM_DEBUG_FILE :
         with open("COM.txt", "a+") as f :
             f.write("-->({0}) {1}\n".format(len(data), data.hex().upper()))
```

### Comparing `ectool-1.1.3/src/ectool/ecag.py` & `ectool-1.1.4/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.3/src/ectool/eccli.py` & `ectool-1.1.4/src/ectool/eccli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             logger.error("timeout for searching, exit")
             sys.exit(2)
             return
     logger.info("Select " + ecargs.port)
     COM = ecargs.port
 
     # burncom = serial.Serial(COM, baudrate=921600, exclusive=None, timeout=1, xonxoff=False, rtscts=False, dsrdtr=False)
-    burncom = serial.Serial(COM, baudrate=921600, timeout=1)
+    burncom = serial.Serial(COM, baudrate=921600, timeout=0.8)
     burncom.dtr = 1
-    burncom.timeout = 1
+    # burncom.timeout = 0.1
 
     logging.info("Go   Sync")
     if 0 != burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_DLBOOT, 2) :
         return -1
     logging.info("Done Sync")
     
     logging.info("Go   AgentBoot download")
```

### Comparing `ectool-1.1.3/src/ectool/ecconst.py` & `ectool-1.1.4/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.3/src/ectool/ecstruct.py` & `ectool-1.1.4/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.3/src/ectool/unpkg.py` & `ectool-1.1.4/src/ectool/unpkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         if img_type == "AP" :
             jdata[name]["burn_addr"] = 0x24000
         if ram :
             jdata[name]["data"] = tmpdata
     if outpath_dir :
         with open(os.path.join(outpath_dir, "image_info.json"), "w") as f :
             json.dump(jdata, f, indent=2)
-    if debug :
+    if outpath_dir and debug :
         print(json.dumps(jdata, indent=2))
     return jdata
 
 if __name__ == "__main__":
     if len(sys.argv) == 3 :
         binpkg_unpack(sys.argv[1], sys.argv[2], False, True)
     else :
```

### Comparing `ectool-1.1.3/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.4/src/ectool.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -20,23 +20,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
- # 移芯工具箱
+# 移芯工具箱
 
-已支持:
-1. EC618的刷机
-2. binpkg格式解包
-
-将要支持
-1. binpkg格式的打包
-2. EC718, EC616的刷机
+支持移芯方案的刷机, 解包, windows/linux/macos 可用
+
+当前支持EC618系列, 例如Air780E/Air700E等模块
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
 # 清华镜像
@@ -48,21 +44,31 @@
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
 
+更多参数执行 `ectool -h` 获取说明
+
 ## TODO List
 
-* [ ] 完整的注释
-* [ ] 测试Linux下的兼容性
+* [x] EC618使用USB刷机
+* [x] binpkg解包
+* [x] 测试Linux下的兼容性
+* [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 支持只刷AP
+* [ ] 完整的注释
+* [ ] SoC日志解析
+
+## Linux刷机过程展示
+
+[![asciicast](https://asciinema.org/a/595464.svg)](https://asciinema.org/a/595464)
 
 ## 参考链接
 
 * 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
 * beanio做的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
 
 ## 开源协议
```

