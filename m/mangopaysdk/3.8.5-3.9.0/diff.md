# Comparing `tmp/mangopaysdk-3.8.5.tar.gz` & `tmp/mangopaysdk-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mangopaysdk-3.8.5.tar", last modified: Fri Dec 18 19:11:44 2020, max compression
+gzip compressed data, was "dist/mangopaysdk-3.9.0.tar", last modified: Tue Feb 23 08:02:16 2021, max compression
```

## Comparing `mangopaysdk-3.8.5.tar` & `mangopaysdk-3.9.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1885 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/DESCRIPTION.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2177 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopaysdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/mangopay/
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/ratelimit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62758 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10845 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6362 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/page.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24716 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      731 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29378 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      560 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3828 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/auth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8835 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9884 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/mangopay/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3897 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_ubos.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_wallets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/tests/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/ubo_declaration_submit.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      669 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/declarative_user.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      637 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/natural_user.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_list_3_per_page_page2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/legal_user_wallet.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_list_2_per_page_page1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/ubo.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/legal_user.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/legal_user_wallet_89.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      629 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/cardregistrations_update.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/legal_user_wallet_99.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1927 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_list_page1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_list_2_per_page.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/ubo_update.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/cardregistrations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      264 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/natural_user_wallet_9.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      380 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/card.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      170 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/ubo_declaration.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_wallet.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/list_ubo_declarations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/natural_user_wallet.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/fixtures/user_list_full.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3255 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_banking_aliases.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      401 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_repudiations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16253 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_refunds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      887 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_kyc_document.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18848 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_bankaccounts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32332 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_preauthorizations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_tokens.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8463 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_transactions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12440 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_disputes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_idempotency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_rate_limit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_clients.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_mandates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6730 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_client_wallets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35614 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_payins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6449 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_documentconsult.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/tests/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/images/image.jpg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2280 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_reports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9904 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_cards.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11402 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/mocks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7880 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_transfers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-18 19:11:44.000000 mangopaysdk-3.8.5/tests/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9030 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/resources/TestKycPageFile.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    11463 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_kycs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      620 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_emoney.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9978 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_notifications.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26396 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_users.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5255 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_payouts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18564 2020-12-18 19:10:20.000000 mangopaysdk-3.8.5/tests/test_base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      150 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/DESCRIPTION.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2177 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      194 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopaysdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/mangopay/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      290 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/signals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/ratelimit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62887 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/resources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10845 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6362 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/page.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25021 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/fields.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      731 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29692 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      560 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3828 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8835 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9880 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      624 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/mangopay/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3897 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_ubos.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_wallets.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/tests/fixtures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      175 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/ubo_declaration_submit.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      669 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/declarative_user.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      637 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/natural_user.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_list_3_per_page_page2.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/legal_user_wallet.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_list_2_per_page_page1.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/ubo.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/legal_user.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/legal_user_wallet_89.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      629 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/cardregistrations_update.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/legal_user_wallet_99.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1927 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_list_page1.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_list_2_per_page.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/ubo_update.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/cardregistrations.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      264 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/natural_user_wallet_9.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      380 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/card.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      170 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/ubo_declaration.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_wallet.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/list_ubo_declarations.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/natural_user_wallet.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/fixtures/user_list_full.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3255 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_banking_aliases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      401 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_repudiations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16253 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_refunds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      887 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_kyc_document.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18848 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_bankaccounts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32472 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_preauthorizations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_tokens.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8558 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_transactions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      277 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/resources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12440 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_disputes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_idempotency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_rate_limit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_clients.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_mandates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6730 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_client_wallets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35650 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_payins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6449 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_documentconsult.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/tests/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/images/image.jpg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2280 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_reports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9904 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_cards.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11402 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/mocks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7880 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_transfers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-23 08:02:16.000000 mangopaysdk-3.9.0/tests/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9030 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/resources/TestKycPageFile.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11463 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_kycs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      620 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_emoney.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9978 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_notifications.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26396 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_users.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5379 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_payouts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18564 2021-02-23 08:01:46.000000 mangopaysdk-3.9.0/tests/test_base.py
```

### Comparing `mangopaysdk-3.8.5/PKG-INFO` & `mangopaysdk-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangopaysdk
-Version: 3.8.5
+Version: 3.9.0
 Summary: A client library written in python to work with mangopay v2 api
 Home-page: https://github.com/Mangopay/mangopay2-python-sdk
 Author: Mangopay (www.mangopay.com)
 Author-email: support@mangopay.com
 License: MIT
 Description: This SDK is a client library for interacting with the Mangopay API.
 Keywords: mangopay api development emoney sdk
