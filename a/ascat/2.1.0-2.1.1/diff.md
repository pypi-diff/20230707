# Comparing `tmp/ascat-2.1.0.tar.gz` & `tmp/ascat-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascat-2.1.0.tar", last modified: Sat Feb 11 20:30:30 2023, max compression
+gzip compressed data, was "ascat-2.1.1.tar", last modified: Fri Jul  7 11:03:35 2023, max compression
```

## Comparing `ascat-2.1.0.tar` & `ascat-2.1.1.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.681198 ascat-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-11 20:30:21.000000 ascat-2.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.661198 ascat-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.665198 ascat-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-11 20:30:21.000000 ascat-2.1.0/.github/workflows/ascat_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-11 20:30:21.000000 ascat-2.1.0/.github/workflows/ascat_windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-11 20:30:21.000000 ascat-2.1.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-11 20:30:21.000000 ascat-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-11 20:30:21.000000 ascat-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-11 20:30:21.000000 ascat-2.1.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-11 20:30:21.000000 ascat-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-11 20:30:21.000000 ascat-2.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-11 20:30:21.000000 ascat-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-02-11 20:30:30.681198 ascat-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-02-11 20:30:21.000000 ascat-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-11 20:30:21.000000 ascat-2.1.0/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.669198 ascat-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.669198 ascat-2.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/ascat_bufr_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    92416 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_cgls_swi_ts.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_cgls_swi_ts.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.669198 ascat-2.1.0/docs/read_cgls_swi_ts_files/
--rw-r--r--   0 runner    (1001) docker     (123)    65951 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   578048 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_eumetsat.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    35677 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_eumetsat.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.669198 ascat-2.1.0/docs/read_eumetsat_files/
--rw-r--r--   0 runner    (1001) docker     (123)    99279 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_19_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   151416 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_5_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   151239 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_8_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   719257 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.673198 ascat-2.1.0/docs/read_hsaf_cdr_files/
--rw-r--r--   0 runner    (1001) docker     (123)    68510 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    77447 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    78359 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   162796 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    78897 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    65970 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
--rw-r--r--   0 runner    (1001) docker     (123)  1256504 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.673198 ascat-2.1.0/docs/read_hsaf_nrt_files/
--rw-r--r--   0 runner    (1001) docker     (123)   173484 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   168175 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   165841 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
--rw-r--r--   0 runner    (1001) docker     (123)   171571 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
--rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
--rw-r--r--   0 runner    (1001) docker     (123)    31452 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
--rw-r--r--   0 runner    (1001) docker     (123)   186561 2023-02-11 20:30:21.000000 ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-11 20:30:21.000000 ascat-2.1.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-11 20:30:21.000000 ascat-2.1.0/environment_win.yml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-11 20:30:21.000000 ascat-2.1.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-11 20:30:30.681198 ascat-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-11 20:30:21.000000 ascat-2.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-11 20:30:21.000000 ascat-2.1.0/setup_env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.661198 ascat-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.673198 ascat-2.1.0/src/ascat/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/cgls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.677199 ascat-2.1.0/src/ascat/download/
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/download/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/download/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.677199 ascat-2.1.0/src/ascat/eumetsat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/eumetsat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/eumetsat/level1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/eumetsat/level2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24586 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/h_saf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.677199 ascat-2.1.0/src/ascat/read_native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29419 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/bufr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/cdr.py
--rw-r--r--   0 runner    (1001) docker     (123)    68934 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/eps_native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.681198 ascat-2.1.0/src/ascat/read_native/formats/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/ccsds.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    67604 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    34467 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    63559 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (123)    66425 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (123)    66555 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    36662 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    68252 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    68256 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (123)    71118 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (123)    70852 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (123)    44139 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42894 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    36664 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    68252 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    68256 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (123)    71118 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (123)    70852 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (123)    44137 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42843 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25966 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31948 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31615 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/read_native/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-02-11 20:30:21.000000 ascat-2.1.0/src/ascat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.673198 ascat-2.1.0/src/ascat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-11 20:30:30.000000 ascat-2.1.0/src/ascat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:30:30.681198 ascat-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/test_cgls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/test_h_saf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/test_level1.py
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-02-11 20:30:21.000000 ascat-2.1.0/tests/test_level2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.882315 ascat-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 11:03:26.000000 ascat-2.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.862315 ascat-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.866315 ascat-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-07 11:03:26.000000 ascat-2.1.1/.github/workflows/ascat_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-07 11:03:26.000000 ascat-2.1.1/.github/workflows/ascat_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 11:03:26.000000 ascat-2.1.1/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-07 11:03:26.000000 ascat-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 11:03:26.000000 ascat-2.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-07 11:03:26.000000 ascat-2.1.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 11:03:26.000000 ascat-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 11:03:26.000000 ascat-2.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 11:03:26.000000 ascat-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-07 11:03:35.882315 ascat-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-07 11:03:26.000000 ascat-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 11:03:26.000000 ascat-2.1.1/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.870315 ascat-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.870315 ascat-2.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/ascat_bufr_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    92416 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_cgls_swi_ts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_cgls_swi_ts.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.870315 ascat-2.1.1/docs/read_cgls_swi_ts_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    65951 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   578048 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_eumetsat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    35677 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_eumetsat.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.870315 ascat-2.1.1/docs/read_eumetsat_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    99279 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151416 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151239 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_8_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   719257 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.874315 ascat-2.1.1/docs/read_hsaf_cdr_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    68510 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77447 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78359 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   162796 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78897 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65970 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1256504 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.874315 ascat-2.1.1/docs/read_hsaf_nrt_files/
+-rw-r--r--   0 runner    (1001) docker     (123)   173484 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168175 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   165841 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   171571 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31452 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)   186561 2023-07-07 11:03:26.000000 ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 11:03:26.000000 ascat-2.1.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 11:03:26.000000 ascat-2.1.1/environment_win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-07 11:03:26.000000 ascat-2.1.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-07 11:03:35.886315 ascat-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-07 11:03:26.000000 ascat-2.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 11:03:26.000000 ascat-2.1.1/setup_env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.862315 ascat-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.874315 ascat-2.1.1/src/ascat/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/cgls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.878315 ascat-2.1.1/src/ascat/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/download/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/download/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.878315 ascat-2.1.1/src/ascat/eumetsat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/eumetsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/eumetsat/level1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/eumetsat/level2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24586 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/h_saf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.878315 ascat-2.1.1/src/ascat/read_native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29419 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/cdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68934 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/eps_native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.882315 ascat-2.1.1/src/ascat/read_native/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/ccsds.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    67604 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    34467 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    63559 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    66425 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    66555 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39840 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36662 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68252 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68256 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    71118 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    70852 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    44139 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42894 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36664 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68252 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68256 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    71118 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    70852 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    44137 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42843 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25966 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31948 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31615 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/read_native/ragged_array_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-07 11:03:26.000000 ascat-2.1.1/src/ascat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.878315 ascat-2.1.1/src/ascat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 11:03:35.000000 ascat-2.1.1/src/ascat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:35.882315 ascat-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/test_cgls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/test_h_saf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/test_level1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-07-07 11:03:26.000000 ascat-2.1.1/tests/test_level2.py
```

### Comparing `ascat-2.1.0/.coveragerc` & `ascat-2.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/.github/workflows/ascat_ubuntu.yml` & `ascat-2.1.1/.github/workflows/ascat_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/.github/workflows/ascat_windows.yml` & `ascat-2.1.1/.github/workflows/ascat_windows.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/.github/workflows/upload_pypi.yml` & `ascat-2.1.1/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/.gitignore` & `ascat-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/.travis.yml` & `ascat-2.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/CHANGELOG.rst` & `ascat-2.1.1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 2.1.1
+=============
+
+- Add draft for indexed ragged array netcdf file reader using xarray
+- Add ASCAT netcdf swath file reader
+
 Version 2.1.0
 =============
 
 - Add support reading ascat fmv 13 for szf, szr, szo
 
 Version 2.0.6
 =============
