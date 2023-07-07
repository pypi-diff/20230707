# Comparing `tmp/bitcoinlib-0.6.7.tar.gz` & `tmp/bitcoinlib-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoinlib-0.6.7.tar", last modified: Wed Dec 14 09:49:37 2022, max compression
+gzip compressed data, was "bitcoinlib-0.6.9.tar", last modified: Mon Mar 13 20:27:59 2023, max compression
```

## Comparing `bitcoinlib-0.6.7.tar` & `bitcoinlib-0.6.9.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.737810 bitcoinlib-0.6.7/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9017 2022-12-14 09:47:53.000000 bitcoinlib-0.6.7/CHANGELOG
--rw-r--r--   0 lennart   (1000) lennart   (1000)    35141 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/LICENSE
--rw-rw-r--   0 lennart   (1000) lennart   (1000)      366 2020-08-31 06:59:23.000000 bitcoinlib-0.6.7/MANIFEST.in
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    16258 2022-12-14 09:49:37.737810 bitcoinlib-0.6.7/PKG-INFO
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    11964 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/README.rst
--rw-r--r--   0 lennart   (1000) lennart   (1000)      881 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/__init__.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.721810 bitcoinlib-0.6.7/bitcoinlib/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     1142 2020-12-02 16:33:21.000000 bitcoinlib-0.6.7/bitcoinlib/__init__.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    28589 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/blocks.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.721810 bitcoinlib-0.6.7/bitcoinlib/config/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)        5 2022-12-14 09:49:24.000000 bitcoinlib-0.6.7/bitcoinlib/config/VERSION
--rw-r--r--   0 lennart   (1000) lennart   (1000)      976 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/config/__init__.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.721810 bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/
--rw-r--r--   0 lennart   (1000) lennart   (1000)      323 2022-06-25 14:49:13.000000 bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     6977 2022-11-19 10:49:07.000000 bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     2273 2022-06-25 14:49:13.000000 bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/opcodes.cpython-38.pyc
--rw-r--r--   0 lennart   (1000) lennart   (1000)      432 2022-06-25 14:49:13.000000 bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/secp256k1.cpython-38.pyc
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    12992 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/config/config.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     2773 2021-09-13 13:30:07.000000 bitcoinlib-0.6.7/bitcoinlib/config/opcodes.py
--rw-r--r--   0 lennart   (1000) lennart   (1000)     1501 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/config/secp256k1.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.725810 bitcoinlib-0.6.7/bitcoinlib/data/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     2267 2022-06-25 15:39:51.000000 bitcoinlib-0.6.7/bitcoinlib/data/config.ini
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     1821 2020-08-31 06:59:23.000000 bitcoinlib-0.6.7/bitcoinlib/data/config.ini.unittest
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    12826 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/bitcoinlib/data/networks.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    11141 2021-12-10 19:31:45.000000 bitcoinlib-0.6.7/bitcoinlib/data/providers.examples.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    11651 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/data/providers.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    12829 2021-09-13 13:30:07.000000 bitcoinlib-0.6.7/bitcoinlib/data/providers.old.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    24432 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/db.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9656 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/db_cache.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    34280 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/encoding.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   102277 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/keys.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     4538 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/main.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9749 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/mnemonic.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    13231 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/networks.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    42380 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/scripts.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.725810 bitcoinlib-0.6.7/bitcoinlib/services/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     1651 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/bitcoinlib/services/__init__.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     7465 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/authproxy.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     4987 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/baseclient.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     8867 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/bcoin.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9741 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/bitaps.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    13907 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/bitcoind.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     4254 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/bitcoinlib/services/bitcoinlibtest.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     3835 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/bitcoinlib/services/bitflyer.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     8358 2022-06-25 15:39:51.000000 bitcoinlib-0.6.7/bitcoinlib/services/bitgo.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     7855 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/blockchaininfo.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    10673 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/bitcoinlib/services/blockchair.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9316 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/blockcypher.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9204 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/blocksmurfer.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    10353 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/blockstream.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     7721 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/chainso.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     6389 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/cryptoid.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    10732 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/dashd.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9575 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/dogecoind.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     7896 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/insightdash.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     8170 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/litecoinblockexplorer.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    13957 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/services/litecoind.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     7943 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/litecoreio.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     9088 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/mempool.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    50848 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/services/services.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.725810 bitcoinlib-0.6.7/bitcoinlib/tools/
--rw-r--r--   0 lennart   (1000) lennart   (1000)      860 2022-02-16 14:57:38.000000 bitcoinlib-0.6.7/bitcoinlib/tools/__init__.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    19508 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/bitcoinlib/tools/clw.py
--rw-r--r--   0 lennart   (1000) lennart   (1000)      912 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/tools/mnemonic_key_create.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     1789 2020-12-02 16:33:21.000000 bitcoinlib-0.6.7/bitcoinlib/tools/sign_raw.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     5347 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/bitcoinlib/tools/wallet_multisig_2of3.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   116127 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/transactions.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    17352 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/bitcoinlib/values.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   201315 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/bitcoinlib/wallets.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.725810 bitcoinlib-0.6.7/bitcoinlib/wordlist/
--rw-r--r--   0 lennart   (1000) lennart   (1000)     8192 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/chinese_simplified.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)     8192 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/chinese_traditional.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    16254 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/dutch.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    13116 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/english.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    16777 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/french.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    16033 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/italian.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    26423 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/japanese.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)    13996 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/bitcoinlib/wordlist/spanish.txt
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.721810 bitcoinlib-0.6.7/bitcoinlib.egg-info/
--rw-r--r--   0 lennart   (1000) lennart   (1000)    16258 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/PKG-INFO
--rw-r--r--   0 lennart   (1000) lennart   (1000)     2997 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/SOURCES.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)        1 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/dependency_links.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)       90 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/entry_points.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)        1 2020-02-01 10:36:01.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/not-zip-safe
--rw-r--r--   0 lennart   (1000) lennart   (1000)      235 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/requires.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)       11 2022-12-14 09:49:37.000000 bitcoinlib-0.6.7/bitcoinlib.egg-info/top_level.txt
--rw-rw-r--   0 lennart   (1000) lennart   (1000)       88 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/requirements.txt
--rw-r--r--   0 lennart   (1000) lennart   (1000)       80 2022-12-14 09:49:37.737810 bitcoinlib-0.6.7/setup.cfg
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     3294 2022-12-14 09:49:24.000000 bitcoinlib-0.6.7/setup.py
-drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2022-12-14 09:49:37.737810 bitcoinlib-0.6.7/tests/
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     1135 2021-09-13 13:30:07.000000 bitcoinlib-0.6.7/tests/__init__.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     4785 2022-03-06 19:01:18.000000 bitcoinlib-0.6.7/tests/benchmark.py
--rw-r--r--   0 lennart   (1000) lennart   (1000)     3207 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/tests/bip38_protected_key_tests.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    95460 2020-08-31 06:59:23.000000 bitcoinlib-0.6.7/tests/block250000.pickle
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   100355 2020-08-31 06:59:23.000000 bitcoinlib-0.6.7/tests/block330000.pickle
--rw-rw-r--   0 lennart   (1000) lennart   (1000)  1276532 2021-09-13 13:30:07.000000 bitcoinlib-0.6.7/tests/block625007.pickle
--rw-rw-r--   0 lennart   (1000) lennart   (1000)  1429145 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/tests/block629999.pickle
--rw-rw-r--   0 lennart   (1000) lennart   (1000)  1497210 2022-06-25 15:39:51.000000 bitcoinlib-0.6.7/tests/block722010.pickle
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    24297 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/tests/db_0_5.py
--rw-r--r--   0 lennart   (1000) lennart   (1000)     2550 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/tests/electrum_keys.json
--rw-r--r--   0 lennart   (1000) lennart   (1000)    14180 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/tests/mnemonics_tests.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    13088 2022-06-25 15:39:51.000000 bitcoinlib-0.6.7/tests/test_blocks.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     2292 2020-08-31 06:59:23.000000 bitcoinlib-0.6.7/tests/test_custom.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     3378 2020-11-04 22:09:53.000000 bitcoinlib-0.6.7/tests/test_db.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    21447 2022-10-29 18:22:40.000000 bitcoinlib-0.6.7/tests/test_encoding.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    56200 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/tests/test_keys.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     5231 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/tests/test_mnemonic.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     3394 2021-12-10 12:35:00.000000 bitcoinlib-0.6.7/tests/test_networks.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    50645 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/tests/test_script.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    55763 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/tests/test_services.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    10424 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/tests/test_tools.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   149400 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/tests/test_transactions.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)    10737 2020-12-02 16:33:21.000000 bitcoinlib-0.6.7/tests/test_values.py
--rw-rw-r--   0 lennart   (1000) lennart   (1000)   137340 2022-12-14 09:42:11.000000 bitcoinlib-0.6.7/tests/test_wallets.py
--rw-r--r--   0 lennart   (1000) lennart   (1000)   109907 2020-02-01 09:34:11.000000 bitcoinlib-0.6.7/tests/transactions_raw.json
--rw-rw-r--   0 lennart   (1000) lennart   (1000)     4710 2020-11-04 08:25:56.000000 bitcoinlib-0.6.7/updatedb.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.896892 bitcoinlib-0.6.9/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9258 2023-03-13 20:25:59.000000 bitcoinlib-0.6.9/CHANGELOG
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    35141 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/LICENSE
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)      366 2020-08-31 06:59:23.000000 bitcoinlib-0.6.9/MANIFEST.in
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    16258 2023-03-13 20:27:59.896892 bitcoinlib-0.6.9/PKG-INFO
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    11964 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/README.rst
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      881 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/__init__.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     1142 2020-12-02 16:33:21.000000 bitcoinlib-0.6.9/bitcoinlib/__init__.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    28589 2023-02-03 15:43:44.000000 bitcoinlib-0.6.9/bitcoinlib/blocks.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/config/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)        5 2023-03-13 20:27:49.000000 bitcoinlib-0.6.9/bitcoinlib/config/VERSION
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      976 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/config/__init__.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      323 2022-06-25 14:49:13.000000 bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     6977 2023-02-03 16:04:37.000000 bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     2273 2022-06-25 14:49:13.000000 bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/opcodes.cpython-38.pyc
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      432 2022-06-25 14:49:13.000000 bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/secp256k1.cpython-38.pyc
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    12992 2023-02-03 15:43:44.000000 bitcoinlib-0.6.9/bitcoinlib/config/config.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     2773 2021-09-13 13:30:07.000000 bitcoinlib-0.6.9/bitcoinlib/config/opcodes.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     1501 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/config/secp256k1.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/data/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     2267 2022-06-25 15:39:51.000000 bitcoinlib-0.6.9/bitcoinlib/data/config.ini
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     1821 2020-08-31 06:59:23.000000 bitcoinlib-0.6.9/bitcoinlib/data/config.ini.unittest
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    12826 2022-03-06 19:01:18.000000 bitcoinlib-0.6.9/bitcoinlib/data/networks.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    13472 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/data/providers.examples.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    11978 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/data/providers.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    12829 2021-09-13 13:30:07.000000 bitcoinlib-0.6.9/bitcoinlib/data/providers.old.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    24432 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/db.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9656 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/db_cache.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    34280 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/encoding.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   102277 2023-02-03 15:43:44.000000 bitcoinlib-0.6.9/bitcoinlib/keys.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     4538 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/main.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9749 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/mnemonic.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    13231 2023-02-03 15:43:44.000000 bitcoinlib-0.6.9/bitcoinlib/networks.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    42380 2023-03-10 13:51:28.000000 bitcoinlib-0.6.9/bitcoinlib/scripts.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/services/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     1653 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/services/__init__.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7465 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/authproxy.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     4987 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/baseclient.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     8862 2023-03-10 21:27:32.000000 bitcoinlib-0.6.9/bitcoinlib/services/bcoin.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9573 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/services/bitaps.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    13907 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/bitcoind.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     4254 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/bitcoinlib/services/bitcoinlibtest.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     3835 2022-03-06 19:01:18.000000 bitcoinlib-0.6.9/bitcoinlib/services/bitflyer.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     8358 2022-06-25 15:39:51.000000 bitcoinlib-0.6.9/bitcoinlib/services/bitgo.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     6869 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/services/blockbook.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7855 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/blockchaininfo.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    10673 2022-03-06 19:01:18.000000 bitcoinlib-0.6.9/bitcoinlib/services/blockchair.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9316 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/blockcypher.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9204 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/blocksmurfer.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    10353 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/blockstream.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7721 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/chainso.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     6389 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/cryptoid.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    10732 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/dashd.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9575 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/dogecoind.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7896 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/insightdash.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7169 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/services/litecoinblockexplorer.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    13957 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/bitcoinlib/services/litecoind.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     7943 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/litecoreio.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     9088 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/mempool.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    50848 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/services/services.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/tools/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      860 2022-02-16 14:57:38.000000 bitcoinlib-0.6.9/bitcoinlib/tools/__init__.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    19508 2022-03-06 19:01:18.000000 bitcoinlib-0.6.9/bitcoinlib/tools/clw.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      912 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/tools/mnemonic_key_create.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     1777 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/tools/sign_raw.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     5347 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/bitcoinlib/tools/wallet_multisig_2of3.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   116127 2023-03-10 13:51:28.000000 bitcoinlib-0.6.9/bitcoinlib/transactions.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    17352 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/bitcoinlib/values.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   201323 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/bitcoinlib/wallets.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib/wordlist/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     8192 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/chinese_simplified.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     8192 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/chinese_traditional.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    16254 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/dutch.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    13116 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/english.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    16777 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/french.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    16033 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/italian.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    26423 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/japanese.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    13996 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/bitcoinlib/wordlist/spanish.txt
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.892892 bitcoinlib-0.6.9/bitcoinlib.egg-info/
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    16258 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/PKG-INFO
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     3030 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)        1 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       90 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/entry_points.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)        1 2020-02-01 10:36:01.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/not-zip-safe
+-rw-r--r--   0 lennart   (1000) lennart   (1000)      235 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/requires.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       11 2023-03-13 20:27:59.000000 bitcoinlib-0.6.9/bitcoinlib.egg-info/top_level.txt
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)       88 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/requirements.txt
+-rw-r--r--   0 lennart   (1000) lennart   (1000)       80 2023-03-13 20:27:59.900892 bitcoinlib-0.6.9/setup.cfg
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     3294 2023-03-13 20:27:49.000000 bitcoinlib-0.6.9/setup.py
+drwxrwxr-x   0 lennart   (1000) lennart   (1000)        0 2023-03-13 20:27:59.896892 bitcoinlib-0.6.9/tests/
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     1135 2021-09-13 13:30:07.000000 bitcoinlib-0.6.9/tests/__init__.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     4785 2022-03-06 19:01:18.000000 bitcoinlib-0.6.9/tests/benchmark.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     3207 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/tests/bip38_protected_key_tests.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    95460 2020-08-31 06:59:23.000000 bitcoinlib-0.6.9/tests/block250000.pickle
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   100355 2020-08-31 06:59:23.000000 bitcoinlib-0.6.9/tests/block330000.pickle
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)  1276532 2021-09-13 13:30:07.000000 bitcoinlib-0.6.9/tests/block625007.pickle
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)  1429145 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/tests/block629999.pickle
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)  1497210 2022-06-25 15:39:51.000000 bitcoinlib-0.6.9/tests/block722010.pickle
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    24297 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/tests/db_0_5.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)     2550 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/tests/electrum_keys.json
+-rw-r--r--   0 lennart   (1000) lennart   (1000)    14180 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/tests/mnemonics_tests.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    13088 2022-06-25 15:39:51.000000 bitcoinlib-0.6.9/tests/test_blocks.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     2292 2020-08-31 06:59:23.000000 bitcoinlib-0.6.9/tests/test_custom.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     3378 2020-11-04 22:09:53.000000 bitcoinlib-0.6.9/tests/test_db.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    21447 2022-10-29 18:22:40.000000 bitcoinlib-0.6.9/tests/test_encoding.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    56200 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/tests/test_keys.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     5231 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/tests/test_mnemonic.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     3394 2021-12-10 12:35:00.000000 bitcoinlib-0.6.9/tests/test_networks.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    50645 2022-12-14 09:42:11.000000 bitcoinlib-0.6.9/tests/test_script.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    55953 2023-03-13 20:01:27.000000 bitcoinlib-0.6.9/tests/test_services.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    10424 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/tests/test_tools.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   149400 2023-03-10 13:51:28.000000 bitcoinlib-0.6.9/tests/test_transactions.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)    10737 2020-12-02 16:33:21.000000 bitcoinlib-0.6.9/tests/test_values.py
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)   137457 2023-03-13 20:16:10.000000 bitcoinlib-0.6.9/tests/test_wallets.py
+-rw-r--r--   0 lennart   (1000) lennart   (1000)   109907 2020-02-01 09:34:11.000000 bitcoinlib-0.6.9/tests/transactions_raw.json
+-rw-rw-r--   0 lennart   (1000) lennart   (1000)     4710 2020-11-04 08:25:56.000000 bitcoinlib-0.6.9/updatedb.py
```

### Comparing `bitcoinlib-0.6.7/CHANGELOG` & `bitcoinlib-0.6.9/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+RELEASE 0.6.9 - Bugfixes and service provider update
+====================================================
+* Remove Chainso provider
+* Add Blockbook providers
+* Fix litecoinblockexplorer, bitaps provider
+* Other bugfixes and unittest issues
+
 RELEASE 0.6.7 - Fix installation, dependencies and provider issues
 ==================================================================
 * Fix installation issues
 * Use pycryptodome for Ripemd160, scrypt and AES
 * Fix Litecoin issues
 * Add support for p2tr addresses
 * Fix support for Blocksmurfer provider
```

### Comparing `bitcoinlib-0.6.7/LICENSE` & `bitcoinlib-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/PKG-INFO` & `bitcoinlib-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bitcoinlib
-Version: 0.6.7
+Version: 0.6.9
 Summary: Bitcoin and Other cryptocurrency Library
 Home-page: http://github.com/1200wd/bitcoinlib
 Author: 1200wd
 Author-email: info@1200wd.com
 License: GNU3
 Description: Python Bitcoin Library
         ======================
```

### Comparing `bitcoinlib-0.6.7/README.rst` & `bitcoinlib-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/__init__.py` & `bitcoinlib-0.6.9/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/__init__.py` & `bitcoinlib-0.6.9/bitcoinlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/blocks.py` & `bitcoinlib-0.6.9/bitcoinlib/blocks.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/__init__.py` & `bitcoinlib-0.6.9/bitcoinlib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/config.cpython-38.pyc` & `bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Nov 19 10:49:07 2022 UTC, .py size: 12992 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a3b4 7863 c032 0000  U.........xc.2..
+00000000: 550d 0d0a 0000 0000 b02b dd63 c032 0000  U........+.c.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 e802 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d07 5a07 0100 6508  ..d.d.l.m.Z...e.
 00000070: 5a09 650a 5a0b 6404 610c 6405 610d 6506  Z.e.Z.d.a.d.a.e.
@@ -58,37 +58,37 @@
 00000390: 5f45 5155 414c 5a04 4f50 5f30 7a07 6861  _EQUALZ.OP_0z.ha
 000003a0: 7368 2d33 325a 046f 705f 6e5a 046f 705f  sh-32Z.op_nZ.op_
 000003b0: 6dda 086d 756c 7469 7369 675a 104f 505f  m..multisigZ.OP_
 000003c0: 4348 4543 4b4d 554c 5449 5349 475a 0a70  CHECKMULTISIGZ.p
 000003d0: 7562 6c69 635f 6b65 795a 094f 505f 5245  ublic_keyZ.OP_RE
 000003e0: 5455 524e 5a0b 7265 7475 726e 5f64 6174  TURNZ.return_dat
 000003f0: 6129 08da 0570 3270 6b68 da04 7032 7368  a)...p2pkh..p2sh
-00000400: da06 7032 7770 6b68 da05 7032 7773 68da  ..p2wpkh..p2wsh.
+00000400: da06 7032 7770 6b68 da05 7032 7773 685a  ..p2wpkh..p2wshZ
 00000410: 0470 3274 7272 0a00 0000 5a04 7032 706b  .p2trr....Z.p2pk
 00000420: 5a08 6e75 6c6c 6461 7461 da09 7369 676e  Z.nulldata..sign
 00000430: 6174 7572 65da 0b53 4947 4841 5348 5f41  ature..SIGHASH_A
 00000440: 4c4c 5a0c 7265 6465 656d 7363 7269 7074  LLZ.redeemscript
 00000450: 5a09 7075 7368 5f73 697a 65da 0d6c 6f63  Z.push_size..loc
 00000460: 6b74 696d 655f 636c 7476 5a16 4f50 5f43  ktime_cltvZ.OP_C
 00000470: 4845 434b 4c4f 434b 5449 4d45 5645 5249  HECKLOCKTIMEVERI
 00000480: 4659 5a07 4f50 5f44 524f 50da 0c6c 6f63  FYZ.OP_DROP..loc
 00000490: 6b74 696d 655f 6373 765a 164f 505f 4348  ktime_csvZ.OP_CH
 000004a0: 4543 4b53 4551 5545 4e43 4556 4552 4946  ECKSEQUENCEVERIF
 000004b0: 5929 07da 0a73 6967 5f70 7562 6b65 79da  Y)...sig_pubkey.
 000004c0: 0d70 3273 685f 6d75 6c74 6973 6967 da0b  .p2sh_multisig..
 000004d0: 7032 7368 5f70 3277 706b 68da 0a70 3273  p2sh_p2wpkh..p2s
-000004e0: 685f 7032 7773 6872 1200 0000 7213 0000  h_p2wshr....r...
-000004f0: 0072 1000 0000 e902 0000 00e9 5000 0000  .r..........P...
+000004e0: 685f 7032 7773 6872 1100 0000 7212 0000  h_p2wshr....r...
+000004f0: 0072 0f00 0000 e902 0000 00e9 5000 0000  .r..........P...
 00000500: 6c03 0000 0000 0000 0002 0069 0000 4000  l..........i..@.
 00000510: e909 0000 0069 ffff 0000 6c03 0000 00fe  .....i....l.....
 00000520: 7fff 7f03 006c 0300 0000 fd7f ff7f 0300  .....l..........
-00000530: da07 656e 676c 6973 685a 0762 6974 636f  ..englishZ.bitco
+00000530: 5a07 656e 676c 6973 685a 0762 6974 636f  Z.englishZ.bitco
 00000540: 696e 7505 0000 00c2 b573 6174 5a04 6d73  inu......satZ.ms