@@ -12,9 +12,9 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `mangopaysdk-3.8.5/README.md` & `mangopaysdk-3.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 
 License
 -------------------------------------------------
 MangopaySDK is distributed under MIT license, see LICENSE file.
 
 Contact
 -------------------------------------------------
-Report bugs or suggest features using [issue tracker at GitHub](https://github.com/MangoPay/mangopay2-python-sdk-v2).
+Report bugs or suggest features using [issue tracker at GitHub](https://github.com/Mangopay/mangopay2-python-sdk/issues).
 
 
 Account creation
 -------------------------------------------------
-You can get yourself a [free sandbox account](https://www.mangopay.com/signup/create-sandbox/) or sign up for a [production account](https://www.mangopay.com/signup/production-account/) (note that validation of your production account can take a few days, so think about doing it in advance of when you actually want to go live).
+You can get yourself a free sandbox account or sign up for a production account by [registering on the Mangopay site](https://www.mangopay.com/start/) (note that validation of your production account involves several steps, so think about doing it in advance of when you actually want to go live).
 
 Inspiration
 -----------
 
 The data model of python-mangopay is highly inspired by [peewee](https://github.com/coleifer/peewee).
 
 Credits
```

### Comparing `mangopaysdk-3.8.5/mangopaysdk.egg-info/PKG-INFO` & `mangopaysdk-3.9.0/mangopaysdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangopaysdk
-Version: 3.8.5
+Version: 3.9.0
 Summary: A client library written in python to work with mangopay v2 api
 Home-page: https://github.com/Mangopay/mangopay2-python-sdk
 Author: Mangopay (www.mangopay.com)
 Author-email: support@mangopay.com
 License: MIT
 Description: This SDK is a client library for interacting with the Mangopay API.
 Keywords: mangopay api development emoney sdk
