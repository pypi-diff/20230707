# Comparing `tmp/cumulus_library-0.4.0.tar.gz` & `tmp/cumulus_library-0.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.4.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.4.0.tar` & `cumulus_library-0.4.0.dev1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-lrwxr-xr-x   0        0        0        0 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      587 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/README.md
--rw-r--r--   0        0        0      963 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       45 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11182 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/cli.py
--rw-r--r--   0        0        0     5249 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      272 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6030 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2876 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2688 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/condition_codable_concept.sql
--rw-r--r--   0        0        0     3612 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0     4480 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/count_core.sql
--rw-r--r--   0        0        0     4176 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/denormalizer.py
--rw-r--r--   0        0        0     2863 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     1505 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     2040 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/encounter_type.sql
--rw-r--r--   0        0        0     4330 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      782 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1231 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2874 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1225 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     6521 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/patient_extensions.sql
--rw-r--r--   0        0        0     1426 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1481 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      824 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-07-07 18:13:23.684496 cumulus_library-0.4.0/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2023-07-07 18:13:23.724498 cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2023-07-07 18:13:23.828501 cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      394 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4643 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16059 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/study_parser.py
--rw-r--r--   0        0        0     1430 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0      577 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1798 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     7462 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2664 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/cumulus_library/upload.py
--rw-r--r--   0        0        0     1588 2023-07-07 18:13:23.836501 cumulus_library-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cumulus_library-0.4.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      587 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/README.md
+-rw-r--r--   0        0        0      963 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       51 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    11182 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5249 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6030 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2549 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2688 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql
+-rw-r--r--   0        0        0     3493 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0     4550 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.sql
+-rw-r--r--   0        0        0     4176 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/denormalizer.py
+-rw-r--r--   0        0        0     2857 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     1505 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     2001 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter_type.sql
+-rw-r--r--   0        0        0     4330 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      782 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1231 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1222 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     6521 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql
+-rw-r--r--   0        0        0     1426 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2023-07-06 16:36:22.124354 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2023-07-06 16:36:22.236356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      394 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4643 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16059 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0     1430 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0      577 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1798 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     7462 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2664 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1588 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 cumulus_library-0.4.0.dev1/PKG-INFO
```

### Comparing `cumulus_library-0.4.0/README.md` & `cumulus_library-0.4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/.sqlfluff` & `cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/base_runner.py` & `cumulus_library-0.4.0.dev1/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/cli.py` & `cumulus_library-0.4.0.dev1/cumulus_library/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/cli_parser.py` & `cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/helper.py` & `cumulus_library-0.4.0.dev1/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/schema/columns.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/schema/counts.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/schema/typesystem.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/schema/valueset.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql`

 * *Files 12% similar despite different names*

```diff
@@ -43,42 +43,31 @@
     date_trunc('year', date(tc.recordeddate)) AS recorded_year
 FROM temp_condition AS tc,
     unnest(category) AS t_category (category_coding), --noqa
     unnest(category_coding.coding) AS t_category_coding (category_row), --noqa
     unnest(code.coding) AS t_coding (code_row) --noqa
 WHERE tc.recordeddate BETWEEN date('2016-01-01') AND current_date;
 
