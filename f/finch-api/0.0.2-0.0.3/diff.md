# Comparing `tmp/finch_api-0.0.2.tar.gz` & `tmp/finch_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch_api-0.0.2.tar", max compression
+gzip compressed data, was "finch_api-0.0.3.tar", max compression
```

## Comparing `finch_api-0.0.2.tar` & `finch_api-0.0.3.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0    11335 2023-05-08 18:28:19.703315 finch_api-0.0.2/LICENSE
--rw-r--r--   0        0        0     7347 2023-05-08 18:28:19.703315 finch_api-0.0.2/README.md
--rw-r--r--   0        0        0     1872 2023-05-08 18:28:19.703315 finch_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1834 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/__init__.py
--rw-r--r--   0        0        0    46017 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_base_client.py
--rw-r--r--   0        0        0     3889 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_base_exceptions.py
--rw-r--r--   0        0        0    17885 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_client.py
--rw-r--r--   0        0        0     1285 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_models.py
--rw-r--r--   0        0        0     4781 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_qs.py
--rw-r--r--   0        0        0      872 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_resource.py
--rw-r--r--   0        0        0     3976 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_types.py
--rw-r--r--   0        0        0     1277 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/__init__.py
--rw-r--r--   0        0        0     6701 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/_utils.py
--rw-r--r--   0        0        0      124 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_version.py
--rw-r--r--   0        0        0    10630 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/pagination.py
--rw-r--r--   0        0        0        0 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/py.typed
--rw-r--r--   0        0        0      321 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/__init__.py
--rw-r--r--   0        0        0     4144 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/account.py
--rw-r--r--   0        0        0      532 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/__init__.py
--rw-r--r--   0        0        0     5758 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/applications.py
--rw-r--r--   0        0        0     1409 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/ats.py
--rw-r--r--   0        0        0     6058 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/candidates.py
--rw-r--r--   0        0        0     5428 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/jobs.py
--rw-r--r--   0        0        0     5532 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/ats/offers.py
--rw-r--r--   0        0        0     2703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/ats/stages.py
--rw-r--r--   0        0        0      703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/__init__.py
--rw-r--r--   0        0        0      231 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/__init__.py
--rw-r--r--   0        0        0    13700 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/benefits.py
--rw-r--r--   0        0        0    13797 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/individuals.py
--rw-r--r--   0        0        0     2021 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/company.py
--rw-r--r--   0        0        0     4175 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/directory.py
--rw-r--r--   0        0        0     1760 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/hris.py
--rw-r--r--   0        0        0      262 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/__init__.py
--rw-r--r--   0        0        0     4278 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/employment_data.py
--rw-r--r--   0        0        0     4552 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/individuals.py
--rw-r--r--   0        0        0     3963 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/pay_statements.py
--rw-r--r--   0        0        0     4247 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/payments.py
--rw-r--r--   0        0        0     2256 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/providers.py
--rw-r--r--   0        0        0      416 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/__init__.py
--rw-r--r--   0        0        0      572 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/__init__.py
--rw-r--r--   0        0        0      512 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/application.py
--rw-r--r--   0        0        0      361 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/application_list_params.py
--rw-r--r--   0        0        0      726 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/candidate.py
--rw-r--r--   0        0        0      355 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/candidate_list_params.py
--rw-r--r--   0        0        0      889 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/job.py
--rw-r--r--   0        0        0      337 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/job_list_params.py
--rw-r--r--   0        0        0      474 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/offer.py
--rw-r--r--   0        0        0      343 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/offer_list_params.py
--rw-r--r--   0        0        0      362 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/stage.py
--rw-r--r--   0        0        0      266 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/disconnect_response.py
--rw-r--r--   0        0        0     1761 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/__init__.py
--rw-r--r--   0        0        0      902 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_create_params.py
--rw-r--r--   0        0        0      220 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_frequency.py
--rw-r--r--   0        0        0      598 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_type.py
--rw-r--r--   0        0        0      278 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_update_params.py
--rw-r--r--   0        0        0      784 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/__init__.py
--rw-r--r--   0        0        0      723 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/enrolled_individual.py
--rw-r--r--   0        0        0      969 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_benefit.py
--rw-r--r--   0        0        0      424 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_enroll_many_params.py
--rw-r--r--   0        0        0      259 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
--rw-r--r--   0        0        0      398 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
--rw-r--r--   0        0        0      329 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_unenroll_params.py
--rw-r--r--   0        0        0      647 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/unenrolled_individual.py
--rw-r--r--   0        0        0      415 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benfit_contribution.py
--rw-r--r--   0        0        0     2209 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/company.py
--rw-r--r--   0        0        0      596 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/company_benefit.py
--rw-r--r--   0        0        0      202 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/create_company_benefits_response.py
--rw-r--r--   0        0        0      376 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/directory_list_individuals_params.py
--rw-r--r--   0        0        0     1361 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual.py
--rw-r--r--   0        0        0     1025 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_in_directory.py
--rw-r--r--   0        0        0      327 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_response.py
--rw-r--r--   0        0        0      480 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_retrieve_many_params.py
--rw-r--r--   0        0        0      367 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/__init__.py
--rw-r--r--   0        0        0     2985 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data.py
--rw-r--r--   0        0        0      363 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data_response.py
--rw-r--r--   0        0        0      703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
--rw-r--r--   0        0        0     3320 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement.py
--rw-r--r--   0        0        0      376 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_response.py
--rw-r--r--   0        0        0      438 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_response_body.py
--rw-r--r--   0        0        0      616 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_retrieve_many_params.py
--rw-r--r--   0        0        0      791 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/payment.py
--rw-r--r--   0        0        0      709 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/payment_list_params.py
--rw-r--r--   0        0        0     1411 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/supported_benefit.py
--rw-r--r--   0        0        0      200 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/update_company_benefit_response.py
--rw-r--r--   0        0        0      724 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/income.py
--rw-r--r--   0        0        0      881 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/introspection.py
--rw-r--r--   0        0        0      631 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/location.py
--rw-r--r--   0        0        0      262 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/money.py
--rw-r--r--   0        0        0      369 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/paging.py
--rw-r--r--   0        0        0      959 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/provider.py
--rw-r--r--   0        0        0     8245 1970-01-01 00:00:00.000000 finch_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-07 14:41:00.722886 finch_api-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7466 2023-07-07 14:41:00.722886 finch_api-0.0.3/README.md
+-rw-r--r--   0        0        0     1871 2023-07-07 14:41:00.726886 finch_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1834 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/__init__.py
+-rw-r--r--   0        0        0    46805 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_base_exceptions.py
+-rw-r--r--   0        0        0    17881 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_client.py
+-rw-r--r--   0        0        0     1285 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_models.py
+-rw-r--r--   0        0        0     4846 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_qs.py
+-rw-r--r--   0        0        0      872 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_resource.py
+-rw-r--r--   0        0        0     5884 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_streaming.py
+-rw-r--r--   0        0        0     4226 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_types.py
+-rw-r--r--   0        0        0     1277 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_utils/_utils.py
+-rw-r--r--   0        0        0      124 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/_version.py
+-rw-r--r--   0        0        0    10630 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/pagination.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/py.typed
+-rw-r--r--   0        0        0      321 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/account.py
+-rw-r--r--   0        0        0      532 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/__init__.py
+-rw-r--r--   0        0        0     6374 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/applications.py
+-rw-r--r--   0        0        0     1409 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/ats.py
+-rw-r--r--   0        0        0     6638 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/candidates.py
+-rw-r--r--   0        0        0     6044 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/jobs.py
+-rw-r--r--   0        0        0     6148 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/offers.py
+-rw-r--r--   0        0        0     2703 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/ats/stages.py
+-rw-r--r--   0        0        0      703 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/benefits/__init__.py
+-rw-r--r--   0        0        0    14280 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/benefits/benefits.py
+-rw-r--r--   0        0        0    14347 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/benefits/individuals.py
+-rw-r--r--   0        0        0     2021 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/company.py
+-rw-r--r--   0        0        0     4175 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/directory.py
+-rw-r--r--   0        0        0     1760 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/hris.py
+-rw-r--r--   0        0        0      262 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     4278 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0     4552 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/individuals/individuals.py
+-rw-r--r--   0        0        0     3963 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/pay_statements.py
+-rw-r--r--   0        0        0     4247 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/hris/payments.py
+-rw-r--r--   0        0        0     2256 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/resources/providers.py
+-rw-r--r--   0        0        0      416 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/__init__.py
+-rw-r--r--   0        0        0      512 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/application.py
+-rw-r--r--   0        0        0      361 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/application_list_params.py
+-rw-r--r--   0        0        0      726 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/candidate.py
+-rw-r--r--   0        0        0      355 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/candidate_list_params.py
+-rw-r--r--   0        0        0      889 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/job.py
+-rw-r--r--   0        0        0      337 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/job_list_params.py
+-rw-r--r--   0        0        0      474 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/offer.py
+-rw-r--r--   0        0        0      343 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/offer_list_params.py
+-rw-r--r--   0        0        0      362 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/ats/stage.py
+-rw-r--r--   0        0        0      266 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/disconnect_response.py
+-rw-r--r--   0        0        0     1761 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefit_create_params.py
+-rw-r--r--   0        0        0      220 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefit_frequency.py
+-rw-r--r--   0        0        0      598 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefit_type.py
+-rw-r--r--   0        0        0      278 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefit_update_params.py
+-rw-r--r--   0        0        0      784 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/enrolled_individual.py
+-rw-r--r--   0        0        0      969 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/individual_benefit.py
+-rw-r--r--   0        0        0      550 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/individual_enroll_many_params.py
+-rw-r--r--   0        0        0      259 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
+-rw-r--r--   0        0        0      398 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
+-rw-r--r--   0        0        0      329 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/individual_unenroll_params.py
+-rw-r--r--   0        0        0      647 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benefits/unenrolled_individual.py
+-rw-r--r--   0        0        0      415 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/benfit_contribution.py
+-rw-r--r--   0        0        0     2209 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/company.py
+-rw-r--r--   0        0        0      596 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/company_benefit.py
+-rw-r--r--   0        0        0      202 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/create_company_benefits_response.py
+-rw-r--r--   0        0        0      376 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/directory_list_individuals_params.py
+-rw-r--r--   0        0        0     1361 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individual.py
+-rw-r--r--   0        0        0     1025 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individual_in_directory.py
+-rw-r--r--   0        0        0      327 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individual_response.py
+-rw-r--r--   0        0        0      480 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individual_retrieve_many_params.py
+-rw-r--r--   0        0        0      367 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     2985 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0      363 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individuals/employment_data_response.py
+-rw-r--r--   0        0        0      703 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
+-rw-r--r--   0        0        0     3320 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/pay_statement.py
+-rw-r--r--   0        0        0      376 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/pay_statement_response.py
+-rw-r--r--   0        0        0      438 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/pay_statement_response_body.py
+-rw-r--r--   0        0        0      616 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/pay_statement_retrieve_many_params.py
+-rw-r--r--   0        0        0      791 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/payment.py
+-rw-r--r--   0        0        0      709 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/payment_list_params.py
+-rw-r--r--   0        0        0     1411 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/supported_benefit.py
+-rw-r--r--   0        0        0      200 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/hris/update_company_benefit_response.py
+-rw-r--r--   0        0        0      724 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/income.py
+-rw-r--r--   0        0        0      881 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/introspection.py
+-rw-r--r--   0        0        0      631 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/location.py
+-rw-r--r--   0        0        0      262 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/money.py
+-rw-r--r--   0        0        0      369 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/paging.py
+-rw-r--r--   0        0        0      959 2023-07-07 14:41:00.726886 finch_api-0.0.3/src/finch/types/provider.py
+-rw-r--r--   0        0        0     8371 1970-01-01 00:00:00.000000 finch_api-0.0.3/PKG-INFO
```

### Comparing `finch_api-0.0.2/LICENSE` & `finch_api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/README.md` & `finch_api-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 ```python
 from finch import Finch
 
 finch = Finch(
     access_token="my access token",
 )
 
-page = finch.hris.directory.list_individuals()
-directory = page.individuals[0]
-print(directory.ein)
+candidate = finch.ats.candidates.retrieve(
+    "<candidate id>",
+)
+print(candidate.first_name)
 ```
 
 ## Async Usage
 
 Simply import `AsyncFinch` instead of `Finch` and use `await` with each API call:
 
 ```python
@@ -39,16 +40,18 @@
 
 finch = AsyncFinch(
     access_token="my access token",
 )
 
 
 async def main():
-    page = await finch.hris.directory.list_individuals()
-    print(page.individuals[0].ein)
+    candidate = await finch.ats.candidates.retrieve(
+        "<candidate id>",
+    )
+    print(candidate.first_name)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -228,19 +231,21 @@
 
 ## Default Headers
 
 We automatically send the `Finch-API-Version` header set to `2020-09-17`.
 
 If you need to, you can override it by setting default headers per-request or on the client object.
 
+Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
+
 ```python
 from finch import Finch
 
 finch = Finch(
-    default_headers={"Finch-API-Version": My - Custom - Value},
+    default_headers={"Finch-API-Version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
@@ -259,13 +264,12 @@
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
-We are keen for your feedback; please email us at [founders@tryfinch.com](mailto:founders@tryfinch.com) or open an issue with questions,
-bugs, or suggestions.
+We are keen for your feedback; please open an [issue](https://www.github.com/Finch-API/finch-api-python/issues) with questions, bugs, or suggestions.
 
 ## Requirements
 
-Python 3.7 or higher.
+Python 3.7 or higher.
```

### Comparing `finch_api-0.0.2/pyproject.toml` & `finch_api-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "finch-api"
-version = "0.0.2"
+version = "0.0.3"
 description = "Client library for the Finch API"
 readme = "README.md"
 authors = ["Finch <founders@tryfinch.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/Finch-API/finch-api-python"
 packages = [
   { include = "finch", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = ">= 0.23.0"
-pydantic = ">= 1.9.0"
+pydantic = "^1.9.0"
 typing-extensions = ">= 4.1.1"
 anyio = ">= 3.5.0"
 distro = ">= 1.7.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "1.1.297"
@@ -26,14 +26,15 @@
 respx = "0.19.2"
 pytest = "7.1.1"
 pytest-asyncio = "0.18.3"
 ruff = "0.0.239"
 isort = "5.10.1"
 time-machine = "^2.9.0"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ["py37"]
```

### Comparing `finch_api-0.0.2/src/finch/__init__.py` & `finch_api-0.0.3/src/finch/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_base_client.py` & `finch_api-0.0.3/src/finch/_base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import uuid
 import inspect
 import platform
 from random import random
 from typing import (
     Any,
     Dict,
-    List,
     Type,
     Union,
     Generic,
     Mapping,
     TypeVar,
     Iterable,
     Iterator,
@@ -41,14 +40,15 @@
     Omit,
     Query,
     ModelT,
     Headers,
     Timeout,
     NoneType,
     NotGiven,
+    ResponseT,
     Transport,
     AnyMapping,
     ProxiesTypes,
     RequestFiles,
     RequestOptions,
     UnknownResponse,
     ModelBuilderProtocol,
@@ -57,148 +57,44 @@
 from ._models import (
     BaseModel,
     GenericModel,
     FinalRequestOptions,
     validate_type,
     construct_type,
 )
+from ._streaming import Stream, AsyncStream
 from ._base_exceptions import (
     APIStatusError,
     APITimeoutError,
     APIConnectionError,
     APIResponseValidationError,
 )
 
 # TODO: make base page type vars covariant
 SyncPageT = TypeVar("SyncPageT", bound="BaseSyncPage[Any]")
 AsyncPageT = TypeVar("AsyncPageT", bound="BaseAsyncPage[Any]")
 
 
-ResponseT = TypeVar(
-    "ResponseT",
-    bound=Union[
-        str,
-        None,
-        BaseModel,
-        List[Any],
-        Dict[str, Any],
-        httpx.Response,
-        UnknownResponse,
-        ModelBuilderProtocol,
-    ],
-)
-
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 
+_StreamT = TypeVar("_StreamT", bound=Stream[Any])
+_AsyncStreamT = TypeVar("_AsyncStreamT", bound=AsyncStream[Any])
+
+
 DEFAULT_TIMEOUT = Timeout(timeout=60.0, connect=5.0)
 DEFAULT_MAX_RETRIES = 2
 DEFAULT_LIMITS = Limits(max_connections=100, max_keepalive_connections=20)
 
 
-class StopStreaming(Exception):
-    """Raised internally when processing of a streamed response should be stopped."""
-
-
-class Stream(Generic[ResponseT]):
-    response: httpx.Response
-
-    def __init__(
-        self,
-        *,
-        cast_to: type[ResponseT],
-        response: httpx.Response,
-        client: SyncAPIClient,
-    ) -> None:
-        self.response = response
-        self._cast_to = cast_to
-        self._client = client
-        self._iterator = self.__iter()
-
-    def __next__(self) -> ResponseT:
-        return self._iterator.__next__()
-
-    def __iter__(self) -> Iterator[ResponseT]:
-        for item in self._iterator:
-            yield item
-
-    def __iter(self) -> Iterator[ResponseT]:
-        cast_to = self._cast_to
-        response = self.response
-        process_line = self._client._process_stream_line
-        process_data = self._client._process_response_data
-
-        awaiting_ping_data = False
-        for raw_line in response.iter_lines():
-            if not raw_line or raw_line == "\n":
-                continue
-
-            if raw_line.startswith("event: ping"):
-                awaiting_ping_data = True
-                continue
-            if awaiting_ping_data:
-                awaiting_ping_data = False
-                continue
-
-            try:
-                line = process_line(raw_line)
-            except StopStreaming:
-                # we are done!
-                break
-
-            yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
-
-
-class AsyncStream(Generic[ResponseT]):
-    response: httpx.Response
-
-    def __init__(
-        self,
-        *,
-        cast_to: type[ResponseT],
-        response: httpx.Response,
-        client: AsyncAPIClient,
-    ) -> None:
-        self.response = response
-        self._cast_to = cast_to
-        self._client = client
-        self._iterator = self.__iter()
-
-    async def __anext__(self) -> ResponseT:
-        return await self._iterator.__anext__()
-
-    async def __aiter__(self) -> AsyncIterator[ResponseT]:
-        async for item in self._iterator:
-            yield item
-
-    async def __iter(self) -> AsyncIterator[ResponseT]:
-        cast_to = self._cast_to
-        response = self.response
-        process_line = self._client._process_stream_line
-        process_data = self._client._process_response_data
-
-        awaiting_ping_data = False
-        async for raw_line in response.aiter_lines():
-            if not raw_line or raw_line == "\n":
-                continue
-
-            if raw_line.startswith("event: ping"):
-                awaiting_ping_data = True
-                continue
-            if awaiting_ping_data:
-                awaiting_ping_data = False
-                continue
-
-            try:
-                line = process_line(raw_line)
-            except StopStreaming:
-                # we are done!
-                break
-
-            yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
+class MissingStreamClassError(TypeError):
+    def __init__(self) -> None:
+        super().__init__(
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `finch._streaming` for reference",
+        )
 
 
 class PageInfo:
     """Stores the necesary information to build the request to retrieve the next page.
 
     Either `url` or `params` must be set.
     """
@@ -478,14 +374,23 @@
             if not options.idempotency_key:
                 options.idempotency_key = self._idempotency_key()
 
             headers[idempotency_header] = options.idempotency_key
 
         return headers
 
+    def _prepare_request(self, request: httpx.Request) -> None:
+        """This method is used as a callback for mutating the `Request` object
+        after it has been constructed.
+
+        This is useful for cases where you want to add certain headers based off of
+        the request properties, e.g. `url`, `method` etc.
+        """
+        return None
+
     def _build_request(
         self,
         options: FinalRequestOptions,
     ) -> httpx.Request:
         headers = self._build_headers(options)
 
         kwargs: dict[str, Any] = {}
@@ -515,28 +420,30 @@
                 if not is_dict(json_data):
                     raise TypeError(
                         f"Expected query input to be a dictionary for multipart requests but got {type(json_data)} instead."
                     )
                 kwargs["data"] = self._serialize_multipartform(json_data)
 
         # TODO: report this error to httpx
-        return self._client.build_request(  # pyright: ignore[reportUnknownMemberType]
+        request = self._client.build_request(  # pyright: ignore[reportUnknownMemberType]
             headers=headers,
             timeout=self.timeout if isinstance(options.timeout, NotGiven) else options.timeout,
             method=options.method,
             url=options.url,
             # the `Query` type that we use is incompatible with qs'
             # `Params` type as it needs to be typed as `Mapping[str, object]`
             # so that passing a `TypedDict` doesn't cause an error.
             # https://github.com/microsoft/pyright/issues/3526#event-6715453066
             params=self.qs.stringify(cast(Mapping[str, Any], params)) if params else None,
             json=json_data,
             files=options.files,
             **kwargs,
         )
+        self._prepare_request(request)
+        return request
 
     def _serialize_multipartform(self, data: Mapping[object, object]) -> dict[str, object]:
         items = self.qs.stringify_items(
             # TODO: type ignore is required as stringify_items is well typed but we can't be
             # well typed without heavy validation.
             data,  # type: ignore
             array_format="brackets",
@@ -620,24 +527,14 @@
             return cast(ResponseT, cast_to.build(response=response, data=data))
 
         if self._strict_response_validation:
             return cast(ResponseT, validate_type(type_=cast_to, value=data))
 
         return cast(ResponseT, construct_type(type_=cast_to, value=data))
 
-    def _process_stream_line(self, contents: str) -> str:
-        """Pre-process an indiviudal line from a streaming response"""
-        if contents == "data: [DONE]\n":
-            raise StopStreaming()
-
-        if contents.startswith("data: "):
-            return contents[6:]
-
-        return contents
-
     @property
     def qs(self) -> Querystring:
         return Querystring()
 
     @property
     def custom_auth(self) -> httpx.Auth | None:
         return None
@@ -741,14 +638,15 @@
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
 class SyncAPIClient(BaseClient):
     _client: httpx.Client
+    _default_stream_cls: type[Stream[Any]] | None = None
 
     def __init__(
         self,
         *,
         version: str,
         base_url: str,
         max_retries: int = DEFAULT_MAX_RETRIES,
@@ -783,15 +681,16 @@
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: Literal[True],
-    ) -> Stream[ResponseT]:
+        stream_cls: Type[_StreamT],
+    ) -> _StreamT:
         ...
 
     @overload
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
@@ -805,65 +704,79 @@
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: Type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         ...
 
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         return self._request(
             cast_to=cast_to,
             options=options,
             stream=stream,
+            stream_cls=stream_cls,
             remaining_retries=remaining_retries,
         )
 
     def _request(
         self,
         *,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: int | None,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None,
+    ) -> ResponseT | _StreamT:
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
 
         try:
             response = self._client.send(request, auth=self.custom_auth, stream=stream)
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             if retries > 0 and self._should_retry(err.response):
-                return self._retry_request(options, cast_to, retries, err.response.headers, stream=stream)
+                return self._retry_request(
+                    options,
+                    cast_to,
+                    retries,
+                    err.response.headers,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                )
 
             # If the response is streamed then we need to explicitly read the response
             # to completion before attempting to access the response text.
             err.response.read()
             raise self._make_status_error_from_response(request, err.response) from None
         except httpx.TimeoutException as err:
             if retries > 0:
-                return self._retry_request(options, cast_to, retries, stream=stream)
+                return self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except Exception as err:
             if retries > 0:
-                return self._retry_request(options, cast_to, retries, stream=stream)
+                return self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APIConnectionError(request=request) from err
 
         if stream:
-            return Stream(cast_to=cast_to, response=response, client=self)
+            stream_cls = stream_cls or cast("type[_StreamT] | None", self._default_stream_cls)
+            if stream_cls is None:
+                raise MissingStreamClassError()
+            return stream_cls(cast_to=cast_to, response=response, client=self)
 
         try:
             rsp = self._process_response(cast_to=cast_to, options=options, response=response)
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(request=request, response=response) from err
 
         return rsp
@@ -872,27 +785,29 @@
         self,
         options: FinalRequestOptions,
         cast_to: Type[ResponseT],
         remaining_retries: int,
         response_headers: Optional[httpx.Headers] = None,
         *,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None,
+    ) -> ResponseT | _StreamT:
         remaining = remaining_retries - 1
         timeout = self._calculate_retry_timeout(remaining, options, response_headers)
 
         # In a synchronous context we are blocking the entire thread. Up to the library user to run the client in a
         # different thread if necessary.
         time.sleep(timeout)
 
         return self._request(
             options=options,
             cast_to=cast_to,
             remaining_retries=remaining,
             stream=stream,
+            stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
@@ -901,25 +816,62 @@
         resp._set_private_attributes(  # pyright: ignore[reportPrivateUsage]
             client=self,
             model=model,
             options=options,
         )
         return resp
 
+    @overload
     def get(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         options: RequestOptions = {},
+        stream: Literal[False] = False,
     ) -> ResponseT:
+        ...
+
+    @overload
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: Literal[True],
+        stream_cls: type[_StreamT],
+    ) -> _StreamT:
+        ...
+
+    @overload
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool,
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
+        ...
+
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool = False,
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         opts = FinalRequestOptions.construct(method="get", url=path, **options)
         # cast is required because mypy complains about returning Any even though
         # it understands the type variables
-        return cast(ResponseT, self.request(cast_to, opts, stream=False))
+        return cast(ResponseT, self.request(cast_to, opts, stream=stream, stream_cls=stream_cls))
 
     @overload
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
@@ -936,42 +888,45 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: Literal[True],
-    ) -> Stream[ResponseT]:
+        stream_cls: type[_StreamT],
+    ) -> _StreamT:
         ...
 
     @overload
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         ...
 
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         opts = FinalRequestOptions.construct(method="post", url=path, json_data=body, files=files, **options)
-        return cast(ResponseT, self.request(cast_to, opts, stream=stream))
+        return cast(ResponseT, self.request(cast_to, opts, stream=stream, stream_cls=stream_cls))
 
     def patch(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
@@ -1015,14 +970,15 @@
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
 class AsyncAPIClient(BaseClient):
     _client: httpx.AsyncClient
+    _default_stream_cls: type[AsyncStream[Any]] | None = None
 
     def __init__(
         self,
         *,
         version: str,
         base_url: str,
         _strict_response_validation: bool,
@@ -1067,87 +1023,102 @@
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: Literal[True],
+        stream_cls: type[_AsyncStreamT],
         remaining_retries: Optional[int] = None,
-    ) -> AsyncStream[ResponseT]:
+    ) -> _AsyncStreamT:
         ...
 
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool,
+        stream_cls: type[_AsyncStreamT] | None = None,
         remaining_retries: Optional[int] = None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         ...
 
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool = False,
+        stream_cls: type[_AsyncStreamT] | None = None,
         remaining_retries: Optional[int] = None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         return await self._request(
             cast_to=cast_to,
             options=options,
             stream=stream,
+            stream_cls=stream_cls,
             remaining_retries=remaining_retries,
         )
 
     async def _request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool,
+        stream_cls: type[_AsyncStreamT] | None,
         remaining_retries: int | None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
 
         try:
             response = await self._client.send(request, auth=self.custom_auth, stream=stream)
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             if retries > 0 and self._should_retry(err.response):
-                return await self._retry_request(options, cast_to, retries, err.response.headers, stream=stream)
+                return await self._retry_request(
+                    options,
+                    cast_to,
+                    retries,
+                    err.response.headers,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                )
 
             # If the response is streamed then we need to explicitly read the response
             # to completion before attempting to access the response text.
             await err.response.aread()
             raise self._make_status_error_from_response(request, err.response) from None
         except httpx.ConnectTimeout as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except httpx.ReadTimeout as err:
             # We explicitly do not retry on ReadTimeout errors as this means
             # that the server processing the request has taken 60 seconds
             # (our default timeout). This likely indicates that something
             # is not working as expected on the server side.
             raise
         except httpx.TimeoutException as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except Exception as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APIConnectionError(request=request) from err
 
         if stream:
-            return AsyncStream(cast_to=cast_to, response=response, client=self)
+            stream_cls = stream_cls or cast("type[_AsyncStreamT] | None", self._default_stream_cls)
+            if stream_cls is None:
+                raise MissingStreamClassError()
+            return stream_cls(cast_to=cast_to, response=response, client=self)
 
         try:
             rsp = self._process_response(cast_to=cast_to, options=options, response=response)
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(request=request, response=response) from err
 
         return rsp
@@ -1156,44 +1127,83 @@
         self,
         options: FinalRequestOptions,
         cast_to: Type[ResponseT],
         remaining_retries: int,
         response_headers: Optional[httpx.Headers] = None,
         *,
         stream: bool,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None,
+    ) -> ResponseT | _AsyncStreamT:
         remaining = remaining_retries - 1
         timeout = self._calculate_retry_timeout(remaining, options, response_headers)
 
         await anyio.sleep(timeout)
 
         return await self._request(
             options=options,
             cast_to=cast_to,
             remaining_retries=remaining,
             stream=stream,
+            stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[AsyncPageT],
         options: FinalRequestOptions,
     ) -> AsyncPaginator[ModelT, AsyncPageT]:
         return AsyncPaginator(client=self, options=options, page_cls=page, model=model)
 
+    @overload
     async def get(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         options: RequestOptions = {},
+        stream: Literal[False] = False,
     ) -> ResponseT:
+        ...
+
+    @overload
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: Literal[True],
+        stream_cls: type[_AsyncStreamT],
+    ) -> _AsyncStreamT:
+        ...
+
+    @overload
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool,
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
+        ...
+
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool = False,
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         opts = FinalRequestOptions.construct(method="get", url=path, **options)
-        return await self.request(cast_to, opts)
+        return await self.request(cast_to, opts, stream=stream, stream_cls=stream_cls)
 
     @overload
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
@@ -1210,42 +1220,45 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: Literal[True],
-    ) -> AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT],
+    ) -> _AsyncStreamT:
         ...
 
     @overload
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: bool,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         ...
 
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: bool = False,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         opts = FinalRequestOptions.construct(method="post", url=path, json_data=body, files=files, **options)
-        return await self.request(cast_to, opts, stream=stream)
+        return await self.request(cast_to, opts, stream=stream, stream_cls=stream_cls)
 
     async def patch(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
```

### Comparing `finch_api-0.0.2/src/finch/_base_exceptions.py` & `finch_api-0.0.3/src/finch/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_client.py` & `finch_api-0.0.3/src/finch/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,23 @@
     Timeout,
     NotGiven,
     Transport,
     ProxiesTypes,
     RequestOptions,
 )
 from ._version import __version__
