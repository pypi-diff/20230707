# Comparing `tmp/adafruit-circuitpython-epd-2.9.4.tar.gz` & `tmp/adafruit-circuitpython-epd-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-epd-2.9.4.tar", last modified: Thu Jun 24 17:13:16 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-epd-2.9.5.tar", last modified: Thu Jul 22 13:43:38 2021, max compression
```

## Comparing `adafruit-circuitpython-epd-2.9.4.tar` & `adafruit-circuitpython-epd-2.9.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.430564 adafruit-circuitpython-epd-2.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.434564 adafruit-circuitpython-epd-2.9.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.434564 adafruit-circuitpython-epd-2.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16232 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.434564 adafruit-circuitpython-epd-2.9.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.434564 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-06-24 17:13:15.000000 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-06-24 17:13:16.000000 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 17:13:15.000000 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-24 17:13:15.000000 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-24 17:13:15.000000 adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.434564 adafruit-circuitpython-epd-2.9.4/adafruit_epd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13074 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/epd.py
--rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/il0373.py
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/il0398.py
--rw-r--r--   0 runner    (1001) docker     (121)     6848 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/il91874.py
--rw-r--r--   0 runner    (1001) docker     (121)     3650 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/mcp_sram.py
--rw-r--r--   0 runner    (1001) docker     (121)     5619 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1608.py
--rw-r--r--   0 runner    (1001) docker     (121)     6680 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1675.py
--rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1675b.py
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1680.py
--rw-r--r--   0 runner    (1001) docker     (121)     6351 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1681.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4155 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_blinka.py
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_bonnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_pillow_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_shieldtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/examples/epd_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-24 17:13:16.438564 adafruit-circuitpython-epd-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-06-24 17:13:06.000000 adafruit-circuitpython-epd-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.521785 adafruit-circuitpython-epd-2.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.521785 adafruit-circuitpython-epd-2.9.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.525785 adafruit-circuitpython-epd-2.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16232 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.525785 adafruit-circuitpython-epd-2.9.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.525785 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-07-22 13:43:38.000000 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-07-22 13:43:38.000000 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-22 13:43:38.000000 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-07-22 13:43:38.000000 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-07-22 13:43:38.000000 adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.525785 adafruit-circuitpython-epd-2.9.5/adafruit_epd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13074 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/epd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/il0373.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5013 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/il0398.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6848 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/il91874.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3650 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/mcp_sram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5619 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1608.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6680 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1675.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1675b.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6754 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1680.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6351 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1681.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5628 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     4848 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4155 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_blinka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3217 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_bonnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3146 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_pillow_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_shieldtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/examples/epd_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-22 13:43:38.529785 adafruit-circuitpython-epd-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-07-22 13:43:26.000000 adafruit-circuitpython-epd-2.9.5/setup.py
```

### Comparing `adafruit-circuitpython-epd-2.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-epd-2.9.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/.github/workflows/build.yml` & `adafruit-circuitpython-epd-2.9.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/.github/workflows/release.yml` & `adafruit-circuitpython-epd-2.9.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/.pre-commit-config.yaml` & `adafruit-circuitpython-epd-2.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/.pylintrc` & `adafruit-circuitpython-epd-2.9.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-epd-2.9.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/LICENSE` & `adafruit-circuitpython-epd-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-epd-2.9.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/LICENSES/MIT.txt` & `adafruit-circuitpython-epd-2.9.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-epd-2.9.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/PKG-INFO` & `adafruit-circuitpython-epd-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-epd
-Version: 2.9.4
+Version: 2.9.5
 Summary: CircuitPython library for EPD e-ink displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_EPD
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-epd-2.9.4/README.rst` & `adafruit-circuitpython-epd-2.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/PKG-INFO` & `adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-epd
-Version: 2.9.4
+Version: 2.9.5
 Summary: CircuitPython library for EPD e-ink displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_EPD
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_circuitpython_epd.egg-info/SOURCES.txt` & `adafruit-circuitpython-epd-2.9.5/adafruit_circuitpython_epd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/epd.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/epd.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/il0373.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/il0373.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/il0398.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/il0398.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/il91874.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/il91874.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/mcp_sram.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/mcp_sram.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1608.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1608.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1675.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1675.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1675b.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1675b.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1680.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1680.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/adafruit_epd/ssd1681.py` & `adafruit-circuitpython-epd-2.9.5/adafruit_epd/ssd1681.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/docs/_static/favicon.ico` & `adafruit-circuitpython-epd-2.9.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/docs/conf.py` & `adafruit-circuitpython-epd-2.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/docs/index.rst` & `adafruit-circuitpython-epd-2.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_bitmap.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_bitmap.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_blinka.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_blinka.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_bonnet.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_bonnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_pillow_demo.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_pillow_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 srcs = None
 rst = digitalio.DigitalInOut(board.D27)
 busy = digitalio.DigitalInOut(board.D17)
 
 # give them all to our driver
 # display = Adafruit_SSD1608(200, 200,        # 1.54" HD mono display
 # display = Adafruit_SSD1675(122, 250,        # 2.13" HD mono display
