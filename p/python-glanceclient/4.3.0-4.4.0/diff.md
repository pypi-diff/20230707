# Comparing `tmp/python-glanceclient-4.3.0.tar.gz` & `tmp/python-glanceclient-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-glanceclient-4.3.0.tar", last modified: Fri Feb 17 10:32:00 2023, max compression
+gzip compressed data, was "python-glanceclient-4.4.0.tar", last modified: Fri Jul  7 14:30:10 2023, max compression
```

## Comparing `python-glanceclient-4.3.0.tar` & `python-glanceclient-4.4.0.tar`

### file list

```diff
@@ -1,200 +1,202 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10895 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38885 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.943458 python-glanceclient-4.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.943458 python-glanceclient-4.3.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.943458 python-glanceclient-4.3.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40489 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/cli/details.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/cli/glance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/cli/property-keys.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.943458 python-glanceclient-4.3.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/reference/apiv2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2466 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14780 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/https.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/progressbar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21001 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27978 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/tests/functional/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/v1/test_readonly_glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.947456 python-glanceclient-4.3.0/glanceclient/tests/functional/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2701 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/v2/test_http_headers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4565 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/functional/v2/test_readonly_glance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.951453 python-glanceclient-4.3.0/glanceclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21075 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_progressbar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41794 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_ssl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11288 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.951453 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32486 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22491 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2549 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.955451 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12218 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_client_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55420 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25659 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12384 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10122 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7260 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   159587 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_shell_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.955451 python-glanceclient-4.3.0/glanceclient/tests/unit/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/badcert.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/ca.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/expired-cert.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3372 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/wildcard-certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.959449 python-glanceclient-4.3.0/glanceclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.959449 python-glanceclient-4.3.0/glanceclient/v1/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17334 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12947 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18868 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v1/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.959449 python-glanceclient-4.3.0/glanceclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/image_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/image_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23259 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22024 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/metadefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7868 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/namespace_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/resource_type_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69842 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/glanceclient/v2/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.963446 python-glanceclient-4.3.0/python_glanceclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6635 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 10:32:00.000000 python-glanceclient-4.3.0/python_glanceclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.939460 python-glanceclient-4.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.967444 python-glanceclient-4.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/del_from_store-2d807c3038283907.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/drop-py-2-7-f10417b8d1dd38fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/drop-python-3-6-and-3-7-0b299b4dc9673c6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/fix-undesirable-raw-python-error-66e3ddaca7b72ae2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/fix_1889666-22dc97ce577eccc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/headers-encoding-bug-rocky-889ccd885a9cc4e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/image-tasks-api-ee3ea043557a1dfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/log-request-id-e7f67a23a0ed5c7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/multi-store-import-45d05a6193ef2c04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/multihash-filter-ef2a48dc48fae9dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4081 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8999 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23567 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/earlier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1100 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-02-17 10:32:00.975440 python-glanceclient-4.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:32:00.971442 python-glanceclient-4.3.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1490 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/tools/fix_ca_bundle.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/tools/glance.bash_completion
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2023-02-17 10:31:32.000000 python-glanceclient-4.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10939 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39253 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40489 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/cli/details.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/cli/glance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/cli/property-keys.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2986 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/reference/apiv2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/glanceclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2466 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/glanceclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14782 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/https.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3298 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/progressbar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21001 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27978 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/glanceclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/glanceclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.078163 python-glanceclient-4.4.0/glanceclient/tests/functional/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/v1/test_readonly_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/tests/functional/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2701 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/v2/test_http_headers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4565 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/functional/v2/test_readonly_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21075 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_progressbar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41794 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_ssl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11288 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32486 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22491 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2549 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12218 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_client_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55420 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4218 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25659 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12384 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10122 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7260 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   159912 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_shell_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/tests/unit/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/badcert.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2171 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/expired-cert.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3247 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/privatekey.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3372 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/wildcard-certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2623 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.082163 python-glanceclient-4.4.0/glanceclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.086163 python-glanceclient-4.4.0/glanceclient/v1/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17334 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12947 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18868 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v1/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.086163 python-glanceclient-4.4.0/glanceclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/image_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/image_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23259 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22024 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/metadefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7868 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/namespace_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/resource_type_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70063 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/glanceclient/v2/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.086163 python-glanceclient-4.4.0/python_glanceclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6721 2023-07-07 14:30:10.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-07-07 14:30:09.000000 python-glanceclient-4.4.0/python_glanceclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.074163 python-glanceclient-4.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.090163 python-glanceclient-4.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/4.4.0_Release-a3c89184f345e5a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/del_from_store-2d807c3038283907.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/drop-py-2-7-f10417b8d1dd38fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/drop-python-3-6-and-3-7-0b299b4dc9673c6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/fix-undesirable-raw-python-error-66e3ddaca7b72ae2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/fix_1889666-22dc97ce577eccc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/headers-encoding-bug-rocky-889ccd885a9cc4e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/image-tasks-api-ee3ea043557a1dfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/log-request-id-e7f67a23a0ed5c7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/multi-store-import-45d05a6193ef2c04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/multihash-filter-ef2a48dc48fae9dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4081 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.090163 python-glanceclient-4.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8999 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23567 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/earlier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1100 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-07 14:30:10.094164 python-glanceclient-4.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1490 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/tools/fix_ca_bundle.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/tools/glance.bash_completion
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2023-07-07 14:29:41.000000 python-glanceclient-4.4.0/tox.ini
```

### Comparing `python-glanceclient-4.3.0/.zuul.yaml` & `python-glanceclient-4.4.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/AUTHORS` & `python-glanceclient-4.4.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 Niall Bunting <niall.bunting@hpe.com>
 NiallBunting <niall.bunting@hp.com>
 NiallBunting <niall.bunting@hpe.com>
 Nicolas Simonds <nic@metacloud.com>
 Nikhil Komawar <nik.komawar@gmail.com>
 Nikhil Komawar <nikhilskomawar@gmail.com>
 Noboru arai <arai@mxa.nes.nec.co.jp>
