# Comparing `tmp/anitya-telegram-0.0.1.tar.gz` & `tmp/anitya-telegram-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anitya-telegram-0.0.1.tar", last modified: Fri Jun 23 20:27:56 2023, max compression
+gzip compressed data, was "anitya-telegram-0.0.2.tar", last modified: Fri Jul  7 20:13:05 2023, max compression
```

## Comparing `anitya-telegram-0.0.1.tar` & `anitya-telegram-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:27:56.851497 anitya-telegram-0.0.1/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-23 20:27:22.000000 anitya-telegram-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2707 2023-06-23 20:27:56.851497 anitya-telegram-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-23 20:27:22.000000 anitya-telegram-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:27:56.847497 anitya-telegram-0.0.1/anitya_telegram/
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-23 20:27:22.000000 anitya-telegram-0.0.1/anitya_telegram/anitya_tg_gw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:27:56.850497 anitya-telegram-0.0.1/anitya_telegram.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2707 2023-06-23 20:27:56.000000 anitya-telegram-0.0.1/anitya_telegram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-23 20:27:56.000000 anitya-telegram-0.0.1/anitya_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:27:56.000000 anitya-telegram-0.0.1/anitya_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-23 20:27:56.000000 anitya-telegram-0.0.1/anitya_telegram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 20:27:56.000000 anitya-telegram-0.0.1/anitya_telegram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1636 2023-06-23 20:27:22.000000 anitya-telegram-0.0.1/config.toml.example
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-23 20:27:46.000000 anitya-telegram-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:27:56.851497 anitya-telegram-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:13:05.190700 anitya-telegram-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-07 20:12:06.000000 anitya-telegram-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-07 20:13:05.188700 anitya-telegram-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-07-07 20:12:06.000000 anitya-telegram-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:13:05.179699 anitya-telegram-0.0.2/anitya_telegram/
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-07 20:12:06.000000 anitya-telegram-0.0.2/anitya_telegram/anitya_tg_gw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:13:05.185700 anitya-telegram-0.0.2/anitya_telegram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-07 20:13:05.000000 anitya-telegram-0.0.2/anitya_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-07 20:13:05.000000 anitya-telegram-0.0.2/anitya_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:13:05.000000 anitya-telegram-0.0.2/anitya_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-07 20:13:05.000000 anitya-telegram-0.0.2/anitya_telegram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-07 20:13:05.000000 anitya-telegram-0.0.2/anitya_telegram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-07 20:12:06.000000 anitya-telegram-0.0.2/config.toml.example
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-07 20:12:56.000000 anitya-telegram-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 20:13:05.190700 anitya-telegram-0.0.2/setup.cfg
```

### Comparing `anitya-telegram-0.0.1/PKG-INFO` & `anitya-telegram-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anitya-telegram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Telegram gateway for Anitya release monitoring system
 Author-email: mirko <mirko+anitya@smthd.com>
 Project-URL: Homepage, https://gitea.smthd.com/mirko/anitya-telegram
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
@@ -62,9 +62,8 @@
 
 * [Release monitoring](https://release-monitoring.org)
 * [Integrating with Anitya](https://release-monitoring.org/static/docs/integrating-with-anitya.html)
 * [Quick Start](https://fedora-messaging.readthedocs.io/en/latest/user-guide/quick-start.html)
 * [Consumers](https://fedora-messaging.readthedocs.io/en/latest/user-guide/consuming.html)
 * [Using the API](https://fedora-messaging.readthedocs.io/en/latest/tutorial/usage.html)
 * [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
-* [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
 * [Date grepper - anitya.project.version.update.v2](https://apps.fedoraproject.org/datagrepper/v2/search?topic=org.release-monitoring.prod.anitya.project.version.update.v2)
```

### Comparing `anitya-telegram-0.0.1/README.md` & `anitya-telegram-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,9 +50,8 @@
 
 * [Release monitoring](https://release-monitoring.org)
 * [Integrating with Anitya](https://release-monitoring.org/static/docs/integrating-with-anitya.html)
 * [Quick Start](https://fedora-messaging.readthedocs.io/en/latest/user-guide/quick-start.html)
 * [Consumers](https://fedora-messaging.readthedocs.io/en/latest/user-guide/consuming.html)
 * [Using the API](https://fedora-messaging.readthedocs.io/en/latest/tutorial/usage.html)
 * [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
-* [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
 * [Date grepper - anitya.project.version.update.v2](https://apps.fedoraproject.org/datagrepper/v2/search?topic=org.release-monitoring.prod.anitya.project.version.update.v2)
```

### Comparing `anitya-telegram-0.0.1/anitya_telegram/anitya_tg_gw.py` & `anitya-telegram-0.0.2/anitya_telegram/anitya_tg_gw.py`

 * *Files identical despite different names*

### Comparing `anitya-telegram-0.0.1/anitya_telegram.egg-info/PKG-INFO` & `anitya-telegram-0.0.2/anitya_telegram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anitya-telegram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Telegram gateway for Anitya release monitoring system
 Author-email: mirko <mirko+anitya@smthd.com>
 Project-URL: Homepage, https://gitea.smthd.com/mirko/anitya-telegram
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
@@ -62,9 +62,8 @@
 
 * [Release monitoring](https://release-monitoring.org)
 * [Integrating with Anitya](https://release-monitoring.org/static/docs/integrating-with-anitya.html)
 * [Quick Start](https://fedora-messaging.readthedocs.io/en/latest/user-guide/quick-start.html)
 * [Consumers](https://fedora-messaging.readthedocs.io/en/latest/user-guide/consuming.html)
 * [Using the API](https://fedora-messaging.readthedocs.io/en/latest/tutorial/usage.html)
 * [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
-* [fedora-messaging](https://fedora-messaging.readthedocs.io/en/latest/user-guide/cli/fedora-messaging.html)
 * [Date grepper - anitya.project.version.update.v2](https://apps.fedoraproject.org/datagrepper/v2/search?topic=org.release-monitoring.prod.anitya.project.version.update.v2)
```

### Comparing `anitya-telegram-0.0.1/config.toml.example` & `anitya-telegram-0.0.2/config.toml.example`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # fedora-messaging --conf config.toml consume --callback-file anitya_tg_gw.py:TelegramForwardConsumer
 
 amqp_url = "amqps://fedora:@rabbitmq.fedoraproject.org/%2Fpublic_pubsub"
 
 [tls]
-ca_cert = "cacert.pem"
-keyfile = "fedora-key.pem"
-certfile = "fedora-cert.pem"
+ca_cert = "conf/cacert.pem"
+keyfile = "conf/fedora-key.pem"
+certfile = "conf/fedora-cert.pem"
 
 [client_properties]
 app = "Anitya-Telegram Gateway"
 
 [exchanges."amq.topic"]
 type = "topic"
 durable = true
```

### Comparing `anitya-telegram-0.0.1/pyproject.toml` & `anitya-telegram-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anitya-telegram"
-version = "0.0.1"
+version = "0.0.2"
 description = "Telegram gateway for Anitya release monitoring system"
 readme = "README.md"
 authors = [
   { name="mirko", email="mirko+anitya@smthd.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