@@ -12,9 +12,9 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `mangopaysdk-3.8.5/mangopaysdk.egg-info/SOURCES.txt` & `mangopaysdk-3.9.0/mangopaysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/LICENSE` & `mangopaysdk-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/resources.py` & `mangopaysdk-3.9.0/mangopay/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
 @python_2_unicode_compatible
 class Wallet(BaseModel):
     owners = ManyToManyField(User, api_name='Owners', related_name='wallets', required=True)
     description = CharField(api_name='Description', required=True)
     currency = CharField(api_name='Currency', required=True)
     balance = MoneyField(api_name='Balance')
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
 
     class Meta:
         verbose_name = 'wallet'
         verbose_name_plural = 'wallets'
         url = '/wallets'
 
     def __init__(self, *args, **kwargs):
@@ -268,22 +268,22 @@
 class Transfer(BaseModel):
     author = ForeignKeyField(User, api_name='AuthorId', required=True)
     credited_user = ForeignKeyField(User, api_name='CreditedUserId', required=True, related_name='credited_users')
     debited_funds = MoneyField(api_name='DebitedFunds', required=True)
     fees = MoneyField(api_name='Fees', required=True)
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId')
     credited_wallet = ForeignKeyField(Wallet, api_name='CreditedWalletId', required=True)
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
     credited_funds = MoneyField(api_name='CreditedFunds')
     status = CharField(api_name='Status',
                        choices=constants.STATUS_CHOICES,
                        default=None)
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
 
     def get_refunds(self, *args, **kwargs):
         kwargs['id'] = self.id
         select = SelectQuery(Refund, *args, **kwargs)
         select.identifier = 'TRANSFER_GET_REFUNDS'
         return select.all(*args, **kwargs)
 
@@ -294,15 +294,15 @@
 
     def __str__(self):
         return 'Transfer from wallet %s to wallet %s' % (self.debited_wallet_id, self.credited_wallet_id)
 
 
 @python_2_unicode_compatible
 class Card(BaseModel):
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
     expiration_date = CharField(api_name='ExpirationDate')
     alias = CharField(api_name='Alias')
     card_provider = CharField(api_name='CardProvider')
     card_type = CharField(api_name='CardType',
                           choices=constants.CARD_TYPE_CHOICES,
                           default=None)
     country = CharField(api_name='Country')
@@ -362,15 +362,15 @@
     access_key = CharField(api_name='AccessKey')
     preregistration_data = CharField(api_name='PreregistrationData')
     registration_data = CharField(api_name='RegistrationData')
     card = ForeignKeyField(Card, api_name='CardId')
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
     status = CharField(api_name='Status', choices=constants.CARD_STATUS_CHOICES, default=None)
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
 
     class Meta:
         verbose_name = 'cardregistration'
         verbose_name_plural = 'cardregistrations'
         url = '/cardregistrations'
 
 
@@ -434,15 +434,15 @@
     credited_user = ForeignKeyField(User, api_name='CreditedUserId', related_name='credited_users')
     credited_funds = MoneyField(api_name='CreditedFunds')
     credited_wallet = ForeignKeyField(Wallet, api_name='CreditedWalletId', required=True)
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId')
     status = CharField(api_name='Status', choices=constants.STATUS_CHOICES, default=None)
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
     type = CharField(api_name='Type', choices=constants.TRANSACTION_TYPE_CHOICES, default=None)
     nature = CharField(api_name='Nature', choices=constants.NATURE_CHOICES, default=None)
     payment_type = CharField(api_name='PaymentType', choices=constants.PAYIN_PAYMENT_TYPE, default=None)
     execution_type = CharField(api_name='ExecutionType', choices=constants.EXECUTION_TYPE_CHOICES, default=None)
 
     def get_refunds(self, *args, **kwargs):
         kwargs['id'] = self.id
@@ -480,22 +480,22 @@
     secure_mode_redirect_url = CharField(api_name='SecureModeRedirectURL')
     secure_mode_return_url = CharField(api_name='SecureModeReturnURL', required=True)
     card = ForeignKeyField(Card, api_name='CardId', required=True)
     secure_mode_needed = BooleanField(api_name='SecureModeNeeded')
     secure_mode = CharField(api_name='SecureMode',
                             choices=constants.SECURE_MODE_CHOICES,
                             default=constants.SECURE_MODE_CHOICES.default)
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
     statement_descriptor = CharField(api_name='StatementDescriptor')
     debited_funds = MoneyField(api_name='DebitedFunds', required=True)
     fees = MoneyField(api_name='Fees', required=True)
     billing = BillingField(api_name='Billing')
     security_info = SecurityInfoField(api_name='SecurityInfo')
     culture = CharField(api_name='Culture')
-    ip_address = CharField(api_name='IpAdress')
+    ip_address = CharField(api_name='IpAddress')
     browser_info = BrowserInfoField(api_name='BrowserInfo')
     shipping = ShippingField(api_name='Shipping')
 
     class Meta:
         verbose_name = 'payin'
         verbose_name_plural = 'payins'
         url = {
@@ -680,20 +680,20 @@
                             choices=constants.SECURE_MODE_CHOICES,
                             default=constants.SECURE_MODE_CHOICES.default,
                             required=True)
     card = ForeignKeyField(Card, api_name='CardId', required=True)
     secure_mode_needed = BooleanField(api_name='SecureModeNeeded')
     secure_mode_redirect_url = CharField(api_name='SecureModeRedirectURL')
     secure_mode_return_url = CharField(api_name='SecureModeReturnURL', required=True)
-    expiration_date = DateField(api_name='ExpirationDate')
+    expiration_date = DateTimeField(api_name='ExpirationDate')
     payin = ForeignKeyField(PayIn, api_name='PayInId')
     billing = BillingField(api_name='Billing')
     security_info = SecurityInfoField(api_name='SecurityInfo')
     multi_capture = BooleanField(api_name='MultiCapture')
-    ip_address = CharField(api_name='IpAdress')
+    ip_address = CharField(api_name='IpAddress')
     browser_info = BrowserInfoField(api_name='BrowserInfo')
     shipping = ShippingField(api_name='Shipping')
 
     def get_transactions(self, *args, **kwargs):
         kwargs['id'] = self.id
         select = SelectQuery(Transaction, *args, **kwargs)
         select.identifier = 'PRE_AUTHORIZATION_TRANSACTIONS'
@@ -735,15 +735,15 @@
 
 
 @python_2_unicode_compatible
 class BankAccount(BaseModel):
     user = ForeignKeyField(User, api_name='UserId', related_name='bankaccounts')
     owner_name = CharField(api_name='OwnerName', required=True)
     owner_address = AddressField(api_name='OwnerAddress', required=True)
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
     type = CharField(api_name='Type', choices=constants.BANK_ACCOUNT_TYPE_CHOICES, default=None, required=True)
     iban = CharField(api_name='IBAN')
     bic = CharField(api_name='BIC')
     account_number = CharField(api_name='AccountNumber')
     sort_code = CharField(api_name='SortCode')
     aba = CharField(api_name='ABA')
     deposit_account_type = CharField(api_name='DepositAccountType',
@@ -799,22 +799,23 @@
     credited_funds = MoneyField(api_name='CreditedFunds')
     debited_funds = MoneyField(api_name='DebitedFunds', required=True)
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId', required=True)
     bank_account = ForeignKeyField(BankAccount, api_name='BankAccountId', required=True)
     status = CharField(api_name='Status', choices=constants.STATUS_CHOICES, default=None)
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
     type = CharField(api_name='Type', choices=constants.TRANSACTION_TYPE_CHOICES, default=None)
     nature = CharField(api_name='Nature', choices=constants.NATURE_CHOICES, default=None)
     payment_type = CharField(api_name='PaymentType', choices=constants.PAYOUT_PAYMENT_TYPE, default=None)
     execution_type = CharField(api_name='ExecutionType', choices=constants.EXECUTION_TYPE_CHOICES, default=None)
     bank_wire_ref = CharField(api_name='BankWireRef')
+    payout_mode_requested = CharField(api_name='PayoutModeRequested')
     credited_user = ForeignKeyField(User, api_name='CreditedUserId')
-    creation_date = DateField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
 
     def get_refunds(self, *args, **kwargs):
         kwargs['id'] = self.id
         select = SelectQuery(Refund, *args, **kwargs)
         select.identifier = 'PAYOUT_GET_REFUNDS'
         return select.all(*args, **kwargs)
 
@@ -842,15 +843,15 @@
     credited_user = ForeignKeyField(User, api_name='CreditedUserId', related_name='credited_users')
     debited_funds = MoneyField(api_name='DebitedFunds')
     credited_funds = MoneyField(api_name='CreditedFunds')
     fees = MoneyField(api_name='Fees')
     status = CharField(api_name='Status', choices=constants.STATUS_CHOICES, default=None)
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
     type = CharField(api_name='Type', choices=constants.TRANSACTION_TYPE_CHOICES, default=None)
     nature = CharField(api_name='Nature', choices=constants.NATURE_CHOICES, default=None)
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId')
     credited_wallet = ForeignKeyField(Wallet, api_name='CreditedWalletId')
     refund_reason = RefundReasonField(api_name='RefundReason')
     initial_transaction_id = CharField(api_name='InitialTransactionId')
     initial_transaction_type = CharField(api_name='InitialTransactionType', choices=constants.TRANSACTION_TYPE_CHOICES,
@@ -953,15 +954,15 @@
     credited_user = ForeignKeyField(User, api_name='CreditedUserId')
     debited_funds = MoneyField(api_name='DebitedFunds')
     credited_funds = MoneyField(api_name='CreditedFunds')
     fees = MoneyField(api_name='Fees')
     status = CharField(api_name='Status', choices=constants.STATUS_CHOICES, default=None)
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
     type = CharField(api_name='Type', choices=constants.TRANSACTION_TYPE_CHOICES, default=None)
     nature = CharField(api_name='Nature', choices=constants.NATURE_CHOICES, default=None)
     credited_wallet = ForeignKeyField(Wallet, api_name='CreditedWalletId')
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId')
     wallet = ForeignKeyField(Wallet, related_name='transactions')
     creation_date = DateTimeField(api_name='CreationDate')
 
@@ -1228,15 +1229,15 @@
     credited_funds = MoneyField(api_name='CreditedFunds')
     fees = MoneyField(api_name='Fees')
     credited_wallet = CharField(Wallet, api_name='CreditedWalletId')
     debited_wallet = ForeignKeyField(Wallet, api_name='DebitedWalletId')
     credited_user = ForeignKeyField(User, api_name='CreditedUserId')
     nature = CharField(api_name='Nature', choices=constants.NATURE_CHOICES, default=None)
     status = CharField(api_name='Status', choices=constants.STATUS_CHOICES, default=None)
-    execution_date = DateField(api_name='ExecutionDate')
+    execution_date = DateTimeField(api_name='ExecutionDate')
     result_code = CharField(api_name='ResultCode')
     result_message = CharField(api_name='ResultMessage')
 
     creation_date = DateTimeField(api_name='CreationDate')
 
     def get_refunds(self, *args, **kwargs):
         kwargs['id'] = self.id
@@ -1447,15 +1448,15 @@
             InsertQuery.identifier: '/wallets/%(wallet_id)s/bankingaliases/accountNumber',
             SelectQuery.identifier: '/bankingaliases/%(id)s',
             UpdateQuery.identifier: '/bankingaliases/%(id)s'
         }
 
 
 class UboDeclaration(BaseModel):
-    creation_date = IntegerField(api_name='CreationDate')
+    creation_date = DateTimeField(api_name='CreationDate')
     processed_date = IntegerField(api_name='ProcessedDate')
     reason = CharField(api_name='Reason')
     message = CharField(api_name='Message')
     status = CharField(api_name='Status', choices=constants.UBO_DECLARATION_STATUS_CHOICES, default=None)
     ubos = ListField(api_name='Ubos')
     user = ForeignKeyField(User)
```

