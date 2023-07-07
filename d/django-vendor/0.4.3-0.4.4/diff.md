# Comparing `tmp/django-vendor-0.4.3.tar.gz` & `tmp/django-vendor-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-0.4.3.tar", last modified: Tue May 30 22:12:35 2023, max compression
+gzip compressed data, was "django-vendor-0.4.4.tar", last modified: Fri Jul  7 19:17:24 2023, max compression
```

## Comparing `django-vendor-0.4.3.tar` & `django-vendor-0.4.4.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-30 22:12:35.782597 django-vendor-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-30 22:11:10.000000 django-vendor-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-30 22:11:10.000000 django-vendor-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:12:35.782597 django-vendor-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.758596 django-vendor-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.762596 django-vendor-0.4.3/src/django_vendor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-30 22:12:35.000000 django-vendor-0.4.3/src/django_vendor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-30 22:12:35.000000 django-vendor-0.4.3/src/django_vendor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:12:35.000000 django-vendor-0.4.3/src/django_vendor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 22:12:35.000000 django-vendor-0.4.3/src/django_vendor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 22:12:35.000000 django-vendor-0.4.3/src/django_vendor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.762596 django-vendor-0.4.3/src/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.762596 django-vendor-0.4.3/src/vendor/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.762596 django-vendor-0.4.3/src/vendor/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.766596 django-vendor-0.4.3/src/vendor/api/v1/authorizenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/authorizenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/authorizenet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.766596 django-vendor-0.4.3/src/vendor/api/v1/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/stripe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.766596 django-vendor-0.4.3/src/vendor/encrypt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/encrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/encrypt/cleartext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.770596 django-vendor-0.4.3/src/vendor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0002_auto_20200912_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0003_auto_20200915_1839.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0004_offer_offer_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0005_auto_20200930_2037.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0006_auto_20201005_2257.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0007_offer_list_bundle_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0008_offer_allow_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0009_auto_20201111_0743.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0010_auto_20201112_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0011_auto_20201120_1750.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0012_auto_20201123_1848.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0013_auto_20201202_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0014_term_types_update_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0015_uuid_payments_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0016_auto_20201203_2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0017_auto_20201203_2107.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0018_add_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0019_fill_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0020_lock_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0021_auto_20210408_2303.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0022_offer_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0023_profile_null_false.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0024_offer_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0025_auto_20210914_0025.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0026_auto_20210914_1209.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0028_add_trial_date_term_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0030_auto_20220414_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0031_pre_invoice_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0032_alter_invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0033_payment_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0034_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0035_add_subscription_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0036_post_payment_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0037_auto_20220609_1644.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0038_auto_20220719_0944.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0039_customerprofile_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0040_auto_20221020_1617.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0041_offer_billing_start_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0042_offer_is_promotional.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/0043_invoice_global_discount.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.774597 django-vendor-0.4.3/src/vendor/models/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/modelmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/models/wishlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.774597 django-vendor-0.4.3/src/vendor/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/processors/authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/processors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/processors/stripe_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.774597 django-vendor-0.4.3/src/vendor/signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/signals/stripe_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.762596 django-vendor-0.4.3/src/vendor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.778597 django-vendor-0.4.3/src/vendor/templates/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/address_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/checkout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.778597 django-vendor-0.4.3/src/vendor/templates/vendor/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/dummy/payment_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.778597 django-vendor-0.4.3/src/vendor/templates/vendor/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/includes/account_info_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/includes/billing_address_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/includes/cost_overview.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/includes/edit_link.html
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/includes/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/invoice_history_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/invoice_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/src/vendor/templates/vendor/manage/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/invoice_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/offer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/offers.html
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/payment_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/product.html
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/products.html
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/profile_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/profile_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/receipt_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/receipt_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_add_payment.html
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_create.html
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/orderitem_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/orderitem_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/orderitem_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/ordersummary.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/payment.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/payment_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/payment_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/purchase_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/purchase_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/refund_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templates/vendor/refund_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/src/vendor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/templatetags/admin_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/src/vendor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/tests/test_authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    42811 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/src/vendor/urls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/urls/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/urls/vendor_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:12:35.782597 django-vendor-0.4.3/src/vendor/views/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-30 22:11:10.000000 django-vendor-0.4.3/src/vendor/views/vendor_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.202021 django-vendor-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 19:17:24.202021 django-vendor-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-07 19:16:09.000000 django-vendor-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 19:16:09.000000 django-vendor-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:17:24.202021 django-vendor-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.182021 django-vendor-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.182021 django-vendor-0.4.4/src/django_vendor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 19:17:24.000000 django-vendor-0.4.4/src/django_vendor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-07 19:17:24.000000 django-vendor-0.4.4/src/django_vendor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:17:24.000000 django-vendor-0.4.4/src/django_vendor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 19:17:24.000000 django-vendor-0.4.4/src/django_vendor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 19:17:24.000000 django-vendor-0.4.4/src/django_vendor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/api/v1/authorizenet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/authorizenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/authorizenet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/api/v1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/stripe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.186021 django-vendor-0.4.4/src/vendor/encrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/encrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/encrypt/cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.190021 django-vendor-0.4.4/src/vendor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0002_auto_20200912_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0003_auto_20200915_1839.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0004_offer_offer_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0005_auto_20200930_2037.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0006_auto_20201005_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0007_offer_list_bundle_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0008_offer_allow_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0009_auto_20201111_0743.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0010_auto_20201112_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0011_auto_20201120_1750.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0012_auto_20201123_1848.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0013_auto_20201202_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0014_term_types_update_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0015_uuid_payments_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0016_auto_20201203_2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0017_auto_20201203_2107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0018_add_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0019_fill_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0020_lock_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0021_auto_20210408_2303.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0022_offer_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0023_profile_null_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0024_offer_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0025_auto_20210914_0025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0026_auto_20210914_1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0028_add_trial_date_term_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0030_auto_20220414_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0031_pre_invoice_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0032_alter_invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0033_payment_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0034_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0035_add_subscription_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0036_post_payment_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0037_auto_20220609_1644.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0038_auto_20220719_0944.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0039_customerprofile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0040_auto_20221020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0041_offer_billing_start_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0042_offer_is_promotional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/0043_invoice_global_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.194021 django-vendor-0.4.4/src/vendor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/modelmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/models/wishlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.194021 django-vendor-0.4.4/src/vendor/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/processors/authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/processors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/processors/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.194021 django-vendor-0.4.4/src/vendor/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/signals/stripe_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.182021 django-vendor-0.4.4/src/vendor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.198021 django-vendor-0.4.4/src/vendor/templates/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/address_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/checkout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.198021 django-vendor-0.4.4/src/vendor/templates/vendor/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/dummy/payment_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.198021 django-vendor-0.4.4/src/vendor/templates/vendor/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/includes/account_info_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/includes/billing_address_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/includes/cost_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/includes/edit_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/includes/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/invoice_history_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/invoice_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.198021 django-vendor-0.4.4/src/vendor/templates/vendor/manage/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/invoice_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/offer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/offers.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/payment_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/product.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/products.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/profile_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/profile_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/receipt_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/receipt_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_add_payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/orderitem_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/orderitem_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/orderitem_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/ordersummary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/payment_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/payment_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/purchase_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/purchase_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/refund_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templates/vendor/refund_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.198021 django-vendor-0.4.4/src/vendor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/templatetags/admin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.202021 django-vendor-0.4.4/src/vendor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/tests/test_authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42637 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.202021 django-vendor-0.4.4/src/vendor/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/urls/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/urls/vendor_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:17:24.202021 django-vendor-0.4.4/src/vendor/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-07-07 19:16:09.000000 django-vendor-0.4.4/src/vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.4.3/PKG-INFO` & `django-vendor-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.3
+Version: 0.4.4
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.3/README.md` & `django-vendor-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/pyproject.toml` & `django-vendor-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor"
-version = "0.4.3"
+version = "0.4.4"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Django App Toolkit for selling digital and physical goods online."
 readme = "README.md"
