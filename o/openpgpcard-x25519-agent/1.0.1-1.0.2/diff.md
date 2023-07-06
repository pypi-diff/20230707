# Comparing `tmp/openpgpcard-x25519-agent-1.0.1.tar.gz` & `tmp/openpgpcard-x25519-agent-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpgpcard-x25519-agent-1.0.1.tar", last modified: Tue May  9 21:27:03 2023, max compression
+gzip compressed data, was "openpgpcard-x25519-agent-1.0.2.tar", last modified: Thu Jul  6 22:16:52 2023, max compression
```

## Comparing `openpgpcard-x25519-agent-1.0.1.tar` & `openpgpcard-x25519-agent-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/
--rw-rw-r--   0 justin    (1000) justin    (1000)      260 2023-05-09 21:16:06.000000 openpgpcard-x25519-agent-1.0.1/.build.yml
--rw-r--r--   0 justin    (1000) justin    (1000)      420 2023-02-08 06:25:10.000000 openpgpcard-x25519-agent-1.0.1/.editorconfig
--rw-rw-r--   0 justin    (1000) justin    (1000)      566 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.1/.gitignore
--rw-rw-r--   0 justin    (1000) justin    (1000)     1771 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 justin    (1000) justin    (1000)    32473 2023-02-08 06:26:50.000000 openpgpcard-x25519-agent-1.0.1/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     3679 2023-03-13 20:44:52.000000 openpgpcard-x25519-agent-1.0.1/README.md
--rw-rw-r--   0 justin    (1000) justin    (1000)      607 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.1/coveragerc
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.560903 openpgpcard-x25519-agent-1.0.1/etc/
--rw-rw-r--   0 justin    (1000) justin    (1000)     2356 2023-03-04 23:50:44.000000 openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.service
--rw-rw-r--   0 justin    (1000) justin    (1000)      246 2023-03-05 02:52:53.000000 openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.socket
--rwxrwxr-x   0 justin    (1000) justin    (1000)     1435 2023-03-05 03:10:33.000000 openpgpcard-x25519-agent-1.0.1/install.sh
--rw-rw-r--   0 justin    (1000) justin    (1000)      254 2023-02-08 01:50:04.000000 openpgpcard-x25519-agent-1.0.1/pyproject.toml
--rw-rw-r--   0 justin    (1000) justin    (1000)     2157 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)      557 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.1/setup.py
--rw-rw-r--   0 justin    (1000) justin    (1000)      404 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/spellcheck-dictionary.txt
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.556900 openpgpcard-x25519-agent-1.0.1/src/
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      466 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    14520 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/card.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2487 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    11252 2023-02-28 02:42:11.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4980 2023-02-28 02:56:43.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client_cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1748 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    28646 2023-03-03 23:17:32.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/msg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    12987 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/server.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/
--rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     1027 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      148 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-02-08 01:29:53.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/not-zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)      141 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       25 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/top_level.txt
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/tests/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1332 2023-02-16 05:43:01.000000 openpgpcard-x25519-agent-1.0.1/tests/conftest.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    15254 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/tests/test_card.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    17671 2023-02-28 02:36:18.000000 openpgpcard-x25519-agent-1.0.1/tests/test_client.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3225 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tests/test_cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    23775 2023-02-28 02:10:34.000000 openpgpcard-x25519-agent-1.0.1/tests/test_msg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    16878 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tests/test_server.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1885 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tox.ini
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.295357 openpgpcard-x25519-agent-1.0.2/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      260 2023-07-06 22:01:28.000000 openpgpcard-x25519-agent-1.0.2/.build.yml
+-rw-r--r--   0 justin    (1000) justin    (1000)      420 2023-02-08 06:25:10.000000 openpgpcard-x25519-agent-1.0.2/.editorconfig
+-rw-rw-r--   0 justin    (1000) justin    (1000)      566 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.2/.gitignore
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1771 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 justin    (1000) justin    (1000)    32473 2023-02-08 06:26:50.000000 openpgpcard-x25519-agent-1.0.2/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-07-06 22:16:52.295357 openpgpcard-x25519-agent-1.0.2/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3679 2023-03-13 20:44:52.000000 openpgpcard-x25519-agent-1.0.2/README.md
+-rw-rw-r--   0 justin    (1000) justin    (1000)      607 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.2/coveragerc
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.287344 openpgpcard-x25519-agent-1.0.2/etc/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2356 2023-03-04 23:50:44.000000 openpgpcard-x25519-agent-1.0.2/etc/openpgpcard-x25519-agent.service
+-rw-rw-r--   0 justin    (1000) justin    (1000)      246 2023-03-05 02:52:53.000000 openpgpcard-x25519-agent-1.0.2/etc/openpgpcard-x25519-agent.socket
+-rwxrwxr-x   0 justin    (1000) justin    (1000)     1435 2023-03-05 03:10:33.000000 openpgpcard-x25519-agent-1.0.2/install.sh
+-rw-rw-r--   0 justin    (1000) justin    (1000)      254 2023-02-08 01:50:04.000000 openpgpcard-x25519-agent-1.0.2/pyproject.toml
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2157 2023-07-06 22:16:52.295357 openpgpcard-x25519-agent-1.0.2/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)      557 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.2/setup.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)      404 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.2/spellcheck-dictionary.txt
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.283337 openpgpcard-x25519-agent-1.0.2/src/
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.291350 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      466 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    14592 2023-07-06 22:01:32.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/card.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2487 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    11252 2023-02-28 02:42:11.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/client.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4980 2023-02-28 02:56:43.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/client_cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1748 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    28646 2023-03-03 23:17:32.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/msg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    12987 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/server.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.291350 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1027 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      148 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-07-06 22:16:42.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)      141 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       25 2023-07-06 22:16:52.000000 openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/top_level.txt
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-07-06 22:16:52.295357 openpgpcard-x25519-agent-1.0.2/tests/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1332 2023-02-16 05:43:01.000000 openpgpcard-x25519-agent-1.0.2/tests/conftest.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    15158 2023-07-06 22:01:32.000000 openpgpcard-x25519-agent-1.0.2/tests/test_card.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    17671 2023-02-28 02:36:18.000000 openpgpcard-x25519-agent-1.0.2/tests/test_client.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3225 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.2/tests/test_cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    23775 2023-02-28 02:10:34.000000 openpgpcard-x25519-agent-1.0.2/tests/test_msg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    16878 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.2/tests/test_server.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1885 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.2/tox.ini
```

### Comparing `openpgpcard-x25519-agent-1.0.1/.gitignore` & `openpgpcard-x25519-agent-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/.pre-commit-config.yaml` & `openpgpcard-x25519-agent-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/LICENSE` & `openpgpcard-x25519-agent-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/PKG-INFO` & `openpgpcard-x25519-agent-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpgpcard-x25519-agent
-Version: 1.0.1
+Version: 1.0.2
 Summary: Socket interface to Curve25519 ECDH from an OpenPGP card.
 Home-page: https://git.sr.ht/~arx10/openpgpcard-x25519-agent
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: GPL-3.0-or-later
 Project-URL: Mailing List, https://lists.sr.ht/~arx10/openpgpcard-x25519-agent
 Project-URL: Source, https://git.sr.ht/~arx10/openpgpcard-x25519-agent
