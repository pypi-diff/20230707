# Comparing `tmp/xToolkit-0.0.85.tar.gz` & `tmp/xToolkit-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xToolkit-0.0.85.tar", last modified: Wed Jun 14 02:27:44 2023, max compression
+gzip compressed data, was "dist\xToolkit-0.0.86.tar", last modified: Fri Jul  7 01:55:58 2023, max compression
```

## Comparing `xToolkit-0.0.85.tar` & `xToolkit-0.0.86.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.625615 xToolkit-0.0.85/
--rw-rw-rw-   0        0        0    25986 2023-06-14 02:27:44.625615 xToolkit-0.0.85/PKG-INFO
--rw-rw-rw-   0        0        0    25696 2023-06-12 08:08:30.000000 xToolkit-0.0.85/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 02:27:44.625615 xToolkit-0.0.85/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-06-14 02:27:34.000000 xToolkit-0.0.85/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.543453 xToolkit-0.0.85/xToolkit/
--rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.85/xToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.552447 xToolkit-0.0.85/xToolkit/xdatetime/
--rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/__init__.py
--rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.555472 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/__init__.py
--rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/xdatetime.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.558501 xToolkit-0.0.85/xToolkit/xfile/
--rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/__init__.py
--rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.562500 xToolkit-0.0.85/xToolkit/xfile/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xfile/dispose/__init__.py
--rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.85/xToolkit/xfile/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.568500 xToolkit-0.0.85/xToolkit/xhotchpotch/
--rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/__init__.py
--rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.573306 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/
--rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/__init__.py
--rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.586511 xToolkit-0.0.85/xToolkit/xlist/
--rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/__init__.py
--rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.590863 xToolkit-0.0.85/xToolkit/xlist/dispose/
--rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/dispose/__init__.py
--rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xlist/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.595052 xToolkit-0.0.85/xToolkit/xstring/
--rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-05-17 07:33:53.000000 xToolkit-0.0.85/xToolkit/xstring/api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.608459 xToolkit-0.0.85/xToolkit/xstring/check/
--rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/check/__init__.py
--rw-rw-rw-   0        0        0    13737 2023-06-14 02:23:04.000000 xToolkit-0.0.85/xToolkit/xstring/check/check.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.610460 xToolkit-0.0.85/xToolkit/xstring/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/dispose/__init__.py
--rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.85/xToolkit/xstring/dispose/dispose.py
--rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xstring/xstring.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.613461 xToolkit-0.0.85/xToolkit/xthreading/
--rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xthreading/__init__.py
--rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xthreading/xthread.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.623617 xToolkit-0.0.85/xToolkit/xtoolkit/
--rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/__init__.py
--rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/judgement.py
--rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.85/xToolkit/xtoolkit/xtoolkit.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:27:44.549445 xToolkit-0.0.85/xToolkit.egg-info/
--rw-rw-rw-   0        0        0    25986 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 02:27:44.000000 xToolkit-0.0.85/xToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.178249 xToolkit-0.0.86/
+-rw-rw-rw-   0        0        0    27400 2023-07-07 01:55:58.177249 xToolkit-0.0.86/PKG-INFO
+-rw-rw-rw-   0        0        0    27110 2023-07-07 01:52:16.000000 xToolkit-0.0.86/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:55:58.178249 xToolkit-0.0.86/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-07-07 01:54:35.000000 xToolkit-0.0.86/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.101344 xToolkit-0.0.86/xToolkit/
+-rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.86/xToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.111364 xToolkit-0.0.86/xToolkit/xdatetime/
+-rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xdatetime/api.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.114307 xToolkit-0.0.86/xToolkit/xdatetime/xdatetime/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xdatetime/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.86/xToolkit/xdatetime/xdatetime/xdatetime.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.117244 xToolkit-0.0.86/xToolkit/xfile/
+-rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xfile/__init__.py
+-rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xfile/api.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.120242 xToolkit-0.0.86/xToolkit/xfile/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xfile/dispose/__init__.py
+-rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.86/xToolkit/xfile/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.129761 xToolkit-0.0.86/xToolkit/xhotchpotch/
+-rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.86/xToolkit/xhotchpotch/__init__.py
+-rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.86/xToolkit/xhotchpotch/api.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.139802 xToolkit-0.0.86/xToolkit/xhotchpotch/dispose/
+-rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.86/xToolkit/xhotchpotch/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.86/xToolkit/xhotchpotch/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.147201 xToolkit-0.0.86/xToolkit/xlist/
+-rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xlist/__init__.py
+-rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xlist/api.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.150199 xToolkit-0.0.86/xToolkit/xlist/dispose/
+-rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xlist/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xlist/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.153200 xToolkit-0.0.86/xToolkit/xstring/
+-rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xstring/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-05-17 07:33:53.000000 xToolkit-0.0.86/xToolkit/xstring/api.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.161065 xToolkit-0.0.86/xToolkit/xstring/check/
+-rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xstring/check/__init__.py
+-rw-rw-rw-   0        0        0    13897 2023-07-07 01:48:52.000000 xToolkit-0.0.86/xToolkit/xstring/check/check.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.163066 xToolkit-0.0.86/xToolkit/xstring/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xstring/dispose/__init__.py
+-rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.86/xToolkit/xstring/dispose/dispose.py
+-rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xstring/xstring.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.166065 xToolkit-0.0.86/xToolkit/xthreading/
+-rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xthreading/__init__.py
+-rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xthreading/xthread.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.176255 xToolkit-0.0.86/xToolkit/xtoolkit/
+-rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xtoolkit/__init__.py
+-rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xtoolkit/judgement.py
+-rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.86/xToolkit/xtoolkit/xtoolkit.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:55:58.107443 xToolkit-0.0.86/xToolkit.egg-info/
+-rw-rw-rw-   0        0        0    27400 2023-07-07 01:55:58.000000 xToolkit-0.0.86/xToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-07-07 01:55:58.000000 xToolkit-0.0.86/xToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 01:55:58.000000 xToolkit-0.0.86/xToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-07 01:55:58.000000 xToolkit-0.0.86/xToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 01:55:58.000000 xToolkit-0.0.86/xToolkit.egg-info/top_level.txt
```

### Comparing `xToolkit-0.0.85/PKG-INFO` & `xToolkit-0.0.86/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xToolkit
-Version: 0.0.85
+Version: 0.0.86
 Summary: UNKNOWN
 Home-page: https://github.com/xionglihong/xToolkit
 Author: xionglihong
 Author-email: xionglihong@163.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -608,42 +608,56 @@
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
 ```
 
 支持的校验类型为：
 
-| 校验类型                | 关键字           | 说明                                           |
-| ----------------------- | ---------------- | ---------------------------------------------- |
-| is_car_number           | 车牌号           |                                                |
-| is_identity_card        | 身份证           |                                                |
-| is_int_or_float         | 整形或浮点型     |                                                |
-| is_int                  | 整形             |                                                |
-| is_datetime_string      | 时间字符串       |                                                |
-| is_url                  | url地址          |                                                |
-| is_phone                | 手机号           |                                                |
-| is_bank_number          | 银行卡           |                                                |
-| is_user_name            | 用户姓名         |                                                |
-| is_user_password        | 密码             |                                                |
-| is_mailbox              | 邮箱             |                                                |
-| is_json                 | json             |                                                |
-| is_choices              | 枚举格式         |                                                |
-| is_car_number_list      | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
-| is_identity_card_list   | 身份证列表       |                                                |
-| is_int_or_float_list    | 整形或浮点型列表 |                                                |
-| is_int_list             | 整形列表         |                                                |
+| 校验类型           | 关键字           | 说明                                           |
+| -------------- | ---------------- | ---------------------------------------------- |
+| is_car_number  | 车牌号           |                                                |
+| is_identity_card | 身份证           |                                                |
+| is_int_or_float | 整形或浮点型     |                                                |
+| is_int         | 整形             |                                                |
+| is_datetime_string | 时间字符串       |                                                |
+| is_url         | url地址          |                                                |
+| is_phone       | 手机号           |                                                |
+| is_bank_number | 银行卡           |                                                |
+| is_user_name   | 用户姓名         |                                                |
+| is_user_password | 密码             |                                                |
+| is_mailbox     | 邮箱             |                                                |
+| is_json        | json             |                                                |
+| is_choices     | 枚举格式         |                                                |
+| is_job         | 工号             |                                                |
+| is_ip_address  | ip地址           |                                                |
+| is_longitude_latitude | 经纬度           | 经纬度，格式为：纬度，经度                     |
+| is_phoenix     | 微鳯号           |                                                |
+| is_verification_code | 验证码           |                                                |
+| is_version     | 版本号           |                                                |
+| is_contact_information | 电话号码         | 包括中国大陆的手机号码和固定电话号码           |
+| is_car_number_list | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
+| is_identity_card_list | 身份证列表       |                                                |
+| is_int_or_float_list | 整形或浮点型列表 |                                                |
+| is_int_list    | 整形列表         |                                                |
 | is_datetime_string_list | 时间字符串列表   |                                                |
-| is_url_list             | url地址列表      |                                                |
-| is_phone_list           | 手机号列表       |                                                |
-| is_bank_number_list     | 银行卡列表       |                                                |
-| is_user_name_list       | 用户姓名列表     |                                                |
-| is_user_password_list   | 密码列表         |                                                |
-| is_mailbox_list         | 邮箱列表         |                                                |
-| is_json_list            | json列表         |                                                |
-| is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
+| is_url_list    | url地址列表      |                                                |
+| is_phone_list  | 手机号列表       |                                                |
+| is_bank_number_list | 银行卡列表       |                                                |
+| is_user_name_list | 用户姓名列表     |                                                |
+| is_user_password_list | 密码列表         |                                                |
+| is_mailbox_list | 邮箱列表         |                                                |
+| is_json_list   | json列表         |                                                |
+| is_list          | 工号列表         |                                                |
+| is_ip_address_list | ip地址列表       |                                                |
+| is_longitude_latitude_list | 经纬度列表       |                                                |
+| is_phoenix_list    | 微鳯号列表       |                                                |
+| is_verification_code_list | 验证码列表       |                                                |
+| is_version_list    | 版本号列表       |                                                |
+| is_contact_information_list | 电话号码列表     |                                                |
+| is_casual_list | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
 - regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
@@ -914,12 +928,22 @@
 
 - 复合参数校验添加ip地址校验
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
-开发计划：
+2022年05月17日 V0.0.85
 
 - 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
 - 密码校验改为必须包含数字和字母，可以包含字符，6到18位
 
+2022年05月17日 V0.0.86
+
+- 修改了邮箱的校验规则，邮箱前缀可以包含数字,大小写字母,+,-,_,汉字等
+- 字符串校验解决，传入None引起的报错
+
+开发计划：
+- 无
+
+
+
```