```

### Comparing `django-vendor-0.4.3/src/django_vendor.egg-info/PKG-INFO` & `django-vendor-0.4.4/src/django_vendor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.3
+Version: 0.4.4
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.3/src/django_vendor.egg-info/SOURCES.txt` & `django-vendor-0.4.4/src/django_vendor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 src/vendor/models/utils.py
 src/vendor/models/validator.py
 src/vendor/models/wishlist.py
 src/vendor/processors/__init__.py
 src/vendor/processors/authorizenet.py
 src/vendor/processors/base.py
 src/vendor/processors/dummy.py
-src/vendor/processors/stripe_processor.py
+src/vendor/processors/stripe.py
 src/vendor/signals/__init__.py
 src/vendor/signals/stripe_signals.py
 src/vendor/templates/vendor/address_detail.html
 src/vendor/templates/vendor/base.html
 src/vendor/templates/vendor/checkout.html
 src/vendor/templates/vendor/index.html
 src/vendor/templates/vendor/integration_form.html
```

### Comparing `django-vendor-0.4.3/src/vendor/admin.py` & `django-vendor-0.4.4/src/vendor/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/api/v1/authorizenet/views.py` & `django-vendor-0.4.4/src/vendor/api/v1/authorizenet/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/api/v1/stripe/views.py` & `django-vendor-0.4.4/src/vendor/api/v1/stripe/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,46 +91,46 @@
 class StripeSubscriptionInvoicePaid(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
         site = get_site_from_request(self.request)
 
         if not self.is_valid_post(site):
             logger.error(f"StripeSubscriptionInvoicePaid error: invalid post")
-            return HttpResponse(status=400, content="StripeSubscriptionInvoicePaid invalid post")
+            return HttpResponse(status=200, content="StripeSubscriptionInvoicePaid invalid post")
 
         if not self.is_incoming_event_correct_and_recurring(self.event, StripeEvents.INVOICE_PAID):
             logger.error(f"StripeSubscriptionInvoicePaid error: invalid event: {self.event}")
             return HttpResponse(status=200, content=f"StripeSubscriptionInvoicePaid error: invalid event: {self.event}")
 
         stripe_invoice = self.event.data.object
         paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at, tz=timezone.utc)
         amount_paid = convert_integer_to_float(stripe_invoice.total)
 
         # TODO nice to move this try/except blocks inside a generic function in the StripeBaseAPI class
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
-            return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
+            return HttpResponse(status=200, content=f"StripeSubscriptionInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
 
         if 'stripe_id' not in customer_profile.meta:
             customer_profile.meta['stripe_id'] = stripe_invoice.customer
             customer_profile.save()
 
         try:
             subscription = Subscription.objects.get(gateway_id=stripe_invoice.subscription, profile=customer_profile)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
-            return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
+            return HttpResponse(status=200, content=f"StripeSubscriptionInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         offer = subscription.get_offer()
 
         if not offer:
             logger.error(f"StripeSubscriptionInvoicePaid {subscription} has no offer attached")
-            return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid {subscription} has no offer attached")
+            return HttpResponse(status=200, content=f"StripeSubscriptionInvoicePaid {subscription} has no offer attached")
 
         invoice = Invoice.objects.create(
             profile=customer_profile,
             site=site,
             ordered_date=paid_date,
             status=InvoiceStatus.COMPLETE
         )
@@ -148,45 +148,45 @@
 class StripeSubscriptionPaymentFailed(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
         site = get_site_from_request(request)
 
         if not self.is_valid_post(site):
             logger.error("StripeSubscriptionPaymentFailed error: invalid post")
-            return HttpResponse(status=400, content="StripeSubscriptionPaymentFailed error: invalid post")
+            return HttpResponse(status=200, content="StripeSubscriptionPaymentFailed error: invalid post")
 
         if not self.is_incoming_event_correct_and_recurring(self.event, StripeEvents.INVOICE_PAYMENT_FAILED):
             logger.error(f"StripeSubscriptionPaymentFailed error: invalid event: {self.event}")
             return HttpResponse(status=200, content=f"StripeSubscriptionPaymentFailed error: invalid event: {self.event}")
 
         stripe_invoice = self.event.data.object
         paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at, tz=timezone.utc)
 
         # TODO nice to move this try/except blocks inside a generic function in the StripeBaseAPI class
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionPaymentFailed error: email: {stripe_invoice.customer_email} does not exist")
-            return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed error: email: {stripe_invoice.customer_email} does not exist")
+            return HttpResponse(status=200, content=f"StripeSubscriptionPaymentFailed error: email: {stripe_invoice.customer_email} does not exist")
 
         if 'stripe_id' not in customer_profile.meta:
             customer_profile.meta['stripe_id'] = stripe_invoice.customer
             customer_profile.save()
 
         try:
             subscription = Subscription.objects.get(gateway_id=stripe_invoice.subscription, profile=customer_profile)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionPaymentFailed customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
-            return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
+            return HttpResponse(status=200, content=f"StripeSubscriptionPaymentFailed customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         offer = subscription.get_offer()
 
         if not offer:
             logger.error(f"StripeSubscriptionPaymentFailed {subscription} has no offer attached")
-            return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed {subscription} has no offer attached")
+            return HttpResponse(status=200, content=f"StripeSubscriptionPaymentFailed {subscription} has no offer attached")
 
         invoice = Invoice.objects.create(
             profile=subscription.profile,
             site=subscription.profile.site,
             ordered_date=paid_date,
             status=InvoiceStatus.COMPLETE
         )
@@ -205,37 +205,37 @@
 class StripeInvoicePaid(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
         site = get_site_from_request(self.request)
 
         if not self.is_valid_post(site):
             logger.error("StripeInvoicePaid error: invalid post")
-            return HttpResponse(status=400, content="StripeInvoicePaid error: invalid post")
+            return HttpResponse(status=200, content="StripeInvoicePaid error: invalid post")
 
         if not self.is_incoming_event_correct(self.event, StripeEvents.INOVICE_PAYMENT_SUCCEEDED):
             logger.error(f"StripeInvoicePaid error: invalid event {self.event}")
             return HttpResponse(status=200, content=f"StripeInvoicePaid error: invalid event {self.event}")
 
         stripe_invoice = self.event.data.object
 
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
-            return HttpResponse(status=400, content=f"StripeInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
+            return HttpResponse(status=200, content=f"StripeInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
 
         if 'stripe_id' not in customer_profile.meta:
             customer_profile.meta['stripe_id'] = stripe_invoice.customer
             customer_profile.save()
 
         try:
             subscription = Subscription.objects.get(gateway_id=stripe_invoice.subscription, profile=customer_profile)
         except ObjectDoesNotExist:
             logger.error(f"StripeInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
-            return HttpResponse(status=400, content=f"StripeInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
+            return HttpResponse(status=200, content=f"StripeInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         payment = subscription.payments.filter(Q(transaction="") | Q(transaction=None), status=PurchaseStatus.QUEUED).first()
         receipt = subscription.receipts.filter(Q(transaction="") | Q(transaction=None)).first()
 
         if not payment and not receipt:
             logger.warning(f"There are no payments to update for subscription: {subscription}. Stripe Invoice: {stripe_invoice.id}")
             return HttpResponse(status=200, content=f"There are no payments to update for subscription: {subscription}. Stripe Invoice: {stripe_invoice.id}")
@@ -255,15 +255,15 @@
 class StripeCardExpiring(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
         site = get_site_from_request(self.request)
 
         if not self.is_valid_post(site):
             logger.error("StripeCardExpiring error: invalid event post")
-            return HttpResponse(status=400, content="StripeCardExpiring error: invalid event post")
+            return HttpResponse(status=200, content="StripeCardExpiring error: invalid event post")
 
         if not self.is_incoming_event_correct(self.event, StripeEvents.SOURCE_EXPIRED):
             logger.error(f"StripeCardExpiring error: invalid event {self.event}")
             return HttpResponse(status=200, content=f"StripeCardExpiring error: invalid event {self.event}")
 
         stripe_card = self.event.data.object
```

### Comparing `django-vendor-0.4.3/src/vendor/api/v1/urls.py` & `django-vendor-0.4.4/src/vendor/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/api/v1/views.py` & `django-vendor-0.4.4/src/vendor/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/apps.py` & `django-vendor-0.4.4/src/vendor/apps.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/config.py` & `django-vendor-0.4.4/src/vendor/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,107 +11,122 @@
 class SiteSelectForm(forms.Form):
     site = forms.ModelChoiceField(queryset=Site.objects.all())
 
 
 class SupportedPaymentProcessor(TextChoices):
     PROMO_CODE_BASE = ("base.PaymentProcessorBase", _("Default Processor"))
     AUTHORIZE_NET = ("authorizenet.AuthorizeNetProcessor", _("Authorize.Net"))
-    STRIPE = ("stripe_processor.StripeProcessor", _("Stripe"))
+    STRIPE = ("stripe.StripeProcessor", _("Stripe"))
 
 
 class PaymentProcessorForm(SiteSelectForm):
-    payment_processor = forms.CharField(label=_("Payment Processor"), widget=forms.Select(choices=SupportedPaymentProcessor.choices))
+    payment_processor = forms.CharField(
+        label=_("Payment Processor"),
+        widget=forms.Select(choices=SupportedPaymentProcessor.choices),
+    )
 
 
 class PaymentProcessorSiteConfig(SiteConfigBaseClass):
     label = _("Payment Processor")
     default = {"payment_processor": "base.PaymentProcessorBase"}
     form_class = PaymentProcessorForm
     key = ""
     instance = None
 
     def __init__(self, site=None):
-        
+
         if site is None:
             site = Site.objects.get_current()
 
         self.key = ".".join([__name__, __class__.__name__])
         super().__init__(site, self.key)
-        
+
         if not self.instance:
-            self.default['payment_processor'] = VENDOR_PAYMENT_PROCESSOR
+            self.default["payment_processor"] = VENDOR_PAYMENT_PROCESSOR
 
     def get_form(self):
         return self.form_class(initial=self.get_initials())
 
     def get_initials(self):
         initial = super().get_initials()
-        initial['site'] = (self.site.pk, self.site.domain)
-        
+        initial["site"] = (self.site.pk, self.site.domain)
+
         if self.instance:
-            initial['payment_processor'] = [choice for choice in SupportedPaymentProcessor.choices if choice[0] == self.instance.value['payment_processor']][0]
+            initial["payment_processor"] = [
+                choice
+                for choice in SupportedPaymentProcessor.choices
+                if choice[0] == self.instance.value["payment_processor"]
+            ][0]
         else:
-            initial['payment_processor'] = SupportedPaymentProcessor.choices[0]
-        
+            initial["payment_processor"] = SupportedPaymentProcessor.choices[0]
+
         return initial
 
     def get_selected_processor(self):
         if self.instance:
-            return [choice for choice in SupportedPaymentProcessor.choices if choice[0] == self.instance.value['payment_processor']][0]
+            return [
+                choice
+                for choice in SupportedPaymentProcessor.choices
+                if choice[0] == self.instance.value["payment_processor"]
+            ][0]
 
         return SupportedPaymentProcessor.choices[0]  # Return Default Processors
 
 
 class StripeConnectAccountForm(SiteSelectForm):
     account_number = forms.CharField(max_length=120)
 
 
 class StripeConnectAccountConfig(SiteConfigBaseClass):
     label = _("Stripe Connect Account")
-    default = {'stripe_connect_account': None}
+    default = {"stripe_connect_account": None}
     form_class = StripeConnectAccountForm
-    key = ''
+    key = ""
     instance = None
 
     def __init__(self, site=None):
-        
+
         if site is None:
             site = Site.objects.get_current()
 
         self.key = ".".join([__name__, __class__.__name__])
         super().__init__(site, self.key)
-        
+
 
 class VendorSiteCommissionForm(SiteSelectForm):
     commission = forms.IntegerField(min_value=0, max_value=100)
 
 
 class VendorSiteCommissionConfig(SiteConfigBaseClass):
     label = _("Vendor Site Commission")
-    default = {'commission': None}
+    default = {"commission": None}
     form_class = VendorSiteCommissionForm
-    key = ''
+    key = ""
     instance = None
 
     def __init__(self, site=None):
-        
+
         if site is None:
             site = Site.objects.get_current()
 
         self.key = ".".join([__name__, __class__.__name__])
         super().__init__(site, self.key)
 
 
 VENDOR_PRODUCT_MODEL = getattr(settings, "VENDOR_PRODUCT_MODEL", "vendor.Product")
 
-VENDOR_PAYMENT_PROCESSOR = getattr(settings, "VENDOR_PAYMENT_PROCESSOR", "dummy.DummyProcessor")
+VENDOR_PAYMENT_PROCESSOR = getattr(
+    settings, "VENDOR_PAYMENT_PROCESSOR", "dummy.DummyProcessor"
+)
 
 DEFAULT_CURRENCY = getattr(settings, "DEFAULT_CURRENCY", "usd")
 
-AVAILABLE_CURRENCIES = getattr(settings, "AVAILABLE_CURRENCIES", {'usd': _('USD Dollars')})
+AVAILABLE_CURRENCIES = getattr(
+    settings, "AVAILABLE_CURRENCIES", {"usd": _("USD Dollars")}
+)
 
 VENDOR_STATE = getattr(settings, "VENDOR_STATE", "DEBUG")
 
 # Encryption settings
-VENDOR_DATA_ENCODER = getattr(settings, "VENDOR_DATA_ENCODER", "vendor.encrypt.cleartext")
-
-
+VENDOR_DATA_ENCODER = getattr(
+    settings, "VENDOR_DATA_ENCODER", "vendor.encrypt.cleartext"
+)
```

### Comparing `django-vendor-0.4.3/src/vendor/forms.py` & `django-vendor-0.4.4/src/vendor/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/integrations.py` & `django-vendor-0.4.4/src/vendor/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0001_initial.py` & `django-vendor-0.4.4/src/vendor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0003_auto_20200915_1839.py` & `django-vendor-0.4.4/src/vendor/migrations/0003_auto_20200915_1839.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0005_auto_20200930_2037.py` & `django-vendor-0.4.4/src/vendor/migrations/0005_auto_20200930_2037.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0006_auto_20201005_2257.py` & `django-vendor-0.4.4/src/vendor/migrations/0006_auto_20201005_2257.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0008_offer_allow_multiple.py` & `django-vendor-0.4.4/src/vendor/migrations/0008_offer_allow_multiple.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0009_auto_20201111_0743.py` & `django-vendor-0.4.4/src/vendor/migrations/0009_auto_20201111_0743.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0010_auto_20201112_0138.py` & `django-vendor-0.4.4/src/vendor/migrations/0010_auto_20201112_0138.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0011_auto_20201120_1750.py` & `django-vendor-0.4.4/src/vendor/migrations/0011_auto_20201120_1750.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0012_auto_20201123_1848.py` & `django-vendor-0.4.4/src/vendor/migrations/0012_auto_20201123_1848.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0013_auto_20201202_1759.py` & `django-vendor-0.4.4/src/vendor/migrations/0013_auto_20201202_1759.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0014_term_types_update_value.py` & `django-vendor-0.4.4/src/vendor/migrations/0014_term_types_update_value.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0015_uuid_payments_receipts.py` & `django-vendor-0.4.4/src/vendor/migrations/0015_uuid_payments_receipts.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0016_auto_20201203_2011.py` & `django-vendor-0.4.4/src/vendor/migrations/0016_auto_20201203_2011.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0017_auto_20201203_2107.py` & `django-vendor-0.4.4/src/vendor/migrations/0017_auto_20201203_2107.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0018_add_uuid_address_profile.py` & `django-vendor-0.4.4/src/vendor/migrations/0018_add_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0019_fill_uuid_address_profile.py` & `django-vendor-0.4.4/src/vendor/migrations/0019_fill_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0020_lock_uuid_address_profile.py` & `django-vendor-0.4.4/src/vendor/migrations/0020_lock_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0021_auto_20210408_2303.py` & `django-vendor-0.4.4/src/vendor/migrations/0021_auto_20210408_2303.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0023_profile_null_false.py` & `django-vendor-0.4.4/src/vendor/migrations/0023_profile_null_false.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0025_auto_20210914_0025.py` & `django-vendor-0.4.4/src/vendor/migrations/0025_auto_20210914_0025.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0026_auto_20210914_1209.py` & `django-vendor-0.4.4/src/vendor/migrations/0026_auto_20210914_1209.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py` & `django-vendor-0.4.4/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0028_add_trial_date_term_details.py` & `django-vendor-0.4.4/src/vendor/migrations/0028_add_trial_date_term_details.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py` & `django-vendor-0.4.4/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0030_auto_20220414_1055.py` & `django-vendor-0.4.4/src/vendor/migrations/0030_auto_20220414_1055.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0031_pre_invoice_status_change.py` & `django-vendor-0.4.4/src/vendor/migrations/0031_pre_invoice_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0033_payment_status.py` & `django-vendor-0.4.4/src/vendor/migrations/0033_payment_status.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0034_subscription.py` & `django-vendor-0.4.4/src/vendor/migrations/0034_subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0035_add_subscription_relation.py` & `django-vendor-0.4.4/src/vendor/migrations/0035_add_subscription_relation.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0036_post_payment_status_change.py` & `django-vendor-0.4.4/src/vendor/migrations/0036_post_payment_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0037_auto_20220609_1644.py` & `django-vendor-0.4.4/src/vendor/migrations/0037_auto_20220609_1644.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0038_auto_20220719_0944.py` & `django-vendor-0.4.4/src/vendor/migrations/0038_auto_20220719_0944.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0040_auto_20221020_1617.py` & `django-vendor-0.4.4/src/vendor/migrations/0040_auto_20221020_1617.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/migrations/0042_offer_is_promotional.py` & `django-vendor-0.4.4/src/vendor/migrations/0042_offer_is_promotional.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/__init__.py` & `django-vendor-0.4.4/src/vendor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/address.py` & `django-vendor-0.4.4/src/vendor/models/address.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/base.py` & `django-vendor-0.4.4/src/vendor/models/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/choice.py` & `django-vendor-0.4.4/src/vendor/models/choice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/invoice.py` & `django-vendor-0.4.4/src/vendor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/modelmanagers.py` & `django-vendor-0.4.4/src/vendor/models/modelmanagers.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/offer.py` & `django-vendor-0.4.4/src/vendor/models/offer.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/payment.py` & `django-vendor-0.4.4/src/vendor/models/payment.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/price.py` & `django-vendor-0.4.4/src/vendor/models/price.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/profile.py` & `django-vendor-0.4.4/src/vendor/models/profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/receipt.py` & `django-vendor-0.4.4/src/vendor/models/receipt.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/subscription.py` & `django-vendor-0.4.4/src/vendor/models/subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/tax.py` & `django-vendor-0.4.4/src/vendor/models/tax.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/utils.py` & `django-vendor-0.4.4/src/vendor/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/validator.py` & `django-vendor-0.4.4/src/vendor/models/validator.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/models/wishlist.py` & `django-vendor-0.4.4/src/vendor/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/processors/__init__.py` & `django-vendor-0.4.4/src/vendor/processors/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from django.utils.module_loading import import_string
 from django.core.exceptions import ObjectDoesNotExist
 
 from vendor.config import PaymentProcessorSiteConfig
 from vendor.processors.authorizenet import AuthorizeNetProcessor
-from vendor.processors.stripe_processor import StripeProcessor, StripeQueryBuilder
+from vendor.processors.stripe import StripeProcessor, StripeQueryBuilder
 from vendor.processors.base import PaymentProcessorBase
 from vendor.processors.dummy import DummyProcessor
 from siteconfigs.models import SiteConfigModel
 
+
 def get_site_payment_processor(site):
     site_processor = PaymentProcessorSiteConfig(site)
-    return import_string(f"vendor.processors.{site_processor.get_key_value('payment_processor')}")
+    return import_string(
+        f"vendor.processors.{site_processor.get_key_value('payment_processor')}"
+    )
```

### Comparing `django-vendor-0.4.3/src/vendor/processors/authorizenet.py` & `django-vendor-0.4.4/src/vendor/processors/authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/processors/base.py` & `django-vendor-0.4.4/src/vendor/processors/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/processors/stripe_processor.py` & `django-vendor-0.4.4/src/vendor/processors/stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/signals/stripe_signals.py` & `django-vendor-0.4.4/src/vendor/signals/stripe_signals.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/checkout.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/checkout.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/includes/account_info_form.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/includes/account_info_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/includes/billing_address_form.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/includes/billing_address_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/includes/cost_overview.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/includes/cost_overview.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/includes/payment_form.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/includes/payment_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/integration_form.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/integration_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/invoice_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/invoice_history_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/invoice_history_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/invoice_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/config_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/dashboard.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/invoice_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/invoice_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/offer.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/offer.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/offers.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/offers.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/payment_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/payment_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/processor_site_config_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/product.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/product.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/products.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/products.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/profile_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/profile_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/profile_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/profile_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/receipt_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/receipt_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/receipt_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/receipt_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_add_payment.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_add_payment.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_create.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_create.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/manage/subscription_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/manage/subscription_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/orderitem_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/orderitem_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/ordersummary.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/ordersummary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/payment_summary.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/payment_summary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/purchase_detail.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/purchase_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/purchase_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/purchase_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templates/vendor/refund_list.html` & `django-vendor-0.4.4/src/vendor/templates/vendor/refund_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/templatetags/admin_tags.py` & `django-vendor-0.4.4/src/vendor/templatetags/admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/tests/__init__.py` & `django-vendor-0.4.4/src/vendor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/tests/test_authorizenet.py` & `django-vendor-0.4.4/src/vendor/tests/test_authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/tests/test_processor.py` & `django-vendor-0.4.4/src/vendor/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/tests/test_stripe.py` & `django-vendor-0.4.4/src/vendor/tests/test_stripe.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         '5200828282828210',  # mastercard debit
     ]
 
     def setup_processor_site_config(self):
         self.processor_site_config = SiteConfigModel()
         self.processor_site_config.site = self.existing_invoice.site
         self.processor_site_config.key = 'vendor.config.PaymentProcessorSiteConfig'
-        self.processor_site_config.value = {"payment_processor": "stripe_processor.StripeProcessor"}
+        self.processor_site_config.value = {"payment_processor": "stripe.StripeProcessor"}
         self.processor_site_config.save()
 
     def setup_user_client(self):
         self.client = Client()
         self.user = User.objects.get(pk=1)
         self.customer = CustomerProfile.objects.get(pk=1)
         self.client.force_login(self.user)
@@ -280,15 +280,15 @@
         self.form_data['credit_card_form']['card_number'] = '4000000000009235'
 
         self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
         self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
 
         self.processor.invoice.total = randrange(1, 1000)
         self.processor.authorize_payment()
-        
+
         self.assertFalse(self.processor.transaction_succeeded)
 
     def test_process_payment_postal_code_check_fails(self):
         """
         Postal code check fails for any code given fo this card number
         """
         self.processor.create_stripe_customers([self.customer])
@@ -585,19 +585,19 @@
         self.processor.transaction_succeeded = False
 
         self.processor.process_customer_profile_payment()
 
         self.assertIsNotNone(self.processor.payment)
         self.assertTrue(self.processor.payment.success)
         self.assertEquals(InvoiceStatus.COMPLETE, self.processor.invoice.status)
-    
+
 
     """
     Commenting out since stripe doesnt allow you to delete Price objects (weird)
-    
+
     def test_check_price_does_exist(self):
         stripe_product = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_annual_license)
         self.pri_monthly['product'] = stripe_product.id
         stripe_price = self.processor.stripe_create_object(self.processor.stripe.Price, self.pri_monthly)
 
         metadata = {
             'key': 'site',
@@ -653,17 +653,17 @@
 
 @skipIf((settings.STRIPE_PUBLIC_KEY or settings.STRIPE_SECRET_KEY) is None, "Strip enviornment variables not set, skipping tests")
 class StripeCRUDObjectTests(TestCase):
 
     def init_test_objects(self):
         self.valid_metadata = {'site': 'sc', 'pk':1}
         self.valid_addr = {'city': "na",'country': "US",'line1': "Salvatierra walk",'postal_code': "90321",'state': 'CA'}
-        
+
         self.cus_norrin_radd = {'name': 'Norrin Radd', 'email': 'norrin@radd.com', 'metadata': self.valid_metadata}
-        
+
         self.pro_monthly_license = {'name': "Monthly License", 'metadata': self.valid_metadata}
         self.pro_annual_license = {"name": "Annual Subscription", 'metadata': self.valid_metadata}
 
         self.pri_monthly = {"currency": "usd", "unit_amount": 1024, "recurring": {"interval": "month", "interval_count": 1, "usage_type": "licensed"}, 'metadata': self.valid_metadata}
         self.card = {'number': 4242424242424242, 'exp_month': "10", 'exp_year': "2023", 'cvc': "9000"}
         self.payment_method = {'type': 'card', 'card': self.card}
         self.cou_first_three_months_coupon = {
@@ -716,15 +716,15 @@
         stripe_product = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_annual_license)
         self.processor.stripe_delete_object(self.processor.stripe.Product, stripe_product.id)
 
         self.assertIsNotNone(stripe_product.id)
 
     def test_create_product_no_name_fail(self):
         del(self.pro_monthly_license['name'])
-        
+
         stripe_product = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_monthly_license)
         self.assertFalse(self.processor.transaction_succeeded)
 
     def test_get_product_success(self):
         stripe_product = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_annual_license)
 
         self.assertIsNotNone(stripe_product.id)
@@ -767,15 +767,15 @@
 
         self.assertIsNotNone(stripe_price.id)
 
     def test_create_price_invalid_field_fail(self):
         self.pri_monthly['type'] = "This is not a valid field"
 
         stripe_price = self.processor.stripe_create_object(self.processor.stripe.Price, self.pri_monthly)
-        
+
         self.assertFalse(self.processor.transaction_succeeded)
 
     ##########
     # Coupon CRUD
     def test_create_coupon_success(self):
         stripe_coupon = self.processor.stripe_create_object(self.processor.stripe.Coupon, self.cou_first_month_free)
 
@@ -783,91 +783,91 @@
 
         self.assertIsNotNone(stripe_coupon.id)
 
     ##########
     # Subscription CRUD
     def test_create_subscription_success(self):
         stripe_cus_norrin_radd = self.processor.stripe_create_object(self.processor.stripe.Customer, self.cus_norrin_radd)
-        
+
         stripe_payment_method = self.processor.stripe_create_object(self.processor.stripe.PaymentMethod, self.payment_method)
 
         setup_intent_object = {
             'customer': stripe_cus_norrin_radd.id,
             'confirm': True,
             'payment_method_types': ['card'],
             'payment_method': stripe_payment_method.id,
             'metadata': self.valid_metadata
         }
         stripe_setup_intent = self.processor.stripe_create_object(self.processor.stripe.SetupIntent, setup_intent_object)
-        
+
         stripe_pro_monthly = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_monthly_license)
-        
+
         self.pri_monthly['product'] = stripe_pro_monthly.id
         stripe_price = self.processor.stripe_create_object(self.processor.stripe.Price, self.pri_monthly)
-        
+
         subscription_obj = {
             'customer': stripe_cus_norrin_radd.id,
             'items': [{'price': stripe_price.id}],
             'default_payment_method': stripe_payment_method.id,
             'metadata': self.valid_metadata,
 
         }
         stripe_subscription = self.processor.stripe_create_object(self.processor.stripe.Subscription, subscription_obj)
 
         self.assertIsNotNone(stripe_subscription.id)
 
     ##########
     # Invoice CRUD
     # def test_create_invoice_success(self):
-        
+
         # setup_intent_object = {
         #     'customer': stripe_cus_norrin_radd.id,
         #     'confirm': True,
         #     'payment_method_types': ['card'],
         #     'payment_method': stripe_payment_method.id,
         #     'metadata': self.valid_metadata
         # }
-        
-        
+
+
         # self.pri_monthly['product'] = stripe_pro_monthly.id
-        
+
         # subscription_obj = {
         #     'customer': stripe_cus_norrin_radd.id,
         #     'items': [{'price': stripe_price.id}],
         #     'default_payment_method': stripe_payment_method.id,
         #     'metadata': self.valid_metadata,
 
         # }
-            
+
         # stripe_invoice_object = {
         #     'metadata': self.valid_metadata,
         #     'subscription': stripe_sub.id,
         #     'customer': stripe_cus_norrin_radd.id,
         #     'statement_descriptor': 'Test description'
         # }
 
 
         # self.assertIsNotNone(stripe_invoice.id)
-        
+
     ##########
     # Setup Intent CRUD
     def test_create_setup_intent_success(self):
 
         stripe_cus_norrin_radd = self.processor.stripe_create_object(self.processor.stripe.Customer, self.cus_norrin_radd)
         stripe_payment_method = self.processor.stripe_create_object(self.processor.stripe.PaymentMethod, self.payment_method)
-        
+
         setup_intent_object = {
             'customer': stripe_cus_norrin_radd.id,
             'confirm': True,
             'payment_method_types': ['card'],
             'payment_method': stripe_payment_method.id,
             'metadata': self.valid_metadata
         }
         stripe_setup_intent = self.processor.stripe_create_object(self.processor.stripe.SetupIntent, setup_intent_object)
-        
+
         self.assertIsNotNone(stripe_setup_intent.id)
 
 
 @skipIf((settings.STRIPE_PUBLIC_KEY or settings.STRIPE_SECRET_KEY) is None, "Strip enviornment variables not set, skipping tests")
 class StripeBuildObjectTests(TestCase):
 
     fixtures = ['user', 'unit_test']
@@ -880,15 +880,15 @@
         self.processor = StripeProcessor(self.site)
 
     def test_build_customer_success(self):
         customer_profile = CustomerProfile.objects.all().first()
 
         customer_data = self.processor.build_customer(customer_profile)
         stripe_customer = self.processor.stripe_create_object(self.processor.stripe.Customer, customer_data)
-        
+
         self.assertIsNotNone(stripe_customer.id)
         self.assertEqual(f"{customer_profile.user.first_name} {customer_profile.user.last_name}", stripe_customer.name)
         self.assertEqual(customer_profile.user.email, stripe_customer.email)
 
     def test_build_product_success(self):
         offer = Offer.objects.all().first()
 
@@ -918,15 +918,15 @@
 
     def test_build_coupon_success(self):
         offer = Offer.objects.all().first()
         price = offer.prices.first()
 
         coupon_data = self.processor.build_coupon(offer, price)
         stripe_coupon = self.processor.stripe_create_object(self.processor.stripe.Coupon, coupon_data)
-        
+
         self.assertIsNotNone(stripe_coupon.id)
         self.assertEqual("".join([str(stripe_coupon.amount_off)[:-2], ".", str(stripe_coupon.amount_off)[-2:]]), str((offer.get_msrp() - price.cost)))
 
     def test_build_subscription_success(self):
         pass
 
     def test_build_payment_method_successs(self):
```

### Comparing `django-vendor-0.4.3/src/vendor/urls/vendor.py` & `django-vendor-0.4.4/src/vendor/urls/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/urls/vendor_admin.py` & `django-vendor-0.4.4/src/vendor/urls/vendor_admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/utils.py` & `django-vendor-0.4.4/src/vendor/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/__init__.py` & `django-vendor-0.4.4/src/vendor/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/config.py` & `django-vendor-0.4.4/src/vendor/views/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/integration.py` & `django-vendor-0.4.4/src/vendor/views/integration.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/mixin.py` & `django-vendor-0.4.4/src/vendor/views/mixin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/report.py` & `django-vendor-0.4.4/src/vendor/views/report.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/vendor.py` & `django-vendor-0.4.4/src/vendor/views/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.3/src/vendor/views/vendor_admin.py` & `django-vendor-0.4.4/src/vendor/views/vendor_admin.py`

 * *Files identical despite different names*

