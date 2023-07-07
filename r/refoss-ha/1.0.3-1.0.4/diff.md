# Comparing `tmp/refoss_ha-1.0.3-py3-none-any.whl.zip` & `tmp/refoss_ha-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8271 bytes, number of entries: 14
+Zip file size: 8269 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 07:21 refoss_ha/__init__.py
--rw-r--r--  2.0 unx      426 b- defN 23-Jul-04 03:03 refoss_ha/const.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jul-07 11:29 refoss_ha/const.py
 -rw-r--r--  2.0 unx      264 b- defN 23-Jul-04 03:03 refoss_ha/enums.py
 -rw-r--r--  2.0 unx     3833 b- defN 23-Jul-04 07:56 refoss_ha/http_device.py
--rw-r--r--  2.0 unx     3226 b- defN 23-Jul-04 07:43 refoss_ha/socket_util.py
+-rw-r--r--  2.0 unx     3224 b- defN 23-Jul-07 11:29 refoss_ha/socket_util.py
 -rw-r--r--  2.0 unx     2094 b- defN 23-Jul-04 03:03 refoss_ha/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-11 12:02 refoss_ha/controller/__init__.py
 -rw-r--r--  2.0 unx     2133 b- defN 23-Jul-04 07:43 refoss_ha/controller/device.py
 -rw-r--r--  2.0 unx      719 b- defN 23-Jul-04 07:43 refoss_ha/controller/system.py
 -rw-r--r--  2.0 unx     2894 b- defN 23-Jul-04 07:43 refoss_ha/controller/toggle.py
--rw-r--r--  2.0 unx      184 b- defN 23-Jul-04 10:14 refoss_ha-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 10:14 refoss_ha-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-04 10:14 refoss_ha-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1110 b- defN 23-Jul-04 10:14 refoss_ha-1.0.3.dist-info/RECORD
-14 files, 16985 bytes uncompressed, 6425 bytes compressed:  62.2%
+-rw-r--r--  2.0 unx      186 b- defN 23-Jul-07 11:34 refoss_ha-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 11:34 refoss_ha-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-07 11:34 refoss_ha-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1110 b- defN 23-Jul-07 11:34 refoss_ha-1.0.4.dist-info/RECORD
+14 files, 16978 bytes uncompressed, 6423 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: refoss_ha/controller/system.py
 Comment: 
 
 Filename: refoss_ha/controller/toggle.py
 Comment: 
 
-Filename: refoss_ha-1.0.3.dist-info/METADATA
+Filename: refoss_ha-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: refoss_ha-1.0.3.dist-info/WHEEL
+Filename: refoss_ha-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: refoss_ha-1.0.3.dist-info/top_level.txt
+Filename: refoss_ha-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: refoss_ha-1.0.3.dist-info/RECORD
+Filename: refoss_ha-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## refoss_ha/const.py

```diff
@@ -12,14 +12,14 @@
 SOCKET_DISCOVER_UPDATE_INTERVAL = 30               #  Device Discovered Once on LAN every 30 seconds
 DEFAULT_COMMAND_TIMEOUT = 10.0
 
 
 HA_SWITCH = "switch"
 
 
-MEROSS_PLATFORMS: Final = [
+PLATFORMS: Final = [
     HA_SWITCH,
 ]
```

## refoss_ha/socket_util.py

```diff
@@ -8,15 +8,15 @@
 from .const import LOGGER
 
 
 discoverMap=dict()
 pushStateDataList=[]
 
 
-class MerossSocket :
+class SocketUtil :
 
     def __init__(self):
         self.socket = socket(AF_INET, SOCK_DGRAM)
         self.socket.setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
         self.event = threading.Event()
 
     def SocketReveiveMsg(self):
```

## Comparing `refoss_ha-1.0.3.dist-info/RECORD` & `refoss_ha-1.0.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 refoss_ha/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-refoss_ha/const.py,sha256=8EzpxUj4ldoLQw9GUvUM8ZMBOm0rf2GKAZT80oTbO3o,426
+refoss_ha/const.py,sha256=ocAuZv4OQxBzfGjcc42BHkcNhxhEWWAjVQ0YzpfBKa0,419
 refoss_ha/enums.py,sha256=e0XoXs8nJZsikplzA2RfY-ilR4q-RdjvSGZ3JIXvrok,264
 refoss_ha/http_device.py,sha256=yMavU6PbJZI3thXpXU982XU0-ukYatUOxL_a9L2gEYk,3833
-refoss_ha/socket_util.py,sha256=fABRpCmCQ04XGZc-WHHuUXwyMkq0x1ZZ7X7r1_-zFCk,3226
+refoss_ha/socket_util.py,sha256=8qyCiiQFvC7EXJS4K61_8DvCJMBPvKIBvdtFkx2PuMg,3224
 refoss_ha/util.py,sha256=C-mThHY-aqfBQNryHWyq7kozp7hc7gUrc7SVKPYONVI,2094
 refoss_ha/controller/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 refoss_ha/controller/device.py,sha256=PWmIl9qu2LMaZ7IjUMR1RvxxfCAbnkPGyAkQbscUrv0,2133
 refoss_ha/controller/system.py,sha256=YFdFSlp8dHS57GoBiz4HfqEOo4XlHClGkgurSnH2lcA,719
 refoss_ha/controller/toggle.py,sha256=FzJFuI6TJT34kdv4QNsrUtIUkYrePswuGP_j2WXkkzU,2894
-refoss_ha-1.0.3.dist-info/METADATA,sha256=JttiAQxf921udRZQdVlW1hZPKaD8HmTnNVYjO7ec8xw,184
-refoss_ha-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-refoss_ha-1.0.3.dist-info/top_level.txt,sha256=GE4dlww_crxGxvz1cACnUjObzDUbg2TvAZqaCxnODnM,10
-refoss_ha-1.0.3.dist-info/RECORD,,
+refoss_ha-1.0.4.dist-info/METADATA,sha256=subFyHyicJ6UIyZSdPC8hzMDam8GZxQcha2Rei2AzIo,186
+refoss_ha-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+refoss_ha-1.0.4.dist-info/top_level.txt,sha256=GE4dlww_crxGxvz1cACnUjObzDUbg2TvAZqaCxnODnM,10
+refoss_ha-1.0.4.dist-info/RECORD,,
```

