# Comparing `tmp/threads-net-0.0.3.tar.gz` & `tmp/threads-net-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.3.tar", last modified: Fri Jul  7 11:49:54 2023, max compression
+gzip compressed data, was "threads-net-0.0.4.tar", last modified: Fri Jul  7 19:24:14 2023, max compression
```

## Comparing `threads-net-0.0.3.tar` & `threads-net-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.642738 threads-net-0.0.3/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.3/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.3/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43426 2023-07-07 11:49:54.642630 threads-net-0.0.3/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    42575 2023-07-07 10:29:58.000000 threads-net-0.0.3/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641565 threads-net-0.0.3/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.3/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      243 2023-07-07 10:23:26.000000 threads-net-0.0.3/examples/get_post.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      230 2023-07-07 10:23:34.000000 threads-net-0.0.3/examples/get_user.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      262 2023-07-07 10:23:42.000000 threads-net-0.0.3/examples/get_user_replies.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      264 2023-07-07 10:23:50.000000 threads-net-0.0.3/examples/get_user_threads.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641666 threads-net-0.0.3/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.3/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 11:49:54.642771 threads-net-0.0.3/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 11:49:26.000000 threads-net-0.0.3/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.641912 threads-net-0.0.3/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.3/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3175 2023-07-07 09:42:09.000000 threads-net-0.0.3/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 11:49:54.642440 threads-net-0.0.3/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43426 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      394 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 11:49:54.000000 threads-net-0.0.3/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.914698 threads-net-0.0.4/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.4/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.4/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43935 2023-07-07 19:24:14.914590 threads-net-0.0.4/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43084 2023-07-07 19:21:59.000000 threads-net-0.0.4/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913622 threads-net-0.0.4/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.4/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      389 2023-07-07 18:52:22.000000 threads-net-0.0.4/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-07 18:47:05.000000 threads-net-0.0.4/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      408 2023-07-07 18:40:46.000000 threads-net-0.0.4/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      410 2023-07-07 18:40:52.000000 threads-net-0.0.4/examples/get_user_threads.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.4/examples/login.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913722 threads-net-0.0.4/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.4/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 19:24:14.914728 threads-net-0.0.4/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 19:23:52.000000 threads-net-0.0.4/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913909 threads-net-0.0.4/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.4/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5379 2023-07-07 19:22:38.000000 threads-net-0.0.4/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.914416 threads-net-0.0.4/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43935 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.3/LICENSE` & `threads-net-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.3/PKG-INFO` & `threads-net-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-Metadata-Version: 2.1
-Name: threads-net
-Version: 0.0.3
-Summary: Threads (threads.net) Python API wrapper
-Home-page: https://github.com/dmytrostriletskyi/threads
-Author: Dmytro Striletskyi
-Author-email: dmytro.striletskyi@gmail.com
-License: MIT
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
+* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
-  * [Get User](#get-user)
+  * [Login](#login)
+  * [Get User By Username](#get-user-by-username)
+  * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
+## Disclaimer
+
+* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
+  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
+  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
+  is used because Threads are backed by Instagram and you login via it as well.
+
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
 ```bash
@@ -52,80 +41,95 @@
 Import the class responsible for `Threads API` communication and start using it with the following commands:
 
 ```python3
 >>> from threads import Threads
 >>> threads = Threads()
 ```
 
-Under the hood, in the constructor (`__init__`), it makes a request to the `Threads API` to fetch a token. It is called 
-`lsd` internally and is required for any request. For anonymous users, it is just generated automatically from 
-API's back-end and passed to front-end. So, basically, you do not need any `API key` or other credentials to use the library.
-
 ### Examples
 
 Find examples of how to use the library functionality in the `examples` folder:
 
 ```bash
 ➜  ls examples
 examples
-├── __init__.py
+├── login.py
 ├── get_post.py
 ├── get_user.py
 ├── get_user_replies.py
 └── get_user_threads.py
 ...
 ```
 
 ## API
 
-### Get User
+### Login
+
+In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
+there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
 
-To get a user, use the following commands:
+```python3
+>>> threads = Threads()
+>>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
+>>> threads.dump_settings('session.json')
+```
+
+Next time, just load the session from the file and use it for login with the following commands:
 
 ```python3
->>> user = threads.get_user(id=314216)
+>>> threads = Threads()
+>>> threads.load_settings('session.json')
+>>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+```
+
+The login method might ask for additional username/password entering, confirmation code and other challenges. But if
+you reuse the session, those should be minimum times. For more information, check this out — 
+https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
+
+### Get User by Username
+
+To get a user by a username, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_username(username='zuck')
 >>> user
 {
-    "data": {
-        "userData": {
-            "user": {
-                "is_private": false,
-                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfANyGvPklT1Hkax6hmmmzvD7QX2vwqYe4XAzZIYo1fGqA&oe=64ACDDC0&_nc_sid=10d13b",
-                "username": "zuck",
-                "hd_profile_pic_versions": [
-                    {
-                        "height": 320,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCjdM98k9QZZVAr3czL_EjLYje6g__zJ8b_q3ZQi8Uqpw&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 320
-                    },
-                    {
-                        "height": 640,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDA1pVfIGaKNihFuUc80xxx8SnNgnqlpvxSCSq9N_n-mQ&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 640
-                    }
-                ],
-                "is_verified": true,
-                "biography": "",
-                "biography_with_entities": null,
-                "follower_count": 1988496,
-                "profile_context_facepile_users": null,
-                "bio_links": [
-                    {
-                        "url": ""
-                    }
-                ],
-                "pk": "314216",
-                "full_name": "Mark Zuckerberg",
-                "id": null
-            }
-        }
-    },
-    "extensions": {
-        "is_final": true
-    }
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
+}
+```
+
+### Get User by Identifier
+
+To get a user by an identifier, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_id(id=314216)
+>>> user
+{
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
@@ -639,8 +643,7 @@
         }
     },
     "extensions": {
         "is_final": true
     }
 }
 ```
-
```

### Comparing `threads-net-0.0.3/README.md` & `threads-net-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,57 @@
+Metadata-Version: 2.1
+Name: threads-net
+Version: 0.0.4
+Summary: Threads (threads.net) Python API wrapper
+Home-page: https://github.com/dmytrostriletskyi/threads
+Author: Dmytro Striletskyi
+Author-email: dmytro.striletskyi@gmail.com
+License: MIT
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
+* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
-  * [Get User](#get-user)
+  * [Login](#login)
+  * [Get User By Username](#get-user-by-username)
+  * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
+## Disclaimer
+
+* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
+  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
+  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
+  is used because Threads are backed by Instagram and you login via it as well.
+
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
 ```bash
@@ -30,80 +63,95 @@
 Import the class responsible for `Threads API` communication and start using it with the following commands:
 
 ```python3
 >>> from threads import Threads
 >>> threads = Threads()
 ```
 
-Under the hood, in the constructor (`__init__`), it makes a request to the `Threads API` to fetch a token. It is called 
-`lsd` internally and is required for any request. For anonymous users, it is just generated automatically from 
-API's back-end and passed to front-end. So, basically, you do not need any `API key` or other credentials to use the library.
-
 ### Examples
 
 Find examples of how to use the library functionality in the `examples` folder:
 
 ```bash
 ➜  ls examples
 examples
-├── __init__.py
+├── login.py
 ├── get_post.py
 ├── get_user.py
 ├── get_user_replies.py
 └── get_user_threads.py
 ...
 ```
 
 ## API
 
-### Get User
+### Login
+
+In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
+there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
 
-To get a user, use the following commands:
+```python3
+>>> threads = Threads()
+>>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
+>>> threads.dump_settings('session.json')
+```
+
+Next time, just load the session from the file and use it for login with the following commands:
 
 ```python3
->>> user = threads.get_user(id=314216)
+>>> threads = Threads()
+>>> threads.load_settings('session.json')
+>>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+```
+
+The login method might ask for additional username/password entering, confirmation code and other challenges. But if
+you reuse the session, those should be minimum times. For more information, check this out — 
+https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
+
+### Get User by Username
+
+To get a user by a username, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_username(username='zuck')
 >>> user
 {
-    "data": {
-        "userData": {
-            "user": {
-                "is_private": false,
-                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfANyGvPklT1Hkax6hmmmzvD7QX2vwqYe4XAzZIYo1fGqA&oe=64ACDDC0&_nc_sid=10d13b",
-                "username": "zuck",
-                "hd_profile_pic_versions": [
-                    {
-                        "height": 320,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCjdM98k9QZZVAr3czL_EjLYje6g__zJ8b_q3ZQi8Uqpw&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 320
-                    },
-                    {
-                        "height": 640,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDA1pVfIGaKNihFuUc80xxx8SnNgnqlpvxSCSq9N_n-mQ&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 640
-                    }
-                ],
-                "is_verified": true,
-                "biography": "",
-                "biography_with_entities": null,
-                "follower_count": 1988496,
-                "profile_context_facepile_users": null,
-                "bio_links": [
-                    {
-                        "url": ""
-                    }
-                ],
-                "pk": "314216",
-                "full_name": "Mark Zuckerberg",
-                "id": null
-            }
-        }
-    },
-    "extensions": {
-        "is_final": true
-    }
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
+}
+```
+
+### Get User by Identifier
+
+To get a user by an identifier, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_id(id=314216)
+>>> user
+{
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
@@ -617,8 +665,7 @@
         }
     },
     "extensions": {
         "is_final": true
     }
 }
 ```
-
```

### Comparing `threads-net-0.0.3/setup.py` & `threads-net-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r', encoding='utf-8') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.3',
+    version='0.0.4',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.3/threads_net.egg-info/PKG-INFO` & `threads-net-0.0.4/threads_net.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.3
+Version: 0.0.4
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -23,24 +23,35 @@
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
+* [Disclaimer](#disclaimer)
 * [Getting started](#getting-started)
   * [How to install](#how-to-install)
   * [Initialization](#initialization)
   * [Examples](#examples)
 * [API](#api)
-  * [Get User](#get-user)
+  * [Login](#login)
+  * [Get User By Username](#get-user-by-username)
+  * [Get User By Identifier](#get-user-by-identifier)
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
+## Disclaimer
+
+* This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
+  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
+  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+* For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
+  is used because Threads are backed by Instagram and you login via it as well.
+
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
 ```bash
@@ -52,80 +63,95 @@
 Import the class responsible for `Threads API` communication and start using it with the following commands:
 
 ```python3
 >>> from threads import Threads
 >>> threads = Threads()
 ```
 
-Under the hood, in the constructor (`__init__`), it makes a request to the `Threads API` to fetch a token. It is called 
-`lsd` internally and is required for any request. For anonymous users, it is just generated automatically from 
-API's back-end and passed to front-end. So, basically, you do not need any `API key` or other credentials to use the library.
-
 ### Examples
 
 Find examples of how to use the library functionality in the `examples` folder:
 
 ```bash
 ➜  ls examples
 examples
-├── __init__.py
+├── login.py
 ├── get_post.py
 ├── get_user.py
 ├── get_user_replies.py
 └── get_user_threads.py
 ...
 ```
 
 ## API
 
-### Get User
+### Login
+
+In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
+there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+
+```python3
+>>> threads = Threads()
+>>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
+>>> threads.dump_settings('session.json')
+```
 
-To get a user, use the following commands:
+Next time, just load the session from the file and use it for login with the following commands:
 
 ```python3
->>> user = threads.get_user(id=314216)
+>>> threads = Threads()
+>>> threads.load_settings('session.json')
+>>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+```
+
+The login method might ask for additional username/password entering, confirmation code and other challenges. But if
+you reuse the session, those should be minimum times. For more information, check this out — 
+https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
+
+### Get User by Username
+
+To get a user by a username, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_username(username='zuck')
 >>> user
 {
-    "data": {
-        "userData": {
-            "user": {
-                "is_private": false,
-                "profile_pic_url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s150x150&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfANyGvPklT1Hkax6hmmmzvD7QX2vwqYe4XAzZIYo1fGqA&oe=64ACDDC0&_nc_sid=10d13b",
-                "username": "zuck",
-                "hd_profile_pic_versions": [
-                    {
-                        "height": 320,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s320x320&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfCjdM98k9QZZVAr3czL_EjLYje6g__zJ8b_q3ZQi8Uqpw&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 320
-                    },
-                    {
-                        "height": 640,
-                        "url": "https://scontent.cdninstagram.com/v/t51.2885-19/357376107_1330597350674698_8884059223384672080_n.jpg?stp=dst-jpg_s640x640&_nc_ht=scontent.cdninstagram.com&_nc_cat=1&_nc_ohc=9PG1NK-L8OkAX-7KBKu&edm=APs17CUBAAAA&ccb=7-5&oh=00_AfDA1pVfIGaKNihFuUc80xxx8SnNgnqlpvxSCSq9N_n-mQ&oe=64ACDDC0&_nc_sid=10d13b",
-                        "width": 640
-                    }
-                ],
-                "is_verified": true,
-                "biography": "",
-                "biography_with_entities": null,
-                "follower_count": 1988496,
-                "profile_context_facepile_users": null,
-                "bio_links": [
-                    {
-                        "url": ""
-                    }
-                ],
-                "pk": "314216",
-                "full_name": "Mark Zuckerberg",
-                "id": null
-            }
-        }
-    },
-    "extensions": {
-        "is_final": true
-    }
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
+}
+```
+
+### Get User by Identifier
+
+To get a user by an identifier, use the following commands:
+
+```python3
+>>> user = threads.get_user_by_id(id=314216)
+>>> user
+{
+    "pk": 314216,
+    "username": "zuck",
+    "full_name": "Mark Zuckerberg",
+    "is_private": False,
+    "profile_pic_url": HttpUrl('https://scontent-hel3-1.cdninstagram.com/v/t51.2885-19/s150x150/123884060_803537687159702_2508263208740189974_n.jpg?...', scheme='https', host='scontent-hel3-1.cdninstagram.com', tld='com', host_type='domain', ...'),
+    "is_verified": False,
+    "media_count": 102,
+    "follower_count": 576,
+    "following_count": 538,
+    "biography": '',
+    "is_business": False
 }
 ```
 
 ### Get User Threads
 
 To get a user's threads, use the following commands:
 
@@ -639,8 +665,7 @@
         }
     },
     "extensions": {
         "is_final": true
     }
 }
 ```
-
```