### Comparing `mangopaysdk-3.8.5/mangopay/constants.py` & `mangopaysdk-3.9.0/mangopay/constants.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/query.py` & `mangopaysdk-3.9.0/mangopay/query.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/fields.py` & `mangopaysdk-3.9.0/mangopay/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,22 +228,24 @@
 
         return value
 
 
 class BillingField(Field):
     def python_value(self, value):
         if value is not None:
-            return Billing(address=value['Address'])
+            return Billing(first_name=value['FirstName'], last_name=value['LastName'], address=value['Address'])
         return value
 
     def api_value(self, value):
         value = super(BillingField, self).api_value(value)
 
         if isinstance(value, Billing):
             value = {
+                'FirstName': value.first_name,
+                'LastName': value.last_name,
                 'Address': value.address
             }
 
         return value
 
 
 class SecurityInfoField(Field):
@@ -746,19 +748,21 @@
 
         return value
 
 
 class ShippingField(Field):
     def python_value(self, value):
         if value is not None:
-            return Shipping(address=value['Address'])
+            return Shipping(first_name=value['FirstName'], last_name=value['LastName'], address=value['Address'])
         return value
 
     def api_value(self, value):
         value = super(ShippingField, self).api_value(value)
 
-        if isinstance(value, Billing):
+        if isinstance(value, Shipping):
             value = {
+                'FirstName': value.first_name,
+                'LastName': value.last_name,
                 'Address': value.address
             }
 
         return value