+Nobuto Murata <nobuto.murata@canonical.com>
 Oleksii Chuprykov <ochuprykov@mirantis.com>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
 OpenStack Release Bot <infra-root@openstack.org>
 Pawel Koniszewski <pawel.koniszewski@intel.com>
 Pranali Deore <pdeore@redhat.com>
 PranaliD <pdeore@redhat.com>
 Rajat Dhasmana <rajatdhasmana@gmail.com>
```

### Comparing `python-glanceclient-4.3.0/CONTRIBUTING.rst` & `python-glanceclient-4.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/ChangeLog` & `python-glanceclient-4.4.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+4.4.0
+-----
+
+* Release notes for 4.4.0
+* Docs generation: mock the six module for autodoc
+* Bump the CHUNKSIZE to use CPU more efficiently
+* do\_image\_import: always pass remote\_\* to gc.images.image\_import
+* Tox4: remove skipsdist
+* do\_image\_import: fix argument retrieval
+* Update master for stable/2023.1
+
 4.3.0
 -----
 
 * Release notes for 4.3.0
 * Fix functional tests and docs generation
 * Boolean options: use strict checking
 * Unhardcode the value of DEFAULT\_PAGE\_SIZE from the tests
@@ -12,14 +23,15 @@
 
 4.2.0
 -----
 
 * schema\_args: Do not generate option for read-only properties
 * Replace osc with glance commands
 * Switch to 2023.1 Python3 unit tests and generic template name
+* md-property-create: add a mandatory "--type" option
 * Update master for stable/zed
 
 4.1.0
 -----
 
 * Add support for glance-download import method
 * Bump default pagesize