-from ._base_client import DEFAULT_LIMITS, DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES
-from ._base_client import Stream as Stream
-from ._base_client import AsyncStream as AsyncStream
-from ._base_client import SyncAPIClient, AsyncAPIClient
+from ._streaming import Stream as Stream
+from ._streaming import AsyncStream as AsyncStream
+from ._base_client import (
+    DEFAULT_LIMITS,
+    DEFAULT_TIMEOUT,
+    DEFAULT_MAX_RETRIES,
+    SyncAPIClient,
+    AsyncAPIClient,
+)
 
 __all__ = [
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
     "resources",
```

### Comparing `finch_api-0.0.2/src/finch/_exceptions.py` & `finch_api-0.0.3/src/finch/_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_models.py` & `finch_api-0.0.3/src/finch/_models.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_qs.py` & `finch_api-0.0.3/src/finch/_qs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         array_format: ArrayFormat = "repeat",
         nested_format: NestedFormat = "brackets",
     ) -> None:
         self.array_format = array_format
         self.nested_format = nested_format
 
     def parse(self, query: str) -> Mapping[str, object]:
-        # TODO
+        # Note: custom format syntax is not supported yet
         return parse_qs(query)
 
     def stringify(
         self,
         params: Params,
         *,
         array_format: NotGivenOr[ArrayFormat] = NOT_GIVEN,
@@ -85,17 +85,19 @@
                     )
                 )
             return items
 
         if isinstance(value, (list, tuple)):
             array_format = opts.array_format
             if array_format == "comma":