--- ###########################################################################
--- Encounter.diagnosis may also join, we can't rely on link to encounter!
--- cond_month is a similar enough proxy for encounter month
-
-CREATE TABLE core__count_condition_month AS WITH
-concept_map AS (
-    SELECT
-        c.recorded_month AS cond_month,
-        c.subject_ref,
-        coalesce(c.encounter_ref, 'None') AS encounter_ref,
-        coalesce(mapping.display, 'None') AS cond_code_display,
-        c.category.code AS cond_category_code
-    FROM core__condition AS c
-    LEFT JOIN core__condition_codable_concepts AS mapping
-        ON c.condition_id = mapping.id
-),
-
-powerset AS (
+CREATE TABLE core__count_condition_month AS
+WITH powerset AS (
     SELECT
-        count(DISTINCT subject_ref) AS cnt_subject,
-        count(DISTINCT encounter_ref) AS cnt_encounter,
-        cond_category_code,
-        cond_month,
-        cond_code_display
-    FROM concept_map
-    GROUP BY cube(cond_category_code, cond_month, cond_code_display)
+        count(DISTINCT cc.subject_ref) AS cnt_subject,
+        count(DISTINCT cc.encounter_ref) AS cnt_encounter,
+        cccc.display AS display,
+        cc.recorded_month,
+        ce.enc_class
+    FROM core__condition AS cc
+    INNER JOIN core__encounter AS ce
+        ON cc.encounter_ref = ce.encounter_ref
+    LEFT JOIN core__condition_codable_concepts AS cccc
+        ON cc.condition_id = cccc.id
+    GROUP BY cube(display, cc.recorded_month, ce.enc_class)
 )
 
-SELECT DISTINCT
+SELECT
     powerset.cnt_subject AS cnt,
-    powerset.cond_category_code,
-    powerset.cond_month,
-    powerset.cond_code_display
+    powerset.recorded_month AS cond_month,
+    powerset.display AS cond_code_display,
+    enc_class.code AS enc_class_code
 FROM powerset
-WHERE powerset.cnt_subject >= 10;
+WHERE powerset.cnt_subject >= 10
+ORDER BY powerset.cnt_subject DESC, powerset.cnt_encounter DESC;
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/condition_codable_concept.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/count_core.py` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,18 +96,15 @@
 
 
 def write_view_sql(view_list_sql: List[str], filename="count_core.sql") -> None:
     """
     :param view_list_sql: SQL prepared statements
     :param filename: path to output file, default 'count_core.sql' in PWD
     """
-    sql_optimizer = concat_view_sql(view_list_sql)
-    sql_optimizer = sql_optimizer.replace("ORDER BY cnt desc", "")
-    sql_optimizer = sql_optimizer.replace("CREATE or replace VIEW", "CREATE TABLE")
-
+    sql_optimizer = concat_view_sql(view_list_sql).replace("ORDER BY cnt desc", "")
     with open(filename, "w") as fout:
         fout.write(sql_optimizer)
 
 
 if __name__ == "__main__":
     write_view_sql(
         [
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/count_core.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -- ###########################################################
-CREATE TABLE core__count_patient AS
+CREATE OR REPLACE VIEW core__count_patient AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
 
         age,
         gender,
         race_display,
@@ -18,15 +18,15 @@
     gender,
     race_display,
     ethnicity_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_month AS
+CREATE OR REPLACE VIEW core__count_encounter_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         start_month,
         enc_class_display,
         age_at_visit,
@@ -53,15 +53,15 @@
     gender,
     race_display,
     ethnicity_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_type AS
+CREATE OR REPLACE VIEW core__count_encounter_type AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         enc_service_display,
@@ -82,15 +82,15 @@
     enc_type_display,
     enc_service_display,
     enc_priority_display
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_type_month AS
+CREATE OR REPLACE VIEW core__count_encounter_type_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         enc_service_display,
@@ -114,15 +114,15 @@
     enc_service_display,
     enc_priority_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_enc_type_month AS
+CREATE OR REPLACE VIEW core__count_encounter_enc_type_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_type_display,
         start_month
@@ -135,15 +135,15 @@
     enc_class_display,
     enc_type_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_service_month AS
+CREATE OR REPLACE VIEW core__count_encounter_service_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_service_display,
         start_month
@@ -156,15 +156,15 @@
     enc_class_display,
     enc_service_display,
     start_month
 FROM powerset
 WHERE cnt_subject >= 10;
 
 -- ###########################################################
-CREATE TABLE core__count_encounter_priority_month AS
+CREATE OR REPLACE VIEW core__count_encounter_priority_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT subject_ref) AS cnt_subject,
         count(DISTINCT encounter_ref) AS cnt_encounter,
         enc_class_display,
         enc_priority_display,
         start_month
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/denormalizer.py` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/denormalizer.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         ) AS author_date,
         concat('DocumentReference/', dr.id) AS doc_ref
     FROM documentreference AS dr
 )
 
 SELECT DISTINCT
     type_coding.type_row AS doc_type,