```

### Comparing `mangopaysdk-3.8.5/mangopay/exceptions.py` & `mangopaysdk-3.9.0/mangopay/exceptions.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/utils.py` & `mangopaysdk-3.9.0/mangopay/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,19 +231,22 @@
 
     def __str__(self):
         return 'PlatformCategorization: %s %s' % (self.business_type, self.sector)
 
 
 @add_camelcase_aliases
 class Billing(object):
-    def __init__(self, address=None):
+    def __init__(self, first_name=None, last_name=None, address=None):
+        self.first_name = first_name
+        self.last_name = last_name
         self.address = address
 
     def __str__(self):
-        return 'Billing: %s' % self.address
+        return 'Billing: %s' % \
+               (self.first_name, self.last_name, self.address)
 
 
 @add_camelcase_aliases
 class SecurityInfo(object):
     def __init__(self, avs_result=None):
         self.avs_result = avs_result
 
@@ -506,19 +509,22 @@
             "TimeZoneOffset": self.timezone_offset,
             "UserAgent": self.user_agent
         }
 
 
 @add_camelcase_aliases
 class Shipping(object):
-    def __init__(self, address=None):
+    def __init__(self, first_name=None, last_name=None, address=None):
+        self.first_name = first_name
+        self.last_name = last_name
         self.address = address
 
     def __str__(self):