### Comparing `xToolkit-0.0.85/README.md` & `xToolkit-0.0.86/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -597,42 +597,56 @@
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
 ```
 
 支持的校验类型为：
 
-| 校验类型                | 关键字           | 说明                                           |
-| ----------------------- | ---------------- | ---------------------------------------------- |
-| is_car_number           | 车牌号           |                                                |
-| is_identity_card        | 身份证           |                                                |
-| is_int_or_float         | 整形或浮点型     |                                                |
-| is_int                  | 整形             |                                                |
-| is_datetime_string      | 时间字符串       |                                                |
-| is_url                  | url地址          |                                                |
-| is_phone                | 手机号           |                                                |
-| is_bank_number          | 银行卡           |                                                |
-| is_user_name            | 用户姓名         |                                                |
-| is_user_password        | 密码             |                                                |
-| is_mailbox              | 邮箱             |                                                |
-| is_json                 | json             |                                                |
-| is_choices              | 枚举格式         |                                                |
-| is_car_number_list      | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
-| is_identity_card_list   | 身份证列表       |                                                |
-| is_int_or_float_list    | 整形或浮点型列表 |                                                |
-| is_int_list             | 整形列表         |                                                |
+| 校验类型           | 关键字           | 说明                                           |
+| -------------- | ---------------- | ---------------------------------------------- |
+| is_car_number  | 车牌号           |                                                |
+| is_identity_card | 身份证           |                                                |
+| is_int_or_float | 整形或浮点型     |                                                |
+| is_int         | 整形             |                                                |
+| is_datetime_string | 时间字符串       |                                                |
+| is_url         | url地址          |                                                |
+| is_phone       | 手机号           |                                                |
+| is_bank_number | 银行卡           |                                                |
+| is_user_name   | 用户姓名         |                                                |
+| is_user_password | 密码             |                                                |
+| is_mailbox     | 邮箱             |                                                |
+| is_json        | json             |                                                |
+| is_choices     | 枚举格式         |                                                |
+| is_job         | 工号             |                                                |
+| is_ip_address  | ip地址           |                                                |
+| is_longitude_latitude | 经纬度           | 经纬度，格式为：纬度，经度                     |
+| is_phoenix     | 微鳯号           |                                                |
+| is_verification_code | 验证码           |                                                |
+| is_version     | 版本号           |                                                |
+| is_contact_information | 电话号码         | 包括中国大陆的手机号码和固定电话号码           |
+| is_car_number_list | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
+| is_identity_card_list | 身份证列表       |                                                |
+| is_int_or_float_list | 整形或浮点型列表 |                                                |
+| is_int_list    | 整形列表         |                                                |
 | is_datetime_string_list | 时间字符串列表   |                                                |
-| is_url_list             | url地址列表      |                                                |
-| is_phone_list           | 手机号列表       |                                                |
-| is_bank_number_list     | 银行卡列表       |                                                |
-| is_user_name_list       | 用户姓名列表     |                                                |
-| is_user_password_list   | 密码列表         |                                                |
-| is_mailbox_list         | 邮箱列表         |                                                |
-| is_json_list            | json列表         |                                                |
-| is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
+| is_url_list    | url地址列表      |                                                |
+| is_phone_list  | 手机号列表       |                                                |
+| is_bank_number_list | 银行卡列表       |                                                |
+| is_user_name_list | 用户姓名列表     |                                                |
+| is_user_password_list | 密码列表         |                                                |
+| is_mailbox_list | 邮箱列表         |                                                |
+| is_json_list   | json列表         |                                                |
+| is_list          | 工号列表         |                                                |
+| is_ip_address_list | ip地址列表       |                                                |
+| is_longitude_latitude_list | 经纬度列表       |                                                |
+| is_phoenix_list    | 微鳯号列表       |                                                |
+| is_verification_code_list | 验证码列表       |                                                |
+| is_version_list    | 版本号列表       |                                                |
+| is_contact_information_list | 电话号码列表     |                                                |
+| is_casual_list | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
 - regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
@@ -903,11 +917,20 @@
 
 - 复合参数校验添加ip地址校验
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
-开发计划：
+2022年05月17日 V0.0.85
 
 - 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
-- 密码校验改为必须包含数字和字母，可以包含字符，6到18位
+- 密码校验改为必须包含数字和字母，可以包含字符，6到18位
+
+2022年05月17日 V0.0.86
+
+- 修改了邮箱的校验规则，邮箱前缀可以包含数字,大小写字母,+,-,_,汉字等
+- 字符串校验解决，传入None引起的报错
+
+开发计划：
+- 无
+
```

