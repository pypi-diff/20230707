# Comparing `tmp/faraday_agent_parameters_types-1.2.0.tar.gz` & `tmp/faraday_agent_parameters_types-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday_agent_parameters_types-1.2.0.tar", last modified: Wed Nov 30 15:21:25 2022, max compression
+gzip compressed data, was "faraday_agent_parameters_types-1.3.0.tar", last modified: Fri Jul  7 19:24:27 2023, max compression
```

## Comparing `faraday_agent_parameters_types-1.2.0.tar` & `faraday_agent_parameters_types-1.3.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.271816 faraday_agent_parameters_types-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      244 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     3781 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      317 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2327 2022-11-30 15:21:25.271816 faraday_agent_parameters_types-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      928 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.263816 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/
--rw-rw-rw-   0 root         (0) root         (0)      319 2022-11-30 15:17:05.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.267816 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_boolean.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_float.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_integer.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_ip.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_list.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_string.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_url.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/faraday_agent_parameters_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.259816 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.271816 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      650 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)      885 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)     1427 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      651 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      541 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nikto2-2.1.3.json
--rw-rw-rw-   0 root         (0) root         (0)     1060 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)     1146 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      631 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      937 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-10-26 15:05:28.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json
--rw-rw-rw-   0 root         (0) root         (0)      597 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      476 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/shodan2-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      571 2022-11-01 18:22:47.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json
--rw-rw-rw-   0 root         (0) root         (0)      533 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      975 2022-11-30 14:53:46.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/w3af-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      519 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      701 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      581 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/zap-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)     3278 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.263816 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2327 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3027 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      135 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-30 15:21:25.000000 faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-11-30 15:21:25.275816 faraday_agent_parameters_types-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2084 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.271816 faraday_agent_parameters_types-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9588 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_faraday_agent_parameters_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 15:21:25.271816 faraday_agent_parameters_types-1.2.0/tests/test_manifests/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_manifests/test-1.5.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_manifests/test-1.7.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_manifests/test-1.8.0.json
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_manifests/test2-1.6.0.json
--rw-rw-rw-   0 root         (0) root         (0)     2068 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.2.0/tests/test_manifests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)      383 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      317 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      928 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.956500 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-07 19:07:52.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.960500 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_float.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_integer.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_ip.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_string.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_url.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-05 20:36:00.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/faraday_agent_parameters_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.956500 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      650 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)      885 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-05-11 13:05:04.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      651 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      541 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nikto2-2.1.3.json
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      631 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      937 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-10-26 15:04:40.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      597 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      476 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/shodan2-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      571 2022-11-01 18:23:20.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      533 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-05-05 20:30:58.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      501 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/w3af-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      519 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      701 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      581 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-10-19 20:22:01.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/zap-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.960500 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-07 19:24:27.000000 faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9588 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/test_faraday_agent_parameters_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 19:24:27.964501 faraday_agent_parameters_types-1.3.0/tests/test_manifests/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/test_manifests/test-1.5.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/test_manifests/test-1.7.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/test_manifests/test-1.8.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-08-22 21:01:13.000000 faraday_agent_parameters_types-1.3.0/tests/test_manifests/test2-1.6.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-11 13:14:49.000000 faraday_agent_parameters_types-1.3.0/tests/test_manifests.py
```

### Comparing `faraday_agent_parameters_types-1.2.0/CONTRIBUTING.rst` & `faraday_agent_parameters_types-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/COPYING` & `faraday_agent_parameters_types-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/PKG-INFO` & `faraday_agent_parameters_types-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_parameters_types
-Version: 1.2.0
+Version: 1.3.0
 Summary: The faraday agents run code remotely to ensure your domains. This info is triggered and published
 Home-page: https://github.com/infobyte/faraday_agent_parameters_types
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `faraday_agent_parameters_types-1.2.0/README.md` & `faraday_agent_parameters_types-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_list.py` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_list.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/custom_types/faraday_string.py` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/custom_types/faraday_string.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/data_types.py` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/data_types.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types/utils.py` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types/utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/PKG-INFO` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday-agent-parameters-types
-Version: 1.2.0
+Version: 1.3.0
 Summary: The faraday agents run code remotely to ensure your domains. This info is triggered and published
 Home-page: https://github.com/infobyte/faraday_agent_parameters_types
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `faraday_agent_parameters_types-1.2.0/faraday_agent_parameters_types.egg-info/SOURCES.txt` & `faraday_agent_parameters_types-1.3.0/faraday_agent_parameters_types.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 faraday_agent_parameters_types/custom_types/faraday_string.py
 faraday_agent_parameters_types/custom_types/faraday_url.py
 faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json
 faraday_agent_parameters_types/static/manifests/burp-2.0.0.json
 faraday_agent_parameters_types/static/manifests/burp-2.0.1.json
 faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json
 faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json
+faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json
 faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json
 faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json
 faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json
 faraday_agent_parameters_types/static/manifests/nikto2-2.1.3.json
 faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json
 faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json
 faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json
```

### Comparing `faraday_agent_parameters_types-1.2.0/setup.py` & `faraday_agent_parameters_types-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/tests/test_faraday_agent_parameters_types.py` & `faraday_agent_parameters_types-1.3.0/tests/test_faraday_agent_parameters_types.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.2.0/tests/test_manifests.py` & `faraday_agent_parameters_types-1.3.0/tests/test_manifests.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                 assert tool["manifest_version"] == "1.7.0"
             if name == "test2":
                 assert tool["manifest_version"] == "1.6.0"
 
     def test_incorrect_version_requested(self):
         with pytest.raises(ValueError) as error:
             get_manifests("hola")
-        assert "Version requested not valid" in str(error.value)
+        assert "Invalid version: 'hola'" in str(error.value)
```

