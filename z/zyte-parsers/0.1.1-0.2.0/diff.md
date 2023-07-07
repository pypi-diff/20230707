# Comparing `tmp/zyte-parsers-0.1.1.tar.gz` & `tmp/zyte-parsers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-parsers-0.1.1.tar", last modified: Wed May 24 13:30:22 2023, max compression
+gzip compressed data, was "zyte-parsers-0.2.0.tar", last modified: Fri Jul  7 13:52:30 2023, max compression
```

## Comparing `zyte-parsers-0.1.1.tar` & `zyte-parsers-0.2.0.tar`

### file list

```diff
@@ -1,318 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.895779 zyte-parsers-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-24 13:30:22.895779 zyte-parsers-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:30:22.895779 zyte-parsers-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.827779 zyte-parsers-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.827779 zyte-parsers-0.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   165805 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_extract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.831779 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/anchors1.html
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/anchors2.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.891779 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0001.html
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0002.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0003.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0004.html
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0005.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0006.html
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0007.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0009.html
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0010.html
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0011.html
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0012.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0013.html
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0014.html
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0015.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0016.html
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0017.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0018.html
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0019.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0020.html
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0021.html
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0022.html
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0024.html
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0027.html
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0028.html
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0029.html
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0030.html
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0032.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0034.html
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0035.html
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0036.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0038.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0039.html
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0040.html
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0041.html
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0042.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0043.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0044.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0045.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0046.html
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0047.html
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0048.html
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0049.html
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0050.html
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0051.html
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0052.html
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0053.html
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0054.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0055.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0056.html
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0057.html
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0058.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0059.html
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0060.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0061.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0062.html
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0063.html
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0064.html
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0065.html
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0066.html
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0068.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0069.html
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0070.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0071.html
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0072.html
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0073.html
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0074.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0076.html
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0077.html
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0078.html
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0079.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0081.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0082.html
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0083.html
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0084.html
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0085.html
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0086.html
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0087.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0088.html
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0089.html
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0090.html
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0091.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0092.html
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0093.html
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0094.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0095.html
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0096.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0097.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0098.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0099.html
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0100.html
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0102.html
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0103.html
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0104.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0105.html
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0106.html
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0107.html
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0108.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0109.html
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0110.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0111.html
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0112.html
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0113.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0114.html
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0115.html
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0117.html
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0118.html
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0120.html
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0122.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0124.html
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0125.html
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0127.html
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0128.html
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0129.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0130.html
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0131.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0132.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0133.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0134.html
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0135.html
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0136.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0137.html
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0138.html
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0139.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0140.html
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0142.html
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0143.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0144.html
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0145.html
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0146.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0147.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0148.html
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0149.html
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0150.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0151.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0152.html
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0153.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0154.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0156.html
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0157.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0158.html
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0159.html
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0161.html
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0162.html
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0163.html
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0164.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0165.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0167.html
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0168.html
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0169.html
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0170.html
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0171.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0172.html
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0173.html
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0174.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0175.html
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0177.html
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0178.html
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0179.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0180.html
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0182.html
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0183.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0184.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0185.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0186.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0187.html
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0188.html
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0189.html
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0190.html
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0191.html
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0192.html
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0193.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0194.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0195.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0196.html
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0197.html
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0199.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0200.html
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0201.html
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0202.html
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0203.html
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0204.html
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0205.html
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0206.html
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0207.html
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0208.html
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0209.html
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0210.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0211.html
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0212.html
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0213.html
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0214.html
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0215.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0216.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0217.html
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0218.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0219.html
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0220.html
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0221.html
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0222.html
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0223.html
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0224.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0225.html
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0226.html
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0227.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0228.html
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0229.html
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0230.html
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0232.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0233.html
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0234.html
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0235.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0236.html
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0237.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0238.html
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0239.html
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0240.html
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0241.html
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0242.html
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0243.html
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0244.html
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0245.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0246.html
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0247.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0248.html
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0249.html
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0250.html
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0251.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0252.html
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0253.html
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0254.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0255.html
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0256.html
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0257.html
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0258.html
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0259.html
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0262.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0263.html
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0264.html
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0265.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0268.html
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0269.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0270.html
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0271.html
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0272.html
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0273.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0274.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0275.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0277.html
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0278.html
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0279.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0280.html
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0281.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0283.html
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0284.html
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0285.html
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0286.html
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0287.html
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0288.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0289.html
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0290.html
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0292.html
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0293.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0294.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0295.html
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0296.html
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0297.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0298.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0299.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0300.html
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/include-non-anchor.html
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-data-vocabulary.html
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-ul-element1.html
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-ul-element2.html
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/self-link.html
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/semantic-markup.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet1.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet2.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet3.html
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet4.html
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet5.html
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet6.html
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet7.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet8.html
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/td-element.html
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/ul-element.html
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/with-drop-down.html
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/with-drop-down2.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/test_breadcrumbs.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.895779 zyte-parsers-0.1.1/zyte_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/zyte_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/zyte_parsers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/zyte_parsers/breadcrumbs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/zyte_parsers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 13:30:01.000000 zyte-parsers-0.1.1/zyte_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:30:22.895779 zyte-parsers-0.1.1/zyte_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-24 13:30:22.000000 zyte-parsers-0.1.1/zyte_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-24 13:30:22.000000 zyte-parsers-0.1.1/zyte_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:30:22.000000 zyte-parsers-0.1.1/zyte_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 13:30:22.000000 zyte-parsers-0.1.1/zyte_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:30:22.000000 zyte-parsers-0.1.1/zyte_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.459575 zyte-parsers-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-07 13:52:30.459575 zyte-parsers-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:52:30.459575 zyte-parsers-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.403572 zyte-parsers-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.403572 zyte-parsers-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1180171 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/brand_values.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165805 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_extract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.411573 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/anchors1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/anchors2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.455575 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0001.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0002.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0003.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0004.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0005.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0006.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0007.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0009.html
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0010.html
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0011.html
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0012.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0013.html
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0014.html
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0015.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0016.html
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0017.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0018.html
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0019.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0020.html
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0021.html
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0022.html
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0024.html
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0027.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0028.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0029.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0030.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0032.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0034.html
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0035.html
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0036.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0038.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0039.html
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0040.html
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0041.html
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0042.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0043.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0044.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0045.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0046.html
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0047.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0048.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0049.html
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0050.html
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0051.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0052.html
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0053.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0054.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0055.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0056.html
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0057.html
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0058.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0059.html
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0060.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0061.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0062.html
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0063.html
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0064.html
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0065.html
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0066.html
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0068.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0069.html
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0070.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0071.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0072.html
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0073.html
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0074.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0076.html
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0077.html
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0078.html
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0079.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0081.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0082.html
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0083.html
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0084.html
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0085.html
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0086.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0087.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0088.html
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0089.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0090.html
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0091.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0092.html
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0093.html
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0094.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0095.html
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0096.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0097.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0098.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0099.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0100.html
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0102.html
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0103.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0104.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0105.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0106.html
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0107.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0108.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0109.html
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0110.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0111.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0112.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0113.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0114.html
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0115.html
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0117.html
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0118.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0120.html
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0122.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0124.html
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0125.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0127.html
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0128.html
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0129.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0130.html
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0131.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0132.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0133.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0134.html
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0135.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0136.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0137.html
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0138.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0139.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0140.html
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0142.html
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0143.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0144.html
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0145.html
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0146.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0147.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0148.html
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0149.html
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0150.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0151.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0152.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0153.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0154.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0156.html
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0157.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0158.html
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0159.html
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0161.html
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0162.html
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0163.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0164.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0165.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0167.html
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0168.html
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0169.html
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0170.html
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0171.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0172.html
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0173.html
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0174.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0175.html
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0177.html
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0178.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0179.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0180.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0182.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0183.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0184.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0185.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0186.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0187.html
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0188.html
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0189.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0190.html
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0191.html
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0192.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0193.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0194.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0195.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0196.html
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0197.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0199.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0200.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0201.html
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0202.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0203.html
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0204.html
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0205.html
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0206.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0207.html
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0208.html
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0209.html
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0210.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0211.html
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0212.html
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0213.html
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0214.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0215.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0216.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0217.html
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0218.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0219.html
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0220.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0221.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0222.html
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0223.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0224.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0225.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0226.html
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0227.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0228.html
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0229.html
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0230.html
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0232.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0233.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0234.html
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0235.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0236.html
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0237.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0238.html
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0239.html
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0240.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0241.html
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0242.html
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0243.html
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0244.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0245.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0246.html
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0247.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0248.html
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0249.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0250.html
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0251.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0252.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0253.html
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0254.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0255.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0256.html
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0257.html
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0258.html
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0259.html
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0262.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0263.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0264.html
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0265.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0268.html
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0269.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0270.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0271.html
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0272.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0273.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0274.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0275.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0277.html
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0278.html
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0279.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0280.html
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0281.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0283.html
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0284.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0285.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0286.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0287.html
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0288.html
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0289.html
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0290.html
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0292.html
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0293.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0294.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0295.html
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0296.html
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0297.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0298.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0299.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0300.html
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/include-non-anchor.html
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-data-vocabulary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-ul-element1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-ul-element2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/self-link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/semantic-markup.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet3.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet4.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet5.html
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet6.html
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet7.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet8.html
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/td-element.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/ul-element.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/with-drop-down.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/with-drop-down2.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/test_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/test_breadcrumbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.459575 zyte-parsers-0.2.0/zyte_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/breadcrumbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-07 13:52:05.000000 zyte-parsers-0.2.0/zyte_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:52:30.459575 zyte-parsers-0.2.0/zyte_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-07 13:52:30.000000 zyte-parsers-0.2.0/zyte_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-07-07 13:52:30.000000 zyte-parsers-0.2.0/zyte_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:52:30.000000 zyte-parsers-0.2.0/zyte_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 13:52:30.000000 zyte-parsers-0.2.0/zyte_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 13:52:30.000000 zyte-parsers-0.2.0/zyte_parsers.egg-info/top_level.txt
```

### Comparing `zyte-parsers-0.1.1/LICENSE` & `zyte-parsers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/PKG-INFO` & `zyte-parsers-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-parsers
-Version: 0.1.1
+Version: 0.2.0
 Summary: Parsing of data from web pages.
 Author-email: Zyte Group Ltd <info@zyte.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Zyte Group Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,21 +28,20 @@
 Project-URL: Source, https://github.com/zytedata/zyte-parsers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 zyte-parsers
 ============