```

### Comparing `python-glanceclient-4.3.0/LICENSE` & `python-glanceclient-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/PKG-INFO` & `python-glanceclient-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-glanceclient
-Version: 4.3.0
+Version: 4.4.0
 Summary: OpenStack Image API Client Library
 Home-page: https://docs.openstack.org/python-glanceclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `python-glanceclient-4.3.0/README.rst` & `python-glanceclient-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/cli/details.rst` & `python-glanceclient-4.4.0/doc/source/cli/details.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/cli/glance.rst` & `python-glanceclient-4.4.0/doc/source/cli/glance.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/cli/index.rst` & `python-glanceclient-4.4.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/cli/property-keys.rst` & `python-glanceclient-4.4.0/doc/source/cli/property-keys.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/conf.py` & `python-glanceclient-4.4.0/doc/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 openstackdocs_bug_project = 'python-glanceclient'
 openstackdocs_bug_tag = ''
 
 # autodoc generation is a bit aggressive and a nuisance when doing heavy
 # text edit cycles.
 # execute "export SPHINX_DEBUG=1" in your terminal to disable
 
+# TODO: remove this once no dependency uses six anymore
+autodoc_mock_imports = ['six']
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The master toctree document.
```

### Comparing `python-glanceclient-4.3.0/doc/source/reference/apiv2.rst` & `python-glanceclient-4.4.0/doc/source/reference/apiv2.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/doc/source/reference/index.rst` & `python-glanceclient-4.4.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/__init__.py` & `python-glanceclient-4.4.0/glanceclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/_i18n.py` & `python-glanceclient-4.4.0/glanceclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/client.py` & `python-glanceclient-4.4.0/glanceclient/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/common/exceptions.py` & `python-glanceclient-4.4.0/glanceclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/common/http.py` & `python-glanceclient-4.4.0/glanceclient/common/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from glanceclient.common import utils
 from glanceclient import exc
 
 osprofiler_web = importutils.try_import("osprofiler.web")
 
 LOG = logging.getLogger(__name__)
 USER_AGENT = 'python-glanceclient'
