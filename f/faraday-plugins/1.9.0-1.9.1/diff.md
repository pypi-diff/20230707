# Comparing `tmp/faraday-plugins-1.9.0.tar.gz` & `tmp/faraday-plugins-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday-plugins-1.9.0.tar", last modified: Thu Dec 15 14:44:53 2022, max compression
+gzip compressed data, was "faraday-plugins-1.9.1.tar", last modified: Tue Jan  3 18:46:45 2023, max compression
```

## Comparing `faraday-plugins-1.9.0.tar` & `faraday-plugins-1.9.1.tar`

### file list

```diff
@@ -1,315 +1,318 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.624612 faraday-plugins-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      219 2022-12-15 14:44:53.624612 faraday-plugins-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4942 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.557606 faraday-plugins-1.9.0/faraday_plugins/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     8889 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.561607 faraday-plugins-1.9.0/faraday_plugins/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10762 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    32462 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/plugins_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    43521 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/port_mapper.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.562607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.563607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/
--rw-rw-rw-   0 root         (0) root         (0)     7616 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6099 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.563607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/
--rw-rw-rw-   0 root         (0) root         (0)     3388 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4647 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.564607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/amap/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/amap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4224 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/amap/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.565607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12742 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.565607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan_csv/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan_csv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan_csv/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.566607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appspider/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appspider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appspider/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.567607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arachni/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arachni/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17699 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arachni/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.568607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arp_scan/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arp_scan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arp_scan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.569607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/bandit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/bandit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2079 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/bandit/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.570607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/beef/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/beef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3703 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/beef/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.570607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/brutexss/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/brutexss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2474 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/brutexss/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.571607 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/burp/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/burp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9251 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/burp/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.572608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/checkmarx/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/checkmarx/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4866 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/checkmarx/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.572608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/cobalt/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/cobalt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3516 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/cobalt/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.573608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dig/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dig/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5956 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dig/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.574608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirb/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3869 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirb/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.574608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirsearch/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirsearch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5367 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirsearch/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.575608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsenum/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsenum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4837 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsenum/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.575608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsmap/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsmap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4608 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsmap/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.576608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsrecon/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsrecon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6618 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsrecon/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.577608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnswalk/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnswalk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnswalk/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.577608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/faraday_csv/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/faraday_csv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14375 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/faraday_csv/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.578608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fierce/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fierce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fierce/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.579608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fortify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fortify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15318 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fortify/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.579608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ftp/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ftp/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.580608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/goohost/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/goohost/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4577 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/goohost/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.581608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/grype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/grype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4698 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/grype/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.581608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hping3/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hping3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2585 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hping3/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.582609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hydra/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hydra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hydra/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.582609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/impact/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/impact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/impact/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.583608 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/
--rw-rw-rw-   0 root         (0) root         (0)     3222 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4755 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.584609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ip360/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ip360/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3317 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ip360/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.585609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/junit/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/junit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4385 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/junit/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.585609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/lynis/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/lynis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12143 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/lynis/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.586609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/maltego/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/maltego/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20935 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/maltego/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.587609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/mbsa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/mbsa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4025 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/mbsa/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.587609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/medusa/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/medusa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/medusa/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.588609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/metasploit/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/metasploit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13194 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/metasploit/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.589609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/naabu/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/naabu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/naabu/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.589609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ncrack/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ncrack/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4428 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ncrack/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.590609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ndiff/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ndiff/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ndiff/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.591609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/
--rw-rw-rw-   0 root         (0) root         (0)     9493 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7613 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.591609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus_sc/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus_sc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2717 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus_sc/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.592609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netdiscover/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netdiscover/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netdiscover/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.593609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparker/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9173 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparker/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.593609 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparkercloud/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparkercloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7585 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparkercloud/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.594610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nexpose_full/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nexpose_full/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13311 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nexpose_full/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.595610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nextnet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nextnet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2017 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nextnet/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.595610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nikto/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nikto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nikto/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.596610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nipper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nipper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7118 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nipper/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.596610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nmap/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nmap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18979 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nmap/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.597610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7736 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.598610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei_legacy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei_legacy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6251 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei_legacy/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.598610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openscap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openscap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openscap/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.599610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openvas/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openvas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16723 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openvas/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.599610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pasteanalyzer/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pasteanalyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pasteanalyzer/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.600610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/peepingtom/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/peepingtom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2528 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/peepingtom/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.601610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/
--rw-rw-rw-   0 root         (0) root         (0)     3078 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.602610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ping/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ping/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ping/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.602610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/propecia/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/propecia/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2135 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/propecia/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.603610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/prowler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/prowler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/prowler/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.603610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualysguard/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualysguard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13529 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualysguard/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.604611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualyswebapp/
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualyswebapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6275 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualyswebapp/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.605610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/rdpscan/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/rdpscan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1844 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/rdpscan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.605610 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reconng/
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reconng/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reconng/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.606611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/retina/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/retina/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7803 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/retina/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.606611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reverseraider/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reverseraider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reverseraider/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.607611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/shodan/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/shodan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/shodan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.608611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/skipfish/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/skipfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7136 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/skipfish/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.608611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sonarqubeapi/
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sonarqubeapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sonarqubeapi/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.609611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sourceclear/
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sourceclear/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3022 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sourceclear/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.609611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sshdefaultscan/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sshdefaultscan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sshdefaultscan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.610611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ssl_labs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ssl_labs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ssl_labs/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.611611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyze/
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyze/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5924 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyze/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.611611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyzejson/
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyzejson/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14562 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyzejson/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.612611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/syhunt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/syhunt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/syhunt/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.613611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/telnet/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/telnet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4333 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/telnet/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.613611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/theharvester/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/theharvester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3987 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/theharvester/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.614611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/traceroute/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/traceroute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/traceroute/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.615611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/
--rw-rw-rw-   0 root         (0) root         (0)     3648 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.615611 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/w3af/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/w3af/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6818 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/w3af/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.616612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wapiti/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wapiti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12599 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wapiti/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.616612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wcscan/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wcscan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4933 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wcscan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.617612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webfuzzer/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webfuzzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webfuzzer/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.618612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webinspect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webinspect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webinspect/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.618612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wfuzz/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wfuzz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wfuzz/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.619612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whatweb/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whatweb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whatweb/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.619612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whitesource/
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whitesource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whitesource/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.620612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whois/
--rwxrwxrwx   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whois/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whois/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.621612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wpscan/
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wpscan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4538 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wpscan/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.621612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/x1/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/x1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5533 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/x1/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.622612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/xsssniper/
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/xsssniper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/xsssniper/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.623612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap/
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8450 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.623612 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/
--rw-rw-rw-   0 root         (0) root         (0)     4282 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/DTO.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 14:44:53.559606 faraday-plugins-1.9.0/faraday_plugins.egg-info/
--rw-r--r--   0 root         (0) root         (0)      219 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10017 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-12-15 14:44:53.000000 faraday-plugins-1.9.0/faraday_plugins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-15 14:44:53.624612 faraday-plugins-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      921 2022-12-15 14:44:31.000000 faraday-plugins-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.448106 faraday-plugins-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      219 2023-01-03 18:46:45.447106 faraday-plugins-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.373099 faraday-plugins-1.9.1/faraday_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8905 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.377099 faraday-plugins-1.9.1/faraday_plugins/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10762 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    32462 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/plugins_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    43521 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/port_mapper.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.377099 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.379099 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/
+-rw-rw-rw-   0 root         (0) root         (0)     7616 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6099 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.380100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4647 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.380100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/amap/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/amap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/amap/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.381100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12742 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.382100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan_csv/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan_csv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan_csv/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.383100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appspider/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appspider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appspider/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.383100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arachni/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arachni/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17699 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arachni/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.384100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arp_scan/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arp_scan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arp_scan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.385100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/bandit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/bandit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/bandit/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.385100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/beef/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/beef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/beef/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.386100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/brutexss/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/brutexss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/brutexss/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.387100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/burp/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/burp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9251 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/burp/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.388100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/checkmarx/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/checkmarx/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4866 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/checkmarx/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.388100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2830 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cis/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.389100 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cobalt/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cobalt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cobalt/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.390101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dig/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dig/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5956 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dig/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.390101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirb/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirb/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.391101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirsearch/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirsearch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5367 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirsearch/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.392101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsenum/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsenum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4837 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsenum/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.393101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsmap/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsmap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4608 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsmap/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.393101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsrecon/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsrecon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6618 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsrecon/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.394101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnswalk/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnswalk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnswalk/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.395101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/faraday_csv/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/faraday_csv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14375 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/faraday_csv/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.396101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fierce/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fierce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5565 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fierce/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.396101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fortify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fortify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15318 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fortify/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.397101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ftp/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ftp/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.398101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/goohost/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/goohost/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/goohost/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.398101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/grype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/grype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/grype/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.399101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hping3/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hping3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hping3/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.400102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hydra/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hydra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hydra/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.400102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/impact/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/impact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/impact/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.401101 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4755 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.402102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ip360/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ip360/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ip360/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.403102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/junit/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/junit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4385 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/junit/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.404102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/lynis/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/lynis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12143 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/lynis/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.404102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/maltego/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/maltego/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20935 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/maltego/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.405102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/mbsa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/mbsa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4025 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/mbsa/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.406102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/medusa/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/medusa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/medusa/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.406102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/metasploit/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/metasploit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13194 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/metasploit/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.407102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/naabu/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/naabu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/naabu/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.408102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ncrack/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ncrack/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4428 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ncrack/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.409102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ndiff/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ndiff/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ndiff/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.410102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7613 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.410102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus_sc/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus_sc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus_sc/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.411102 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netdiscover/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netdiscover/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netdiscover/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.412103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparker/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9173 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparker/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.412103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparkercloud/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparkercloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7585 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparkercloud/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.413103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nexpose_full/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nexpose_full/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13311 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nexpose_full/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.414103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nextnet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nextnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nextnet/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.415103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nikto/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nikto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nikto/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.415103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nipper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nipper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7118 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nipper/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.416103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nmap/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nmap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18979 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nmap/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.417103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7752 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.417103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei_legacy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei_legacy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei_legacy/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.418103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openscap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openscap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openscap/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.419103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openvas/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openvas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16723 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openvas/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.420103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pasteanalyzer/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pasteanalyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pasteanalyzer/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.420103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/peepingtom/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/peepingtom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2528 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/peepingtom/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.421103 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.422104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ping/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ping/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.423104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/propecia/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/propecia/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/propecia/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.424104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/prowler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/prowler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/prowler/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.424104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualysguard/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualysguard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13529 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualysguard/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.425104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualyswebapp/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualyswebapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualyswebapp/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.426104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/rdpscan/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/rdpscan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/rdpscan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.426104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reconng/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reconng/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reconng/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.427104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/retina/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/retina/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7803 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/retina/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.428104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reverseraider/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reverseraider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reverseraider/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.428104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/shodan/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/shodan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/shodan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.429104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/skipfish/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/skipfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7136 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/skipfish/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.430104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sonarqubeapi/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sonarqubeapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sonarqubeapi/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.430104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sourceclear/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sourceclear/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3022 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sourceclear/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.431104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sshdefaultscan/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sshdefaultscan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sshdefaultscan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.432104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ssl_labs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ssl_labs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ssl_labs/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.432104 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyze/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyze/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5924 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyze/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.433105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyzejson/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyzejson/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14562 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyzejson/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.434105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/syhunt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/syhunt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/syhunt/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.435105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/telnet/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/telnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4333 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/telnet/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.435105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/theharvester/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/theharvester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/theharvester/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.436105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/traceroute/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/traceroute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/traceroute/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.437105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.438105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/w3af/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/w3af/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6818 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/w3af/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.438105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wapiti/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wapiti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12599 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wapiti/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.439105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wcscan/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wcscan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4933 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wcscan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.440105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webfuzzer/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webfuzzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webfuzzer/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.441105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webinspect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webinspect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webinspect/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.441105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wfuzz/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wfuzz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wfuzz/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.442105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whatweb/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whatweb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whatweb/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.443105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whitesource/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whitesource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whitesource/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.443105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whois/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whois/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whois/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.444105 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wpscan/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wpscan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4538 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wpscan/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.445106 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/x1/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/x1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5533 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/x1/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.445106 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/xsssniper/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/xsssniper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/xsssniper/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.446106 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.447106 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/DTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 18:46:45.375099 faraday-plugins-1.9.1/faraday_plugins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-01-03 18:46:45.000000 faraday-plugins-1.9.1/faraday_plugins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-03 18:46:45.448106 faraday-plugins-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-01-03 18:46:20.000000 faraday-plugins-1.9.1/setup.py
```

### Comparing `faraday-plugins-1.9.0/COPYING` & `faraday-plugins-1.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/README.md` & `faraday-plugins-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/commands.py` & `faraday-plugins-1.9.1/faraday_plugins/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import getpass
 import io
 import json
 import logging
 import os
 import shlex