```

### Comparing `ascat-2.1.0/LICENSE.txt` & `ascat-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/PKG-INFO` & `ascat-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Readers and converters for data acquired by the ASCAT sensor on-board the Metop satellites
 Home-page: https://www.geo.tuwien.ac.at/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, http://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.1.0/README.rst` & `ascat-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/Makefile` & `ascat-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/ascat_bufr_format.rst` & `ascat-2.1.1/docs/ascat_bufr_format.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/conf.py` & `ascat-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/examples.rst` & `ascat-2.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/index.rst` & `ascat-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_cgls_swi_ts.ipynb` & `ascat-2.1.1/docs/read_cgls_swi_ts.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_cgls_swi_ts.rst` & `ascat-2.1.1/docs/read_cgls_swi_ts.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png` & `ascat-2.1.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_eumetsat.ipynb` & `ascat-2.1.1/docs/read_eumetsat.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_eumetsat.rst` & `ascat-2.1.1/docs/read_eumetsat.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_19_0.png` & `ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_19_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_5_0.png` & `ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_5_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_eumetsat_files/read_eumetsat_8_0.png` & `ascat-2.1.1/docs/read_eumetsat_files/read_eumetsat_8_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr.ipynb` & `ascat-2.1.1/docs/read_hsaf_cdr.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr.rst` & `ascat-2.1.1/docs/read_hsaf_cdr.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png` & `ascat-2.1.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt.ipynb` & `ascat-2.1.1/docs/read_hsaf_nrt.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt.rst` & `ascat-2.1.1/docs/read_hsaf_nrt.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png` & `ascat-2.1.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/setup.cfg` & `ascat-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/setup.py` & `ascat-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/cgls.py` & `ascat-2.1.1/src/ascat/cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/download/connectors.py` & `ascat-2.1.1/src/ascat/download/connectors.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/download/interface.py` & `ascat-2.1.1/src/ascat/download/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/eumetsat/level1.py` & `ascat-2.1.1/src/ascat/eumetsat/level1.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/eumetsat/level2.py` & `ascat-2.1.1/src/ascat/eumetsat/level2.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/file_handling.py` & `ascat-2.1.1/src/ascat/file_handling.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/h_saf.py` & `ascat-2.1.1/src/ascat/h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/bufr.py` & `ascat-2.1.1/src/ascat/read_native/bufr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/cdr.py` & `ascat-2.1.1/src/ascat/read_native/cdr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/eps_native.py` & `ascat-2.1.1/src/ascat/read_native/eps_native.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/ccsds.xml` & `ascat-2.1.1/src/ascat/read_native/formats/ccsds.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps.dtd` & `ascat-2.1.1/src/ascat/read_native/formats/eps.dtd`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps.xsl` & `ascat-2.1.1/src/ascat/read_native/formats/eps.xsl`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml` & `ascat-2.1.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/read_native/hdf5.py` & `ascat-2.1.1/src/ascat/read_native/hdf5.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/src/ascat/utils.py` & `ascat-2.1.1/src/ascat/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -21,21 +21,37 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from datetime import timedelta
 from gzip import GzipFile
 from tempfile import NamedTemporaryFile
 
 import numpy as np
 import xarray as xr
 
 