```

### Comparing `zyte-parsers-0.1.1/README.rst` & `zyte-parsers-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/pyproject.toml` & `zyte-parsers-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "attrs>=21.3.0",
     "html-text",
     "lxml",
     "parsel",
     "w3lib",
 ]
```

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_extract.json` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_extract.json`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/anchors1.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/anchors1.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0002.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0002.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0003.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0003.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0007.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0007.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0010.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0010.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0012.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0012.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0015.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0015.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0017.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0017.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0018.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0018.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0019.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0019.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0021.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0021.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0024.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0024.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0027.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0027.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0028.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0028.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0029.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0029.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0030.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0030.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0032.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0032.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0036.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0036.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0039.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0039.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0041.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0041.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0042.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0042.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0043.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0043.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0046.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0046.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0048.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0048.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0050.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0050.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0051.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0051.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0052.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0052.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0053.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0053.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0054.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0054.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0060.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0060.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0063.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0063.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0066.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0066.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0070.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0070.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0072.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0072.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0076.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0076.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0077.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0077.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0078.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0078.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0079.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0079.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0083.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0083.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0084.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0084.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0085.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0085.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0086.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0086.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0087.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0087.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0088.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0088.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0089.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0089.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0090.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0090.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0091.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0091.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0097.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0097.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0104.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0104.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0106.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0106.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0107.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0107.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0108.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0108.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0111.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0111.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0112.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0112.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0113.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0113.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0117.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0117.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0118.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0118.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0120.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0120.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0127.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0127.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0128.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0128.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0129.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0129.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0130.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0130.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0131.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0131.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0132.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0132.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0134.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0134.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0135.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0135.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0136.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0136.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0138.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0138.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0139.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0139.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0142.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0142.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0146.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0146.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0147.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0147.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0149.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0149.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0153.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0153.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0154.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0154.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0157.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0157.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0159.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0159.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0161.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0161.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0163.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0163.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0164.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0164.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0169.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0169.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0171.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0171.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0172.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0172.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0174.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0174.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0177.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0177.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0178.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0178.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0182.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0182.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0183.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0183.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0184.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0184.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0185.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0185.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0188.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0188.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0190.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0190.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0193.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0193.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0196.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0196.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0197.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0197.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0199.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0199.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0203.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0203.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0205.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0205.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0207.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0207.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0210.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0210.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0212.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0212.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0215.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0215.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0217.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0217.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0222.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0222.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0223.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0223.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0224.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0224.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0226.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0226.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0229.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0229.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0232.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0232.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0234.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0234.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0235.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0235.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0237.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0237.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0244.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0244.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0245.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0245.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0247.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0247.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0248.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0248.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0250.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0250.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0253.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0253.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0256.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0256.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0257.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0257.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0259.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0259.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0264.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0264.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0271.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0271.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0272.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0272.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0273.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0273.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0277.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0277.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0278.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0278.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0279.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0279.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0281.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0281.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0284.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0284.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0287.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0287.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0288.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0288.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0289.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0289.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0290.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0290.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0298.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0298.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0299.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0299.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/generated/snippet0300.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/generated/snippet0300.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-data-vocabulary.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-data-vocabulary.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-ul-element1.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-ul-element1.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/nested-ul-element2.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/nested-ul-element2.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/semantic-markup.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/semantic-markup.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet4.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet4.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet5.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet5.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet6.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet6.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/snippet7.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/snippet7.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/td-element.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/td-element.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/ul-element.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/ul-element.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/with-drop-down.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/with-drop-down.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/data/breadcrumb_items_snippets/with-drop-down2.html` & `zyte-parsers-0.2.0/tests/data/breadcrumb_items_snippets/with-drop-down2.html`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/tests/test_breadcrumbs.py` & `zyte-parsers-0.2.0/tests/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/zyte_parsers/api.py` & `zyte-parsers-0.2.0/zyte_parsers/api.py`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/zyte_parsers/breadcrumbs.py` & `zyte-parsers-0.2.0/zyte_parsers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `zyte-parsers-0.1.1/zyte_parsers/utils.py` & `zyte-parsers-0.2.0/zyte_parsers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import itertools
 from typing import Any, Callable, Iterable, Optional
 from urllib.parse import urljoin
 
 import html_text