-                # TODO: support list of objects?
                 return [
-                    (key, ",".join(self._primitive_value_to_str(item) for item in value if item is not None)),
+                    (
+                        key,
+                        ",".join(self._primitive_value_to_str(item) for item in value if item is not None),
+                    ),
                 ]
             elif array_format == "repeat":
                 items = []
                 for item in value:
                     items.extend(self._stringify_item(key, item, opts))
                 return items
             elif array_format == "indices":
```

### Comparing `finch_api-0.0.2/src/finch/_resource.py` & `finch_api-0.0.3/src/finch/_resource.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_types.py` & `finch_api-0.0.3/src/finch/_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 
 from typing import (
     IO,
     TYPE_CHECKING,
+    Any,
     Dict,
+    List,
     Type,
     Tuple,
     Union,
     Mapping,
     TypeVar,
     Optional,
     Sequence,
 )
 from typing_extensions import Literal, Protocol, TypedDict, runtime_checkable
 
+import httpx
 import pydantic
 from httpx import Proxy, Timeout, Response, BaseTransport
 
+if TYPE_CHECKING:
+    from ._models import BaseModel
+
 Transport = BaseTransport
 Query = Mapping[str, object]
 Body = object
 AnyMapping = Mapping[str, object]
 ModelT = TypeVar("ModelT", bound=pydantic.BaseModel)
 _T = TypeVar("_T")
 
