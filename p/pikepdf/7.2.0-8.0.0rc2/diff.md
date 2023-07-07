# Comparing `tmp/pikepdf-7.2.0.tar.gz` & `tmp/pikepdf-8.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-7.2.0.tar", last modified: Thu Apr 13 06:58:17 2023, max compression
+gzip compressed data, was "pikepdf-8.0.0rc2.tar", last modified: Fri Jul  7 09:57:15 2023, max compression
```

## Comparing `pikepdf-7.2.0.tar` & `pikepdf-8.0.0rc2.tar`

### file list

```diff
@@ -1,231 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.790136 pikepdf-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.758135 pikepdf-7.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17023 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12523 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14331 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-2.5.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21305 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21097 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CECILL-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    20272 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/GFDL-1.2-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)    16727 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/Zlib.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-04-13 06:55:41.000000 pikepdf-7.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-04-13 06:58:17.786136 pikepdf-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6034 2023-04-13 06:55:41.000000 pikepdf-7.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/build-scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/environ-from-pyproject.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      382 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-build-sdist-deps.bash
--rwxr-xr-x   0 runner    (1001) docker     (122)      482 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-build-wheel-deps.bash
--rwxr-xr-x   0 runner    (1001) docker     (122)      225 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-download-qpdf.bash
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-install-libxmp.bash
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/win-download-qpdf.ps1
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7687 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/_ext/fix_pybind11_autodoc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/_notebooks/
--rw-r--r--   0 runner    (1001) docker     (122)     6560 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/_notebooks/pages.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/filters.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/settings.rst
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/binary-wheels.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12349 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (122)   543264 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/28fish.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/acrobat-attachments.png
--rw-r--r--   0 runner    (1001) docker     (122)    26172 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/congress_im0.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pdfcoords.svg
--rw-r--r--   0 runner    (1001) docker     (122)   148388 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike-cartoon.png
--rw-r--r--   0 runner    (1001) docker     (122)    88609 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike-release.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    32321 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike.png
--rw-r--r--   0 runner    (1001) docker     (122)    29276 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pikemen.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    65692 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/save-pike.jpg
--rw-r--r--   0 runner    (1001) docker     (122)   155993 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/sushi.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     5602 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/references/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/arch.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/resources.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/docs/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version0.rst
--rw-r--r--   0 runner    (1001) docker     (122)    17003 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version1.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version2.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version3.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version4.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4745 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version5.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version6.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version7.rst
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/docs/topics/
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/attachments.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/content_streams.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/encoding.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/images.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6187 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/nametrees.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/objects.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/outlines.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/overlays.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/page.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/pagelayout.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/pages.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/security.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/streams.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-04-13 06:55:41.000000 pikepdf-7.2.0/examples/find_links.py
--rw-r--r--   0 runner    (1001) docker     (122)    38728 2023-04-13 06:55:41.000000 pikepdf-7.2.0/licenses-for-wheels.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-04-13 06:55:41.000000 pikepdf-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 06:58:17.790136 pikepdf-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-04-13 06:55:41.000000 pikepdf-7.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.758135 pikepdf-7.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.774135 pikepdf-7.2.0/src/core/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/gsl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42088 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10354 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14258 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.774135 pikepdf-7.2.0/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)    25624 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.778135 pikepdf-7.2.0/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (122)    36142 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    31934 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    14786 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.778135 pikepdf-7.2.0/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5304 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.782136 pikepdf-7.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.786136 pikepdf-7.2.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/1biticc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/Gray.icc
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/aquamarine-cie.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/aquamarine-cie.png
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/cmyk-jpeg.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/congress-gray.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/congress.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/content-stream-errors.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/form.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/formxobject.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/fourpages.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/graph-encrypted.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/graph.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/image-mono-inline.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/invalid_creationdate.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/jbig2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/jbig2global.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/outlines.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal-1bit-rgb.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal-1bit-trivial.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal.pdf
--rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pdfx.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pike-flate-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pike-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pink-palette-icc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pink-palette-icc.png
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/rle.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/sandwich.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    35498 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.832679 pikepdf-8.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-07 09:57:15.828679 pikepdf-8.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6030 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 09:57:15.832679 pikepdf-8.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.808679 pikepdf-8.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.816679 pikepdf-8.0.0rc2/src/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42088 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14258 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.820679 pikepdf-8.0.0rc2/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.824679 pikepdf-8.0.0rc2/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32038 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.820679 pikepdf-8.0.0rc2/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.828679 pikepdf-8.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36923 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_sanity.py
```

### Comparing `pikepdf-7.2.0/LICENSE.txt` & `pikepdf-8.0.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/PKG-INFO` & `pikepdf-8.0.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 7.2.0
+Version: 8.0.0rc2
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
@@ -16,28 +16,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: mypy
 Provides-Extra: test
 License-File: LICENSE.txt
 
 <!-- SPDX-FileCopyrightText: 2022 James R. Barlow -->
 <!-- SPDX-License-Identifier: MPL-2.0 -->
 
 pikepdf
 =======
 
 **pikepdf** is a Python library for reading and writing PDF files.
 
