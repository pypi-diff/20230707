# Comparing `tmp/s3cps3-6.6.5.tar.gz` & `tmp/s3cps3-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s3cps3-6.6.5.tar", last modified: Fri Jul  7 08:12:10 2023, max compression
+gzip compressed data, was "dist/s3cps3-6.6.6.tar", last modified: Fri Jul  7 08:38:10 2023, max compression
```

## Comparing `s3cps3-6.6.5.tar` & `s3cps3-6.6.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:12:10.000000 s3cps3-6.6.5/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-6.6.5/LICENSE
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       80 2023-07-05 10:09:29.000000 s3cps3-6.6.5/MANIFEST.in
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2582 2023-07-07 08:12:10.000000 s3cps3-6.6.5/PKG-INFO
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-6.6.5/s3cps3/__init__.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-6.6.5/s3cps3/commons.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2212 2023-07-06 02:46:29.000000 s3cps3-6.6.5/s3cps3/listbucket.py
--rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)    10431 2023-07-07 06:51:21.000000 s3cps3-6.6.5/s3cps3/main.xsh
--rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       94 2023-07-07 06:46:43.000000 s3cps3-6.6.5/s3cps3/s32s3
--rwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      437 2023-05-29 13:19:00.000000 s3cps3-6.6.5/s3cps3/s3bigcp.sh
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4119 2023-07-06 02:43:40.000000 s3cps3-6.6.5/s3cps3/s3cps3.py
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2582 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      299 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      122 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/requires.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-07 08:12:10.000000 s3cps3-6.6.5/s3cps3.egg-info/top_level.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-07 08:12:10.000000 s3cps3-6.6.5/setup.cfg
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      701 2023-07-07 08:08:44.000000 s3cps3-6.6.5/setup.py
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:38:10.000000 s3cps3-6.6.6/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-6.6.6/LICENSE
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       80 2023-07-05 10:09:29.000000 s3cps3-6.6.6/MANIFEST.in
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2640 2023-07-07 08:38:10.000000 s3cps3-6.6.6/PKG-INFO
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2509 2023-07-07 08:08:30.000000 s3cps3-6.6.6/README.md
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-6.6.6/s3cps3/__init__.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-6.6.6/s3cps3/commons.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2212 2023-07-06 02:46:29.000000 s3cps3-6.6.6/s3cps3/listbucket.py
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)    10431 2023-07-07 06:51:21.000000 s3cps3-6.6.6/s3cps3/main.xsh
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       94 2023-07-07 06:46:43.000000 s3cps3-6.6.6/s3cps3/s32s3
+-rwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      437 2023-05-29 13:19:00.000000 s3cps3-6.6.6/s3cps3/s3bigcp.sh
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4119 2023-07-06 02:43:40.000000 s3cps3-6.6.6/s3cps3/s3cps3.py
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2640 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      309 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      122 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-07 08:38:10.000000 s3cps3-6.6.6/s3cps3.egg-info/top_level.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-07 08:38:10.000000 s3cps3-6.6.6/setup.cfg
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      722 2023-07-07 08:37:46.000000 s3cps3-6.6.6/setup.py
```

### Comparing `s3cps3-6.6.5/LICENSE` & `s3cps3-6.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.5/PKG-INFO` & `s3cps3-6.6.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: s3cps3
-Version: 6.6.5
-License-File: LICENSE
-
 
 ## 命令功能
 #### 实现数据桶到数据桶之间的数据传输功能，无需先下载到本地再上传；
 #### 考虑到可能遇到大批量小文件传输的需求，本包可实现通过扫描分割大小文件，并将大文件通过aws包的cp命令传输，为小文件分配python多线程传输，提高传输效率;
 #### 考虑到可能遇到各种因素导致传输中断，在中断后为了节省时间可以通过读取上一次扫描后生成的大小文件列表，跳过重新扫描这一步骤；
```

### Comparing `s3cps3-6.6.5/s3cps3/commons.py` & `s3cps3-6.6.6/s3cps3/commons.py`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.5/s3cps3/listbucket.py` & `s3cps3-6.6.6/s3cps3/listbucket.py`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.5/s3cps3/main.xsh` & `s3cps3-6.6.6/s3cps3/main.xsh`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.5/s3cps3/s3cps3.py` & `s3cps3-6.6.6/s3cps3/s3cps3.py`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.5/s3cps3.egg-info/PKG-INFO` & `s3cps3-6.6.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: s3cps3
-Version: 6.6.5
+Version: 6.6.6
 License-File: LICENSE
 