### Comparing `xToolkit-0.0.85/setup.py` & `xToolkit-0.0.86/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.85'
+VERSION = '0.0.86'
 
 # 导入信息说明文档
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='xToolkit',
```

### Comparing `xToolkit-0.0.85/xToolkit/__init__.py` & `xToolkit-0.0.86/xToolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xdatetime/api.py` & `xToolkit-0.0.86/xToolkit/xdatetime/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xdatetime/xdatetime/xdatetime.py` & `xToolkit-0.0.86/xToolkit/xdatetime/xdatetime/xdatetime.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xfile/api.py` & `xToolkit-0.0.86/xToolkit/xfile/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xfile/dispose/dispose.py` & `xToolkit-0.0.86/xToolkit/xfile/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xhotchpotch/api.py` & `xToolkit-0.0.86/xToolkit/xhotchpotch/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xhotchpotch/dispose/dispose.py` & `xToolkit-0.0.86/xToolkit/xhotchpotch/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xlist/api.py` & `xToolkit-0.0.86/xToolkit/xlist/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xlist/dispose/dispose.py` & `xToolkit-0.0.86/xToolkit/xlist/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xstring/api.py` & `xToolkit-0.0.86/xToolkit/xstring/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xstring/check/check.py` & `xToolkit-0.0.86/xToolkit/xstring/check/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,21 +153,21 @@
         expression = "^(?![0-9]+$)(?![a-zA-Z]+$)[0-9A-Za-z\W]{6,18}$"
         return self.__regular_expression(expression)
 
     # 邮箱
     @property
     def is_mailbox(self):
         """
-        第一种：只允许英文字母、数字、下划线、英文句号、以及中划线组成
+        第一种：可以包含英文字母、数字、下划线、英文句号、以及中划线、减号、加号
         第二种：名称允许汉字、字母、数字，域名只允许英文域名
         二种中任何一种即可
         """
         expression = "{}|{}".format(
-            "^([a-zA-Z0-9_-]+@[a-zA-Z0-9_-]+(\\.[a-zA-Z0-9_-]+)+)",
-            "([A-Za-z0-9\u4e00-\u9fa5]+@[a-zA-Z0-9_-]+(\\.[a-zA-Z0-9_-]+)+)$"
+            "^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*",
+            "([A-Za-z0-9\u4e00-\u9fa5]+@[a-zA-Z0-9_-]+(\\.[a-zA-Z0-9_-]+)+)$",
         )
 
         return self.__regular_expression(expression)
 
     # 工号
     @property
     def is_job(self):