```

### Comparing `openpgpcard-x25519-agent-1.0.1/README.md` & `openpgpcard-x25519-agent-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/coveragerc` & `openpgpcard-x25519-agent-1.0.2/coveragerc`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.service` & `openpgpcard-x25519-agent-1.0.2/etc/openpgpcard-x25519-agent.service`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/install.sh` & `openpgpcard-x25519-agent-1.0.2/install.sh`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/setup.cfg` & `openpgpcard-x25519-agent-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/setup.py` & `openpgpcard-x25519-agent-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/card.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Card utilities."""
 
-from base64 import b64encode
+from base64 import b64decode, b64encode
 from getpass import getpass
 from logging import getLogger
 
 from OpenPGPpy import (
     ConnectionException,
     DataException,
     OpenPGPcard,
@@ -65,14 +65,16 @@
     0x6B00: "wrong parameters",
     0x6D00: "instruction code not supported",
     0x6E00: "class not supported",
     0x6F00: "no precise diagnosis",
     0x9000: "command correct",
 }
 
+EXAMPLE_KEY = b64decode("xTIBA5rboUvnH4htodjb6e697QjLERt1NAB4mZqp8Dg=")
+
 
 def count_all_cards():
     """Number of cards.
 
     Returns:
         int: Count of cards.
     """
@@ -345,15 +347,15 @@
     card = get_card_by_id(card_id) if card_id else get_default_card()
 
     # print info to stdout
     print(format_card_info(card))  # noqa: T201
     print("Enter card user PIN: ")  # noqa: T201
     pin = getpass("").encode()
 
-    calculate_shared_secret(card, bytearray(b"\xff" * 32), pin)
+    calculate_shared_secret(card, EXAMPLE_KEY, pin)
 
 
 def get_key_type(card, slot=ENCRYPTION_SLOT):
     """Type of key in the specified slot of the specified card.
 
     Arguments:
         card (OpenPGPcard): Card.
```

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cli.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/cli.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/client.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client_cli.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/client_cli.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cnf.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/cnf.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/msg.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/msg.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/server.py` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent/server.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/PKG-INFO` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpgpcard-x25519-agent
-Version: 1.0.1
+Version: 1.0.2
 Summary: Socket interface to Curve25519 ECDH from an OpenPGP card.
 Home-page: https://git.sr.ht/~arx10/openpgpcard-x25519-agent
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: GPL-3.0-or-later
 Project-URL: Mailing List, https://lists.sr.ht/~arx10/openpgpcard-x25519-agent
 Project-URL: Source, https://git.sr.ht/~arx10/openpgpcard-x25519-agent