-        return 'Shipping: %s' % self.address
+        return 'Shipping: %s' % \
+               (self.first_name, self.last_name, self.address)
 
 
 @add_camelcase_aliases
 class ScopeBlocked(object):
     def __init__(self, inflows=None, outflows=None):
         self.inflows = inflows
         self.outflows = outflows
```

### Comparing `mangopaysdk-3.8.5/mangopay/compat.py` & `mangopaysdk-3.9.0/mangopay/compat.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/auth.py` & `mangopaysdk-3.9.0/mangopay/auth.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/base.py` & `mangopaysdk-3.9.0/mangopay/base.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/mangopay/api.py` & `mangopaysdk-3.9.0/mangopay/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def custom_request(self, method, url, data=None, idempotency_key=None, oauth_request=False,
                        is_mangopay_request=False, **params):
         params = params or {}
 
         headers = {}
 
         if is_mangopay_request:
-            headers['User-Agent'] = 'MangoPay V2 SDK Python ' + str(mangopay.package_version)
+            headers['User-Agent'] = 'MangoPay V2 Python/' + str(mangopay.package_version)
             if oauth_request:
                 headers['Authorization'] = self.auth_manager.basic_token()
                 headers['Content-Type'] = 'application/x-www-form-urlencoded'
             else:
                 headers['Authorization'] = self.auth_manager.get_token()
                 headers['Content-Type'] = 'application/json'