@@ -185,15 +185,14 @@
         """
         expression = "^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$"
         return self.__regular_expression(expression)
 
     # 经纬度
     @property
     def is_longitude_latitude(self):
-        print("-")
         """
         经纬度，格式为：纬度，经度
         其中纬度的范围在-90到90之间，经度的范围在-180到180之间
         """
         expression = "^[-]?([1-8]?\d(\.\d+)?|90(\.0+)?)\s*[,]\s*[-]?(180(\.0+)?|((1[0-7]\d)|([1-9]?\d))(\.\d+)?)$"
         return self.__regular_expression(expression)
 
@@ -217,15 +216,15 @@
 
     # 版本号
     @property
     def is_version(self):
         """
         版本号 格式为 V0.0.1
         """
-        expression = "^V[0-99]\.[0-99]\.[1-99]$"
+        expression = "^V([0-9]|[1-9][0-9]?)\.([0-9]|[1-9][0-9]?)\.([1-9]|[1-9][0-9])$"
         return self.__regular_expression(expression)
 
     # 电话号码
     @property
     def is_contact_information(self):
         """
         包括中国大陆的手机号码和固定电话号码
@@ -350,14 +349,18 @@
         choices = kwargs["choices"] if kwargs.get("choices") else None
         max_length = kwargs["max_length"] if kwargs.get("max_length") else None  # 最大字符串长度
         regular = kwargs["regular"] if kwargs.get("regular") else None  # 自定义正则表达式
 
         result = False
         # 如果长度超出最大长度
         if max_length:
+            # 长度判断只接受字符串
+            if not isinstance(self.parameter, (str,)):
+                return False
+
             if len(self.parameter) > max_length:
                 return result
 
         if is_blank is True:
             if self.parameter:
                 result = self.regular_logic(rule, choices=choices, regular=regular)
             else:
```

### Comparing `xToolkit-0.0.85/xToolkit/xstring/dispose/dispose.py` & `xToolkit-0.0.86/xToolkit/xstring/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xstring/xstring.py` & `xToolkit-0.0.86/xToolkit/xstring/xstring.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xthreading/xthread.py` & `xToolkit-0.0.86/xToolkit/xthreading/xthread.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit/xtoolkit/judgement.py` & `xToolkit-0.0.86/xToolkit/xtoolkit/judgement.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.85/xToolkit.egg-info/PKG-INFO` & `xToolkit-0.0.86/xToolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xToolkit
-Version: 0.0.85
+Version: 0.0.86
 Summary: UNKNOWN
 Home-page: https://github.com/xionglihong/xToolkit
 Author: xionglihong
 Author-email: xionglihong@163.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -608,42 +608,56 @@
                 return GlobalReturn(code=10001, msg="{}为{}，格式错误".format(key, item))
 
         return GlobalReturn(**OperationOrderForm().select_order_list(request=request, **parameter))
 ```
 
 支持的校验类型为：
 
-| 校验类型                | 关键字           | 说明                                           |
-| ----------------------- | ---------------- | ---------------------------------------------- |
-| is_car_number           | 车牌号           |                                                |
-| is_identity_card        | 身份证           |                                                |
-| is_int_or_float         | 整形或浮点型     |                                                |
-| is_int                  | 整形             |                                                |
-| is_datetime_string      | 时间字符串       |                                                |
-| is_url                  | url地址          |                                                |
-| is_phone                | 手机号           |                                                |
-| is_bank_number          | 银行卡           |                                                |
-| is_user_name            | 用户姓名         |                                                |
-| is_user_password        | 密码             |                                                |
-| is_mailbox              | 邮箱             |                                                |
-| is_json                 | json             |                                                |
-| is_choices              | 枚举格式         |                                                |
-| is_car_number_list      | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
-| is_identity_card_list   | 身份证列表       |                                                |
-| is_int_or_float_list    | 整形或浮点型列表 |                                                |
-| is_int_list             | 整形列表         |                                                |
+| 校验类型           | 关键字           | 说明                                           |
+| -------------- | ---------------- | ---------------------------------------------- |
+| is_car_number  | 车牌号           |                                                |
+| is_identity_card | 身份证           |                                                |
+| is_int_or_float | 整形或浮点型     |                                                |
+| is_int         | 整形             |                                                |
+| is_datetime_string | 时间字符串       |                                                |
+| is_url         | url地址          |                                                |
+| is_phone       | 手机号           |                                                |
+| is_bank_number | 银行卡           |                                                |
+| is_user_name   | 用户姓名         |                                                |
+| is_user_password | 密码             |                                                |
+| is_mailbox     | 邮箱             |                                                |
+| is_json        | json             |                                                |
+| is_choices     | 枚举格式         |                                                |
+| is_job         | 工号             |                                                |
+| is_ip_address  | ip地址           |                                                |
+| is_longitude_latitude | 经纬度           | 经纬度，格式为：纬度，经度                     |
+| is_phoenix     | 微鳯号           |                                                |
+| is_verification_code | 验证码           |                                                |
+| is_version     | 版本号           |                                                |
+| is_contact_information | 电话号码         | 包括中国大陆的手机号码和固定电话号码           |
+| is_car_number_list | 车牌号列表       | 列表的每一个值为车牌号，以下同理               |
+| is_identity_card_list | 身份证列表       |                                                |
+| is_int_or_float_list | 整形或浮点型列表 |                                                |
+| is_int_list    | 整形列表         |                                                |
 | is_datetime_string_list | 时间字符串列表   |                                                |
-| is_url_list             | url地址列表      |                                                |
-| is_phone_list           | 手机号列表       |                                                |
-| is_bank_number_list     | 银行卡列表       |                                                |
-| is_user_name_list       | 用户姓名列表     |                                                |
-| is_user_password_list   | 密码列表         |                                                |
-| is_mailbox_list         | 邮箱列表         |                                                |
-| is_json_list            | json列表         |                                                |
-| is_casual_list          | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
+| is_url_list    | url地址列表      |                                                |
+| is_phone_list  | 手机号列表       |                                                |
+| is_bank_number_list | 银行卡列表       |                                                |
+| is_user_name_list | 用户姓名列表     |                                                |
+| is_user_password_list | 密码列表         |                                                |
+| is_mailbox_list | 邮箱列表         |                                                |
+| is_json_list   | json列表         |                                                |
+| is_list          | 工号列表         |                                                |
+| is_ip_address_list | ip地址列表       |                                                |
+| is_longitude_latitude_list | 经纬度列表       |                                                |
+| is_phoenix_list    | 微鳯号列表       |                                                |
+| is_verification_code_list | 验证码列表       |                                                |
+| is_version_list    | 版本号列表       |                                                |
+| is_contact_information_list | 电话号码列表     |                                                |
+| is_casual_list | 任意列表         | 列表里面的值不进行校验，只能确保整体是一个列表 |
 
 参数说明 xstring.formative(parameter, **kwargs)：
 
 - parameter 为需要校验的参数名称
 - is_blank 是否可以为空，如果可以为空，不进行规则校验，直接返回空字符串，如果用户传了，就进行规则校验
 - rule 为正则标识，如果rule为is_choices，必须传choices，choices为枚举值，choices的类型为列表
 - regular 为自定义正则表达式，如果传入自定义正则表达式就使用用户的正则表达式
@@ -914,12 +928,22 @@
 
 - 复合参数校验添加ip地址校验
 
 2022年05月17日 V0.0.84
 
 - 复合参数校验添加自定义正则表达式校验
 
-开发计划：
+2022年05月17日 V0.0.85
 
 - 加入微鳯号校验，经纬度格式校验，版本号，大陆联系号码正则表达式校验
 - 密码校验改为必须包含数字和字母，可以包含字符，6到18位
 
+2022年05月17日 V0.0.86
+
+- 修改了邮箱的校验规则，邮箱前缀可以包含数字,大小写字母,+,-,_,汉字等
+- 字符串校验解决，传入None引起的报错
+
+开发计划：
+- 无
+
+
+
```

### Comparing `xToolkit-0.0.85/xToolkit.egg-info/SOURCES.txt` & `xToolkit-0.0.86/xToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