```

### Comparing `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt` & `openpgpcard-x25519-agent-1.0.2/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/conftest.py` & `openpgpcard-x25519-agent-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/test_card.py` & `openpgpcard-x25519-agent-1.0.2/tests/test_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 EXAMPLE_KEY_HEX = "C53201039ADBA14BE71F886DA1D8DBE9EEBDED08CB111B75340078999AA9F038"
 EXAMPLE_KEY_64 = "xTIBA5rboUvnH4htodjb6e697QjLERt1NAB4mZqp8Dg="
 
 DECIPHER_KEY_COMMAND_PREFIX = "002A8086 27 A6 25 7F49 22 86 20"
 DECIPHER_EXAMPLE_KEY_COMMAND = list(
     bytes.fromhex(f"{DECIPHER_KEY_COMMAND_PREFIX} {EXAMPLE_KEY_HEX}")
 )
-DECIPHER_TEST_CARD_COMMAND = list(bytes.fromhex(DECIPHER_KEY_COMMAND_PREFIX)) + (
-    [0xFF] * 32
-)
 
 
 def test_count_all_cards_when_none(all_cards_mock):
     assert count_all_cards() == 0
 
 
 def test_count_all_cards_when_multiple(five_cards_mock):
@@ -272,17 +269,17 @@
         ([], 0x90, 0x00),
         (b"test", 0x90, 0x00),
     )
 
     cli_test_card()
 
     assert sent == [
-        DECIPHER_TEST_CARD_COMMAND,
+        DECIPHER_EXAMPLE_KEY_COMMAND,
         [0, 0x20, 0, 0x82, 3, 0x66, 0x6F, 0x6F],
-        DECIPHER_TEST_CARD_COMMAND,
+        DECIPHER_EXAMPLE_KEY_COMMAND,
     ]
 
 
 def test_get_key_type_when_app_data_missing():
     card = MagicMock()
     card.get_application_data.return_value = {}
```

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/test_client.py` & `openpgpcard-x25519-agent-1.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/test_cnf.py` & `openpgpcard-x25519-agent-1.0.2/tests/test_cnf.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/test_msg.py` & `openpgpcard-x25519-agent-1.0.2/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tests/test_server.py` & `openpgpcard-x25519-agent-1.0.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.1/tox.ini` & `openpgpcard-x25519-agent-1.0.2/tox.ini`

 * *Files identical despite different names*