-00000550: 6174 da01 6eda 0373 6174 5a03 6669 6ef5  at..n..satZ.fin.
-00000560: 0200 0000 c2b5 da01 6dda 0163 da01 64da  ........m..c..d.
+00000550: 6174 da01 6e5a 0373 6174 5a03 6669 6ef5  at..nZ.satZ.fin.
+00000560: 0200 0000 c2b5 da01 6dda 0163 da01 645a  ........m..c..dZ
 00000570: 0264 61da 0168 da01 6bda 014d da01 47da  .da..h..k..M..G.
 00000580: 0154 da01 50da 0145 da01 5ada 0159 2914  .T..P..E..Z..Y).
 00000590: 679b 2ba1 869b 8406 3d67 9564 79e1 7ffd  g.+.....=g.dy...
 000005a0: a53d 6795 d626 e80b 2e11 3e67 3a8c 30e2  .=g..&....>g:.0.
 000005b0: 8e79 453e 6748 afbc 9af2 d77a 3e67 8ded  .yE>gH.....z>g..
 000005c0: b5a0 f7c6 b03e 67fc a9f1 d24d 6250 3f67  .....>g....MbP?g
 000005d0: 7b14 ae47 e17a 843f 679a 9999 9999 99b9  {..G.z.?g.......
@@ -97,40 +97,40 @@
 00000600: 0300 0000 0010 4a29 a303 6c04 0000 0000  ......J)..l.....
 00000610: 008d 49fa 351c 006c 0400 0000 0000 c84e  ..I.5..l.......N
 00000620: ce5a 056f 6c05 0000 0000 0040 3d17 374d  .Z.ol......@=.7M
 00000630: 2e63 036c 0600 0000 0000 0042 b633 765e  .c.l.......B.3v^
 00000640: 213c 1a00 da02 6e74 7a05 5554 462d 3863  !<....ntz.UTF-8c
 00000650: 0000 0000 0000 0000 0000 0000 0100 0000  ................
 00000660: 0200 0000 4700 0000 7308 0000 0064 0164  ....G...s....d.d
-00000670: 0267 0253 0029 034e da05 656e 5f55 53da  .g.S.).N..en_US.
+00000670: 0267 0253 0029 034e 5a05 656e 5f55 53da  .g.S.).NZ.en_US.
 00000680: 0475 7466 38a9 0029 01da 0461 7267 7372  .utf8..)...argsr
-00000690: 3100 0000 7231 0000 00fa 392f 686f 6d65  1...r1....9/home
+00000690: 2c00 0000 722c 0000 00fa 392f 686f 6d65  ,...r,....9/home
 000006a0: 2f6c 656e 6e61 7274 2f63 6f64 652f 6269  /lennart/code/bi
 000006b0: 7463 6f69 6e6c 6962 2f62 6974 636f 696e  tcoinlib/bitcoin
 000006c0: 6c69 622f 636f 6e66 6967 2f63 6f6e 6669  lib/config/confi
 000006d0: 672e 7079 da08 3c6c 616d 6264 613e 7c00  g.py..<lambda>|.
-000006e0: 0000 f300 0000 0072 3400 0000 7a60 4c6f  .......r4...z`Lo
+000006e0: 0000 f300 0000 0072 2f00 0000 7a60 4c6f  .......r/...z`Lo
 000006f0: 6361 6c65 2069 7320 6375 7272 656e 746c  cale is currentl
 00000700: 7920 7365 7420 746f 2027 2573 272e 2054  y set to '%s'. T
 00000710: 6869 7320 6c69 6272 6172 7920 6e65 6564  his library need
 00000720: 7320 7468 6520 6c6f 6361 6c65 2073 6574  s the locale set
 00000730: 2074 6f20 5554 462d 3820 746f 2066 756e   to UTF-8 to fun
 00000740: 6374 696f 6e20 7072 6f70 6572 6c79 da06  ction properly..
 00000750: 6261 7365 3538 da06 6265 6368 3332 da02  base58..bech32..
 00000760: 6263 da02 7462 5a03 6c74 635a 0474 6c74  bc..tbZ.ltcZ.tlt
 00000770: 635a 0574 6461 7368 5a03 626c 74da 066c  cZ.tdashZ.blt..l
 00000780: 6567 6163 7969 a330 c82b 720b 0000 0046  egacyi.0.+r....F
 00000790: 7a42 5369 6e67 6c65 206b 6579 2077 616c  zBSingle key wal
 000007a0: 6c65 7420 7769 7468 206e 6f20 6869 6572  let with no hier
 000007b0: 6172 6368 6963 616c 2064 6574 6572 6d69  archical determi
 000007c0: 6e69 7374 6963 206b 6579 2073 7472 7563  nistic key struc
-000007d0: 7475 7265 2907 da07 7075 7270 6f73 65da  ture)...purpose.
+000007d0: 7475 7265 2907 5a07 7075 7270 6f73 65da  ture).Z.purpose.
 000007e0: 0b73 6372 6970 745f 7479 7065 da0c 7769  .script_type..wi
 000007f0: 746e 6573 735f 7479 7065 720a 0000 00da  tness_typer.....
-00000800: 0865 6e63 6f64 696e 67da 0b64 6573 6372  .encoding..descr
+00000800: 0865 6e63 6f64 696e 675a 0b64 6573 6372  .encodingZ.descr
 00000810: 6970 7469 6f6e 5a08 6b65 795f 7061 7468  iptionZ.key_path
 00000820: e92c 0000 007a 324c 6567 6163 7920 7761  .,...z2Legacy wa
 00000830: 6c6c 6574 2075 7369 6e67 2070 6179 2d74  llet using pay-t
 00000840: 6f2d 7075 626c 6963 2d6b 6579 2d68 6173  o-public-key-has
 00000850: 6820 7363 7269 7074 737a 0870 7572 706f  h scriptsz.purpo
 00000860: 7365 277a 0a63 6f69 6e5f 7479 7065 277a  se'z.coin_type'z
 00000870: 0861 6363 6f75 6e74 275a 0663 6861 6e67  .account'Z.chang
@@ -208,45 +208,45 @@
 00000cf0: 0000 007a 2c7c 0372 1888 006a 007c 007c  ...z,|.r...j.|.|
 00000d00: 017c 0264 018d 037d 046e 1088 006a 017c  .|.d...}.n...j.|
 00000d10: 007c 017c 0264 018d 037d 047c 0457 0053  .|.|.d...}.|.W.S
 00000d20: 0004 0074 026b 0a72 4401 0001 0001 007c  ...t.k.rD......|
 00000d30: 0206 0059 0053 0058 0064 0053 0029 024e  ...Y.S.X.d.S.).N
 00000d40: a901 da08 6661 6c6c 6261 636b 2903 5a0a  ....fallback).Z.
 00000d50: 6765 7462 6f6f 6c65 616e da03 6765 74da  getboolean..get.
-00000d60: 0945 7863 6570 7469 6f6e 2905 da07 7365  .Exception)...se
-00000d70: 6374 696f 6eda 0376 6172 7247 0000 00da  ction..varrG....
+00000d60: 0945 7863 6570 7469 6f6e 2905 5a07 7365  .Exception).Z.se
+00000d70: 6374 696f 6eda 0376 6172 7240 0000 00da  ction..varr@....
 00000d80: 0a69 735f 626f 6f6c 6561 6eda 0376 616c  .is_boolean..val
-00000d90: a901 da06 636f 6e66 6967 7231 0000 0072  ....configr1...r
-00000da0: 3300 0000 da0a 636f 6e66 6967 5f67 6574  3.....config_get
+00000d90: a901 da06 636f 6e66 6967 722c 0000 0072  ....configr,...r
+00000da0: 2e00 0000 da0a 636f 6e66 6967 5f67 6574  ......config_get
 00000db0: de00 0000 730e 0000 0000 0102 0104 0112  ....s...........
 00000dc0: 0210 0106 010e 017a 1f72 6561 645f 636f  .......z.read_co
 00000dd0: 6e66 6967 2e3c 6c6f 6361 6c73 3e2e 636f  nfig.<locals>.co
 00000de0: 6e66 6967 5f67 6574 da0f 4243 4c5f 434f  nfig_get..BCL_CO
 00000df0: 4e46 4947 5f46 494c 457a 187e 2f2e 6269  NFIG_FILEz.~/.bi
 00000e00: 7463 6f69 6e6c 6962 2f63 6f6e 6669 672e  tcoinlib/config.
 00000e10: 696e 697a 0b2e 6269 7463 6f69 6e6c 6962  iniz..bitcoinlib
 00000e20: da04 6461 7461 7a2b 4269 7463 6f69 6e6c  ..dataz+Bitcoinl
 00000e30: 6962 2063 6f6e 6669 6775 7261 7469 6f6e  ib configuration
 00000e40: 2066 696c 6520 6e6f 7420 666f 756e 643a   file not found:
-00000e50: 2025 73da 096c 6f63 6174 696f 6e73 5a08   %s..locationsZ.
+00000e50: 2025 735a 096c 6f63 6174 696f 6e73 5a08   %sZ.locationsZ.
 00000e60: 6461 7461 5f64 6972 7a0d 7e2f 2e62 6974  data_dirz.~/.bit
-00000e70: 636f 696e 6c69 6272 4600 0000 5a0c 6461  coinlibrF...Z.da
+00000e70: 636f 696e 6c69 6272 3f00 0000 5a0c 6461  coinlibr?...Z.da
 00000e80: 7461 6261 7365 5f64 6972 5a08 6461 7461  tabase_dirZ.data
 00000e90: 6261 7365 5429 02da 0770 6172 656e 7473  baseT)...parents
 00000ea0: da08 6578 6973 745f 6f6b da14 6465 6661  ..exist_ok..defa
 00000eb0: 756c 745f 6461 7461 6261 7365 6669 6c65  ult_databasefile
 00000ec0: 7a11 6269 7463 6f69 6e6c 6962 2e73 716c  z.bitcoinlib.sql
 00000ed0: 6974 655a 0a70 6f73 7467 7265 7371 6c5a  iteZ.postgresqlZ
 00000ee0: 056d 7973 716c da1a 6465 6661 756c 745f  .mysql..default_
 00000ef0: 6461 7461 6261 7365 6669 6c65 5f63 6163  databasefile_cac
 00000f00: 6865 7a17 6269 7463 6f69 6e6c 6962 5f63  hez.bitcoinlib_c
 00000f10: 6163 6865 2e73 716c 6974 65da 0663 6f6d  ache.sqlite..com
 00000f20: 6d6f 6e5a 1661 6c6c 6f77 5f64 6174 6162  monZ.allow_datab
-00000f30: 6173 655f 7468 7265 6164 7329 0272 4700  ase_threads).rG.
-00000f40: 0000 724c 0000 005a 1773 6572 7669 6365  ..rL...Z.service
+00000f30: 6173 655f 7468 7265 6164 7329 0272 4000  ase_threads).r@.
+00000f40: 0000 7244 0000 005a 1773 6572 7669 6365  ..rD...Z.service
 00000f50: 5f63 6163 6869 6e67 5f65 6e61 626c 6564  _caching_enabled
 00000f60: 5a04 6c6f 6773 5a19 656e 6162 6c65 5f62  Z.logsZ.enable_b
 00000f70: 6974 636f 696e 6c69 625f 6c6f 6767 696e  itcoinlib_loggin
 00000f80: 675a 086c 6f67 5f66 696c 657a 0e62 6974  gZ.log_filez.bit
 00000f90: 636f 696e 6c69 622e 6c6f 675a 086c 6f67  coinlib.logZ.log
 00000fa0: 6c65 7665 6c5a 1074 696d 656f 7574 5f72  levelZ.timeout_r
 00000fb0: 6571 7565 7374 735a 1273 6572 7669 6365  equestsZ.service
@@ -259,16 +259,16 @@
 00001020: 745f 7769 746e 6573 735f 7479 7065 da1c  t_witness_type..
 00001030: 554e 4954 5445 5354 535f 4655 4c4c 5f44  UNITTESTS_FULL_D
 00001040: 4154 4142 4153 455f 5445 5354 2905 7206  ATABASE_TEST).r.
 00001050: 0000 0054 da04 5472 7565 da04 7472 7565  ...T..True..true
 00001060: da04 5452 5545 2901 4629 24da 0c63 6f6e  ..TRUE).F)$..con
 00001070: 6669 6770 6172 7365 72da 0c43 6f6e 6669  figparser..Confi
 00001080: 6750 6172 7365 72da 026f 73da 0765 6e76  gParser..os..env
-00001090: 6972 6f6e 7248 0000 0072 0200 0000 da0a  ironrH...r......
-000010a0: 6578 7061 6e64 7573 6572 7251 0000 00da  expanduserrQ....
+00001090: 6972 6f6e 7241 0000 0072 0200 0000 da0a  ironrA...r......
+000010a0: 6578 7061 6e64 7573 6572 7249 0000 005a  expanduserrI...Z
 000010b0: 0b69 735f 6162 736f 6c75 7465 da04 686f  .is_absolute..ho
 000010c0: 6d65 da06 6578 6973 7473 da0f 4243 4c5f  me..exists..BCL_
 000010d0: 494e 5354 414c 4c5f 4449 52da 0749 4f45  INSTALL_DIR..IOE
 000010e0: 7272 6f72 da03 7374 72da 0472 6561 64da  rror..str..read.
 000010f0: 0c42 434c 5f44 4154 415f 4449 52da 1042  .BCL_DATA_DIR..B
 00001100: 434c 5f44 4154 4142 4153 455f 4449 52da  CL_DATABASE_DIR.
 00001110: 056d 6b64 6972 da10 4445 4641 554c 545f  .mkdir..DEFAULT_
@@ -286,26 +286,26 @@
 000011d0: 1253 4552 5649 4345 5f4d 4158 5f45 5252  .SERVICE_MAX_ERR
 000011e0: 4f52 53da 104d 4158 5f54 5241 4e53 4143  ORS..MAX_TRANSAC
 000011f0: 5449 4f4e 53da 1642 4c4f 434b 5f43 4f55  TIONS..BLOCK_COU
 00001200: 4e54 5f43 4143 4845 5f54 494d 45da 1044  NT_CACHE_TIME..D
 00001210: 4546 4155 4c54 5f4c 414e 4755 4147 45da  EFAULT_LANGUAGE.
 00001220: 0f44 4546 4155 4c54 5f4e 4554 574f 524b  .DEFAULT_NETWORK
 00001230: da14 4445 4641 554c 545f 5749 544e 4553  ..DEFAULT_WITNES
-00001240: 535f 5459 5045 7259 0000 0029 0672 5000  S_TYPErY...).rP.
+00001240: 535f 5459 5045 7250 0000 0029 0672 4800  S_TYPErP...).rH.
 00001250: 0000 5a10 636f 6e66 6967 5f66 696c 655f  ..Z.config_file_
-00001260: 6e61 6d65 7252 0000 0072 5600 0000 7257  namerR...rV...rW
+00001260: 6e61 6d65 724a 0000 0072 4d00 0000 724e  namerJ...rM...rN
 00001270: 0000 005a 0c66 756c 6c5f 6462 5f74 6573  ...Z.full_db_tes
-00001280: 7472 3100 0000 724e 0000 0072 3300 0000  tr1...rN...r3...
+00001280: 7472 2c00 0000 7246 0000 0072 2e00 0000  tr,...rF...r....
 00001290: da0b 7265 6164 5f63 6f6e 6669 67db 0000  ..read_config...
 000012a0: 0073 5800 0000 0001 0802 0e12 0c01 0401  .sX.............
 000012b0: 0e02 0801 0801 1001 0801 0c01 0801 1001  ................
 000012c0: 0e01 1603 1201 0e02 0cff 0602 1401 0e02  ................
 000012d0: 0cff 0602 1801 0e01 1001 1003 1001 1401  ................
 000012e0: 1001 0e03 1201 1201 1201 1203 0e01 0e01  ................
-000012f0: 0e02 0c01 0601 0a01 0402 0601 0401 727d  ..............r}
+000012f0: 0e02 0c01 0601 0a01 0402 0601 0401 7273  ..............rs
 00001300: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00001310: 0500 0000 0a00 0000 4300 0000 73ae 0000  ........C...s...
 00001320: 0074 0074 0164 0183 027d 007c 00a0 02a1  .t.t.d...}.|....
 00001330: 0072 1664 0053 007c 00a0 0364 02a1 018f  .r.d.S.|...d....
 00001340: 427d 0164 0374 0474 05a0 06a1 00a0 07a1  B}.d.t.t........
 00001350: 0074 08a0 09a1 0074 08a0 0aa1 0074 08a0  .t.....t.....t..
 00001360: 0ba1 0074 08a0 0ca1 0074 08a0 08a1 0066  ...t.....t.....f
@@ -341,50 +341,50 @@
 00001540: 2020 2020 203a 2025 730a 436f 6d70 696c       : %s.Compil
 00001550: 6572 2020 2020 2020 2020 2020 3a20 2573  er          : %s
 00001560: 0a42 7569 6c64 2020 2020 2020 2020 2020  .Build          
 00001570: 2020 203a 2025 730a 4f53 2056 6572 7369     : %s.OS Versi
 00001580: 6f6e 2020 2020 2020 2020 3a20 2573 0a50  on        : %s.P
 00001590: 6c61 7466 6f72 6d20 2020 2020 2020 2020  latform         
 000015a0: 203a 2025 730a 7201 0000 0029 01da 0863   : %s.r....)...c
-000015b0: 6f70 7966 696c 6572 5200 0000 2902 7a04  opyfilerR...).z.
+000015b0: 6f70 7966 696c 6572 4a00 0000 2902 7a04  opyfilerJ...).z.
 000015c0: 2e69 6e69 7a05 2e6a 736f 6e29 1572 0200  .iniz..json).r..
-000015d0: 0000 7269 0000 0072 6400 0000 da04 6f70  ..ri...rd.....op
+000015d0: 0000 725f 0000 0072 5a00 0000 da04 6f70  ..r_...rZ.....op
 000015e0: 656e da12 4249 5443 4f49 4e4c 4942 5f56  en..BITCOINLIB_V
 000015f0: 4552 5349 4f4e 7203 0000 00da 036e 6f77  ERSIONr......now
-00001600: da09 6973 6f66 6f72 6d61 74da 0870 6c61  ..isoformat..pla
-00001610: 7466 6f72 6dda 0e70 7974 686f 6e5f 7665  tform..python_ve
-00001620: 7273 696f 6eda 0f70 7974 686f 6e5f 636f  rsion..python_co
-00001630: 6d70 696c 6572 da0c 7079 7468 6f6e 5f62  mpiler..python_b
+00001600: 5a09 6973 6f66 6f72 6d61 74da 0870 6c61  Z.isoformat..pla
+00001610: 7466 6f72 6d5a 0e70 7974 686f 6e5f 7665  tformZ.python_ve
+00001620: 7273 696f 6e5a 0f70 7974 686f 6e5f 636f  rsionZ.python_co
+00001630: 6d70 696c 6572 5a0c 7079 7468 6f6e 5f62  mpilerZ.python_b
 00001640: 7569 6c64 da07 7665 7273 696f 6eda 0577  uild..version..w
-00001650: 7269 7465 da06 7368 7574 696c 727f 0000  rite..shutilr...
-00001660: 0072 6500 0000 da07 6974 6572 6469 72da  .re.....iterdir.
-00001670: 0673 7566 6669 7872 6700 0000 da04 6e61  .suffixrg.....na
+00001650: 7269 7465 5a06 7368 7574 696c 7275 0000  riteZ.shutilru..
+00001660: 0072 5b00 0000 5a07 6974 6572 6469 72da  .r[...Z.iterdir.
+00001670: 0673 7566 6669 7872 5d00 0000 da04 6e61  .suffixr].....na
 00001680: 6d65 2905 5a0b 696e 7374 6c6f 6766 696c  me).Z.instlogfil
 00001690: 65da 0166 5a0f 696e 7374 616c 6c5f 6d65  e..fZ.install_me
-000016a0: 7373 6167 6572 7f00 0000 da04 6669 6c65  ssager......file
-000016b0: 7231 0000 0072 3100 0000 7233 0000 00da  r1...r1...r3....
+000016a0: 7373 6167 6572 7500 0000 da04 6669 6c65  ssageru.....file
+000016b0: 722c 0000 0072 2c00 0000 722e 0000 00da  r,...r,...r.....
 000016c0: 0e69 6e69 7469 616c 697a 655f 6c69 6228  .initialize_lib(
 000016d0: 0100 0073 2400 0000 0002 0a01 0801 0402  ...s$...........
 000016e0: 0c01 020b 1201 0600 0600 0600 06ff 02f5  ................
-000016f0: 040d 1403 0c01 1201 0a01 0201 7290 0000  ............r...
+000016f0: 040d 1403 0c01 1201 0a01 0201 7280 0000  ............r...
 00001700: 007a 0e63 6f6e 6669 672f 5645 5253 494f  .z.config/VERSIO
-00001710: 4e29 3f72 5f00 0000 da06 6c6f 6361 6c65  N)?r_.....locale
-00001720: 7284 0000 0072 5d00 0000 da04 656e 756d  r....r].....enum
+00001710: 4e29 3f72 5600 0000 5a06 6c6f 6361 6c65  N)?rV...Z.locale
+00001720: 7279 0000 0072 5400 0000 da04 656e 756d  ry...rT.....enum
 00001730: da07 7061 7468 6c69 6272 0200 0000 7203  ..pathlibr....r.