-CHUNKSIZE = 1024 * 64  # 64kB
+CHUNKSIZE = 1024 * 1024  # 1MiB
 REQ_ID_HEADER = 'X-OpenStack-Request-ID'
 TOKEN_HEADERS = ['X-Auth-Token', 'X-Service-Token']
 
 
 def encode_headers(headers):
     """Encodes headers.
```

### Comparing `python-glanceclient-4.3.0/glanceclient/common/https.py` & `python-glanceclient-4.4.0/glanceclient/common/https.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/common/progressbar.py` & `python-glanceclient-4.4.0/glanceclient/common/progressbar.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/common/utils.py` & `python-glanceclient-4.4.0/glanceclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/exc.py` & `python-glanceclient-4.4.0/glanceclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/shell.py` & `python-glanceclient-4.4.0/glanceclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/functional/README.rst` & `python-glanceclient-4.4.0/glanceclient/tests/functional/README.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/functional/base.py` & `python-glanceclient-4.4.0/glanceclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/functional/v1/test_readonly_glance.py` & `python-glanceclient-4.4.0/glanceclient/tests/functional/v1/test_readonly_glance.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/functional/v2/test_http_headers.py` & `python-glanceclient-4.4.0/glanceclient/tests/functional/v2/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/functional/v2/test_readonly_glance.py` & `python-glanceclient-4.4.0/glanceclient/tests/functional/v2/test_readonly_glance.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_base.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_client.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_exc.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_exc.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_http.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_progressbar.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_progressbar.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_shell.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_ssl.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_ssl.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/test_utils.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_image_members.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_images.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_shell.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v1/test_versions.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v1/test_versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/base.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/fixtures.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/fixtures.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_cache.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_cache.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_client_requests.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_client_requests.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_images.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_info.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_info.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_members.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_namespaces.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_objects.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_objects.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_properties.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_properties.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_resource_types.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_metadefs_tags.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_metadefs_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_schemas.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_schemas.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_shell_v2.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_shell_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -2236,18 +2236,18 @@
                         remote_region=None, remote_image_id=None,
                         remote_service_interface=None,
                         all_stores=None, allow_failure=True,
                         backend=None, stores=None)
 
     def test_image_import_glance_download(self):
         args = self._make_args(
-            {'id': 'IMG-01', 'uri': None, 'remote-region': 'REGION2',
-             'remote-image-id': 'IMG-02',
+            {'id': 'IMG-01', 'uri': None, 'remote_region': 'REGION2',
+             'remote_image_id': 'IMG-02',
              'import_method': 'glance-download',
-             'remote-service-interface': 'public'})
+             'remote_service_interface': 'public'})
         with mock.patch.object(self.gc.images, 'image_import') as mock_import:
             with mock.patch.object(self.gc.images, 'get') as mocked_get:
                 with mock.patch.object(self.gc.images,
                                        'get_import_info') as mocked_info:
                     mocked_get.return_value = {'status': 'queued',
                                                'container_format': 'bare',
                                                'disk_format': 'raw'}
@@ -2275,15 +2275,17 @@
                                                'container_format': 'bare',
                                                'disk_format': 'raw'}
                     mocked_info.return_value = self.import_info_response
                     mock_import.return_value = None
                     test_shell.do_image_import(self.gc, args)
                     mock_import.assert_called_once_with(
                         'IMG-02', 'glance-direct', None, stores=None,
-                        all_stores=None, allow_failure=True, backend=None)
+                        all_stores=None, allow_failure=True,
+                        remote_region=None, remote_image_id=None,
+                        remote_service_interface=None, backend=None)
                     mocked_utils_print_image.assert_not_called()
 
     @mock.patch('glanceclient.common.utils.print_image')
     @mock.patch('glanceclient.v2.shell._validate_backend')
     def test_image_import_multiple_stores(self, mocked_utils_print_image,
                                           msvb):
         args = self._make_args(
@@ -2936,36 +2938,40 @@
                                                      ['name', 'prefix',
                                                       'properties_target'])
 
     def test_do_md_property_create(self):
         args = self._make_args({'namespace': 'MyNamespace',
                                 'name': "MyProperty",
                                 'title': "Title",
+                                'type': 'boolean',
                                 'schema': '{}'})
         with mock.patch.object(self.gc.metadefs_property,
                                'create') as mocked_create:
             expect_property = {
                 'namespace': 'MyNamespace',
                 'name': 'MyProperty',
-                'title': 'Title'
+                'title': 'Title',
+                'type': 'boolean',
             }
 
             mocked_create.return_value = expect_property
 
             test_shell.do_md_property_create(self.gc, args)
 
             mocked_create.assert_called_once_with('MyNamespace',
                                                   name='MyProperty',
-                                                  title='Title')
+                                                  title='Title',
+                                                  type='boolean')
             utils.print_dict.assert_called_once_with(expect_property)
 
     def test_do_md_property_create_invalid_schema(self):
         args = self._make_args({'namespace': 'MyNamespace',
                                 'name': "MyProperty",
                                 'title': "Title",
+                                'type': "boolean",
                                 'schema': 'Invalid'})
         self.assertRaises(SystemExit, test_shell.do_md_property_create,
                           self.gc, args)
 
     def test_do_md_property_update(self):
         args = self._make_args({'namespace': 'MyNamespace',
                                 'property': 'MyProperty',
```

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_tags.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_tasks.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_tasks.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/v2/test_versions.py` & `python-glanceclient-4.4.0/glanceclient/tests/unit/v2/test_versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/ca.crt` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/ca.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/certificate.crt` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/expired-cert.crt` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/expired-cert.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/privatekey.key` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/privatekey.key`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/wildcard-certificate.crt` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/wildcard-certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt` & `python-glanceclient-4.4.0/glanceclient/tests/unit/var/wildcard-san-certificate.crt`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/tests/utils.py` & `python-glanceclient-4.4.0/glanceclient/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/__init__.py` & `python-glanceclient-4.4.0/glanceclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/apiclient/base.py` & `python-glanceclient-4.4.0/glanceclient/v1/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/apiclient/exceptions.py` & `python-glanceclient-4.4.0/glanceclient/v1/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/apiclient/utils.py` & `python-glanceclient-4.4.0/glanceclient/v1/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/client.py` & `python-glanceclient-4.4.0/glanceclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/image_members.py` & `python-glanceclient-4.4.0/glanceclient/v1/image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/images.py` & `python-glanceclient-4.4.0/glanceclient/v1/images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/shell.py` & `python-glanceclient-4.4.0/glanceclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v1/versions.py` & `python-glanceclient-4.4.0/glanceclient/v1/versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/__init__.py` & `python-glanceclient-4.4.0/glanceclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/cache.py` & `python-glanceclient-4.4.0/glanceclient/v2/cache.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/client.py` & `python-glanceclient-4.4.0/glanceclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/image_members.py` & `python-glanceclient-4.4.0/glanceclient/v2/image_members.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/image_schema.py` & `python-glanceclient-4.4.0/glanceclient/v2/image_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/image_tags.py` & `python-glanceclient-4.4.0/glanceclient/v2/image_tags.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/images.py` & `python-glanceclient-4.4.0/glanceclient/v2/images.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/info.py` & `python-glanceclient-4.4.0/glanceclient/v2/info.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/metadefs.py` & `python-glanceclient-4.4.0/glanceclient/v2/metadefs.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/namespace_schema.py` & `python-glanceclient-4.4.0/glanceclient/v2/namespace_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/resource_type_schema.py` & `python-glanceclient-4.4.0/glanceclient/v2/resource_type_schema.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/schemas.py` & `python-glanceclient-4.4.0/glanceclient/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/shell.py` & `python-glanceclient-4.4.0/glanceclient/v2/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,17 +774,17 @@
 def do_image_import(gc, args):
     """Initiate the image import taskflow."""
     backend = getattr(args, "store", None)
     stores = getattr(args, "stores", None)
     all_stores = getattr(args, "os_all_stores", None)
     allow_failure = getattr(args, "os_allow_failure", True)
     uri = getattr(args, "uri", None)
-    remote_region = getattr(args, "remote-region", None)
-    remote_image_id = getattr(args, "remote-image-id", None)
-    remote_service_interface = getattr(args, "remote-service-interface", None)
+    remote_region = getattr(args, "remote_region", None)
+    remote_image_id = getattr(args, "remote_image_id", None)
+    remote_service_interface = getattr(args, "remote_service_interface", None)
 
     if not getattr(args, 'from_create', False):
         if (args.store and (stores or all_stores)) or (stores and all_stores):
             utils.exit("Only one of --store, --stores and --all-stores can be "
                        "provided")
         elif args.store:
             backend = args.store
@@ -797,18 +797,22 @@
         if stores:
             for store in stores:
                 _validate_backend(store, gc)
 
     if getattr(args, 'from_create', False):
         # this command is being called "internally" so we can skip
         # validation -- just do the import and get out of here
-        gc.images.image_import(args.id, args.import_method, args.uri,
-                               backend=backend,
-                               stores=stores, all_stores=all_stores,
-                               allow_failure=allow_failure)
+        gc.images.image_import(
+            args.id, args.import_method, args.uri,
+            remote_region=remote_region,
+            remote_image_id=remote_image_id,
+            remote_service_interface=remote_service_interface,
+            backend=backend,
+            stores=stores, all_stores=all_stores,
+            allow_failure=allow_failure)
         return
 
     # do input validation
     try:
         import_methods = gc.images.get_import_info().get('import-methods')
     except exc.HTTPNotFound:
         utils.exit('Target Glance does not support Image Import workflow')
@@ -1214,22 +1218,24 @@
            help=_('Name of namespace the property will belong.'))
 @utils.arg('--name', metavar='<NAME>', required=True,
            help=_('Internal name of a property.'))
 @utils.arg('--title', metavar='<TITLE>', required=True,
            help=_('Property name displayed to the user.'))
 @utils.arg('--schema', metavar='<SCHEMA>', required=True,
            help=_('Valid JSON schema of a property.'))
+@utils.arg('--type', metavar='<TYPE>', required=True,
+           help=_('Type of the property'))
 def do_md_property_create(gc, args):
     """Create a new metadata definitions property inside a namespace."""
     try:
         schema = json.loads(args.schema)
     except ValueError:
         utils.exit('Schema is not a valid JSON object.')
     else:
-        fields = {'name': args.name, 'title': args.title}
+        fields = {'name': args.name, 'title': args.title, 'type': args.type}
         fields.update(schema)
         new_property = gc.metadefs_property.create(args.namespace, **fields)
         utils.print_dict(new_property)
 
 
 @utils.arg('namespace', metavar='<NAMESPACE>',
            help=_('Name of namespace the property belongs.'))
```

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/tasks.py` & `python-glanceclient-4.4.0/glanceclient/v2/tasks.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/glanceclient/v2/versions.py` & `python-glanceclient-4.4.0/glanceclient/v2/versions.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/python_glanceclient.egg-info/PKG-INFO` & `python-glanceclient-4.4.0/python_glanceclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-glanceclient
-Version: 4.3.0
+Version: 4.4.0
 Summary: OpenStack Image API Client Library
 Home-page: https://docs.openstack.org/python-glanceclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `python-glanceclient-4.3.0/python_glanceclient.egg-info/SOURCES.txt` & `python-glanceclient-4.4.0/python_glanceclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 python_glanceclient.egg-info/top_level.txt
 releasenotes/notes/.placeholder
 releasenotes/notes/2.16.0_Release-43ebe06b74a272ba.yaml
 releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml
 releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml
 releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml
 releasenotes/notes/4.3.0_Release-1a7acbd472e16c72.yaml
+releasenotes/notes/4.4.0_Release-a3c89184f345e5a2.yaml
 releasenotes/notes/add-member-get-command-11c15e0a94ecd39a.yaml
 releasenotes/notes/add-support-for-glance-download-import-method-10525254db3e8e7a.yaml
 releasenotes/notes/boolean-properties-strict-checking-bdd624b5da81e723.yaml
 releasenotes/notes/bp-use-keystoneauth-e12f300e58577b13.yaml
 releasenotes/notes/check-for-md5-59db8fd67870b214.yaml
 releasenotes/notes/copy-existing-image-619b7e6bc3394446.yaml
 releasenotes/notes/del_from_store-2d807c3038283907.yaml
@@ -145,14 +146,15 @@
 releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml
 releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml
 releasenotes/notes/return-request-id-to-caller-47f4c0a684b1d88e.yaml
 releasenotes/notes/rm-deprecate-ssl-opts-c88225a4ba2285ad.yaml
 releasenotes/notes/rocky-2.11.0-ba936fd5e969198d.yaml
 releasenotes/notes/sess_client_grid-3c2101609110f413.yaml
 releasenotes/notes/validation-data-support-dfb2463914818cd2.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/earlier.rst
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/2.17.0_Release-c67392be3b428d10.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/3.1.0_Release-1337ddc753b88905.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/3.6.0_Release-04d3b5017747290b.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/check-for-md5-59db8fd67870b214.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/hidden-images-support-9e2277ad62bf0d31.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/http-headers-per-rfc-8187-aafa3199f863be81.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/multi-store-support-acc7ad0e7e8b6f99.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/multihash-download-verification-596e91bf7b68e7db.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/multihash-support-f1474590cf3ef5cf.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml` & `python-glanceclient-4.4.0/releasenotes/notes/pike-relnote-2c77b01aa8799f35.yaml`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/source/conf.py` & `python-glanceclient-4.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/releasenotes/source/earlier.rst` & `python-glanceclient-4.4.0/releasenotes/source/earlier.rst`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/run_tests.sh` & `python-glanceclient-4.4.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/setup.cfg` & `python-glanceclient-4.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/setup.py` & `python-glanceclient-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/tools/fix_ca_bundle.sh` & `python-glanceclient-4.4.0/tools/fix_ca_bundle.sh`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/tools/glance.bash_completion` & `python-glanceclient-4.4.0/tools/glance.bash_completion`

 * *Files identical despite different names*

### Comparing `python-glanceclient-4.3.0/tox.ini` & `python-glanceclient-4.4.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [tox]
 envlist = py39,pep8
 minversion = 3.18.0
-skipsdist = True
 
 [testenv]
 usedevelop = True
 setenv = OS_STDOUT_NOCAPTURE=False
          OS_STDERR_NOCAPTURE=False
          PYTHONDONTWRITEBYTECODE=1
```