-import subprocess
+import subprocess # nosec
 import sys
 from pathlib import Path
 
 import click
 from tabulate import tabulate
 
 from faraday_plugins import __version__
@@ -138,15 +138,15 @@
     modified_command = plugin.processCommandString(getpass.getuser(), current_path, command)
     if modified_command:
         command = modified_command
     if dont_run:
         color_message = click.style("Command: ", fg="green")
         click.echo(f"{color_message} {command}")
     else:
-        p = subprocess.Popen(shlex.split(command), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        p = subprocess.Popen(shlex.split(command), stdout=subprocess.PIPE, stderr=subprocess.PIPE) # nosec
         output = io.StringIO()
         while True:
             retcode = p.poll()
             line = p.stdout.readline().decode('utf-8')
             if show_output:
                 sys.stdout.write(line)
             output.write(line)
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/manager.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/plugins_utils.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/plugins_utils.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/port_mapper.txt` & `faraday-plugins-1.9.1/faraday_plugins/plugins/port_mapper.txt`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/acunetix_json/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/acunetix_json/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/amap/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/amap/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appscan_csv/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appscan_csv/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/appspider/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/appspider/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arachni/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arachni/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/arp_scan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/arp_scan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/bandit/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/bandit/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/beef/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/beef/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         This method will discard the output the shell sends, it will read it from
         the xml where it expects it to be present.
 
         NOTE: if 'debug' is true then it is being run from a test case and the
         output being sent is valid.
         """
         try:
-            f = urlopen(self.getSetting("Host") + "/api/hooks?token=" + self.getSetting("Authkey"))
+            f = urlopen(self.getSetting("Host") + "/api/hooks?token=" + self.getSetting("Authkey")) # nosec
             data = json.loads(f.read())
         except Exception:
             self.logger.info("[BeEF] - Connection with api")
             return
 
         if "hooked-browsers" in data:
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/brutexss/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/brutexss/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/burp/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/burp/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/checkmarx/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/checkmarx/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/cobalt/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/cobalt/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dig/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dig/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirb/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirb/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dirsearch/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dirsearch/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsenum/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsenum/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsmap/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsmap/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnsrecon/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnsrecon/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/dnswalk/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/dnswalk/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/faraday_csv/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/faraday_csv/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fierce/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fierce/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,23 +113,23 @@
     def resolveCNAME(self, item, items):
         for i in items:
             if (item['ip'] in i['hosts']):
                 item['ip'] = i['ip']
                 return item
         try:
             item['ip'] = self.resolve_hostname(item['ip'])
-        except:
-            pass  # nosec
+        except: # nosec
+            pass
         return item
 
     def resolveNS(self, item, items):
         try:
             item['hosts'][0] = item['ip']
             item['ip'] = self.resolve_hostname(item['ip'])
-        except:
+        except: # nosec
             pass
         return item
 
     def parseOutputString(self, output):
 
         parser = FierceParser(output)
         for item in parser.items:
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/fortify/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/fortify/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ftp/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ftp/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/goohost/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/goohost/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/grype/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/grype/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hping3/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hping3/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/hydra/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/hydra/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/impact/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/impact/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/invicti/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/invicti/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ip360/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ip360/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/junit/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/junit/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/lynis/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/lynis/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/maltego/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/maltego/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/mbsa/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/mbsa/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/medusa/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/medusa/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/metasploit/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/metasploit/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/naabu/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/naabu/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ncrack/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ncrack/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ndiff/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ndiff/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nessus_sc/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nessus_sc/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netdiscover/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netdiscover/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparker/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparker/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/netsparkercloud/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/netsparkercloud/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nexpose_full/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nexpose_full/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nextnet/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nextnet/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nikto/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nikto/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nipper/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nipper/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nmap/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nmap/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Faraday Penetration Test IDE
 Copyright (C) 2020  Infobyte LLC (http://www.infobytesec.com/)
 See the file 'doc/LICENSE' for the license information
 
 """
-import subprocess
+import subprocess # nosec
 import re
 import sys
 import json
 from dateutil.parser import parse
 from urllib.parse import urlparse
 from packaging import version
 from faraday_plugins.plugins.plugin import PluginMultiLineJsonFormat
@@ -178,15 +178,15 @@
                           r" --json -irr -o %s" % self._output_file_path,
                           command_string)
 
     def canParseCommandString(self, current_input):
         can_parse = super().canParseCommandString(current_input)
         if can_parse:
             try:
-                proc = subprocess.Popen([self.command, '-version'], stderr=subprocess.PIPE)
+                proc = subprocess.Popen([self.command, '-version'], stderr=subprocess.PIPE) # nosec
                 output = proc.stderr.read()
                 match = re.search(r"Current Version: ([0-9.]+)", output.decode('UTF-8'))
                 if match:
                     nuclei_version = match.groups()[0]
                     return version.parse(nuclei_version) >= version.parse("2.5.3")
                 else:
                     return False
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/nuclei_legacy/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/nuclei_legacy/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess # nosec
 import re
 import json
 from packaging import version
 from urllib.parse import urlparse
 from dateutil.parser import parse
 from faraday_plugins.plugins.plugin import PluginMultiLineJsonFormat
 
@@ -134,15 +134,15 @@
                           r"--json -irr -o %s" % self._output_file_path,
                           command_string)
 
     def canParseCommandString(self, current_input):
         can_parse = super().canParseCommandString(current_input)
         if can_parse:
             try:
-                proc = subprocess.Popen([self.command, '-version'], stderr=subprocess.PIPE)
+                proc = subprocess.Popen([self.command, '-version'], stderr=subprocess.PIPE) # nosec
                 output = proc.stderr.read()
                 match = re.search(r"Current Version: ([0-9.]+)", output.decode('UTF-8'))
                 if match:
                     nuclei_version = match.groups()[0]
                     return version.parse(nuclei_version) <= version.parse("2.5.2")
                 else:
                     return False
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openscap/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openscap/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/openvas/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/openvas/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pasteanalyzer/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pasteanalyzer/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/peepingtom/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/peepingtom/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/pentera/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/pentera/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ping/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ping/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/propecia/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/propecia/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/prowler/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/prowler/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualysguard/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualysguard/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/qualyswebapp/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/qualyswebapp/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/rdpscan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/rdpscan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reconng/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reconng/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/retina/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/retina/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/reverseraider/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/reverseraider/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/shodan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/shodan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/skipfish/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/skipfish/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sonarqubeapi/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sonarqubeapi/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sourceclear/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sourceclear/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sshdefaultscan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sshdefaultscan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/ssl_labs/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/ssl_labs/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyze/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyze/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/sslyzejson/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/sslyzejson/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/syhunt/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/syhunt/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/telnet/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/telnet/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/theharvester/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/theharvester/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/traceroute/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/traceroute/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         parameters.reverse()
         hostName = parameters[0]
 
         try:
             int(hostName)
             # No exception => host is the next item.
             hostName = parameters[1]
-        except:
+        except: # nosec
             pass
 
         # Add host and note with output of traceroute.
         hostId = self.createAndAddHost(hostName)
         self.createAndAddNoteToHost(hostId, "Traceroute Results", output)
 
         print("[*]Parse finished, API faraday called...")
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/trivy_json/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/trivy_json/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/w3af/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/w3af/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wapiti/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wapiti/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wcscan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wcscan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webfuzzer/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webfuzzer/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/webinspect/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/webinspect/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
                 try:
                     field = section.find("Name").text
                     value = section.find("SectionText").text
 
                     faraday_obj_name = map_objects_fields.get(field)[0]
                     faraday_field = map_objects_fields.get(field)[1]
-                except:
+                except: # nosec
                     continue
 
                 if faraday_field == "reference" and value != "":
                     obj[faraday_obj_name].get("reference").append(cleanhtml(value))
                 else:
                     obj[faraday_obj_name].update({faraday_field:value})
```

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wfuzz/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wfuzz/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whatweb/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whatweb/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whitesource/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whitesource/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/whois/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/whois/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/wpscan/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/wpscan/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/x1/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/x1/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/xsssniper/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/xsssniper/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/DTO.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/DTO.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins/plugins/repo/zap_json/plugin.py` & `faraday-plugins-1.9.1/faraday_plugins/plugins/repo/zap_json/plugin.py`

 * *Files identical despite different names*

### Comparing `faraday-plugins-1.9.0/faraday_plugins.egg-info/SOURCES.txt` & `faraday-plugins-1.9.1/faraday_plugins.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 faraday_plugins/plugins/repo/beef/plugin.py
 faraday_plugins/plugins/repo/brutexss/__init__.py
 faraday_plugins/plugins/repo/brutexss/plugin.py
 faraday_plugins/plugins/repo/burp/__init__.py
 faraday_plugins/plugins/repo/burp/plugin.py
 faraday_plugins/plugins/repo/checkmarx/__init__.py
 faraday_plugins/plugins/repo/checkmarx/plugin.py
+faraday_plugins/plugins/repo/cis/__init__.py
+faraday_plugins/plugins/repo/cis/plugin.py
 faraday_plugins/plugins/repo/cobalt/__init__.py
 faraday_plugins/plugins/repo/cobalt/plugin.py
 faraday_plugins/plugins/repo/dig/__init__.py
 faraday_plugins/plugins/repo/dig/plugin.py
 faraday_plugins/plugins/repo/dirb/__init__.py
 faraday_plugins/plugins/repo/dirb/plugin.py
 faraday_plugins/plugins/repo/dirsearch/__init__.py
```

### Comparing `faraday-plugins-1.9.0/setup.py` & `faraday-plugins-1.9.1/setup.py`

 * *Files identical despite different names*

