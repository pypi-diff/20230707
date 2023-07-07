# Comparing `tmp/creditas-1.0.0.0.tar.gz` & `tmp/creditas-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creditas-1.0.0.0.tar", last modified: Fri Jul  7 10:23:08 2023, max compression
+gzip compressed data, was "creditas-1.0.0.1.tar", last modified: Fri Jul  7 10:43:06 2023, max compression
```

## Comparing `creditas-1.0.0.0.tar` & `creditas-1.0.0.1.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.428265 creditas-1.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 10:22:56.000000 creditas-1.0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-07 10:23:08.428265 creditas-1.0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-07-07 10:22:56.000000 creditas-1.0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.376263 creditas-1.0.0.0/creditas/
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.380263 creditas-1.0.0.0/creditas/api/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/administration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/aisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23947 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/balance_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/card_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/cisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/example_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/loan_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29283 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/payment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/pisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/statement_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.400264 creditas-1.0.0.0/creditas/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_term_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_transaction_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_transaction_filter_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/account_transaction_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/aisp_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/aisp_account_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/aisp_account_transaction_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body10.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body12.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body13.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body14.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body15.py
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body16.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body17.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body19.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body20.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body21.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body23.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body24.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body25.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body26.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body27.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body28.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body7.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body8.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/body9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/cispaccountbalancecheck_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/clientregistrationcreate_client_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/debit_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_transaction_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_transaction_authorization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_validation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_validation_data_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/error_validation_data_validation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20010.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20011.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20012.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20013.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20014.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20015.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20016.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20017.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20018.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2001_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20020.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20021.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20022.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20023.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20024.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20025.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20026.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20027.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20028.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20029.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20030.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response20031.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2004.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2005.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2006.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2007.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response2009.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response500.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response5001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/inline_response5002.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/loan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/money.py
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_common_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_domestic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_domestic_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_filter_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_foreign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_foreign_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_sepa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/payment_order_sepa_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/paymentdomesticcreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/paymentdomesticcreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/paymentforeigncreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/paymentsepacreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/paymentsepacreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/pisppaymentdomesticcreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/pisppaymentsepacreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/models/source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-07-07 10:22:56.000000 creditas-1.0.0.0/creditas/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.376263 creditas-1.0.0.0/creditas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-07 10:23:08.000000 creditas-1.0.0.0/creditas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-07 10:23:08.000000 creditas-1.0.0.0/creditas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:23:08.000000 creditas-1.0.0.0/creditas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 10:23:08.000000 creditas-1.0.0.0/creditas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 10:23:08.000000 creditas-1.0.0.0/creditas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:23:08.428265 creditas-1.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-07 10:22:56.000000 creditas-1.0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:23:08.428265 creditas-1.0.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_term_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_transaction_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_transaction_filter_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_account_transaction_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_administration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_aisp_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_aisp_account_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_aisp_account_transaction_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_aisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_balance_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body10.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body11.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body12.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body13.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body14.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body15.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body16.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body17.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body18.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body19.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body2.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body20.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body21.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body22.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body23.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body24.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body25.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body26.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body27.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body28.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body3.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body4.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body5.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body6.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body7.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body8.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_body9.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_card_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_cisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_cispaccountbalancecheck_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_clientregistrationcreate_client_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_debit_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_transaction_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_transaction_authorization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_validation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_validation_data_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_error_validation_data_validation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_example_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20010.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20011.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20012.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20013.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20014.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20015.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20016.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2001_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20021.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20022.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20023.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20025.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20026.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20027.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20028.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20029.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20030.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response20031.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2004.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2005.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2006.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2007.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response2009.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response500.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response5001.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_inline_response5002.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_loan_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_common_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_domestic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_domestic_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_filter_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_foreign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_foreign_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_sepa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_payment_order_sepa_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_paymentdomesticcreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_paymentdomesticcreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_paymentforeigncreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_paymentsepacreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_paymentsepacreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_pisp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_pisppaymentdomesticcreate_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_pisppaymentsepacreate_partner_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_source_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_statement_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 10:22:56.000000 creditas-1.0.0.0/test/test_transaction_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.530325 creditas-1.0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 10:42:53.000000 creditas-1.0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-07 10:43:06.530325 creditas-1.0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-07-07 10:42:53.000000 creditas-1.0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.490321 creditas-1.0.0.1/creditas/
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.494322 creditas-1.0.0.1/creditas/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/administration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/aisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23947 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/balance_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/card_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/cisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/example_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29283 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/pisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/statement_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api/transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.510323 creditas-1.0.0.1/creditas/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_term_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_transaction_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_transaction_filter_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/account_transaction_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/aisp_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/aisp_account_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/aisp_account_transaction_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body20.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body26.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body27.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/body9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/cispaccountbalancecheck_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/clientregistrationcreate_client_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/debit_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_transaction_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_transaction_authorization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_validation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_validation_data_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/error_validation_data_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20014.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2001_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20025.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20027.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20028.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20029.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response20031.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response2009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response5001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/inline_response5002.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_common_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_domestic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_domestic_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_filter_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_foreign_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_sepa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/payment_order_sepa_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/paymentdomesticcreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/paymentdomesticcreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/paymentforeigncreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/paymentsepacreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/paymentsepacreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/pisppaymentdomesticcreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/pisppaymentsepacreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/models/source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-07-07 10:42:53.000000 creditas-1.0.0.1/creditas/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.490321 creditas-1.0.0.1/creditas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-07 10:43:06.000000 creditas-1.0.0.1/creditas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-07 10:43:06.000000 creditas-1.0.0.1/creditas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:43:06.000000 creditas-1.0.0.1/creditas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 10:43:06.000000 creditas-1.0.0.1/creditas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 10:43:06.000000 creditas-1.0.0.1/creditas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:43:06.530325 creditas-1.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 10:42:53.000000 creditas-1.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:43:06.526325 creditas-1.0.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_term_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_transaction_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_transaction_filter_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_account_transaction_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_administration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_aisp_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_aisp_account_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_aisp_account_transaction_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_aisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_balance_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body22.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body23.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body25.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body26.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body27.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body28.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_body9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_card_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_cisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_cispaccountbalancecheck_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_clientregistrationcreate_client_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_debit_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_transaction_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_transaction_authorization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_validation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_validation_data_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_error_validation_data_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_example_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20014.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2001_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20025.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20027.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20028.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20029.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response20031.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response2009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response5001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_inline_response5002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_common_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_domestic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_domestic_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_filter_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_foreign_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_sepa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_payment_order_sepa_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_paymentdomesticcreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_paymentdomesticcreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_paymentforeigncreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_paymentsepacreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_paymentsepacreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_pisp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_pisppaymentdomesticcreate_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_pisppaymentsepacreate_partner_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_source_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_statement_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 10:42:53.000000 creditas-1.0.0.1/test/test_transaction_api.py
```

### Comparing `creditas-1.0.0.0/LICENSE` & `creditas-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/README.md` & `creditas-1.0.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Disclaimer
 
 This code has been autogenerated by [Swagger Codegen](https://github.com/swagger-api/swagger-codegen). I do only minimal changes, like adding this info, adding helper scripts for code generation, or fixing some bugs (if needed). I'm not affiliated with Banka Creditas.
 
 ### Versioning
 
-The package version follows the API version. However, as the autogenerated code may be broken, it is necessary to provide an extended versioning (like `1.0.0.1`), where the last number (`1`) represents a patch to the autogenerated code.
+The package version follows the API version. However, as the autogenerated code or the docs may require fixes, it is necessary to provide an extended versioning (like `1.0.0.1`), where the last number (`1`) represents an additional patch.
 
 Also, surprisingly, **Creditas API versioning does not follow [Semantic Versioning](https://semver.org/)**. E.g. the API version `1.0.1` introduces breaking changes to `1.0.0`. Consider to define the the package version in your requirements like this: `creditas==1.0.0.*`. Then no breaking changes should sneak in, but additional fixes are still allowed.
 
 ### License
 
 From [Swagger Codegen license info](https://github.com/swagger-api/swagger-codegen#license-information-on-generated-code):
 > When code is generated from this project, it shall be considered AS IS and owned by the user of the software. There are no warranties--expressed or implied--for generated code. You can do what you wish with it, and once generated, the code is your responsibility and subject to the licensing terms that you deem appropriate.
@@ -22,15 +22,15 @@
 ## Description
 
 This is specification of the Creditas OpenAPI. It contains definitions of Creditas banking services exposed via API accessible on the internet.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.0
+- Package version: 1.0.0.1
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.creditas.cz/otevrene-bankovnictvi](https://www.creditas.cz/otevrene-bankovnictvi)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `creditas-1.0.0.0/creditas/__init__.py` & `creditas-1.0.0.1/creditas/__init__.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/__init__.py` & `creditas-1.0.0.1/creditas/api/__init__.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/account_api.py` & `creditas-1.0.0.1/creditas/api/account_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/administration_api.py` & `creditas-1.0.0.1/creditas/api/administration_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/aisp_api.py` & `creditas-1.0.0.1/creditas/api/aisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/authorization_api.py` & `creditas-1.0.0.1/creditas/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/balance_api.py` & `creditas-1.0.0.1/creditas/api/balance_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/card_api.py` & `creditas-1.0.0.1/creditas/api/card_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/cisp_api.py` & `creditas-1.0.0.1/creditas/api/cisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/example_api.py` & `creditas-1.0.0.1/creditas/api/example_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/loan_api.py` & `creditas-1.0.0.1/creditas/api/loan_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/payment_api.py` & `creditas-1.0.0.1/creditas/api/payment_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/pisp_api.py` & `creditas-1.0.0.1/creditas/api/pisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/statement_api.py` & `creditas-1.0.0.1/creditas/api/statement_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api/transaction_api.py` & `creditas-1.0.0.1/creditas/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/api_client.py` & `creditas-1.0.0.1/creditas/api_client.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/configuration.py` & `creditas-1.0.0.1/creditas/configuration.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/__init__.py` & `creditas-1.0.0.1/creditas/models/__init__.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_current.py` & `creditas-1.0.0.1/creditas/models/account_current.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_savings.py` & `creditas-1.0.0.1/creditas/models/account_savings.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_statement.py` & `creditas-1.0.0.1/creditas/models/account_statement.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_term_deposit.py` & `creditas-1.0.0.1/creditas/models/account_term_deposit.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_transaction.py` & `creditas-1.0.0.1/creditas/models/account_transaction.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_transaction_filter.py` & `creditas-1.0.0.1/creditas/models/account_transaction_filter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_transaction_filter_partner_account.py` & `creditas-1.0.0.1/creditas/models/account_transaction_filter_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/account_transaction_partner_account.py` & `creditas-1.0.0.1/creditas/models/account_transaction_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/aisp_account.py` & `creditas-1.0.0.1/creditas/models/aisp_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/aisp_account_transaction.py` & `creditas-1.0.0.1/creditas/models/aisp_account_transaction.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/aisp_account_transaction_partner_account.py` & `creditas-1.0.0.1/creditas/models/aisp_account_transaction_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body.py` & `creditas-1.0.0.1/creditas/models/body.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body1.py` & `creditas-1.0.0.1/creditas/models/body1.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body10.py` & `creditas-1.0.0.1/creditas/models/body10.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body11.py` & `creditas-1.0.0.1/creditas/models/body11.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body12.py` & `creditas-1.0.0.1/creditas/models/body12.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body13.py` & `creditas-1.0.0.1/creditas/models/body13.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body14.py` & `creditas-1.0.0.1/creditas/models/body14.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body15.py` & `creditas-1.0.0.1/creditas/models/body15.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body16.py` & `creditas-1.0.0.1/creditas/models/body16.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body17.py` & `creditas-1.0.0.1/creditas/models/body17.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body18.py` & `creditas-1.0.0.1/creditas/models/body18.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body19.py` & `creditas-1.0.0.1/creditas/models/body19.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body2.py` & `creditas-1.0.0.1/creditas/models/body2.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body20.py` & `creditas-1.0.0.1/creditas/models/body20.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body21.py` & `creditas-1.0.0.1/creditas/models/body21.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body22.py` & `creditas-1.0.0.1/creditas/models/body22.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body23.py` & `creditas-1.0.0.1/creditas/models/body23.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body24.py` & `creditas-1.0.0.1/creditas/models/body24.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body25.py` & `creditas-1.0.0.1/creditas/models/body25.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body26.py` & `creditas-1.0.0.1/creditas/models/body26.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body27.py` & `creditas-1.0.0.1/creditas/models/body27.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body28.py` & `creditas-1.0.0.1/creditas/models/body28.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body3.py` & `creditas-1.0.0.1/creditas/models/body3.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body4.py` & `creditas-1.0.0.1/creditas/models/body4.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body5.py` & `creditas-1.0.0.1/creditas/models/body5.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body6.py` & `creditas-1.0.0.1/creditas/models/body6.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body7.py` & `creditas-1.0.0.1/creditas/models/body7.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body8.py` & `creditas-1.0.0.1/creditas/models/body8.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/body9.py` & `creditas-1.0.0.1/creditas/models/body9.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/cispaccountbalancecheck_card.py` & `creditas-1.0.0.1/creditas/models/cispaccountbalancecheck_card.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/clientregistrationcreate_client_application.py` & `creditas-1.0.0.1/creditas/models/clientregistrationcreate_client_application.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/debit_card.py` & `creditas-1.0.0.1/creditas/models/debit_card.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_basic.py` & `creditas-1.0.0.1/creditas/models/error_basic.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_transaction_authorization.py` & `creditas-1.0.0.1/creditas/models/error_transaction_authorization.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_transaction_authorization_data.py` & `creditas-1.0.0.1/creditas/models/error_transaction_authorization_data.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_validation.py` & `creditas-1.0.0.1/creditas/models/error_validation.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_validation_data.py` & `creditas-1.0.0.1/creditas/models/error_validation_data.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_validation_data_parameter.py` & `creditas-1.0.0.1/creditas/models/error_validation_data_parameter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/error_validation_data_validation_result.py` & `creditas-1.0.0.1/creditas/models/error_validation_data_validation_result.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response200.py` & `creditas-1.0.0.1/creditas/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2001.py` & `creditas-1.0.0.1/creditas/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20010.py` & `creditas-1.0.0.1/creditas/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20011.py` & `creditas-1.0.0.1/creditas/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20012.py` & `creditas-1.0.0.1/creditas/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20013.py` & `creditas-1.0.0.1/creditas/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20014.py` & `creditas-1.0.0.1/creditas/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20015.py` & `creditas-1.0.0.1/creditas/models/inline_response20015.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20016.py` & `creditas-1.0.0.1/creditas/models/inline_response20016.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20017.py` & `creditas-1.0.0.1/creditas/models/inline_response20017.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20018.py` & `creditas-1.0.0.1/creditas/models/inline_response20018.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20019.py` & `creditas-1.0.0.1/creditas/models/inline_response20019.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2001_devices.py` & `creditas-1.0.0.1/creditas/models/inline_response2001_devices.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2002.py` & `creditas-1.0.0.1/creditas/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20020.py` & `creditas-1.0.0.1/creditas/models/inline_response20020.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20021.py` & `creditas-1.0.0.1/creditas/models/inline_response20021.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20022.py` & `creditas-1.0.0.1/creditas/models/inline_response20022.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20023.py` & `creditas-1.0.0.1/creditas/models/inline_response20023.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20024.py` & `creditas-1.0.0.1/creditas/models/inline_response20024.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20025.py` & `creditas-1.0.0.1/creditas/models/inline_response20025.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20026.py` & `creditas-1.0.0.1/creditas/models/inline_response20026.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20027.py` & `creditas-1.0.0.1/creditas/models/inline_response20027.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20028.py` & `creditas-1.0.0.1/creditas/models/inline_response20028.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20029.py` & `creditas-1.0.0.1/creditas/models/inline_response20029.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2003.py` & `creditas-1.0.0.1/creditas/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20030.py` & `creditas-1.0.0.1/creditas/models/inline_response20030.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response20031.py` & `creditas-1.0.0.1/creditas/models/inline_response20031.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2004.py` & `creditas-1.0.0.1/creditas/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2005.py` & `creditas-1.0.0.1/creditas/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2006.py` & `creditas-1.0.0.1/creditas/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2007.py` & `creditas-1.0.0.1/creditas/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2008.py` & `creditas-1.0.0.1/creditas/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response2009.py` & `creditas-1.0.0.1/creditas/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response500.py` & `creditas-1.0.0.1/creditas/models/inline_response500.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response5001.py` & `creditas-1.0.0.1/creditas/models/inline_response5001.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/inline_response5002.py` & `creditas-1.0.0.1/creditas/models/inline_response5002.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/loan.py` & `creditas-1.0.0.1/creditas/models/loan.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/money.py` & `creditas-1.0.0.1/creditas/models/money.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_common.py` & `creditas-1.0.0.1/creditas/models/payment_order_common.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_common_partner_account.py` & `creditas-1.0.0.1/creditas/models/payment_order_common_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_domestic.py` & `creditas-1.0.0.1/creditas/models/payment_order_domestic.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_domestic_partner_account.py` & `creditas-1.0.0.1/creditas/models/payment_order_domestic_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_filter.py` & `creditas-1.0.0.1/creditas/models/payment_order_filter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_filter_partner_account.py` & `creditas-1.0.0.1/creditas/models/payment_order_filter_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_foreign.py` & `creditas-1.0.0.1/creditas/models/payment_order_foreign.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_foreign_partner_account.py` & `creditas-1.0.0.1/creditas/models/payment_order_foreign_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_sepa.py` & `creditas-1.0.0.1/creditas/models/payment_order_sepa.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/payment_order_sepa_partner_account.py` & `creditas-1.0.0.1/creditas/models/payment_order_sepa_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/paymentdomesticcreate_partner_account.py` & `creditas-1.0.0.1/creditas/models/paymentdomesticcreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/paymentdomesticcreate_source_account.py` & `creditas-1.0.0.1/creditas/models/paymentdomesticcreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/paymentforeigncreate_partner_account.py` & `creditas-1.0.0.1/creditas/models/paymentforeigncreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/paymentsepacreate_partner_account.py` & `creditas-1.0.0.1/creditas/models/paymentsepacreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/paymentsepacreate_source_account.py` & `creditas-1.0.0.1/creditas/models/paymentsepacreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/pisppaymentdomesticcreate_source_account.py` & `creditas-1.0.0.1/creditas/models/pisppaymentdomesticcreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/pisppaymentsepacreate_partner_account.py` & `creditas-1.0.0.1/creditas/models/pisppaymentsepacreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/models/source_account.py` & `creditas-1.0.0.1/creditas/models/source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas/rest.py` & `creditas-1.0.0.1/creditas/rest.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/creditas.egg-info/SOURCES.txt` & `creditas-1.0.0.1/creditas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/setup.py` & `creditas-1.0.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,39 +8,42 @@
     OpenAPI spec version: 1.0.0
     Contact: is@creditas.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
+from pathlib import Path
 
 NAME = "creditas"
-VERSION = "1.0.0.0"
+VERSION = "1.0.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = [
     "certifi>=2017.4.17",
     "python-dateutil>=2.1",
     "six>=1.10",
     "urllib3>=1.23"
 ]
     
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 
 setup(
     name=NAME,
     version=VERSION,
     description="Creditas OpenAPI",
     author_email="is@creditas.cz",
     url="",
     keywords=["Swagger", "Creditas OpenAPI"],
     install_requires=REQUIRES,
     packages=find_packages(),
     include_package_data=True,
-    long_description="""\
-    This is specification of the Creditas OpenAPI. It contains definitions of Creditas banking services exposed via API accessible on the internet.  # noqa: E501
-    """
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
```

### Comparing `creditas-1.0.0.0/test/test_account_api.py` & `creditas-1.0.0.1/test/test_account_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_current.py` & `creditas-1.0.0.1/test/test_account_current.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_savings.py` & `creditas-1.0.0.1/test/test_account_savings.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_statement.py` & `creditas-1.0.0.1/test/test_account_statement.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_term_deposit.py` & `creditas-1.0.0.1/test/test_account_term_deposit.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_transaction.py` & `creditas-1.0.0.1/test/test_account_transaction.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_transaction_filter.py` & `creditas-1.0.0.1/test/test_account_transaction_filter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_transaction_filter_partner_account.py` & `creditas-1.0.0.1/test/test_account_transaction_filter_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_account_transaction_partner_account.py` & `creditas-1.0.0.1/test/test_account_transaction_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_administration_api.py` & `creditas-1.0.0.1/test/test_administration_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_aisp_account.py` & `creditas-1.0.0.1/test/test_aisp_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_aisp_account_transaction.py` & `creditas-1.0.0.1/test/test_aisp_account_transaction.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_aisp_account_transaction_partner_account.py` & `creditas-1.0.0.1/test/test_aisp_account_transaction_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_aisp_api.py` & `creditas-1.0.0.1/test/test_aisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_authorization_api.py` & `creditas-1.0.0.1/test/test_authorization_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_balance_api.py` & `creditas-1.0.0.1/test/test_balance_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body.py` & `creditas-1.0.0.1/test/test_body.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body1.py` & `creditas-1.0.0.1/test/test_body1.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body10.py` & `creditas-1.0.0.1/test/test_body10.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body11.py` & `creditas-1.0.0.1/test/test_body11.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body12.py` & `creditas-1.0.0.1/test/test_body12.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body13.py` & `creditas-1.0.0.1/test/test_body13.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body14.py` & `creditas-1.0.0.1/test/test_body14.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body15.py` & `creditas-1.0.0.1/test/test_body15.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body16.py` & `creditas-1.0.0.1/test/test_body16.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body17.py` & `creditas-1.0.0.1/test/test_body17.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body18.py` & `creditas-1.0.0.1/test/test_body18.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body19.py` & `creditas-1.0.0.1/test/test_body19.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body2.py` & `creditas-1.0.0.1/test/test_body2.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body20.py` & `creditas-1.0.0.1/test/test_body20.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body21.py` & `creditas-1.0.0.1/test/test_body21.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body22.py` & `creditas-1.0.0.1/test/test_body22.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body23.py` & `creditas-1.0.0.1/test/test_body23.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body24.py` & `creditas-1.0.0.1/test/test_body24.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body25.py` & `creditas-1.0.0.1/test/test_body25.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body26.py` & `creditas-1.0.0.1/test/test_body26.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body27.py` & `creditas-1.0.0.1/test/test_body27.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body28.py` & `creditas-1.0.0.1/test/test_body28.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body3.py` & `creditas-1.0.0.1/test/test_body3.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body4.py` & `creditas-1.0.0.1/test/test_body4.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body5.py` & `creditas-1.0.0.1/test/test_body5.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body6.py` & `creditas-1.0.0.1/test/test_body6.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body7.py` & `creditas-1.0.0.1/test/test_body7.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body8.py` & `creditas-1.0.0.1/test/test_body8.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_body9.py` & `creditas-1.0.0.1/test/test_body9.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_card_api.py` & `creditas-1.0.0.1/test/test_card_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_cisp_api.py` & `creditas-1.0.0.1/test/test_cisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_cispaccountbalancecheck_card.py` & `creditas-1.0.0.1/test/test_cispaccountbalancecheck_card.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_clientregistrationcreate_client_application.py` & `creditas-1.0.0.1/test/test_clientregistrationcreate_client_application.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_debit_card.py` & `creditas-1.0.0.1/test/test_debit_card.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_basic.py` & `creditas-1.0.0.1/test/test_error_basic.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_transaction_authorization.py` & `creditas-1.0.0.1/test/test_error_transaction_authorization.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_transaction_authorization_data.py` & `creditas-1.0.0.1/test/test_error_transaction_authorization_data.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_validation.py` & `creditas-1.0.0.1/test/test_error_validation.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_validation_data.py` & `creditas-1.0.0.1/test/test_error_validation_data.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_validation_data_parameter.py` & `creditas-1.0.0.1/test/test_error_validation_data_parameter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_error_validation_data_validation_result.py` & `creditas-1.0.0.1/test/test_error_validation_data_validation_result.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_example_api.py` & `creditas-1.0.0.1/test/test_example_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response200.py` & `creditas-1.0.0.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2001.py` & `creditas-1.0.0.1/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20010.py` & `creditas-1.0.0.1/test/test_inline_response20010.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20011.py` & `creditas-1.0.0.1/test/test_inline_response20011.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20012.py` & `creditas-1.0.0.1/test/test_inline_response20012.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20013.py` & `creditas-1.0.0.1/test/test_inline_response20013.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20014.py` & `creditas-1.0.0.1/test/test_inline_response20014.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20015.py` & `creditas-1.0.0.1/test/test_inline_response20015.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20016.py` & `creditas-1.0.0.1/test/test_inline_response20016.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20017.py` & `creditas-1.0.0.1/test/test_inline_response20017.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20018.py` & `creditas-1.0.0.1/test/test_inline_response20018.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20019.py` & `creditas-1.0.0.1/test/test_inline_response20019.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2001_devices.py` & `creditas-1.0.0.1/test/test_inline_response2001_devices.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2002.py` & `creditas-1.0.0.1/test/test_inline_response2002.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20020.py` & `creditas-1.0.0.1/test/test_inline_response20020.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20021.py` & `creditas-1.0.0.1/test/test_inline_response20021.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20022.py` & `creditas-1.0.0.1/test/test_inline_response20022.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20023.py` & `creditas-1.0.0.1/test/test_inline_response20023.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20024.py` & `creditas-1.0.0.1/test/test_inline_response20024.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20025.py` & `creditas-1.0.0.1/test/test_inline_response20025.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20026.py` & `creditas-1.0.0.1/test/test_inline_response20026.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20027.py` & `creditas-1.0.0.1/test/test_inline_response20027.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20028.py` & `creditas-1.0.0.1/test/test_inline_response20028.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20029.py` & `creditas-1.0.0.1/test/test_inline_response20029.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2003.py` & `creditas-1.0.0.1/test/test_inline_response2003.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20030.py` & `creditas-1.0.0.1/test/test_inline_response20030.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response20031.py` & `creditas-1.0.0.1/test/test_inline_response20031.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2004.py` & `creditas-1.0.0.1/test/test_inline_response2004.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2005.py` & `creditas-1.0.0.1/test/test_inline_response2005.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2006.py` & `creditas-1.0.0.1/test/test_inline_response2006.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2007.py` & `creditas-1.0.0.1/test/test_inline_response2007.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2008.py` & `creditas-1.0.0.1/test/test_inline_response2008.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response2009.py` & `creditas-1.0.0.1/test/test_inline_response2009.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response500.py` & `creditas-1.0.0.1/test/test_inline_response500.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response5001.py` & `creditas-1.0.0.1/test/test_inline_response5001.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_inline_response5002.py` & `creditas-1.0.0.1/test/test_inline_response5002.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_loan.py` & `creditas-1.0.0.1/test/test_loan.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_loan_api.py` & `creditas-1.0.0.1/test/test_loan_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_money.py` & `creditas-1.0.0.1/test/test_money.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_api.py` & `creditas-1.0.0.1/test/test_payment_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_common.py` & `creditas-1.0.0.1/test/test_payment_order_common.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_common_partner_account.py` & `creditas-1.0.0.1/test/test_payment_order_common_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_domestic.py` & `creditas-1.0.0.1/test/test_payment_order_domestic.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_domestic_partner_account.py` & `creditas-1.0.0.1/test/test_payment_order_domestic_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_filter.py` & `creditas-1.0.0.1/test/test_payment_order_filter.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_filter_partner_account.py` & `creditas-1.0.0.1/test/test_payment_order_filter_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_foreign.py` & `creditas-1.0.0.1/test/test_payment_order_foreign.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_foreign_partner_account.py` & `creditas-1.0.0.1/test/test_payment_order_foreign_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_sepa.py` & `creditas-1.0.0.1/test/test_payment_order_sepa.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_payment_order_sepa_partner_account.py` & `creditas-1.0.0.1/test/test_payment_order_sepa_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_paymentdomesticcreate_partner_account.py` & `creditas-1.0.0.1/test/test_paymentdomesticcreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_paymentdomesticcreate_source_account.py` & `creditas-1.0.0.1/test/test_paymentdomesticcreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_paymentforeigncreate_partner_account.py` & `creditas-1.0.0.1/test/test_paymentforeigncreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_paymentsepacreate_partner_account.py` & `creditas-1.0.0.1/test/test_paymentsepacreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_paymentsepacreate_source_account.py` & `creditas-1.0.0.1/test/test_paymentsepacreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_pisp_api.py` & `creditas-1.0.0.1/test/test_pisp_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_pisppaymentdomesticcreate_source_account.py` & `creditas-1.0.0.1/test/test_pisppaymentdomesticcreate_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_pisppaymentsepacreate_partner_account.py` & `creditas-1.0.0.1/test/test_pisppaymentsepacreate_partner_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_source_account.py` & `creditas-1.0.0.1/test/test_source_account.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_statement_api.py` & `creditas-1.0.0.1/test/test_statement_api.py`

 * *Files identical despite different names*

### Comparing `creditas-1.0.0.0/test/test_transaction_api.py` & `creditas-1.0.0.1/test/test_transaction_api.py`

 * *Files identical despite different names*

