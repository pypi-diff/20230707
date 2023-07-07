# Comparing `tmp/vbcore-2.2.0rc2.tar.gz` & `tmp/vbcore-2.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.2.0rc2.tar", last modified: Thu Jul  6 08:50:09 2023, max compression
+gzip compressed data, was "vbcore-2.2.0rc4.tar", last modified: Fri Jul  7 00:26:26 2023, max compression
```

## Comparing `vbcore-2.2.0rc2.tar` & `vbcore-2.2.0rc4.tar`

### file list

```diff
@@ -1,207 +1,210 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.006003 vbcore-2.2.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-06 08:50:09.006003 vbcore-2.2.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.986003 vbcore-2.2.0rc2/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     5007 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:50:09.007003 vbcore-2.2.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.989003 vbcore-2.2.0rc2/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.991003 vbcore-2.2.0rc2/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.991003 vbcore-2.2.0rc2/vbcore/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.991003 vbcore-2.2.0rc2/vbcore/data/transformations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.992003 vbcore-2.2.0rc2/vbcore/data/transformations/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/dicttoxml.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/data/transformations/builders/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.993003 vbcore-2.2.0rc2/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.995003 vbcore-2.2.0rc2/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6774 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/db/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.996003 vbcore-2.2.0rc2/vbcore/dictutils/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/dictutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15787 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/dictutils/flatter_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/dictutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.997003 vbcore-2.2.0rc2/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.997003 vbcore-2.2.0rc2/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.998003 vbcore-2.2.0rc2/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     6516 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.998003 vbcore-2.2.0rc2/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.998003 vbcore-2.2.0rc2/vbcore/net/ftpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/ftpclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/ftpclient/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/ftpclient/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5363 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/net/socks_smtp.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.999003 vbcore-2.2.0rc2/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.999003 vbcore-2.2.0rc2/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/standalone/wsgi_gunicorn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.000003 vbcore-2.2.0rc2/vbcore/stringutils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/stringutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/stringutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/stringutils/notations.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.000003 vbcore-2.2.0rc2/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.001003 vbcore-2.2.0rc2/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.002003 vbcore-2.2.0rc2/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/ftpclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.002003 vbcore-2.2.0rc2/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.004003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.flake8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.004003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.git-hooks/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.004003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.005003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/liccheck.ini
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.005003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.006003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:09.006003 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/entrypoints/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/skel/version.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/tools/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2853 2023-07-06 08:49:58.000000 vbcore-2.2.0rc2/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:50:08.990003 vbcore-2.2.0rc2/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5537 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 08:50:08.000000 vbcore-2.2.0rc2/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.779605 vbcore-2.2.0rc4/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5164 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.783605 vbcore-2.2.0rc4/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.788605 vbcore-2.2.0rc4/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.789605 vbcore-2.2.0rc4/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.791605 vbcore-2.2.0rc4/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6774 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.791605 vbcore-2.2.0rc4/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15787 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.792605 vbcore-2.2.0rc4/vbcore/excel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/excel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/excel/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6516 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.795605 vbcore-2.2.0rc4/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.795605 vbcore-2.2.0rc4/vbcore/net/ftpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6132 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5363 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/socks_smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.796605 vbcore-2.2.0rc4/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.796605 vbcore-2.2.0rc4/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.797605 vbcore-2.2.0rc4/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.798605 vbcore-2.2.0rc4/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.798605 vbcore-2.2.0rc4/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.800605 vbcore-2.2.0rc4/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/ftpclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.800605 vbcore-2.2.0rc4/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.flake8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.804605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/liccheck.ini
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/entrypoints/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.785605 vbcore-2.2.0rc4/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5585 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.2.0rc2/requirements/requirements-all.txt` & `vbcore-2.2.0rc4/requirements/requirements-all.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,18 @@
     # via -r requirements/requirements.txt
 cryptography==41.0.1
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.txt
+et-xmlfile==1.1.0
+    # via
+    #   -r requirements/requirements-extra.txt
+    #   openpyxl
 frozenlist==1.3.3
     # via
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   aiosignal
 gql==3.4.1
     # via -r requirements/requirements-extra.txt
@@ -92,14 +96,16 @@
     # via -r requirements/requirements-extra.txt
 multidict==6.0.4
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   yarl
+openpyxl==3.1.2
+    # via -r requirements/requirements-extra.txt
 paramiko==3.2.0
     # via -r requirements/requirements-net.txt
 ply==3.11
     # via
     #   -r requirements/requirements-extra.txt
     #   rule-engine
 psutil==5.9.5