-00001740: 0000 0072 6700 0000 da09 5459 5045 5f54  ...rg.....TYPE_T
-00001750: 4558 5472 7500 0000 5a08 5459 5045 5f49  EXTru...Z.TYPE_I
-00001760: 4e54 7274 0000 0072 5100 0000 da08 5f5f  NTrt...rQ.....__
-00001770: 6669 6c65 5f5f 7254 0000 0072 6500 0000  file__rT...re...
-00001780: 7269 0000 0072 6a00 0000 726c 0000 0072  ri...rj...rl...r
-00001790: 6e00 0000 7272 0000 0072 7100 0000 726f  n...rr...rq...ro
-000017a0: 0000 0072 7600 0000 7278 0000 0072 7900  ...rv...rx...ry.
-000017b0: 0000 7277 0000 005a 1453 4352 4950 545f  ..rw...Z.SCRIPT_
+00001740: 0000 0072 5d00 0000 da09 5459 5045 5f54  ...r].....TYPE_T
+00001750: 4558 5472 6b00 0000 5a08 5459 5045 5f49  EXTrk...Z.TYPE_I
+00001760: 4e54 726a 0000 0072 4900 0000 da08 5f5f  NTrj...rI.....__
+00001770: 6669 6c65 5f5f 724b 0000 0072 5b00 0000  file__rK...r[...
+00001780: 725f 0000 0072 6000 0000 7262 0000 0072  r_...r`...rb...r
+00001790: 6400 0000 7268 0000 0072 6700 0000 7265  d...rh...rg...re
+000017a0: 0000 0072 6c00 0000 726e 0000 0072 6f00  ...rl...rn...ro.
+000017b0: 0000 726d 0000 005a 1453 4352 4950 545f  ..rm...Z.SCRIPT_
 000017c0: 5459 5045 535f 4c4f 434b 494e 475a 1653  TYPES_LOCKINGZ.S
 000017d0: 4352 4950 545f 5459 5045 535f 554e 4c4f  CRIPT_TYPES_UNLO
-000017e0: 434b 494e 4772 1100 0000 5a0c 5349 4748  CKINGr....Z.SIGH
+000017e0: 434b 494e 4772 1000 0000 5a0c 5349 4748  CKINGr....Z.SIGH
 000017f0: 4153 485f 4e4f 4e45 5a0e 5349 4748 4153  ASH_NONEZ.SIGHAS
 00001800: 485f 5349 4e47 4c45 5a14 5349 4748 4153  H_SINGLEZ.SIGHAS
 00001810: 485f 414e 594f 4e45 4341 4e50 4159 5a1e  H_ANYONECANPAYZ.
 00001820: 5345 5155 454e 4345 5f4c 4f43 4b54 494d  SEQUENCE_LOCKTIM
 00001830: 455f 4449 5341 424c 455f 464c 4147 5a1b  E_DISABLE_FLAGZ.
 00001840: 5345 5155 454e 4345 5f4c 4f43 4b54 494d  SEQUENCE_LOCKTIM
 00001850: 455f 5459 5045 5f46 4c41 475a 1d53 4551  E_TYPE_FLAGZ.SEQ
@@ -393,32 +393,32 @@
 00001880: 454e 4345 5f4c 4f43 4b54 494d 455f 4d41  ENCE_LOCKTIME_MA
 00001890: 534b 5a18 5345 5155 454e 4345 5f45 4e41  SKZ.SEQUENCE_ENA
 000018a0: 424c 455f 4c4f 434b 5449 4d45 5a17 5345  BLE_LOCKTIMEZ.SE
 000018b0: 5155 454e 4345 5f52 4550 4c41 4345 5f42  QUENCE_REPLACE_B
 000018c0: 595f 4645 455a 1a53 4947 4e41 5455 5245  Y_FEEZ.SIGNATURE
 000018d0: 5f56 4552 5349 4f4e 5f53 5441 4e44 4152  _VERSION_STANDAR
 000018e0: 445a 1853 4947 4e41 5455 5245 5f56 4552  DZ.SIGNATURE_VER
-000018f0: 5349 4f4e 5f53 4547 5749 5472 7a00 0000  SION_SEGWITrz...
-00001900: 727b 0000 005a 144e 4554 574f 524b 5f44  r{...Z.NETWORK_D
-00001910: 454e 4f4d 494e 4154 4f52 5372 8d00 0000  ENOMINATORSr....
+000018f0: 5349 4f4e 5f53 4547 5749 5472 7000 0000  SION_SEGWITrp...
+00001900: 7271 0000 005a 144e 4554 574f 524b 5f44  rq...Z.NETWORK_D
+00001910: 454e 4f4d 494e 4154 4f52 5372 7d00 0000  ENOMINATORSr}...
 00001920: da14 6765 7470 7265 6665 7272 6564 656e  ..getpreferreden
-00001930: 636f 6469 6e67 da07 5f6c 6f63 616c 65da  coding.._locale.
+00001930: 636f 6469 6e67 da07 5f6c 6f63 616c 655a  coding.._localeZ
 00001940: 115f 6765 7464 6566 6175 6c74 6c6f 6361  ._getdefaultloca
 00001950: 6c65 da10 456e 7669 726f 6e6d 656e 7445  le..EnvironmentE
 00001960: 7272 6f72 5a1b 5355 5050 4f52 5445 445f  rrorZ.SUPPORTED_
 00001970: 4144 4452 4553 535f 454e 434f 4449 4e47  ADDRESS_ENCODING
 00001980: 535a 1845 4e43 4f44 494e 475f 4245 4348  SZ.ENCODING_BECH
-00001990: 3332 5f50 5245 4649 5845 5372 7c00 0000  32_PREFIXESr|...
+00001990: 3332 5f50 5245 4649 5845 5372 7200 0000  32_PREFIXESrr...
 000019a0: da0d 4245 4348 3332 4d5f 434f 4e53 545a  ..BECH32M_CONSTZ
 000019b0: 1557 414c 4c45 545f 4b45 595f 5354 5255  .WALLET_KEY_STRU
-000019c0: 4354 5552 4553 7259 0000 0072 7000 0000  CTURESrY...rp...
-000019d0: 727d 0000 0072 9000 0000 7280 0000 0072  r}...r....r....r
-000019e0: 6800 0000 da05 7374 7269 7072 8100 0000  h.....stripr....
-000019f0: 7231 0000 0072 3100 0000 7231 0000 0072  r1...r1...r1...r
-00001a00: 3300 0000 da08 3c6d 6f64 756c 653e 1500  3.....<module>..
+000019c0: 4354 5552 4553 7250 0000 0072 6600 0000  CTURESrP...rf...
+000019d0: 7273 0000 0072 8000 0000 7276 0000 0072  rs...r....rv...r
+000019e0: 5e00 0000 da05 7374 7269 7072 7700 0000  ^.....striprw...
+000019f0: 722c 0000 0072 2c00 0000 722c 0000 0072  r,...r,...r,...r
+00001a00: 2e00 0000 da08 3c6d 6f64 756c 653e 1500  ......<module>..
 00001a10: 0000 732a 0100 0008 0108 0108 0108 0108  ..s*............
 00001a20: 010c 010c 0304 0104 0104 0404 010e 0104  ................
 00001a30: 0104 0104 0104 0104 0304 0104 0304 0104  ................
 00001a40: 0104 0104 050c 0108 0106 0106 0106 010a  ................
 00001a50: 0106 0106 f706 0e08 0108 010a 0108 0108  ................
 00001a60: 0108 0104 f806 0b04 0104 0104 0104 0204  ................
 00001a70: 0104 0104 0104 0104 0104 0204 0104 0304  ................
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/__pycache__/opcodes.cpython-38.pyc` & `bitcoinlib-0.6.9/bitcoinlib/config/__pycache__/opcodes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/config.py` & `bitcoinlib-0.6.9/bitcoinlib/config/config.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/opcodes.py` & `bitcoinlib-0.6.9/bitcoinlib/config/opcodes.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/config/secp256k1.py` & `bitcoinlib-0.6.9/bitcoinlib/config/secp256k1.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/config.ini` & `bitcoinlib-0.6.9/bitcoinlib/data/config.ini`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/config.ini.unittest` & `bitcoinlib-0.6.9/bitcoinlib/data/config.ini.unittest`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/networks.json` & `bitcoinlib-0.6.9/bitcoinlib/data/networks.json`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/providers.examples.json` & `bitcoinlib-0.6.9/bitcoinlib/data/providers.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3725198412698413%*

 * *Differences: {"'blockbook'": "OrderedDict([('provider', 'blockbook'), ('network', 'bitcoin'), ('client_class', "*

 * *                "'BlockbookClient'), ('provider_coin_id', ''), ('url', "*

 * *                "'https://bitcoinblockexplorers.com/api/v2/'), ('api_key', ''), ('priority', 10), "*

 * *                "('denominator', 100000000), ('network_overrides', None)])",*

 * * "'blockbook.dash'": "OrderedDict([('provider', 'blockbook'), ('network', 'dash'), "*

 * *                     "('client_class', 'BlockbookClient'), ('provider_coin_id […]*

```diff
@@ -1,30 +1,8 @@
 {
-    "bcoin": {
-        "api_key": "",
-        "client_class": "BcoinClient",
-        "denominator": 100000000,
-        "network": "bitcoin",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "bcoin",
-        "provider_coin_id": "",
-        "url": ""
-    },
-    "bcoin.testnet": {
-        "api_key": "",
-        "client_class": "BcoinClient",
-        "denominator": 100000000,
-        "network": "testnet",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "bcoin",
-        "provider_coin_id": "",
-        "url": ""
-    },
     "bitaps": {
         "api_key": "",
         "client_class": "BitapsClient",
         "denominator": 100000000,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
@@ -72,36 +50,14 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "bitaps",
         "provider_coin_id": "",
         "url": "https://api.bitaps.com/btc/testnet/v1/"
     },
-    "bitcoind": {
-        "api_key": "",
-        "client_class": "BitcoindClient",
-        "denominator": 100000000,
-        "network": "bitcoin",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "bitcoind",
-        "provider_coin_id": "",
-        "url": "http://rpcuser:mypasswod@localhost:8332"
-    },
-    "bitcoind.testnet": {
-        "api_key": "",
-        "client_class": "BitcoindClient",
-        "denominator": 100000000,
-        "network": "testnet",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "bitcoind",
-        "provider_coin_id": "",
-        "url": "http://rpcuser:mypasswod@localhost:18332"
-    },
     "bitcoinlib_test": {
         "api_key": "",
         "client_class": "BitcoinLibTestClient",
         "denominator": 100000000,
         "network": "bitcoinlib_test",
         "network_overrides": null,
         "priority": 10,
@@ -127,14 +83,80 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "bitgo",
         "provider_coin_id": "",
         "url": "https://test.bitgo.com/api/v1/"
     },
+    "blockbook": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://bitcoinblockexplorers.com/api/v2/"
+    },
+    "blockbook.dash": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "dash",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://dashblockexplorer.com/api/v2/"
+    },
+    "blockbook.dogecoin": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "dogecoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://dogeblocks.com/api/v2/"
+    },
+    "blockbook.litecoin": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "litecoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://litecoinblockexplorer.net/api/v2/"
+    },
+    "blockbook.litecoin.legacy": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "litecoin_legacy",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://litecoinblockexplorer.net/api/v2/"
+    },
+    "blockbook.testnet2": {
+        "api_key": "",
+        "client_class": "BlockbookClient",
+        "denominator": 100000000,
+        "network": "testnet",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockbook",
+        "provider_coin_id": "",
+        "url": "https://tbtc1.blockbook.bitaccess.net/api/v2/"
+    },
     "blockchaininfo": {
         "api_key": "",
         "client_class": "BlockchainInfoClient",
         "denominator": 1,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
@@ -149,24 +171,57 @@
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockchair",
         "provider_coin_id": "",
         "url": "https://api.blockchair.com/bitcoin/"
     },
-    "blockcypher": {
+    "blockchair.dash": {
         "api_key": "",
-        "client_class": "BlockCypher",
-        "denominator": 1,
-        "network": "bitcoin",
+        "client_class": "BlockChairClient",
+        "denominator": 100000000,
+        "network": "dash",
         "network_overrides": null,
         "priority": 10,
-        "provider": "blockcypher",
+        "provider": "blockchair",
+        "provider_coin_id": "",
+        "url": "https://api.blockchair.com/dash/"
+    },
+    "blockchair.dogecoin": {
+        "api_key": "",
+        "client_class": "BlockChairClient",
+        "denominator": 100000000,
+        "network": "dogecoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockchair",
+        "provider_coin_id": "",
+        "url": "https://api.blockchair.com/dogecoin/"
+    },
+    "blockchair.litecoin": {
+        "api_key": "",
+        "client_class": "BlockChairClient",
+        "denominator": 100000000,
+        "network": "litecoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockchair",
+        "provider_coin_id": "",
+        "url": "https://api.blockchair.com/litecoin/"
+    },
+    "blockchair.testnet": {
+        "api_key": "",
+        "client_class": "BlockChairClient",
+        "denominator": 100000000,
+        "network": "testnet",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockchair",
         "provider_coin_id": "",
-        "url": "https://api.blockcypher.com/v1/btc/main/"
+        "url": "https://api.blockchair.com/bitcoin/testnet/"
     },
     "blockcypher.dogecoin": {
         "api_key": "",
         "client_class": "BlockCypher",
         "denominator": 1,
         "network": "dogecoin",
         "network_overrides": null,
@@ -195,24 +250,35 @@
         "network": "litecoin_legacy",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockcypher",
         "provider_coin_id": "",
         "url": "https://api.blockcypher.com/v1/ltc/main/"
     },
-    "blockcypher.testnet": {
+    "blocksmurfer": {
         "api_key": "",
-        "client_class": "BlockCypher",
-        "denominator": 1,
+        "client_class": "BlocksmurferClient",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blocksmurfer",
+        "provider_coin_id": "",
+        "url": "https://harari.blocksmurfer.io/api/v1/btc/"
+    },
+    "blocksmurfer.testnet": {
+        "api_key": "",
+        "client_class": "BlocksmurferClient",
+        "denominator": 100000000,
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
-        "provider": "blockcypher",
+        "provider": "blocksmurfer",
         "provider_coin_id": "",
-        "url": "https://api.blockcypher.com/v1/btc/test3/"
+        "url": "https://harari.blocksmurfer.io/api/v1/tbtc/"
     },
     "blockstream": {
         "api_key": "",
         "client_class": "BlockstreamClient",
         "denominator": 100000000,
         "network": "bitcoin",
         "network_overrides": null,
@@ -229,198 +295,141 @@
         "network_overrides": null,
         "priority": 10,
         "provider": "blockstream",
         "provider_coin_id": "",
         "url": "https://blockstream.info/testnet/api/"
     },
     "cryptoid.dash": {
-        "api_key": "",
+        "api_key": "api-key-needed",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "dash",
         "url": "https://chainz.cryptoid.info/"
     },
     "cryptoid.litecoin": {
-        "api_key": "",
+        "api_key": "api-key-needed",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "ltc",
         "url": "https://chainz.cryptoid.info/"
     },
     "cryptoid.litecoin.legacy": {
-        "api_key": "",
+        "api_key": "api-key-needed",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "litecoin_legacy",
         "network_overrides": {
             "prefix_address_p2sh": "32"
         },
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "ltc",
         "url": "https://chainz.cryptoid.info/"
     },
-    "dashd": {
-        "api_key": "",
-        "client_class": "DashdClient",
-        "denominator": 100000000,
-        "network": "dash",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "dashd",
-        "provider_coin_id": "",
-        "url": ""
-    },
-    "dashd.testnet": {
-        "api_key": "",
-        "client_class": "DashdClient",
-        "denominator": 100000000,
-        "network": "dash_testnet",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "dashd",
-        "provider_coin_id": "",
-        "url": ""
-    },
-    "dogecoin": {
-        "api_key": "",
-        "client_class": "DogecoindClient",
-        "denominator": 100000000,
-        "network": "dogecoin",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "dogecoind",
-        "provider_coin_id": "",
-        "url": ""
-    },
-    "dogecoind.testnet": {
-        "api_key": "",
-        "client_class": "DogecoindClient",
-        "denominator": 100000000,
-        "network": "dogecoin_testnet",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "dogecoind",
-        "provider_coin_id": "",
-        "url": ""
-    },
     "insightdash": {
         "api_key": "",
         "client_class": "InsightDashClient",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
         "provider": "insightdash",
         "provider_coin_id": "",
         "url": "https://insight.dash.org/api/"
     },
-    "litecoinblockexplorer.litecoin": {
+    "litecoinblockexplorer": {
         "api_key": "",
         "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
-        "network": "litecoin",
+        "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://litecoinblockexplorer.net/api/"
+        "url": "https://bitcoinblockexplorers.com/api/v1/"
     },
-    "litecoinblockexplorer.litecoin.legacy": {
+    "litecoinblockexplorer.dash": {
         "api_key": "",
         "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
-        "network": "litecoin_legacy",
+        "network": "dash",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://litecoinblockexplorer.net/api/"
+        "url": "https://dashblockexplorer.com/api/v1/"
     },
-    "litecoind": {
+    "litecoinblockexplorer.dogecoin": {
         "api_key": "",
-        "client_class": "LitecoindClient",
-        "denominator": 100000000,
-        "network": "litecoin",
-        "network_overrides": null,
-        "priority": 20,
-        "provider": "litecoind",
-        "provider_coin_id": "",
-        "url": ""
-    },
-    "litecoind.testnet": {
-        "api_key": "",
-        "client_class": "LitecoindClient",
+        "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
-        "network": "litecoin_testnet",
+        "network": "dogecoin",
         "network_overrides": null,
-        "priority": 20,
-        "provider": "litecoind",
+        "priority": 10,
+        "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": ""
+        "url": "https://dogeblocks.com/api/v1/"
     },
-    "litecoreio.litecoin": {
+    "litecoinblockexplorer.litecoin": {
         "api_key": "",
-        "client_class": "LitecoreIOClient",
+        "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
         "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
-        "provider": "litecoreio",
+        "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://insight.litecore.io/api/"
+        "url": "https://litecoinblockexplorer.net/api/v1/"
     },
-    "litecoreio.litecoin.legacy": {
+    "litecoinblockexplorer.litecoin.legacy": {
         "api_key": "",
-        "client_class": "LitecoreIOClient",
+        "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
         "network": "litecoin_legacy",
-        "network_overrides": {
-            "prefix_address_p2sh": "32"
-        },
+        "network_overrides": null,
         "priority": 10,
-        "provider": "litecoreio",
+        "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://insight.litecore.io/api/"
+        "url": "https://litecoinblockexplorer.net/api/v1/"
     },
-    "litecoreio.litecoin.testnet": {
+    "litecoinblockexplorer.testnet2": {
         "api_key": "",
-        "client_class": "LitecoreIOClient",
+        "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
-        "network": "litecoin_testnet",
+        "network": "testnet",
         "network_overrides": null,
         "priority": 10,
-        "provider": "litecoreio",
+        "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://testnet.litecore.io/api/"
+        "url": "https://tbtc1.blockbook.bitaccess.net/api/v1/"
     },
-    "smartbit": {
+    "mempool": {
         "api_key": "",
-        "client_class": "SmartbitClient",
-        "denominator": 100000000,
+        "client_class": "MempoolClient",
+        "denominator": 1,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
-        "provider": "smartbit",
+        "provider": "mempool",
         "provider_coin_id": "",
-        "url": "https://api.smartbit.com.au/v1/"
+        "url": "https://mempool.space/api/"
     },
-    "smartbit.testnet": {
+    "mempool.testnet": {
         "api_key": "",
-        "client_class": "SmartbitClient",
-        "denominator": 100000000,
+        "client_class": "MempoolClient",
+        "denominator": 1,
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
-        "provider": "smartbit",
+        "provider": "mempool",
         "provider_coin_id": "",
-        "url": "https://testnet-api.smartbit.com.au/v1/"
+        "url": "https://mempool.space/testnet/api/"
     }
 }
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/providers.json` & `bitcoinlib-0.6.9/bitcoinlib/data/providers.old.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7789855072463767%*

 * *Differences: {"'blockcypher'": "OrderedDict([('provider', 'blockcypher'), ('network', 'bitcoin'), "*

 * *                  "('client_class', 'BlockCypher'), ('provider_coin_id', ''), ('url', "*

 * *                  "'https://api.blockcypher.com/v1/btc/main/'), ('api_key', ''), ('priority', 10), "*

 * *                  "('denominator', 1), ('network_overrides', None)])",*

 * * "'blockcypher.testnet'": "OrderedDict([('provider', 'blockcypher'), ('network', 'testnet'), "*

 * *                          "('client_class', 'BlockCypher'), ('provider […]*

```diff
@@ -149,14 +149,25 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockchair",
         "provider_coin_id": "",
         "url": "https://api.blockchair.com/bitcoin/testnet/"
     },
+    "blockcypher": {
+        "api_key": "",
+        "client_class": "BlockCypher",
+        "denominator": 1,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "blockcypher",
+        "provider_coin_id": "",
+        "url": "https://api.blockcypher.com/v1/btc/main/"
+    },
     "blockcypher.dogecoin": {
         "api_key": "",
         "client_class": "BlockCypher",
         "denominator": 1,
         "network": "dogecoin",
         "network_overrides": null,
         "priority": 10,
@@ -184,35 +195,35 @@
         "network": "litecoin_legacy",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockcypher",
         "provider_coin_id": "",
         "url": "https://api.blockcypher.com/v1/ltc/main/"
     },
-    "blocksmurfer": {
+    "blockcypher.testnet": {
         "api_key": "",
-        "client_class": "BlocksmurferClient",
-        "denominator": 100000000,
-        "network": "bitcoin",
+        "client_class": "BlockCypher",
+        "denominator": 1,
+        "network": "testnet",
         "network_overrides": null,
         "priority": 10,
-        "provider": "blocksmurfer",
+        "provider": "blockcypher",
         "provider_coin_id": "",
-        "url": "https://harari.blocksmurfer.io/api/v1/btc/"
+        "url": "https://api.blockcypher.com/v1/btc/test3/"
     },
-    "blocksmurfer.testnet": {
+    "blocksmurfer": {
         "api_key": "",
         "client_class": "BlocksmurferClient",
         "denominator": 100000000,
-        "network": "testnet",
+        "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "blocksmurfer",
         "provider_coin_id": "",
-        "url": "https://harari.blocksmurfer.io/api/v1/tbtc/"
+        "url": "http://blocksmurfer.io/api/v1/btc/"
     },
     "blockstream": {
         "api_key": "",
         "client_class": "BlockstreamClient",
         "denominator": 100000000,
         "network": "bitcoin",
         "network_overrides": null,
@@ -228,14 +239,25 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockstream",
         "provider_coin_id": "",
         "url": "https://blockstream.info/testnet/api/"
     },
+    "chainso": {
+        "api_key": "",
+        "client_class": "ChainSo",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 8,
+        "provider": "chainso",
+        "provider_coin_id": "BTC",
+        "url": "https://chain.so/api/v2/"
+    },
     "chainso.dash": {
         "api_key": "",
         "client_class": "ChainSo",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
@@ -316,38 +338,49 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "chainso",
         "provider_coin_id": "BTCTEST",
         "url": "https://chain.so/api/v2/"
     },
+    "coinfees": {
+        "api_key": "",
+        "client_class": "CoinfeesClient",
+        "denominator": 1,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "coinfees",
+        "provider_coin_id": "",
+        "url": "https://bitcoinfees.earn.com/api/v1/"
+    },
     "cryptoid.dash": {
-        "api_key": "api-key-needed",
+        "api_key": "",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "dash",
         "url": "https://chainz.cryptoid.info/"
     },
     "cryptoid.litecoin": {
-        "api_key": "api-key-needed",
+        "api_key": "",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "ltc",
         "url": "https://chainz.cryptoid.info/"
     },
     "cryptoid.litecoin.legacy": {
-        "api_key": "api-key-needed",
+        "api_key": "",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "litecoin_legacy",
         "network_overrides": {
             "prefix_address_p2sh": "32"
         },
         "priority": 10,
@@ -393,43 +426,56 @@
         "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
         "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://litecoinblockexplorer.net/api/v1/"
+        "url": "https://litecoinblockexplorer.net/api/"
     },
     "litecoinblockexplorer.litecoin.legacy": {
         "api_key": "",
         "client_class": "LitecoinBlockexplorerClient",
         "denominator": 100000000,
         "network": "litecoin_legacy",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
-        "url": "https://litecoinblockexplorer.net/api/v1/"
+        "url": "https://litecoinblockexplorer.net/api/"
     },
-    "mempool": {
+    "litecoreio.litecoin": {
         "api_key": "",
-        "client_class": "MempoolClient",
-        "denominator": 1,
-        "network": "bitcoin",
+        "client_class": "LitecoreIOClient",
+        "denominator": 100000000,
+        "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
-        "provider": "mempool",
+        "provider": "litecoreio",
         "provider_coin_id": "",
-        "url": "https://mempool.space/api/"
+        "url": "https://insight.litecore.io/api/"
     },
-    "mempool.testnet": {
+    "litecoreio.litecoin.legacy": {
         "api_key": "",
-        "client_class": "MempoolClient",
-        "denominator": 1,
-        "network": "testnet",
+        "client_class": "LitecoreIOClient",
+        "denominator": 100000000,
+        "network": "litecoin_legacy",
+        "network_overrides": {
+            "prefix_address_p2sh": "32"
+        },
+        "priority": 10,
+        "provider": "litecoreio",
+        "provider_coin_id": "",
+        "url": "https://insight.litecore.io/api/"
+    },
+    "litecoreio.litecoin.testnet": {
+        "api_key": "",
+        "client_class": "LitecoreIOClient",
+        "denominator": 100000000,
+        "network": "litecoin_testnet",
         "network_overrides": null,
         "priority": 10,
-        "provider": "mempool",
+        "provider": "litecoreio",
         "provider_coin_id": "",
-        "url": "https://mempool.space/testnet/api/"
+        "url": "https://testnet.litecore.io/api/"
     }
 }
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/data/providers.old.json` & `bitcoinlib-0.6.9/bitcoinlib/data/providers.examples.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6792452830188679%*

 * *Differences: {"'bcoin'": "OrderedDict([('provider', 'bcoin'), ('network', 'bitcoin'), ('client_class', "*

 * *            "'BcoinClient'), ('provider_coin_id', ''), ('url', ''), ('api_key', ''), ('priority', "*

 * *            "20), ('denominator', 100000000), ('network_overrides', None)])",*

 * * "'bcoin.testnet'": "OrderedDict([('provider', 'bcoin'), ('network', 'testnet'), ('client_class', "*

 * *                    "'BcoinClient'), ('provider_coin_id', ''), ('url', ''), ('api_key', ''), "*

 * *                    "('priority', 20), ('denomi […]*

```diff
@@ -1,8 +1,30 @@
 {
+    "bcoin": {
+        "api_key": "",
+        "client_class": "BcoinClient",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "bcoin",
+        "provider_coin_id": "",
+        "url": ""
+    },
+    "bcoin.testnet": {
+        "api_key": "",
+        "client_class": "BcoinClient",
+        "denominator": 100000000,
+        "network": "testnet",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "bcoin",
+        "provider_coin_id": "",
+        "url": ""
+    },
     "bitaps": {
         "api_key": "",
         "client_class": "BitapsClient",
         "denominator": 100000000,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
@@ -50,14 +72,36 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "bitaps",
         "provider_coin_id": "",
         "url": "https://api.bitaps.com/btc/testnet/v1/"
     },
+    "bitcoind": {
+        "api_key": "",
+        "client_class": "BitcoindClient",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "bitcoind",
+        "provider_coin_id": "",
+        "url": "http://rpcuser:mypasswod@localhost:8332"
+    },
+    "bitcoind.testnet": {
+        "api_key": "",
+        "client_class": "BitcoindClient",
+        "denominator": 100000000,
+        "network": "testnet",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "bitcoind",
+        "provider_coin_id": "",
+        "url": "http://rpcuser:mypasswod@localhost:18332"
+    },
     "bitcoinlib_test": {
         "api_key": "",
         "client_class": "BitcoinLibTestClient",
         "denominator": 100000000,
         "network": "bitcoinlib_test",
         "network_overrides": null,
         "priority": 10,
@@ -105,58 +149,14 @@
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockchair",
         "provider_coin_id": "",
         "url": "https://api.blockchair.com/bitcoin/"
     },
-    "blockchair.dash": {
-        "api_key": "",
-        "client_class": "BlockChairClient",
-        "denominator": 100000000,
-        "network": "dash",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "blockchair",
-        "provider_coin_id": "",
-        "url": "https://api.blockchair.com/dash/"
-    },
-    "blockchair.dogecoin": {
-        "api_key": "",
-        "client_class": "BlockChairClient",
-        "denominator": 100000000,
-        "network": "dogecoin",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "blockchair",
-        "provider_coin_id": "",
-        "url": "https://api.blockchair.com/dogecoin/"
-    },
-    "blockchair.litecoin": {
-        "api_key": "",
-        "client_class": "BlockChairClient",
-        "denominator": 100000000,
-        "network": "litecoin",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "blockchair",
-        "provider_coin_id": "",
-        "url": "https://api.blockchair.com/litecoin/"
-    },
-    "blockchair.testnet": {
-        "api_key": "",
-        "client_class": "BlockChairClient",
-        "denominator": 100000000,
-        "network": "testnet",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "blockchair",
-        "provider_coin_id": "",
-        "url": "https://api.blockchair.com/bitcoin/testnet/"
-    },
     "blockcypher": {
         "api_key": "",
         "client_class": "BlockCypher",
         "denominator": 1,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
@@ -206,25 +206,14 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockcypher",
         "provider_coin_id": "",
         "url": "https://api.blockcypher.com/v1/btc/test3/"
     },
-    "blocksmurfer": {
-        "api_key": "",
-        "client_class": "BlocksmurferClient",
-        "denominator": 100000000,
-        "network": "bitcoin",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "blocksmurfer",
-        "provider_coin_id": "",
-        "url": "http://blocksmurfer.io/api/v1/btc/"
-    },
     "blockstream": {
         "api_key": "",
         "client_class": "BlockstreamClient",
         "denominator": 100000000,
         "network": "bitcoin",
         "network_overrides": null,
         "priority": 10,
@@ -239,25 +228,14 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "blockstream",
         "provider_coin_id": "",
         "url": "https://blockstream.info/testnet/api/"
     },
-    "chainso": {
-        "api_key": "",
-        "client_class": "ChainSo",
-        "denominator": 100000000,
-        "network": "bitcoin",
-        "network_overrides": null,
-        "priority": 8,
-        "provider": "chainso",
-        "provider_coin_id": "BTC",
-        "url": "https://chain.so/api/v2/"
-    },
     "chainso.dash": {
         "api_key": "",
         "client_class": "ChainSo",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
@@ -338,25 +316,14 @@
         "network": "testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "chainso",
         "provider_coin_id": "BTCTEST",
         "url": "https://chain.so/api/v2/"
     },
-    "coinfees": {
-        "api_key": "",
-        "client_class": "CoinfeesClient",
-        "denominator": 1,
-        "network": "bitcoin",
-        "network_overrides": null,
-        "priority": 10,
-        "provider": "coinfees",
-        "provider_coin_id": "",
-        "url": "https://bitcoinfees.earn.com/api/v1/"
-    },
     "cryptoid.dash": {
         "api_key": "",
         "client_class": "CryptoID",
         "denominator": 100000000,
         "network": "dash",
         "network_overrides": null,
         "priority": 10,
@@ -384,14 +351,36 @@
             "prefix_address_p2sh": "32"
         },
         "priority": 10,
         "provider": "cryptoid",
         "provider_coin_id": "ltc",
         "url": "https://chainz.cryptoid.info/"
     },
+    "dashd": {
+        "api_key": "",
+        "client_class": "DashdClient",
+        "denominator": 100000000,
+        "network": "dash",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "dashd",
+        "provider_coin_id": "",
+        "url": ""
+    },
+    "dashd.testnet": {
+        "api_key": "",
+        "client_class": "DashdClient",
+        "denominator": 100000000,
+        "network": "dash_testnet",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "dashd",
+        "provider_coin_id": "",
+        "url": ""
+    },
     "dogecoin": {
         "api_key": "",
         "client_class": "DogecoindClient",
         "denominator": 100000000,
         "network": "dogecoin",
         "network_overrides": null,
         "priority": 20,
@@ -439,14 +428,36 @@
         "network": "litecoin_legacy",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoinblockexplorer",
         "provider_coin_id": "",
         "url": "https://litecoinblockexplorer.net/api/"
     },
+    "litecoind": {
+        "api_key": "",
+        "client_class": "LitecoindClient",
+        "denominator": 100000000,
+        "network": "litecoin",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "litecoind",
+        "provider_coin_id": "",
+        "url": ""
+    },
+    "litecoind.testnet": {
+        "api_key": "",
+        "client_class": "LitecoindClient",
+        "denominator": 100000000,
+        "network": "litecoin_testnet",
+        "network_overrides": null,
+        "priority": 20,
+        "provider": "litecoind",
+        "provider_coin_id": "",
+        "url": ""
+    },
     "litecoreio.litecoin": {
         "api_key": "",
         "client_class": "LitecoreIOClient",
         "denominator": 100000000,
         "network": "litecoin",
         "network_overrides": null,
         "priority": 10,
@@ -473,9 +484,31 @@
         "denominator": 100000000,
         "network": "litecoin_testnet",
         "network_overrides": null,
         "priority": 10,
         "provider": "litecoreio",
         "provider_coin_id": "",
         "url": "https://testnet.litecore.io/api/"
+    },
+    "smartbit": {
+        "api_key": "",
+        "client_class": "SmartbitClient",
+        "denominator": 100000000,
+        "network": "bitcoin",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "smartbit",
+        "provider_coin_id": "",
+        "url": "https://api.smartbit.com.au/v1/"
+    },
+    "smartbit.testnet": {
+        "api_key": "",
+        "client_class": "SmartbitClient",
+        "denominator": 100000000,
+        "network": "testnet",
+        "network_overrides": null,
+        "priority": 10,
+        "provider": "smartbit",
+        "provider_coin_id": "",
+        "url": "https://testnet-api.smartbit.com.au/v1/"
     }
 }
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/db.py` & `bitcoinlib-0.6.9/bitcoinlib/db.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/db_cache.py` & `bitcoinlib-0.6.9/bitcoinlib/db_cache.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/encoding.py` & `bitcoinlib-0.6.9/bitcoinlib/encoding.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/keys.py` & `bitcoinlib-0.6.9/bitcoinlib/keys.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/main.py` & `bitcoinlib-0.6.9/bitcoinlib/main.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/mnemonic.py` & `bitcoinlib-0.6.9/bitcoinlib/mnemonic.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/networks.py` & `bitcoinlib-0.6.9/bitcoinlib/networks.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/scripts.py` & `bitcoinlib-0.6.9/bitcoinlib/scripts.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/__init__.py` & `bitcoinlib-0.6.9/bitcoinlib/services/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,10 +32,10 @@
 import bitcoinlib.services.blockchair
 import bitcoinlib.services.bcoin
 import bitcoinlib.services.bitaps
 import bitcoinlib.services.litecoinblockexplorer
 import bitcoinlib.services.insightdash
 import bitcoinlib.services.blockstream
 import bitcoinlib.services.blocksmurfer
-import bitcoinlib.services.chainso
 import bitcoinlib.services.mempool
 import bitcoinlib.services.bitflyer
+import bitcoinlib.services.blockbook
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/authproxy.py` & `bitcoinlib-0.6.9/bitcoinlib/services/authproxy.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/baseclient.py` & `bitcoinlib-0.6.9/bitcoinlib/services/baseclient.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bcoin.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bcoin.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         return int(balance)
 
     def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
         # First get all transactions for this address from the blockchain
         txs = self.gettransactions(address, limit=50)
 
         # Fail if large number of transactions are found
-        if not len(txs) >= 50:
+        if len(txs) > 50:
             raise ClientError("If not all transactions are known, we cannot determine utxo's")
 
         utxos = []
         for tx in txs:
             for unspent in tx.outputs:
                 if unspent.address != address:
                     continue
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bitaps.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bitgo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    BitAps client
-#    © 2019 August - 1200 Web Development <http://1200wd.com/>
+#    BitGo Client
+#    © 2017-2019 July - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -22,208 +22,184 @@
 from datetime import datetime
 from bitcoinlib.main import MAX_TRANSACTIONS
 from bitcoinlib.services.baseclient import BaseClient, ClientError
 from bitcoinlib.transactions import Transaction
 
 _logger = logging.getLogger(__name__)
 
-PROVIDERNAME = 'bitaps'
-# Please note: In the Bitaps API, the first couple of Bitcoin blocks are not correctly indexed,
-# so transactions from these blocks are missing.
+PROVIDERNAME = 'bitgo'
+LIMIT_TX = 49
 
 
-class BitapsClient(BaseClient):
+class BitGoClient(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
-    def compose_request(self, category, command='', data='', variables=None, req_type='blockchain', method='get'):
-        url_path = req_type + '/' + category
-        if command:
-            url_path += '/' + command
+    def compose_request(self, category, data, cmd='', variables=None, method='get'):
         if data:
-            if url_path[-1:] != '/':
-                url_path += '/'
-            url_path += data
-        return self.request(url_path, variables=variables, method=method)
-
-    # def _parse_transaction(self, tx):
-    #     status = 'unconfirmed'
-    #     if tx['confirmations']:
-    #         status = 'confirmed'
-    #     date = None
-    #     if 'timestamp' in tx and tx['timestamp']:
-    #         date = datetime.utcfromtimestamp(tx['timestamp'])
-    #     elif 'blockTime' in tx and tx['blockTime']:
-    #         date = datetime.utcfromtimestamp(tx['blockTime'])
-    #     block_height = None
-    #     if 'blockHeight' in tx:
-    #         block_height = tx['blockHeight']
-    #     witness_type = 'legacy'
-    #     if tx['segwit']:
-    #         witness_type = 'segwit'
-    #
-    #     t = Transaction(
-    #         locktime=tx['lockTime'], version=tx['version'], network=self.network, fee=tx['fee'],
-    #         fee_per_kb=None if 'feeRate' not in tx else int(tx['feeRate']), size=tx['size'],
-    #         txid=tx['txId'], date=date, confirmations=tx['confirmations'], block_height=block_height,
-    #         input_total=tx['inputsAmount'], output_total=tx['outputsAmount'], status=status, coinbase=tx['coinbase'],
-    #         verified=None if 'valid' not in tx else tx['valid'], witness_type=witness_type)
-    #
-    #     for n, ti in tx['vIn'].items():
-    #         if t.coinbase:
-    #             t.add_input(prev_txid=ti['txId'], output_n=ti['vOut'], unlocking_script=ti['scriptSig'],
-    #                         sequence=ti['sequence'], index_n=int(n), value=0)
-    #         else:
-    #             t.add_input(prev_txid=ti['txId'], output_n=ti['vOut'], unlocking_script=ti['scriptSig'],
-    #                         unlocking_script_unsigned=ti['scriptPubKey'],
-    #                         address='' if 'address' not in ti else ti['address'], sequence=ti['sequence'],
-    #                         index_n=int(n), value=ti['amount'], strict=self.strict)
-    #
-    #     for _, to in tx['vOut'].items():
-    #         spending_txid = None if not to['spent'] else to['spent'][0]['txId']
-    #         spending_index_n = None if not to['spent'] else to['spent'][0]['vIn']
-    #         t.add_output(to['value'], '' if 'address' not in to else to['address'],
-    #                      '' if 'addressHash' not in to else to['addressHash'], lock_script=to['scriptPubKey'],
-    #                      spent=bool(to['spent']), spending_txid=spending_txid, spending_index_n=spending_index_n,
-    #                      strict=self.strict)
-    #
-    #     return t
-
-    def getbalance(self, addresslist):
-        balance = 0
-        for address in addresslist:
-            res = self.compose_request('address', 'state', address)
-            balance += res['data']['balance']
-        return balance
+            data = '/' + data
+        url_path = category + data
+        if cmd != '':
+            url_path += '/' + cmd
+        return self.request(url_path, variables, method=method)
+
+    # def getbalance(self, addresslist):
+    #     balance = 0
+    #     for address in addresslist:
+    #         res = self.compose_request('address', address)
+    #         balance += res['balance']
+    #     return balance
 
     def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
         utxos = []
-        page = 1
-        while True:
-            variables = {'mode': 'verbose', 'limit': 50, 'page': page, 'order': 'asc'}
-            try:
-                res = self.compose_request('address', 'transactions', address, variables)
-                res2 = self.compose_request('address', 'unconfirmed/transactions', address, variables)
-            except ClientError as e:
-                if "address not found" in self.resp.text:
-                    return []
-                else:
-                    raise ClientError(e.msg)
-            txs = res['data']['list']
-            txs += res2['data']['list']
-            for tx in txs:
-                for outp in tx['vOut']:
-                    utxo = tx['vOut'][outp]
-                    if 'address' not in utxo or utxo['address'] != address or utxo['spent']:
-                        continue
-                    utxos.append(
-                        {
-                            'address': utxo['address'],
-                            'txid': tx['txId'],
-                            'confirmations': 0 if 'confirmations' not in tx else tx['confirmations'],
-                            'output_n': int(outp),
-                            'input_n': 0,
-                            'block_height': None if 'blockHeight' not in tx else tx['blockHeight'],
-                            'fee': None,
-                            'size': 0,
-                            'value': utxo['value'],
-                            'script': utxo['scriptPubKey'],
-                            'date': datetime.utcfromtimestamp(tx['timestamp'])
-                         }
-                    )
-                if tx['txId'] == after_txid:
-                    utxos = []
-            page += 1
-            if page > res['data']['pages']:
+        skip = 0
+        total = 1
+        while total > skip:
+            variables = {'limit': 100, 'skip': skip}
+            res = self.compose_request('address', address, 'unspents', variables)
+            for utxo in res['unspents'][::-1]:
+                if utxo['tx_hash'] == after_txid:
+                    break
+                utxos.append(
+                    {
+                        'address': utxo['address'],
+                        'txid': utxo['tx_hash'],
+                        'confirmations': utxo['confirmations'],
+                        'output_n': utxo['tx_output_n'],
+                        'input_n': 0,
+                        'block_height': int(utxo['blockHeight']) if utxo['blockHeight'] else None,
+                        'fee': None,
+                        'size': 0,
+                        'value': int(round(utxo['value'] * self.units, 0)),
+                        'script': utxo['script'],
+                        'date': datetime.strptime(utxo['date'], "%Y-%m-%dT%H:%M:%S.%fZ")
+                     }
+                )
+            total = res['total']
+            skip = res['start'] + res['count']
+            if skip > 2000:
+                _logger.info("BitGoClient: UTXO's list has been truncated, list is incomplete")
                 break
-        return utxos[:limit]
+        return utxos[::-1][:limit]
 
-    # FIXME: Disabled results very unpredictable, seem randomized... :(
+    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
     # def gettransaction(self, txid):
-    #     res = self.compose_request('transaction', txid)
-    #     return self._parse_transaction(res['data'])
-    #
+    #     tx = self.compose_request('tx', txid)
+    #     t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
+    #     t.status = 'unconfirmed'
+    #     t.date = None
+    #     if tx['confirmations']:
+    #         t.status = 'confirmed'
+    #         t.date = datetime.strptime(tx['date'], "%Y-%m-%dT%H:%M:%S.%fZ")
+    #     t.confirmations = tx['confirmations']
+    #     if 'height' in tx:
+    #         t.block_height = tx['height']
+    #         t.block_hash = tx['blockhash']
+    #     t.fee = tx['fee']
+    #     t.rawtx = to_bytes(tx['hex'])
+    #     t.size = len(tx['hex']) // 2
+    #     t.network = self.network
+    #     if t.coinbase:
+    #         input_values = []
+    #         t.input_total = t.output_total
+    #     else:
+    #         input_values = [(inp['account'], -inp['value']) for inp in tx['entries'] if inp['value'] < 0]
+    #         if len(input_values) >= 49:
+    #             raise ClientError("More then 49 transaction inputs not supported by bitgo")
+    #         t.input_total = sum([x[1] for x in input_values])
+    #     for i in t.inputs:
+    #         if not i.address and not t.coinbase:
+    #             raise ClientError("Address missing in input. Provider might not support segwit transactions")
+    #         if len(t.inputs) != len(input_values):
+    #             i.value = None
+    #             continue
+    #         value = [x[1] for x in input_values if x[0] == i.address]
+    #         if len(value) != 1:
+    #             _logger.info("BitGoClient: Address %s input value should be found exactly 1 times in value list" %
+    #                             i.address)
+    #             i.value = None
+    #         else:
+    #             i.value = value[0]
+    #     for o in t.outputs:
+    #         o.spent = None
+    #     if t.input_total != t.output_total + t.fee:
+    #         t.input_total = t.output_total + t.fee
+    #     return t
+
+    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
     # def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-    #     page = 0
     #     txs = []
-    #     while True:
-    #         variables = {'mode': 'verbose', 'limit': 50, 'page': page, 'order': 'asc'}
-    #         try:
-    #             res = self.compose_request('address', 'transactions', address, variables)
-    #         except ClientError:
-    #             if "address not found" in self.resp.text:
-    #                 return []
-    #         for tx in res['data']['list']:
-    #             txs.append(self._parse_transaction(tx))
-    #             if tx['txId'] == after_txid:
-    #                 txs = []
-    #         if len(txs) > limit:
+    #     txids = []
+    #     skip = 0
+    #     total = 1
+    #     while total > skip:
+    #         variables = {'limit': LIMIT_TX, 'skip': skip}
+    #         res = self.compose_request('address', address, 'tx', variables)
+    #         for tx in res['transactions']:
+    #             if tx['id'] not in txids:
+    #                 txids.insert(0, tx['id'])
+    #         total = res['total']
+    #         # if total > 2000:
+    #         #     raise ClientError("BitGoClient: Transactions list limit exceeded > 2000")
+    #         skip = res['start'] + res['count']
+    #         if len(txids) > limit:
     #             break
-    #         page += 1
-    #         if page >= res['data']['pages']:
-    #             break
-    #     return txs[:limit]
+    #     if after_txid:
+    #         txids = txids[txids.index(after_txid) + 1:]
+    #     for txid in txids[:limit]:
+    #         txs.append(self.gettransaction(txid))
+    #     return txs
 
+    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
     # def getrawtransaction(self, txid):
-    #     tx = self.compose_request('transaction', txid)
-    #     return tx['data']['rawTx']
+    #     tx = self.compose_request('tx', txid)
+    #     t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
+    #     for i in t.inputs:
+    #         if not i.address:
+    #             raise ClientError("Address missing in input. Provider might not support segwit transactions")
+    #     return tx['hex']
 
     # def sendrawtransaction
 
-    # def estimatefee
+    def estimatefee(self, blocks):
+        res = self.compose_request('tx', 'fee', variables={'numBlocks': blocks})
+        return res['feePerKb']
 
     def blockcount(self):
-        return self.compose_request('block', 'last')['data']['height']
+        return self.compose_request('block', 'latest')['height']
 
-    # def mempool(self, txid):
-    #     if txid:
-    #         t = self.gettransaction(txid)
-    #         if t and not t.confirmations:
-    #             return [t.txid]
-    #     else:
-    #         res = self.compose_request('transactions', type='mempool')
-    #         return [tx['hash'] for tx in res['data']['transactions']]
-    #     return []
+    # def mempool
 
-    # FIXME: Bitaps doesn't seem to return block data anymore...
     # def getblock(self, blockid, parse_transactions, page, limit):
-    #     if limit > 100:
-    #         limit = 100
-    #     res = self.compose_request('block', str(blockid),
-    #                                variables={'transactions': True, 'limit': limit, 'page': page})
-    #     bd = res['data']['block']
-    #     td = res['data']['transactions']
-    #     txids = [tx['txId'] for tx in td['list']]
+    #     bd = self.compose_request('block', str(blockid))
     #     if parse_transactions:
     #         txs = []
-    #         for txid in txids:
+    #         for txid in bd['transactions'][(page-1)*limit:page*limit]:
     #             try:
     #                 txs.append(self.gettransaction(txid))
     #             except Exception as e:
     #                 _logger.error("Could not parse tx %s with error %s" % (txid, e))
     #     else:
-    #         txs = txids
+    #         txs = bd['transactions']
     #
     #     block = {
-    #         'bits': bd['bits'],
-    #         'depth': bd['confirmations'],
-    #         'hash': bd['hash'],
+    #         'bits': None,
+    #         'depth': None,
+    #         'hash': bd['id'],
     #         'height': bd['height'],
     #         'merkle_root': bd['merkleRoot'],
     #         'nonce': bd['nonce'],
-    #         'prev_block': bd['previousBlockHash'],
-    #         'time': datetime.utcfromtimestamp(bd['blockTime']),
-    #         'total_txs': bd['transactionsCount'],
+    #         'prev_block': bd['previous'],
+    #         'time': datetime.strptime(bd['date'], "%Y-%m-%dT%H:%M:%S.%fZ").replace(microsecond=0),
+    #         'total_txs': len(bd['transactions']),
     #         'txs': txs,
     #         'version': bd['version'],
-    #         'page': td['page'],
-    #         'pages': td['pages'],
-    #         'limit': td['limit']
+    #         'page': page,
+    #         'pages': None if not limit else int(len(bd['transactions']) // limit) + (len(bd['transactions']) % limit > 0),
+    #         'limit': limit
     #     }
     #     return block
 
-    # def isspent(self, txid, output_n):
-    #     t = self.gettransaction(txid)
-    #     return 1 if t.outputs[output_n].spent else 0
+    # def isspent(self, txid, index):
 
     # def getinfo(self):
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bitcoind.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bitcoind.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bitcoinlibtest.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bitcoinlibtest.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bitflyer.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bitflyer.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/bitgo.py` & `bitcoinlib-0.6.9/bitcoinlib/services/blockcypher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    BitGo Client
+#    BlockCypher client
 #    © 2017-2019 July - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
@@ -16,190 +16,205 @@
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import logging
 from datetime import datetime
+from datetime import timezone
 from bitcoinlib.main import MAX_TRANSACTIONS
 from bitcoinlib.services.baseclient import BaseClient, ClientError
 from bitcoinlib.transactions import Transaction
 
-_logger = logging.getLogger(__name__)
+PROVIDERNAME = 'blockcypher'
 
-PROVIDERNAME = 'bitgo'
-LIMIT_TX = 49
+_logger = logging.getLogger(__name__)
 
 
-class BitGoClient(BaseClient):
+class BlockCypher(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
-    def compose_request(self, category, data, cmd='', variables=None, method='get'):
-        if data:
-            data = '/' + data
-        url_path = category + data
-        if cmd != '':
-            url_path += '/' + cmd
-        return self.request(url_path, variables, method=method)
-
-    # def getbalance(self, addresslist):
-    #     balance = 0
-    #     for address in addresslist:
-    #         res = self.compose_request('address', address)
-    #         balance += res['balance']
-    #     return balance
-
-    def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-        utxos = []
-        skip = 0
-        total = 1
-        while total > skip:
-            variables = {'limit': 100, 'skip': skip}
-            res = self.compose_request('address', address, 'unspents', variables)
-            for utxo in res['unspents'][::-1]:
-                if utxo['tx_hash'] == after_txid:
-                    break
-                utxos.append(
-                    {
-                        'address': utxo['address'],
-                        'txid': utxo['tx_hash'],
-                        'confirmations': utxo['confirmations'],
-                        'output_n': utxo['tx_output_n'],
-                        'input_n': 0,
-                        'block_height': int(utxo['blockHeight']) if utxo['blockHeight'] else None,
-                        'fee': None,
-                        'size': 0,
-                        'value': int(round(utxo['value'] * self.units, 0)),
-                        'script': utxo['script'],
-                        'date': datetime.strptime(utxo['date'], "%Y-%m-%dT%H:%M:%S.%fZ")
-                     }
-                )
-            total = res['total']
-            skip = res['start'] + res['count']
-            if skip > 2000:
-                _logger.info("BitGoClient: UTXO's list has been truncated, list is incomplete")
-                break
-        return utxos[::-1][:limit]
-
-    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
-    # def gettransaction(self, txid):
-    #     tx = self.compose_request('tx', txid)
-    #     t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
-    #     t.status = 'unconfirmed'
-    #     t.date = None
-    #     if tx['confirmations']:
-    #         t.status = 'confirmed'
-    #         t.date = datetime.strptime(tx['date'], "%Y-%m-%dT%H:%M:%S.%fZ")
-    #     t.confirmations = tx['confirmations']
-    #     if 'height' in tx:
-    #         t.block_height = tx['height']
-    #         t.block_hash = tx['blockhash']
-    #     t.fee = tx['fee']
-    #     t.rawtx = to_bytes(tx['hex'])
-    #     t.size = len(tx['hex']) // 2
-    #     t.network = self.network
-    #     if t.coinbase:
-    #         input_values = []
-    #         t.input_total = t.output_total
-    #     else:
-    #         input_values = [(inp['account'], -inp['value']) for inp in tx['entries'] if inp['value'] < 0]
-    #         if len(input_values) >= 49:
-    #             raise ClientError("More then 49 transaction inputs not supported by bitgo")
-    #         t.input_total = sum([x[1] for x in input_values])
-    #     for i in t.inputs:
-    #         if not i.address and not t.coinbase:
-    #             raise ClientError("Address missing in input. Provider might not support segwit transactions")
-    #         if len(t.inputs) != len(input_values):
-    #             i.value = None
-    #             continue
-    #         value = [x[1] for x in input_values if x[0] == i.address]
-    #         if len(value) != 1:
-    #             _logger.info("BitGoClient: Address %s input value should be found exactly 1 times in value list" %
-    #                             i.address)
-    #             i.value = None
-    #         else:
-    #             i.value = value[0]
-    #     for o in t.outputs:
-    #         o.spent = None
-    #     if t.input_total != t.output_total + t.fee:
-    #         t.input_total = t.output_total + t.fee
-    #     return t
-
-    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
-    # def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-    #     txs = []
-    #     txids = []
-    #     skip = 0
-    #     total = 1
-    #     while total > skip:
-    #         variables = {'limit': LIMIT_TX, 'skip': skip}
-    #         res = self.compose_request('address', address, 'tx', variables)
-    #         for tx in res['transactions']:
-    #             if tx['id'] not in txids:
-    #                 txids.insert(0, tx['id'])
-    #         total = res['total']
-    #         # if total > 2000:
-    #         #     raise ClientError("BitGoClient: Transactions list limit exceeded > 2000")
-    #         skip = res['start'] + res['count']
-    #         if len(txids) > limit:
-    #             break
-    #     if after_txid:
-    #         txids = txids[txids.index(after_txid) + 1:]
-    #     for txid in txids[:limit]:
-    #         txs.append(self.gettransaction(txid))
-    #     return txs
-
-    # RAW TRANSACTION DOES NOT CONTAIN CORRECT RAW TRANSACTION (MISSING SIGS)
-    # def getrawtransaction(self, txid):
-    #     tx = self.compose_request('tx', txid)
-    #     t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
-    #     for i in t.inputs:
-    #         if not i.address:
-    #             raise ClientError("Address missing in input. Provider might not support segwit transactions")
-    #     return tx['hex']
-
-    # def sendrawtransaction
+    def compose_request(self, function, data, parameter='', variables=None, method='get'):
+        url_path = function + '/' + data
+        if parameter:
+            url_path += '/' + parameter
+        if variables is None:
+            variables = {}
+        if self.api_key:
+            variables.update({'token': self.api_key})
+        return self.request(url_path, variables, method)
+
+    def getbalance(self, addresslist):
+        addresslist = self._addresslist_convert(addresslist)
+        addresses = ';'.join([a.address for a in addresslist])
+        res = self.compose_request('addrs', addresses, 'balance')
+        balance = 0.0
+        if not isinstance(res, list):
+            res = [res]
+        for rec in res:
+            balance += float(rec['final_balance'])
+        return int(balance * self.units)
+
+    # Disabled: Invalid results for https://api.blockcypher.com/v1/ltc/main/addrs/LVqLipGhyQ1nWtPPc8Xp3zn6JxcU1Hi8eG?unspentOnly=1&limit=2000
+    # def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+    #     address = self._address_convert(address)
+    #     res = self.compose_request('addrs', address.address, variables={'unspentOnly': 1, 'limit': 2000})
+    #     transactions = []
+    #     if not isinstance(res, list):
+    #         res = [res]
+    #     for a in res:
+    #         txrefs = a.setdefault('txrefs', []) + a.get('unconfirmed_txrefs', [])
+    #         if len(txrefs) > 500:
+    #             _logger.warning("BlockCypher: Large number of transactions for address %s, "
+    #                             "Transaction list may be incomplete" % address)
+    #         for tx in txrefs:
+    #             if tx['tx_hash'] == after_txid:
+    #                 break
+    #             tdate = None
+    #             if 'confirmed' in tx:
+    #                 try:
+    #                     tdate = datetime.strptime(tx['confirmed'], "%Y-%m-%dT%H:%M:%SZ")
+    #                 except ValueError:
+    #                     tdate = datetime.strptime(tx['confirmed'], "%Y-%m-%dT%H:%M:%S.%fZ")
+    #             transactions.append({
+    #                 'address': address.address_orig,
+    #                 'txid': tx['tx_hash'],
+    #                 'confirmations': tx['confirmations'],
+    #                 'output_n': tx['tx_output_n'],
+    #                 'index': 0,
+    #                 'value': int(round(tx['value'] * self.units, 0)),
+    #                 'script': '',
+    #                 'block_height': None,
+    #                 'date': tdate
+    #             })
+    #     return transactions[::-1][:limit]
+
+    def gettransaction(self, txid):
+        tx = self.compose_request('txs', txid, variables={'includeHex': 'true'})
+        t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
+        if tx['confirmations']:
+            t.status = 'confirmed'
+            t.date = datetime.strptime(tx['confirmed'][:19], "%Y-%m-%dT%H:%M:%S")
+        else:
+            t.status = 'unconfirmed'
+        t.confirmations = tx['confirmations']
+        t.block_height = tx['block_height'] if tx['block_height'] > 0 else None
+        t.fee = tx['fees']
+        t.rawtx = bytes.fromhex(tx['hex'])
+        t.size = int(len(tx['hex']) / 2)
+        t.network = self.network
+        t.input_total = 0
+        if len(t.inputs) != len(tx['inputs']):
+            raise ClientError("Invalid number of inputs provided. Raw tx: %d, blockcypher: %d" %
+                              (len(t.inputs), len(tx['inputs'])))
+        for n, i in enumerate(t.inputs):
+            if not t.coinbase and not (tx['inputs'][n]['output_index'] == i.output_n_int and
+                                       tx['inputs'][n]['prev_hash'] == i.prev_txid.hex()):
+                raise ClientError("Transaction inputs do not match raw transaction")
+            if 'output_value' in tx['inputs'][n]:
+                if not t.coinbase:
+                    i.value = tx['inputs'][n]['output_value']
+                t.input_total += i.value
+        if len(t.outputs) != len(tx['outputs']):
+            raise ClientError("Invalid number of outputs provided. Raw tx: %d, blockcypher: %d" %
+                              (len(t.outputs), len(tx['outputs'])))
+        for n, o in enumerate(t.outputs):
+            if 'spent_by' in tx['outputs'][n]:
+                o.spent = True
+                o.spending_txid = tx['outputs'][n]['spent_by']
+        return t
+
+    def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+        txs = []
+        address = self._address_convert(address)
+        res = self.compose_request('addrs', address.address, variables={'unspentOnly': 0, 'limit': 2000})
+        if not isinstance(res, list):
+            res = [res]
+        for a in res:
+            txrefs = a.get('txrefs', []) + a.get('unconfirmed_txrefs', [])
+            txids = []
+            for t in txrefs[::-1]:
+                if t['tx_hash'] not in txids:
+                    txids.append(t['tx_hash'])
+                if t['tx_hash'] == after_txid:
+                    txids = []
+            if len(txids) > 500:
+                _logger.info("BlockCypher: Large number of transactions for address %s, "
+                             "Transaction list may be incomplete" % address.address_orig)
+            for txid in txids[:limit]:
+                t = self.gettransaction(txid)
+                txs.append(t)
+        return txs
+
+    def getrawtransaction(self, txid):
+        return self.compose_request('txs', txid, variables={'includeHex': 'true'})['hex']
+
+    def sendrawtransaction(self, rawtx):
+        # BlockCypher sometimes accepts transactions, but does not push them to the network :(
+        if self.network.name in ['bitcoin', 'litecoin']:
+            raise ClientError("Avoid stuck transactions, skip usage of blockcypher provider")
+        res = self.compose_request('txs', 'push', variables={'tx': rawtx}, method='post')
+        return {
+            'txid': res['tx']['hash'],
+            'response_dict': res
+        }
 
     def estimatefee(self, blocks):
-        res = self.compose_request('tx', 'fee', variables={'numBlocks': blocks})
-        return res['feePerKb']
+        res = self.compose_request('', '')
+        if blocks <= 10:
+            return res['medium_fee_per_kb']
+        else:
+            return res['low_fee_per_kb']
 
     def blockcount(self):
-        return self.compose_request('block', 'latest')['height']
-
-    # def mempool
-
-    # def getblock(self, blockid, parse_transactions, page, limit):
-    #     bd = self.compose_request('block', str(blockid))
-    #     if parse_transactions:
-    #         txs = []
-    #         for txid in bd['transactions'][(page-1)*limit:page*limit]:
-    #             try:
-    #                 txs.append(self.gettransaction(txid))
-    #             except Exception as e:
-    #                 _logger.error("Could not parse tx %s with error %s" % (txid, e))
-    #     else:
-    #         txs = bd['transactions']
-    #
-    #     block = {
-    #         'bits': None,
-    #         'depth': None,
-    #         'hash': bd['id'],
-    #         'height': bd['height'],
-    #         'merkle_root': bd['merkleRoot'],
-    #         'nonce': bd['nonce'],
-    #         'prev_block': bd['previous'],
-    #         'time': datetime.strptime(bd['date'], "%Y-%m-%dT%H:%M:%S.%fZ").replace(microsecond=0),
-    #         'total_txs': len(bd['transactions']),
-    #         'txs': txs,
-    #         'version': bd['version'],
-    #         'page': page,
-    #         'pages': None if not limit else int(len(bd['transactions']) // limit) + (len(bd['transactions']) % limit > 0),
-    #         'limit': limit
-    #     }
-    #     return block
+        return self.compose_request('', '')['height']
 
-    # def isspent(self, txid, index):
+    def mempool(self, txid):
+        if txid:
+            tx = self.compose_request('txs', txid)
+            if tx['confirmations'] == 0:
+                return [tx['hash']]
+            else:
+                return []
+        return False
+
+    def getblock(self, blockid, parse_transactions, page, limit):
+        if limit > 100:
+            limit = 100
+        bd = self.compose_request('blocks', str(blockid), variables={'limit': limit, 'txstart': ((page-1)*limit)})
+        if parse_transactions:
+            txs = []
+            for txid in bd['txids']:
+                try:
+                    txs.append(self.gettransaction(txid))
+                except Exception as e:
+                    _logger.error("Could not parse tx %s with error %s" % (txid, e))
+        else:
+            txs = bd['txids']
+
+        block = {
+            'bits': bd['bits'],
+            'depth': bd['depth'],
+            'block_hash': bd['hash'],
+            'height': bd['height'],
+            'merkle_root': bd['mrkl_root'],
+            'nonce': bd['nonce'],
+            'prev_block': bd['prev_block'],
+            'time': int(datetime.strptime(bd['time'], "%Y-%m-%dT%H:%M:%SZ").replace(tzinfo=timezone.utc).timestamp()),
+            'tx_count': bd['n_tx'],
+            'txs': txs,
+            'version': bd['ver'],
+            'page': page,
+            'pages': None if not limit else int(bd['n_tx'] // limit) + (bd['n_tx'] % limit > 0),
+            'limit': limit
+        }
+        return block
+
+    # def getrawblock(self, blockid):
+
+    def isspent(self, txid, output_n):
+        t = self.gettransaction(txid)
+        return 1 if t.outputs[output_n].spent else 0
 
     # def getinfo(self):
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/blockchaininfo.py` & `bitcoinlib-0.6.9/bitcoinlib/services/blockchaininfo.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/blockchair.py` & `bitcoinlib-0.6.9/bitcoinlib/services/blockchair.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/blockcypher.py` & `bitcoinlib-0.6.9/bitcoinlib/services/mempool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    BlockCypher client
-#    © 2017-2019 July - 1200 Web Development <http://1200wd.com/>
+#    mempool.space client
+#    © 2021-2022 - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -16,205 +16,207 @@
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import logging
 from datetime import datetime
-from datetime import timezone
 from bitcoinlib.main import MAX_TRANSACTIONS
 from bitcoinlib.services.baseclient import BaseClient, ClientError
 from bitcoinlib.transactions import Transaction
+from bitcoinlib.encoding import varstr
 
-PROVIDERNAME = 'blockcypher'
+PROVIDERNAME = 'mempool'
+# Please note: In the Blockstream API, the first couple of Bitcoin blocks are not correctly indexed,
+# so transactions from these blocks are missing.
 
 _logger = logging.getLogger(__name__)
 
 
-class BlockCypher(BaseClient):
+class MempoolClient(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
-    def compose_request(self, function, data, parameter='', variables=None, method='get'):
-        url_path = function + '/' + data
+    def compose_request(self, function, data='', parameter='', parameter2='', variables=None, post_data='',
+                        method='get'):
+        url_path = function
+        if data:
+            url_path += '/' + data
         if parameter:
             url_path += '/' + parameter
+        if parameter2:
+            url_path += '/' + parameter2
         if variables is None:
             variables = {}
         if self.api_key:
             variables.update({'token': self.api_key})
-        return self.request(url_path, variables, method)
+        return self.request(url_path, variables, method, post_data=post_data)
 
     def getbalance(self, addresslist):
-        addresslist = self._addresslist_convert(addresslist)
-        addresses = ';'.join([a.address for a in addresslist])
-        res = self.compose_request('addrs', addresses, 'balance')
-        balance = 0.0
-        if not isinstance(res, list):
-            res = [res]
-        for rec in res:
-            balance += float(rec['final_balance'])
-        return int(balance * self.units)
-
-    # Disabled: Invalid results for https://api.blockcypher.com/v1/ltc/main/addrs/LVqLipGhyQ1nWtPPc8Xp3zn6JxcU1Hi8eG?unspentOnly=1&limit=2000
-    # def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-    #     address = self._address_convert(address)
-    #     res = self.compose_request('addrs', address.address, variables={'unspentOnly': 1, 'limit': 2000})
-    #     transactions = []
-    #     if not isinstance(res, list):
-    #         res = [res]
-    #     for a in res:
-    #         txrefs = a.setdefault('txrefs', []) + a.get('unconfirmed_txrefs', [])
-    #         if len(txrefs) > 500:
-    #             _logger.warning("BlockCypher: Large number of transactions for address %s, "
-    #                             "Transaction list may be incomplete" % address)
-    #         for tx in txrefs:
-    #             if tx['tx_hash'] == after_txid:
-    #                 break
-    #             tdate = None
-    #             if 'confirmed' in tx:
-    #                 try:
-    #                     tdate = datetime.strptime(tx['confirmed'], "%Y-%m-%dT%H:%M:%SZ")
-    #                 except ValueError:
-    #                     tdate = datetime.strptime(tx['confirmed'], "%Y-%m-%dT%H:%M:%S.%fZ")
-    #             transactions.append({
-    #                 'address': address.address_orig,
-    #                 'txid': tx['tx_hash'],
-    #                 'confirmations': tx['confirmations'],
-    #                 'output_n': tx['tx_output_n'],
-    #                 'index': 0,
-    #                 'value': int(round(tx['value'] * self.units, 0)),
-    #                 'script': '',
-    #                 'block_height': None,
-    #                 'date': tdate
-    #             })
-    #     return transactions[::-1][:limit]
+        balance = 0
+        for address in addresslist:
+            res = self.compose_request('address', address)
+            balance += res['chain_stats']['funded_txo_sum'] - res['chain_stats']['spent_txo_sum']
+        return balance
+
+    def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+        self.latest_block = self.blockcount() if not self.latest_block else self.latest_block
+        res = self.compose_request('address', address, 'utxo')
+        utxos = []
+        # # key=lambda k: (k[2], pow(10, 20)-k[0].transaction_id, k[3]), reverse=True
+        res = sorted(res, key=lambda k: 0 if 'block_height' not in k['status'] else k['status']['block_height'])
+        for a in res:
+            confirmations = 0
+            block_height = None
+            if 'block_height' in a['status']:
+                block_height = a['status']['block_height']
+                confirmations = self.latest_block - block_height
+            utxos.append({
+                'address': address,
+                'txid': a['txid'],
+                'confirmations': confirmations,
+                'output_n': a['vout'],
+                'input_n': 0,
+                'block_height': block_height,
+                'fee': None,
+                'size': 0,
+                'value': a['value'],
+                'script': '',
+                'date': None if 'block_time' not in a['status'] else datetime.utcfromtimestamp(a['status']['block_time'])
+            })
+            if a['txid'] == after_txid:
+                utxos = []
+        return utxos[:limit]
+
+    def _parse_transaction(self, tx):
+        block_height = None if 'block_height' not in tx['status'] else tx['status']['block_height']
+        confirmations = 0
+        tx_date = None
+        status = 'unconfirmed'
+        if tx['status']['confirmed']:
+            if block_height:
+                self.latest_block = self.blockcount() if not self.latest_block else self.latest_block
+                confirmations = self.latest_block - block_height + 1
+            tx_date = datetime.utcfromtimestamp(tx['status']['block_time'])
+            status = 'confirmed'
+
+        t = Transaction(locktime=tx['locktime'], version=tx['version'], network=self.network, block_height=block_height,
+                        fee=tx['fee'], size=tx['size'], txid=tx['txid'], date=tx_date, confirmations=confirmations,
+                        status=status, coinbase=tx['vin'][0]['is_coinbase'])
+        for ti in tx['vin']:
+            if ti['is_coinbase']:
+                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'], unlocking_script=ti['scriptsig'], value=0,
+                            sequence=ti['sequence'], strict=self.strict)
+            else:
+                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'],
+                            unlocking_script=ti['scriptsig'], value=ti['prevout']['value'],
+                            address=ti['prevout'].get('scriptpubkey_address', ''),
+                            unlocking_script_unsigned=ti['prevout']['scriptpubkey'], sequence=ti['sequence'],
+                            witnesses=None if 'witness' not in ti else [bytes.fromhex(w) for w in ti['witness']],
+                            strict=self.strict)
+        for to in tx['vout']:
+            t.add_output(value=to['value'], address=to.get('scriptpubkey_address', ''), spent=None,
+                         lock_script=to['scriptpubkey'], strict=self.strict)
+        if 'segwit' in [i.witness_type for i in t.inputs] or 'p2sh-segwit' in [i.witness_type for i in t.inputs]:
+            t.witness_type = 'segwit'
+        t.update_totals()
+        return t
 
     def gettransaction(self, txid):
-        tx = self.compose_request('txs', txid, variables={'includeHex': 'true'})
-        t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
-        if tx['confirmations']:
-            t.status = 'confirmed'
-            t.date = datetime.strptime(tx['confirmed'][:19], "%Y-%m-%dT%H:%M:%S")
-        else:
-            t.status = 'unconfirmed'
-        t.confirmations = tx['confirmations']
-        t.block_height = tx['block_height'] if tx['block_height'] > 0 else None
-        t.fee = tx['fees']
-        t.rawtx = bytes.fromhex(tx['hex'])
-        t.size = int(len(tx['hex']) / 2)
-        t.network = self.network
-        t.input_total = 0
-        if len(t.inputs) != len(tx['inputs']):
-            raise ClientError("Invalid number of inputs provided. Raw tx: %d, blockcypher: %d" %
-                              (len(t.inputs), len(tx['inputs'])))
-        for n, i in enumerate(t.inputs):
-            if not t.coinbase and not (tx['inputs'][n]['output_index'] == i.output_n_int and
-                                       tx['inputs'][n]['prev_hash'] == i.prev_txid.hex()):
-                raise ClientError("Transaction inputs do not match raw transaction")
-            if 'output_value' in tx['inputs'][n]:
-                if not t.coinbase:
-                    i.value = tx['inputs'][n]['output_value']
-                t.input_total += i.value
-        if len(t.outputs) != len(tx['outputs']):
-            raise ClientError("Invalid number of outputs provided. Raw tx: %d, blockcypher: %d" %
-                              (len(t.outputs), len(tx['outputs'])))
-        for n, o in enumerate(t.outputs):
-            if 'spent_by' in tx['outputs'][n]:
-                o.spent = True
-                o.spending_txid = tx['outputs'][n]['spent_by']
-        return t
+        tx = self.compose_request('tx', txid)
+        return self._parse_transaction(tx)
 
     def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+        prtxs = []
+        before_txid = ''
+        while True:
+            txs = self.compose_request('address', address, 'txs/chain', before_txid)
+            prtxs += txs
+            if len(txs) == 25:
+                before_txid = txs[-1:][0]['txid']
+            else:
+                break
+            if len(prtxs) > limit:
+                break
         txs = []
-        address = self._address_convert(address)
-        res = self.compose_request('addrs', address.address, variables={'unspentOnly': 0, 'limit': 2000})
-        if not isinstance(res, list):
-            res = [res]
-        for a in res:
-            txrefs = a.get('txrefs', []) + a.get('unconfirmed_txrefs', [])
-            txids = []
-            for t in txrefs[::-1]:
-                if t['tx_hash'] not in txids:
-                    txids.append(t['tx_hash'])
-                if t['tx_hash'] == after_txid:
-                    txids = []
-            if len(txids) > 500:
-                _logger.info("BlockCypher: Large number of transactions for address %s, "
-                             "Transaction list may be incomplete" % address.address_orig)
-            for txid in txids[:limit]:
-                t = self.gettransaction(txid)
+        for tx in prtxs[::-1]:
+            t = self._parse_transaction(tx)
+            if t:
                 txs.append(t)
-        return txs
+            if t.txid == after_txid:
+                txs = []
+            if len(txs) > limit:
+                break
+        return txs[:limit]
 
     def getrawtransaction(self, txid):
-        return self.compose_request('txs', txid, variables={'includeHex': 'true'})['hex']
+        return self.compose_request('tx', txid, 'hex')
 
     def sendrawtransaction(self, rawtx):
-        # BlockCypher sometimes accepts transactions, but does not push them to the network :(
-        if self.network.name in ['bitcoin', 'litecoin']:
-            raise ClientError("Avoid stuck transactions, skip usage of blockcypher provider")
-        res = self.compose_request('txs', 'push', variables={'tx': rawtx}, method='post')
-        return {
-            'txid': res['tx']['hash'],
-            'response_dict': res
-        }
+        return self.compose_request('tx', post_data=rawtx, method='post')
 
     def estimatefee(self, blocks):
-        res = self.compose_request('', '')
-        if blocks <= 10:
-            return res['medium_fee_per_kb']
+        estimates = self.compose_request('v1/fees', 'recommended')
+        if blocks < 2:
+            return estimates['fastestFee'] * 1000
+        elif blocks < 4:
+            return estimates['halfHourFee'] * 1000
+        if blocks < 7:
+            return estimates['hourFee'] * 1000
         else:
-            return res['low_fee_per_kb']
+            return estimates['minimumFee'] * 1000
 
     def blockcount(self):
-        return self.compose_request('', '')['height']
+        res = self.compose_request('blocks', 'tip', 'height')
+        return res
 
-    def mempool(self, txid):
-        if txid:
-            tx = self.compose_request('txs', txid)
-            if tx['confirmations'] == 0:
-                return [tx['hash']]
-            else:
-                return []
-        return False
+    def mempool(self, txid=''):
+        txids = self.compose_request('mempool', 'txids')
+        if not txid:
+            return txids
+        if txid in txids:
+            return [txid]
+        return []
 
     def getblock(self, blockid, parse_transactions, page, limit):
-        if limit > 100:
-            limit = 100
-        bd = self.compose_request('blocks', str(blockid), variables={'limit': limit, 'txstart': ((page-1)*limit)})
+        if isinstance(blockid, int):
+            blockid = self.compose_request('block-height', str(blockid))
+        if (page == 1 and limit == 10) or limit > 25:
+            limit = 25
+        bd = self.compose_request('block', blockid)
+        btxs = self.compose_request('block', blockid, 'txs', str((page-1)*limit))
         if parse_transactions:
             txs = []
-            for txid in bd['txids']:
-                try:
-                    txs.append(self.gettransaction(txid))
-                except Exception as e:
-                    _logger.error("Could not parse tx %s with error %s" % (txid, e))
+            for tx in btxs[:limit]:
+                txs.append(self._parse_transaction(tx))
         else:
-            txs = bd['txids']
+            txs = [tx['txid'] for tx in btxs]
 
         block = {
             'bits': bd['bits'],
-            'depth': bd['depth'],
-            'block_hash': bd['hash'],
+            'depth': None,
+            'block_hash': bd['id'],
             'height': bd['height'],
-            'merkle_root': bd['mrkl_root'],
+            'merkle_root': bd['merkle_root'],
             'nonce': bd['nonce'],
-            'prev_block': bd['prev_block'],
-            'time': int(datetime.strptime(bd['time'], "%Y-%m-%dT%H:%M:%SZ").replace(tzinfo=timezone.utc).timestamp()),
-            'tx_count': bd['n_tx'],
+            'prev_block': bd['previousblockhash'],
+            'time': bd['timestamp'],
+            'tx_count': bd['tx_count'],
             'txs': txs,
-            'version': bd['ver'],
+            'version': bd['version'],
             'page': page,
-            'pages': None if not limit else int(bd['n_tx'] // limit) + (bd['n_tx'] % limit > 0),
+            'pages': None if not limit else int(bd['tx_count'] // limit) + (bd['tx_count'] % limit > 0),
             'limit': limit
         }
         return block
 
-    # def getrawblock(self, blockid):
+    def getrawblock(self, blockid):
+        if isinstance(blockid, int):
+            blockid = self.compose_request('block-height', str(blockid))
+        return self.compose_request('block', blockid, 'raw').hex()
 
     def isspent(self, txid, output_n):
-        t = self.gettransaction(txid)
-        return 1 if t.outputs[output_n].spent else 0
+        res = self.compose_request('tx', txid, 'outspend', str(output_n))
+        return 1 if res['spent'] else 0
 
     # def getinfo(self):
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/blocksmurfer.py` & `bitcoinlib-0.6.9/bitcoinlib/services/blocksmurfer.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/blockstream.py` & `bitcoinlib-0.6.9/bitcoinlib/services/blockstream.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/chainso.py` & `bitcoinlib-0.6.9/bitcoinlib/services/chainso.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/cryptoid.py` & `bitcoinlib-0.6.9/bitcoinlib/services/cryptoid.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/dashd.py` & `bitcoinlib-0.6.9/bitcoinlib/services/dashd.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/dogecoind.py` & `bitcoinlib-0.6.9/bitcoinlib/services/dogecoind.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/insightdash.py` & `bitcoinlib-0.6.9/bitcoinlib/services/insightdash.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/litecoinblockexplorer.py` & `bitcoinlib-0.6.9/bitcoinlib/services/litecoreio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    litecoinblockexplorer.net Client
-#    © 2019-2022 - 1200 Web Development <http://1200wd.com/>
+#    Litecore.io Client
+#    © 2018-2022 - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -14,86 +14,87 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-import logging
 from datetime import datetime
+import logging
 from bitcoinlib.main import MAX_TRANSACTIONS
 from bitcoinlib.services.baseclient import BaseClient
 from bitcoinlib.transactions import Transaction
 
-PROVIDERNAME = 'litecoinblockexplorer'
+PROVIDERNAME = 'litecoreio'
 REQUEST_LIMIT = 50
 
 _logger = logging.getLogger(__name__)
 
 
-class LitecoinBlockexplorerClient(BaseClient):
+class LitecoreIOClient(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
     def compose_request(self, category, data, cmd='', variables=None, method='get', offset=0):
         url_path = category
         if data:
-            url_path += '/' + data + ('' if not cmd else '/' + cmd)
+            url_path += '/' + data + '/' + cmd
         if variables is None:
             variables = {}
         variables.update({'from': offset, 'to': offset+REQUEST_LIMIT})
         return self.request(url_path, variables, method=method)
 
     def _convert_to_transaction(self, tx):
         if tx['confirmations']:
             status = 'confirmed'
         else:
             status = 'unconfirmed'
         fees = None if 'fees' not in tx else int(round(float(tx['fees']) * self.units, 0))
-        value_in = 0 if 'valueIn' not in tx else int(round(float(tx['valueIn']) * self.units, 0))
+        value_in = 0 if 'valueIn' not in tx else tx['valueIn']
         isCoinbase = False
         if 'isCoinBase' in tx and tx['isCoinBase']:
             isCoinbase = True
         txdate = None
         if 'blocktime' in tx:
             txdate = datetime.utcfromtimestamp(tx['blocktime'])
-        t = Transaction(locktime=tx.get('locktime', 0), version=tx['version'], network=self.network, fee=fees,
-                        txid=tx['txid'], date=txdate,
-                        confirmations=tx['confirmations'], block_height=tx['blockheight'], status=status,
+        t = Transaction(locktime=tx['locktime'], version=tx['version'], network=self.network,
+                        fee=fees, size=tx['size'], txid=tx['txid'],
+                        date=txdate, confirmations=tx['confirmations'],
+                        block_height=tx['blockheight'], status=status,
                         input_total=int(round(float(value_in) * self.units, 0)), coinbase=isCoinbase,
-                        output_total=int(round(float(tx['valueOut']) * self.units, 0)), size=len(tx['hex']) // 2)
+                        output_total=int(round(float(tx['valueOut']) * self.units, 0)))
         for ti in tx['vin']:
             if isCoinbase:
                 t.add_input(prev_txid=32 * b'\0', output_n=4*b'\xff', unlocking_script=ti['coinbase'], index_n=ti['n'],
-                            script_type='coinbase', sequence=ti.get('sequence', 0), value=0)
+                            script_type='coinbase', sequence=ti['sequence'], value=0)
             else:
-                value = int(round(float(ti['value'] or 0) * self.units, 0))
-                us = '' if 'hex' not in ti['scriptSig'] else ti['scriptSig']['hex']
-                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'], unlocking_script=us,
-                            index_n=ti['n'], value=value, sequence=ti.get('sequence', 0),
-                            double_spend=ti.get('doubleSpentTxID', False),
-                            strict=self.strict)
+                value = int(round(float(ti['value']) * self.units, 0))
+                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'], unlocking_script=ti['scriptSig']['hex'],
+                            index_n=ti['n'], value=value, sequence=ti['sequence'],
+                            double_spend=False if ti['doubleSpentTxID'] is None else ti['doubleSpentTxID'])
         for to in tx['vout']:
             value = int(round(float(to['value']) * self.units, 0))
-            t.add_output(value=value, lock_script=to['scriptPubKey']['hex'], address=to['scriptPubKey']['addresses'][0],
-                         spent=to['spent'], output_n=to['n'], strict=self.strict)
+            t.add_output(value=value, lock_script=to['scriptPubKey']['hex'],
+                         spent=True if to['spentTxId'] else False, output_n=to['n'],
+                         spending_txid=None if not to['spentTxId'] else to['spentTxId'],
+                         spending_index_n=None if not to['spentIndex'] else to['spentIndex'], strict=self.strict)
         return t
 
     def getbalance(self, addresslist):
         balance = 0
         addresslist = self._addresslist_convert(addresslist)
         for a in addresslist:
-            res = self.compose_request('address', a.address)
-            balance += int(float(res['balance']) / self.network.denominator)
+            res = self.compose_request('addr', a.address, 'balance')
+            balance += res
         return balance
 
     def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
         address = self._address_convert(address)
-        res = self.compose_request('utxo', address.address)
+        res = self.compose_request('addrs', address.address, 'utxo')
         txs = []
         for tx in res:
             if tx['txid'] == after_txid:
                 break
             txs.append({
                 'address': address.address_orig,
                 'txid': tx['txid'],
@@ -105,95 +106,92 @@
                 'size': 0,
                 'value': tx['satoshis'],
                 'script': tx['scriptPubKey'],
                 'date': None
             })
         return txs[::-1][:limit]
 
-    def gettransaction(self, txid):
-        tx = self.compose_request('tx', txid)
+    def gettransaction(self, tx_id):
+        tx = self.compose_request('tx', tx_id)
         return self._convert_to_transaction(tx)
 
-    # FIXME: Not available anymore
-    # def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-    #     address = self._address_convert(address)
-    #     res = self.compose_request('addrs', address.address, 'txs')
-    #     txs = []
-    #     txs_dict = res['items'][::-1]
-    #     if after_txid:
-    #         txs_dict = txs_dict[[t['txid'] for t in txs_dict].index(after_txid) + 1:]
-    #     for tx in txs_dict[:limit]:
-    #         if tx['txid'] == after_txid:
-    #             break
-    #         txs.append(self._convert_to_transaction(tx))
-    #     return txs
+    def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+        address = self._address_convert(address)
+        res = self.compose_request('addrs', address.address, 'txs')
+        txs = []
+        txs_dict = res['items'][::-1]
+        if after_txid:
+            txs_dict = txs_dict[[t['txid'] for t in txs_dict].index(after_txid) + 1:]
+        for tx in txs_dict[:limit]:
+            if tx['txid'] == after_txid:
+                break
+            txs.append(self._convert_to_transaction(tx))
+        return txs
 
-    def getrawtransaction(self, txid):
-        res = self.compose_request('tx', txid)
-        return res['hex']
+    def getrawtransaction(self, tx_id):
+        res = self.compose_request('rawtx', tx_id)
+        return res['rawtx']
 
     def sendrawtransaction(self, rawtx):
-        res = self.compose_request('sendtx', data=rawtx)
+        res = self.compose_request('tx', 'send', variables={'rawtx': rawtx}, method='post')
         return {
-            'txid': res['result'],
+            'txid': res['txid'],
             'response_dict': res
         }
 
-    def estimatefee(self, blocks):
-        res = self.compose_request('estimatefee', str(blocks))
-        return int(float(res['result']) / self.network.denominator)
+    # def estimatefee
 
     def blockcount(self):
         res = self.compose_request('status', '', variables={'q': 'getinfo'})
-        return res['blockbook']['bestHeight']
+        return res['info']['blocks']
 
     def mempool(self, txid):
         res = self.compose_request('tx', txid)
         if res['confirmations'] == 0:
             return res['txid']
         return []
 
     def getblock(self, blockid, parse_transactions, page, limit):
-        bd = self.compose_request('block', str(blockid))
+        if isinstance(blockid, int):
+            blockid = self.compose_request('block-index', str(blockid))['blockHash']
+        bd = self.compose_request('block', blockid)
         if parse_transactions:
             txs = []
-            for tx in bd['txs'][(page-1)*limit:page*limit]:
+            for txid in bd['tx'][(page-1)*limit:page*limit]:
                 # try:
-                txs.append(self.gettransaction(tx['txid']))
+                txs.append(self.gettransaction(txid))
                 # except Exception as e:
-                #     _logger.error("Could not parse tx %s with error %s" % (tx['id'], e))
+                #     _logger.error("Could not parse tx %s with error %s" % (txid, e))
         else:
-            txs = [tx['txid'] for tx in bd['txs']]
+            txs = bd['tx']
 
         block = {
-            'bits': bd['bits'],
+            'bits': int(bd['bits'], 16),
             'depth': bd['confirmations'],
             'block_hash': bd['hash'],
             'height': bd['height'],
-            'merkle_root': bd['merkleRoot'],
+            'merkle_root': bd['merkleroot'],
             'nonce': bd['nonce'],
-            'prev_block': bd['previousBlockHash'],
+            'prev_block': bd['previousblockhash'],
             'time': bd['time'],
-            'tx_count': len(bd['txs']),
+            'tx_count': len(bd['tx']),
             'txs': txs,
             'version': bd['version'],
             'page': page,
-            'pages': None if not limit else int(len(bd['txs']) // limit) + (len(bd['txs']) % limit > 0),
+            'pages': None if not limit else int(len(bd['tx']) // limit) + (len(bd['tx']) % limit > 0),
             'limit': limit
         }
         return block
 
-    # def getrawblock(self, blockid):
-
     def isspent(self, txid, output_n):
         t = self.gettransaction(txid)
         return 1 if t.outputs[output_n].spent else 0
 
     def getinfo(self):
-        info = self.compose_request('status', '')
+        info = self.compose_request('status', '')['info']
         return {
-            'blockcount': info['backend']['blocks'],
-            'chain': info['backend']['chain'],
-            'difficulty': int(float(info['backend']['difficulty'])),
+            'blockcount': info['blocks'],
+            'chain': info['network'],
+            'difficulty': int(float(info['difficulty'])),
             'hashrate': 0,
-            'mempool_size': info['blockbook']['mempoolSize'],
-        }
+            'mempool_size': 0,
+        }
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/litecoind.py` & `bitcoinlib-0.6.9/bitcoinlib/services/litecoind.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/litecoreio.py` & `bitcoinlib-0.6.9/bitcoinlib/services/bitaps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    Litecore.io Client
-#    © 2018-2022 - 1200 Web Development <http://1200wd.com/>
+#    BitAps client
+#    © 2019 August - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -14,184 +14,215 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-from datetime import datetime
 import logging
+from datetime import datetime
 from bitcoinlib.main import MAX_TRANSACTIONS
-from bitcoinlib.services.baseclient import BaseClient
+from bitcoinlib.services.baseclient import BaseClient, ClientError
 from bitcoinlib.transactions import Transaction
 
-PROVIDERNAME = 'litecoreio'
-REQUEST_LIMIT = 50
-
 _logger = logging.getLogger(__name__)
 
+PROVIDERNAME = 'bitaps'
+# Please note: In the Bitaps API, the first couple of Bitcoin blocks are not correctly indexed,
+# so transactions from these blocks are missing.
 
-class LitecoreIOClient(BaseClient):
+
+class BitapsClient(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
-    def compose_request(self, category, data, cmd='', variables=None, method='get', offset=0):
-        url_path = category
+    def compose_request(self, category, command='', data='', variables=None, req_type='blockchain', method='get'):
+        url_path = req_type + '/' + category
+        if command:
+            url_path += '/' + command
         if data:
-            url_path += '/' + data + '/' + cmd
-        if variables is None:
-            variables = {}
-        variables.update({'from': offset, 'to': offset+REQUEST_LIMIT})
-        return self.request(url_path, variables, method=method)
+            if url_path[-1:] != '/':
+                url_path += '/'
+            url_path += data
+        return self.request(url_path, variables=variables, method=method)
 
-    def _convert_to_transaction(self, tx):
+    def _parse_transaction(self, tx):
+        status = 'unconfirmed'
         if tx['confirmations']:
             status = 'confirmed'
-        else:
-            status = 'unconfirmed'
-        fees = None if 'fees' not in tx else int(round(float(tx['fees']) * self.units, 0))
-        value_in = 0 if 'valueIn' not in tx else tx['valueIn']
-        isCoinbase = False
-        if 'isCoinBase' in tx and tx['isCoinBase']:
-            isCoinbase = True
-        txdate = None
-        if 'blocktime' in tx:
-            txdate = datetime.utcfromtimestamp(tx['blocktime'])
-        t = Transaction(locktime=tx['locktime'], version=tx['version'], network=self.network,
-                        fee=fees, size=tx['size'], txid=tx['txid'],
-                        date=txdate, confirmations=tx['confirmations'],
-                        block_height=tx['blockheight'], status=status,
-                        input_total=int(round(float(value_in) * self.units, 0)), coinbase=isCoinbase,
-                        output_total=int(round(float(tx['valueOut']) * self.units, 0)))
-        for ti in tx['vin']:
-            if isCoinbase:
-                t.add_input(prev_txid=32 * b'\0', output_n=4*b'\xff', unlocking_script=ti['coinbase'], index_n=ti['n'],
-                            script_type='coinbase', sequence=ti['sequence'], value=0)
+        date = None
+        if 'timestamp' in tx and tx['timestamp']:
+            date = datetime.utcfromtimestamp(tx['timestamp'])
+        elif 'blockTime' in tx and tx['blockTime']:
+            date = datetime.utcfromtimestamp(tx['blockTime'])
+        block_height = None
+        if 'blockHeight' in tx:
+            block_height = tx['blockHeight']
+        witness_type = 'legacy'
+        if tx['segwit']:
+            witness_type = 'segwit'
+
+        t = Transaction(
+            locktime=tx['lockTime'], version=tx['version'], network=self.network, fee=tx['fee'],
+            fee_per_kb=None if 'feeRate' not in tx else int(tx['feeRate']), size=tx['size'],
+            txid=tx['txId'], date=date, confirmations=tx['confirmations'], block_height=block_height,
+            input_total=tx['inputsAmount'], output_total=tx['outputsAmount'], status=status, coinbase=tx['coinbase'],
+            verified=None if 'valid' not in tx else tx['valid'], witness_type=witness_type)
+
+        for n, ti in tx['vIn'].items():
+            if t.coinbase:
+                t.add_input(prev_txid=ti['txId'], output_n=ti['vOut'], unlocking_script=ti['scriptSig'],
+                            sequence=ti['sequence'], index_n=int(n), value=0)
             else:
-                value = int(round(float(ti['value']) * self.units, 0))
-                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'], unlocking_script=ti['scriptSig']['hex'],
-                            index_n=ti['n'], value=value, sequence=ti['sequence'],
-                            double_spend=False if ti['doubleSpentTxID'] is None else ti['doubleSpentTxID'])
-        for to in tx['vout']:
-            value = int(round(float(to['value']) * self.units, 0))
-            t.add_output(value=value, lock_script=to['scriptPubKey']['hex'],
-                         spent=True if to['spentTxId'] else False, output_n=to['n'],
-                         spending_txid=None if not to['spentTxId'] else to['spentTxId'],
-                         spending_index_n=None if not to['spentIndex'] else to['spentIndex'], strict=self.strict)
+                t.add_input(prev_txid=ti['txId'], output_n=ti['vOut'], unlocking_script=ti['scriptSig'],
+                            unlocking_script_unsigned=ti['scriptPubKey'], witnesses=ti.get('txInWitness', []),
+                            address='' if 'address' not in ti else ti['address'], sequence=ti['sequence'],
+                            index_n=int(n), value=ti['amount'], strict=self.strict)
+
+        for _, to in tx['vOut'].items():
+            spending_txid = None if not to['spent'] else to['spent'][0]['txId']
+            spending_index_n = None if not to['spent'] else to['spent'][0]['vIn']
+            t.add_output(to['value'], '' if 'address' not in to else to['address'],
+                         '' if 'addressHash' not in to else to['addressHash'], lock_script=to['scriptPubKey'],
+                         spent=bool(to['spent']), spending_txid=spending_txid, spending_index_n=spending_index_n,
+                         strict=self.strict)
+
         return t
 
     def getbalance(self, addresslist):
         balance = 0
-        addresslist = self._addresslist_convert(addresslist)
-        for a in addresslist:
-            res = self.compose_request('addr', a.address, 'balance')
-            balance += res
+        for address in addresslist:
+            res = self.compose_request('address', 'state', address)
+            balance += res['data']['balance']
         return balance
 
     def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-        address = self._address_convert(address)
-        res = self.compose_request('addrs', address.address, 'utxo')
-        txs = []
-        for tx in res:
-            if tx['txid'] == after_txid:
+        utxos = []
+        page = 1
+        while True:
+            variables = {'mode': 'verbose', 'limit': 50, 'page': page, 'order': 'asc'}
+            try:
+                res = self.compose_request('address', 'transactions', address, variables)
+                res2 = self.compose_request('address', 'unconfirmed/transactions', address, variables)
+            except ClientError as e:
+                if "address not found" in self.resp.text:
+                    return []
+                else:
+                    raise ClientError(e.msg)
+            txs = res['data']['list']
+            txs += res2['data']['list']
+            for tx in txs:
+                for outp in tx['vOut']:
+                    utxo = tx['vOut'][outp]
+                    if 'address' not in utxo or utxo['address'] != address or utxo['spent']:
+                        continue
+                    utxos.append(
+                        {
+                            'address': utxo['address'],
+                            'txid': tx['txId'],
+                            'confirmations': 0 if 'confirmations' not in tx else tx['confirmations'],
+                            'output_n': int(outp),
+                            'input_n': 0,
+                            'block_height': None if 'blockHeight' not in tx else tx['blockHeight'],
+                            'fee': None,
+                            'size': 0,
+                            'value': utxo['value'],
+                            'script': utxo['scriptPubKey'],
+                            'date': datetime.utcfromtimestamp(tx['timestamp'])
+                         }
+                    )
+                if tx['txId'] == after_txid:
+                    utxos = []
+            page += 1
+            if page > res['data']['pages']:
                 break
-            txs.append({
-                'address': address.address_orig,
-                'txid': tx['txid'],
-                'confirmations': tx['confirmations'],
-                'output_n': tx['vout'],
-                'input_n': 0,
-                'block_height': tx['height'],
-                'fee': None,
-                'size': 0,
-                'value': tx['satoshis'],
-                'script': tx['scriptPubKey'],
-                'date': None
-            })
-        return txs[::-1][:limit]
-
-    def gettransaction(self, tx_id):
-        tx = self.compose_request('tx', tx_id)
-        return self._convert_to_transaction(tx)
+        return utxos[:limit]
+
+    def gettransaction(self, txid):
+        res = self.compose_request('transaction', txid)
+        return self._parse_transaction(res['data'])
 
     def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-        address = self._address_convert(address)
-        res = self.compose_request('addrs', address.address, 'txs')
+        page = 0
         txs = []
-        txs_dict = res['items'][::-1]
-        if after_txid:
-            txs_dict = txs_dict[[t['txid'] for t in txs_dict].index(after_txid) + 1:]
-        for tx in txs_dict[:limit]:
-            if tx['txid'] == after_txid:
+        while True:
+            variables = {'mode': 'verbose', 'limit': MAX_TRANSACTIONS, 'page': page, 'order': 'asc'}
+            try:
+                res = self.compose_request('address', 'transactions', address, variables)
+            except ClientError:
+                if "address not found" in self.resp.text:
+                    return []
+            for tx in res['data']['list']:
+                txs.append(self._parse_transaction(tx))
+                if tx['txId'] == after_txid:
+                    txs = []
+            if len(txs) > limit:
+                break
+            page += 1
+            if page >= res['data']['pages']:
                 break
-            txs.append(self._convert_to_transaction(tx))
-        return txs
+        return txs[:limit]
 
-    def getrawtransaction(self, tx_id):
-        res = self.compose_request('rawtx', tx_id)
-        return res['rawtx']
-
-    def sendrawtransaction(self, rawtx):
-        res = self.compose_request('tx', 'send', variables={'rawtx': rawtx}, method='post')
-        return {
-            'txid': res['txid'],
-            'response_dict': res
-        }
+    # def getrawtransaction(self, txid):
+    #     tx = self.compose_request('transaction', txid)
+    #     return tx['data']['rawTx']
+
+    # def sendrawtransaction
 
     # def estimatefee
 
     def blockcount(self):
-        res = self.compose_request('status', '', variables={'q': 'getinfo'})
-        return res['info']['blocks']
+        return self.compose_request('block', 'last')['data']['height']
+
+    # def mempool(self, txid):
+    #     if txid:
+    #         t = self.gettransaction(txid)
+    #         if t and not t.confirmations:
+    #             return [t.txid]
+    #     else:
+    #         res = self.compose_request('transactions', type='mempool')
+    #         return [tx['hash'] for tx in res['data']['transactions']]
+    #     return []
+
+    # FIXME: Bitaps doesn't seem to return block data anymore...
+    # def getblock(self, blockid, parse_transactions, page, limit):
+    #     if limit > 100:
+    #         limit = 100
+    #     res = self.compose_request('block', str(blockid),
+    #                                variables={'transactions': True, 'limit': limit, 'page': page})
+    #     bd = res['data']['block']
+    #     td = res['data']['transactions']
+    #     txids = [tx['txId'] for tx in td['list']]
+    #     if parse_transactions:
+    #         txs = []
+    #         for txid in txids:
+    #             try:
+    #                 txs.append(self.gettransaction(txid))
+    #             except Exception as e:
+    #                 _logger.error("Could not parse tx %s with error %s" % (txid, e))
+    #     else:
+    #         txs = txids
+    #
+    #     block = {
+    #         'bits': bd['bits'],
+    #         'depth': bd['confirmations'],
+    #         'hash': bd['hash'],
+    #         'height': bd['height'],
+    #         'merkle_root': bd['merkleRoot'],
+    #         'nonce': bd['nonce'],
+    #         'prev_block': bd['previousBlockHash'],
+    #         'time': datetime.utcfromtimestamp(bd['blockTime']),
+    #         'total_txs': bd['transactionsCount'],
+    #         'txs': txs,
+    #         'version': bd['version'],
+    #         'page': td['page'],
+    #         'pages': td['pages'],
+    #         'limit': td['limit']
+    #     }
+    #     return block
+
+    # def isspent(self, txid, output_n):
+    #     t = self.gettransaction(txid)
+    #     return 1 if t.outputs[output_n].spent else 0
 
-    def mempool(self, txid):
-        res = self.compose_request('tx', txid)
-        if res['confirmations'] == 0:
-            return res['txid']
-        return []
-
-    def getblock(self, blockid, parse_transactions, page, limit):
-        if isinstance(blockid, int):
-            blockid = self.compose_request('block-index', str(blockid))['blockHash']
-        bd = self.compose_request('block', blockid)
-        if parse_transactions:
-            txs = []
-            for txid in bd['tx'][(page-1)*limit:page*limit]:
-                # try:
-                txs.append(self.gettransaction(txid))
-                # except Exception as e:
-                #     _logger.error("Could not parse tx %s with error %s" % (txid, e))
-        else:
-            txs = bd['tx']
-
-        block = {
-            'bits': int(bd['bits'], 16),
-            'depth': bd['confirmations'],
-            'block_hash': bd['hash'],
-            'height': bd['height'],
-            'merkle_root': bd['merkleroot'],
-            'nonce': bd['nonce'],
-            'prev_block': bd['previousblockhash'],
-            'time': bd['time'],
-            'tx_count': len(bd['tx']),
-            'txs': txs,
-            'version': bd['version'],
-            'page': page,
-            'pages': None if not limit else int(len(bd['tx']) // limit) + (len(bd['tx']) % limit > 0),
-            'limit': limit
-        }
-        return block
-
-    def isspent(self, txid, output_n):
-        t = self.gettransaction(txid)
-        return 1 if t.outputs[output_n].spent else 0
-
-    def getinfo(self):
-        info = self.compose_request('status', '')['info']
-        return {
-            'blockcount': info['blocks'],
-            'chain': info['network'],
-            'difficulty': int(float(info['difficulty'])),
-            'hashrate': 0,
-            'mempool_size': 0,
-        }
+    # def getinfo(self):
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/mempool.py` & `bitcoinlib-0.6.9/bitcoinlib/services/litecoinblockexplorer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 #    BitcoinLib - Python Cryptocurrency Library
-#    mempool.space client
-#    © 2021-2022 - 1200 Web Development <http://1200wd.com/>
+#    litecoinblockexplorer.net Client
+#    © 2019-2022 - 1200 Web Development <http://1200wd.com/>
 #
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU Affero General Public License as
 #    published by the Free Software Foundation, either version 3 of the
 #    License, or (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -17,206 +17,174 @@
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import logging
 from datetime import datetime
 from bitcoinlib.main import MAX_TRANSACTIONS
-from bitcoinlib.services.baseclient import BaseClient, ClientError
+from bitcoinlib.services.baseclient import BaseClient
 from bitcoinlib.transactions import Transaction
-from bitcoinlib.encoding import varstr
 
-PROVIDERNAME = 'mempool'
-# Please note: In the Blockstream API, the first couple of Bitcoin blocks are not correctly indexed,
-# so transactions from these blocks are missing.
+PROVIDERNAME = 'litecoinblockexplorer'
+REQUEST_LIMIT = 50
 
 _logger = logging.getLogger(__name__)
 
 
-class MempoolClient(BaseClient):
+class LitecoinBlockexplorerClient(BaseClient):
 
     def __init__(self, network, base_url, denominator, *args):
         super(self.__class__, self).__init__(network, PROVIDERNAME, base_url, denominator, *args)
 
-    def compose_request(self, function, data='', parameter='', parameter2='', variables=None, post_data='',
-                        method='get'):
-        url_path = function
+    def compose_request(self, category, data, cmd='', variables=None, method='get', offset=0):
+        url_path = category
         if data:
-            url_path += '/' + data
-        if parameter:
-            url_path += '/' + parameter
-        if parameter2:
-            url_path += '/' + parameter2
+            url_path += '/' + data + ('' if not cmd else '/' + cmd)
         if variables is None:
             variables = {}
-        if self.api_key:
-            variables.update({'token': self.api_key})
-        return self.request(url_path, variables, method, post_data=post_data)
+        variables.update({'from': offset, 'to': offset+REQUEST_LIMIT})
+        return self.request(url_path, variables, method=method)
+
+    def _convert_to_transaction(self, tx):
+        if tx['confirmations']:
+            status = 'confirmed'
+        else:
+            status = 'unconfirmed'
+        fees = None if 'fees' not in tx else int(round(float(tx['fees']) * self.units, 0))
+        value_in = 0 if 'valueIn' not in tx else int(round(float(tx['valueIn']) * self.units, 0))
+        txdate = None
+        if 'blocktime' in tx:
+            txdate = datetime.utcfromtimestamp(tx['blocktime'])
+        t = Transaction.parse_hex(tx['hex'], strict=self.strict, network=self.network)
+        t.fee = fees
+        t.input_total = value_in
+        t.output_total = int(round(float(tx['valueOut']) * self.units, 0))
+        t.fees = int(round(float(tx['fees']) * self.units, 0))
+        t.date = txdate
+        t.confirmations = tx['confirmations']
+        t.block_height = tx['blockheight']
+        if t.confirmations == 0:
+            t.block_height = None
+            t.date = None
+        t.block_hash = tx.get('blockhash', '')
+        t.status = status
+        for n, ti in enumerate(tx['vin']):
+            t.inputs[n].value = int(round(float(ti['value'] or 0) * self.units, 0))
+        for i, to in enumerate(tx['vout']):
+            t.outputs[i].spent = to['spent']
+        return t
 
     def getbalance(self, addresslist):
         balance = 0
-        for address in addresslist:
-            res = self.compose_request('address', address)
-            balance += res['chain_stats']['funded_txo_sum'] - res['chain_stats']['spent_txo_sum']
+        addresslist = self._addresslist_convert(addresslist)
+        for a in addresslist:
+            res = self.compose_request('address', a.address)
+            balance += int(float(res['balance']) / self.network.denominator)
         return balance
 
     def getutxos(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-        self.latest_block = self.blockcount() if not self.latest_block else self.latest_block
-        res = self.compose_request('address', address, 'utxo')
-        utxos = []
-        # # key=lambda k: (k[2], pow(10, 20)-k[0].transaction_id, k[3]), reverse=True
-        res = sorted(res, key=lambda k: 0 if 'block_height' not in k['status'] else k['status']['block_height'])
-        for a in res:
-            confirmations = 0
-            block_height = None
-            if 'block_height' in a['status']:
-                block_height = a['status']['block_height']
-                confirmations = self.latest_block - block_height
-            utxos.append({
-                'address': address,
-                'txid': a['txid'],
-                'confirmations': confirmations,
-                'output_n': a['vout'],
+        address = self._address_convert(address)
+        res = self.compose_request('utxo', address.address)
+        txs = []
+        for tx in res:
+            if tx['txid'] == after_txid:
+                break
+            txs.append({
+                'address': address.address_orig,
+                'txid': tx['txid'],
+                'confirmations': tx['confirmations'],
+                'output_n': tx['vout'],
                 'input_n': 0,
-                'block_height': block_height,
+                'block_height': tx['height'],
                 'fee': None,
                 'size': 0,
-                'value': a['value'],
-                'script': '',
-                'date': None if 'block_time' not in a['status'] else datetime.utcfromtimestamp(a['status']['block_time'])
+                'value': tx['satoshis'],
+                'script': tx.get('scriptPubKey', ''),
+                'date': None
             })
-            if a['txid'] == after_txid:
-                utxos = []
-        return utxos[:limit]
-
-    def _parse_transaction(self, tx):
-        block_height = None if 'block_height' not in tx['status'] else tx['status']['block_height']
-        confirmations = 0
-        tx_date = None
-        status = 'unconfirmed'
-        if tx['status']['confirmed']:
-            if block_height:
-                self.latest_block = self.blockcount() if not self.latest_block else self.latest_block
-                confirmations = self.latest_block - block_height + 1
-            tx_date = datetime.utcfromtimestamp(tx['status']['block_time'])
-            status = 'confirmed'
-
-        t = Transaction(locktime=tx['locktime'], version=tx['version'], network=self.network, block_height=block_height,
-                        fee=tx['fee'], size=tx['size'], txid=tx['txid'], date=tx_date, confirmations=confirmations,
-                        status=status, coinbase=tx['vin'][0]['is_coinbase'])
-        for ti in tx['vin']:
-            if ti['is_coinbase']:
-                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'], unlocking_script=ti['scriptsig'], value=0,
-                            sequence=ti['sequence'], strict=self.strict)
-            else:
-                t.add_input(prev_txid=ti['txid'], output_n=ti['vout'],
-                            unlocking_script=ti['scriptsig'], value=ti['prevout']['value'],
-                            address=ti['prevout'].get('scriptpubkey_address', ''),
-                            unlocking_script_unsigned=ti['prevout']['scriptpubkey'], sequence=ti['sequence'],
-                            witnesses=None if 'witness' not in ti else [bytes.fromhex(w) for w in ti['witness']],
-                            strict=self.strict)
-        for to in tx['vout']:
-            t.add_output(value=to['value'], address=to.get('scriptpubkey_address', ''), spent=None,
-                         lock_script=to['scriptpubkey'], strict=self.strict)
-        if 'segwit' in [i.witness_type for i in t.inputs] or 'p2sh-segwit' in [i.witness_type for i in t.inputs]:
-            t.witness_type = 'segwit'
-        t.update_totals()
-        return t
+        return txs[::-1][:limit]
 
     def gettransaction(self, txid):
         tx = self.compose_request('tx', txid)
-        return self._parse_transaction(tx)
+        return self._convert_to_transaction(tx)
 
-    def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
-        prtxs = []
-        before_txid = ''
-        while True:
-            txs = self.compose_request('address', address, 'txs/chain', before_txid)
-            prtxs += txs
-            if len(txs) == 25:
-                before_txid = txs[-1:][0]['txid']
-            else:
-                break
-            if len(prtxs) > limit:
-                break
-        txs = []
-        for tx in prtxs[::-1]:
-            t = self._parse_transaction(tx)
-            if t:
-                txs.append(t)
-            if t.txid == after_txid:
-                txs = []
-            if len(txs) > limit:
-                break
-        return txs[:limit]
+    # FIXME: Not available anymore
+    # def gettransactions(self, address, after_txid='', limit=MAX_TRANSACTIONS):
+    #     address = self._address_convert(address)
+    #     res = self.compose_request('addrs', address.address, 'txs')
+    #     txs = []
+    #     txs_dict = res['items'][::-1]
+    #     if after_txid:
+    #         txs_dict = txs_dict[[t['txid'] for t in txs_dict].index(after_txid) + 1:]
+    #     for tx in txs_dict[:limit]:
+    #         if tx['txid'] == after_txid:
+    #             break
+    #         txs.append(self._convert_to_transaction(tx))
+    #     return txs
 
     def getrawtransaction(self, txid):
-        return self.compose_request('tx', txid, 'hex')
+        res = self.compose_request('tx', txid)
+        return res['hex']
 
     def sendrawtransaction(self, rawtx):
-        return self.compose_request('tx', post_data=rawtx, method='post')
+        res = self.compose_request('sendtx', data=rawtx)
+        return {
+            'txid': res['result'],
+            'response_dict': res
+        }
 
     def estimatefee(self, blocks):
-        estimates = self.compose_request('v1/fees', 'recommended')
-        if blocks < 2:
-            return estimates['fastestFee'] * 1000
-        elif blocks < 4:
-            return estimates['halfHourFee'] * 1000
-        if blocks < 7:
-            return estimates['hourFee'] * 1000
-        else:
-            return estimates['minimumFee'] * 1000
+        res = self.compose_request('estimatefee', str(int(blocks)+1))
+        return int(float(res['result']) / self.network.denominator)
 
     def blockcount(self):
-        res = self.compose_request('blocks', 'tip', 'height')
-        return res
+        res = self.compose_request('status', '', variables={'q': 'getinfo'})
+        return res['blockbook']['bestHeight']
 
-    def mempool(self, txid=''):
-        txids = self.compose_request('mempool', 'txids')
-        if not txid:
-            return txids
-        if txid in txids:
-            return [txid]
+    def mempool(self, txid):
+        res = self.compose_request('tx', txid)
+        if res['confirmations'] == 0:
+            return res['txid']
         return []
 
     def getblock(self, blockid, parse_transactions, page, limit):
-        if isinstance(blockid, int):
-            blockid = self.compose_request('block-height', str(blockid))
-        if (page == 1 and limit == 10) or limit > 25:
-            limit = 25
-        bd = self.compose_request('block', blockid)
-        btxs = self.compose_request('block', blockid, 'txs', str((page-1)*limit))
+        bd = self.compose_request('block', str(blockid))
         if parse_transactions:
             txs = []
-            for tx in btxs[:limit]:
-                txs.append(self._parse_transaction(tx))
+            for tx in bd['txs'][(page-1)*limit:page*limit]:
+                txs.append(self.gettransaction(tx['txid']))
         else:
-            txs = [tx['txid'] for tx in btxs]
+            txs = [tx['txid'] for tx in bd['txs']]
 
         block = {
-            'bits': bd['bits'],
-            'depth': None,
-            'block_hash': bd['id'],
+            'bits': int(bd['bits'], 16),
+            'depth': bd['confirmations'],
+            'block_hash': bd['hash'],
             'height': bd['height'],
-            'merkle_root': bd['merkle_root'],
-            'nonce': bd['nonce'],
-            'prev_block': bd['previousblockhash'],
-            'time': bd['timestamp'],
-            'tx_count': bd['tx_count'],
+            'merkle_root': bd['merkleRoot'],
+            'nonce': int(bd['nonce']),
+            'prev_block': bd['previousBlockHash'],
+            'time': bd['time'],
+            'tx_count': bd['txCount'],
             'txs': txs,
             'version': bd['version'],
             'page': page,
-            'pages': None if not limit else int(bd['tx_count'] // limit) + (bd['tx_count'] % limit > 0),
+            'pages': None if not limit else int(len(bd['txs']) // limit) + (len(bd['txs']) % limit > 0),
             'limit': limit
         }
         return block
 
-    def getrawblock(self, blockid):
-        if isinstance(blockid, int):
-            blockid = self.compose_request('block-height', str(blockid))
-        return self.compose_request('block', blockid, 'raw').hex()
+    # def getrawblock(self, blockid):
 
     def isspent(self, txid, output_n):
-        res = self.compose_request('tx', txid, 'outspend', str(output_n))
-        return 1 if res['spent'] else 0
+        t = self.gettransaction(txid)
+        return 1 if t.outputs[output_n].spent else 0
 
-    # def getinfo(self):
+    def getinfo(self):
+        info = self.compose_request('status', '')
+        return {
+            'blockcount': info['backend']['blocks'],
+            'chain': info['backend']['chain'],
+            'difficulty': int(float(info['backend']['difficulty'])),
+            'hashrate': 0,
+            'mempool_size': info['blockbook']['mempoolSize'],
+        }
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/services/services.py` & `bitcoinlib-0.6.9/bitcoinlib/services/services.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/tools/__init__.py` & `bitcoinlib-0.6.9/bitcoinlib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/tools/clw.py` & `bitcoinlib-0.6.9/bitcoinlib/tools/clw.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/tools/mnemonic_key_create.py` & `bitcoinlib-0.6.9/bitcoinlib/tools/mnemonic_key_create.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/tools/sign_raw.py` & `bitcoinlib-0.6.9/bitcoinlib/tools/sign_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # w.get_key()
 # w.utxos_update()
 # w.info()
 # t = w.sweep(w.new_key().address, 10000, fee=1000)
 # raw_tx = t.raw_hex()
 # t.info()
 
-# Raw partially signed transaction transaction
+# Raw partially signed transaction
 raw_tx = ''
 if not raw_tx:
     raw_tx = input("Paste raw transaction hex: ")
 
 t = Transaction.import_raw(raw_tx)
 
 key_str = input("Enter private key or mnemonic passphrase: ")
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/tools/wallet_multisig_2of3.py` & `bitcoinlib-0.6.9/bitcoinlib/tools/wallet_multisig_2of3.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/transactions.py` & `bitcoinlib-0.6.9/bitcoinlib/transactions.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/values.py` & `bitcoinlib-0.6.9/bitcoinlib/values.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wallets.py` & `bitcoinlib-0.6.9/bitcoinlib/wallets.py`

 * *Files 0% similar despite different names*

```diff
@@ -2560,17 +2560,17 @@
         :param network: Network name. Leave empty for default network
         :type network: str
 
         :return int: Total balance
         """
 
         network, account_id, acckey = self._get_account_defaults(network, account_id)
-        balance = Service(network=network, providers=self.providers, cache_uri=self.db_cache_uri).\
-            getbalance(self.addresslist(account_id=account_id, network=network))
-        if balance:
+        srv = Service(network=network, providers=self.providers, cache_uri=self.db_cache_uri)
+        balance = srv.getbalance(self.addresslist(account_id=account_id, network=network))
+        if srv.results:
             new_balance = {
                 'account_id': account_id,
                 'network': network,
                 'balance': balance
             }
             old_balance_item = [bi for bi in self._balances if bi['network'] == network and
                                 bi['account_id'] == account_id]
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/chinese_simplified.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/chinese_traditional.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/dutch.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/dutch.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/english.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/french.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/italian.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/japanese.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib/wordlist/spanish.txt` & `bitcoinlib-0.6.9/bitcoinlib/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/bitcoinlib.egg-info/PKG-INFO` & `bitcoinlib-0.6.9/bitcoinlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bitcoinlib
-Version: 0.6.7
+Version: 0.6.9
 Summary: Bitcoin and Other cryptocurrency Library
 Home-page: http://github.com/1200wd/bitcoinlib
 Author: 1200wd
 Author-email: info@1200wd.com
 License: GNU3
 Description: Python Bitcoin Library
         ======================
```

### Comparing `bitcoinlib-0.6.7/bitcoinlib.egg-info/SOURCES.txt` & `bitcoinlib-0.6.9/bitcoinlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 bitcoinlib/services/baseclient.py
 bitcoinlib/services/bcoin.py
 bitcoinlib/services/bitaps.py
 bitcoinlib/services/bitcoind.py
 bitcoinlib/services/bitcoinlibtest.py
 bitcoinlib/services/bitflyer.py
 bitcoinlib/services/bitgo.py
+bitcoinlib/services/blockbook.py
 bitcoinlib/services/blockchaininfo.py
 bitcoinlib/services/blockchair.py
 bitcoinlib/services/blockcypher.py
 bitcoinlib/services/blocksmurfer.py
 bitcoinlib/services/blockstream.py
 bitcoinlib/services/chainso.py
 bitcoinlib/services/cryptoid.py
```

### Comparing `bitcoinlib-0.6.7/setup.py` & `bitcoinlib-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from setuptools import setup
 from codecs import open
 import os
 import sys
 
 here = os.path.abspath(os.path.dirname(__file__))
-version = '0.6.7'
+version = '0.6.9'
 
 # Get the long description from the relevant file
 readmetxt = ''
 try:
       with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
           readmetxt = f.read()
 except:
```

### Comparing `bitcoinlib-0.6.7/tests/__init__.py` & `bitcoinlib-0.6.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/benchmark.py` & `bitcoinlib-0.6.9/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/bip38_protected_key_tests.json` & `bitcoinlib-0.6.9/tests/bip38_protected_key_tests.json`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/block250000.pickle` & `bitcoinlib-0.6.9/tests/block250000.pickle`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/block330000.pickle` & `bitcoinlib-0.6.9/tests/block330000.pickle`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/block625007.pickle` & `bitcoinlib-0.6.9/tests/block625007.pickle`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/block629999.pickle` & `bitcoinlib-0.6.9/tests/block629999.pickle`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/block722010.pickle` & `bitcoinlib-0.6.9/tests/block722010.pickle`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/db_0_5.py` & `bitcoinlib-0.6.9/tests/db_0_5.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/electrum_keys.json` & `bitcoinlib-0.6.9/tests/electrum_keys.json`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/mnemonics_tests.json` & `bitcoinlib-0.6.9/tests/mnemonics_tests.json`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_blocks.py` & `bitcoinlib-0.6.9/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_custom.py` & `bitcoinlib-0.6.9/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_db.py` & `bitcoinlib-0.6.9/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_encoding.py` & `bitcoinlib-0.6.9/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_keys.py` & `bitcoinlib-0.6.9/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_mnemonic.py` & `bitcoinlib-0.6.9/tests/test_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_networks.py` & `bitcoinlib-0.6.9/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_script.py` & `bitcoinlib-0.6.9/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_services.py` & `bitcoinlib-0.6.9/tests/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,52 +426,53 @@
 
         for provider in srv.results:
             print("Comparing provider %s" % provider)
             self.assertTrue(srv.results[provider].verify())
             self.assertDictEqualExt(srv.results[provider].as_dict(), expected_dict,
                                     ['block_hash', 'block_height', 'spent', 'value'])
 
-    def test_service_gettransaction_dash(self):
-        expected_dict = {'block_hash': '000000000000002eddff510f4f6c61243e350102c58bdf8c986430b405ce7a22',
-                         'network': 'dash', 'input_total': 2575500000, 'fee_per_kb': None, 'outputs': [
-                {'public_key_hash': 'de4b569d39f05bfc43f56a1b22d7783a7d0661d4', 'output_n': 0, 'spent': True,
-                 'public_key': '', 'address': 'XvxE6SRkZMbhBW34QfrgxPqcNmgTsRvyeJ', 'script_type': 'p2pkh',
-                 'script': '76a914de4b569d39f05bfc43f56a1b22d7783a7d0661d488ac', 'value': 2500000000},
-                {'public_key_hash': '1495ac5ca428a17197c7cb5065614d8eabfcf8cb', 'output_n': 1, 'spent': True,
-                 'public_key': '', 'address': 'XcZgeaA4cwUqBqtKUPfZHUme8a5G3gA8LC', 'script_type': 'p2pkh',
-                 'script': '76a9141495ac5ca428a17197c7cb5065614d8eabfcf8cb88ac', 'value': 75300000}],
-                         'output_total': 2575300000, 'block_height': 900147, 'locktime': 0, 'flag': None,
-                         'coinbase': False,
-                         'status': 'confirmed', 'version': 1,
-                         'hash': '885042c885dc0d44167ce71ce82bb28b09bdd8445b7639ea96a5f5be8ceba4cf', 'size': 226,
-                         'fee': 200000, 'inputs': [
-                {'redeemscript': '', 'address': 'XczHdW9k4Kg9mu6AdJayJ1PJtfX3Z9wYxm', 'double_spend': False,
-                 'sequence': 4294967295,
-                 'prev_txid': 'b37c4f45295d9c5382800b6bb2289cedf3e63bd0621d0644083510cd24cdfbed', 'output_n': 1,
-                 'signatures': [
-                     'e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b62f1cc0f33d036c1c60a7d561de0'
-                     '6067528fffca52292d803b75e53f7dfbf63d',
-                     'e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b62f1cc0f33d036c1c60a7d561de0'
-                     '6067528fffca52292d803b75e53f7dfbf63d'],
-                 'public_key': '028bd465d7eb03bbee946c3a277ad1b331f78add78c6723eed00097520edc21ed2', 'index_n': 0,
-                 'script_type': 'sig_pubkey',
-                 'script': '483045022100e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b022062f1cc'
-                           '0f33d036c1c60a7d561de06067528fffca52292d803b75e53f7dfbf63d0121028bd465d7eb03bbee946c3a'
-                           '277ad1b331f78add78c6723eed00097520edc21ed2',
-                 'value': 2575500000}], 'date': datetime(2018, 7, 8, 21, 35, 58)}
-
-        srv = ServiceTest(network='dash', min_providers=3)
-
-        # Get transactions by hash
-        srv.gettransaction('885042c885dc0d44167ce71ce82bb28b09bdd8445b7639ea96a5f5be8ceba4cf')
-        for provider in srv.results:
-            print("Comparing provider %s" % provider)
-            self.assertTrue(srv.results[provider].verify())
-            self.assertDictEqualExt(srv.results[provider].as_dict(), expected_dict,
-                                    ['block_hash', 'block_height', 'spent', 'value'])
+    # FIXME: Disabled, not enough working providers
+    # def test_service_gettransaction_dash(self):
+    #     expected_dict = {'block_hash': '000000000000002eddff510f4f6c61243e350102c58bdf8c986430b405ce7a22',
+    #                      'network': 'dash', 'input_total': 2575500000, 'fee_per_kb': None, 'outputs': [
+    #             {'public_key_hash': 'de4b569d39f05bfc43f56a1b22d7783a7d0661d4', 'output_n': 0, 'spent': True,
+    #              'public_key': '', 'address': 'XvxE6SRkZMbhBW34QfrgxPqcNmgTsRvyeJ', 'script_type': 'p2pkh',
+    #              'script': '76a914de4b569d39f05bfc43f56a1b22d7783a7d0661d488ac', 'value': 2500000000},
+    #             {'public_key_hash': '1495ac5ca428a17197c7cb5065614d8eabfcf8cb', 'output_n': 1, 'spent': True,
+    #              'public_key': '', 'address': 'XcZgeaA4cwUqBqtKUPfZHUme8a5G3gA8LC', 'script_type': 'p2pkh',
+    #              'script': '76a9141495ac5ca428a17197c7cb5065614d8eabfcf8cb88ac', 'value': 75300000}],
+    #                      'output_total': 2575300000, 'block_height': 900147, 'locktime': 0, 'flag': None,
+    #                      'coinbase': False,
+    #                      'status': 'confirmed', 'version': 1,
+    #                      'hash': '885042c885dc0d44167ce71ce82bb28b09bdd8445b7639ea96a5f5be8ceba4cf', 'size': 226,
+    #                      'fee': 200000, 'inputs': [
+    #             {'redeemscript': '', 'address': 'XczHdW9k4Kg9mu6AdJayJ1PJtfX3Z9wYxm', 'double_spend': False,
+    #              'sequence': 4294967295,
+    #              'prev_txid': 'b37c4f45295d9c5382800b6bb2289cedf3e63bd0621d0644083510cd24cdfbed', 'output_n': 1,
+    #              'signatures': [
+    #                  'e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b62f1cc0f33d036c1c60a7d561de0'
+    #                  '6067528fffca52292d803b75e53f7dfbf63d',
+    #                  'e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b62f1cc0f33d036c1c60a7d561de0'
+    #                  '6067528fffca52292d803b75e53f7dfbf63d'],
+    #              'public_key': '028bd465d7eb03bbee946c3a277ad1b331f78add78c6723eed00097520edc21ed2', 'index_n': 0,
+    #              'script_type': 'sig_pubkey',
+    #              'script': '483045022100e87b6a6dff07d1b91d12f530992cf8fa9f26a541af525337bbbc5c954cbf072b022062f1cc'
+    #                        '0f33d036c1c60a7d561de06067528fffca52292d803b75e53f7dfbf63d0121028bd465d7eb03bbee946c3a'
+    #                        '277ad1b331f78add78c6723eed00097520edc21ed2',
+    #              'value': 2575500000}], 'date': datetime(2018, 7, 8, 21, 35, 58)}
+    #
+    #     srv = ServiceTest(network='dash', min_providers=3)
+    #
+    #     # Get transactions by hash
+    #     srv.gettransaction('885042c885dc0d44167ce71ce82bb28b09bdd8445b7639ea96a5f5be8ceba4cf')
+    #     for provider in srv.results:
+    #         print("Comparing provider %s" % provider)
+    #         self.assertTrue(srv.results[provider].verify())
+    #         self.assertDictEqualExt(srv.results[provider].as_dict(), expected_dict,
+    #                                 ['block_hash', 'block_height', 'spent', 'value'])
 
     def test_service_gettransactions_litecoin(self):
         txid = '832518d58e9678bcdb9fe0e417a138daeb880c3a2ee1fb1659f1179efc383c25'
         address = 'Lct7CEpiN7e72rUXmYucuhqnCy5F5Vc6Vg'
         block_height = 400003
         input_total = 122349237
         output_total = 122349237
@@ -667,22 +668,23 @@
         n_blocks = None
         for provider in srv.results:
             if n_blocks is not None:
                 self.assertAlmostEqual(srv.results[provider], n_blocks, delta=5000,
                                        msg="Provider %s value %d != %d" % (provider, srv.results[provider], n_blocks))
             n_blocks = srv.results[provider]
 
-        # Test Dash network
-        srv = ServiceTest(min_providers=3, network='dash')
-        n_blocks = None
-        for provider in srv.results:
-            if n_blocks is not None:
-                self.assertAlmostEqual(srv.results[provider], n_blocks, delta=5000,
-                                       msg="Provider %s value %d != %d" % (provider, srv.results[provider], n_blocks))
-            n_blocks = srv.results[provider]
+        # FIXME: Disabled, not enough working providers
+        # # Test Dash network
+        # srv = ServiceTest(min_providers=3, network='dash')
+        # n_blocks = None
+        # for provider in srv.results:
+        #     if n_blocks is not None:
+        #         self.assertAlmostEqual(srv.results[provider], n_blocks, delta=5000,
+        #                                msg="Provider %s value %d != %d" % (provider, srv.results[provider], n_blocks))
+        #     n_blocks = srv.results[provider]
 
     def test_service_max_providers(self):
         srv = ServiceTest(max_providers=1, cache_uri='')
         srv._blockcount = None
         srv.blockcount()
         self.assertEqual(srv.resultcount, 1)
 
@@ -701,20 +703,21 @@
         txid = 'b348f416ff86b28652c2e7f961fbcb1a6099fbb398c6e902e37b680208498d77'
         srv = ServiceTest(min_providers=3, network='litecoin')
         srv.mempool(txid)
         for provider in srv.results:
             # print("Mempool: Comparing ltc provider %s" % provider)
             self.assertListEqual(srv.results[provider], [])
 
-        txid = '15641a37e21a0cf7611a1633954be645512f1ab725a0d5077a9ad0aa0ca20bed'
-        srv = ServiceTest(min_providers=3, network='dash')
-        srv.mempool(txid)
-        for provider in srv.results:
-            # print("Mempool: Comparing dash provider %s" % provider)
-            self.assertListEqual(srv.results[provider], [])
+        # FIXME: Disabled, not enough working providers
+        # txid = '15641a37e21a0cf7611a1633954be645512f1ab725a0d5077a9ad0aa0ca20bed'
+        # srv = ServiceTest(min_providers=3, network='dash')
+        # srv.mempool(txid)
+        # for provider in srv.results:
+        #     # print("Mempool: Comparing dash provider %s" % provider)
+        #     self.assertListEqual(srv.results[provider], [])
 
     # FIXME: Disabled, not enough working providers
     # def test_service_dash(self):
     #     srv = ServiceTest(network='dash')
     #     address = 'XoLTipv6ryWECYu94vbkmDjntAXqNgouTW'
     #     txid = 'f770f05d2b1c63b71b2650227252da06ef226661982c4ee9b136b64f77bbbd0c'
     #     self.assertGreaterEqual(srv.getbalance(address), 50000000000)
@@ -739,15 +742,15 @@
             self.assertEqual(len(blk['txs']), 10)
             if blk['version']:
                 self.assertEqual(blk['version'], 1)
             self.assertEqual(blk['txs'][9],
                              '13e3167d46334600b59a5aa286dd02147ac33e64bfc2e188e1f0c0a442182584')
 
     def test_service_getblock_height(self):
-        srv = ServiceTest(timeout=TIMEOUT_TEST, exclude_providers=['chainso'], cache_uri='')
+        srv = ServiceTest(timeout=TIMEOUT_TEST, cache_uri='')
         b = srv.getblock(599999, parse_transactions=True, limit=3)
         print("Test getblock using provider %s" % list(srv.results.keys())[0])
         self.assertEqual(b.height, 599999)
         self.assertEqual(to_hexstring(b.block_hash), '00000000000000000003ecd827f336c6971f6f77a0b9fba362398dd867975645')
         self.assertEqual(to_hexstring(b.merkle_root), 'ca13ce7f21619f73fb5a062696ec06a4427c6ad9e523e7bc1cf5287c137ddcea')
         self.assertEqual(b.nonce_int, 687352075)
         if list(srv.results.keys())[0] != 'blockchair':
@@ -949,15 +952,15 @@
     #                             'c756b40fd5226c8ebe3c279e4f5aebc034b6d48d21039b904498e7702692b72b265dfb0221994bb850'
     #                             '5ee50837aba768083b3a25aba952aeffffffff0240787d010000000017a914d9f17035fdd2180e4e67'
     #                             'de2c17d63c218948780a875022d64ead01000017a91494d0071ed66b6584650440fdc6dfc2916a119b'
     #                             '068700000000')
 
     def test_service_cache_transactions_after_txid(self):
         # Do not store anything in cache if after_txid is used
-        srv = ServiceTest(cache_uri=DATABASEFILE_CACHE_UNITTESTS2, exclude_providers=['chainso', 'mempool'])
+        srv = ServiceTest(cache_uri=DATABASEFILE_CACHE_UNITTESTS2, exclude_providers=['mempool'])
         address = '12spqcvLTFhL38oNJDDLfW1GpFGxLdaLCL'
         res = srv.gettransactions(address,
                                   after_txid='5f31da8f47a5bd92a6929179082c559e8acc270a040b19838230aab26309cf2d')
         self.assertGreaterEqual(len(res), 1)
         self.assertGreaterEqual(srv.results_cache_n, 0)
         res = srv.gettransactions(address)
         self.assertGreaterEqual(len(res), 1)
@@ -1003,15 +1006,15 @@
         srv.gettransaction('4156e78f347e47d2ccdd4a19614d958c6e4502d09a68f63ed0c72691f63a5028')
         txs = srv.gettransactions(address, limit=5)
         self.assertGreaterEqual(len(txs), 5)
         txs = srv.gettransactions(address, after_txid=after_txid, limit=5)
         self.assertGreaterEqual(len(txs), 5)
 
     def test_service_cache_correctly_update_spent_info(self):
-        srv = ServiceTest(cache_uri=DATABASEFILE_CACHE_UNITTESTS2, exclude_providers=['chainso'])
+        srv = ServiceTest(cache_uri=DATABASEFILE_CACHE_UNITTESTS2)
         srv.gettransactions('1KoAvaL3wfpcNvGCQYkqFJG9Ccqm52sZHa', limit=1)
         txs = srv.gettransactions('1KoAvaL3wfpcNvGCQYkqFJG9Ccqm52sZHa')
         self.assertTrue(txs[0].outputs[0].spent)
 
     def test_service_cache_getblock_hash(self):
 
         def check_block_128594(b):
@@ -1025,15 +1028,15 @@
                              '000000000000166d87b745a1d2af24f51c4b98021f8c027954711ce45f2024b3')
             self.assertEqual(b.time, 1307204137)
             self.assertEqual(b.tx_count, 93)
             self.assertEqual(b.version_int, 1)
             self.assertEqual(b.transactions[0].txid, '85249ed3a9526b980e9b7c37b0be9a8fb6bd4462418d7dd808ad702a00777577')
 
         for cache_db in DATABASES_CACHE:
-            srv = ServiceTest(cache_uri=cache_db, exclude_providers=['chainso', 'blockchair', 'bitcoind'])
+            srv = ServiceTest(cache_uri=cache_db, exclude_providers=['blockchair', 'bitcoind'])
             b = srv.getblock('0000000000001a7dcac3c01bf10c5d5fe53dc8cc4b9c94001662e9d7bd36f6cc', limit=1)
             print("Test getblock with hash using provider %s" % list(srv.results.keys())[0])
             check_block_128594(b)
             self.assertEqual(srv.results_cache_n, 0)
 
             # Now retrieve from cache
             bc = srv.getblock('0000000000001a7dcac3c01bf10c5d5fe53dc8cc4b9c94001662e9d7bd36f6cc', limit=1)
```

### Comparing `bitcoinlib-0.6.7/tests/test_tools.py` & `bitcoinlib-0.6.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_transactions.py` & `bitcoinlib-0.6.9/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_values.py` & `bitcoinlib-0.6.9/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/tests/test_wallets.py` & `bitcoinlib-0.6.9/tests/test_wallets.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,29 +822,31 @@
     def test_wallet_multiple_networks_import_error(self):
         pk_dashtest = 'YXsfembHRwpatrAVUGY8MBUuKwhUDf9EEWeZwGoEfE5appg5rLjSfZ1GwoaNB5DgUZ2aVuU1ezmg7zDefubuWkZ17et5o' \
                       'KoMgKnjvAZ6a4Yn2QZg'
         error_str = "Network bitcoinlib_test not available in this wallet, please create an account for this network " \
                     "first."
         self.assertRaisesRegexp(WalletError, error_str, self.wallet.import_key, pk_dashtest)
 
-    def test_wallet_multiple_networks_value(self):
-        pk = 'vprv9DMUxX4ShgxMM1FFB24BgXE3fMYXKicceSdMUtfhyyUzKNkCvPeYrcoZpPezahBEzFc23yHTPj46eqx3jKuQpQFq5kbd2oxDysdteSN16sH'
-        wallet_delete_if_exists('test_wallet_multiple_networks_value', force=True, db_uri=self.DATABASE_URI)
-        w = wallet_create_or_open('test_wallet_multiple_networks_value', keys=pk, db_uri=self.DATABASE_URI)
-        w.new_account(network='bitcoin')
-        w.new_account(network='bitcoinlib_test')
-        w.utxos_update(networks='testnet')
-        self.assertEqual(len(w.utxos(network='testnet')), 1)
-        w.utxos_update(networks='bitcoinlib_test')
-        self.assertEqual(len(w.utxos(network='bitcoinlib_test')), 4)
-        t = w.send_to('blt1qctnl4yk3qepjy3uu36kved5ds6q9g8c6raan7l', '50 mTST', offline=False)
-        self.assertTrue(t.pushed)
-        t = w.send_to('tb1qhq6x777xpj32jm005qppxa6gyxt3qrc376ye6c', '0.1 mTBTC')
-        self.assertFalse(t.pushed)
-        self.assertTrue(t.verified)
+    # FIXME: Disabled for now, too many unknown failures
+    # def test_wallet_multiple_networks_value(self):
+    #     pk = 'vprv9DMUxX4ShgxMM1FFB24BgXE3fMYXKicceSdMUtfhyyUzKNkCvPeYrcoZpPezahBEzFc23yHTPj46eqx3jKuQpQFq5kbd2oxDysd' \
+    #          'teSN16sH'
+    #     wallet_delete_if_exists('test_wallet_multiple_networks_value', force=True, db_uri=self.DATABASE_URI)
+    #     w = wallet_create_or_open('test_wallet_multiple_networks_value', keys=pk, db_uri=self.DATABASE_URI)
+    #     w.new_account(network='bitcoin')
+    #     w.new_account(network='bitcoinlib_test')
+    #     w.utxos_update(networks='testnet')
+    #     self.assertEqual(len(w.utxos(network='testnet')), 2)
+    #     w.utxos_update(networks='bitcoinlib_test')
+    #     self.assertEqual(len(w.utxos(network='bitcoinlib_test')), 4)
+    #     t = w.send_to('blt1qctnl4yk3qepjy3uu36kved5ds6q9g8c6raan7l', '50 mTST', offline=False)
+    #     self.assertTrue(t.pushed)
+    #     t = w.send_to('tb1qhq6x777xpj32jm005qppxa6gyxt3qrc376ye6c', '0.1 mTBTC', fee=1000)
+    #     self.assertFalse(t.pushed)
+    #     self.assertTrue(t.verified)
 
 
 @parameterized_class(*params)
 class TestWalletMultiNetworksMultiAccount(TestWalletMixin, unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `bitcoinlib-0.6.7/tests/transactions_raw.json` & `bitcoinlib-0.6.9/tests/transactions_raw.json`

 * *Files identical despite different names*

### Comparing `bitcoinlib-0.6.7/updatedb.py` & `bitcoinlib-0.6.9/updatedb.py`

 * *Files identical despite different names*