-
-## 命令功能
-#### 实现数据桶到数据桶之间的数据传输功能，无需先下载到本地再上传；
-#### 考虑到可能遇到大批量小文件传输的需求，本包可实现通过扫描分割大小文件，并将大文件通过aws包的cp命令传输，为小文件分配python多线程传输，提高传输效率;
-#### 考虑到可能遇到各种因素导致传输中断，在中断后为了节省时间可以通过读取上一次扫描后生成的大小文件列表，跳过重新扫描这一步骤；
-
-
-## 安装
-### linux命令
-s3cps3及其依赖项的安装使用pip和setuptools提供的一系列打包功能。为保证安装顺利，建议使用：
-#### pip:9.0.2或更高版本
-#### setuptools：36.2.0或更高版本
-#### 安装s3cps3最安全的方法实在virtualenv中使用pip：
-$ pip -m install s3cps3
-#### 或者，如果您没有在virtualenv中安装，则全局安装：
-$ sudo python -m pip install s3cps3
-### awscli配置
-#### 在使用s3cps3之前，您需要配置AWS凭证，您可以通过多种方式执行此操作：
-#### 最快的入门方法是运行aws configure命令：
-#### $ aws configure
-#### AWS Access Key ID: MYACCESSKEY
-#### AWS Secret Access Key: MYSECRETKEY
-#### Default region name [us-west-2]: us-west-2
-#### Default output format [None]: json
-#### 要使用环境变量，请执行以下操作：
-#### $ export AWS_ACCESS_KEY_ID=<access_key>
-#### $ export AWS_SECRET_ACCESS_KEY=<secret_key>
-#### 要使用共享凭据文件(credentials)，请创建一个INI格式的文件，如下所示：
-#### [default]
-#### aws_access_key_id=MYACCESSKEY
-#### aws_secret_access_key=MYSECRETKEY
-
-#### [testing]
-#### aws_access_key_id=MYACCESKEY
-#### aws_secret_access_key=MYSECRETKEY
-
-#### 要使用配置文件，请创建一个INI格式的文件，如下所示：
-#### [default]
-#### aws_access_key_id=default access key
-#### aws_secret_access_key=default secret key
-
-#### [profile testing]
-#### aws_access_key_id=testing access key
-#### aws_secret_access_key=testing secret key
-
-#### [plugins]
-#### endpoint = awscli_plugin_endpoint
-
-## 使用
-#### s3cps3命令具有以下结构：
-#### s32cp options parameters options parameters ..
-#### 例如，从源数据桶传输文件到目标数据桶，可以参考：
-#### s32s3 --s src_profile@s3://path/to/src/ --d dst_profile@s3://path/to/dst/
-#### 如果想要调用上次扫描的大小文件列表，可以参考：
-#### s32s3 --s src_profile@s3://path/to/src/ --d dst_profile@s3://path/to/dst/ --c 1
-
-
-
+
+## 命令功能
+#### 实现数据桶到数据桶之间的数据传输功能，无需先下载到本地再上传；
+#### 考虑到可能遇到大批量小文件传输的需求，本包可实现通过扫描分割大小文件，并将大文件通过aws包的cp命令传输，为小文件分配python多线程传输，提高传输效率;
+#### 考虑到可能遇到各种因素导致传输中断，在中断后为了节省时间可以通过读取上一次扫描后生成的大小文件列表，跳过重新扫描这一步骤；
+
+
+## 安装
+### linux命令
+s3cps3及其依赖项的安装使用pip和setuptools提供的一系列打包功能。为保证安装顺利，建议使用：
+#### pip:9.0.2或更高版本
+#### setuptools：36.2.0或更高版本
+#### 安装s3cps3最安全的方法实在virtualenv中使用pip：
+$ pip -m install s3cps3
+#### 或者，如果您没有在virtualenv中安装，则全局安装：
+$ sudo python -m pip install s3cps3
+### awscli配置
+#### 在使用s3cps3之前，您需要配置AWS凭证，您可以通过多种方式执行此操作：
+#### 最快的入门方法是运行aws configure命令：
+#### $ aws configure
+#### AWS Access Key ID: MYACCESSKEY
+#### AWS Secret Access Key: MYSECRETKEY
+#### Default region name [us-west-2]: us-west-2
+#### Default output format [None]: json
+#### 要使用环境变量，请执行以下操作：
+#### $ export AWS_ACCESS_KEY_ID=<access_key>
+#### $ export AWS_SECRET_ACCESS_KEY=<secret_key>
+#### 要使用共享凭据文件(credentials)，请创建一个INI格式的文件，如下所示：
+#### [default]
+#### aws_access_key_id=MYACCESSKEY
+#### aws_secret_access_key=MYSECRETKEY
+
+#### [testing]
+#### aws_access_key_id=MYACCESKEY
+#### aws_secret_access_key=MYSECRETKEY
+
+#### 要使用配置文件，请创建一个INI格式的文件，如下所示：
+#### [default]
+#### aws_access_key_id=default access key
+#### aws_secret_access_key=default secret key
+
+#### [profile testing]
+#### aws_access_key_id=testing access key
+#### aws_secret_access_key=testing secret key
+
+#### [plugins]
+#### endpoint = awscli_plugin_endpoint
+
+## 使用
+#### s3cps3命令具有以下结构：
+#### s32cp options parameters options parameters ..
+#### 例如，从源数据桶传输文件到目标数据桶，可以参考：
+#### s32s3 --s src_profile@s3://path/to/src/ --d dst_profile@s3://path/to/dst/
+#### 如果想要调用上次扫描的大小文件列表，可以参考：
+#### s32s3 --s src_profile@s3://path/to/src/ --d dst_profile@s3://path/to/dst/ --c 1
+
+
+
```