-    coalesce(type_coding.type_row.code, 'None') AS doc_type_code,
+    coalesce(type_coding.type_row.code, '?') AS doc_type_code,
     CASE
         WHEN
             type_coding.type_row.display IS NOT NULL
             THEN replace(type_coding.type_row.display, ',')
         ELSE type_row.code
     END AS doc_type_display,
     tdr.status,
@@ -61,15 +61,15 @@
 WITH powerset AS (
     SELECT
         count(DISTINCT d.subject_ref) AS cnt_subject,
         count(DISTINCT d.encounter_ref) AS cnt_encounter,
         count(DISTINCT d.doc_id) AS cnt_document,
         d.doc_type_display,
         d.author_month,
-        e.enc_class.display AS enc_class_code
+        e.enc_class.code AS enc_class_code
     FROM core__documentreference AS d, core__encounter AS e
     WHERE d.encounter_ref = e.encounter_ref
     GROUP BY cube(d.doc_type_display, d.author_month, e.enc_class)
 )
 
 SELECT DISTINCT
     cnt_document AS cnt,
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/encounter_type.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter_type.sql`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 CREATE TABLE core__encounter_type AS WITH
 join_enc_type AS (
     SELECT DISTINCT
         e.encounter_id,
         t.as_coding
     FROM core__encounter AS e,
         unnest(enc_type) AS tr (as_row), --noqa: AL05
-        unnest(tr.as_row.coding) AS t (as_coding) --noqa: AL05
+        unnest(tr.as_row.coding) AS t (as_coding)
 ),
 
 join_service AS (
     SELECT DISTINCT
         e.encounter_id,
         t.as_coding
     FROM core__encounter AS e,
-        unnest(service_type.coding) AS t (as_coding) --noqa: AL05
+        unnest(service_type.coding) AS t (as_coding)
 ),
 
 join_priority AS (
     SELECT DISTINCT
         e.encounter_id,
         t.as_coding
     FROM core__encounter AS e,
-        unnest(priority.coding) AS t (as_coding) --noqa: AL05
+        unnest(priority.coding) AS t (as_coding)
 )
 
 SELECT DISTINCT
     e.enc_class_code,
     e.enc_class_display,
     coalesce(join_enc_type.as_coding.system, 'None') AS enc_type_system,
     coalesce(join_enc_type.as_coding.code, 'None') AS enc_type_code,
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/observation.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     tp.gender,
     tp.birthdate,
     date_diff('year', tp.birthdate, current_date) AS age,
     CASE
         WHEN
             t_address.addr_row.postalcode IS NOT NULL
             THEN substr(t_address.addr_row.postalcode, 1, 3)
-        ELSE 'None'
+        ELSE '?'
     END AS postalcode3,
     tp.subject_id,
     tp.subject_ref,
     coalesce(tp.race_display, ARRAY['unknown']) AS race_display,
     coalesce(tp.ethnicity_display, ARRAY['unknown']) AS ethnicity_display
 FROM
     temp_patient AS tp,
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/patient_extensions.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         cp.gender,
         cp.race_display,
         cp.ethnicity_display,
         cp.subject_ref,
         ce.encounter_ref,
         cd.doc_ref,
         date_diff('day', ce.start_date, cd.author_date) AS diff_enc_note_days,
-        coalesce(ce.enc_class.display, 'None') AS enc_class_code,
-        coalesce(cd.doc_type.code, 'None') AS doc_type_code,
+        coalesce(ce.enc_class.code, '?') AS enc_class_code,
+        coalesce(cd.doc_type.code, '?') AS doc_type_code,
         coalesce(cd.doc_type.display, cd.doc_type.code) AS doc_type_display
     FROM
         core__patient AS cp,
         core__encounter AS ce,
         core__documentreference AS cd
     WHERE
         (cp.subject_ref = ce.subject_ref)
```

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/study_parser.py` & `cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/template_sql/templates.py` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/cumulus_library/upload.py` & `cumulus_library-0.4.0.dev1/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/pyproject.toml` & `cumulus_library-0.4.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.4.0/PKG-INFO` & `cumulus_library-0.4.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.4.0
+Version: 0.4.0.dev1
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