-# display = Adafruit_SSD1680(122, 250,        # 2.13" HD Tri-color display
+# display = Adafruit_SSD1680(122, 250,        # 2.13" HD Tri-color or mono display
 # display = Adafruit_SSD1681(200, 200,        # 1.54" HD Tri-color display
 # display = Adafruit_IL91874(176, 264,        # 2.7" Tri-color display
 # display = Adafruit_IL0373(152, 152,         # 1.54" Tri-color display
 # display = Adafruit_IL0373(128, 296,         # 2.9" Tri-color display
 # display = Adafruit_IL0398(400, 300,         # 4.2" Tri-color display
 display = Adafruit_IL0373(
     104,
@@ -66,15 +66,15 @@
 
 image = Image.new("RGB", (display.width, display.height))
 
 # Get drawing object to draw on image.
 draw = ImageDraw.Draw(image)
 
 # Draw a filled box as the background
-draw.rectangle((0, 0, display.width, display.height), fill=BACKGROUND_COLOR)
+draw.rectangle((0, 0, display.width - 1, display.height - 1), fill=BACKGROUND_COLOR)
 
 # Draw a smaller inner foreground rectangle
 draw.rectangle(
     (BORDER, BORDER, display.width - BORDER - 1, display.height - BORDER - 1),
     fill=FOREGROUND_COLOR,
 )
```

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_pillow_image.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_pillow_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 srcs = None
 rst = digitalio.DigitalInOut(board.D27)
 busy = digitalio.DigitalInOut(board.D17)
 
 # give them all to our driver
 # display = Adafruit_SSD1608(200, 200,        # 1.54" HD mono display
 # display = Adafruit_SSD1675(122, 250,        # 2.13" HD mono display
-# display = Adafruit_SSD1680(122, 250,        # 2.13" HD Tri-color display
+# display = Adafruit_SSD1680(122, 250,        # 2.13" HD Tri-color or mono display
 # display = Adafruit_SSD1681(200, 200,        # 1.54" HD Tri-color display
 # display = Adafruit_IL91874(176, 264,        # 2.7" Tri-color display
 # display = Adafruit_IL0373(152, 152,         # 1.54" Tri-color display
 # display = Adafruit_IL0373(128, 296,         # 2.9" Tri-color display
 # display = Adafruit_IL0398(400, 300,         # 4.2" Tri-color display
 display = Adafruit_IL0373(
     104,
```

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_shieldtest.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_shieldtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/examples/epd_simpletest.py` & `adafruit-circuitpython-epd-2.9.5/examples/epd_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-epd-2.9.4/setup.py` & `adafruit-circuitpython-epd-2.9.5/setup.py`

 * *Files identical despite different names*