```

### Comparing `mangopaysdk-3.8.5/mangopay/__init__.py` & `mangopaysdk-3.9.0/mangopay/__init__.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/setup.py` & `mangopaysdk-3.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'DESCRIPTION.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mangopaysdk',
-    version='3.8.5',
+    version='3.9.0',
     description='A client library written in python to work with mangopay v2 api',
     long_description='This SDK is a client library for interacting with the Mangopay API.',
     url='https://github.com/Mangopay/mangopay2-python-sdk',
     author='Mangopay (www.mangopay.com)',
     author_email='support@mangopay.com',
     license='MIT',
     classifiers=[
```

### Comparing `mangopaysdk-3.8.5/tests/test_ubos.py` & `mangopaysdk-3.9.0/tests/test_ubos.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_wallets.py` & `mangopaysdk-3.9.0/tests/test_wallets.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/declarative_user.json` & `mangopaysdk-3.9.0/tests/fixtures/declarative_user.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/natural_user.json` & `mangopaysdk-3.9.0/tests/fixtures/natural_user.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/user_list_3_per_page_page2.json` & `mangopaysdk-3.9.0/tests/fixtures/user_list_3_per_page_page2.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/legal_user.json` & `mangopaysdk-3.9.0/tests/fixtures/legal_user.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/cardregistrations_update.json` & `mangopaysdk-3.9.0/tests/fixtures/cardregistrations_update.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/user_list_page1.json` & `mangopaysdk-3.9.0/tests/fixtures/user_list_page1.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/cardregistrations.json` & `mangopaysdk-3.9.0/tests/fixtures/cardregistrations.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/fixtures/user_list_full.json` & `mangopaysdk-3.9.0/tests/fixtures/user_list_full.json`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_banking_aliases.py` & `mangopaysdk-3.9.0/tests/test_banking_aliases.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_refunds.py` & `mangopaysdk-3.9.0/tests/test_refunds.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_kyc_document.py` & `mangopaysdk-3.9.0/tests/test_kyc_document.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_bankaccounts.py` & `mangopaysdk-3.9.0/tests/test_bankaccounts.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_preauthorizations.py` & `mangopaysdk-3.9.0/tests/test_preauthorizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,14 +702,16 @@
         billing = Billing()
         billing.address = Address()
         billing.address.address_line_1 = "Main Street"
         billing.address.address_line_2 = "no. 5 ap. 6"
         billing.address.country = "FR"
         billing.address.city = "Lyon"
         billing.address.postal_code = "65400"
+        billing.last_name = "Doe"
+        billing.first_name = "John"
         pre_authorization.billing = billing
 
         saved_pre_authorization = pre_authorization.save()
 
         self.assertIsNotNone(saved_pre_authorization)
         security_info = saved_pre_authorization['security_info']
         self.assertIsInstance(security_info, SecurityInfo)
@@ -750,14 +752,16 @@
         billing = Billing()
         billing.address = Address()
         billing.address.address_line_1 = "Main Street"
         billing.address.address_line_2 = "no. 5 ap. 6"
         billing.address.country = "FR"
         billing.address.city = "Lyon"
         billing.address.postal_code = "65400"
+        billing.last_name = "Doe"
+        billing.first_name = "John"
         pre_authorization.billing = billing
 
         saved_pre_authorization = pre_authorization.save()
 
         wallet = BaseTestLive.get_johns_wallet()
 
         payin = PreAuthorizedPayIn()
```

### Comparing `mangopaysdk-3.8.5/tests/test_tokens.py` & `mangopaysdk-3.9.0/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_transactions.py` & `mangopaysdk-3.9.0/tests/test_transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
+import time
+from datetime import date, datetime
+
+import responses
+
+from mangopay.utils import Money, timestamp_from_date
 from tests import settings
 from tests.resources import Transfer, Transaction
 from tests.test_base import BaseTest
 
-from mangopay.utils import Money
-
-from datetime import date
-
-import responses
-import time
-
+today = datetime.utcnow().date()
+today_timestamp = timestamp_from_date(today)
 
 class TransactionsTest(BaseTest):
     @responses.activate
     def test_retrieve_transactions(self):
         self.mock_natural_user()
         self.mock_legal_user()
         self.mock_user_wallet()
@@ -39,15 +40,15 @@
                     "Fees": {
                         "Currency": "EUR",
                         "Amount": 100
                     },
                     "Status": "SUCCEEDED",
                     "ResultCode": "000000",
                     "ResultMessage": "Success",
-                    "ExecutionDate": int(time.mktime(date.today().timetuple())),
+                    "ExecutionDate": today_timestamp,
                     "Type": "TRANSFER",
                     "Nature": "REGULAR",
                     "DebitedWalletId": "1167496",
                     "CreditedWalletId": "1167504"
                 },
                 'status': 200
             },
@@ -70,15 +71,15 @@
                         "Fees": {
                             "Currency": "EUR",
                             "Amount": 0
                         },
                         "Status": "CREATED",
                         "ResultCode": "000000",
                         "ResultMessage": "Success",
-                        "ExecutionDate": "2015-05-15",
+                        "ExecutionDate": today_timestamp,
                         "Type": "TRANSFER",
                         "Nature": "REFUND",
                         "DebitedWalletId": "1174774"
                     }
                 ],
                 'status': 200,
                 'match_querystring': True
@@ -102,15 +103,15 @@
                         "Fees": {
                             "Currency": "EUR",
                             "Amount": 0
                         },
                         "Status": "CREATED",
                         "ResultCode": "000000",
                         "ResultMessage": "Success",
-                        "ExecutionDate": "2015-05-15",
+                        "ExecutionDate": today_timestamp,
                         "Type": "TRANSFER",
                         "Nature": "REFUND",
                         "DebitedWalletId": "1174774"
                     }
                 ],
                 'status': 200,
                 'match_querystring': True
@@ -134,15 +135,15 @@
                         "Fees": {
                             "Currency": "EUR",
                             "Amount": 0
                         },
                         "Status": "FAILED",
                         "ResultCode": "000000",
                         "ResultMessage": "Success",
-                        "ExecutionDate": "2015-05-15",
+                        "ExecutionDate": today_timestamp,
                         "Type": "TRANSFER",
                         "Nature": "REFUND",
                         "DebitedWalletId": "1174774"
                     }
                 ],
                 'status': 200,
                 'match_querystring': True