@@ -139,7 +145,12 @@
 
 class HeadersLikeProtocol(Protocol):
     def get(self, __key: str) -> str | None:
         ...
 
 
 HeadersLike = Union[Headers, HeadersLikeProtocol]
+
+ResponseT = TypeVar(
+    "ResponseT",
+    bound="Union[str, None, BaseModel, List[Any], Dict[str, Any], httpx.Response, UnknownResponse, ModelBuilderProtocol]",
+)
```

### Comparing `finch_api-0.0.2/src/finch/_utils/__init__.py` & `finch_api-0.0.3/src/finch/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/_utils/_transform.py` & `finch_api-0.0.3/src/finch/_utils/_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 def _maybe_transform_key(key: str, type_: type) -> str:
     annotated_type = _get_annoted_type(type_)
     if annotated_type is None:
         # no `Annotated` definition for this type, no transformation needed
         return key
 
     # ignore the first argument as it is the actual type
-    annotations = get_args(type_)[1:]
+    annotations = get_args(annotated_type)[1:]
     for annotation in annotations:
         if isinstance(annotation, PropertyInfo) and annotation.alias is not None:
             return annotation.alias
 
     return key
```

### Comparing `finch_api-0.0.2/src/finch/_utils/_utils.py` & `finch_api-0.0.3/src/finch/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/pagination.py` & `finch_api-0.0.3/src/finch/pagination.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/account.py` & `finch_api-0.0.3/src/finch/resources/account.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/ats/__init__.py` & `finch_api-0.0.3/src/finch/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/ats/applications.py` & `finch_api-0.0.3/src/finch/resources/ats/applications.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Application:
-        """Gets an application from an organization."""
+        """
+        Gets an application from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/ats/applications/{application_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Application,
         )
@@ -89,15 +100,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Application:
-        """Gets an application from an organization."""
+        """
+        Gets an application from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/ats/applications/{application_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Application,
         )