-from lxml.html import fromstring  # noqa: F401
+from lxml.html import HtmlElement, fromstring  # noqa: F401
 from parsel import Selector  # noqa: F401
 from w3lib.html import strip_html5_whitespace
 
 from zyte_parsers.api import SelectorOrElement, input_to_element
 
 
 def is_js_url(url: str) -> bool:
@@ -104,7 +105,21 @@
     >>> first_satisfying([0, ""], default=2)
     2
     """
     try:
         return next(x for x in xs if condition_fun(x))
     except StopIteration:
         return default
+
+
+def iterwalk_limited(node: HtmlElement, search_depth: int) -> Iterable[HtmlElement]:
+    yield node
+
+    if search_depth <= 0:
+        return
+
+    for child in node:
+        yield from iterwalk_limited(child, search_depth - 1)
+
+
+def take(iterable: Iterable[Any], n: int):
+    return list(itertools.islice(iterable, n))
```

### Comparing `zyte-parsers-0.1.1/zyte_parsers.egg-info/PKG-INFO` & `zyte-parsers-0.2.0/zyte_parsers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-parsers
-Version: 0.1.1
+Version: 0.2.0
 Summary: Parsing of data from web pages.
 Author-email: Zyte Group Ltd <info@zyte.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Zyte Group Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,21 +28,20 @@
 Project-URL: Source, https://github.com/zytedata/zyte-parsers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 zyte-parsers
 ============
```

### Comparing `zyte-parsers-0.1.1/zyte_parsers.egg-info/SOURCES.txt` & `zyte-parsers-0.2.0/zyte_parsers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 tests/__init__.py
 tests/requirements.txt
+tests/test_brand.py
 tests/test_breadcrumbs.py
 tests/utils.py
+tests/data/brand_values.json
 tests/data/breadcrumb_items_extract.json
 tests/data/breadcrumb_items_snippets/anchors1.html
 tests/data/breadcrumb_items_snippets/anchors2.html
 tests/data/breadcrumb_items_snippets/include-non-anchor.html
 tests/data/breadcrumb_items_snippets/nested-breadcrumbs.html
 tests/data/breadcrumb_items_snippets/nested-data-vocabulary.html
 tests/data/breadcrumb_items_snippets/nested-ul-element1.html
@@ -295,14 +297,15 @@
 tests/data/breadcrumb_items_snippets/generated/snippet0296.html
 tests/data/breadcrumb_items_snippets/generated/snippet0297.html
 tests/data/breadcrumb_items_snippets/generated/snippet0298.html
 tests/data/breadcrumb_items_snippets/generated/snippet0299.html
 tests/data/breadcrumb_items_snippets/generated/snippet0300.html
 zyte_parsers/__init__.py
 zyte_parsers/api.py
+zyte_parsers/brand.py
 zyte_parsers/breadcrumbs.py
 zyte_parsers/py.typed
 zyte_parsers/utils.py
 zyte_parsers.egg-info/PKG-INFO
 zyte_parsers.egg-info/SOURCES.txt
 zyte_parsers.egg-info/dependency_links.txt
 zyte_parsers.egg-info/requires.txt
```