@@ -168,15 +169,15 @@
                         "Fees": {
                             "Currency": "EUR",
                             "Amount": 100
                         },
                         "Status": "CREATED",
                         "ResultCode": "000000",
                         "ResultMessage": "Success",
-                        "ExecutionDate": 1383156788,
+                        "ExecutionDate": today_timestamp,
                         "Type": "TRANSFER",
                         "Nature": "REGULAR",
                         "CreditedWalletId": "1167504",
                         "DebitedWalletId": "1167494"
                     }
                 ],
                 'status': 200
```

### Comparing `mangopaysdk-3.8.5/tests/test_disputes.py` & `mangopaysdk-3.9.0/tests/test_disputes.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_idempotency.py` & `mangopaysdk-3.9.0/tests/test_idempotency.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_clients.py` & `mangopaysdk-3.9.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_mandates.py` & `mangopaysdk-3.9.0/tests/test_mandates.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_client_wallets.py` & `mangopaysdk-3.9.0/tests/test_client_wallets.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_payins.py` & `mangopaysdk-3.9.0/tests/test_payins.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,15 @@
         pay_in.secure_mode_return_url = "http://www.example.com/"
         address = Address()
         address.address_line_1 = "Big Street"
         address.address_line_2 = "no 2 ap 6"
         address.country = "FR"
         address.city = "Lyon"
         address.postal_code = "68400"
-        pay_in.billing = Billing(address=address)
+        pay_in.billing = Billing(first_name="John", last_name="Doe", address=address)
 
         result = pay_in.save()
 
         self.assertIsNotNone(result)
         security_info = result['security_info']
         self.assertIsNotNone(security_info)
         self.assertIsInstance(security_info, SecurityInfo)
```

### Comparing `mangopaysdk-3.8.5/tests/test_documentconsult.py` & `mangopaysdk-3.9.0/tests/test_documentconsult.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/images/image.jpg` & `mangopaysdk-3.9.0/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_reports.py` & `mangopaysdk-3.9.0/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_cards.py` & `mangopaysdk-3.9.0/tests/test_cards.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/mocks.py` & `mangopaysdk-3.9.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_transfers.py` & `mangopaysdk-3.9.0/tests/test_transfers.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/resources/TestKycPageFile.png` & `mangopaysdk-3.9.0/tests/resources/TestKycPageFile.png`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_kycs.py` & `mangopaysdk-3.9.0/tests/test_kycs.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_emoney.py` & `mangopaysdk-3.9.0/tests/test_emoney.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_notifications.py` & `mangopaysdk-3.9.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_users.py` & `mangopaysdk-3.9.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_payouts.py` & `mangopaysdk-3.9.0/tests/test_payouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             {
                 'method': responses.POST,
                 'url': settings.MANGOPAY_API_SANDBOX_URL+settings.MANGOPAY_CLIENT_ID+'/payouts/bankwire',
                 'body': {
                     "Id": 30047,
                     "CreditedFunds": None,
                     "BankWireRef": "John Doe's trousers",
+                    "PayoutModeRequested": "INSTANT_PAYMENT",
                     "DebitedFunds": {"Currency": "EUR", "Amount": 1000},
                     "BankAccountId": 6784645,
                     "AuthorId": 6784642,
                     "Tag": "Custom data",
                     "Fees": {"Currency": "EUR", "Amount": 100},
                     "DebitedWalletId": 6784644
                 },
@@ -78,15 +79,16 @@
                     "Status": "SUCCEEDED",
                     "ResultCode": "00000",
                     "ExecutionDate": 1374233532,
                     "Type": "PAY_OUT",
                     "Nature": "NORMAL",
                     "DebitedWalletId": "30025",
                     "BankAccountId": "30027",
-                    "BankWireRef": "John Doe's trousers"
+                    "BankWireRef": "John Doe's trousers",
+                    "PayoutModeRequested": "INSTANT_PAYMENT"
                 },
                 'status': 200
             }])
 
         params = {
             "owner_name": "Victor Hugo",
             "user": self.legal_user,
```

### Comparing `mangopaysdk-3.8.5/tests/test_utils.py` & `mangopaysdk-3.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mangopaysdk-3.8.5/tests/test_base.py` & `mangopaysdk-3.9.0/tests/test_base.py`

 * *Files identical despite different names*

