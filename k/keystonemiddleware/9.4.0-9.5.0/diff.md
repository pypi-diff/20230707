# Comparing `tmp/keystonemiddleware-9.4.0.tar.gz` & `tmp/keystonemiddleware-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystonemiddleware-9.4.0.tar", last modified: Wed Feb 16 18:49:38 2022, max compression
+gzip compressed data, was "keystonemiddleware-9.5.0.tar", last modified: Fri May 20 12:33:03 2022, max compression
```

## Comparing `keystonemiddleware-9.4.0.tar` & `keystonemiddleware-9.5.0.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.886717 keystonemiddleware-9.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7805 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45718 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11900 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2022-02-16 18:49:38.886717 keystonemiddleware-9.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/config-generator/keystonemiddleware.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/ext/apidoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/audit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7780 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48742 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/images/audit.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/images/graphs_authComp.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/images/graphs_authCompDelegate.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12511 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/doc/source/middlewarearchitecture.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.862717 keystonemiddleware-9.4.0/keystonemiddleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.866717 keystonemiddleware-9.4.0/keystonemiddleware/_common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/_common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5789 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/_common/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.866717 keystonemiddleware-9.4.0/keystonemiddleware/audit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7510 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/audit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12568 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/audit/_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/audit/_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37618 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12627 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7395 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_memcache_crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11791 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8889 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_user_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/ec2_token.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/echo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/echo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/echo/__main__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/echo/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.854717 keystonemiddleware-9.4.0/keystonemiddleware/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.854717 keystonemiddleware-9.4.0/keystonemiddleware/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2057 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/keystonemiddleware.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.854717 keystonemiddleware-9.4.0/keystonemiddleware/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/keystonemiddleware.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9532 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/s3_token.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.870717 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3049 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20183 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8956 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4529 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_oslo_messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_logging_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.874717 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3962 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84331 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_auth_token_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7824 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_base_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6564 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5163 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4703 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_connection_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3336 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_memcache_crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9930 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6198 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_user_auth_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19346 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/client_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6985 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_ec2_token_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_entry_points.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10208 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_s3_token_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5845 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.866717 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6364 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-02-16 18:49:38.000000 keystonemiddleware-9.4.0/keystonemiddleware.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.858717 keystonemiddleware-9.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/allow-expired-5ddbabcffc5678af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/authprotocol-accepts-oslo-config-config-a37212b60f58e154.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bp-whitelist-extension-for-app-creds-badf088c8ad584bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1490804-87c0ff8e764945c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1544840-a534127f8663e40f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1583690-da67472d7afff0bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1583699-dba4fe6c057e2be5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1583702-a4469dc1556878b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1649735-3c68f3243e474775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1677308-a2fa7de67f21cd84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1695038-2cbedcabf8ecc057.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1737115-fa3d41e3d3cd7177.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1737119-4afe548d28fbf8bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1747655-6e563d9317bb0f13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1762362-3d092b15c7bab3a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1766731-3b29192cfeb77964.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1782404-c4e37bbc83756a89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1789351-102e2e5119be38b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1800017-0e5a9b8f62b5ca60.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1803940-9a39c66014763af0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1809101-6b5088443d5970ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug-1813739-80eae72371903119.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/bug_1540115-677cf5016bc46348.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/change-default-identity-endpoint-fab39579255c31bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/delay_auth_instead_of_503-f9b46bf4fbc11455.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/deprecate-caching-tokens-in-process-a412b0f1dea84cb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/deprecate-eventlet-unsafe-memcacheclientpool-f8b4a6733513d73e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/drop-py-2-7-6655f421a9cac0a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/ec2-v2-removal-6a886210cbc9d3e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/fix-audit-no-service-endpoint-ports-72b2009d631dcf19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/interface-option-ed551d2a3162668d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/ksm_4.1.0-3cd78446d8e63616.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/remove_kwargs_to_fetch_token-20e3451ed192ab6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/removed-as-of-ussuri-4e1ea485ba8801c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/rename-auth-uri-d223d883f5898aee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/s3token_auth_uri-490c1287d90b9df7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/notes/x-is-admin-project-header-97f1882e209fe727.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.858717 keystonemiddleware-9.4.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.858717 keystonemiddleware-9.4.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30832 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.858717 keystonemiddleware-9.4.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.882717 keystonemiddleware-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.858717 keystonemiddleware-9.4.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-16 18:49:38.886717 keystonemiddleware-9.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2022-02-16 18:49:38.886717 keystonemiddleware-9.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2022-02-16 18:49:03.000000 keystonemiddleware-9.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.178202 keystonemiddleware-9.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7844 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45903 2022-05-20 12:33:02.000000 keystonemiddleware-9.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11900 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2599 2022-05-20 12:33:03.178202 keystonemiddleware-9.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/config-generator/keystonemiddleware.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/ext/apidoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/audit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7780 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48742 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/images/audit.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/images/graphs_authComp.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/images/graphs_authCompDelegate.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12511 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/doc/source/middlewarearchitecture.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/keystonemiddleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/keystonemiddleware/_common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/_common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5789 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/_common/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/keystonemiddleware/audit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7508 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/audit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12568 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/audit/_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/audit/_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37618 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12627 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7395 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_memcache_crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11791 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8889 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_user_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/ec2_token.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/echo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/echo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/echo/__main__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/echo/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/keystonemiddleware/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/keystonemiddleware/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2057 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/keystonemiddleware.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/keystonemiddleware/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/keystonemiddleware.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9532 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/s3_token.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.166194 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3049 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20183 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8956 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4529 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_oslo_messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_logging_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.170197 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3962 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    84331 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_auth_token_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7824 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_base_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6564 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5163 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4703 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_connection_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3336 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_memcache_crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9930 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6198 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_user_auth_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19346 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/client_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6985 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_ec2_token_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_entry_points.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10208 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_s3_token_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5845 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.162191 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2599 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6371 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-05-20 12:33:03.000000 keystonemiddleware-9.5.0/keystonemiddleware.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.174199 keystonemiddleware-9.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/allow-expired-5ddbabcffc5678af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/authprotocol-accepts-oslo-config-config-a37212b60f58e154.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bp-whitelist-extension-for-app-creds-badf088c8ad584bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1490804-87c0ff8e764945c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1544840-a534127f8663e40f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1583690-da67472d7afff0bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1583699-dba4fe6c057e2be5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1583702-a4469dc1556878b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1649735-3c68f3243e474775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1677308-a2fa7de67f21cd84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1695038-2cbedcabf8ecc057.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1737115-fa3d41e3d3cd7177.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1737119-4afe548d28fbf8bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1747655-6e563d9317bb0f13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1762362-3d092b15c7bab3a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1766731-3b29192cfeb77964.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1782404-c4e37bbc83756a89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1789351-102e2e5119be38b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1800017-0e5a9b8f62b5ca60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1803940-9a39c66014763af0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1809101-6b5088443d5970ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug-1813739-80eae72371903119.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/bug_1540115-677cf5016bc46348.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/change-default-identity-endpoint-fab39579255c31bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/delay_auth_instead_of_503-f9b46bf4fbc11455.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/deprecate-caching-tokens-in-process-a412b0f1dea84cb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/deprecate-eventlet-unsafe-memcacheclientpool-f8b4a6733513d73e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/drop-py-2-7-6655f421a9cac0a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/ec2-v2-removal-6a886210cbc9d3e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/fix-audit-no-service-endpoint-ports-72b2009d631dcf19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/interface-option-ed551d2a3162668d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/ksm_4.1.0-3cd78446d8e63616.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/remove_kwargs_to_fetch_token-20e3451ed192ab6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/removed-as-of-ussuri-4e1ea485ba8801c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/rename-auth-uri-d223d883f5898aee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/s3token_auth_uri-490c1287d90b9df7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/notes/x-is-admin-project-header-97f1882e209fe727.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.174199 keystonemiddleware-9.5.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.174199 keystonemiddleware-9.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.174199 keystonemiddleware-9.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.174199 keystonemiddleware-9.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30832 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.178202 keystonemiddleware-9.5.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.158189 keystonemiddleware-9.5.0/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-20 12:33:03.178202 keystonemiddleware-9.5.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2022-05-20 12:33:03.178202 keystonemiddleware-9.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2022-05-20 12:32:24.000000 keystonemiddleware-9.5.0/tox.ini
```

### Comparing `keystonemiddleware-9.4.0/AUTHORS` & `keystonemiddleware-9.5.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 Shevek <shevek@nebula.com>
 Spencer Yu <yushb@gohighsec.com>
 Stefan Nica <snica@suse.com>
 Steve Martinelli <s.martinelli@gmail.com>
 Steve Martinelli <stevemar@ca.ibm.com>
 Steven Hardy <shardy@redhat.com>
 Stuart McLaren <stuart.mclaren@hp.com>
+Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Thomas Goirand <thomas@goirand.fr>
 Thomas Goirand <zigo@debian.org>
 Thomas Herve <therve@redhat.com>
 Thomas Herve <thomas.herve@enovance.com>
 Tim Burke <tim.burke@gmail.com>
 Tin Lam <tin@irrational.io>
```

### Comparing `keystonemiddleware-9.4.0/CONTRIBUTING.rst` & `keystonemiddleware-9.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/ChangeLog` & `keystonemiddleware-9.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 CHANGES
 =======
 
+9.5.0
+-----
+
+* Drop lower-constraints.txt and its testing
+* Update master for stable/yoga
+
 9.4.0
 -----
 
 * Update master for stable/xena
+* Add Python 3 only classifier
 * Update master for stable/wallaby
 * Update master for stable/victoria
+* Add oslo.config.opts entrypoint for audit middleware options
 
 9.3.0
 -----
 
 * Imported Translations from Zanata
 * Switch to eventlet-safe oslo.cache's MemcacheClientPool
 * Updating lower-constraints job as non voting
```

### Comparing `keystonemiddleware-9.4.0/HACKING.rst` & `keystonemiddleware-9.5.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/LICENSE` & `keystonemiddleware-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/PKG-INFO` & `keystonemiddleware-9.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystonemiddleware
-Version: 9.4.0
+Version: 9.5.0
 Summary: Middleware for OpenStack Identity
 Home-page: https://docs.openstack.org/keystonemiddleware/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -48,12 +48,13 @@
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: audit_notifications
 Provides-Extra: test