+def daterange(start_date, end_date):
+    """
+    Generator for daily datetimes.
+
+    Parameters
+    ----------
+    start_date : datetime
+        Start date.
+    end_date : datetime
+        End date.
+    """
+    for n in range(int((end_date - start_date).days)):
+        yield start_date + timedelta(n)
+
+
 def tmp_unzip(filename):
     """
     Unzip file to temporary directory.
 
     Parameters
     ----------
     filename : str
@@ -64,15 +80,15 @@
         Values in dB domain.
 
     Returns
     -------
     val : numpy.ndarray
         Values in linear domain.
     """
-    return 10 ** (val / 10.)
+    return 10**(val / 10.)
 
 
 def lin2db(val):
     """
     Converting from linear to dB domain.
 
     Parameters
@@ -111,15 +127,15 @@
         Window radius needed to achieve the given half power radius
 
     """
     window = window.lower()
     hp_weight = 0.5
     if window == 'hamming':
         alpha = 0.54
-        r = (np.pi * hp_radius) / np.arccos((hp_weight-alpha) / (1-alpha))
+        r = (np.pi * hp_radius) / np.arccos((hp_weight - alpha) / (1 - alpha))
     elif window == 'boxcar':
         r = hp_radius
     else:
         raise ValueError('Window name not supported.')
 
     return r
```

### Comparing `ascat-2.1.0/src/ascat.egg-info/PKG-INFO` & `ascat-2.1.1/src/ascat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.1.0
+Version: 2.1.1
 Summary: Readers and converters for data acquired by the ASCAT sensor on-board the Metop satellites
 Home-page: https://www.geo.tuwien.ac.at/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, http://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.1.0/src/ascat.egg-info/SOURCES.txt` & `ascat-2.1.1/src/ascat.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 src/ascat/eumetsat/level2.py
 src/ascat/read_native/__init__.py
 src/ascat/read_native/bufr.py
 src/ascat/read_native/cdr.py
 src/ascat/read_native/eps_native.py
 src/ascat/read_native/hdf5.py
 src/ascat/read_native/nc.py
+src/ascat/read_native/ragged_array_ts.py
 src/ascat/read_native/formats/ccsds.xml
 src/ascat/read_native/formats/eps.dtd
 src/ascat/read_native/formats/eps.xsl
 src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