```

### Comparing `finch_api-0.0.2/src/finch/resources/ats/ats.py` & `finch_api-0.0.3/src/finch/resources/ats/ats.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/ats/candidates.py` & `finch_api-0.0.3/src/finch/resources/ats/candidates.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Candidate:
         """Gets a candidate from an organization.
 
         A candidate represents an individual
         associated with one or more applications.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
             f"/ats/candidates/{candidate_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Candidate,
@@ -99,14 +108,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Candidate:
         """Gets a candidate from an organization.
 
         A candidate represents an individual
         associated with one or more applications.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
             f"/ats/candidates/{candidate_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Candidate,
```

### Comparing `finch_api-0.0.2/src/finch/resources/ats/jobs.py` & `finch_api-0.0.3/src/finch/resources/ats/jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Job:
-        """Gets a job from an organization."""
+        """
+        Gets a job from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/ats/jobs/{job_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Job,
         )
@@ -89,15 +100,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Job:
-        """Gets a job from an organization."""
+        """
+        Gets a job from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/ats/jobs/{job_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Job,
         )
```

### Comparing `finch_api-0.0.2/src/finch/resources/ats/offers.py` & `finch_api-0.0.3/src/finch/resources/ats/offers.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Offer:
-        """Get a single offer from an organization."""
+        """
+        Get a single offer from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/ats/offers/{offer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Offer,
         )
@@ -89,15 +100,26 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Offer:
-        """Get a single offer from an organization."""
+        """
+        Get a single offer from an organization.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/ats/offers/{offer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Offer,
         )