```

### Comparing `vbcore-2.2.0rc2/requirements/requirements-build.txt` & `vbcore-2.2.0rc4/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-crypto.txt` & `vbcore-2.2.0rc4/requirements/requirements-crypto.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-db.txt` & `vbcore-2.2.0rc4/requirements/requirements-db.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-dev.txt` & `vbcore-2.2.0rc4/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-extra.txt` & `vbcore-2.2.0rc4/requirements/requirements-extra.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,32 @@
     # via jsonschema
 backoff==2.2.1
     # via gql
 chardet==5.1.0
     # via -r requirements/requirements-extra.in
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.in
+et-xmlfile==1.1.0
+    # via openpyxl
 gql==3.4.1
     # via -r requirements/requirements-extra.in
 graphql-core==3.2.3
     # via gql
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.in
 idna==3.4
     # via
     #   -c requirements/requirements-build.txt
     #   yarl
 jsonschema==4.17.3
     # via -r requirements/requirements-extra.in
 multidict==6.0.4
     # via yarl
+openpyxl==3.1.2
+    # via -r requirements/requirements-extra.in
 ply==3.11
     # via rule-engine
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements.txt
```

### Comparing `vbcore-2.2.0rc2/requirements/requirements-http.txt` & `vbcore-2.2.0rc4/requirements/requirements-http.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-net.txt` & `vbcore-2.2.0rc4/requirements/requirements-net.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-scheduler.txt` & `vbcore-2.2.0rc4/requirements/requirements-scheduler.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements-test.txt` & `vbcore-2.2.0rc4/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/requirements/requirements.txt` & `vbcore-2.2.0rc4/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/setup.py` & `vbcore-2.2.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/aio.py` & `vbcore-2.2.0rc4/vbcore/aio.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/base.py` & `vbcore-2.2.0rc4/vbcore/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/batch.py` & `vbcore-2.2.0rc4/vbcore/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/configurator.py` & `vbcore-2.2.0rc4/vbcore/configurator.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/context.py` & `vbcore-2.2.0rc4/vbcore/context.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/crypto/argon.py` & `vbcore-2.2.0rc4/vbcore/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/crypto/base.py` & `vbcore-2.2.0rc4/vbcore/crypto/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/crypto/bcrypt.py` & `vbcore-2.2.0rc4/vbcore/crypto/bcrypt.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/crypto/factory.py` & `vbcore-2.2.0rc4/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/crypto/hashes.py` & `vbcore-2.2.0rc4/vbcore/crypto/hashes.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/csvfile.py` & `vbcore-2.2.0rc4/vbcore/csvfile.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/base.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/csv.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/csv.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/dicttoxml.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/dicttoxml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/factory.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/html.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/html.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/json.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/xml.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/xml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/data/transformations/builders/yaml.py` & `vbcore-2.2.0rc4/vbcore/data/transformations/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/datastruct/buffer.py` & `vbcore-2.2.0rc4/vbcore/datastruct/buffer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/datastruct/cache.py` & `vbcore-2.2.0rc4/vbcore/datastruct/cache.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/datastruct/dictionaries.py` & `vbcore-2.2.0rc4/vbcore/datastruct/dictionaries.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/datastruct/lazy.py` & `vbcore-2.2.0rc4/vbcore/datastruct/lazy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/datastruct/orderer_set.py` & `vbcore-2.2.0rc4/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/date_helper.py` & `vbcore-2.2.0rc4/vbcore/date_helper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/events.py` & `vbcore-2.2.0rc4/vbcore/db/events.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/exceptions.py` & `vbcore-2.2.0rc4/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/listener.py` & `vbcore-2.2.0rc4/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/mixins.py` & `vbcore-2.2.0rc4/vbcore/db/mixins.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/mysql_dumper.py` & `vbcore-2.2.0rc4/vbcore/db/mysql_dumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/schema.py` & `vbcore-2.2.0rc4/vbcore/db/schema.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/sqla.py` & `vbcore-2.2.0rc4/vbcore/db/sqla.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/support.py` & `vbcore-2.2.0rc4/vbcore/db/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/db/views.py` & `vbcore-2.2.0rc4/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/dictutils/flatter_dict.py` & `vbcore-2.2.0rc4/vbcore/dictutils/flatter_dict.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/dispatcher.py` & `vbcore-2.2.0rc4/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/enums.py` & `vbcore-2.2.0rc4/vbcore/enums.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/exceptions.py` & `vbcore-2.2.0rc4/vbcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/factory.py` & `vbcore-2.2.0rc4/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/files.py` & `vbcore-2.2.0rc4/vbcore/files.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/batch.py` & `vbcore-2.2.0rc4/vbcore/http/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/client.py` & `vbcore-2.2.0rc4/vbcore/http/client.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/gql.py` & `vbcore-2.2.0rc4/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/headers.py` & `vbcore-2.2.0rc4/vbcore/http/headers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/httpcode.py` & `vbcore-2.2.0rc4/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/httpdumper.py` & `vbcore-2.2.0rc4/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/proxy.py` & `vbcore-2.2.0rc4/vbcore/http/proxy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/rpc.py` & `vbcore-2.2.0rc4/vbcore/http/rpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/http/useragent.py` & `vbcore-2.2.0rc4/vbcore/http/useragent.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/importer.py` & `vbcore-2.2.0rc4/vbcore/importer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/json.py` & `vbcore-2.2.0rc4/vbcore/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.2.0rc4/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/jsonschema/support.py` & `vbcore-2.2.0rc4/vbcore/jsonschema/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/lambdas.py` & `vbcore-2.2.0rc4/vbcore/lambdas.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/loggers.py` & `vbcore-2.2.0rc4/vbcore/loggers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/misc.py` & `vbcore-2.2.0rc4/vbcore/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/net/ftpclient/legacy.py` & `vbcore-2.2.0rc4/vbcore/net/ftpclient/legacy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/net/ftpclient/sftp.py` & `vbcore-2.2.0rc4/vbcore/net/ftpclient/sftp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/net/helpers.py` & `vbcore-2.2.0rc4/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/net/sendmail.py` & `vbcore-2.2.0rc4/vbcore/net/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/net/socks_smtp.py` & `vbcore-2.2.0rc4/vbcore/net/socks_smtp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/rule_engine/base.py` & `vbcore-2.2.0rc4/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/rule_engine/engine.py` & `vbcore-2.2.0rc4/vbcore/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/standalone/scheduler.py` & `vbcore-2.2.0rc4/vbcore/standalone/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.2.0rc4/vbcore/standalone/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/stringutils/misc.py` & `vbcore-2.2.0rc4/vbcore/stringutils/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/stringutils/notations.py` & `vbcore-2.2.0rc4/vbcore/stringutils/notations.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/system.py` & `vbcore-2.2.0rc4/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tester/asserter.py` & `vbcore-2.2.0rc4/vbcore/tester/asserter.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tester/fetchmail.py` & `vbcore-2.2.0rc4/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tester/helpers.py` & `vbcore-2.2.0rc4/vbcore/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tester/http.py` & `vbcore-2.2.0rc4/vbcore/tester/http.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/cli.py` & `vbcore-2.2.0rc4/vbcore/tools/cli.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/crypto.py` & `vbcore-2.2.0rc4/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/database.py` & `vbcore-2.2.0rc4/vbcore/tools/database.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/entrypoint.py` & `vbcore-2.2.0rc4/vbcore/tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/ftpclient.py` & `vbcore-2.2.0rc4/vbcore/tools/ftpclient.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/init.py` & `vbcore-2.2.0rc4/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.gitignore` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.gitignore`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/.pylintrc` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.pylintrc`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/Makefile` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/README.md` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/README.md`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/liccheck.ini` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/liccheck.ini`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/initializer/skeleton/setup.py` & `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/scheduler.py` & `vbcore-2.2.0rc4/vbcore/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/sendmail.py` & `vbcore-2.2.0rc4/vbcore/tools/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/tools/wsgi_gunicorn.py` & `vbcore-2.2.0rc4/vbcore/tools/wsgi_gunicorn.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 @CliOpt.string("-u", "--user", envvar="GU_USER", default=os.geteuid())
 @CliOpt.string("-g", "--group", envvar="GU_GROUP", default=os.getegid())
 @CliOpt.string("--worker-class", envvar="GU_WORKER_CLASS")
 @CliOpt.choice(
     "-W",
     "--worker-type",
     envvar="GU_WORKER_TYPE",
-    values=WorkerType.items(),
-    default=WorkerType.DEFAULT.name,
+    default="DEFAULT",
+    values=["DEFAULT", "UVICORN", "MEINHELD"],
     callback=lambda _, __, x: WorkerType(x.upper()),
     case_sensitive=False,
 )
 def main(**kwargs):
     """start the gunicorn server"""
     server = GUnicornServer(**kwargs)
     server.run_forever()
```