-[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
+[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
 
 pikepdf is based on [QPDF](https://github.com/qpdf/qpdf), a powerful PDF manipulation and repair library.
 
 Python + QPDF = "py" + "qpdf" = "pyqpdf", which looks like a dyslexia test. Say it out loud, and it sounds like "pikepdf".
 
 ```python
 # Elegant, Pythonic API
@@ -74,15 +75,15 @@
 | Creates linearized ("fast web view") PDFs                           | ✔                                           | ✘                                         |
 | Test suite coverage                                                 | ![codecov][codecov]                         | ![codecovpypdf2][codecovpypdf]            |
 | Creates PDFs that pass PDF validation tests                         | ✔                                           | ✘                                         |
 | Modifies PDF/A without breaking PDF/A compliance                    | ✔                                           | ✘                                         |
 | PDF XMP metadata editing                                            | ✔                                           | read-only                                 |
 | Integrates with Jupyter and IPython notebooks for rapid development | ✔                                           | ✘                                         |
 
-[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J
+[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J
 
 [codecovpypdf]: https://codecov.io/gh/py-pdf/pypdf/branch/main/graph/badge.svg?token=id42cGNZ5Z
 
 Testimonials
 ------------
 
 > I decided to try writing a quick Python program with pikepdf to automate [something] and it "just worked". –Jay Berkenbilt, creator of QPDF
```

### Comparing `pikepdf-7.2.0/README.md` & `pikepdf-8.0.0rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!-- SPDX-License-Identifier: MPL-2.0 -->
 
 pikepdf
 =======
 
 **pikepdf** is a Python library for reading and writing PDF files.
 
-[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
+[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
 
 pikepdf is based on [QPDF](https://github.com/qpdf/qpdf), a powerful PDF manipulation and repair library.
 
 Python + QPDF = "py" + "qpdf" = "pyqpdf", which looks like a dyslexia test. Say it out loud, and it sounds like "pikepdf".
 
 ```python
 # Elegant, Pythonic API
@@ -47,15 +47,15 @@
 | Creates linearized ("fast web view") PDFs                           | ✔                                           | ✘                                         |
 | Test suite coverage                                                 | ![codecov][codecov]                         | ![codecovpypdf2][codecovpypdf]            |
 | Creates PDFs that pass PDF validation tests                         | ✔                                           | ✘                                         |
 | Modifies PDF/A without breaking PDF/A compliance                    | ✔                                           | ✘                                         |
 | PDF XMP metadata editing                                            | ✔                                           | read-only                                 |
 | Integrates with Jupyter and IPython notebooks for rapid development | ✔                                           | ✘                                         |
 
-[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J
+[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J
 
 [codecovpypdf]: https://codecov.io/gh/py-pdf/pypdf/branch/main/graph/badge.svg?token=id42cGNZ5Z
 
 Testimonials
 ------------
 
 > I decided to try writing a quick Python program with pikepdf to automate [something] and it "just worked". –Jay Berkenbilt, creator of QPDF
```

### Comparing `pikepdf-7.2.0/pyproject.toml` & `pikepdf-8.0.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SPDX-FileCopyrightText: 2022 James R. Barlow
 # SPDX-License-Identifier: MPL-2.0
 
 [build-system]
 requires = [
   "setuptools >= 61",
-  "setuptools-scm[toml] >= 7.0.5",
   "wheel >= 0.37",
   "pybind11 >= 2.10.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pikepdf"
-dynamic = ["version"]
+version = "8.0.0rc2"
 description = "Read and write PDFs with Python, powered by qpdf"
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["PDF"]
 authors = [
   { name = "James R. Barlow", email= "james@purplerock.ca"}
 ]
@@ -31,34 +30,38 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
     "Pillow>=9.0",
+    "Pillow<10; platform_python_implementation == 'PyPy'",
     "deprecation",
     "lxml>=4.8",
     "packaging",
 ]
 
 [project.urls]
 documentation = "https://pikepdf.readthedocs.io/"
 repository = "https://github.com/pikepdf/pikepdf"
 changelog = "https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html"
 
 [project.optional-dependencies]
+dev = [
+    "pre-commit",
+    "typer[all]"
+]
 docs = [
     "GitPython",
     "PyGithub",
     "Sphinx>=3",
     "ipython",
     "matplotlib",
     "pybind11",
     "requests",
-    "setuptools-scm",
     "sphinx-design",
     "sphinx-issues",
     "sphinx-rtd-theme",
     "tomli;python_version < '3.11'",
 ]
 mypy = [
     "lxml-stubs",
@@ -66,14 +69,15 @@
     "types-requests",
     "types-setuptools",
 ]
 test = [
     "attrs>=20.2.0",
     "coverage[toml]",
     "hypothesis>=6.36",
+    "numpy>=1.21.0",
     "psutil>=5.9",
     "pybind11",
     "pytest>=6.2.5",
     "pytest-cov>=3.0.0",
     "pytest-timeout>=2.1.0",
     "pytest-xdist>=2.5.0",
     "python-dateutil>=2.8.1",
@@ -83,16 +87,14 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 pikepdf = ["*.dll", "py.typed"]
 
-[tool.setuptools_scm]
-
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311"]
 skip-string-normalization = true
 include = '\.pyi?$'
 exclude = '''
 /(
@@ -113,38 +115,35 @@
 '''
 
 [tool.cibuildwheel]
 test-command = "pytest -nauto {project}/tests"
 test-extras = "test"
 # cp36: ancient
 # pp37: discontinued by Pillow - https://pypi.org/project/Pillow/#files
-# pp*-win32: lxml does not build win32 for pp, so we can't support it
 # Reminder:
 #   build.yml sets CIBW_BUILD to select what can be built
 #   this file sets skip to deselect what cannot be built
-skip = ["cp36-*", "cp37-*", "pp37-*", "pp*-win32", "*musllinux*", "pp*-manylinux*_aarch64"]
-test-skip = "*_arm64 *_universal2:arm64"
+skip = ["cp36-*", "cp37-*", "pp37-*", "*-win32", "*musllinux*", "pp*-manylinux*_aarch64"]
+test-skip = "*_universal2:arm64"
 
 [tool.cibuildwheel.environment]
-QPDF_MIN_VERSION = "11.2.0"
-QPDF_VERSION = "11.2.0"
+QPDF_MIN_VERSION = "11.4.0"
+QPDF_VERSION = "11.4.0"
 QPDF_PATTERN = "https://github.com/qpdf/qpdf/releases/download/vVERSION/qpdf-VERSION.tar.gz"
 
 [tool.cibuildwheel.linux]
 before-all = [
   "yum install -y wget libxml2-devel libxslt-devel libjpeg-turbo-devel zlib-devel",
   "bash build-scripts/linux-install-libxmp.bash",
   "bash build-scripts/linux-download-qpdf.bash $QPDF_VERSION",
   "bash build-scripts/linux-build-wheel-deps.bash"
 ]
 environment-pass = ["CI"]
 manylinux-x86_64-image = "manylinux2014"
-manylinux-i686-image = "manylinux2014"
 manylinux-pypy_x86_64-image = "manylinux2014"
-manylinux-pypy_i686-image = "manylinux2014"
 # Status of exotic images as of 2022-07
 # musllinux: see below
 # pp*-manylinux*_aarch64: no Pillow pypy-aarch64 wheels yet
 
 [[tool.cibuildwheel.overrides]]
 # musllinux image was based on Alpine 3.12
 # We need Alpine 3.16 or newer to get newer required package versions
@@ -222,13 +221,14 @@
 ]
 ignore = ["D105"]  # docstring in magic method
 src = ["src"]
 target-version = "py38"
 
 [tool.ruff.isort]
 known-first-party = ["pikepdf._core"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "tests/*test*.py" = ["D", "E501"]
```

### Comparing `pikepdf-7.2.0/setup.py` & `pikepdf-8.0.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 # Use cast because mypy has trouble seeing Pybind11Extension is a subclass of
 # Extension.
 extmodule: Extension = cast(
     Extension,
     Pybind11Extension(
         'pikepdf._core',
-        sorted(glob('src/core/*.cpp')),
+        sources=sorted(glob('src/core/*.cpp')),
         depends=sorted(glob('src/core/*.h')),
         include_dirs=[
             # Path to pybind11 headers
             *extra_includes,
         ],
         define_macros=[('POINTERHOLDER_TRANSITION', '4')],
         library_dirs=[*extra_library_dirs],
```

### Comparing `pikepdf-7.2.0/src/core/annotation.cpp` & `pikepdf-8.0.0rc2/src/core/annotation.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/embeddedfiles.cpp` & `pikepdf-8.0.0rc2/src/core/embeddedfiles.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/gsl.h` & `pikepdf-8.0.0rc2/src/core/gsl.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // SPDX-FileCopyrightText: 2015 Microsoft Corporation. All rights reserved.
 
 // SPDX-License-Identifier: MIT
 
 // Simplified from
-// https://raw.githubusercontent.com/microsoft/GSL/master/include/gsl/util
+// https://raw.githubusercontent.com/microsoft/GSL/main/include/gsl/util
 
 #pragma once
 
 #include <utility>
 
 namespace gsl {
```

### Comparing `pikepdf-7.2.0/src/core/jbig2-inl.h` & `pikepdf-8.0.0rc2/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/job.cpp` & `pikepdf-8.0.0rc2/src/core/job.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/logger.cpp` & `pikepdf-8.0.0rc2/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/mmap_inputsource-inl.h` & `pikepdf-8.0.0rc2/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/nametree.cpp` & `pikepdf-8.0.0rc2/src/core/nametree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/numbertree.cpp` & `pikepdf-8.0.0rc2/src/core/numbertree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/object.cpp` & `pikepdf-8.0.0rc2/src/core/object.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/object_convert.cpp` & `pikepdf-8.0.0rc2/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/object_repr.cpp` & `pikepdf-8.0.0rc2/src/core/object_repr.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -118,47 +118,51 @@
     auto pythonic_typename = objecthandle_pythonic_typename(h);
     if (pythonic_typename.empty()) {
         return objecthandle_scalar_value(h);
     }
     return objecthandle_pythonic_typename(h) + "(" + objecthandle_scalar_value(h) + ")";
 }
 
-std::string peek_stream_data(QPDFObjectHandle h, uint recursion_depth)
+std::string preview_stream_data(QPDFObjectHandle h, uint recursion_depth)
 {
+    // If we are looking at the top level object, decode a stream of up to
+    // MAX_BUFFER_TO_EXPAND and display up to MAX_PEEK_BYTES.
+
     const uint MAX_PEEK_RECURSION_DEPTH = 1;
     const size_t MAX_PEEK_BYTES         = 20;
+    const size_t MAX_BUFFER_TO_EXPAND   = 10000;
 
-    std::ostringstream ss;
-    ss.imbue(std::locale::classic());
+    std::string s;
 
-    if (recursion_depth > MAX_PEEK_RECURSION_DEPTH) {
-        ss << "<...>";
-        return ss.str();
+    unsigned long long stream_length;
+    if (recursion_depth > MAX_PEEK_RECURSION_DEPTH ||
+        !h.getDict().getKeyIfDict("/Length").getValueAsUInt(stream_length) ||
+        stream_length > MAX_BUFFER_TO_EXPAND) {
+        return "<...>";
     }
 
     auto buffer = h.getStreamData();
     auto data   = buffer->getBuffer();
-    std::string data_str(reinterpret_cast<const char *>(data),
-        std::min(MAX_PEEK_BYTES, buffer->getSize()));
 
-    py::bytes pydata(data_str); // Use py::bytes to format output like Python does
+    // Use py::bytes to format output like Python does
+    py::bytes pydata(reinterpret_cast<const char *>(data),
+        std::min(MAX_PEEK_BYTES, buffer->getSize()));
+    s = std::string(py::repr(pydata));
     if (buffer->getSize() > MAX_PEEK_BYTES) {
-        ss << py::repr(pydata) << "...";
-    } else {
-        ss << py::repr(pydata);
+        s += "...";
     }
-    return ss.str();
+    return s;
 }
 
 static std::string objecthandle_repr_inner(QPDFObjectHandle h,
     uint recursion_depth,
     uint indent_depth,
-    uint &object_count,            // shared between recursive calls
-    std::set<QPDFObjGen> &visited, // shared between recursive calls
-    bool &pure_expr)               // shared between recursive calls
+    uint &object_count,            // shared among recursive calls
+    std::set<QPDFObjGen> &visited, // shared among recursive calls
+    bool &pure_expr)               // shared among recursive calls
 {
     const uint MAX_OBJECT_COUNT = 40;
 
     StackGuard sg(" objecthandle_repr_inner");
     std::ostringstream ss;
     ss.imbue(std::locale::classic());
 
@@ -262,15 +266,15 @@
         ss << std::string(indent_depth * 2, ' ') // Restore previous indent level
            << "}";
         break;
     case qpdf_object_type_e::ot_stream:
         pure_expr = false;
         ss << objecthandle_pythonic_typename(h) << "("
            << "owner=<...>, "
-           << "data=" << peek_stream_data(h, recursion_depth) << ", "
+           << "data=" << preview_stream_data(h, recursion_depth) << ", "
            << objecthandle_repr_inner(h.getDict(),
                   recursion_depth + 1,
                   indent_depth, // Don't indent here to align dict with stream
                   object_count,
                   visited,
                   pure_expr)
            << ")";
```

### Comparing `pikepdf-7.2.0/src/core/page.cpp` & `pikepdf-8.0.0rc2/src/core/page.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/parsers.cpp` & `pikepdf-8.0.0rc2/src/core/parsers.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/parsers.h` & `pikepdf-8.0.0rc2/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/pikepdf.cpp` & `pikepdf-8.0.0rc2/src/core/pikepdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/pikepdf.h` & `pikepdf-8.0.0rc2/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/pipeline.cpp` & `pikepdf-8.0.0rc2/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/pipeline.h` & `pikepdf-8.0.0rc2/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/qpdf.cpp` & `pikepdf-8.0.0rc2/src/core/qpdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/qpdf_inputsource-inl.h` & `pikepdf-8.0.0rc2/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/qpdf_pagelist.cpp` & `pikepdf-8.0.0rc2/src/core/qpdf_pagelist.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/qpdf_pagelist.h` & `pikepdf-8.0.0rc2/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/rectangle.cpp` & `pikepdf-8.0.0rc2/src/core/rectangle.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/tokenfilter.cpp` & `pikepdf-8.0.0rc2/src/core/tokenfilter.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/utils.cpp` & `pikepdf-8.0.0rc2/src/core/utils.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/core/utils.h` & `pikepdf-8.0.0rc2/src/core/utils.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/__init__.py` & `pikepdf-8.0.0rc2/src/pikepdf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 
 """A library for manipulating PDFs."""
 
 # isort:skip_file
 
 from __future__ import annotations
 
+__version__ = "8.0.0rc2"
+
 try:
     from . import _core
 except ImportError as _e:  # pragma: no cover
     _msg = "pikepdf's extension library failed to import"
     raise ImportError(_msg) from _e
 
-try:
-    from ._version import __version__
-except ImportError as _e:  # pragma: no cover
-    raise ImportError("Failed to determine version") from _e
-
 from ._core import (
     AccessMode,
     Annotation,
     AttachedFileSpec,
     ContentStreamInlineImage,
     ContentStreamInstruction,
     DataDecodingError,
```

### Comparing `pikepdf-7.2.0/src/pikepdf/_augments.py` & `pikepdf-8.0.0rc2/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/_cpphelpers.py` & `pikepdf-8.0.0rc2/src/pikepdf/_cpphelpers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/_methods.py` & `pikepdf-8.0.0rc2/src/pikepdf/_methods.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/_qpdf.py` & `pikepdf-8.0.0rc2/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/_xml.py` & `pikepdf-8.0.0rc2/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/codec.py` & `pikepdf-8.0.0rc2/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/jbig2.py` & `pikepdf-8.0.0rc2/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/__init__.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/_content_stream.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/_content_stream.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/_transcoding.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/encryption.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/encryption.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/image.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,15 +533,15 @@
                 palette,
             )
         else:
             im = _transcoding.image_from_byte_buffer(buffer, self.size, stride)
         return im
 
     def _extract_transcoded_1bit(self) -> Image.Image:
-        if self.mode in ('RGB', 'CMYK'):
+        if not self.image_mask and self.mode in ('RGB', 'CMYK'):
             raise UnsupportedImageTypeError("1-bit RGB and CMYK are not supported")
         try:
             data = self.read_bytes()
         except (RuntimeError, PdfError) as e:
             if (
                 'read_bytes called on unfilterable stream' in str(e)
                 and not jbig2.get_decoder().available()
@@ -556,15 +556,21 @@
 
         if self.palette is not None:
             base_mode, palette = self.palette
             im = _transcoding.fix_1bit_palette_image(im, base_mode, palette)
 
         return im
 
+    def _extract_transcoded_mask(self) -> Image.Image:
+        return self._extract_transcoded_1bit()
+
     def _extract_transcoded(self) -> Image.Image:
+        if self.image_mask:
+            return self._extract_transcoded_mask()
+
         if self.mode in {'DeviceN', 'Separation'}:
             raise HifiPrintImageNotTranscodableError()
 
         if self.mode == 'RGB' and self.bits_per_component == 8:
             # Cannot use the zero-copy .get_stream_buffer here, we have 3-byte
             # RGB and Pillow needs RGBX.
             im = Image.frombuffer(
```

### Comparing `pikepdf-7.2.0/src/pikepdf/models/matrix.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf/models/metadata.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,18 +124,19 @@
 )
 
 # These are the illegal characters in XML 1.0. (XML 1.1 is a bit more permissive,
 # but we'll be strict to ensure wider compatibility.)
 re_xml_illegal_chars = re.compile(
     r"(?u)[^\x09\x0A\x0D\x20-\U0000D7FF\U0000E000-\U0000FFFD\U00010000-\U0010FFFF]"
 )
-re_xml_illegal_bytes = re.compile(
-    br"[^\x09\x0A\x0D\x20-\xFF]|&#0;"
-    # br"&#(?:[0-9]|0[0-9]|1[0-9]|2[0-9]|3[0-1]|x[0-9A-Fa-f]|x0[0-9A-Fa-f]|x1[0-9A-Fa-f]);"
-)
+re_xml_illegal_bytes = re.compile(br"[^\x09\x0A\x0D\x20-\xFF]|&#0;")
+
+# Might want to check re_xml_illegal_bytes for patterns such as:
+# br"&#(?:[0-9]|0[0-9]|1[0-9]|2[0-9]|3[0-1]
+#   |x[0-9A-Fa-f]|x0[0-9A-Fa-f]|x1[0-9A-Fa-f]);"
 
 
 def _parser_basic(xml: bytes):
     return parse_xml(BytesIO(xml))
 
 
 def _parser_strip_illegal_bytes(xml: bytes):
@@ -255,15 +256,15 @@
         XMP supports multiple author values, while DocumentInfo has a string,
         so we return the values separated by semi-colons.
         """
         if isinstance(xmp_val, str):
             return xmp_val
         if xmp_val is None or xmp_val == [None]:
             return None
-        return '; '.join(xmp_val)
+        return '; '.join(author for author in xmp_val if author is not None)
 
 
 class DateConverter(Converter):
     """Convert XMP dates to DocumentInfo."""
 
     @staticmethod
     def xmp_from_docinfo(docinfo_val):
```

### Comparing `pikepdf-7.2.0/src/pikepdf/models/outlines.py` & `pikepdf-8.0.0rc2/src/pikepdf/models/outlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,13 +416,34 @@
         if Name.Outlines not in self._pdf.Root:
             return
         outlines = self._pdf.Root.Outlines or {}
         first_obj = outlines.get(Name.First)
         if first_obj:
             self._load_level_outline(first_obj, root, 0, set())
 
+    def add(self, title: str, destination: Array | int | None) -> OutlineItem:
+        """Add an item to the outline.
+
+        Arguments:
+            title: Title of the outline item.
+            destination: Destination to jump to when the item is selected.
+
+        Returns:
+            The newly created :class:`OutlineItem`.
+        """
+        if self._root is None:
+            self._load()
+        item = OutlineItem(title, destination)
+        if self._root is None:
+            self._root = [item]
+        else:
+            self._root.append(item)
+        if not self._updating:
+            self._save()
+        return item
+
     @property
     def root(self) -> list[OutlineItem]:
         """Return the root node of the outline."""
         if self._root is None:
             self._load()
         return cast(List[OutlineItem], self._root)
```

### Comparing `pikepdf-7.2.0/src/pikepdf/objects.py` & `pikepdf-8.0.0rc2/src/pikepdf/objects.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-8.0.0rc2/src/pikepdf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 7.2.0
+Version: 8.0.0rc2
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
@@ -16,28 +16,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: mypy
 Provides-Extra: test
 License-File: LICENSE.txt
 
 <!-- SPDX-FileCopyrightText: 2022 James R. Barlow -->
 <!-- SPDX-License-Identifier: MPL-2.0 -->
 
 pikepdf
 =======
 
 **pikepdf** is a Python library for reading and writing PDF files.
 
-[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
+[![Build Status](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml/badge.svg)](https://github.com/pikepdf/pikepdf/actions/workflows/build.yml) [![PyPI](https://img.shields.io/pypi/v/pikepdf.svg)](https://pypi.org/project/pikepdf/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pikepdf) ![PyPy](https://img.shields.io/badge/PyPy-3.8%20|%203.9-blue) ![PyPI - License](https://img.shields.io/pypi/l/pikepdf) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pikepdf)  [![codecov](https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J)](https://codecov.io/gh/pikepdf/pikepdf)
 
 pikepdf is based on [QPDF](https://github.com/qpdf/qpdf), a powerful PDF manipulation and repair library.
 
 Python + QPDF = "py" + "qpdf" = "pyqpdf", which looks like a dyslexia test. Say it out loud, and it sounds like "pikepdf".
 
 ```python
 # Elegant, Pythonic API
@@ -74,15 +75,15 @@
 | Creates linearized ("fast web view") PDFs                           | ✔                                           | ✘                                         |
 | Test suite coverage                                                 | ![codecov][codecov]                         | ![codecovpypdf2][codecovpypdf]            |
 | Creates PDFs that pass PDF validation tests                         | ✔                                           | ✘                                         |
 | Modifies PDF/A without breaking PDF/A compliance                    | ✔                                           | ✘                                         |
 | PDF XMP metadata editing                                            | ✔                                           | read-only                                 |
 | Integrates with Jupyter and IPython notebooks for rapid development | ✔                                           | ✘                                         |
 
-[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/master/graph/badge.svg?token=8FJ755317J
+[codecov]: https://codecov.io/gh/pikepdf/pikepdf/branch/main/graph/badge.svg?token=8FJ755317J
 
 [codecovpypdf]: https://codecov.io/gh/py-pdf/pypdf/branch/main/graph/badge.svg?token=id42cGNZ5Z
 
 Testimonials
 ------------
 
 > I decided to try writing a quick Python program with pikepdf to automate [something] and it "just worked". –Jay Berkenbilt, creator of QPDF
```

### Comparing `pikepdf-7.2.0/src/pikepdf.egg-info/requires.txt` & `pikepdf-8.0.0rc2/src/pikepdf.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Pillow>=9.0
 deprecation
 lxml>=4.8
 packaging
 
+[:platform_python_implementation == "PyPy"]
+Pillow<10
+
+[dev]
+pre-commit
+typer[all]
+
 [docs]
 GitPython
 PyGithub
 Sphinx>=3
 ipython
 matplotlib
 pybind11
 requests
-setuptools-scm
 sphinx-design
 sphinx-issues
 sphinx-rtd-theme
 
 [docs:python_version < "3.11"]
 tomli
 
@@ -25,14 +31,15 @@
 types-requests
 types-setuptools
 
 [test]
 attrs>=20.2.0
 coverage[toml]
 hypothesis>=6.36
+numpy>=1.21.0
 psutil>=5.9
 pybind11
 pytest>=6.2.5
 pytest-cov>=3.0.0
 pytest-timeout>=2.1.0
 pytest-xdist>=2.5.0
 python-dateutil>=2.8.1
```

### Comparing `pikepdf-7.2.0/tests/test_annotation.py` & `pikepdf-8.0.0rc2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_attachments.py` & `pikepdf-8.0.0rc2/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_augments.py` & `pikepdf-8.0.0rc2/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_codec.py` & `pikepdf-8.0.0rc2/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_decimal.py` & `pikepdf-8.0.0rc2/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_dictionary.py` & `pikepdf-8.0.0rc2/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_encrypt.py` & `pikepdf-8.0.0rc2/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_errors.py` & `pikepdf-8.0.0rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_filters.py` & `pikepdf-8.0.0rc2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_foreign.py` & `pikepdf-8.0.0rc2/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_formxobject.py` & `pikepdf-8.0.0rc2/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_image_access.py` & `pikepdf-8.0.0rc2/tests/test_image_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1228,7 +1228,61 @@
     assert not diff.getbbox()
     # if diff.getbbox():
     #     im.save('im1.png')
     #     im_roundtrip.save('im2.png')
     #     diff.save('imdiff.png')
     #     breakpoint()
     #     assert False
+
+
+class StencilMaskSpec(NamedTuple):
+    width: int
+    height: int
+    imbytes: bytes
+
+    def to_pdf(self):
+        pdf = pikepdf.new()
+        pdfw, pdfh = 36 * self.width, 36 * self.height
+
+        pdf.add_blank_page(page_size=(pdfw, pdfh))
+
+        imobj = Stream(
+            pdf,
+            self.imbytes,
+            Width=self.width,
+            Height=self.height,
+            Type=Name.XObject,
+            Subtype=Name.Image,
+            ImageMask=True,
+        )
+
+        pdf.pages[0].Contents = Stream(
+            pdf, b'%f 0 0 %f 0 0 cm 0.5 0.75 1.0 rg /Im0 Do' % (pdfw, pdfh)
+        )
+        pdf.pages[0].Resources = Dictionary(XObject=Dictionary(Im0=imobj))
+        pdf.pages[0].MediaBox = Array([0, 0, pdfw, pdfh])
+        return pdf
+
+
+@st.composite
+def valid_random_stencil_mask_spec(
+    draw,
+    widths=st.integers(min_value=1, max_value=16),
+    heights=st.integers(min_value=1, max_value=16),
+):
+    width = draw(widths)
+    height = draw(heights)
+
+    min_imbytes = _next_multiple(width, 8) * height // 8
+    imbytes = draw(st.binary(min_size=min_imbytes, max_size=min_imbytes))
+
+    return StencilMaskSpec(width, height, imbytes)
+
+
+@given(spec=valid_random_stencil_mask_spec())
+def test_extract_stencil_mask(spec):
+    pdf = spec.to_pdf()
+    pim = PdfImage(pdf.pages[0].Resources.XObject.Im0)
+    bio = BytesIO()
+    pim.extract_to(stream=bio)
+    im = Image.open(bio)
+    assert im.mode == '1'
```

### Comparing `pikepdf-7.2.0/tests/test_io.py` & `pikepdf-8.0.0rc2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_ipython.py` & `pikepdf-8.0.0rc2/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_job.py` & `pikepdf-8.0.0rc2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_matrix.py` & `pikepdf-8.0.0rc2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_metadata.py` & `pikepdf-8.0.0rc2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_nametree.py` & `pikepdf-8.0.0rc2/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_numbertree.py` & `pikepdf-8.0.0rc2/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_object.py` & `pikepdf-8.0.0rc2/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_objectlist.py` & `pikepdf-8.0.0rc2/tests/test_objectlist.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_outlines.py` & `pikepdf-8.0.0rc2/tests/test_outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_page.py` & `pikepdf-8.0.0rc2/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_pages.py` & `pikepdf-8.0.0rc2/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_parsers.py` & `pikepdf-8.0.0rc2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_pdf.py` & `pikepdf-8.0.0rc2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_pdfa.py` & `pikepdf-8.0.0rc2/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_private_pdfs.py` & `pikepdf-8.0.0rc2/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_rectangle.py` & `pikepdf-8.0.0rc2/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_refcount.py` & `pikepdf-8.0.0rc2/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.2.0/tests/test_repr.py` & `pikepdf-8.0.0rc2/tests/test_repr.py`

 * *Files 16% similar despite different names*

```diff
@@ -116,16 +116,17 @@
 def dequote(s):
     # Elide the difference between b"" and b''
     return s.replace('"', '').replace("'", '')
 
 
 @given(binary(min_size=0, max_size=300))
 @example(b'hi')
+@example(b'\x00\x00\x00\t \'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"')
 def test_repr_stream(data):
     with pikepdf.new() as pdf:
-        pdf.Root.Stream = pikepdf.Stream(pdf, data, {'/Type': '/Example'})
+        pdf.Root.Stream = pikepdf.Stream(pdf, data, {'/Type': '/Example', '/Length': 2})
         assert '/Example' in repr(pdf.Root.Stream)
 
         if len(data) <= 20:
             assert dequote(repr(data)) in dequote(repr(pdf.Root.Stream))
         else:
-            assert dequote(repr(data)[:20]) in dequote(repr(pdf.Root.Stream))
+            assert dequote(repr(data)[:18]) in dequote(repr(pdf.Root.Stream))
```

### Comparing `pikepdf-7.2.0/tests/test_sanity.py` & `pikepdf-8.0.0rc2/tests/test_sanity.py`

 * *Files identical despite different names*