```

### Comparing `finch_api-0.0.2/src/finch/resources/ats/stages.py` & `finch_api-0.0.3/src/finch/resources/ats/stages.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/__init__.py` & `finch_api-0.0.3/src/finch/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/benefits/benefits.py` & `finch_api-0.0.3/src/finch/resources/hris/benefits/benefits.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
             "/employer/benefits",
             body=maybe_transform(
                 {
-                    "type": type,
                     "description": description,
                     "frequency": frequency,
+                    "type": type,
                 },
                 benefit_create_params.BenefitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CreateCompanyBenefitsResponse,
@@ -91,14 +91,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CompanyBenefit:
         """
         **Availability: Automated Benefits providers only**
 
         Lists benefit information for a given benefit
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
             f"/employer/benefits/{benefit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CompanyBenefit,
@@ -228,17 +237,17 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
             "/employer/benefits",
             body=maybe_transform(
                 {
-                    "type": type,
                     "description": description,
                     "frequency": frequency,
+                    "type": type,
                 },
                 benefit_create_params.BenefitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CreateCompanyBenefitsResponse,
@@ -255,14 +264,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CompanyBenefit:
         """
         **Availability: Automated Benefits providers only**
 
         Lists benefit information for a given benefit
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
             f"/employer/benefits/{benefit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CompanyBenefit,
```

### Comparing `finch_api-0.0.2/src/finch/resources/hris/benefits/individuals.py` & `finch_api-0.0.3/src/finch/resources/hris/benefits/individuals.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class Individuals(SyncAPIResource):
     def enroll_many(
         self,
         benefit_id: str,
         *,
-        individuals: List[individual_enroll_many_params.IndividualEnrollManyParam],
+        individuals: List[individual_enroll_many_params.Individual],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncSinglePage[EnrolledIndividual]:
@@ -80,14 +80,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> IndividualEnrolledIDsResponse:
         """
         **Availability: Automated Benefits providers only**
 
         Lists individuals currently enrolled in a given benefit.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
             f"/employer/benefits/{benefit_id}/enrolled",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=IndividualEnrolledIDsResponse,
@@ -181,15 +190,15 @@
 
 
 class AsyncIndividuals(AsyncAPIResource):
     def enroll_many(
         self,
         benefit_id: str,
         *,
-        individuals: List[individual_enroll_many_params.IndividualEnrollManyParam],
+        individuals: List[individual_enroll_many_params.Individual],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[EnrolledIndividual, AsyncSinglePage[EnrolledIndividual]]:
@@ -238,14 +247,23 @@
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> IndividualEnrolledIDsResponse:
         """
         **Availability: Automated Benefits providers only**
 
         Lists individuals currently enrolled in a given benefit.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
             f"/employer/benefits/{benefit_id}/enrolled",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=IndividualEnrolledIDsResponse,
```

### Comparing `finch_api-0.0.2/src/finch/resources/hris/company.py` & `finch_api-0.0.3/src/finch/resources/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/directory.py` & `finch_api-0.0.3/src/finch/resources/hris/directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/hris.py` & `finch_api-0.0.3/src/finch/resources/hris/hris.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/individuals/employment_data.py` & `finch_api-0.0.3/src/finch/resources/hris/individuals/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/individuals/individuals.py` & `finch_api-0.0.3/src/finch/resources/hris/individuals/individuals.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,16 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/employer/individual",
             page=SyncResponsesPage[IndividualResponse],
             body=maybe_transform(
                 {
-                    "requests": requests,
                     "options": options,
+                    "requests": requests,
                 },
                 individual_retrieve_many_params.IndividualRetrieveManyParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             model=IndividualResponse,
@@ -99,16 +99,16 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/employer/individual",
             page=AsyncResponsesPage[IndividualResponse],
             body=maybe_transform(
                 {
-                    "requests": requests,
                     "options": options,
+                    "requests": requests,
                 },
                 individual_retrieve_many_params.IndividualRetrieveManyParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             model=IndividualResponse,
```

### Comparing `finch_api-0.0.2/src/finch/resources/hris/pay_statements.py` & `finch_api-0.0.3/src/finch/resources/hris/pay_statements.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/resources/hris/payments.py` & `finch_api-0.0.3/src/finch/resources/hris/payments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "start_date": start_date,
                         "end_date": end_date,
+                        "start_date": start_date,
                     },
                     payment_list_params.PaymentListParams,
                 ),
             ),
             model=Payment,
         )
 
@@ -103,15 +103,15 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "start_date": start_date,
                         "end_date": end_date,
+                        "start_date": start_date,
                     },
                     payment_list_params.PaymentListParams,
                 ),
             ),
             model=Payment,
         )
```

### Comparing `finch_api-0.0.2/src/finch/resources/providers.py` & `finch_api-0.0.3/src/finch/resources/providers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/ats/__init__.py` & `finch_api-0.0.3/src/finch/types/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/ats/application.py` & `finch_api-0.0.3/src/finch/types/ats/application.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 
 class RejectedReason(BaseModel):
     text: Optional[str]
 
 
 class Application(BaseModel):
-    candidate_id: str
-
     id: str
 
+    candidate_id: str
+
     job_id: str
 
     offer_id: Optional[str]
 
     rejected_at: Optional[datetime]
 
     rejected_reason: Optional[RejectedReason]
```

### Comparing `finch_api-0.0.2/src/finch/types/ats/candidate.py` & `finch_api-0.0.3/src/finch/types/ats/candidate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 class PhoneNumber(BaseModel):
     data: Optional[str]
 
     type: Optional[str]
 
 
 class Candidate(BaseModel):
+    id: str
+
     application_ids: List[str]
     """Array of Finch uuids corresponding to `application`s for this individual"""
 
     created_at: datetime
 
     emails: List[Email]
 
     first_name: Optional[str]
 
     full_name: Optional[str]
 
-    id: str
-
     last_activity_at: datetime
 
     last_name: Optional[str]
 
     phone_numbers: List[PhoneNumber]
```

### Comparing `finch_api-0.0.2/src/finch/types/ats/job.py` & `finch_api-0.0.3/src/finch/types/ats/job.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 class HiringTeam(BaseModel):
     hiring_managers: Optional[List[HiringTeamHiringManager]]
 
     recruiters: Optional[List[HiringTeamRecruiter]]
 
 
 class Job(BaseModel):
+    id: str
+
     closed_at: Optional[datetime]
 
     created_at: Optional[datetime]
 
     department: Department
 
     hiring_team: HiringTeam
 
-    id: str
-
     name: Optional[str]
 
     status: Optional[Literal["open", "closed", "on_hold", "draft", "archived"]]
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/__init__.py` & `finch_api-0.0.3/src/finch/types/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefit_create_params.py` & `finch_api-0.0.3/src/finch/types/hris/benefit_create_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefit_type.py` & `finch_api-0.0.3/src/finch/types/hris/benefit_type.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefits/__init__.py` & `finch_api-0.0.3/src/finch/types/hris/benefits/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefits/enrolled_individual.py` & `finch_api-0.0.3/src/finch/types/hris/benefits/enrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefits/individual_benefit.py` & `finch_api-0.0.3/src/finch/types/hris/benefits/individual_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/benefits/unenrolled_individual.py` & `finch_api-0.0.3/src/finch/types/hris/benefits/unenrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/company.py` & `finch_api-0.0.3/src/finch/types/hris/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,36 +2,15 @@
 
 from typing import List, Optional
 from typing_extensions import Literal
 
 from ...types import location
 from ..._models import BaseModel
 
