# Comparing `tmp/conekta-6.0.0.tar.gz` & `tmp/conekta-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conekta-6.0.0.tar", last modified: Fri Jun  9 16:02:01 2023, max compression
+gzip compressed data, was "conekta-6.0.1.tar", last modified: Fri Jul  7 16:46:13 2023, max compression
```

## Comparing `conekta-6.0.0.tar` & `conekta-6.0.1.tar`

### file list

```diff
@@ -1,268 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-09 16:01:51.000000 conekta-6.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 16:01:51.000000 conekta-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 16:01:51.000000 conekta-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27601 2023-06-09 16:02:01.189855 conekta-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26852 2023-06-09 16:01:51.000000 conekta-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.157855 conekta-6.0.0/conekta/
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.161855 conekta-6.0.0/conekta/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43665 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/antifraud_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40760 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/charges_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/companies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    63028 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/customers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28260 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/discounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25270 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/logs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    67602 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    51140 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/payment_link_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38951 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/payment_methods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41008 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27109 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/products_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28786 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/shipping_contacts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/shippings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57213 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/subscriptions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27176 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/taxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/webhook_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47871 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30526 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/conekta/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_create_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_create_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/blacklist_rule_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_bank_transfer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_cash_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_order_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_order_response_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_request_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charges_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_order_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_order_template_customer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkouts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkouts_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_fiscal_info_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_fiscal_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_payout_destination_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_payment_methods_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_payment_methods_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_risk_rules_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_antifraud_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_antifraud_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_request_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_just_customer_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_just_customer_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_method_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response_shipping_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response_shipping_contacts_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_response_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_update_fiscal_entities_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_update_shipping_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customers_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/delete_api_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/delete_api_keys_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/deleted_blacklist_rule_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/deleted_whitelist_rule_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/details_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/email_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/error_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/events_resend_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_api_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_api_keys_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_charges_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_charges_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_companies_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_companies_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_customer_payment_method_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_events_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_orders_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_payment_method_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_plans_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_plans_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transactions_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transfers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transfers_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhook_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhook_keys_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhooks_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhooks_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/log_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/logs_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_capture_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_discount_lines_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_refund_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_request_customer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_charges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_charges_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_customer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_customer_info_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_discount_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_discount_lines_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity_address_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_products_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_shipping_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_shipping_contact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_tax_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/orders_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_bank_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_recurrent_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_data_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_order_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_order_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/shipping_order_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/shipping_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/sms_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_response_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_destination_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_method_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_antifraud_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_payment_methods_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_discount_lines_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_payment_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_create_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/whitelistlist_rule_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.161855 conekta-6.0.0/conekta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27601 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 16:01:51.000000 conekta-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 16:02:01.193856 conekta-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-09 16:01:51.000000 conekta-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_antifraud_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_charges_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_companies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_customers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_discounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_payment_link_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_payment_methods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_products_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_shipping_contacts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_shippings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_subscriptions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_taxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_webhook_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_webhooks_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.150551 conekta-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-07 16:46:02.000000 conekta-6.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 16:46:02.000000 conekta-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 16:46:02.000000 conekta-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-07-07 16:46:13.150551 conekta-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-07-07 16:46:02.000000 conekta-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.110548 conekta-6.0.1/conekta/
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.118548 conekta-6.0.1/conekta/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43665 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/antifraud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40748 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/balances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/charges_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63028 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/customers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46902 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/discounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25270 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67602 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51140 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/payment_link_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38951 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41008 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27109 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/products_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28786 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/shipping_contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27258 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/shippings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57213 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/subscriptions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27176 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/webhook_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47871 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30526 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.150551 conekta-6.0.1/conekta/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_create_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_response_on_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/api_key_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/balance_common_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/blacklist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_data_payment_method_bank_transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_data_payment_method_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_data_payment_method_cash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_order_response_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_request_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response_refunds_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charge_response_refunds_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/charges_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkout_order_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkout_order_template_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkouts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/checkouts_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/company_fiscal_info_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/company_fiscal_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/company_payout_destination_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/create_customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/create_customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/create_customer_payment_methods_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/create_customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/create_risk_rules_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_antifraud_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_antifraud_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_fiscal_entities_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_fiscal_entities_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_fiscal_entities_request_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_info_just_customer_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_info_just_customer_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_payment_methods_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_payment_methods_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_response_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_response_shipping_contacts_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts_data_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_shipping_contacts_response_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_update_fiscal_entities_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customer_update_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/customers_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/delete_api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/delete_api_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/deleted_blacklist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/deleted_whitelist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/details_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/discount_lines_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/discount_lines_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/discount_lines_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/email_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/error_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/events_resend_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_api_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_charges_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_charges_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_companies_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_companies_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_customer_payment_method_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_events_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_order_discount_lines_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_order_discount_lines_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_orders_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_payment_method_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_plans_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_plans_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_transactions_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_transfers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_transfers_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_webhook_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_webhook_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_webhooks_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/get_webhooks_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/logs_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_capture_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_discount_lines_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_refund_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_request_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_charges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_charges_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_customer_info_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_discount_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_discount_lines_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_fiscal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_fiscal_entity_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_fiscal_entity_address_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_products_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_shipping_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_response_shipping_contact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_tax_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/order_update_request_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/orders_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_bank_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_card_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_card_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_cash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_cash_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_cash_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_cash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_cash_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_spei_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_spei_recurrent_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/payment_method_spei_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/plan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/plan_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/product_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/product_data_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/product_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/product_order_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/risk_rules_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/risk_rules_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/shipping_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/shipping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/sms_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/subscription_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/subscription_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/subscription_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/subscription_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/token_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/token_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/token_response_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/transfer_destination_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/transfer_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/transfers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_customer_antifraud_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_order_discount_lines_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_order_tax_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_order_tax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_order_tax_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/update_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_key_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_key_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_key_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/models/whitelistlist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-07 16:46:02.000000 conekta-6.0.1/conekta/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.114548 conekta-6.0.1/conekta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-07-07 16:46:13.000000 conekta-6.0.1/conekta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-07 16:46:13.000000 conekta-6.0.1/conekta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:46:13.000000 conekta-6.0.1/conekta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 16:46:13.000000 conekta-6.0.1/conekta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 16:46:13.000000 conekta-6.0.1/conekta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 16:46:02.000000 conekta-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 16:46:13.154552 conekta-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 16:46:02.000000 conekta-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:46:13.150551 conekta-6.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_antifraud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_balances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_charges_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_customers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_discounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_payment_link_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_products_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_shipping_contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_shippings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_subscriptions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_webhook_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-07 16:46:02.000000 conekta-6.0.1/test/test_webhooks_api.py
```

### Comparing `conekta-6.0.0/AUTHORS.md` & `conekta-6.0.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/LICENSE` & `conekta-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/PKG-INFO` & `conekta-6.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-Metadata-Version: 2.1
-Name: conekta
-Version: 6.0.0
-Summary: This is a Python library that allows interaction with https://api.conekta.io API.
-Home-page: https://github.com/conekta/conekta-python
-Author: Engineering Conekta
-Author-email: Engineering Conekta <engineering@conekta.com>
-License: MIT-LICENSE
-Project-URL: Homepage, https://github.com/conekta/conekta-python
-Project-URL: Bug Tracker, https://github.com/conekta/conekta-python/issues
-Keywords: OpenAPI,OpenAPI-Generator,Conekta API
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # conekta
 Conekta sdk
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2.1.0
-- Package version: 6.0.0
+- Package version: 6.0.1
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://github.com/conekta/openapi/issues](https://github.com/conekta/openapi/issues)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -120,27 +101,30 @@
 *AntifraudApi* | [**get_rule_blacklist**](docs/AntifraudApi.md#get_rule_blacklist) | **GET** /antifraud/blacklists | Get list of blacklisted rules
 *AntifraudApi* | [**get_rule_whitelist**](docs/AntifraudApi.md#get_rule_whitelist) | **GET** /antifraud/whitelists | Get a list of whitelisted rules
 *ApiKeysApi* | [**create_api_key**](docs/ApiKeysApi.md#create_api_key) | **POST** /api_keys | Create Api Key
 *ApiKeysApi* | [**delete_api_key**](docs/ApiKeysApi.md#delete_api_key) | **DELETE** /api_keys/{id} | Delete Api Key
 *ApiKeysApi* | [**get_api_key**](docs/ApiKeysApi.md#get_api_key) | **GET** /api_keys/{id} | Get Api Key
 *ApiKeysApi* | [**get_api_keys**](docs/ApiKeysApi.md#get_api_keys) | **GET** /api_keys | Get list of Api Keys
 *ApiKeysApi* | [**update_api_key**](docs/ApiKeysApi.md#update_api_key) | **PUT** /api_keys/{id} | Update Api Key
+*BalancesApi* | [**get_balance**](docs/BalancesApi.md#get_balance) | **GET** /balances | Get a company&#39;s balance
 *ChargesApi* | [**get_charges**](docs/ChargesApi.md#get_charges) | **GET** /charges | Get A List of Charges
 *ChargesApi* | [**orders_create_charge**](docs/ChargesApi.md#orders_create_charge) | **POST** /orders/{id}/charges | Create charge
 *CompaniesApi* | [**get_companies**](docs/CompaniesApi.md#get_companies) | **GET** /companies | Get List of Companies
 *CompaniesApi* | [**get_company**](docs/CompaniesApi.md#get_company) | **GET** /companies/{id} | Get Company
 *CustomersApi* | [**create_customer**](docs/CustomersApi.md#create_customer) | **POST** /customers | Create customer
 *CustomersApi* | [**create_customer_fiscal_entities**](docs/CustomersApi.md#create_customer_fiscal_entities) | **POST** /customers/{id}/fiscal_entities | Create Fiscal Entity
 *CustomersApi* | [**delete_customer_by_id**](docs/CustomersApi.md#delete_customer_by_id) | **DELETE** /customers/{id} | Delete Customer
 *CustomersApi* | [**get_customer_by_id**](docs/CustomersApi.md#get_customer_by_id) | **GET** /customers/{id} | Get Customer
 *CustomersApi* | [**get_customers**](docs/CustomersApi.md#get_customers) | **GET** /customers | Get a list of customers
 *CustomersApi* | [**update_customer**](docs/CustomersApi.md#update_customer) | **PUT** /customers/{id} | Update customer
 *CustomersApi* | [**update_customer_fiscal_entities**](docs/CustomersApi.md#update_customer_fiscal_entities) | **PUT** /customers/{id}/fiscal_entities/{fiscal_entities_id} | Update  Fiscal Entity
 *DiscountsApi* | [**orders_create_discount_line**](docs/DiscountsApi.md#orders_create_discount_line) | **POST** /orders/{id}/discount_lines | Create Discount
 *DiscountsApi* | [**orders_delete_discount_lines**](docs/DiscountsApi.md#orders_delete_discount_lines) | **DELETE** /orders/{id}/discount_lines/{discount_lines_id} | Delete Discount
+*DiscountsApi* | [**orders_get_discount_line**](docs/DiscountsApi.md#orders_get_discount_line) | **GET** /orders/{id}/discount_lines/{discount_lines_id} | Get Discount
+*DiscountsApi* | [**orders_get_discount_lines**](docs/DiscountsApi.md#orders_get_discount_lines) | **GET** /orders/{id}/discount_lines | Get a List of Discount
 *DiscountsApi* | [**orders_update_discount_lines**](docs/DiscountsApi.md#orders_update_discount_lines) | **PUT** /orders/{id}/discount_lines/{discount_lines_id} | Update Discount
 *EventsApi* | [**get_event**](docs/EventsApi.md#get_event) | **GET** /events/{id} | Get Event
 *EventsApi* | [**get_events**](docs/EventsApi.md#get_events) | **GET** /events | Get list of Events
 *EventsApi* | [**resend_event**](docs/EventsApi.md#resend_event) | **POST** /events/{event_id}/webhook_logs/{webhook_log_id}/resend | Resend Event
 *LogsApi* | [**get_log_by_id**](docs/LogsApi.md#get_log_by_id) | **GET** /logs/{id} | Get Log
 *LogsApi* | [**get_logs**](docs/LogsApi.md#get_logs) | **GET** /logs | Get List Of Logs
 *OrdersApi* | [**cancel_order**](docs/OrdersApi.md#cancel_order) | **POST** /orders/{id}/cancel | Cancel Order
@@ -205,15 +189,18 @@
 
 ## Documentation For Models
 
  - [ApiKeyCreateResponse](docs/ApiKeyCreateResponse.md)
  - [ApiKeyCreateResponseAllOf](docs/ApiKeyCreateResponseAllOf.md)
  - [ApiKeyRequest](docs/ApiKeyRequest.md)
  - [ApiKeyResponse](docs/ApiKeyResponse.md)
+ - [ApiKeyResponseOnDelete](docs/ApiKeyResponseOnDelete.md)
  - [ApiKeyUpdateRequest](docs/ApiKeyUpdateRequest.md)
+ - [BalanceCommonField](docs/BalanceCommonField.md)
+ - [BalanceResponse](docs/BalanceResponse.md)
  - [BlacklistRuleResponse](docs/BlacklistRuleResponse.md)
  - [ChargeDataPaymentMethodBankTransferResponse](docs/ChargeDataPaymentMethodBankTransferResponse.md)
  - [ChargeDataPaymentMethodCardResponse](docs/ChargeDataPaymentMethodCardResponse.md)
  - [ChargeDataPaymentMethodCashResponse](docs/ChargeDataPaymentMethodCashResponse.md)
  - [ChargeOrderResponse](docs/ChargeOrderResponse.md)
  - [ChargeOrderResponsePaymentMethod](docs/ChargeOrderResponsePaymentMethod.md)
  - [ChargeRequest](docs/ChargeRequest.md)
@@ -291,14 +278,16 @@
  - [GetChargesResponse](docs/GetChargesResponse.md)
  - [GetChargesResponseAllOf](docs/GetChargesResponseAllOf.md)
  - [GetCompaniesResponse](docs/GetCompaniesResponse.md)
  - [GetCompaniesResponseAllOf](docs/GetCompaniesResponseAllOf.md)
  - [GetCustomerPaymentMethodDataResponse](docs/GetCustomerPaymentMethodDataResponse.md)
  - [GetEventsResponse](docs/GetEventsResponse.md)
  - [GetEventsResponseAllOf](docs/GetEventsResponseAllOf.md)
+ - [GetOrderDiscountLinesResponse](docs/GetOrderDiscountLinesResponse.md)
+ - [GetOrderDiscountLinesResponseAllOf](docs/GetOrderDiscountLinesResponseAllOf.md)
  - [GetOrdersResponse](docs/GetOrdersResponse.md)
  - [GetPaymentMethodResponse](docs/GetPaymentMethodResponse.md)
  - [GetPaymentMethodResponseAllOf](docs/GetPaymentMethodResponseAllOf.md)
  - [GetPlansResponse](docs/GetPlansResponse.md)
  - [GetPlansResponseAllOf](docs/GetPlansResponseAllOf.md)
  - [GetTransactionsResponse](docs/GetTransactionsResponse.md)
  - [GetTransactionsResponseAllOf](docs/GetTransactionsResponseAllOf.md)
@@ -329,14 +318,15 @@
  - [OrderResponseFiscalEntityAddressAllOf](docs/OrderResponseFiscalEntityAddressAllOf.md)
  - [OrderResponseProducts](docs/OrderResponseProducts.md)
  - [OrderResponseProductsAllOf](docs/OrderResponseProductsAllOf.md)
  - [OrderResponseShippingContact](docs/OrderResponseShippingContact.md)
  - [OrderResponseShippingContactAllOf](docs/OrderResponseShippingContactAllOf.md)
  - [OrderTaxRequest](docs/OrderTaxRequest.md)
  - [OrderUpdateRequest](docs/OrderUpdateRequest.md)
+ - [OrderUpdateRequestCustomerInfo](docs/OrderUpdateRequestCustomerInfo.md)
  - [OrdersResponse](docs/OrdersResponse.md)
  - [Page](docs/Page.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodBankTransfer](docs/PaymentMethodBankTransfer.md)
  - [PaymentMethodCard](docs/PaymentMethodCard.md)
  - [PaymentMethodCardRequest](docs/PaymentMethodCardRequest.md)
```

### Comparing `conekta-6.0.0/README.md` & `conekta-6.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+Metadata-Version: 2.1
+Name: conekta
+Version: 6.0.1
+Summary: This is a Python library that allows interaction with https://api.conekta.io API.
+Home-page: https://github.com/conekta/conekta-python
+Author: Engineering Conekta
+Author-email: Engineering Conekta <engineering@conekta.com>
+License: MIT-LICENSE
+Project-URL: Homepage, https://github.com/conekta/conekta-python
+Project-URL: Bug Tracker, https://github.com/conekta/conekta-python/issues
+Keywords: OpenAPI,OpenAPI-Generator,Conekta API
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
 # conekta
 Conekta sdk
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2.1.0
-- Package version: 6.0.0
+- Package version: 6.0.1
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://github.com/conekta/openapi/issues](https://github.com/conekta/openapi/issues)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -101,27 +120,30 @@
 *AntifraudApi* | [**get_rule_blacklist**](docs/AntifraudApi.md#get_rule_blacklist) | **GET** /antifraud/blacklists | Get list of blacklisted rules
 *AntifraudApi* | [**get_rule_whitelist**](docs/AntifraudApi.md#get_rule_whitelist) | **GET** /antifraud/whitelists | Get a list of whitelisted rules
 *ApiKeysApi* | [**create_api_key**](docs/ApiKeysApi.md#create_api_key) | **POST** /api_keys | Create Api Key
 *ApiKeysApi* | [**delete_api_key**](docs/ApiKeysApi.md#delete_api_key) | **DELETE** /api_keys/{id} | Delete Api Key
 *ApiKeysApi* | [**get_api_key**](docs/ApiKeysApi.md#get_api_key) | **GET** /api_keys/{id} | Get Api Key
 *ApiKeysApi* | [**get_api_keys**](docs/ApiKeysApi.md#get_api_keys) | **GET** /api_keys | Get list of Api Keys
 *ApiKeysApi* | [**update_api_key**](docs/ApiKeysApi.md#update_api_key) | **PUT** /api_keys/{id} | Update Api Key
+*BalancesApi* | [**get_balance**](docs/BalancesApi.md#get_balance) | **GET** /balances | Get a company&#39;s balance
 *ChargesApi* | [**get_charges**](docs/ChargesApi.md#get_charges) | **GET** /charges | Get A List of Charges
 *ChargesApi* | [**orders_create_charge**](docs/ChargesApi.md#orders_create_charge) | **POST** /orders/{id}/charges | Create charge
 *CompaniesApi* | [**get_companies**](docs/CompaniesApi.md#get_companies) | **GET** /companies | Get List of Companies
 *CompaniesApi* | [**get_company**](docs/CompaniesApi.md#get_company) | **GET** /companies/{id} | Get Company
 *CustomersApi* | [**create_customer**](docs/CustomersApi.md#create_customer) | **POST** /customers | Create customer
 *CustomersApi* | [**create_customer_fiscal_entities**](docs/CustomersApi.md#create_customer_fiscal_entities) | **POST** /customers/{id}/fiscal_entities | Create Fiscal Entity
 *CustomersApi* | [**delete_customer_by_id**](docs/CustomersApi.md#delete_customer_by_id) | **DELETE** /customers/{id} | Delete Customer
 *CustomersApi* | [**get_customer_by_id**](docs/CustomersApi.md#get_customer_by_id) | **GET** /customers/{id} | Get Customer
 *CustomersApi* | [**get_customers**](docs/CustomersApi.md#get_customers) | **GET** /customers | Get a list of customers
 *CustomersApi* | [**update_customer**](docs/CustomersApi.md#update_customer) | **PUT** /customers/{id} | Update customer
 *CustomersApi* | [**update_customer_fiscal_entities**](docs/CustomersApi.md#update_customer_fiscal_entities) | **PUT** /customers/{id}/fiscal_entities/{fiscal_entities_id} | Update  Fiscal Entity
 *DiscountsApi* | [**orders_create_discount_line**](docs/DiscountsApi.md#orders_create_discount_line) | **POST** /orders/{id}/discount_lines | Create Discount
 *DiscountsApi* | [**orders_delete_discount_lines**](docs/DiscountsApi.md#orders_delete_discount_lines) | **DELETE** /orders/{id}/discount_lines/{discount_lines_id} | Delete Discount
+*DiscountsApi* | [**orders_get_discount_line**](docs/DiscountsApi.md#orders_get_discount_line) | **GET** /orders/{id}/discount_lines/{discount_lines_id} | Get Discount
+*DiscountsApi* | [**orders_get_discount_lines**](docs/DiscountsApi.md#orders_get_discount_lines) | **GET** /orders/{id}/discount_lines | Get a List of Discount
 *DiscountsApi* | [**orders_update_discount_lines**](docs/DiscountsApi.md#orders_update_discount_lines) | **PUT** /orders/{id}/discount_lines/{discount_lines_id} | Update Discount
 *EventsApi* | [**get_event**](docs/EventsApi.md#get_event) | **GET** /events/{id} | Get Event
 *EventsApi* | [**get_events**](docs/EventsApi.md#get_events) | **GET** /events | Get list of Events
 *EventsApi* | [**resend_event**](docs/EventsApi.md#resend_event) | **POST** /events/{event_id}/webhook_logs/{webhook_log_id}/resend | Resend Event
 *LogsApi* | [**get_log_by_id**](docs/LogsApi.md#get_log_by_id) | **GET** /logs/{id} | Get Log
 *LogsApi* | [**get_logs**](docs/LogsApi.md#get_logs) | **GET** /logs | Get List Of Logs
 *OrdersApi* | [**cancel_order**](docs/OrdersApi.md#cancel_order) | **POST** /orders/{id}/cancel | Cancel Order
@@ -186,15 +208,18 @@
 
 ## Documentation For Models
 
  - [ApiKeyCreateResponse](docs/ApiKeyCreateResponse.md)
  - [ApiKeyCreateResponseAllOf](docs/ApiKeyCreateResponseAllOf.md)
  - [ApiKeyRequest](docs/ApiKeyRequest.md)
  - [ApiKeyResponse](docs/ApiKeyResponse.md)
+ - [ApiKeyResponseOnDelete](docs/ApiKeyResponseOnDelete.md)
  - [ApiKeyUpdateRequest](docs/ApiKeyUpdateRequest.md)
+ - [BalanceCommonField](docs/BalanceCommonField.md)
+ - [BalanceResponse](docs/BalanceResponse.md)
  - [BlacklistRuleResponse](docs/BlacklistRuleResponse.md)
  - [ChargeDataPaymentMethodBankTransferResponse](docs/ChargeDataPaymentMethodBankTransferResponse.md)
  - [ChargeDataPaymentMethodCardResponse](docs/ChargeDataPaymentMethodCardResponse.md)
  - [ChargeDataPaymentMethodCashResponse](docs/ChargeDataPaymentMethodCashResponse.md)
  - [ChargeOrderResponse](docs/ChargeOrderResponse.md)
  - [ChargeOrderResponsePaymentMethod](docs/ChargeOrderResponsePaymentMethod.md)
  - [ChargeRequest](docs/ChargeRequest.md)
@@ -272,14 +297,16 @@
  - [GetChargesResponse](docs/GetChargesResponse.md)
  - [GetChargesResponseAllOf](docs/GetChargesResponseAllOf.md)
  - [GetCompaniesResponse](docs/GetCompaniesResponse.md)
  - [GetCompaniesResponseAllOf](docs/GetCompaniesResponseAllOf.md)
  - [GetCustomerPaymentMethodDataResponse](docs/GetCustomerPaymentMethodDataResponse.md)
  - [GetEventsResponse](docs/GetEventsResponse.md)
  - [GetEventsResponseAllOf](docs/GetEventsResponseAllOf.md)
+ - [GetOrderDiscountLinesResponse](docs/GetOrderDiscountLinesResponse.md)
+ - [GetOrderDiscountLinesResponseAllOf](docs/GetOrderDiscountLinesResponseAllOf.md)
  - [GetOrdersResponse](docs/GetOrdersResponse.md)
  - [GetPaymentMethodResponse](docs/GetPaymentMethodResponse.md)
  - [GetPaymentMethodResponseAllOf](docs/GetPaymentMethodResponseAllOf.md)
  - [GetPlansResponse](docs/GetPlansResponse.md)
  - [GetPlansResponseAllOf](docs/GetPlansResponseAllOf.md)
  - [GetTransactionsResponse](docs/GetTransactionsResponse.md)
  - [GetTransactionsResponseAllOf](docs/GetTransactionsResponseAllOf.md)
@@ -310,14 +337,15 @@
  - [OrderResponseFiscalEntityAddressAllOf](docs/OrderResponseFiscalEntityAddressAllOf.md)
  - [OrderResponseProducts](docs/OrderResponseProducts.md)
  - [OrderResponseProductsAllOf](docs/OrderResponseProductsAllOf.md)
  - [OrderResponseShippingContact](docs/OrderResponseShippingContact.md)
  - [OrderResponseShippingContactAllOf](docs/OrderResponseShippingContactAllOf.md)
  - [OrderTaxRequest](docs/OrderTaxRequest.md)
  - [OrderUpdateRequest](docs/OrderUpdateRequest.md)
+ - [OrderUpdateRequestCustomerInfo](docs/OrderUpdateRequestCustomerInfo.md)
  - [OrdersResponse](docs/OrdersResponse.md)
  - [Page](docs/Page.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodBankTransfer](docs/PaymentMethodBankTransfer.md)
  - [PaymentMethodCard](docs/PaymentMethodCard.md)
  - [PaymentMethodCardRequest](docs/PaymentMethodCardRequest.md)
```

### Comparing `conekta-6.0.0/conekta/__init__.py` & `conekta-6.0.1/conekta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     Contact: engineering@conekta.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "6.0.0"
+__version__ = "6.0.1"
 
 # import apis into sdk package
 from conekta.api.antifraud_api import AntifraudApi
 from conekta.api.api_keys_api import ApiKeysApi
+from conekta.api.balances_api import BalancesApi
 from conekta.api.charges_api import ChargesApi
 from conekta.api.companies_api import CompaniesApi
 from conekta.api.customers_api import CustomersApi
 from conekta.api.discounts_api import DiscountsApi
 from conekta.api.events_api import EventsApi
 from conekta.api.logs_api import LogsApi
 from conekta.api.orders_api import OrdersApi
@@ -53,15 +54,18 @@
 from conekta.exceptions import ApiException
 
 # import models into sdk package
 from conekta.models.api_key_create_response import ApiKeyCreateResponse
 from conekta.models.api_key_create_response_all_of import ApiKeyCreateResponseAllOf
 from conekta.models.api_key_request import ApiKeyRequest
 from conekta.models.api_key_response import ApiKeyResponse
+from conekta.models.api_key_response_on_delete import ApiKeyResponseOnDelete
 from conekta.models.api_key_update_request import ApiKeyUpdateRequest
+from conekta.models.balance_common_field import BalanceCommonField
+from conekta.models.balance_response import BalanceResponse
 from conekta.models.blacklist_rule_response import BlacklistRuleResponse
 from conekta.models.charge_data_payment_method_bank_transfer_response import ChargeDataPaymentMethodBankTransferResponse
 from conekta.models.charge_data_payment_method_card_response import ChargeDataPaymentMethodCardResponse
 from conekta.models.charge_data_payment_method_cash_response import ChargeDataPaymentMethodCashResponse
 from conekta.models.charge_order_response import ChargeOrderResponse
 from conekta.models.charge_order_response_payment_method import ChargeOrderResponsePaymentMethod
 from conekta.models.charge_request import ChargeRequest
@@ -139,14 +143,16 @@
 from conekta.models.get_charges_response import GetChargesResponse
 from conekta.models.get_charges_response_all_of import GetChargesResponseAllOf
 from conekta.models.get_companies_response import GetCompaniesResponse
 from conekta.models.get_companies_response_all_of import GetCompaniesResponseAllOf
 from conekta.models.get_customer_payment_method_data_response import GetCustomerPaymentMethodDataResponse
 from conekta.models.get_events_response import GetEventsResponse
 from conekta.models.get_events_response_all_of import GetEventsResponseAllOf
+from conekta.models.get_order_discount_lines_response import GetOrderDiscountLinesResponse
+from conekta.models.get_order_discount_lines_response_all_of import GetOrderDiscountLinesResponseAllOf
 from conekta.models.get_orders_response import GetOrdersResponse
 from conekta.models.get_payment_method_response import GetPaymentMethodResponse
 from conekta.models.get_payment_method_response_all_of import GetPaymentMethodResponseAllOf
 from conekta.models.get_plans_response import GetPlansResponse
 from conekta.models.get_plans_response_all_of import GetPlansResponseAllOf
 from conekta.models.get_transactions_response import GetTransactionsResponse
 from conekta.models.get_transactions_response_all_of import GetTransactionsResponseAllOf
@@ -177,14 +183,15 @@
 from conekta.models.order_response_fiscal_entity_address_all_of import OrderResponseFiscalEntityAddressAllOf
 from conekta.models.order_response_products import OrderResponseProducts
 from conekta.models.order_response_products_all_of import OrderResponseProductsAllOf
 from conekta.models.order_response_shipping_contact import OrderResponseShippingContact
 from conekta.models.order_response_shipping_contact_all_of import OrderResponseShippingContactAllOf
 from conekta.models.order_tax_request import OrderTaxRequest
 from conekta.models.order_update_request import OrderUpdateRequest
+from conekta.models.order_update_request_customer_info import OrderUpdateRequestCustomerInfo
 from conekta.models.orders_response import OrdersResponse
 from conekta.models.page import Page
 from conekta.models.pagination import Pagination
 from conekta.models.payment_method import PaymentMethod
 from conekta.models.payment_method_bank_transfer import PaymentMethodBankTransfer
 from conekta.models.payment_method_card import PaymentMethodCard
 from conekta.models.payment_method_card_request import PaymentMethodCardRequest
```

### Comparing `conekta-6.0.0/conekta/api/__init__.py` & `conekta-6.0.1/conekta/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 
 # import apis into api package
 from conekta.api.antifraud_api import AntifraudApi
 from conekta.api.api_keys_api import ApiKeysApi
+from conekta.api.balances_api import BalancesApi
 from conekta.api.charges_api import ChargesApi
 from conekta.api.companies_api import CompaniesApi
 from conekta.api.customers_api import CustomersApi
 from conekta.api.discounts_api import DiscountsApi
 from conekta.api.events_api import EventsApi
 from conekta.api.logs_api import LogsApi
 from conekta.api.orders_api import OrdersApi
```

### Comparing `conekta-6.0.0/conekta/api/antifraud_api.py` & `conekta-6.0.1/conekta/api/antifraud_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/api_keys_api.py` & `conekta-6.0.1/conekta/api/api_keys_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,75 +521,75 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_api_keys(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, search : Annotated[Optional[StrictStr], Field(description="General order search, e.g. by mail, reference etc.")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, **kwargs) -> GetApiKeysResponse:  # noqa: E501
+    def get_api_keys(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, search : Annotated[Optional[StrictStr], Field(description="General search, e.g. by id, description, prefix")] = None, **kwargs) -> GetApiKeysResponse:  # noqa: E501
         """Get list of Api Keys  # noqa: E501
 
         Consume the list of api keys you have  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_api_keys(accept_language, x_child_company_id, limit, search, next, previous, async_req=True)
+        >>> thread = api.get_api_keys(accept_language, x_child_company_id, limit, next, previous, search, async_req=True)
         >>> result = thread.get()
 
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param limit: The numbers of items to return, the maximum value is 250
         :type limit: int
-        :param search: General order search, e.g. by mail, reference etc.
-        :type search: str
         :param next: next page
         :type next: str
         :param previous: previous page
         :type previous: str
+        :param search: General search, e.g. by id, description, prefix
+        :type search: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GetApiKeysResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_api_keys_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_api_keys_with_http_info(accept_language, x_child_company_id, limit, search, next, previous, **kwargs)  # noqa: E501
+        return self.get_api_keys_with_http_info(accept_language, x_child_company_id, limit, next, previous, search, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_api_keys_with_http_info(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, search : Annotated[Optional[StrictStr], Field(description="General order search, e.g. by mail, reference etc.")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_api_keys_with_http_info(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, search : Annotated[Optional[StrictStr], Field(description="General search, e.g. by id, description, prefix")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Get list of Api Keys  # noqa: E501
 
         Consume the list of api keys you have  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_api_keys_with_http_info(accept_language, x_child_company_id, limit, search, next, previous, async_req=True)
+        >>> thread = api.get_api_keys_with_http_info(accept_language, x_child_company_id, limit, next, previous, search, async_req=True)
         >>> result = thread.get()
 
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param limit: The numbers of items to return, the maximum value is 250
         :type limit: int
-        :param search: General order search, e.g. by mail, reference etc.
-        :type search: str
         :param next: next page
         :type next: str
         :param previous: previous page
         :type previous: str
+        :param search: General search, e.g. by id, description, prefix
+        :type search: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -613,17 +613,17 @@
 
         _params = locals()
 
         _all_params = [
             'accept_language',
             'x_child_company_id',
             'limit',
-            'search',
             'next',
-            'previous'
+            'previous',
+            'search'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -649,23 +649,23 @@
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('limit') is not None:  # noqa: E501
             _query_params.append(('limit', _params['limit']))
 
-        if _params.get('search') is not None:  # noqa: E501
-            _query_params.append(('search', _params['search']))
-
         if _params.get('next') is not None:  # noqa: E501
             _query_params.append(('next', _params['next']))
 
         if _params.get('previous') is not None:  # noqa: E501
             _query_params.append(('previous', _params['previous']))
 
+        if _params.get('search') is not None:  # noqa: E501
+            _query_params.append(('search', _params['search']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['accept_language']:
             _header_params['Accept-Language'] = _params['accept_language']
 
         if _params['x_child_company_id']:
             _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
```

### Comparing `conekta-6.0.0/conekta/api/charges_api.py` & `conekta-6.0.1/conekta/api/charges_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/companies_api.py` & `conekta-6.0.1/conekta/api/companies_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/customers_api.py` & `conekta-6.0.1/conekta/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/discounts_api.py` & `conekta-6.0.1/conekta/api/taxes_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,88 +20,88 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
 from typing import Optional
 
-from conekta.models.discount_lines_response import DiscountLinesResponse
-from conekta.models.order_discount_lines_request import OrderDiscountLinesRequest
-from conekta.models.update_order_discount_lines_request import UpdateOrderDiscountLinesRequest
+from conekta.models.order_tax_request import OrderTaxRequest
+from conekta.models.update_order_tax_request import UpdateOrderTaxRequest
+from conekta.models.update_order_tax_response import UpdateOrderTaxResponse
 
 from conekta.api_client import ApiClient
 from conekta.api_response import ApiResponse
 from conekta.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DiscountsApi(object):
+class TaxesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def orders_create_discount_line(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_discount_lines_request : Annotated[OrderDiscountLinesRequest, Field(..., description="requested field for a discount lines")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> DiscountLinesResponse:  # noqa: E501
-        """Create Discount  # noqa: E501
+    def orders_create_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_tax_request : Annotated[OrderTaxRequest, Field(..., description="requested field for a taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
+        """Create Tax  # noqa: E501
 
-        Create discount lines for an existing orden  # noqa: E501
+        Create new taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_create_discount_line(id, order_discount_lines_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_create_taxes(id, order_tax_request, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param order_discount_lines_request: requested field for a discount lines (required)
-        :type order_discount_lines_request: OrderDiscountLinesRequest
+        :param order_tax_request: requested field for a taxes (required)
+        :type order_tax_request: OrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DiscountLinesResponse
+        :rtype: UpdateOrderTaxResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_create_discount_line_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_create_discount_line_with_http_info(id, order_discount_lines_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the orders_create_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.orders_create_taxes_with_http_info(id, order_tax_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def orders_create_discount_line_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_discount_lines_request : Annotated[OrderDiscountLinesRequest, Field(..., description="requested field for a discount lines")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Create Discount  # noqa: E501
+    def orders_create_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_tax_request : Annotated[OrderTaxRequest, Field(..., description="requested field for a taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Create Tax  # noqa: E501
 
-        Create discount lines for an existing orden  # noqa: E501
+        Create new taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_create_discount_line_with_http_info(id, order_discount_lines_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_create_taxes_with_http_info(id, order_tax_request, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param order_discount_lines_request: requested field for a discount lines (required)
-        :type order_discount_lines_request: OrderDiscountLinesRequest
+        :param order_tax_request: requested field for a taxes (required)
+        :type order_tax_request: OrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -120,22 +120,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DiscountLinesResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'order_discount_lines_request',
+            'order_tax_request',
             'accept_language',
             'x_child_company_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -148,15 +148,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method orders_create_discount_line" % _key
+                    " to method orders_create_taxes" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -176,16 +176,16 @@
             _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['order_discount_lines_request'] is not None:
-            _body_params = _params['order_discount_lines_request']
+        if _params['order_tax_request'] is not None:
+            _body_params = _params['order_tax_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -194,22 +194,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "DiscountLinesResponse",
+            '200': "UpdateOrderTaxResponse",
             '401': "Error",
             '404': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
-            '/orders/{id}/discount_lines', 'POST',
+            '/orders/{id}/tax_lines', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -218,63 +218,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def orders_delete_discount_lines(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], discount_lines_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> DiscountLinesResponse:  # noqa: E501
-        """Delete Discount  # noqa: E501
+    def orders_delete_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
+        """Delete Tax  # noqa: E501
 
-        Delete an existing discount lines for an existing orden  # noqa: E501
+        Delete taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_delete_discount_lines(id, discount_lines_id, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_delete_taxes(id, tax_id, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param discount_lines_id: identifier (required)
-        :type discount_lines_id: str
+        :param tax_id: identifier (required)
+        :type tax_id: str
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DiscountLinesResponse
+        :rtype: UpdateOrderTaxResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_delete_discount_lines_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_delete_discount_lines_with_http_info(id, discount_lines_id, accept_language, x_child_company_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the orders_delete_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.orders_delete_taxes_with_http_info(id, tax_id, accept_language, x_child_company_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def orders_delete_discount_lines_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], discount_lines_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Delete Discount  # noqa: E501
+    def orders_delete_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Delete Tax  # noqa: E501
 
-        Delete an existing discount lines for an existing orden  # noqa: E501
+        Delete taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_delete_discount_lines_with_http_info(id, discount_lines_id, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_delete_taxes_with_http_info(id, tax_id, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param discount_lines_id: identifier (required)
-        :type discount_lines_id: str
+        :param tax_id: identifier (required)
+        :type tax_id: str
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -293,22 +293,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DiscountLinesResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'discount_lines_id',
+            'tax_id',
             'accept_language',
             'x_child_company_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -321,28 +321,28 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method orders_delete_discount_lines" % _key
+                    " to method orders_delete_taxes" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
-        if _params['discount_lines_id']:
-            _path_params['discount_lines_id'] = _params['discount_lines_id']
+        if _params['tax_id']:
+            _path_params['tax_id'] = _params['tax_id']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['accept_language']:
@@ -360,23 +360,23 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "DiscountLinesResponse",
+            '200': "UpdateOrderTaxResponse",
             '401': "Error",
-            '404': "Error",
             '422': "Error",
+            '404': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
-            '/orders/{id}/discount_lines/{discount_lines_id}', 'DELETE',
+            '/orders/{id}/tax_lines/{tax_id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -385,67 +385,67 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def orders_update_discount_lines(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], discount_lines_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_discount_lines_request : Annotated[UpdateOrderDiscountLinesRequest, Field(..., description="requested field for a discount lines")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> DiscountLinesResponse:  # noqa: E501
-        """Update Discount  # noqa: E501
+    def orders_update_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_tax_request : Annotated[UpdateOrderTaxRequest, Field(..., description="requested field for taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
+        """Update Tax  # noqa: E501
 
-        Update an existing discount lines for an existing orden  # noqa: E501
+        Update taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_update_discount_lines(id, discount_lines_id, update_order_discount_lines_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_update_taxes(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param discount_lines_id: identifier (required)
-        :type discount_lines_id: str
-        :param update_order_discount_lines_request: requested field for a discount lines (required)
-        :type update_order_discount_lines_request: UpdateOrderDiscountLinesRequest
+        :param tax_id: identifier (required)
+        :type tax_id: str
+        :param update_order_tax_request: requested field for taxes (required)
+        :type update_order_tax_request: UpdateOrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DiscountLinesResponse
+        :rtype: UpdateOrderTaxResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_update_discount_lines_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_update_discount_lines_with_http_info(id, discount_lines_id, update_order_discount_lines_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the orders_update_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.orders_update_taxes_with_http_info(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def orders_update_discount_lines_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], discount_lines_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_discount_lines_request : Annotated[UpdateOrderDiscountLinesRequest, Field(..., description="requested field for a discount lines")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Update Discount  # noqa: E501
+    def orders_update_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_tax_request : Annotated[UpdateOrderTaxRequest, Field(..., description="requested field for taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Update Tax  # noqa: E501
 
-        Update an existing discount lines for an existing orden  # noqa: E501
+        Update taxes for an existing orden  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_update_discount_lines_with_http_info(id, discount_lines_id, update_order_discount_lines_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.orders_update_taxes_with_http_info(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param discount_lines_id: identifier (required)
-        :type discount_lines_id: str
-        :param update_order_discount_lines_request: requested field for a discount lines (required)
-        :type update_order_discount_lines_request: UpdateOrderDiscountLinesRequest
+        :param tax_id: identifier (required)
+        :type tax_id: str
+        :param update_order_tax_request: requested field for taxes (required)
+        :type update_order_tax_request: UpdateOrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -464,23 +464,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DiscountLinesResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'discount_lines_id',
-            'update_order_discount_lines_request',
+            'tax_id',
+            'update_order_tax_request',
             'accept_language',
             'x_child_company_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -493,28 +493,28 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method orders_update_discount_lines" % _key
+                    " to method orders_update_taxes" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
-        if _params['discount_lines_id']:
-            _path_params['discount_lines_id'] = _params['discount_lines_id']
+        if _params['tax_id']:
+            _path_params['tax_id'] = _params['tax_id']
 
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['accept_language']:
@@ -524,16 +524,16 @@
             _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['update_order_discount_lines_request'] is not None:
-            _body_params = _params['update_order_discount_lines_request']
+        if _params['update_order_tax_request'] is not None:
+            _body_params = _params['update_order_tax_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -542,23 +542,23 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "DiscountLinesResponse",
+            '200': "UpdateOrderTaxResponse",
             '401': "Error",
-            '404': "Error",
             '422': "Error",
+            '404': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
-            '/orders/{id}/discount_lines/{discount_lines_id}', 'PUT',
+            '/orders/{id}/tax_lines/{tax_id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `conekta-6.0.0/conekta/api/events_api.py` & `conekta-6.0.1/conekta/api/events_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/logs_api.py` & `conekta-6.0.1/conekta/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/orders_api.py` & `conekta-6.0.1/conekta/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/payment_link_api.py` & `conekta-6.0.1/conekta/api/payment_link_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/payment_methods_api.py` & `conekta-6.0.1/conekta/api/payment_methods_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/plans_api.py` & `conekta-6.0.1/conekta/api/plans_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/products_api.py` & `conekta-6.0.1/conekta/api/products_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/shipping_contacts_api.py` & `conekta-6.0.1/conekta/api/shipping_contacts_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/shippings_api.py` & `conekta-6.0.1/conekta/api/shippings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,14 +363,15 @@
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
             '200': "ShippingOrderResponse",
             '401': "Error",
             '404': "Error",
             '422': "Error",
+            '428': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
             '/orders/{id}/shipping_lines/{shipping_id}', 'DELETE',
             _path_params,
             _query_params,
```

### Comparing `conekta-6.0.0/conekta/api/subscriptions_api.py` & `conekta-6.0.1/conekta/api/subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/taxes_api.py` & `conekta-6.0.1/conekta/api/transfers_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,92 +16,87 @@
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
+from pydantic import Field, StrictStr, conint
 
 from typing import Optional
 
-from conekta.models.order_tax_request import OrderTaxRequest
-from conekta.models.update_order_tax_request import UpdateOrderTaxRequest
-from conekta.models.update_order_tax_response import UpdateOrderTaxResponse
+from conekta.models.get_transfers_response import GetTransfersResponse
+from conekta.models.transfer_response import TransferResponse
 
 from conekta.api_client import ApiClient
 from conekta.api_response import ApiResponse
 from conekta.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TaxesApi(object):
+class TransfersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def orders_create_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_tax_request : Annotated[OrderTaxRequest, Field(..., description="requested field for a taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
-        """Create Tax  # noqa: E501
+    def get_transfer(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> TransferResponse:  # noqa: E501
+        """Get Transfer  # noqa: E501
 
-        Create new taxes for an existing orden  # noqa: E501
+        Get the details of a Transfer  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_create_taxes(id, order_tax_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.get_transfer(id, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param order_tax_request: requested field for a taxes (required)
-        :type order_tax_request: OrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UpdateOrderTaxResponse
+        :rtype: TransferResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_create_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_create_taxes_with_http_info(id, order_tax_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the get_transfer_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.get_transfer_with_http_info(id, accept_language, x_child_company_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def orders_create_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], order_tax_request : Annotated[OrderTaxRequest, Field(..., description="requested field for a taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Create Tax  # noqa: E501
+    def get_transfer_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Get Transfer  # noqa: E501
 
-        Create new taxes for an existing orden  # noqa: E501
+        Get the details of a Transfer  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_create_taxes_with_http_info(id, order_tax_request, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.get_transfer_with_http_info(id, accept_language, x_child_company_id, async_req=True)
         >>> result = thread.get()
 
         :param id: Identifier of the resource (required)
         :type id: str
-        :param order_tax_request: requested field for a taxes (required)
-        :type order_tax_request: OrderTaxRequest
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -120,22 +115,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TransferResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'order_tax_request',
             'accept_language',
             'x_child_company_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -148,15 +142,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method orders_create_taxes" % _key
+                    " to method get_transfer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -176,40 +170,30 @@
             _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['order_tax_request'] is not None:
-            _body_params = _params['order_tax_request']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "UpdateOrderTaxResponse",
+            '200': "TransferResponse",
             '401': "Error",
             '404': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
-            '/orders/{id}/tax_lines', 'POST',
+            '/transfers/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -218,67 +202,75 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def orders_delete_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
-        """Delete Tax  # noqa: E501
+    def get_transfers(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, search : Annotated[Optional[StrictStr], Field(description="General order search, e.g. by mail, reference etc.")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, **kwargs) -> GetTransfersResponse:  # noqa: E501
+        """Get a list of transfers  # noqa: E501
 
-        Delete taxes for an existing orden  # noqa: E501
+        Get transfers details in the form of a list  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_delete_taxes(id, tax_id, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.get_transfers(accept_language, x_child_company_id, limit, search, next, previous, async_req=True)
         >>> result = thread.get()
 
-        :param id: Identifier of the resource (required)
-        :type id: str
-        :param tax_id: identifier (required)
-        :type tax_id: str
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
+        :param limit: The numbers of items to return, the maximum value is 250
+        :type limit: int
+        :param search: General order search, e.g. by mail, reference etc.
+        :type search: str
+        :param next: next page
+        :type next: str
+        :param previous: previous page
+        :type previous: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UpdateOrderTaxResponse
+        :rtype: GetTransfersResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_delete_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_delete_taxes_with_http_info(id, tax_id, accept_language, x_child_company_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the get_transfers_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.get_transfers_with_http_info(accept_language, x_child_company_id, limit, search, next, previous, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def orders_delete_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Delete Tax  # noqa: E501
+    def get_transfers_with_http_info(self, accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, limit : Annotated[Optional[conint(strict=True, le=250, ge=1)], Field(description="The numbers of items to return, the maximum value is 250")] = None, search : Annotated[Optional[StrictStr], Field(description="General order search, e.g. by mail, reference etc.")] = None, next : Annotated[Optional[StrictStr], Field(description="next page")] = None, previous : Annotated[Optional[StrictStr], Field(description="previous page")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Get a list of transfers  # noqa: E501
 
-        Delete taxes for an existing orden  # noqa: E501
+        Get transfers details in the form of a list  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.orders_delete_taxes_with_http_info(id, tax_id, accept_language, x_child_company_id, async_req=True)
+        >>> thread = api.get_transfers_with_http_info(accept_language, x_child_company_id, limit, search, next, previous, async_req=True)
         >>> result = thread.get()
 
-        :param id: Identifier of the resource (required)
-        :type id: str
-        :param tax_id: identifier (required)
-        :type tax_id: str
         :param accept_language: Use for knowing which language to use
         :type accept_language: str
         :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
         :type x_child_company_id: str
+        :param limit: The numbers of items to return, the maximum value is 250
+        :type limit: int
+        :param search: General order search, e.g. by mail, reference etc.
+        :type search: str
+        :param next: next page
+        :type next: str
+        :param previous: previous page
+        :type previous: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -293,24 +285,26 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetTransfersResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'tax_id',
             'accept_language',
-            'x_child_company_id'
+            'x_child_company_id',
+            'limit',
+            'search',
+            'next',
+            'previous'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -321,244 +315,66 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method orders_delete_taxes" % _key
+                    " to method get_transfers" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-        if _params['tax_id']:
-            _path_params['tax_id'] = _params['tax_id']
-
 
         # process the query parameters
         _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        if _params['accept_language']:
-            _header_params['Accept-Language'] = _params['accept_language']
-
-        if _params['x_child_company_id']:
-            _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['bearerAuth']  # noqa: E501
-
-        _response_types_map = {
-            '200': "UpdateOrderTaxResponse",
-            '401': "Error",
-            '422': "Error",
-            '404': "Error",
-            '500': "Error",
-        }
-
-        return self.api_client.call_api(
-            '/orders/{id}/tax_lines/{tax_id}', 'DELETE',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def orders_update_taxes(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_tax_request : Annotated[UpdateOrderTaxRequest, Field(..., description="requested field for taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> UpdateOrderTaxResponse:  # noqa: E501
-        """Update Tax  # noqa: E501
+        if _params.get('limit') is not None:  # noqa: E501
+            _query_params.append(('limit', _params['limit']))
 
-        Update taxes for an existing orden  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
+        if _params.get('search') is not None:  # noqa: E501
+            _query_params.append(('search', _params['search']))
 
-        >>> thread = api.orders_update_taxes(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, async_req=True)
-        >>> result = thread.get()
+        if _params.get('next') is not None:  # noqa: E501
+            _query_params.append(('next', _params['next']))
 
-        :param id: Identifier of the resource (required)
-        :type id: str
-        :param tax_id: identifier (required)
-        :type tax_id: str
-        :param update_order_tax_request: requested field for taxes (required)
-        :type update_order_tax_request: UpdateOrderTaxRequest
-        :param accept_language: Use for knowing which language to use
-        :type accept_language: str
-        :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
-        :type x_child_company_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: UpdateOrderTaxResponse
-        """
-        kwargs['_return_http_data_only'] = True
-        if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the orders_update_taxes_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.orders_update_taxes_with_http_info(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def orders_update_taxes_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Identifier of the resource")], tax_id : Annotated[StrictStr, Field(..., description="identifier")], update_order_tax_request : Annotated[UpdateOrderTaxRequest, Field(..., description="requested field for taxes")], accept_language : Annotated[Optional[StrictStr], Field(description="Use for knowing which language to use")] = None, x_child_company_id : Annotated[Optional[StrictStr], Field(description="In the case of a holding company, the company id of the child company to which will process the request.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """Update Tax  # noqa: E501
+        if _params.get('previous') is not None:  # noqa: E501
+            _query_params.append(('previous', _params['previous']))
 
-        Update taxes for an existing orden  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.orders_update_taxes_with_http_info(id, tax_id, update_order_tax_request, accept_language, x_child_company_id, async_req=True)
-        >>> result = thread.get()
-
-        :param id: Identifier of the resource (required)
-        :type id: str
-        :param tax_id: identifier (required)
-        :type tax_id: str
-        :param update_order_tax_request: requested field for taxes (required)
-        :type update_order_tax_request: UpdateOrderTaxRequest
-        :param accept_language: Use for knowing which language to use
-        :type accept_language: str
-        :param x_child_company_id: In the case of a holding company, the company id of the child company to which will process the request.
-        :type x_child_company_id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the 
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :type _preload_content: bool, optional
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :type _return_http_data_only: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(UpdateOrderTaxResponse, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'id',
-            'tax_id',
-            'update_order_tax_request',
-            'accept_language',
-            'x_child_company_id'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method orders_update_taxes" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-        if _params['tax_id']:
-            _path_params['tax_id'] = _params['tax_id']
-
-
-        # process the query parameters
-        _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['accept_language']:
             _header_params['Accept-Language'] = _params['accept_language']
 
         if _params['x_child_company_id']:
             _header_params['X-Child-Company-Id'] = _params['x_child_company_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['update_order_tax_request'] is not None:
-            _body_params = _params['update_order_tax_request']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/vnd.conekta-v2.1.0+json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "UpdateOrderTaxResponse",
+            '200': "GetTransfersResponse",
             '401': "Error",
-            '422': "Error",
-            '404': "Error",
             '500': "Error",
         }
 
         return self.api_client.call_api(
-            '/orders/{id}/tax_lines/{tax_id}', 'PUT',
+            '/transfers', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `conekta-6.0.0/conekta/api/tokens_api.py` & `conekta-6.0.1/conekta/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/transactions_api.py` & `conekta-6.0.1/conekta/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/webhook_keys_api.py` & `conekta-6.0.1/conekta/api/webhook_keys_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api/webhooks_api.py` & `conekta-6.0.1/conekta/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/api_client.py` & `conekta-6.0.1/conekta/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         'datetime': datetime.datetime,
         'object': object,
     }
     data = {
       'lang': 'python',
       'lang_version': platform.python_version(),
       'publisher': 'conekta',
-      'bindings_version': '6.0.0',
+      'bindings_version': '6.0.1',
       'uname': platform.uname()
     }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
                  cookie=None, pool_threads=1):
         # use default configuration if none is provided
@@ -81,15 +81,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Conekta/v2 PythonBindings/6.0.0'
+        self.user_agent = 'Conekta/v2 PythonBindings/6.0.1'
         self.conekta_user_agent = json.dumps(self.data)
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `conekta-6.0.0/conekta/api_response.py` & `conekta-6.0.1/conekta/api_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/configuration.py` & `conekta-6.0.1/conekta/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.1.0\n"\
-               "SDK Package Version: 6.0.0".\
+               "SDK Package Version: 6.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `conekta-6.0.0/conekta/exceptions.py` & `conekta-6.0.1/conekta/exceptions.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/__init__.py` & `conekta-6.0.1/conekta/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 
 # import models into model package
 from conekta.models.api_key_create_response import ApiKeyCreateResponse
 from conekta.models.api_key_create_response_all_of import ApiKeyCreateResponseAllOf
 from conekta.models.api_key_request import ApiKeyRequest
 from conekta.models.api_key_response import ApiKeyResponse
+from conekta.models.api_key_response_on_delete import ApiKeyResponseOnDelete
 from conekta.models.api_key_update_request import ApiKeyUpdateRequest
+from conekta.models.balance_common_field import BalanceCommonField
+from conekta.models.balance_response import BalanceResponse
 from conekta.models.blacklist_rule_response import BlacklistRuleResponse
 from conekta.models.charge_data_payment_method_bank_transfer_response import ChargeDataPaymentMethodBankTransferResponse
 from conekta.models.charge_data_payment_method_card_response import ChargeDataPaymentMethodCardResponse
 from conekta.models.charge_data_payment_method_cash_response import ChargeDataPaymentMethodCashResponse
 from conekta.models.charge_order_response import ChargeOrderResponse
 from conekta.models.charge_order_response_payment_method import ChargeOrderResponsePaymentMethod
 from conekta.models.charge_request import ChargeRequest
@@ -101,14 +104,16 @@
 from conekta.models.get_charges_response import GetChargesResponse
 from conekta.models.get_charges_response_all_of import GetChargesResponseAllOf
 from conekta.models.get_companies_response import GetCompaniesResponse
 from conekta.models.get_companies_response_all_of import GetCompaniesResponseAllOf
 from conekta.models.get_customer_payment_method_data_response import GetCustomerPaymentMethodDataResponse
 from conekta.models.get_events_response import GetEventsResponse
 from conekta.models.get_events_response_all_of import GetEventsResponseAllOf
+from conekta.models.get_order_discount_lines_response import GetOrderDiscountLinesResponse
+from conekta.models.get_order_discount_lines_response_all_of import GetOrderDiscountLinesResponseAllOf
 from conekta.models.get_orders_response import GetOrdersResponse
 from conekta.models.get_payment_method_response import GetPaymentMethodResponse
 from conekta.models.get_payment_method_response_all_of import GetPaymentMethodResponseAllOf
 from conekta.models.get_plans_response import GetPlansResponse
 from conekta.models.get_plans_response_all_of import GetPlansResponseAllOf
 from conekta.models.get_transactions_response import GetTransactionsResponse
 from conekta.models.get_transactions_response_all_of import GetTransactionsResponseAllOf
@@ -139,14 +144,15 @@
 from conekta.models.order_response_fiscal_entity_address_all_of import OrderResponseFiscalEntityAddressAllOf
 from conekta.models.order_response_products import OrderResponseProducts
 from conekta.models.order_response_products_all_of import OrderResponseProductsAllOf
 from conekta.models.order_response_shipping_contact import OrderResponseShippingContact
 from conekta.models.order_response_shipping_contact_all_of import OrderResponseShippingContactAllOf
 from conekta.models.order_tax_request import OrderTaxRequest
 from conekta.models.order_update_request import OrderUpdateRequest
+from conekta.models.order_update_request_customer_info import OrderUpdateRequestCustomerInfo
 from conekta.models.orders_response import OrdersResponse
 from conekta.models.page import Page
 from conekta.models.pagination import Pagination
 from conekta.models.payment_method import PaymentMethod
 from conekta.models.payment_method_bank_transfer import PaymentMethodBankTransfer
 from conekta.models.payment_method_card import PaymentMethodCard
 from conekta.models.payment_method_card_request import PaymentMethodCardRequest
```

### Comparing `conekta-6.0.0/conekta/models/api_key_create_response.py` & `conekta-6.0.1/conekta/models/delete_api_keys_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class ApiKeyCreateResponse(BaseModel):
+class DeleteApiKeysResponse(BaseModel):
     """
-    ApiKeyCreateResponse
+    DeleteApiKeysResponse
     """
-    authentication_token: Optional[StrictStr] = Field(None, description="It is occupied as a user when authenticated with basic authentication, with a blank password. This value will only appear once, in the request to create a new key")
     active: Optional[StrictBool] = Field(None, description="Indicates if the api key is active")
-    created_at: Optional[StrictInt] = Field(None, description="Unix timestamp in seconds with the creation date of the api key")
-    description: Optional[StrictStr] = Field(None, description="Detail of the use that will be given to the api key")
-    id: Optional[StrictStr] = Field(None, description="Unique identifier of the api key")
-    livemode: Optional[StrictBool] = Field(None, description="Indicates if the api key is in live mode")
-    object: Optional[StrictStr] = Field(None, description="Object name, value is api_key")
+    created_at: Optional[StrictInt] = Field(None, description="Unix timestamp in seconds of when the api key was created")
+    description: Optional[StrictStr] = Field(None, description="A name or brief explanation of what this api key is used for")
+    livemode: Optional[StrictBool] = Field(None, description="Indicates if the api key is in production")
     prefix: Optional[StrictStr] = Field(None, description="The first few characters of the authentication_token")
-    role: Optional[StrictStr] = Field(None, description="Indicates the user account private=owner or public=public")
-    __properties = ["authentication_token", "active", "created_at", "description", "id", "livemode", "object", "prefix", "role"]
+    id: Optional[StrictStr] = Field(None, description="Unique identifier of the api key")
+    object: Optional[StrictStr] = Field(None, description="Object name, value is 'api_key'")
+    deleted: Optional[StrictBool] = None
+    role: Optional[StrictStr] = Field(None, description="Indicates if the api key is private or public")
+    __properties = ["active", "created_at", "description", "livemode", "prefix", "id", "object", "deleted", "role"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,41 +47,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ApiKeyCreateResponse:
-        """Create an instance of ApiKeyCreateResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> DeleteApiKeysResponse:
+        """Create an instance of DeleteApiKeysResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ApiKeyCreateResponse:
-        """Create an instance of ApiKeyCreateResponse from a dict"""
+    def from_dict(cls, obj: dict) -> DeleteApiKeysResponse:
+        """Create an instance of DeleteApiKeysResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ApiKeyCreateResponse.parse_obj(obj)
+            return DeleteApiKeysResponse.parse_obj(obj)
 
-        _obj = ApiKeyCreateResponse.parse_obj({
-            "authentication_token": obj.get("authentication_token"),
+        _obj = DeleteApiKeysResponse.parse_obj({
             "active": obj.get("active"),
             "created_at": obj.get("created_at"),
             "description": obj.get("description"),
-            "id": obj.get("id"),
             "livemode": obj.get("livemode"),
-            "object": obj.get("object"),
             "prefix": obj.get("prefix"),
+            "id": obj.get("id"),
+            "object": obj.get("object"),
+            "deleted": obj.get("deleted"),
             "role": obj.get("role")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/api_key_create_response_all_of.py` & `conekta-6.0.1/conekta/models/pagination.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
-class ApiKeyCreateResponseAllOf(BaseModel):
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+
+class Pagination(BaseModel):
     """
-    ApiKeyCreateResponseAllOf
+    pagination metadata
     """
-    authentication_token: Optional[StrictStr] = Field(None, description="It is occupied as a user when authenticated with basic authentication, with a blank password. This value will only appear once, in the request to create a new key")
-    __properties = ["authentication_token"]
+    has_more: StrictBool = Field(..., description="Indicates if there are more pages to be requested")
+    object: StrictStr = Field(..., description="Object type, in this case is list")
+    __properties = ["has_more", "object"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ApiKeyCreateResponseAllOf:
-        """Create an instance of ApiKeyCreateResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> Pagination:
+        """Create an instance of Pagination from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ApiKeyCreateResponseAllOf:
-        """Create an instance of ApiKeyCreateResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> Pagination:
+        """Create an instance of Pagination from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ApiKeyCreateResponseAllOf.parse_obj(obj)
+            return Pagination.parse_obj(obj)
 
-        _obj = ApiKeyCreateResponseAllOf.parse_obj({
-            "authentication_token": obj.get("authentication_token")
+        _obj = Pagination.parse_obj({
+            "has_more": obj.get("has_more"),
+            "object": obj.get("object")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/api_key_request.py` & `conekta-6.0.1/conekta/models/webhook_key_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-
-class ApiKeyRequest(BaseModel):
+class WebhookKeyRequest(BaseModel):
     """
-    ApiKeyRequest
+    WebhookKeyRequest
     """
-    active: StrictBool = Field(..., description="Indicates if the api key is active")
-    description: StrictStr = Field(..., description="Detail of the use that will be given to the api key")
-    role: StrictStr = Field(...)
-    __properties = ["active", "description", "role"]
+    active: Optional[StrictBool] = Field(True, description="Indicates if the webhook key is active")
+    __properties = ["active"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,35 +39,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ApiKeyRequest:
-        """Create an instance of ApiKeyRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> WebhookKeyRequest:
+        """Create an instance of WebhookKeyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ApiKeyRequest:
-        """Create an instance of ApiKeyRequest from a dict"""
+    def from_dict(cls, obj: dict) -> WebhookKeyRequest:
+        """Create an instance of WebhookKeyRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ApiKeyRequest.parse_obj(obj)
+            return WebhookKeyRequest.parse_obj(obj)
 
-        _obj = ApiKeyRequest.parse_obj({
-            "active": obj.get("active"),
-            "description": obj.get("description"),
-            "role": obj.get("role")
+        _obj = WebhookKeyRequest.parse_obj({
+            "active": obj.get("active") if obj.get("active") is not None else True
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/api_key_response.py` & `conekta-6.0.1/conekta/models/api_key_response_on_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class ApiKeyResponse(BaseModel):
+class ApiKeyResponseOnDelete(BaseModel):
     """
     api keys model
     """
     active: Optional[StrictBool] = Field(None, description="Indicates if the api key is active")
-    created_at: Optional[StrictInt] = Field(None, description="Unix timestamp in seconds with the creation date of the api key")
-    description: Optional[StrictStr] = Field(None, description="Detail of the use that will be given to the api key")
-    id: Optional[StrictStr] = Field(None, description="Unique identifier of the api key")
-    livemode: Optional[StrictBool] = Field(None, description="Indicates if the api key is in live mode")
-    object: Optional[StrictStr] = Field(None, description="Object name, value is api_key")
+    created_at: Optional[StrictInt] = Field(None, description="Unix timestamp in seconds of when the api key was created")
+    description: Optional[StrictStr] = Field(None, description="A name or brief explanation of what this api key is used for")
+    livemode: Optional[StrictBool] = Field(None, description="Indicates if the api key is in production")
     prefix: Optional[StrictStr] = Field(None, description="The first few characters of the authentication_token")
-    role: Optional[StrictStr] = Field(None, description="Indicates the user account private=owner or public=public")
-    __properties = ["active", "created_at", "description", "id", "livemode", "object", "prefix", "role"]
+    id: Optional[StrictStr] = Field(None, description="Unique identifier of the api key")
+    object: Optional[StrictStr] = Field(None, description="Object name, value is 'api_key'")
+    deleted: Optional[StrictBool] = Field(None, description="Indicates if the api key was deleted")
+    role: Optional[StrictStr] = Field(None, description="Indicates if the api key is private or public")
+    __properties = ["active", "created_at", "description", "livemode", "prefix", "id", "object", "deleted", "role"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -46,40 +47,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ApiKeyResponse:
-        """Create an instance of ApiKeyResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> ApiKeyResponseOnDelete:
+        """Create an instance of ApiKeyResponseOnDelete from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ApiKeyResponse:
-        """Create an instance of ApiKeyResponse from a dict"""
+    def from_dict(cls, obj: dict) -> ApiKeyResponseOnDelete:
+        """Create an instance of ApiKeyResponseOnDelete from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ApiKeyResponse.parse_obj(obj)
+            return ApiKeyResponseOnDelete.parse_obj(obj)
 
-        _obj = ApiKeyResponse.parse_obj({
+        _obj = ApiKeyResponseOnDelete.parse_obj({
             "active": obj.get("active"),
             "created_at": obj.get("created_at"),
             "description": obj.get("description"),
-            "id": obj.get("id"),
             "livemode": obj.get("livemode"),
-            "object": obj.get("object"),
             "prefix": obj.get("prefix"),
+            "id": obj.get("id"),
+            "object": obj.get("object"),
+            "deleted": obj.get("deleted"),
             "role": obj.get("role")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/api_key_update_request.py` & `conekta-6.0.1/conekta/models/api_key_update_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
 class ApiKeyUpdateRequest(BaseModel):
     """
     ApiKeyUpdateRequest
     """
     active: Optional[StrictBool] = Field(None, description="Indicates if the webhook key is active")
-    description: Optional[StrictStr] = Field(None, description="Detail of the use that will be given to the api key")
+    description: Optional[StrictStr] = Field(None, description="A name or brief explanation of what this api key is used for")
     __properties = ["active", "description"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `conekta-6.0.0/conekta/models/blacklist_rule_response.py` & `conekta-6.0.1/conekta/models/blacklist_rule_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_data_payment_method_bank_transfer_response.py` & `conekta-6.0.1/conekta/models/charge_data_payment_method_bank_transfer_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_data_payment_method_card_response.py` & `conekta-6.0.1/conekta/models/charge_data_payment_method_card_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,31 +16,32 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictStr, conlist, constr
 
 class ChargeDataPaymentMethodCardResponse(BaseModel):
     """
     use for card responses
     """
     account_type: Optional[StrictStr] = None
     auth_code: Optional[StrictStr] = None
     brand: Optional[StrictStr] = None
+    contract_id: Optional[constr(strict=True, max_length=10, min_length=10)] = Field(None, description="Id sent for recurrent charges.")
     country: Optional[StrictStr] = None
     exp_month: Optional[StrictStr] = None
     exp_year: Optional[StrictStr] = None
     fraud_indicators: Optional[conlist(Any)] = None
     issuer: Optional[StrictStr] = None
     last4: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
-    __properties = ["account_type", "auth_code", "brand", "country", "exp_month", "exp_year", "fraud_indicators", "issuer", "last4", "name"]
+    __properties = ["account_type", "auth_code", "brand", "contract_id", "country", "exp_month", "exp_year", "fraud_indicators", "issuer", "last4", "name"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -73,14 +74,15 @@
         if not isinstance(obj, dict):
             return ChargeDataPaymentMethodCardResponse.parse_obj(obj)
 
         _obj = ChargeDataPaymentMethodCardResponse.parse_obj({
             "account_type": obj.get("account_type"),
             "auth_code": obj.get("auth_code"),
             "brand": obj.get("brand"),
+            "contract_id": obj.get("contract_id"),
             "country": obj.get("country"),
             "exp_month": obj.get("exp_month"),
             "exp_year": obj.get("exp_year"),
             "fraud_indicators": obj.get("fraud_indicators"),
             "issuer": obj.get("issuer"),
             "last4": obj.get("last4"),
             "name": obj.get("name")
```

### Comparing `conekta-6.0.0/conekta/models/charge_data_payment_method_cash_response.py` & `conekta-6.0.1/conekta/models/charge_data_payment_method_cash_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_order_response.py` & `conekta-6.0.1/conekta/models/charge_order_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_order_response_payment_method.py` & `conekta-6.0.1/conekta/models/charge_order_response_payment_method.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_request.py` & `conekta-6.0.1/conekta/models/charge_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_request_payment_method.py` & `conekta-6.0.1/conekta/models/charge_request_payment_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr, constr
 
 class ChargeRequestPaymentMethod(BaseModel):
     """
     Payment method used in the charge. Go to the [payment methods](https://developers.conekta.com/reference/m%C3%A9todos-de-pago) section for more details 
     """
     expires_at: Optional[StrictInt] = Field(None, description="Method expiration date as unix timestamp")
     type: StrictStr = Field(...)
     token_id: Optional[StrictStr] = None
     payment_source_id: Optional[StrictStr] = None
-    __properties = ["expires_at", "type", "token_id", "payment_source_id"]
+    contract_id: Optional[constr(strict=True, max_length=10, min_length=10)] = Field(None, description="Optional id sent to indicate the bank contract for recurrent card charges.")
+    __properties = ["expires_at", "type", "token_id", "payment_source_id", "contract_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -67,11 +68,12 @@
         if not isinstance(obj, dict):
             return ChargeRequestPaymentMethod.parse_obj(obj)
 
         _obj = ChargeRequestPaymentMethod.parse_obj({
             "expires_at": obj.get("expires_at"),
             "type": obj.get("type"),
             "token_id": obj.get("token_id"),
-            "payment_source_id": obj.get("payment_source_id")
+            "payment_source_id": obj.get("payment_source_id"),
+            "contract_id": obj.get("contract_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/charge_response.py` & `conekta-6.0.1/conekta/models/charge_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_response_channel.py` & `conekta-6.0.1/conekta/models/charge_response_channel.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_response_payment_method.py` & `conekta-6.0.1/conekta/models/charge_response_payment_method.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charge_response_refunds.py` & `conekta-6.0.1/conekta/models/charge_response_refunds.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
     ChargeResponseRefunds
     """
     has_more: StrictBool = Field(..., description="Indicates if there are more pages to be requested")
     object: StrictStr = Field(..., description="Object type, in this case is list")
     next_page_url: Optional[StrictStr] = Field(None, description="URL of the next page.")
     previous_page_url: Optional[StrictStr] = Field(None, description="Url of the previous page.")
-    data: Optional[conlist(ChargeResponseRefundsData)] = None
+    data: Optional[conlist(ChargeResponseRefundsData)] = Field(None, description="refunds")
     __properties = ["has_more", "object", "next_page_url", "previous_page_url", "data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `conekta-6.0.0/conekta/models/charge_response_refunds_all_of.py` & `conekta-6.0.1/conekta/models/charge_response_refunds_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, conlist
+from pydantic import BaseModel, Field, conlist
 from conekta.models.charge_response_refunds_data import ChargeResponseRefundsData
 
 class ChargeResponseRefundsAllOf(BaseModel):
     """
     ChargeResponseRefundsAllOf
     """
-    data: Optional[conlist(ChargeResponseRefundsData)] = None
+    data: Optional[conlist(ChargeResponseRefundsData)] = Field(None, description="refunds")
     __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `conekta-6.0.0/conekta/models/charge_response_refunds_data.py` & `conekta-6.0.1/conekta/models/charge_response_refunds_data.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/charges_data_response.py` & `conekta-6.0.1/conekta/models/charges_data_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkout.py` & `conekta-6.0.1/conekta/models/checkout.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkout_order_template.py` & `conekta-6.0.1/conekta/models/checkout_order_template.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkout_order_template_customer_info.py` & `conekta-6.0.1/conekta/models/checkout_order_template_customer_info.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkout_request.py` & `conekta-6.0.1/conekta/models/checkout_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
 
 class CheckoutRequest(BaseModel):
     """
-    [Checkout](https://developers.conekta.com/reference/checkout) details 
+    [Checkout](https://developers.conekta.com/v2.1.0/reference/payment-link) details 
     """
     allowed_payment_methods: conlist(StrictStr) = Field(..., description="Are the payment methods available for this link")
     expires_at: Optional[StrictInt] = Field(None, description="Unix timestamp of checkout expiration")
     failure_url: Optional[StrictStr] = Field(None, description="Redirection url back to the site in case of failed payment, applies only to HostedPayment.")
     monthly_installments_enabled: Optional[StrictBool] = None
     monthly_installments_options: Optional[conlist(StrictInt)] = None
     name: Optional[StrictStr] = Field(None, description="Reason for payment")
```

### Comparing `conekta-6.0.0/conekta/models/checkout_response.py` & `conekta-6.0.1/conekta/models/checkout_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkouts_response.py` & `conekta-6.0.1/conekta/models/checkouts_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/checkouts_response_all_of.py` & `conekta-6.0.1/conekta/models/checkouts_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/company_fiscal_info_address_response.py` & `conekta-6.0.1/conekta/models/company_fiscal_info_address_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/company_fiscal_info_response.py` & `conekta-6.0.1/conekta/models/company_fiscal_info_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/company_payout_destination_response.py` & `conekta-6.0.1/conekta/models/company_payout_destination_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/company_response.py` & `conekta-6.0.1/conekta/models/company_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response.py` & `conekta-6.0.1/conekta/models/create_customer_fiscal_entities_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response_all_of.py` & `conekta-6.0.1/conekta/models/create_customer_fiscal_entities_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/create_customer_payment_methods_request.py` & `conekta-6.0.1/conekta/models/create_customer_payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/create_customer_payment_methods_response.py` & `conekta-6.0.1/conekta/models/create_customer_payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/create_risk_rules_data.py` & `conekta-6.0.1/conekta/models/create_risk_rules_data.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer.py` & `conekta-6.0.1/conekta/models/customer.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_address.py` & `conekta-6.0.1/conekta/models/customer_address.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_antifraud_info.py` & `conekta-6.0.1/conekta/models/customer_antifraud_info.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_antifraud_info_response.py` & `conekta-6.0.1/conekta/models/customer_antifraud_info_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_fiscal_entities_data_response.py` & `conekta-6.0.1/conekta/models/customer_fiscal_entities_data_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_fiscal_entities_request.py` & `conekta-6.0.1/conekta/models/customer_fiscal_entities_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_fiscal_entities_request_address.py` & `conekta-6.0.1/conekta/models/customer_fiscal_entities_request_address.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_fiscal_entities_response.py` & `conekta-6.0.1/conekta/models/customer_fiscal_entities_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_fiscal_entities_response_all_of.py` & `conekta-6.0.1/conekta/models/customer_fiscal_entities_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_info.py` & `conekta-6.0.1/conekta/models/customer_info.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_info_just_customer_id.py` & `conekta-6.0.1/conekta/models/customer_info_just_customer_id.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_info_just_customer_id_response.py` & `conekta-6.0.1/conekta/models/customer_info_just_customer_id_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_info_response.py` & `conekta-6.0.1/conekta/models/customer_info_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_payment_method_request.py` & `conekta-6.0.1/conekta/models/customer_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_payment_methods.py` & `conekta-6.0.1/conekta/models/customer_payment_methods.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_payment_methods_data.py` & `conekta-6.0.1/conekta/models/customer_payment_methods_data.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_payment_methods_request.py` & `conekta-6.0.1/conekta/models/customer_payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_payment_methods_response.py` & `conekta-6.0.1/conekta/models/customer_payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_response.py` & `conekta-6.0.1/conekta/models/customer_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_response_shipping_contacts.py` & `conekta-6.0.1/conekta/models/customer_response_shipping_contacts.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_response_shipping_contacts_all_of.py` & `conekta-6.0.1/conekta/models/customer_response_shipping_contacts_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts_address.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts_address.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts_data_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response_all_of.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts_response.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_shipping_contacts_response_address.py` & `conekta-6.0.1/conekta/models/customer_shipping_contacts_response_address.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_update_fiscal_entities_request.py` & `conekta-6.0.1/conekta/models/customer_update_fiscal_entities_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customer_update_shipping_contacts.py` & `conekta-6.0.1/conekta/models/customer_update_shipping_contacts.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customers_response.py` & `conekta-6.0.1/conekta/models/customers_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/customers_response_all_of.py` & `conekta-6.0.1/conekta/models/customers_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/delete_api_keys_response.py` & `conekta-6.0.1/conekta/models/risk_rules_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class DeleteApiKeysResponse(BaseModel):
+class RiskRulesData(BaseModel):
     """
-    DeleteApiKeysResponse
+    RiskRulesData
     """
-    active: Optional[StrictBool] = Field(None, description="Indicates if the api key is active")
-    created_at: Optional[StrictInt] = Field(None, description="Unix timestamp in seconds with the creation date of the api key")
-    description: Optional[StrictStr] = Field(None, description="Detail of the use that will be given to the api key")
-    id: Optional[StrictStr] = Field(None, description="Unique identifier of the api key")
-    livemode: Optional[StrictBool] = Field(None, description="Indicates if the api key is in live mode")
-    object: Optional[StrictStr] = Field(None, description="Object name, value is api_key")
-    prefix: Optional[StrictStr] = Field(None, description="The first few characters of the authentication_token")
-    role: Optional[StrictStr] = Field(None, description="Indicates the user account private=owner or public=public")
-    deleted: Optional[StrictBool] = None
-    __properties = ["active", "created_at", "description", "id", "livemode", "object", "prefix", "role", "deleted"]
+    id: Optional[StrictStr] = Field(None, description="rule id")
+    field: Optional[StrictStr] = Field(None, description="field to be used for the rule")
+    created_at: Optional[StrictStr] = Field(None, description="rule creation date")
+    value: Optional[StrictStr] = Field(None, description="value to be used for the rule")
+    is_global: Optional[StrictBool] = Field(None, description="if the rule is global")
+    is_test: Optional[StrictBool] = Field(None, description="if the rule is test")
+    description: Optional[StrictStr] = Field(None, description="description of the rule")
+    __properties = ["id", "field", "created_at", "value", "is_global", "is_test", "description"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,41 +45,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeleteApiKeysResponse:
-        """Create an instance of DeleteApiKeysResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> RiskRulesData:
+        """Create an instance of RiskRulesData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeleteApiKeysResponse:
-        """Create an instance of DeleteApiKeysResponse from a dict"""
+    def from_dict(cls, obj: dict) -> RiskRulesData:
+        """Create an instance of RiskRulesData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DeleteApiKeysResponse.parse_obj(obj)
+            return RiskRulesData.parse_obj(obj)
 
-        _obj = DeleteApiKeysResponse.parse_obj({
-            "active": obj.get("active"),
-            "created_at": obj.get("created_at"),
-            "description": obj.get("description"),
+        _obj = RiskRulesData.parse_obj({
             "id": obj.get("id"),
-            "livemode": obj.get("livemode"),
-            "object": obj.get("object"),
-            "prefix": obj.get("prefix"),
-            "role": obj.get("role"),
-            "deleted": obj.get("deleted")
+            "field": obj.get("field"),
+            "created_at": obj.get("created_at"),
+            "value": obj.get("value"),
+            "is_global": obj.get("is_global"),
+            "is_test": obj.get("is_test"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/delete_api_keys_response_all_of.py` & `conekta-6.0.1/conekta/models/delete_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/deleted_blacklist_rule_response.py` & `conekta-6.0.1/conekta/models/deleted_blacklist_rule_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/deleted_whitelist_rule_response.py` & `conekta-6.0.1/conekta/models/deleted_whitelist_rule_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/details.py` & `conekta-6.0.1/conekta/models/details.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/details_error.py` & `conekta-6.0.1/conekta/models/details_error.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/discount_lines_data_response.py` & `conekta-6.0.1/conekta/models/discount_lines_data_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+
 from pydantic import BaseModel, Field, StrictStr, conint
 
 class DiscountLinesDataResponse(BaseModel):
     """
     DiscountLinesDataResponse
     """
     amount: conint(strict=True, ge=0) = Field(..., description="The amount to be deducted from the total sum of all payments, in cents.")
     code: StrictStr = Field(..., description="Discount code.")
     type: StrictStr = Field(..., description="It can be 'loyalty', 'campaign', 'coupon' o 'sign'")
-    id: Optional[StrictStr] = None
-    object: Optional[StrictStr] = None
-    parent_id: Optional[StrictStr] = None
+    id: StrictStr = Field(..., description="The discount line id")
+    object: StrictStr = Field(..., description="The object name")
+    parent_id: StrictStr = Field(..., description="The order id")
     __properties = ["amount", "code", "type", "id", "object", "parent_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `conekta-6.0.0/conekta/models/discount_lines_response.py` & `conekta-6.0.1/conekta/models/update_order_discount_lines_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,25 +18,22 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, conint
 
-class DiscountLinesResponse(BaseModel):
+class UpdateOrderDiscountLinesRequest(BaseModel):
     """
-    DiscountLinesResponse
+    List of discounts that apply to the order.
     """
-    amount: conint(strict=True, ge=0) = Field(..., description="The amount to be deducted from the total sum of all payments, in cents.")
-    code: StrictStr = Field(..., description="Discount code.")
-    type: StrictStr = Field(..., description="It can be 'loyalty', 'campaign', 'coupon' o 'sign'")
-    id: Optional[StrictStr] = None
-    object: Optional[StrictStr] = None
-    parent_id: Optional[StrictStr] = None
-    __properties = ["amount", "code", "type", "id", "object", "parent_id"]
+    amount: Optional[conint(strict=True, ge=0)] = None
+    code: Optional[StrictStr] = Field(None, description="Discount code.")
+    type: Optional[StrictStr] = None
+    __properties = ["amount", "code", "type"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -44,38 +41,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DiscountLinesResponse:
-        """Create an instance of DiscountLinesResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrderDiscountLinesRequest:
+        """Create an instance of UpdateOrderDiscountLinesRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DiscountLinesResponse:
-        """Create an instance of DiscountLinesResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrderDiscountLinesRequest:
+        """Create an instance of UpdateOrderDiscountLinesRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DiscountLinesResponse.parse_obj(obj)
+            return UpdateOrderDiscountLinesRequest.parse_obj(obj)
 
-        _obj = DiscountLinesResponse.parse_obj({
+        _obj = UpdateOrderDiscountLinesRequest.parse_obj({
             "amount": obj.get("amount"),
             "code": obj.get("code"),
-            "type": obj.get("type"),
-            "id": obj.get("id"),
-            "object": obj.get("object"),
-            "parent_id": obj.get("parent_id")
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/discount_lines_response_all_of.py` & `conekta-6.0.1/conekta/models/get_order_discount_lines_response_all_of.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, conlist
+from conekta.models.discount_lines_response import DiscountLinesResponse
 
-class DiscountLinesResponseAllOf(BaseModel):
+class GetOrderDiscountLinesResponseAllOf(BaseModel):
     """
-    DiscountLinesResponseAllOf
+    GetOrderDiscountLinesResponseAllOf
     """
-    id: Optional[StrictStr] = None
-    object: Optional[StrictStr] = None
-    parent_id: Optional[StrictStr] = None
-    __properties = ["id", "object", "parent_id"]
+    data: Optional[conlist(DiscountLinesResponse)] = None
+    __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,35 +40,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DiscountLinesResponseAllOf:
-        """Create an instance of DiscountLinesResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> GetOrderDiscountLinesResponseAllOf:
+        """Create an instance of GetOrderDiscountLinesResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DiscountLinesResponseAllOf:
-        """Create an instance of DiscountLinesResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> GetOrderDiscountLinesResponseAllOf:
+        """Create an instance of GetOrderDiscountLinesResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DiscountLinesResponseAllOf.parse_obj(obj)
+            return GetOrderDiscountLinesResponseAllOf.parse_obj(obj)
 
-        _obj = DiscountLinesResponseAllOf.parse_obj({
-            "id": obj.get("id"),
-            "object": obj.get("object"),
-            "parent_id": obj.get("parent_id")
+        _obj = GetOrderDiscountLinesResponseAllOf.parse_obj({
+            "data": [DiscountLinesResponse.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/email_checkout_request.py` & `conekta-6.0.1/conekta/models/email_checkout_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/error.py` & `conekta-6.0.1/conekta/models/error.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/error_all_of.py` & `conekta-6.0.1/conekta/models/error_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/event_response.py` & `conekta-6.0.1/conekta/models/event_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/events_resend_response.py` & `conekta-6.0.1/conekta/models/events_resend_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_api_keys_response.py` & `conekta-6.0.1/conekta/models/get_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_api_keys_response_all_of.py` & `conekta-6.0.1/conekta/models/get_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_charges_response.py` & `conekta-6.0.1/conekta/models/get_charges_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_charges_response_all_of.py` & `conekta-6.0.1/conekta/models/get_charges_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_companies_response.py` & `conekta-6.0.1/conekta/models/get_companies_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_companies_response_all_of.py` & `conekta-6.0.1/conekta/models/get_companies_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_customer_payment_method_data_response.py` & `conekta-6.0.1/conekta/models/get_customer_payment_method_data_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_events_response.py` & `conekta-6.0.1/conekta/models/get_events_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_events_response_all_of.py` & `conekta-6.0.1/conekta/models/get_events_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_orders_response.py` & `conekta-6.0.1/conekta/models/get_orders_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_payment_method_response.py` & `conekta-6.0.1/conekta/models/get_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_payment_method_response_all_of.py` & `conekta-6.0.1/conekta/models/get_payment_method_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_plans_response.py` & `conekta-6.0.1/conekta/models/get_plans_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_plans_response_all_of.py` & `conekta-6.0.1/conekta/models/get_plans_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_transactions_response.py` & `conekta-6.0.1/conekta/models/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_transactions_response_all_of.py` & `conekta-6.0.1/conekta/models/get_transactions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_transfers_response.py` & `conekta-6.0.1/conekta/models/get_transfers_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_transfers_response_all_of.py` & `conekta-6.0.1/conekta/models/get_transfers_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_webhook_keys_response.py` & `conekta-6.0.1/conekta/models/get_webhook_keys_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_webhook_keys_response_all_of.py` & `conekta-6.0.1/conekta/models/get_webhook_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_webhooks_response.py` & `conekta-6.0.1/conekta/models/get_webhooks_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/get_webhooks_response_all_of.py` & `conekta-6.0.1/conekta/models/get_webhooks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/log_response.py` & `conekta-6.0.1/conekta/models/log_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/logs_response.py` & `conekta-6.0.1/conekta/models/logs_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/logs_response_data.py` & `conekta-6.0.1/conekta/models/logs_response_data.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_capture_request.py` & `conekta-6.0.1/conekta/models/order_capture_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_discount_lines_request.py` & `conekta-6.0.1/conekta/models/order_discount_lines_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_refund_request.py` & `conekta-6.0.1/conekta/models/order_refund_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_request.py` & `conekta-6.0.1/conekta/models/order_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, conlist, constr
+from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 from conekta.models.charge_request import ChargeRequest
 from conekta.models.checkout_request import CheckoutRequest
 from conekta.models.customer_shipping_contacts import CustomerShippingContacts
 from conekta.models.order_discount_lines_request import OrderDiscountLinesRequest
 from conekta.models.order_request_customer_info import OrderRequestCustomerInfo
 from conekta.models.order_tax_request import OrderTaxRequest
 from conekta.models.product import Product
@@ -36,21 +36,22 @@
     """
     charges: Optional[conlist(ChargeRequest)] = Field(None, description="List of [charges](https://developers.conekta.com/v2.1.0/reference/orderscreatecharge) that are applied to the order")
     checkout: Optional[CheckoutRequest] = None
     currency: constr(strict=True, max_length=3) = Field(..., description="Currency with which the payment will be made. It uses the 3-letter code of the [International Standard ISO 4217.](https://es.wikipedia.org/wiki/ISO_4217)")
     customer_info: OrderRequestCustomerInfo = Field(...)
     discount_lines: Optional[conlist(OrderDiscountLinesRequest)] = Field(None, description="List of [discounts](https://developers.conekta.com/v2.1.0/reference/orderscreatediscountline) that are applied to the order. You must have at least one discount.")
     line_items: conlist(Product) = Field(..., description="List of [products](https://developers.conekta.com/v2.1.0/reference/orderscreateproduct) that are sold in the order. You must have at least one product.")
-    metadata: Optional[Dict[str, Any]] = None
+    metadata: Optional[Dict[str, Any]] = Field(None, description="Metadata associated with the order")
     needs_shipping_contact: Optional[StrictBool] = Field(None, description="Allows you to fill out the shipping information at checkout")
     pre_authorize: Optional[StrictBool] = Field(False, description="Indicates whether the order charges must be preauthorized")
+    processing_mode: Optional[StrictStr] = Field(None, description="Indicates the processing mode for the order, either ecommerce, recurrent or validation.")
     shipping_contact: Optional[CustomerShippingContacts] = None
     shipping_lines: Optional[conlist(ShippingRequest)] = Field(None, description="List of [shipping costs](https://developers.conekta.com/v2.1.0/reference/orderscreateshipping). If the online store offers digital products.")
     tax_lines: Optional[conlist(OrderTaxRequest)] = Field(None, description="List of [taxes](https://developers.conekta.com/v2.1.0/reference/orderscreatetaxes) that are applied to the order.")
-    __properties = ["charges", "checkout", "currency", "customer_info", "discount_lines", "line_items", "metadata", "needs_shipping_contact", "pre_authorize", "shipping_contact", "shipping_lines", "tax_lines"]
+    __properties = ["charges", "checkout", "currency", "customer_info", "discount_lines", "line_items", "metadata", "needs_shipping_contact", "pre_authorize", "processing_mode", "shipping_contact", "shipping_lines", "tax_lines"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -133,13 +134,14 @@
             "currency": obj.get("currency"),
             "customer_info": OrderRequestCustomerInfo.from_dict(obj.get("customer_info")) if obj.get("customer_info") is not None else None,
             "discount_lines": [OrderDiscountLinesRequest.from_dict(_item) for _item in obj.get("discount_lines")] if obj.get("discount_lines") is not None else None,
             "line_items": [Product.from_dict(_item) for _item in obj.get("line_items")] if obj.get("line_items") is not None else None,
             "metadata": obj.get("metadata"),
             "needs_shipping_contact": obj.get("needs_shipping_contact"),
             "pre_authorize": obj.get("pre_authorize") if obj.get("pre_authorize") is not None else False,
+            "processing_mode": obj.get("processing_mode"),
             "shipping_contact": CustomerShippingContacts.from_dict(obj.get("shipping_contact")) if obj.get("shipping_contact") is not None else None,
             "shipping_lines": [ShippingRequest.from_dict(_item) for _item in obj.get("shipping_lines")] if obj.get("shipping_lines") is not None else None,
             "tax_lines": [OrderTaxRequest.from_dict(_item) for _item in obj.get("tax_lines")] if obj.get("tax_lines") is not None else None
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/order_request_customer_info.py` & `conekta-6.0.1/conekta/models/order_request_customer_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 ORDERREQUESTCUSTOMERINFO_ONE_OF_SCHEMAS = ["CustomerInfo", "CustomerInfoJustCustomerId"]
 
 class OrderRequestCustomerInfo(BaseModel):
     """
-    OrderRequestCustomerInfo
+    Customer information
     """
     # data type: CustomerInfo
     oneof_schema_1_validator: Optional[CustomerInfo] = None
     # data type: CustomerInfoJustCustomerId
     oneof_schema_2_validator: Optional[CustomerInfoJustCustomerId] = None
     actual_instance: Any
     one_of_schemas: List[str] = Field(ORDERREQUESTCUSTOMERINFO_ONE_OF_SCHEMAS, const=True)
```

### Comparing `conekta-6.0.0/conekta/models/order_response.py` & `conekta-6.0.1/conekta/models/order_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,18 @@
     id: Optional[StrictStr] = None
     is_refundable: Optional[StrictBool] = None
     line_items: Optional[OrderResponseProducts] = None
     livemode: Optional[StrictBool] = Field(None, description="Whether the object exists in live mode or test mode")
     metadata: Optional[Dict[str, Any]] = Field(None, description="Set of key-value pairs that you can attach to an object. This can be useful for storing additional information about the object in a structured format.")
     object: Optional[StrictStr] = Field(None, description="String representing the object’s type. Objects of the same type share the same value.")
     payment_status: Optional[StrictStr] = Field(None, description="The payment status of the order.")
+    processing_mode: Optional[StrictStr] = Field(None, description="Indicates the processing mode for the order, either ecommerce, recurrent or validation.")
     shipping_contact: Optional[OrderResponseShippingContact] = None
     updated_at: Optional[StrictInt] = Field(None, description="The time at which the object was last updated in seconds since the Unix epoch")
-    __properties = ["amount", "amount_refunded", "channel", "charges", "checkout", "created_at", "currency", "customer_info", "discount_lines", "fiscal_entity", "id", "is_refundable", "line_items", "livemode", "metadata", "object", "payment_status", "shipping_contact", "updated_at"]
+    __properties = ["amount", "amount_refunded", "channel", "charges", "checkout", "created_at", "currency", "customer_info", "discount_lines", "fiscal_entity", "id", "is_refundable", "line_items", "livemode", "metadata", "object", "payment_status", "processing_mode", "shipping_contact", "updated_at"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -128,12 +129,13 @@
             "id": obj.get("id"),
             "is_refundable": obj.get("is_refundable"),
             "line_items": OrderResponseProducts.from_dict(obj.get("line_items")) if obj.get("line_items") is not None else None,
             "livemode": obj.get("livemode"),
             "metadata": obj.get("metadata"),
             "object": obj.get("object"),
             "payment_status": obj.get("payment_status"),
+            "processing_mode": obj.get("processing_mode"),
             "shipping_contact": OrderResponseShippingContact.from_dict(obj.get("shipping_contact")) if obj.get("shipping_contact") is not None else None,
             "updated_at": obj.get("updated_at")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/order_response_charges.py` & `conekta-6.0.1/conekta/models/order_response_charges.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_charges_all_of.py` & `conekta-6.0.1/conekta/models/order_response_charges_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_checkout.py` & `conekta-6.0.1/conekta/models/order_response_checkout.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_customer_info.py` & `conekta-6.0.1/conekta/models/order_response_customer_info.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_customer_info_all_of.py` & `conekta-6.0.1/conekta/models/order_response_customer_info_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_discount_lines.py` & `conekta-6.0.1/conekta/models/order_response_discount_lines.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_discount_lines_all_of.py` & `conekta-6.0.1/conekta/models/order_response_discount_lines_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_fiscal_entity.py` & `conekta-6.0.1/conekta/models/order_response_fiscal_entity.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_fiscal_entity_address.py` & `conekta-6.0.1/conekta/models/order_response_fiscal_entity_address.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_fiscal_entity_address_all_of.py` & `conekta-6.0.1/conekta/models/order_response_fiscal_entity_address_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_products.py` & `conekta-6.0.1/conekta/models/order_response_products.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_products_all_of.py` & `conekta-6.0.1/conekta/models/order_response_products_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_shipping_contact.py` & `conekta-6.0.1/conekta/models/order_response_shipping_contact.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_response_shipping_contact_all_of.py` & `conekta-6.0.1/conekta/models/order_response_shipping_contact_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_tax_request.py` & `conekta-6.0.1/conekta/models/order_tax_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/order_update_request.py` & `conekta-6.0.1/conekta/models/order_update_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 from typing import Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 from conekta.models.charge_request import ChargeRequest
 from conekta.models.checkout_request import CheckoutRequest
 from conekta.models.customer_shipping_contacts import CustomerShippingContacts
 from conekta.models.order_discount_lines_request import OrderDiscountLinesRequest
-from conekta.models.order_request_customer_info import OrderRequestCustomerInfo
 from conekta.models.order_tax_request import OrderTaxRequest
+from conekta.models.order_update_request_customer_info import OrderUpdateRequestCustomerInfo
 from conekta.models.product import Product
 from conekta.models.shipping_request import ShippingRequest
 
 class OrderUpdateRequest(BaseModel):
     """
     a order
     """
     charges: Optional[conlist(ChargeRequest)] = None
     checkout: Optional[CheckoutRequest] = None
     currency: Optional[constr(strict=True, max_length=3)] = Field(None, description="Currency with which the payment will be made. It uses the 3-letter code of the [International Standard ISO 4217.](https://es.wikipedia.org/wiki/ISO_4217)")
-    customer_info: Optional[OrderRequestCustomerInfo] = None
+    customer_info: Optional[OrderUpdateRequestCustomerInfo] = None
     discount_lines: Optional[conlist(OrderDiscountLinesRequest)] = Field(None, description="List of [discounts](https://developers.conekta.com/v2.1.0/reference/orderscreatediscountline) that are applied to the order. You must have at least one discount.")
     line_items: Optional[conlist(Product)] = Field(None, description="List of [products](https://developers.conekta.com/v2.1.0/reference/orderscreateproduct) that are sold in the order. You must have at least one product.")
     metadata: Optional[Dict[str, StrictStr]] = None
     pre_authorize: Optional[StrictBool] = Field(False, description="Indicates whether the order charges must be preauthorized")
     shipping_contact: Optional[CustomerShippingContacts] = None
     shipping_lines: Optional[conlist(ShippingRequest)] = Field(None, description="List of [shipping costs](https://developers.conekta.com/v2.1.0/reference/orderscreateshipping). If the online store offers digital products.")
     tax_lines: Optional[conlist(OrderTaxRequest)] = None
@@ -126,15 +126,15 @@
         if not isinstance(obj, dict):
             return OrderUpdateRequest.parse_obj(obj)
 
         _obj = OrderUpdateRequest.parse_obj({
             "charges": [ChargeRequest.from_dict(_item) for _item in obj.get("charges")] if obj.get("charges") is not None else None,
             "checkout": CheckoutRequest.from_dict(obj.get("checkout")) if obj.get("checkout") is not None else None,
             "currency": obj.get("currency"),
-            "customer_info": OrderRequestCustomerInfo.from_dict(obj.get("customer_info")) if obj.get("customer_info") is not None else None,
+            "customer_info": OrderUpdateRequestCustomerInfo.from_dict(obj.get("customer_info")) if obj.get("customer_info") is not None else None,
             "discount_lines": [OrderDiscountLinesRequest.from_dict(_item) for _item in obj.get("discount_lines")] if obj.get("discount_lines") is not None else None,
             "line_items": [Product.from_dict(_item) for _item in obj.get("line_items")] if obj.get("line_items") is not None else None,
             "metadata": obj.get("metadata"),
             "pre_authorize": obj.get("pre_authorize") if obj.get("pre_authorize") is not None else False,
             "shipping_contact": CustomerShippingContacts.from_dict(obj.get("shipping_contact")) if obj.get("shipping_contact") is not None else None,
             "shipping_lines": [ShippingRequest.from_dict(_item) for _item in obj.get("shipping_lines")] if obj.get("shipping_lines") is not None else None,
             "tax_lines": [OrderTaxRequest.from_dict(_item) for _item in obj.get("tax_lines")] if obj.get("tax_lines") is not None else None
```

### Comparing `conekta-6.0.0/conekta/models/orders_response.py` & `conekta-6.0.1/conekta/models/orders_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/page.py` & `conekta-6.0.1/conekta/models/page.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/pagination.py` & `conekta-6.0.1/conekta/models/payment_method_card_request_all_of.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-
-class Pagination(BaseModel):
+class PaymentMethodCardRequestAllOf(BaseModel):
     """
-    pagination metadata
+    PaymentMethodCardRequestAllOf
     """
-    has_more: StrictBool = Field(..., description="Indicates if there are more pages to be requested")
-    object: StrictStr = Field(..., description="Object type, in this case is list")
-    __properties = ["has_more", "object"]
+    token_id: Optional[StrictStr] = Field(None, description="Token id that will be used to create a \"card\" type payment method. See the (subscriptions)[https://developers.conekta.com/v2.1.0/reference/createsubscription] tutorial for more information on how to tokenize cards.")
+    __properties = ["token_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,34 +39,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Pagination:
-        """Create an instance of Pagination from a JSON string"""
+    def from_json(cls, json_str: str) -> PaymentMethodCardRequestAllOf:
+        """Create an instance of PaymentMethodCardRequestAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Pagination:
-        """Create an instance of Pagination from a dict"""
+    def from_dict(cls, obj: dict) -> PaymentMethodCardRequestAllOf:
+        """Create an instance of PaymentMethodCardRequestAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Pagination.parse_obj(obj)
+            return PaymentMethodCardRequestAllOf.parse_obj(obj)
 
-        _obj = Pagination.parse_obj({
-            "has_more": obj.get("has_more"),
-            "object": obj.get("object")
+        _obj = PaymentMethodCardRequestAllOf.parse_obj({
+            "token_id": obj.get("token_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/payment_method.py` & `conekta-6.0.1/conekta/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_bank_transfer.py` & `conekta-6.0.1/conekta/models/payment_method_bank_transfer.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_card.py` & `conekta-6.0.1/conekta/models/payment_method_card.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictStr, conlist, constr
 
 class PaymentMethodCard(BaseModel):
     """
     PaymentMethodCard
     """
     type: Optional[StrictStr] = None
     object: StrictStr = Field(...)
     account_type: Optional[StrictStr] = None
     auth_code: Optional[StrictStr] = None
     brand: Optional[StrictStr] = None
+    contract_id: Optional[constr(strict=True, max_length=10, min_length=10)] = Field(None, description="Id sent for recurrent charges.")
     country: Optional[StrictStr] = None
     exp_month: Optional[StrictStr] = None
     exp_year: Optional[StrictStr] = None
     fraud_indicators: Optional[conlist(Any)] = None
     issuer: Optional[StrictStr] = None
     last4: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
-    __properties = ["type", "object", "account_type", "auth_code", "brand", "country", "exp_month", "exp_year", "fraud_indicators", "issuer", "last4", "name"]
+    __properties = ["type", "object", "account_type", "auth_code", "brand", "contract_id", "country", "exp_month", "exp_year", "fraud_indicators", "issuer", "last4", "name"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -77,14 +78,15 @@
 
         _obj = PaymentMethodCard.parse_obj({
             "type": obj.get("type"),
             "object": obj.get("object"),
             "account_type": obj.get("account_type"),
             "auth_code": obj.get("auth_code"),
             "brand": obj.get("brand"),
+            "contract_id": obj.get("contract_id"),
             "country": obj.get("country"),
             "exp_month": obj.get("exp_month"),
             "exp_year": obj.get("exp_year"),
             "fraud_indicators": obj.get("fraud_indicators"),
             "issuer": obj.get("issuer"),
             "last4": obj.get("last4"),
             "name": obj.get("name")
```

### Comparing `conekta-6.0.0/conekta/models/payment_method_card_request.py` & `conekta-6.0.1/conekta/models/payment_method_card_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_card_request_all_of.py` & `conekta-6.0.1/conekta/models/payment_method_spei_recurrent_all_of.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr
 
-class PaymentMethodCardRequestAllOf(BaseModel):
+class PaymentMethodSpeiRecurrentAllOf(BaseModel):
     """
-    PaymentMethodCardRequestAllOf
+    use for spei responses
     """
-    token_id: Optional[StrictStr] = Field(None, description="Token id that will be used to create a \"card\" type payment method. See the (subscriptions)[https://developers.conekta.com/v2.1.0/reference/createsubscription] tutorial for more information on how to tokenize cards.")
-    __properties = ["token_id"]
+    reference: Optional[StrictStr] = None
+    expires_at: Optional[StrictStr] = None
+    __properties = ["reference", "expires_at"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PaymentMethodCardRequestAllOf:
-        """Create an instance of PaymentMethodCardRequestAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> PaymentMethodSpeiRecurrentAllOf:
+        """Create an instance of PaymentMethodSpeiRecurrentAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PaymentMethodCardRequestAllOf:
-        """Create an instance of PaymentMethodCardRequestAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> PaymentMethodSpeiRecurrentAllOf:
+        """Create an instance of PaymentMethodSpeiRecurrentAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PaymentMethodCardRequestAllOf.parse_obj(obj)
+            return PaymentMethodSpeiRecurrentAllOf.parse_obj(obj)
 
-        _obj = PaymentMethodCardRequestAllOf.parse_obj({
-            "token_id": obj.get("token_id")
+        _obj = PaymentMethodSpeiRecurrentAllOf.parse_obj({
+            "reference": obj.get("reference"),
+            "expires_at": obj.get("expires_at")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/payment_method_card_response.py` & `conekta-6.0.1/conekta/models/payment_method_card_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_card_response_all_of.py` & `conekta-6.0.1/conekta/models/payment_method_card_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_cash.py` & `conekta-6.0.1/conekta/models/payment_method_cash.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_cash_request.py` & `conekta-6.0.1/conekta/models/payment_method_cash_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_cash_request_all_of.py` & `conekta-6.0.1/conekta/models/payment_method_cash_request_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_cash_response.py` & `conekta-6.0.1/conekta/models/payment_method_cash_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_cash_response_all_of.py` & `conekta-6.0.1/conekta/models/payment_method_cash_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_response.py` & `conekta-6.0.1/conekta/models/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_spei_recurrent.py` & `conekta-6.0.1/conekta/models/payment_method_spei_recurrent.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/payment_method_spei_recurrent_all_of.py` & `conekta-6.0.1/conekta/models/product_order_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 
-class PaymentMethodSpeiRecurrentAllOf(BaseModel):
+class ProductOrderResponseAllOf(BaseModel):
     """
-    use for spei responses
+    ProductOrderResponseAllOf
     """
-    reference: Optional[StrictStr] = None
-    expires_at: Optional[StrictStr] = None
-    __properties = ["reference", "expires_at"]
+    id: Optional[StrictStr] = None
+    object: Optional[StrictStr] = None
+    parent_id: Optional[StrictStr] = None
+    __properties = ["id", "object", "parent_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,34 +41,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PaymentMethodSpeiRecurrentAllOf:
-        """Create an instance of PaymentMethodSpeiRecurrentAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> ProductOrderResponseAllOf:
+        """Create an instance of ProductOrderResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PaymentMethodSpeiRecurrentAllOf:
-        """Create an instance of PaymentMethodSpeiRecurrentAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> ProductOrderResponseAllOf:
+        """Create an instance of ProductOrderResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PaymentMethodSpeiRecurrentAllOf.parse_obj(obj)
+            return ProductOrderResponseAllOf.parse_obj(obj)
 
-        _obj = PaymentMethodSpeiRecurrentAllOf.parse_obj({
-            "reference": obj.get("reference"),
-            "expires_at": obj.get("expires_at")
+        _obj = ProductOrderResponseAllOf.parse_obj({
+            "id": obj.get("id"),
+            "object": obj.get("object"),
+            "parent_id": obj.get("parent_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/payment_method_spei_request.py` & `conekta-6.0.1/conekta/models/payment_method_spei_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/plan_request.py` & `conekta-6.0.1/conekta/models/plan_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/plan_response.py` & `conekta-6.0.1/conekta/models/plan_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/plan_update_request.py` & `conekta-6.0.1/conekta/models/plan_update_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/product.py` & `conekta-6.0.1/conekta/models/product.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/product_data_response.py` & `conekta-6.0.1/conekta/models/product_data_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/product_data_response_all_of.py` & `conekta-6.0.1/conekta/models/product_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/product_order_response.py` & `conekta-6.0.1/conekta/models/product_order_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/product_order_response_all_of.py` & `conekta-6.0.1/conekta/models/update_order_tax_response_all_of.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 
-class ProductOrderResponseAllOf(BaseModel):
+class UpdateOrderTaxResponseAllOf(BaseModel):
     """
-    ProductOrderResponseAllOf
+    UpdateOrderTaxResponseAllOf
     """
     id: Optional[StrictStr] = None
     object: Optional[StrictStr] = None
     parent_id: Optional[StrictStr] = None
     __properties = ["id", "object", "parent_id"]
 
     class Config:
@@ -41,35 +41,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ProductOrderResponseAllOf:
-        """Create an instance of ProductOrderResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrderTaxResponseAllOf:
+        """Create an instance of UpdateOrderTaxResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ProductOrderResponseAllOf:
-        """Create an instance of ProductOrderResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrderTaxResponseAllOf:
+        """Create an instance of UpdateOrderTaxResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ProductOrderResponseAllOf.parse_obj(obj)
+            return UpdateOrderTaxResponseAllOf.parse_obj(obj)
 
-        _obj = ProductOrderResponseAllOf.parse_obj({
+        _obj = UpdateOrderTaxResponseAllOf.parse_obj({
             "id": obj.get("id"),
             "object": obj.get("object"),
             "parent_id": obj.get("parent_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/risk_rules.py` & `conekta-6.0.1/conekta/models/risk_rules.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/risk_rules_data.py` & `conekta-6.0.1/conekta/models/token_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,27 +17,26 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
+from conekta.models.token_response_checkout import TokenResponseCheckout
 
-class RiskRulesData(BaseModel):
+class TokenResponse(BaseModel):
     """
-    RiskRulesData
+    token response
     """
-    id: Optional[StrictStr] = Field(None, description="rule id")
-    field: Optional[StrictStr] = Field(None, description="field to be used for the rule")
-    created_at: Optional[StrictStr] = Field(None, description="rule creation date")
-    value: Optional[StrictStr] = Field(None, description="value to be used for the rule")
-    is_global: Optional[StrictBool] = Field(None, description="if the rule is global")
-    is_test: Optional[StrictBool] = Field(None, description="if the rule is test")
-    description: Optional[StrictStr] = Field(None, description="description of the rule")
-    __properties = ["id", "field", "created_at", "value", "is_global", "is_test", "description"]
+    checkout: Optional[TokenResponseCheckout] = None
+    id: StrictStr = Field(..., description="Unique identifier for the token generated by Conekta.")
+    livemode: StrictBool = Field(..., description="Indicates whether the token is in live mode or test mode.")
+    object: StrictStr = Field(..., description="Indicates the type of object, in this case token")
+    used: StrictBool = Field(..., description="Indicates if the token has been used")
+    __properties = ["checkout", "id", "livemode", "object", "used"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -45,39 +44,45 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> RiskRulesData:
-        """Create an instance of RiskRulesData from a JSON string"""
+    def from_json(cls, json_str: str) -> TokenResponse:
+        """Create an instance of TokenResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of checkout
+        if self.checkout:
+            _dict['checkout'] = self.checkout.to_dict()
+        # set to None if checkout (nullable) is None
+        # and __fields_set__ contains the field
+        if self.checkout is None and "checkout" in self.__fields_set__:
+            _dict['checkout'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> RiskRulesData:
-        """Create an instance of RiskRulesData from a dict"""
+    def from_dict(cls, obj: dict) -> TokenResponse:
+        """Create an instance of TokenResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return RiskRulesData.parse_obj(obj)
+            return TokenResponse.parse_obj(obj)
 
-        _obj = RiskRulesData.parse_obj({
+        _obj = TokenResponse.parse_obj({
+            "checkout": TokenResponseCheckout.from_dict(obj.get("checkout")) if obj.get("checkout") is not None else None,
             "id": obj.get("id"),
-            "field": obj.get("field"),
-            "created_at": obj.get("created_at"),
-            "value": obj.get("value"),
-            "is_global": obj.get("is_global"),
-            "is_test": obj.get("is_test"),
-            "description": obj.get("description")
+            "livemode": obj.get("livemode"),
+            "object": obj.get("object"),
+            "used": obj.get("used")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/risk_rules_list.py` & `conekta-6.0.1/conekta/models/risk_rules_list.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/shipping_order_response.py` & `conekta-6.0.1/conekta/models/shipping_order_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/shipping_request.py` & `conekta-6.0.1/conekta/models/shipping_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/sms_checkout_request.py` & `conekta-6.0.1/conekta/models/sms_checkout_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/subscription_events_response.py` & `conekta-6.0.1/conekta/models/subscription_events_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/subscription_request.py` & `conekta-6.0.1/conekta/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/subscription_response.py` & `conekta-6.0.1/conekta/models/subscription_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/subscription_update_request.py` & `conekta-6.0.1/conekta/models/subscription_update_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/token.py` & `conekta-6.0.1/conekta/models/token.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/token_card.py` & `conekta-6.0.1/conekta/models/token_card.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/token_checkout.py` & `conekta-6.0.1/conekta/models/token_checkout.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/token_response.py` & `conekta-6.0.1/conekta/models/whitelistlist_rule_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-from conekta.models.token_response_checkout import TokenResponseCheckout
+from pydantic import BaseModel, Field, StrictStr
 
-class TokenResponse(BaseModel):
+class WhitelistlistRuleResponse(BaseModel):
     """
-    token response
+    WhitelistlistRuleResponse
     """
-    checkout: Optional[TokenResponseCheckout] = None
-    id: StrictStr = Field(..., description="Unique identifier for the token generated by Conekta.")
-    livemode: StrictBool = Field(..., description="Indicates whether the token is in live mode or test mode.")
-    object: StrictStr = Field(..., description="Indicates the type of object, in this case token")
-    used: StrictBool = Field(..., description="Indicates if the token has been used")
-    __properties = ["checkout", "id", "livemode", "object", "used"]
+    id: Optional[StrictStr] = Field(None, description="Whitelist rule id")
+    field: Optional[StrictStr] = Field(None, description="field used for whitelists rule")
+    value: Optional[StrictStr] = Field(None, description="value used for whitelists rule")
+    description: Optional[StrictStr] = Field(None, description="use an description for whitelisted rule")
+    __properties = ["id", "field", "value", "description"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -44,45 +42,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TokenResponse:
-        """Create an instance of TokenResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelistlistRuleResponse:
+        """Create an instance of WhitelistlistRuleResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of checkout
-        if self.checkout:
-            _dict['checkout'] = self.checkout.to_dict()
-        # set to None if checkout (nullable) is None
-        # and __fields_set__ contains the field
-        if self.checkout is None and "checkout" in self.__fields_set__:
-            _dict['checkout'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TokenResponse:
-        """Create an instance of TokenResponse from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelistlistRuleResponse:
+        """Create an instance of WhitelistlistRuleResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return TokenResponse.parse_obj(obj)
+            return WhitelistlistRuleResponse.parse_obj(obj)
 
-        _obj = TokenResponse.parse_obj({
-            "checkout": TokenResponseCheckout.from_dict(obj.get("checkout")) if obj.get("checkout") is not None else None,
+        _obj = WhitelistlistRuleResponse.parse_obj({
             "id": obj.get("id"),
-            "livemode": obj.get("livemode"),
-            "object": obj.get("object"),
-            "used": obj.get("used")
+            "field": obj.get("field"),
+            "value": obj.get("value"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/token_response_checkout.py` & `conekta-6.0.1/conekta/models/token_response_checkout.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/transaction_response.py` & `conekta-6.0.1/conekta/models/transaction_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/transfer_destination_response.py` & `conekta-6.0.1/conekta/models/transfer_destination_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/transfer_method_response.py` & `conekta-6.0.1/conekta/models/transfer_method_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/transfer_response.py` & `conekta-6.0.1/conekta/models/transfer_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/transfers_response.py` & `conekta-6.0.1/conekta/models/transfers_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_customer.py` & `conekta-6.0.1/conekta/models/update_customer.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_customer_antifraud_info.py` & `conekta-6.0.1/conekta/models/update_customer_antifraud_info.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response.py` & `conekta-6.0.1/conekta/models/update_customer_fiscal_entities_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response_all_of.py` & `conekta-6.0.1/conekta/models/update_customer_fiscal_entities_response_all_of.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_customer_payment_methods_response.py` & `conekta-6.0.1/conekta/models/update_customer_payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_order_discount_lines_request.py` & `conekta-6.0.1/conekta/models/update_order_tax_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, conint
+from typing import Any, Dict, Optional
+from pydantic import BaseModel, Field, conint, constr
 
-class UpdateOrderDiscountLinesRequest(BaseModel):
+class UpdateOrderTaxRequest(BaseModel):
     """
-    List of discounts that apply to the order.
+    create new taxes for an existing order
     """
-    amount: Optional[conint(strict=True, ge=0)] = None
-    code: Optional[StrictStr] = Field(None, description="Discount code.")
-    type: Optional[StrictStr] = None
-    __properties = ["amount", "code", "type"]
+    amount: Optional[conint(strict=True, ge=0)] = Field(None, description="The amount to be collected for tax in cents")
+    description: Optional[constr(strict=True, min_length=2)] = Field(None, description="description or tax's name")
+    metadata: Optional[Dict[str, Dict[str, Any]]] = None
+    __properties = ["amount", "description", "metadata"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,35 +41,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrderDiscountLinesRequest:
-        """Create an instance of UpdateOrderDiscountLinesRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrderTaxRequest:
+        """Create an instance of UpdateOrderTaxRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrderDiscountLinesRequest:
-        """Create an instance of UpdateOrderDiscountLinesRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrderTaxRequest:
+        """Create an instance of UpdateOrderTaxRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateOrderDiscountLinesRequest.parse_obj(obj)
+            return UpdateOrderTaxRequest.parse_obj(obj)
 
-        _obj = UpdateOrderDiscountLinesRequest.parse_obj({
+        _obj = UpdateOrderTaxRequest.parse_obj({
             "amount": obj.get("amount"),
-            "code": obj.get("code"),
-            "type": obj.get("type")
+            "description": obj.get("description"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/update_order_tax_request.py` & `conekta-6.0.1/conekta/models/update_order_tax_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, conint, constr
+from pydantic import BaseModel, Field, StrictStr, conint, constr
 
-class UpdateOrderTaxRequest(BaseModel):
+class UpdateOrderTaxResponse(BaseModel):
     """
-    create new taxes for an existing order
+    create new taxes for an existing order response
     """
-    amount: Optional[conint(strict=True, ge=0)] = Field(None, description="The amount to be collected for tax in cents")
-    description: Optional[constr(strict=True, min_length=2)] = Field(None, description="description or tax's name")
-    metadata: Optional[Dict[str, Dict[str, Any]]] = None
-    __properties = ["amount", "description", "metadata"]
+    amount: conint(strict=True, ge=0) = Field(..., description="The amount to be collected for tax in cents")
+    description: constr(strict=True, min_length=2) = Field(..., description="description or tax's name")
+    metadata: Optional[Dict[str, Any]] = None
+    id: StrictStr = Field(...)
+    object: Optional[StrictStr] = None
+    parent_id: Optional[StrictStr] = None
+    __properties = ["amount", "description", "metadata", "id", "object", "parent_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,35 +44,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrderTaxRequest:
-        """Create an instance of UpdateOrderTaxRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrderTaxResponse:
+        """Create an instance of UpdateOrderTaxResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrderTaxRequest:
-        """Create an instance of UpdateOrderTaxRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrderTaxResponse:
+        """Create an instance of UpdateOrderTaxResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateOrderTaxRequest.parse_obj(obj)
+            return UpdateOrderTaxResponse.parse_obj(obj)
 
-        _obj = UpdateOrderTaxRequest.parse_obj({
+        _obj = UpdateOrderTaxResponse.parse_obj({
             "amount": obj.get("amount"),
             "description": obj.get("description"),
-            "metadata": obj.get("metadata")
+            "metadata": obj.get("metadata"),
+            "id": obj.get("id"),
+            "object": obj.get("object"),
+            "parent_id": obj.get("parent_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/update_order_tax_response.py` & `conekta-6.0.1/conekta/models/balance_common_field.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,28 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, conint, constr
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class UpdateOrderTaxResponse(BaseModel):
+class BalanceCommonField(BaseModel):
     """
-    create new taxes for an existing order response
+    balance common fields model
     """
-    amount: conint(strict=True, ge=0) = Field(..., description="The amount to be collected for tax in cents")
-    description: constr(strict=True, min_length=2) = Field(..., description="description or tax's name")
-    metadata: Optional[Dict[str, Any]] = None
-    id: StrictStr = Field(...)
-    object: Optional[StrictStr] = None
-    parent_id: Optional[StrictStr] = None
-    __properties = ["amount", "description", "metadata", "id", "object", "parent_id"]
+    amount: Optional[StrictInt] = Field(None, description="The balance's amount")
+    currency: Optional[StrictStr] = Field(None, description="The balance's currency")
+    __properties = ["amount", "currency"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -44,38 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrderTaxResponse:
-        """Create an instance of UpdateOrderTaxResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> BalanceCommonField:
+        """Create an instance of BalanceCommonField from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrderTaxResponse:
-        """Create an instance of UpdateOrderTaxResponse from a dict"""
+    def from_dict(cls, obj: dict) -> BalanceCommonField:
+        """Create an instance of BalanceCommonField from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateOrderTaxResponse.parse_obj(obj)
+            return BalanceCommonField.parse_obj(obj)
 
-        _obj = UpdateOrderTaxResponse.parse_obj({
+        _obj = BalanceCommonField.parse_obj({
             "amount": obj.get("amount"),
-            "description": obj.get("description"),
-            "metadata": obj.get("metadata"),
-            "id": obj.get("id"),
-            "object": obj.get("object"),
-            "parent_id": obj.get("parent_id")
+            "currency": obj.get("currency")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/update_order_tax_response_all_of.py` & `conekta-6.0.1/conekta/models/update_product.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, StrictStr, conint, conlist, constr
 
-class UpdateOrderTaxResponseAllOf(BaseModel):
+class UpdateProduct(BaseModel):
     """
-    UpdateOrderTaxResponseAllOf
+    UpdateProduct
     """
-    id: Optional[StrictStr] = None
-    object: Optional[StrictStr] = None
-    parent_id: Optional[StrictStr] = None
-    __properties = ["id", "object", "parent_id"]
+    antifraud_info: Optional[Dict[str, Dict[str, Any]]] = None
+    description: Optional[constr(strict=True, max_length=250)] = None
+    sku: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    unit_price: Optional[conint(strict=True, ge=0)] = None
+    quantity: Optional[conint(strict=True, ge=1)] = None
+    tags: Optional[conlist(StrictStr)] = None
+    brand: Optional[StrictStr] = None
+    metadata: Optional[Dict[str, StrictStr]] = None
+    __properties = ["antifraud_info", "description", "sku", "name", "unit_price", "quantity", "tags", "brand", "metadata"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,35 +47,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrderTaxResponseAllOf:
-        """Create an instance of UpdateOrderTaxResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateProduct:
+        """Create an instance of UpdateProduct from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrderTaxResponseAllOf:
-        """Create an instance of UpdateOrderTaxResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateProduct:
+        """Create an instance of UpdateProduct from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateOrderTaxResponseAllOf.parse_obj(obj)
+            return UpdateProduct.parse_obj(obj)
 
-        _obj = UpdateOrderTaxResponseAllOf.parse_obj({
-            "id": obj.get("id"),
-            "object": obj.get("object"),
-            "parent_id": obj.get("parent_id")
+        _obj = UpdateProduct.parse_obj({
+            "antifraud_info": obj.get("antifraud_info"),
+            "description": obj.get("description"),
+            "sku": obj.get("sku"),
+            "name": obj.get("name"),
+            "unit_price": obj.get("unit_price"),
+            "quantity": obj.get("quantity"),
+            "tags": obj.get("tags"),
+            "brand": obj.get("brand"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/update_payment_methods.py` & `conekta-6.0.1/conekta/models/update_payment_methods.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/update_product.py` & `conekta-6.0.1/conekta/models/webhook_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,31 +15,32 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, StrictStr, conint, conlist, constr
+from typing import List, Optional
+from pydantic import BaseModel, StrictBool, StrictStr, conlist
 
-class UpdateProduct(BaseModel):
+class WebhookResponse(BaseModel):
     """
-    UpdateProduct
+    webhooks model
     """
-    antifraud_info: Optional[Dict[str, Dict[str, Any]]] = None
-    description: Optional[constr(strict=True, max_length=250)] = None
-    sku: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    unit_price: Optional[conint(strict=True, ge=0)] = None
-    quantity: Optional[conint(strict=True, ge=1)] = None
-    tags: Optional[conlist(StrictStr)] = None
-    brand: Optional[StrictStr] = None
-    metadata: Optional[Dict[str, StrictStr]] = None
-    __properties = ["antifraud_info", "description", "sku", "name", "unit_price", "quantity", "tags", "brand", "metadata"]
+    deleted: Optional[StrictBool] = None
+    development_enabled: Optional[StrictBool] = None
+    id: Optional[StrictStr] = None
+    livemode: Optional[StrictBool] = None
+    object: Optional[StrictStr] = None
+    production_enabled: Optional[StrictBool] = None
+    status: Optional[StrictStr] = None
+    subscribed_events: Optional[conlist(StrictStr)] = None
+    synchronous: Optional[StrictBool] = None
+    url: Optional[StrictStr] = None
+    __properties = ["deleted", "development_enabled", "id", "livemode", "object", "production_enabled", "status", "subscribed_events", "synchronous", "url"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,41 +48,47 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateProduct:
-        """Create an instance of UpdateProduct from a JSON string"""
+    def from_json(cls, json_str: str) -> WebhookResponse:
+        """Create an instance of WebhookResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if deleted (nullable) is None
+        # and __fields_set__ contains the field
+        if self.deleted is None and "deleted" in self.__fields_set__:
+            _dict['deleted'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateProduct:
-        """Create an instance of UpdateProduct from a dict"""
+    def from_dict(cls, obj: dict) -> WebhookResponse:
+        """Create an instance of WebhookResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateProduct.parse_obj(obj)
+            return WebhookResponse.parse_obj(obj)
 
-        _obj = UpdateProduct.parse_obj({
-            "antifraud_info": obj.get("antifraud_info"),
-            "description": obj.get("description"),
-            "sku": obj.get("sku"),
-            "name": obj.get("name"),
-            "unit_price": obj.get("unit_price"),
-            "quantity": obj.get("quantity"),
-            "tags": obj.get("tags"),
-            "brand": obj.get("brand"),
-            "metadata": obj.get("metadata")
+        _obj = WebhookResponse.parse_obj({
+            "deleted": obj.get("deleted"),
+            "development_enabled": obj.get("development_enabled"),
+            "id": obj.get("id"),
+            "livemode": obj.get("livemode"),
+            "object": obj.get("object"),
+            "production_enabled": obj.get("production_enabled"),
+            "status": obj.get("status"),
+            "subscribed_events": obj.get("subscribed_events"),
+            "synchronous": obj.get("synchronous"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/webhook_key_create_response.py` & `conekta-6.0.1/conekta/models/webhook_key_create_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/webhook_key_delete_response.py` & `conekta-6.0.1/conekta/models/webhook_key_delete_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/webhook_key_request.py` & `conekta-6.0.1/conekta/models/webhook_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool
+from typing import Any, Dict, Optional
+from pydantic import BaseModel, StrictInt, StrictStr
 
-class WebhookKeyRequest(BaseModel):
+class WebhookLog(BaseModel):
     """
-    WebhookKeyRequest
+    WebhookLog
     """
-    active: Optional[StrictBool] = Field(True, description="Indicates if the webhook key is active")
-    __properties = ["active"]
+    failed_attempts: Optional[StrictInt] = None
+    id: Optional[StrictStr] = None
+    last_attempted_at: Optional[StrictInt] = None
+    last_http_response_status: Optional[StrictInt] = None
+    object: Optional[StrictStr] = None
+    response_data: Optional[Dict[str, Any]] = None
+    url: Optional[StrictStr] = None
+    __properties = ["failed_attempts", "id", "last_attempted_at", "last_http_response_status", "object", "response_data", "url"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +45,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebhookKeyRequest:
-        """Create an instance of WebhookKeyRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> WebhookLog:
+        """Create an instance of WebhookLog from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WebhookKeyRequest:
-        """Create an instance of WebhookKeyRequest from a dict"""
+    def from_dict(cls, obj: dict) -> WebhookLog:
+        """Create an instance of WebhookLog from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WebhookKeyRequest.parse_obj(obj)
+            return WebhookLog.parse_obj(obj)
 
-        _obj = WebhookKeyRequest.parse_obj({
-            "active": obj.get("active") if obj.get("active") is not None else True
+        _obj = WebhookLog.parse_obj({
+            "failed_attempts": obj.get("failed_attempts"),
+            "id": obj.get("id"),
+            "last_attempted_at": obj.get("last_attempted_at"),
+            "last_http_response_status": obj.get("last_http_response_status"),
+            "object": obj.get("object"),
+            "response_data": obj.get("response_data"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/models/webhook_key_response.py` & `conekta-6.0.1/conekta/models/webhook_key_response.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/webhook_key_update_request.py` & `conekta-6.0.1/conekta/models/webhook_key_update_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/webhook_request.py` & `conekta-6.0.1/conekta/models/webhook_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/webhook_update_request.py` & `conekta-6.0.1/conekta/models/webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta/models/whitelistlist_rule_response.py` & `conekta-6.0.1/conekta/models/discount_lines_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
-class WhitelistlistRuleResponse(BaseModel):
+from pydantic import BaseModel, Field, StrictStr, conint
+
+class DiscountLinesResponse(BaseModel):
     """
-    WhitelistlistRuleResponse
+    DiscountLinesResponse
     """
-    id: Optional[StrictStr] = Field(None, description="Whitelist rule id")
-    field: Optional[StrictStr] = Field(None, description="field used for whitelists rule")
-    value: Optional[StrictStr] = Field(None, description="value used for whitelists rule")
-    description: Optional[StrictStr] = Field(None, description="use an description for whitelisted rule")
-    __properties = ["id", "field", "value", "description"]
+    amount: conint(strict=True, ge=0) = Field(..., description="The amount to be deducted from the total sum of all payments, in cents.")
+    code: StrictStr = Field(..., description="Discount code.")
+    type: StrictStr = Field(..., description="It can be 'loyalty', 'campaign', 'coupon' o 'sign'")
+    id: StrictStr = Field(..., description="The discount line id")
+    object: StrictStr = Field(..., description="The object name")
+    parent_id: StrictStr = Field(..., description="The order id")
+    __properties = ["amount", "code", "type", "id", "object", "parent_id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -42,36 +44,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WhitelistlistRuleResponse:
-        """Create an instance of WhitelistlistRuleResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> DiscountLinesResponse:
+        """Create an instance of DiscountLinesResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WhitelistlistRuleResponse:
-        """Create an instance of WhitelistlistRuleResponse from a dict"""
+    def from_dict(cls, obj: dict) -> DiscountLinesResponse:
+        """Create an instance of DiscountLinesResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return WhitelistlistRuleResponse.parse_obj(obj)
+            return DiscountLinesResponse.parse_obj(obj)
 
-        _obj = WhitelistlistRuleResponse.parse_obj({
+        _obj = DiscountLinesResponse.parse_obj({
+            "amount": obj.get("amount"),
+            "code": obj.get("code"),
+            "type": obj.get("type"),
             "id": obj.get("id"),
-            "field": obj.get("field"),
-            "value": obj.get("value"),
-            "description": obj.get("description")
+            "object": obj.get("object"),
+            "parent_id": obj.get("parent_id")
         })
         return _obj
```

### Comparing `conekta-6.0.0/conekta/rest.py` & `conekta-6.0.1/conekta/rest.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/conekta.egg-info/PKG-INFO` & `conekta-6.0.1/conekta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conekta
-Version: 6.0.0
+Version: 6.0.1
 Summary: This is a Python library that allows interaction with https://api.conekta.io API.
 Home-page: https://github.com/conekta/conekta-python
 Author: Engineering Conekta
 Author-email: Engineering Conekta <engineering@conekta.com>
 License: MIT-LICENSE
 Project-URL: Homepage, https://github.com/conekta/conekta-python
 Project-URL: Bug Tracker, https://github.com/conekta/conekta-python/issues
@@ -19,15 +19,15 @@
 
 # conekta
 Conekta sdk
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2.1.0
-- Package version: 6.0.0
+- Package version: 6.0.1
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://github.com/conekta/openapi/issues](https://github.com/conekta/openapi/issues)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -120,27 +120,30 @@
 *AntifraudApi* | [**get_rule_blacklist**](docs/AntifraudApi.md#get_rule_blacklist) | **GET** /antifraud/blacklists | Get list of blacklisted rules
 *AntifraudApi* | [**get_rule_whitelist**](docs/AntifraudApi.md#get_rule_whitelist) | **GET** /antifraud/whitelists | Get a list of whitelisted rules
 *ApiKeysApi* | [**create_api_key**](docs/ApiKeysApi.md#create_api_key) | **POST** /api_keys | Create Api Key
 *ApiKeysApi* | [**delete_api_key**](docs/ApiKeysApi.md#delete_api_key) | **DELETE** /api_keys/{id} | Delete Api Key
 *ApiKeysApi* | [**get_api_key**](docs/ApiKeysApi.md#get_api_key) | **GET** /api_keys/{id} | Get Api Key
 *ApiKeysApi* | [**get_api_keys**](docs/ApiKeysApi.md#get_api_keys) | **GET** /api_keys | Get list of Api Keys
 *ApiKeysApi* | [**update_api_key**](docs/ApiKeysApi.md#update_api_key) | **PUT** /api_keys/{id} | Update Api Key
+*BalancesApi* | [**get_balance**](docs/BalancesApi.md#get_balance) | **GET** /balances | Get a company&#39;s balance
 *ChargesApi* | [**get_charges**](docs/ChargesApi.md#get_charges) | **GET** /charges | Get A List of Charges
 *ChargesApi* | [**orders_create_charge**](docs/ChargesApi.md#orders_create_charge) | **POST** /orders/{id}/charges | Create charge
 *CompaniesApi* | [**get_companies**](docs/CompaniesApi.md#get_companies) | **GET** /companies | Get List of Companies
 *CompaniesApi* | [**get_company**](docs/CompaniesApi.md#get_company) | **GET** /companies/{id} | Get Company
 *CustomersApi* | [**create_customer**](docs/CustomersApi.md#create_customer) | **POST** /customers | Create customer
 *CustomersApi* | [**create_customer_fiscal_entities**](docs/CustomersApi.md#create_customer_fiscal_entities) | **POST** /customers/{id}/fiscal_entities | Create Fiscal Entity
 *CustomersApi* | [**delete_customer_by_id**](docs/CustomersApi.md#delete_customer_by_id) | **DELETE** /customers/{id} | Delete Customer
 *CustomersApi* | [**get_customer_by_id**](docs/CustomersApi.md#get_customer_by_id) | **GET** /customers/{id} | Get Customer
 *CustomersApi* | [**get_customers**](docs/CustomersApi.md#get_customers) | **GET** /customers | Get a list of customers
 *CustomersApi* | [**update_customer**](docs/CustomersApi.md#update_customer) | **PUT** /customers/{id} | Update customer
 *CustomersApi* | [**update_customer_fiscal_entities**](docs/CustomersApi.md#update_customer_fiscal_entities) | **PUT** /customers/{id}/fiscal_entities/{fiscal_entities_id} | Update  Fiscal Entity
 *DiscountsApi* | [**orders_create_discount_line**](docs/DiscountsApi.md#orders_create_discount_line) | **POST** /orders/{id}/discount_lines | Create Discount
 *DiscountsApi* | [**orders_delete_discount_lines**](docs/DiscountsApi.md#orders_delete_discount_lines) | **DELETE** /orders/{id}/discount_lines/{discount_lines_id} | Delete Discount
+*DiscountsApi* | [**orders_get_discount_line**](docs/DiscountsApi.md#orders_get_discount_line) | **GET** /orders/{id}/discount_lines/{discount_lines_id} | Get Discount
+*DiscountsApi* | [**orders_get_discount_lines**](docs/DiscountsApi.md#orders_get_discount_lines) | **GET** /orders/{id}/discount_lines | Get a List of Discount
 *DiscountsApi* | [**orders_update_discount_lines**](docs/DiscountsApi.md#orders_update_discount_lines) | **PUT** /orders/{id}/discount_lines/{discount_lines_id} | Update Discount
 *EventsApi* | [**get_event**](docs/EventsApi.md#get_event) | **GET** /events/{id} | Get Event
 *EventsApi* | [**get_events**](docs/EventsApi.md#get_events) | **GET** /events | Get list of Events
 *EventsApi* | [**resend_event**](docs/EventsApi.md#resend_event) | **POST** /events/{event_id}/webhook_logs/{webhook_log_id}/resend | Resend Event
 *LogsApi* | [**get_log_by_id**](docs/LogsApi.md#get_log_by_id) | **GET** /logs/{id} | Get Log
 *LogsApi* | [**get_logs**](docs/LogsApi.md#get_logs) | **GET** /logs | Get List Of Logs
 *OrdersApi* | [**cancel_order**](docs/OrdersApi.md#cancel_order) | **POST** /orders/{id}/cancel | Cancel Order
@@ -205,15 +208,18 @@
 
 ## Documentation For Models
 
  - [ApiKeyCreateResponse](docs/ApiKeyCreateResponse.md)
  - [ApiKeyCreateResponseAllOf](docs/ApiKeyCreateResponseAllOf.md)
  - [ApiKeyRequest](docs/ApiKeyRequest.md)
  - [ApiKeyResponse](docs/ApiKeyResponse.md)
+ - [ApiKeyResponseOnDelete](docs/ApiKeyResponseOnDelete.md)
  - [ApiKeyUpdateRequest](docs/ApiKeyUpdateRequest.md)
+ - [BalanceCommonField](docs/BalanceCommonField.md)
+ - [BalanceResponse](docs/BalanceResponse.md)
  - [BlacklistRuleResponse](docs/BlacklistRuleResponse.md)
  - [ChargeDataPaymentMethodBankTransferResponse](docs/ChargeDataPaymentMethodBankTransferResponse.md)
  - [ChargeDataPaymentMethodCardResponse](docs/ChargeDataPaymentMethodCardResponse.md)
  - [ChargeDataPaymentMethodCashResponse](docs/ChargeDataPaymentMethodCashResponse.md)
  - [ChargeOrderResponse](docs/ChargeOrderResponse.md)
  - [ChargeOrderResponsePaymentMethod](docs/ChargeOrderResponsePaymentMethod.md)
  - [ChargeRequest](docs/ChargeRequest.md)
@@ -291,14 +297,16 @@
  - [GetChargesResponse](docs/GetChargesResponse.md)
  - [GetChargesResponseAllOf](docs/GetChargesResponseAllOf.md)
  - [GetCompaniesResponse](docs/GetCompaniesResponse.md)
  - [GetCompaniesResponseAllOf](docs/GetCompaniesResponseAllOf.md)
  - [GetCustomerPaymentMethodDataResponse](docs/GetCustomerPaymentMethodDataResponse.md)
  - [GetEventsResponse](docs/GetEventsResponse.md)
  - [GetEventsResponseAllOf](docs/GetEventsResponseAllOf.md)
+ - [GetOrderDiscountLinesResponse](docs/GetOrderDiscountLinesResponse.md)
+ - [GetOrderDiscountLinesResponseAllOf](docs/GetOrderDiscountLinesResponseAllOf.md)
  - [GetOrdersResponse](docs/GetOrdersResponse.md)
  - [GetPaymentMethodResponse](docs/GetPaymentMethodResponse.md)
  - [GetPaymentMethodResponseAllOf](docs/GetPaymentMethodResponseAllOf.md)
  - [GetPlansResponse](docs/GetPlansResponse.md)
  - [GetPlansResponseAllOf](docs/GetPlansResponseAllOf.md)
  - [GetTransactionsResponse](docs/GetTransactionsResponse.md)
  - [GetTransactionsResponseAllOf](docs/GetTransactionsResponseAllOf.md)
@@ -329,14 +337,15 @@
  - [OrderResponseFiscalEntityAddressAllOf](docs/OrderResponseFiscalEntityAddressAllOf.md)
  - [OrderResponseProducts](docs/OrderResponseProducts.md)
  - [OrderResponseProductsAllOf](docs/OrderResponseProductsAllOf.md)
  - [OrderResponseShippingContact](docs/OrderResponseShippingContact.md)
  - [OrderResponseShippingContactAllOf](docs/OrderResponseShippingContactAllOf.md)
  - [OrderTaxRequest](docs/OrderTaxRequest.md)
  - [OrderUpdateRequest](docs/OrderUpdateRequest.md)
+ - [OrderUpdateRequestCustomerInfo](docs/OrderUpdateRequestCustomerInfo.md)
  - [OrdersResponse](docs/OrdersResponse.md)
  - [Page](docs/Page.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodBankTransfer](docs/PaymentMethodBankTransfer.md)
  - [PaymentMethodCard](docs/PaymentMethodCard.md)
  - [PaymentMethodCardRequest](docs/PaymentMethodCardRequest.md)
```

### Comparing `conekta-6.0.0/conekta.egg-info/SOURCES.txt` & `conekta-6.0.1/conekta.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 conekta.egg-info/SOURCES.txt
 conekta.egg-info/dependency_links.txt
 conekta.egg-info/requires.txt
 conekta.egg-info/top_level.txt
 conekta/api/__init__.py
 conekta/api/antifraud_api.py
 conekta/api/api_keys_api.py
+conekta/api/balances_api.py
 conekta/api/charges_api.py
 conekta/api/companies_api.py
 conekta/api/customers_api.py
 conekta/api/discounts_api.py
 conekta/api/events_api.py
 conekta/api/logs_api.py
 conekta/api/orders_api.py
@@ -40,15 +41,18 @@
 conekta/api/webhook_keys_api.py
 conekta/api/webhooks_api.py
 conekta/models/__init__.py
 conekta/models/api_key_create_response.py
 conekta/models/api_key_create_response_all_of.py
 conekta/models/api_key_request.py
 conekta/models/api_key_response.py
+conekta/models/api_key_response_on_delete.py
 conekta/models/api_key_update_request.py
+conekta/models/balance_common_field.py
+conekta/models/balance_response.py
 conekta/models/blacklist_rule_response.py
 conekta/models/charge_data_payment_method_bank_transfer_response.py
 conekta/models/charge_data_payment_method_card_response.py
 conekta/models/charge_data_payment_method_cash_response.py
 conekta/models/charge_order_response.py
 conekta/models/charge_order_response_payment_method.py
 conekta/models/charge_request.py
@@ -126,14 +130,16 @@
 conekta/models/get_charges_response.py
 conekta/models/get_charges_response_all_of.py
 conekta/models/get_companies_response.py
 conekta/models/get_companies_response_all_of.py
 conekta/models/get_customer_payment_method_data_response.py
 conekta/models/get_events_response.py
 conekta/models/get_events_response_all_of.py
+conekta/models/get_order_discount_lines_response.py
+conekta/models/get_order_discount_lines_response_all_of.py
 conekta/models/get_orders_response.py
 conekta/models/get_payment_method_response.py
 conekta/models/get_payment_method_response_all_of.py
 conekta/models/get_plans_response.py
 conekta/models/get_plans_response_all_of.py
 conekta/models/get_transactions_response.py
 conekta/models/get_transactions_response_all_of.py
@@ -164,14 +170,15 @@
 conekta/models/order_response_fiscal_entity_address_all_of.py
 conekta/models/order_response_products.py
 conekta/models/order_response_products_all_of.py
 conekta/models/order_response_shipping_contact.py
 conekta/models/order_response_shipping_contact_all_of.py
 conekta/models/order_tax_request.py
 conekta/models/order_update_request.py
+conekta/models/order_update_request_customer_info.py
 conekta/models/orders_response.py
 conekta/models/page.py
 conekta/models/pagination.py
 conekta/models/payment_method.py
 conekta/models/payment_method_bank_transfer.py
 conekta/models/payment_method_card.py
 conekta/models/payment_method_card_request.py
@@ -234,14 +241,15 @@
 conekta/models/webhook_log.py
 conekta/models/webhook_request.py
 conekta/models/webhook_response.py
 conekta/models/webhook_update_request.py
 conekta/models/whitelistlist_rule_response.py
 test/test_antifraud_api.py
 test/test_api_keys_api.py
+test/test_balances_api.py
 test/test_charges_api.py
 test/test_companies_api.py
 test/test_customers_api.py
 test/test_discounts_api.py
 test/test_events_api.py
 test/test_logs_api.py
 test/test_orders_api.py
```

### Comparing `conekta-6.0.0/pyproject.toml` & `conekta-6.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conekta"
-version = "6.0.0"
+version = "6.0.1"
 description = "Conekta API"
 authors = ["Engineering Conekta <engineering@conekta.com>"]
 license = "MIT-LICENSE"
 readme = "README.md"
 repository = "https://github.com/conekta/conekta-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Conekta API"]
 
@@ -28,15 +28,15 @@
 [tool.setuptools_scm]
 
 [tool.pylint.'MESSAGES CONTROL']
 extension-pkg-whitelist = "pydantic"
 
 [project]
 name = "conekta"
-version = "6.0.0"
+version = "6.0.1"
 authors = [
   { name="Engineering Conekta", email="engineering@conekta.com" },
 ]
 description = "This is a Python library that allows interaction with https://api.conekta.io API."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `conekta-6.0.0/setup.py` & `conekta-6.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "conekta"
-VERSION = "6.0.0"
+VERSION = "6.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `conekta-6.0.0/test/test_antifraud_api.py` & `conekta-6.0.1/test/test_antifraud_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_api_keys_api.py` & `conekta-6.0.1/test/test_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_charges_api.py` & `conekta-6.0.1/test/test_charges_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_companies_api.py` & `conekta-6.0.1/test/test_companies_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_customers_api.py` & `conekta-6.0.1/test/test_customers_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_discounts_api.py` & `conekta-6.0.1/test/test_discounts_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_events_api.py` & `conekta-6.0.1/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_logs_api.py` & `conekta-6.0.1/test/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_orders_api.py` & `conekta-6.0.1/test/test_orders_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_payment_link_api.py` & `conekta-6.0.1/test/test_payment_link_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_payment_methods_api.py` & `conekta-6.0.1/test/test_payment_methods_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_plans_api.py` & `conekta-6.0.1/test/test_plans_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_products_api.py` & `conekta-6.0.1/test/test_products_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_shipping_contacts_api.py` & `conekta-6.0.1/test/test_shipping_contacts_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_shippings_api.py` & `conekta-6.0.1/test/test_shippings_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_subscriptions_api.py` & `conekta-6.0.1/test/test_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_taxes_api.py` & `conekta-6.0.1/test/test_taxes_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_tokens_api.py` & `conekta-6.0.1/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_transactions_api.py` & `conekta-6.0.1/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_transfers_api.py` & `conekta-6.0.1/test/test_transfers_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_webhook_keys_api.py` & `conekta-6.0.1/test/test_webhook_keys_api.py`

 * *Files identical despite different names*

### Comparing `conekta-6.0.0/test/test_webhooks_api.py` & `conekta-6.0.1/test/test_webhooks_api.py`

 * *Files identical despite different names*