```

### Comparing `keystonemiddleware-9.4.0/README.rst` & `keystonemiddleware-9.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/Makefile` & `keystonemiddleware-9.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/ext/apidoc.py` & `keystonemiddleware-9.5.0/doc/ext/apidoc.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/requirements.txt` & `keystonemiddleware-9.5.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/audit.rst` & `keystonemiddleware-9.5.0/doc/source/audit.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/conf.py` & `keystonemiddleware-9.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/images/audit.png` & `keystonemiddleware-9.5.0/doc/source/images/audit.png`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/images/graphs_authComp.svg` & `keystonemiddleware-9.5.0/doc/source/images/graphs_authComp.svg`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/images/graphs_authCompDelegate.svg` & `keystonemiddleware-9.5.0/doc/source/images/graphs_authCompDelegate.svg`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/index.rst` & `keystonemiddleware-9.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/installation.rst` & `keystonemiddleware-9.5.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/doc/source/middlewarearchitecture.rst` & `keystonemiddleware-9.5.0/doc/source/middlewarearchitecture.rst`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/_common/config.py` & `keystonemiddleware-9.5.0/keystonemiddleware/_common/config.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/audit/__init__.py` & `keystonemiddleware-9.5.0/keystonemiddleware/audit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     https://docs.openstack.org/keystonemiddleware/latest/audit.html
     """
 
     def __init__(self, app, **conf):
         self._application = app
         self._conf = config.Config('audit',
                                    AUDIT_MIDDLEWARE_GROUP,
-                                   _list_opts(),
+                                   list_opts(),
                                    conf)
         global _LOG
         _LOG = logging.getLogger(conf.get('log_name', __name__))
         self._service_name = conf.get('service_name')
         self._ignore_req_list = [x.upper().strip() for x in
                                  conf.get('ignore_req_list', '').split(',')]
         self._cadf_audit = _api.OpenStackAuditApi(conf.get('audit_map_file'),
@@ -161,15 +161,15 @@
             self._process_response(req)
             raise
         else:
             self._process_response(req, response)
         return response
 
 
-def _list_opts():
+def list_opts():
     """Return a list of oslo_config options available in audit middleware.
 
     The returned list includes all oslo_config options which may be registered
     at runtime by the project.
 
     Each element of the list is a tuple. The first element is the name of the
     group under which the list of elements in the second element will be