-__all__ = ["Company", "Entity", "Department", "DepartmentParent", "Account"]
-
-
-class Entity(BaseModel):
-    subtype: Optional[Literal["s_corporation", "c_corporation", "b_corporation"]]
-    """The tax payer subtype of the company."""
-
-    type: Optional[Literal["llc", "corporation", "sole_proprietor", "non_profit", "partnership", "cooperative"]]
-    """The tax payer type of the company."""
-
-
-class DepartmentParent(BaseModel):
-    name: Optional[str]
-    """The parent department's name."""
-
-
-class Department(BaseModel):
-    name: Optional[str]
-    """The department name."""
-
-    parent: Optional[DepartmentParent]
-    """The parent department, if present."""
+__all__ = ["Company", "Account", "Department", "DepartmentParent", "Entity"]
 
 
 class Account(BaseModel):
     account_name: Optional[str]
     """The name of the bank associated in the payroll/HRIS system."""
 
     account_number: Optional[str]
@@ -46,30 +25,51 @@
     routing_number: Optional[str]
     """A nine-digit code that's based on the U.S.
 
     Bank location where your account was opened.
     """
 
 
+class DepartmentParent(BaseModel):
+    name: Optional[str]
+    """The parent department's name."""
+
+
+class Department(BaseModel):
+    name: Optional[str]
+    """The department name."""
+
+    parent: Optional[DepartmentParent]
+    """The parent department, if present."""
+
+
+class Entity(BaseModel):
+    subtype: Optional[Literal["s_corporation", "c_corporation", "b_corporation"]]
+    """The tax payer subtype of the company."""
+
+    type: Optional[Literal["llc", "corporation", "sole_proprietor", "non_profit", "partnership", "cooperative"]]
+    """The tax payer type of the company."""
+
+
 class Company(BaseModel):
+    id: str
+    """A stable Finch `id` (UUID v4) for the company."""
+
     accounts: Optional[List[Account]]
     """An array of bank account objects associated with the payroll/HRIS system."""
 
     departments: Optional[List[Optional[Department]]]
     """The array of company departments."""
 
     ein: Optional[str]
     """The employer identification number."""
 
     entity: Optional[Entity]
     """The entity type object."""
 
-    id: str
-    """A stable Finch `id` (UUID v4) for the company."""
-
     legal_name: Optional[str]
     """The legal name of the company."""
 
     locations: Optional[List[Optional[location.Location]]]
 
     primary_email: Optional[str]
     """The email of the main administrator on the account."""
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/company_benefit.py` & `finch_api-0.0.3/src/finch/types/hris/company_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/individual.py` & `finch_api-0.0.3/src/finch/types/hris/individual.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 class PhoneNumber(BaseModel):
     data: Optional[str]
 
     type: Optional[Literal["work", "personal"]]
 
 
 class Individual(BaseModel):
+    id: Optional[str]
+    """A stable Finch `id` (UUID v4) for an individual in the company."""
+
     dob: Optional[str]
 
     emails: Optional[List[Email]]
 
     first_name: Optional[str]
     """The legal first name of the individual."""
 
     gender: Optional[Literal["female", "male", "other", "decline_to_specify"]]
     """The gender of the individual."""
 
-    id: Optional[str]
-    """A stable Finch `id` (UUID v4) for an individual in the company."""
-
     last_name: Optional[str]
     """The legal last name of the individual."""
 
     middle_name: Optional[str]
     """The legal middle name of the individual."""
 
     phone_numbers: Optional[List[Optional[PhoneNumber]]]
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/individual_in_directory.py` & `finch_api-0.0.3/src/finch/types/hris/individual_in_directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
 
 from ..._models import BaseModel
 
-__all__ = ["IndividualInDirectory", "Manager", "Department"]
-
-
-class Manager(BaseModel):
-    id: Optional[str]
-    """A stable Finch `id` (UUID v4) for an individual in the company."""
+__all__ = ["IndividualInDirectory", "Department", "Manager"]
 
 
 class Department(BaseModel):
     name: Optional[str]
     """The name of the department."""
 
 
+class Manager(BaseModel):
+    id: Optional[str]
+    """A stable Finch `id` (UUID v4) for an individual in the company."""
+
+
 class IndividualInDirectory(BaseModel):
+    id: Optional[str]
+    """A stable Finch id (UUID v4) for an individual in the company."""
+
     department: Optional[Department]
     """The department object."""
 
     first_name: Optional[str]
     """The legal first name of the individual."""
 
-    id: Optional[str]
-    """A stable Finch id (UUID v4) for an individual in the company."""
-
     is_active: Optional[bool]
     """`true` if the individual is an active employee or contractor at the company."""
 
     last_name: Optional[str]
     """The legal last name of the individual."""
 
     manager: Optional[Manager]
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/individuals/employment_data.py` & `finch_api-0.0.3/src/finch/types/hris/individuals/employment_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 from typing_extensions import Literal
 
 from pydantic import Field as FieldInfo
 
 from ....types import income, location
 from ...._models import BaseModel
 
-__all__ = ["EmploymentData", "Manager", "Department", "Employment"]
-
-
-class Manager(BaseModel):
-    id: Optional[str]
-    """A stable Finch `id` (UUID v4) for an individual in the company."""
+__all__ = ["EmploymentData", "Department", "Employment", "Manager"]
 
 
 class Department(BaseModel):
     name: Optional[str]
     """The name of the department associated with the individual."""
 
 
@@ -29,32 +24,37 @@
     `individual_contractor`.
     """
 
     type: Optional[Literal["employee", "contractor"]]
     """The main employment type of the individual."""
 
 
+class Manager(BaseModel):
+    id: Optional[str]
+    """A stable Finch `id` (UUID v4) for an individual in the company."""
+
+
 class EmploymentData(BaseModel):
+    id: Optional[str]
+    """string A stable Finch `id` (UUID v4) for an individual in the company."""
+
     class_code: Optional[str]
     """Worker's compensation classification code for this employee"""
 
     department: Optional[Department]
     """The department object."""
 
     employment: Optional[Employment]
     """The employment object."""
 
     end_date: Optional[str]
 
     first_name: Optional[str]
     """The legal first name of the individual."""
 
