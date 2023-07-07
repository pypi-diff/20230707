# Comparing `tmp/ectool-1.0.2.tar.gz` & `tmp/ectool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.0.2.tar", last modified: Thu Jul  6 15:09:22 2023, max compression
+gzip compressed data, was "ectool-1.1.0.tar", last modified: Fri Jul  7 07:01:39 2023, max compression
```

## Comparing `ectool-1.0.2.tar` & `ectool-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:09:22.946923 ectool-1.0.2/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1209 2023-07-06 15:09:22.946923 ectool-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-07-06 14:20:41.000000 ectool-1.0.2/README.md
--rw-rw-rw-   0        0        0      113 2023-07-06 15:09:22.947923 ectool-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     7870 2023-07-06 15:08:38.000000 ectool-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:09:22.928922 ectool-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 15:09:22.938923 ectool-1.0.2/src/ectool/
--rw-rw-rw-   0        0        0      112 2023-07-06 14:56:04.000000 ectool-1.0.2/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15134 2023-07-06 14:56:04.000000 ectool-1.0.2/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0     2527 2023-07-06 15:00:58.000000 ectool-1.0.2/src/ectool/ecburn.py
--rw-rw-rw-   0        0        0     1249 2023-07-06 14:41:48.000000 ectool-1.0.2/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.0.2/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     1811 2023-07-04 13:47:02.000000 ectool-1.0.2/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:09:22.945923 ectool-1.0.2/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     1209 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 15:09:22.000000 ectool-1.0.2/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.768663 ectool-1.1.0/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1585 2023-07-07 07:01:39.768663 ectool-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-07-07 06:59:20.000000 ectool-1.1.0/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-07 07:01:39.769663 ectool-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     7895 2023-07-07 06:56:02.000000 ectool-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.746662 ectool-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.759663 ectool-1.1.0/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.0/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15521 2023-07-07 06:53:51.000000 ectool-1.1.0/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.0/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     5069 2023-07-07 07:00:17.000000 ectool-1.1.0/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.0/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.0/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3790 2023-07-07 06:32:49.000000 ectool-1.1.0/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.767662 ectool-1.1.0/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     1585 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.0.2/LICENSE` & `ectool-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.0.2/setup.py` & `ectool-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.2",  # Required
+    version="1.1.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -119,15 +119,15 @@
     python_requires=">=3.7, <4",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=["cstruct"],  # Optional
+    install_requires=["cstruct", "pyserial", "py7zr"],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
@@ -141,24 +141,24 @@
     package_data={  # Optional
         #"sample": ["package_data.dat"],
     },
     # Entry points. The following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
         "console_scripts": [
-            "ectool=ectool:main",
+            "ectool=ectool.eccli:main",
         ],
     },
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={  # Optional
-        "Bug Reports": "https://github.com/openLuat/ectools2py/issues",
-        "Source": "https://github.com/openLuat/ectools2py/",
+        "Bug Reports": "https://github.com/openLuat/ectool2py/issues",
+        "Source": "https://github.com/openLuat/ectool2py/",
     },
 )
```

### Comparing `ectool-1.0.2/src/ectool/ecaction.py` & `ectool-1.1.0/src/ectool/ecaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,24 @@
             if send_buff == recv_buff :
                 logging.debug("sync done")
                 return 0
 
     logging.error("sync fail")
     return -1
 
-def burn_agboot(burncom, agent, baud, hashtype=None, pullupQspi=1):
+def burn_agboot(burncom, path_or_data, baud, hashtype=None, pullupQspi=1):
     logging.debug("Burn agent boot start")
     ret = package_base_info(burncom, get_imageid(enBurnImageType.BTYPE_HEAD))
     if ret != 0:
         return ret
-    with open(agent, "rb") as f :
-        fdata = f.read()
+    if path_or_data.__class__.__name__ == "bytes" :
+        fdata = path_or_data
+    else :
+        with open(path_or_data, "rb") as f :
+            fdata = f.read()
     logging.debug("agentboot file size " + str(len(fdata)))
     ret = package_image_head(burncom, fdata, enBurnImageType.BTYPE_AGBOOT, 0)
     if ret != 0:
         return ret
     ret = burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_DLBOOT, 2)
     if ret != 0:
         return ret
@@ -87,16 +90,16 @@
     pCmd.len = len(fdata)
     ret = package_data(burncom, pCmd, fdata, pullupQspi=1)
     if ret != 0:
         return ret
 
     return 0
 
-def burn_img(burncom, path, img_type, storType, addr):
-    logging.debug("Burn image start " + path + " " + str(img_type))
+def burn_img(burncom, path_or_data, img_type, storType, addr, tag="NAME"):
+    logging.debug("Burn image start " + str(img_type))
     # 1. 先执行一次 LPC Sync
     ret = burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_LPC, 2)
     if ret != 0 :
         logging.error("lpc sync fail")
         return -1
     # 2. lpc burn one
     ret, _ = package_lpc_burn_one(burncom, img_type, storType)
@@ -112,16 +115,20 @@
     if ret != 0 :
         logging.error("agentboot(1) sync fail")
         return -1
     ret = package_base_info(burncom, enBurnImageType.BTYPE_HEAD, False)
     if ret != 0 :
         logging.error("package_base_info fail")
         return -1
-    with open(path, "rb") as f :
-        fdata = f.read()
+    
+    if path_or_data.__class__.__name__ == "bytes" :
+        fdata = path_or_data
+    else :
+        with open(path_or_data, "rb") as f :
+            fdata = f.read()
     ret = package_image_head(burncom, fdata, img_type, addr, baud=0, bDlBoot=False, pullupQspi=0)
     if ret != 0 :
         logging.error("package_image_head fail")
         return -1
 
     remain = len(fdata)
     data_offset = 0
@@ -146,17 +153,19 @@
         ret = package_data(burncom, pCmd, fdata[data_offset:data_offset + data_len], False)
         if ret != 0:
             logging.error("package_data fail")
             break
 
         data_offset += data_len
         remain -= data_len
+        logging.info("downloading " + tag + " " + str(int(data_offset*100/len(fdata))) + "%")
     logging.debug("almost done burn_img")
     if ret == 0 :
         ret, tmpdata = package_lpc_get_burn_status(burncom)
+    logging.info("downloading " + tag + " 100%")
     return ret
 
 
 def sys_reset(burncom) :
     ret = burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_LPC, 2)
     if ret != 0 :
         logging.error("sys_reset fail")
@@ -259,15 +268,15 @@
         cmd.len = (crc8_maxim(struct.pack("<I", tmplen)[:3]) << 24) + tmplen
     com_write(burncom, cmd.pack() + data + struct.pack("<I", ckVal))
     recv_buff = com_read(burncom, 6)
     if recv_buff :
         logging.debug("rsp buff " + recv_buff.hex())
         rsp = stlpcRsp()
         rsp.unpack(recv_buff)
-        logging.info("lpc rsp " + str(rsp.state) + " " + str(rsp.len))
+        logging.debug("lpc rsp " + str(rsp.state) + " " + str(rsp.len))
         if rsp.len > 0 :
             recv_buff = com_read(burncom, rsp.len)
         crc32_buff = com_read(burncom, 4)
         if crc32_buff :
             logging.debug("lpc rsp CRC32 " + crc32_buff.hex().upper())
         if rsp.state != 0 :
             logging.warning("read lpc rsp not ACK " + str(rsp.state))
```

### Comparing `ectool-1.0.2/src/ectool/ecstruct.py` & `ectool-1.1.0/src/ectool/ecstruct.py`

 * *Files identical despite different names*