```

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/audit/_api.py` & `keystonemiddleware-9.5.0/keystonemiddleware/audit/_api.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/audit/_notifier.py` & `keystonemiddleware-9.5.0/keystonemiddleware/audit/_notifier.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/__init__.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/__init__.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_auth.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_auth.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_base.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_base.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_cache.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_cache.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_exceptions.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_exceptions.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_identity.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_identity.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_memcache_crypt.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_memcache_crypt.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_opts.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_opts.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_request.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_request.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/auth_token/_user_plugin.py` & `keystonemiddleware-9.5.0/keystonemiddleware/auth_token/_user_plugin.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/ec2_token.py` & `keystonemiddleware-9.5.0/keystonemiddleware/ec2_token.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/echo/service.py` & `keystonemiddleware-9.5.0/keystonemiddleware/echo/service.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/exceptions.py` & `keystonemiddleware-9.5.0/keystonemiddleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/fixture.py` & `keystonemiddleware-9.5.0/keystonemiddleware/fixture.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/i18n.py` & `keystonemiddleware-9.5.0/keystonemiddleware/i18n.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/keystonemiddleware.po` & `keystonemiddleware-9.5.0/keystonemiddleware/locale/en_GB/LC_MESSAGES/keystonemiddleware.po`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/keystonemiddleware.po` & `keystonemiddleware-9.5.0/keystonemiddleware/locale/ko_KR/LC_MESSAGES/keystonemiddleware.po`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/opts.py` & `keystonemiddleware-9.5.0/keystonemiddleware/opts.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/s3_token.py` & `keystonemiddleware-9.5.0/keystonemiddleware/s3_token.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/base.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/base.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_api.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_api.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_middleware.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_middleware.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_audit_oslo_messaging.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_audit_oslo_messaging.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/audit/test_logging_notifier.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/audit/test_logging_notifier.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/base.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/base.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_auth.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_auth.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_auth_token_middleware.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_auth_token_middleware.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_base_middleware.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_base_middleware.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_cache.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_cache.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_config.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_config.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_connection_pool.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_memcache_crypt.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_memcache_crypt.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_request.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_request.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/auth_token/test_user_auth_plugin.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/auth_token/test_user_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/client_fixtures.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_access_rules.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_access_rules.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_ec2_token_middleware.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_ec2_token_middleware.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_entry_points.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_fixtures.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_opts.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/test_s3_token_middleware.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/test_s3_token_middleware.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware/tests/unit/utils.py` & `keystonemiddleware-9.5.0/keystonemiddleware/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware.egg-info/PKG-INFO` & `keystonemiddleware-9.5.0/keystonemiddleware.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystonemiddleware
-Version: 9.4.0
+Version: 9.5.0
 Summary: Middleware for OpenStack Identity
 Home-page: https://docs.openstack.org/keystonemiddleware/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -48,12 +48,13 @@
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: audit_notifications
 Provides-Extra: test
```

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware.egg-info/SOURCES.txt` & `keystonemiddleware-9.5.0/keystonemiddleware.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 HACKING.rst
 LICENSE
 README.rst
 babel.cfg
-lower-constraints.txt
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 config-generator/keystonemiddleware.conf
 doc/.gitignore
@@ -139,12 +138,13 @@
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
+releasenotes/source/yoga.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
 releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
 releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
 releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
```

### Comparing `keystonemiddleware-9.4.0/keystonemiddleware.egg-info/requires.txt` & `keystonemiddleware-9.5.0/keystonemiddleware.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/allow-expired-5ddbabcffc5678af.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/allow-expired-5ddbabcffc5678af.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/bug-1490804-87c0ff8e764945c1.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/bug-1490804-87c0ff8e764945c1.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/bug-1649735-3c68f3243e474775.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/bug-1649735-3c68f3243e474775.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/bug-1677308-a2fa7de67f21cd84.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/bug-1677308-a2fa7de67f21cd84.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/bug-1695038-2cbedcabf8ecc057.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/bug-1695038-2cbedcabf8ecc057.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/deprecate-caching-tokens-in-process-a412b0f1dea84cb9.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/deprecate-caching-tokens-in-process-a412b0f1dea84cb9.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/notes/deprecate-eventlet-unsafe-memcacheclientpool-f8b4a6733513d73e.yaml` & `keystonemiddleware-9.5.0/releasenotes/notes/deprecate-eventlet-unsafe-memcacheclientpool-f8b4a6733513d73e.yaml`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/source/conf.py` & `keystonemiddleware-9.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `keystonemiddleware-9.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `keystonemiddleware-9.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `keystonemiddleware-9.5.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/setup.cfg` & `keystonemiddleware-9.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 
 [files]
 packages = 
 	keystonemiddleware
@@ -28,14 +29,15 @@
 [global]
 setup-hooks = 
 	pbr.hooks.setup_hook
 
 [entry_points]
 oslo.config.opts = 
 	keystonemiddleware.auth_token = keystonemiddleware.auth_token._opts:list_opts
+	keystonemiddleware.audit = keystonemiddleware.audit:list_opts
 paste.filter_factory = 
 	auth_token = keystonemiddleware.auth_token:filter_factory
 	audit = keystonemiddleware.audit:filter_factory
 	ec2_token = keystonemiddleware.ec2_token:filter_factory
 	s3_token = keystonemiddleware.s3_token:filter_factory
 
 [compile_catalog]
```

### Comparing `keystonemiddleware-9.4.0/setup.py` & `keystonemiddleware-9.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/test-requirements.txt` & `keystonemiddleware-9.5.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `keystonemiddleware-9.4.0/tox.ini` & `keystonemiddleware-9.5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -81,13 +81,7 @@
 import_exceptions =
     keystonemiddleware.i18n
 
 [doc8]
 extensions = .rst, .yaml
 # lines should not be longer than 79 characters.
 max-line-length = 79
-
-[testenv:lower-constraints]
-deps =
-  -c{toxinidir}/lower-constraints.txt
-  -r{toxinidir}/test-requirements.txt
-  -r{toxinidir}/requirements.txt
```

