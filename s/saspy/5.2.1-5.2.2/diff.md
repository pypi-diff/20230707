# Comparing `tmp/saspy-5.2.1.tar.gz` & `tmp/saspy-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.2.1.tar", last modified: Wed May 31 16:30:52 2023, max compression
+gzip compressed data, was "saspy-5.2.2.tar", last modified: Fri Jul  7 20:04:31 2023, max compression
```

## Comparing `saspy-5.2.1.tar` & `saspy-5.2.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.031150 saspy-5.2.1/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-05-31 16:30:36.000000 saspy-5.2.1/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-05-31 16:30:36.000000 saspy-5.2.1/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-05-31 16:30:52.030150 saspy-5.2.1/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-05-31 16:30:36.000000 saspy-5.2.1/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-05-31 16:30:36.000000 saspy-5.2.1/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.005149 saspy-5.2.1/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.007149 saspy-5.2.1/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.018149 saspy-5.2.1/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.022149 saspy-5.2.1/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.029150 saspy-5.2.1/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   130270 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87007 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87149 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    99717 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.030150 saspy-5.2.1/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-05-31 16:30:36.000000 saspy-5.2.1/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-05-31 16:30:52.006149 saspy-5.2.1/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-05-31 16:30:51.000000 saspy-5.2.1/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-05-31 16:30:51.000000 saspy-5.2.1/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-05-31 16:30:51.000000 saspy-5.2.1/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-05-31 16:30:51.000000 saspy-5.2.1/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-05-31 16:30:51.000000 saspy-5.2.1/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-05-31 16:30:52.031150 saspy-5.2.1/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-05-31 16:30:36.000000 saspy-5.2.1/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.341883 saspy-5.2.2/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-07-07 20:04:15.000000 saspy-5.2.2/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-07-07 20:04:15.000000 saspy-5.2.2/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-07 20:04:31.340883 saspy-5.2.2/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-07-07 20:04:15.000000 saspy-5.2.2/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-07-07 20:04:15.000000 saspy-5.2.2/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.320881 saspy-5.2.2/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.322882 saspy-5.2.2/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.331882 saspy-5.2.2/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.334882 saspy-5.2.2/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.339883 saspy-5.2.2/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   130270 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    87058 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    87201 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    99770 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.340883 saspy-5.2.2/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.321882 saspy-5.2.2/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-07-07 20:04:31.341883 saspy-5.2.2/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-07-07 20:04:15.000000 saspy-5.2.2/setup.py
```

### Comparing `saspy-5.2.1/LICENSE.md` & `saspy-5.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/PKG-INFO` & `saspy-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.2.1
+Version: 5.2.2
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.2.1/README.md` & `saspy-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/SASLogLexer.py` & `saspy-5.2.2/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/__init__.py` & `saspy-5.2.2/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/autocfg.py` & `saspy-5.2.2/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.2.2/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/sas.core.jar` & `saspy-5.2.2/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.2.2/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.2.2/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/pyiom/saspy2j.class` & `saspy-5.2.2/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/pyiom/saspy2j.java` & `saspy-5.2.2/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/saspyiom.jar` & `saspy-5.2.2/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/NOTICE.md` & `saspy-5.2.2/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.2.2/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.2.2/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/libname_gen.sas` & `saspy-5.2.2/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasViyaML.py` & `saspy-5.2.2/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sas_magic.py` & `saspy-5.2.2/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasbase.py` & `saspy-5.2.2/saspy/sasbase.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sascfg.py` & `saspy-5.2.2/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasdata.py` & `saspy-5.2.2/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasdecorator.py` & `saspy-5.2.2/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasets.py` & `saspy-5.2.2/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasexceptions.py` & `saspy-5.2.2/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasiocom.py` & `saspy-5.2.2/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasiohttp.py` & `saspy-5.2.2/saspy/sasiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import os
 import ssl
 import sys
 import urllib
 import warnings
 import io
 import ssl
+import atexit
 
 import tempfile as tf
 from time import sleep
 from threading import Thread
 
 from saspy.sasexceptions import (SASHTTPauthenticateError, SASHTTPconnectionError, SASHTTPsubmissionError)
 
@@ -800,14 +801,16 @@
       if self.sascfg.verbose:
          logger.info("SAS server started using Context "+self.sascfg.ctxname+" with SESSION_ID="+self.pid)
 
       self._refthd = Thread(target=self._refresh_thread, args=())
       self._refthd.daemon = True
       self._refthd.start()
 
+      atexit.register(self._endsas)
+
       return self.pid
 
    def _endsas(self):
       rc = 0
       if self._session:
          # DELETE Session
          conn = self.sascfg.HTTPConn; conn.connect()
```

### Comparing `saspy-5.2.1/saspy/sasioiom.py` & `saspy-5.2.2/saspy/sasioiom.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import subprocess
 from time import sleep
 import socket as socks
 import tempfile as tf
 import codecs
 import warnings
 import io
+import atexit
 
 import logging
 logger = logging.getLogger('saspy')
 
 try:
    import pandas as pd
    import numpy  as np
@@ -555,14 +556,17 @@
          logger.fatal("Attempted to run program "+pgm+" with the following parameters:"+str(parms)+"\n")
          if zero:
             logger.fatal("Be sure the path to sspiauth.dll is in your System PATH"+"\n")
          return None
 
       if self.sascfg.verbose:
          logger.info("SAS Connection established. Subprocess id is "+str(pid)+"\n")
+
+      atexit.register(self._endsas)
+
       return self.pid
 
    def _endsas(self):
       rc = 0
       if self.pid:
          if os.name == 'nt':
             pid = self.pid.pid
```

### Comparing `saspy-5.2.1/saspy/sasiostdio.py` & `saspy-5.2.2/saspy/sasiostdio.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from   time import sleep
 import socket as socks
 import codecs
 import select as sel
 import warnings
 import io
 import re
+import atexit
 
 import logging
 logger = logging.getLogger('saspy')
 
 try:
    import pandas as pd
    import numpy  as np
@@ -486,16 +487,20 @@
             msg += "Try running the following command (where saspy is running) manually to see if you can get more information on what went wrong:\n"+s+"\n"
             logger.error(msg)
             return None
 
       if self.sascfg.verbose:
          pid = self.pid if os.name != 'nt' else self.pid.pid
          logger.info("SAS Connection established. Subprocess id is "+str(pid)+"\n")
+
+      atexit.register(self._endsas)
+
       return self.pid
 
+
    if os.name == 'nt':
       def _read_out(self):
          while True:
             lst = self.pid.stdout.read(4096000)
             if lst == b'':
                break
             self.stdout.put(lst)
```

### Comparing `saspy-5.2.1/saspy/sasml.py` & `saspy-5.2.2/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasproccommons.py` & `saspy-5.2.2/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasqc.py` & `saspy-5.2.2/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasresults.py` & `saspy-5.2.2/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasstat.py` & `saspy-5.2.2/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sastabulate.py` & `saspy-5.2.2/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/sasutil.py` & `saspy-5.2.2/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy/scripts/run_sas.py` & `saspy-5.2.2/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/saspy.egg-info/PKG-INFO` & `saspy-5.2.2/saspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.2.1
+Version: 5.2.2
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.2.1/saspy.egg-info/SOURCES.txt` & `saspy-5.2.2/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.2.1/setup.py` & `saspy-5.2.2/setup.py`

 * *Files identical despite different names*