-    id: Optional[str]
-    """string A stable Finch `id` (UUID v4) for an individual in the company."""
-
     income_history: Optional[List[Optional[income.Income]]]
     """The array of income history."""
 
     income: Optional[income.Income]
     """The employee's income as reported by the provider.
 
     This may not always be annualized income, but may be in units of bi-weekly,
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py` & `finch_api-0.0.3/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from typing import List
 from typing_extensions import Required, TypedDict
 
 __all__ = ["EmploymentDataRetrieveManyParams", "Request"]
 
 
+class EmploymentDataRetrieveManyParams(TypedDict, total=False):
+    requests: Required[List[Request]]
+    """The array of batch requests."""
+
+
 class Request(TypedDict, total=False):
     individual_id: Required[str]
     """A stable Finch `id` (UUID v4) for an individual in the company.
 
     There is no limit to the number of `individual_id` to send per request. It is
     preferantial to send all ids in a single request for Finch to optimize provider
     rate-limits.
     """
-
-
-class EmploymentDataRetrieveManyParams(TypedDict, total=False):
-    requests: Required[List[Request]]
-    """The array of batch requests."""
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/pay_statement.py` & `finch_api-0.0.3/src/finch/types/hris/pay_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional
 from typing_extensions import Literal
 
 from ...types import money
 from ..._models import BaseModel
 from ...types.hris import benefit_type
 
-__all__ = ["PayStatement", "Earning", "Tax", "EmployeeDeduction", "EmployerContribution"]
+__all__ = ["PayStatement", "Earning", "EmployeeDeduction", "EmployerContribution", "Tax"]
 
 
 class Earning(BaseModel):
     amount: Optional[int]
     """The earnings amount in cents."""
 
     currency: Optional[str]
@@ -43,31 +43,14 @@
             "1099",
             "other",
         ]
     ]
     """The type of earning."""
 
 
-class Tax(BaseModel):
-    amount: Optional[int]
-    """The tax amount in cents."""
-
-    currency: Optional[str]
-    """The currency code."""
-
-    employer: Optional[bool]
-    """`true` if the amount is paid by the employers."""
-
-    name: Optional[str]
-    """The exact name of tax from the pay statement."""
-
-    type: Optional[Literal["state", "federal", "local", "fica"]]
-    """The type of taxes."""
-
-
 class EmployeeDeduction(BaseModel):
     amount: Optional[int]
     """The deduction amount in cents."""
 
     currency: Optional[str]
     """The deduction currency."""
 
@@ -91,14 +74,31 @@
     name: Optional[str]
     """The contribution name from the pay statement."""
 
     type: Optional[benefit_type.BenefitType]
     """Type of benefit."""
 
 
+class Tax(BaseModel):
+    amount: Optional[int]
+    """The tax amount in cents."""
+
+    currency: Optional[str]
+    """The currency code."""
+
+    employer: Optional[bool]
+    """`true` if the amount is paid by the employers."""
+
+    name: Optional[str]
+    """The exact name of tax from the pay statement."""
+
+    type: Optional[Literal["state", "federal", "local", "fica"]]
+    """The type of taxes."""
+
+
 class PayStatement(BaseModel):
     earnings: Optional[List[Optional[Earning]]]
     """The array of earnings objects associated with this pay statement"""
 
     employee_deductions: Optional[List[Optional[EmployeeDeduction]]]
     """The array of deductions objects associated with this pay statement."""
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/pay_statement_retrieve_many_params.py` & `finch_api-0.0.3/src/finch/types/hris/pay_statement_retrieve_many_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from typing import List
 from typing_extensions import Required, TypedDict
 
 __all__ = ["PayStatementRetrieveManyParams", "Request"]
 
 
+class PayStatementRetrieveManyParams(TypedDict, total=False):
+    requests: Required[List[Request]]
+    """The array of batch requests."""
+
+
 class Request(TypedDict, total=False):
     payment_id: Required[str]
     """A stable Finch `id` (UUID v4) for a payment."""
 
     limit: int
     """Number of pay statements to return (defaults to all)."""
 
     offset: int
     """Index to start from."""
-
-
-class PayStatementRetrieveManyParams(TypedDict, total=False):
-    requests: Required[List[Request]]
-    """The array of batch requests."""
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/payment.py` & `finch_api-0.0.3/src/finch/types/hris/payment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 class PayPeriod(BaseModel):
     end_date: Optional[str]
 
     start_date: Optional[str]
 
 
 class Payment(BaseModel):
+    id: Optional[str]
+    """The unique id for the payment."""
+
     company_debit: Optional[money.Money]
 
     debit_date: Optional[str]
 
     employee_taxes: Optional[money.Money]
 
     employer_taxes: Optional[money.Money]
 
     gross_pay: Optional[money.Money]
 
-    id: Optional[str]
-    """The unique id for the payment."""
-
     individual_ids: Optional[List[str]]
     """Array of every individual on this payment."""
 
     net_pay: Optional[money.Money]
 
     pay_date: Optional[str]
```

### Comparing `finch_api-0.0.2/src/finch/types/hris/payment_list_params.py` & `finch_api-0.0.3/src/finch/types/hris/payment_list_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/hris/supported_benefit.py` & `finch_api-0.0.3/src/finch/types/hris/supported_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/income.py` & `finch_api-0.0.3/src/finch/types/income.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/introspection.py` & `finch_api-0.0.3/src/finch/types/introspection.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/location.py` & `finch_api-0.0.3/src/finch/types/location.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.2/src/finch/types/provider.py` & `finch_api-0.0.3/src/finch/types/provider.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from .._models import BaseModel
 
 __all__ = ["Provider"]
 
 
 class Provider(BaseModel):
+    id: Optional[str]
+    """The id of the payroll provider used in Connect."""
+
     display_name: Optional[str]
     """The display name of the payroll provider."""
 
     icon: Optional[str]
     """The url to the official icon of the payroll provider."""
 
-    id: Optional[str]
-    """The id of the payroll provider used in Connect."""
-
     logo: Optional[str]
     """The url to the official logo of the payroll provider."""
 
     manual: Optional[bool]
     """
     Whether the Finch integration with this provider uses the Assisted Connect Flow
     by default.
```

### Comparing `finch_api-0.0.2/PKG-INFO` & `finch_api-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Client library for the Finch API
 Home-page: https://github.com/Finch-API/finch-api-python
 License: Apache-2.0
 Author: Finch
 Author-email: founders@tryfinch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.5.0)
 Requires-Dist: distro (>=1.7.0)
 Requires-Dist: httpx (>=0.23.0)
-Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.1.1)
 Project-URL: Repository, https://github.com/Finch-API/finch-api-python
 Description-Content-Type: text/markdown
 
 # Finch Python API Library
 
 [![PyPI version](https://img.shields.io/pypi/v/finch-api.svg)](https://pypi.org/project/finch-api/)
@@ -45,17 +45,18 @@
 ```python
 from finch import Finch
 
 finch = Finch(
     access_token="my access token",
 )
 
-page = finch.hris.directory.list_individuals()
-directory = page.individuals[0]
-print(directory.ein)
+candidate = finch.ats.candidates.retrieve(
+    "<candidate id>",
+)
+print(candidate.first_name)
 ```
 
 ## Async Usage
 
 Simply import `AsyncFinch` instead of `Finch` and use `await` with each API call:
 
 ```python
@@ -63,16 +64,18 @@
 
 finch = AsyncFinch(
     access_token="my access token",
 )
 
 
 async def main():
-    page = await finch.hris.directory.list_individuals()
-    print(page.individuals[0].ein)
+    candidate = await finch.ats.candidates.retrieve(
+        "<candidate id>",
+    )
+    print(candidate.first_name)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -252,19 +255,21 @@
 
 ## Default Headers
 
 We automatically send the `Finch-API-Version` header set to `2020-09-17`.
 
 If you need to, you can override it by setting default headers per-request or on the client object.
 
+Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
+
 ```python
 from finch import Finch
 
 finch = Finch(
-    default_headers={"Finch-API-Version": My - Custom - Value},
+    default_headers={"Finch-API-Version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
@@ -283,13 +288,13 @@
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
-We are keen for your feedback; please email us at [founders@tryfinch.com](mailto:founders@tryfinch.com) or open an issue with questions,
-bugs, or suggestions.
+We are keen for your feedback; please open an [issue](https://www.github.com/Finch-API/finch-api-python/issues) with questions, bugs, or suggestions.
 
 ## Requirements
 
 Python 3.7 or higher.
+
```