### Comparing `vbcore-2.2.0rc2/vbcore/types.py` & `vbcore-2.2.0rc4/vbcore/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore/yaml.py` & `vbcore-2.2.0rc4/vbcore/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc2/vbcore.egg-info/SOURCES.txt` & `vbcore-2.2.0rc4/vbcore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 vbcore/db/schema.py
 vbcore/db/sqla.py
 vbcore/db/support.py
 vbcore/db/views.py
 vbcore/dictutils/__init__.py
 vbcore/dictutils/flatter_dict.py
 vbcore/dictutils/misc.py
+vbcore/excel/__init__.py
+vbcore/excel/report.py
 vbcore/http/__init__.py
 vbcore/http/batch.py
 vbcore/http/client.py
 vbcore/http/gql.py
 vbcore/http/headers.py
 vbcore/http/httpcode.py
 vbcore/http/httpdumper.py
```

### Comparing `vbcore-2.2.0rc2/vbcore.egg-info/requires.txt` & `vbcore-2.2.0rc4/vbcore.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 chardet
 jsonschema
 rule_engine
 gql
 gunicorn
 defusedxml
 xmltodict
+openpyxl
 
 [crypto]
 argon2-cffi
 bcrypt
 
 [db]
 sqlalchemy
@@ -44,14 +45,15 @@
 chardet
 jsonschema
 rule_engine
 gql
 gunicorn
 defusedxml
 xmltodict
+openpyxl
 
 [http]
 aiohttp
 requests
 user_agents
 
 [net]
```