```

### Comparing `ascat-2.1.0/tests/test_cgls.py` & `ascat-2.1.1/tests/test_cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/tests/test_download.py` & `ascat-2.1.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/tests/test_h_saf.py` & `ascat-2.1.1/tests/test_h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.1.0/tests/test_level1.py` & `ascat-2.1.1/tests/test_level1.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,18 +125,18 @@
             nptest.assert_allclose(self.eps_ds[field],
                                    self.nc_ds[field], atol=0.1)
 
     def test_read_szf(self):
         """
         Test read SZF formats.
         """
-        self.eps_ds, metadata = self.eps_szf.read()
-        self.h5_ds, metadata = self.h5_szf.read()
+        self.eps_ds, eps_metadata = self.eps_szf.read()
+        self.h5_ds, h5_metadata = self.h5_szf.read()
 
-        for antenna in ['lf', 'lm', 'la', 'rf', 'rm', 'ra']:
+        for antenna in ['lf-vv', 'lm-vv', 'la-vv', 'rf-vv', 'rm-vv', 'ra-vv']:
             for coord in ['lon', 'lat']:
                 nptest.assert_allclose(self.eps_ds[antenna][coord],
                                        self.h5_ds[antenna][coord], atol=1e-4)
 
             matching = ['sig', 'inc', 'azi', 'sat_id', 'as_des_pass',
                         'beam_number', 'swath_indicator']
 
@@ -271,21 +271,21 @@
             ['2018-06-11T04:18:00.630', '2018-06-11T04:18:00.630',
              '2018-06-11T04:18:01.479', '2018-06-11T04:18:01.479',
              '2018-06-11T04:18:01.479', '2018-06-11T04:18:01.479',
              '2018-06-11T04:18:01.479', '2018-06-11T04:18:01.479',
              '2018-06-11T04:18:01.479', '2018-06-11T04:18:01.479'],
             dtype='datetime64[ms]')
 
-        nptest.assert_allclose(self.reader['lf']['lat'][:25],
+        nptest.assert_allclose(self.reader['lf-vv']['lat'][:25],
                                lat_should, atol=1e-5)
-        nptest.assert_allclose(self.reader['lf']['lon'][:25],
+        nptest.assert_allclose(self.reader['lf-vv']['lon'][:25],
                                lon_should, atol=1e-5)
-        nptest.assert_allclose(self.reader['lf']['sig'][:25],
+        nptest.assert_allclose(self.reader['lf-vv']['sig'][:25],
                                sig_should, atol=1e-5)
-        nptest.assert_equal(self.reader['lf']['time'][190:200], t_should)
+        nptest.assert_equal(self.reader['lf-vv']['time'][190:200], t_should)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL1bFileList(unittest.TestCase):
 
     """
     Test read AscatL1bFileList in various formats.
@@ -401,15 +401,15 @@
         Test read date for SZF formats.
         """
         dt = datetime(2018, 6, 11, 4, 18, 0)
 
         eps_data, metadata = self.eps_szf.read(dt)
         hdf5_data, metadata = self.hdf5_szf.read(dt)
 
-        for antenna in ['lf', 'lm', 'la', 'rf', 'rm', 'ra']:
+        for antenna in ['lf-vv', 'lm-vv', 'la-vv', 'rf-vv', 'rm-vv', 'ra-vv']:
             for coord in ['lon', 'lat']:
                 nptest.assert_allclose(eps_data[antenna][coord],
                                        hdf5_data[antenna][coord], atol=1e-4)
 
             matching = ['sig', 'inc', 'azi', 'sat_id', 'as_des_pass',
                         'land_frac', 'f_usable', 'f_land', 'beam_number',
                         'swath_indicator']
@@ -424,15 +424,15 @@
         """
         dt_start = datetime(2018, 6, 11, 4, 18, 0)
         dt_end = datetime(2018, 6, 11, 4, 19, 0)
 
         eps_data, metadata = self.eps_szf.read_period(dt_start, dt_end)
         hdf5_data, metadata = self.hdf5_szf.read_period(dt_start, dt_end)
 
-        for antenna in ['lf', 'lm', 'la', 'rf', 'rm', 'ra']:
+        for antenna in ['lf-vv', 'lm-vv', 'la-vv', 'rf-vv', 'rm-vv', 'ra-vv']:
             for coord in ['lon', 'lat']:
                 nptest.assert_allclose(eps_data[antenna][coord],
                                        hdf5_data[antenna][coord], atol=1e-4)
 
             matching = ['sig', 'inc', 'azi', 'sat_id', 'as_des_pass',
                         'land_frac', 'f_usable', 'f_land', 'beam_number',
                         'swath_indicator']
```

### Comparing `ascat-2.1.0/tests/test_level2.py` & `ascat-2.1.1/tests/test_level2.py`

 * *Files identical despite different names*

