# Comparing `tmp/spidermon-1.8.0.tar.gz` & `tmp/spidermon-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spidermon-1.8.0.tar", last modified: Fri Jan 11 13:42:51 2019, max compression
+gzip compressed data, was "dist/spidermon-1.9.0.tar", last modified: Wed Mar 13 11:47:50 2019, max compression
```

## Comparing `spidermon-1.8.0.tar` & `spidermon-1.9.0.tar`

### file list

```diff
@@ -1,160 +1,166 @@
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon.egg-info/
--rw-rw-r--   0 renne     (1001) renne     (1001)     4712 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon.egg-info/SOURCES.txt
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-11-13 19:25:15.000000 spidermon-1.8.0/spidermon.egg-info/not-zip-safe
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2019-01-11 13:42:50.000000 spidermon-1.8.0/spidermon.egg-info/dependency_links.txt
--rw-rw-r--   0 renne     (1001) renne     (1001)      197 2019-01-11 13:42:50.000000 spidermon-1.8.0/spidermon.egg-info/requires.txt
--rw-rw-r--   0 renne     (1001) renne     (1001)     1042 2019-01-11 13:42:50.000000 spidermon-1.8.0/spidermon.egg-info/PKG-INFO
--rw-rw-r--   0 renne     (1001) renne     (1001)       16 2019-01-11 13:42:50.000000 spidermon-1.8.0/spidermon.egg-info/top_level.txt
--rw-rw-r--   0 renne     (1001) renne     (1001)     1042 2019-01-11 13:42:51.000000 spidermon-1.8.0/PKG-INFO
--rw-rw-r--   0 renne     (1001) renne     (1001)       88 2019-01-11 13:42:51.000000 spidermon-1.8.0/setup.cfg
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/tests/
--rw-rw-r--   0 renne     (1001) renne     (1001)    57973 2018-11-13 19:05:18.000000 spidermon-1.8.0/tests/test_validators_jsonschema.py
--rw-rw-r--   0 renne     (1001) renne     (1001)    21101 2018-11-13 19:05:18.000000 spidermon-1.8.0/tests/test_validators_schematics.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     7231 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_suites.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2169 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_descriptions.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/tests/fixtures/
--rw-rw-r--   0 renne     (1001) renne     (1001)     4229 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/expressions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      344 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/cases.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1481 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/ordering.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      331 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/stats.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        0 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2429 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/levels.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      849 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/validators.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1360 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/names.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1666 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/descriptions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      517 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/suites.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      198 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/fixtures/items.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        0 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1174 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_data.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     6325 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_levels.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1074 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_expressions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1608 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_loaders.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     8304 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_names.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3483 2018-10-23 19:46:59.000000 spidermon-1.8.0/tests/test_ordering.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/utils/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1178 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/utils/text.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/utils/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2086 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/utils/hubstorage.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/core/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1801 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/options.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2866 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/monitors.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1637 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/actions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3833 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/factories.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     6634 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/core/suites.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1519 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/loaders.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/monitors/
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/monitors/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/
--rw-rw-r--   0 renne     (1001) renne     (1001)     4208 2018-11-13 19:05:18.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/spider.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      275 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/stats.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      155 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      265 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/job.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     7698 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/monitors/mixins/validation.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/
--rw-rw-r--   0 renne     (1001) renne     (1001)     7431 2018-12-13 15:42:15.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/default/
--rw-rw-r--   0 renne     (1001) renne     (1001)       30 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/default/message.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)       59 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/default/attachments.jinja
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/
--rw-rw-r--   0 renne     (1001) renne     (1001)      244 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/message.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)      310 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/attachments.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)     1107 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/macros.jinja
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/
--rw-rw-r--   0 renne     (1001) renne     (1001)      384 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/message.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)      310 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/attachments.jinja
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/start/
--rw-rw-r--   0 renne     (1001) renne     (1001)      170 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/start/message.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)     2771 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/slack/notifiers.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/email/
--rw-rw-r--   0 renne     (1001) renne     (1001)     5099 2018-12-13 15:42:15.000000 spidermon-1.8.0/spidermon/contrib/actions/email/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1269 2018-12-13 15:42:15.000000 spidermon-1.8.0/spidermon/contrib/actions/email/ses.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/jobs/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1516 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/jobs/tags.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/jobs/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      128 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/
--rw-rw-r--   0 renne     (1001) renne     (1001)     5135 2018-12-21 14:02:49.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/s3.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1164 2018-11-13 19:05:18.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/
--rw-rw-r--   0 renne     (1001) renne     (1001)    14362 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)     3238 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.css
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1264 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/report.css
--rw-rw-r--   0 renne     (1001) renne     (1001)      104 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/small.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)     3755 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/email.css
--rw-rw-r--   0 renne     (1001) renne     (1001)      868 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/base.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)      105 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/medium.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)      102 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/big.jinja
--rw-rw-r--   0 renne     (1001) renne     (1001)      900 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/actions/reports/files.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1751 2019-01-03 19:45:12.000000 spidermon-1.8.0/spidermon/contrib/actions/templates.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/scrapy/
--rw-rw-r--   0 renne     (1001) renne     (1001)     4344 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/scrapy/extensions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     6584 2018-11-20 19:05:59.000000 spidermon-1.8.0/spidermon/contrib/scrapy/pipelines.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1665 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/scrapy/stats.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/scrapy/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     4254 2018-11-13 19:05:18.000000 spidermon-1.8.0/spidermon/contrib/scrapy/runners.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/validation/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1642 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/messages.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1330 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/validator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      575 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/translator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      108 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/validation/schematics/
--rw-rw-r--   0 renne     (1001) renne     (1001)     4082 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/schematics/validator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3790 2018-11-13 19:05:18.000000 spidermon-1.8.0/spidermon/contrib/validation/schematics/translator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/schematics/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1069 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/schematics/monkeypatches.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      860 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/utils.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/validation/jsonschema/
--rw-rw-r--   0 renne     (1001) renne     (1001)      880 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/jsonschema/formats.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1279 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/jsonschema/validator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3425 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/jsonschema/translator.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/validation/jsonschema/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/pytest/
--rw-rw-r--   0 renne     (1001) renne     (1001)        0 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/pytest/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/pytest/plugins/
--rw-rw-r--   0 renne     (1001) renne     (1001)      376 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/pytest/plugins/filter_monitors.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/pytest/plugins/__init__.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/contrib/stats/
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/stats/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      792 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/stats/analyzer.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2901 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/contrib/stats/counters.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      462 2019-01-08 18:52:25.000000 spidermon-1.8.0/spidermon/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3623 2018-12-28 17:32:17.000000 spidermon-1.8.0/spidermon/runners.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      757 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/data.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3327 2018-12-21 14:03:47.000000 spidermon-1.8.0/spidermon/settings.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/python/
--rw-rw-r--   0 renne     (1001) renne     (1001)     1042 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/context.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3346 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/interpreter.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      694 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/monitors.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      119 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3207 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/factory.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      731 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/python/schemas.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      587 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/exceptions.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/decorators/
--rw-rw-r--   0 renne     (1001) renne     (1001)      809 2018-11-20 20:09:11.000000 spidermon-1.8.0/spidermon/decorators/monitors.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      269 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/decorators/actions.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     1257 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/decorators/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     2114 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/templates.py
-drwxrwxr-x   0 renne     (1001) renne     (1001)        0 2019-01-11 13:42:51.000000 spidermon-1.8.0/spidermon/results/
--rw-rw-r--   0 renne     (1001) renne     (1001)     5380 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/results/text.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     5330 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/results/monitor.py
--rw-rw-r--   0 renne     (1001) renne     (1001)        1 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/results/__init__.py
--rw-rw-r--   0 renne     (1001) renne     (1001)     3089 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/results/steps.py
--rw-rw-r--   0 renne     (1001) renne     (1001)      787 2018-10-23 19:46:59.000000 spidermon-1.8.0/spidermon/results/items.py
--rw-rw-r--   0 renne     (1001) renne     (1001)       57 2018-11-13 19:05:18.000000 spidermon-1.8.0/MANIFEST.in
--rw-rw-r--   0 renne     (1001) renne     (1001)     1511 2018-11-13 19:05:18.000000 spidermon-1.8.0/LICENSE
--rw-rw-r--   0 renne     (1001) renne     (1001)     2088 2019-01-08 18:52:25.000000 spidermon-1.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2019-03-13 11:46:09.000000 spidermon-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-03-13 11:46:09.000000 spidermon-1.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1160 2019-03-13 11:47:50.000000 spidermon-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1490 2019-03-13 11:46:09.000000 spidermon-1.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-03-13 11:47:50.000000 spidermon-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2019-03-13 11:46:09.000000 spidermon-1.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/email/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5192 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/email/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/email/ses.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/jobs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/jobs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/jobs/tags.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1198 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      877 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/files.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5316 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/s3.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      868 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/base.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/big.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3755 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/email.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/medium.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1264 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/report.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/small.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3238 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14362 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/sentry/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4411 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/sentry/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7696 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3042 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/notifiers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/default/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/default/attachments.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/default/message.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/attachments.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      384 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/message.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/macros.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/attachments.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      244 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/periodic/message.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/start/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      170 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/start/message.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1751 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/actions/templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/monitors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4136 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      275 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/stats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8096 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/monitors/mixins/validation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/pytest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/pytest/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/pytest/plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/pytest/plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/pytest/plugins/filter_monitors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/scrapy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5365 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/extensions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5131 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/monitors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6652 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4332 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/runners.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/scrapy/stats.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/stats/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/stats/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/stats/analyzer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2903 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/stats/counters.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/validation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/validation/jsonschema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/jsonschema/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      548 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/jsonschema/formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2626 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/jsonschema/translator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/jsonschema/validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1642 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/messages.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/contrib/validation/schematics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/schematics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/schematics/monkeypatches.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2979 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/schematics/translator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/schematics/validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/translator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/contrib/validation/validator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1620 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3788 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2854 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/monitors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/options.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6672 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/core/suites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      781 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/decorators/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1366 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/decorators/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/decorators/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/decorators/monitors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/loaders.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/python/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/context.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3216 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/factory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/interpreter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/monitors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/python/schemas.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/results/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/results/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      788 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/results/items.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5367 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/results/monitor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3155 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/results/steps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5455 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/results/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3602 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/runners.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3129 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/utils/hubstorage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-03-13 11:46:09.000000 spidermon-1.9.0/spidermon/utils/text.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1160 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4852 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-03-13 11:47:50.000000 spidermon-1.9.0/spidermon.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 11:47:50.000000 spidermon-1.9.0/tests/fixtures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/cases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/descriptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4156 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/items.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2668 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/levels.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/names.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/ordering.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      316 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/stats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      417 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/suites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      720 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/fixtures/validators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1173 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2187 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_descriptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3895 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_extension.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5748 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_levels.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1465 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_loaders.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5762 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_monitors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8273 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_names.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3412 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_ordering.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6293 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_suites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53641 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_validators_jsonschema.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19713 2019-03-13 11:46:09.000000 spidermon-1.9.0/tests/test_validators_schematics.py
```

### Comparing `spidermon-1.8.0/spidermon.egg-info/SOURCES.txt` & `spidermon-1.9.0/spidermon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+README.rst
 setup.cfg
 setup.py
 spidermon/__init__.py
 spidermon/data.py
 spidermon/exceptions.py
 spidermon/loaders.py
 spidermon/runners.py
@@ -29,14 +30,15 @@
 spidermon/contrib/actions/reports/templates/reports/email/bases/report/big.jinja
 spidermon/contrib/actions/reports/templates/reports/email/bases/report/email.css
 spidermon/contrib/actions/reports/templates/reports/email/bases/report/medium.jinja
 spidermon/contrib/actions/reports/templates/reports/email/bases/report/report.css
 spidermon/contrib/actions/reports/templates/reports/email/bases/report/small.jinja
 spidermon/contrib/actions/reports/templates/reports/email/monitors/result.css
 spidermon/contrib/actions/reports/templates/reports/email/monitors/result.jinja
+spidermon/contrib/actions/sentry/__init__.py
 spidermon/contrib/actions/slack/__init__.py
 spidermon/contrib/actions/slack/notifiers.py
 spidermon/contrib/actions/slack/templates/slack/default/attachments.jinja
 spidermon/contrib/actions/slack/templates/slack/default/message.jinja
 spidermon/contrib/actions/slack/templates/slack/spider/notifier/macros.jinja
 spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/attachments.jinja
 spidermon/contrib/actions/slack/templates/slack/spider/notifier/finish/message.jinja
@@ -50,14 +52,15 @@
 spidermon/contrib/monitors/mixins/stats.py
 spidermon/contrib/monitors/mixins/validation.py
 spidermon/contrib/pytest/__init__.py
 spidermon/contrib/pytest/plugins/__init__.py
 spidermon/contrib/pytest/plugins/filter_monitors.py
 spidermon/contrib/scrapy/__init__.py
 spidermon/contrib/scrapy/extensions.py
+spidermon/contrib/scrapy/monitors.py
 spidermon/contrib/scrapy/pipelines.py
 spidermon/contrib/scrapy/runners.py
 spidermon/contrib/scrapy/stats.py
 spidermon/contrib/stats/__init__.py
 spidermon/contrib/stats/analyzer.py
 spidermon/contrib/stats/counters.py
 spidermon/contrib/validation/__init__.py
@@ -96,16 +99,18 @@
 spidermon/utils/__init__.py
 spidermon/utils/hubstorage.py
 spidermon/utils/text.py
 tests/__init__.py
 tests/test_data.py
 tests/test_descriptions.py
 tests/test_expressions.py
+tests/test_extension.py
 tests/test_levels.py
 tests/test_loaders.py
+tests/test_monitors.py
 tests/test_names.py
 tests/test_ordering.py
 tests/test_suites.py
 tests/test_validators_jsonschema.py
 tests/test_validators_schematics.py
 tests/fixtures/__init__.py
 tests/fixtures/cases.py
```

### Comparing `spidermon-1.8.0/spidermon.egg-info/PKG-INFO` & `spidermon-1.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spidermon
-Version: 1.8.0
+Version: 1.9.0
 Summary: Spidermon is a framework to build monitors for Scrapy spiders.
 Home-page: https://github.com/scrapinghub/spidermon
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 License: BSD
 Description: Spidermon is a framework to build monitors for Scrapy spiders.
 Platform: UNKNOWN
@@ -19,7 +19,12 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: monitoring
+Provides-Extra: tests
+Provides-Extra: validation
+Provides-Extra: pep8
+Provides-Extra: docs
```

### Comparing `spidermon-1.8.0/PKG-INFO` & `spidermon-1.9.0/spidermon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spidermon
-Version: 1.8.0
+Version: 1.9.0
 Summary: Spidermon is a framework to build monitors for Scrapy spiders.
 Home-page: https://github.com/scrapinghub/spidermon
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 License: BSD
 Description: Spidermon is a framework to build monitors for Scrapy spiders.
 Platform: UNKNOWN
@@ -19,7 +19,12 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: monitoring
+Provides-Extra: tests
+Provides-Extra: validation
+Provides-Extra: pep8
+Provides-Extra: docs
```

### Comparing `spidermon-1.8.0/tests/test_validators_jsonschema.py` & `spidermon-1.9.0/tests/test_validators_jsonschema.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 
 
 class SchemaTestCaseMetaclass(type):
     def __new__(mcs, name, bases, attrs):
         def _test_function(data_test):
             def _function(self):
                 validator = JSONSchemaValidator(data_test.schema or self.schema)
-                assert validator.validate(data_test.data) == (data_test.valid, data_test.expected_errors)
+                assert validator.validate(data_test.data) == (
+                    data_test.valid,
+                    data_test.expected_errors,
+                )
+
             return _function
+
         cls = super(SchemaTestCaseMetaclass, mcs).__new__(mcs, name, bases, attrs)
-        for dt in getattr(cls, 'data_tests', []):
-            function_name = 'test_%s' % slugify(dt.name, separator='_').lower()
+        for dt in getattr(cls, "data_tests", []):
+            function_name = "test_%s" % slugify(dt.name, separator="_").lower()
             setattr(cls, function_name, _test_function(dt))
         return cls
 
 
 class SchemaTest(six.with_metaclass(SchemaTestCaseMetaclass, TestCase)):
     schema = {}
     data_tests = []
@@ -37,62 +42,43 @@
         self.schema = schema
 
 
 class AdditionalItems(SchemaTest):
     data_tests = [
         DataTest(
             name="additionalItems as schema, additional items match schema",
-            schema={
-                "items": [{}],
-                "additionalItems": {"type": "integer"},
-            },
+            schema={"items": [{}], "additionalItems": {"type": "integer"}},
             data=[None, 2, 3, 4],
             valid=True,
         ),
         DataTest(
             name="additionalItems as schema, additional items do not match schema",
-            schema={
-                "items": [{}],
-                "additionalItems": {"type": "integer"},
-            },
+            schema={"items": [{}], "additionalItems": {"type": "integer"}},
             data=[None, 2, 3, "foo"],
             valid=False,
-            expected_errors={
-                '3': [messages.INVALID_INT],
-            }
+            expected_errors={"3": [messages.INVALID_INT]},
         ),
         DataTest(
             name="no additionalItems, all items match schema",
-            schema={
-                "items": {},
-                "additionalItems": False
-            },
+            schema={"items": {}, "additionalItems": False},
             data=[1, 2, 3, 4, 5],
-            valid=True
+            valid=True,
         ),
         DataTest(
             name="array of items with no additionalItems, no additional items present",
-            schema={
-                "items": [{}, {}, {}],
-                "additionalItems": False
-            },
+            schema={"items": [{}, {}, {}], "additionalItems": False},
             data=[1, 2, 3],
-            valid=True
+            valid=True,
         ),
         DataTest(
             name="array of items with no additionalItems, additional items are not permitted",
-            schema={
-                "items": [{}, {}, {}],
-                "additionalItems": False
-            },
+            schema={"items": [{}, {}, {}], "additionalItems": False},
             data=[1, 2, 3, 4],
             valid=False,
-            expected_errors={
-                '': [messages.TOO_MANY_ITEMS],
-            }
+            expected_errors={"": [messages.TOO_MANY_ITEMS]},
         ),
         DataTest(
             name="additionalItems as false without items, valid",
             schema={"additionalItems": False},
             data=[1, 2, 3, 4, 5],
             valid=True,
         ),
@@ -109,61 +95,55 @@
             valid=True,
         ),
         DataTest(
             name="array, sequence without extra item",
             schema={
                 "type": "array",
                 "items": [{"type": "boolean"}, {"type": "integer"}, {"type": "string"}],
-                "additionalItems": {"type": "boolean"}
+                "additionalItems": {"type": "boolean"},
             },
             data=[True, 1, "foo"],
             valid=True,
         ),
         DataTest(
             name="array, sequence with valid extra item",
             schema={
                 "type": "array",
                 "items": [{"type": "boolean"}, {"type": "integer"}, {"type": "string"}],
-                "additionalItems": {"type": "boolean"}
+                "additionalItems": {"type": "boolean"},
             },
             data=[True, 1, "foo", True],
             valid=True,
         ),
         DataTest(
             name="array, sequence with invalid extra item",
             schema={
                 "type": "array",
                 "items": [{"type": "boolean"}, {"type": "integer"}, {"type": "string"}],
-                "additionalItems": {"type": "boolean"}
+                "additionalItems": {"type": "boolean"},
             },
             data=[True, 1, "foo", 1],
             valid=False,
-            expected_errors={
-                '3': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"3": [messages.INVALID_BOOLEAN]},
         ),
     ]
 
 
 class AdditionalProperties(SchemaTest):
     schema_false = {
         "properties": {"foo": {}, "bar": {}},
         "patternProperties": {"^v": {}},
-        "additionalProperties": False
+        "additionalProperties": False,
     }
     schema_allows_schema = {
         "properties": {"foo": {}, "bar": {}},
-        "additionalProperties": {"type": "boolean"}
-    }
-    schema_alone = {
-        "additionalProperties": {"type": "boolean"}
-    }
-    schema_no = {
-        "properties": {"foo": {}, "bar": {}}
+        "additionalProperties": {"type": "boolean"},
     }
+    schema_alone = {"additionalProperties": {"type": "boolean"}}
+    schema_no = {"properties": {"foo": {}, "bar": {}}}
     data_tests = [
         DataTest(
             name="schema_false, no additional properties is valid",
             schema=schema_false,
             data={"foo": 1},
             valid=True,
         ),
@@ -173,16 +153,16 @@
             data={"foo": 1, "bar": 2, "quux": "boom"},
             valid=False,
             expected_errors={
                 # Used with jsonschema 2.4.0:
                 # '': [messages.UNEXPECTED_FIELD],
                 # This changed in jsonschema 2.6.0:
                 # https://github.com/Julian/jsonschema/pull/317
-                '': [messages.REGEX_NOT_MATCHED],
-            }
+                "": [messages.REGEX_NOT_MATCHED]
+            },
         ),
         DataTest(
             name="schema_false, ignores non-objects",
             schema=schema_false,
             data=[1, 2, 3],
             valid=True,
         ),
@@ -197,197 +177,139 @@
             schema=schema_allows_schema,
             data={"foo": 1},
             valid=True,
         ),
         DataTest(
             name="schema_allows_schema, additional valid property",
             schema=schema_allows_schema,
-            data={"foo": 1, "bar": 2, "quux" : True},
+            data={"foo": 1, "bar": 2, "quux": True},
             valid=True,
         ),
         DataTest(
             name="schema_allows_schema, additional invalid property",
             schema=schema_allows_schema,
-            data={"foo": 1, "bar": 2, "quux" : 12},
+            data={"foo": 1, "bar": 2, "quux": 12},
             valid=False,
-            expected_errors={
-                'quux': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"quux": [messages.INVALID_BOOLEAN]},
         ),
         DataTest(
             name="schema_alone, additional valid property",
             schema=schema_alone,
             data={"foo": True},
             valid=True,
         ),
         DataTest(
             name="schema_alone, additional invalid property",
             schema=schema_alone,
             data={"foo": 1},
             valid=False,
-            expected_errors={
-                'foo': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"foo": [messages.INVALID_BOOLEAN]},
         ),
         DataTest(
             name="schema_no, additional properties are allowed",
             schema=schema_no,
-            data={"foo":1, "bar":2, "quux":True},
+            data={"foo": 1, "bar": 2, "quux": True},
             valid=True,
         ),
     ]
 
 
 class AllOf(SchemaTest):
     schema = {
         "type": "object",
-        "properties": {
-            "A": {"type": "boolean"},
-            "B": {"type": "boolean"}
-        },
-        "allOf": [
-            {"required": ["A"]},
-            {"required": ["B"]}
-        ]
+        "properties": {"A": {"type": "boolean"}, "B": {"type": "boolean"}},
+        "allOf": [{"required": ["A"]}, {"required": ["B"]}],
     }
     data_tests = [
         DataTest(
             name="Empty object",
             data={},
             valid=False,
             expected_errors={
-                'A': [messages.MISSING_REQUIRED_FIELD],
-                'B': [messages.MISSING_REQUIRED_FIELD],
-            }
+                "A": [messages.MISSING_REQUIRED_FIELD],
+                "B": [messages.MISSING_REQUIRED_FIELD],
+            },
         ),
         DataTest(
             name="Mismatch B",
             data={"A": True},
             valid=False,
-            expected_errors={
-                'B': [messages.MISSING_REQUIRED_FIELD],
-            }
+            expected_errors={"B": [messages.MISSING_REQUIRED_FIELD]},
         ),
         DataTest(
             name="Mismatch A",
             data={"B": True},
             valid=False,
-            expected_errors={
-                'A': [messages.MISSING_REQUIRED_FIELD],
-            }
-        ),
-        DataTest(
-            name="Both values",
-            data={"A": False, "B": False},
-            valid=True,
+            expected_errors={"A": [messages.MISSING_REQUIRED_FIELD]},
         ),
+        DataTest(name="Both values", data={"A": False, "B": False}, valid=True),
         DataTest(
             name="Wrong type for A",
             data={"A": 1, "B": False},
             valid=False,
-            expected_errors={
-                'A': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"A": [messages.INVALID_BOOLEAN]},
         ),
         DataTest(
             name="Wrong type for both",
             data={"A": 1, "B": 1},
             valid=False,
             expected_errors={
-                'A': [messages.INVALID_BOOLEAN],
-                'B': [messages.INVALID_BOOLEAN],
-            }
+                "A": [messages.INVALID_BOOLEAN],
+                "B": [messages.INVALID_BOOLEAN],
+            },
         ),
     ]
 
 
 class AnyOf(SchemaTest):
     schema = {
         "type": "object",
-        "properties": {
-            "A": {"type": "boolean"},
-            "B": {"type": "boolean"}
-        },
-        "anyOf": [
-            {"required": ["A"]},
-            {"required": ["B"]}
-        ]
+        "properties": {"A": {"type": "boolean"}, "B": {"type": "boolean"}},
+        "anyOf": [{"required": ["A"]}, {"required": ["B"]}],
     }
     data_tests = [
         DataTest(
             name="Empty object",
             data={},
             valid=False,
-            expected_errors={
-                '': [messages.NOT_VALID_UNDER_ANY_SCHEMA],
-            }
-        ),
-        DataTest(
-            name="Mismatch B",
-            data={"A": True},
-            valid=True,
-        ),
-        DataTest(
-            name="Mismatch A",
-            data={"B": True},
-            valid=True,
-        ),
-        DataTest(
-            name="Both values",
-            data={"A": False, "B": False},
-            valid=True,
+            expected_errors={"": [messages.NOT_VALID_UNDER_ANY_SCHEMA]},
         ),
+        DataTest(name="Mismatch B", data={"A": True}, valid=True),
+        DataTest(name="Mismatch A", data={"B": True}, valid=True),
+        DataTest(name="Both values", data={"A": False, "B": False}, valid=True),
         DataTest(
             name="Wrong type for A",
             data={"A": 1, "B": False},
             valid=False,
-            expected_errors={
-                'A': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"A": [messages.INVALID_BOOLEAN]},
         ),
         DataTest(
             name="Wrong type for both",
             data={"A": 1, "B": 1},
             valid=False,
             expected_errors={
-                'A': [messages.INVALID_BOOLEAN],
-                'B': [messages.INVALID_BOOLEAN],
-            }
+                "A": [messages.INVALID_BOOLEAN],
+                "B": [messages.INVALID_BOOLEAN],
+            },
         ),
     ]
 
 
 class Dependencies(SchemaTest):
-    schema_single = {
-        "dependencies": {
-            "bar": ["foo"],
-        },
-    }
-    schema_multiple = {
-        "dependencies": {
-            "quux": ["foo", "bar"],
-        },
-    }
+    schema_single = {"dependencies": {"bar": ["foo"]}}
+    schema_multiple = {"dependencies": {"quux": ["foo", "bar"]}}
     schema_multiple_subschema = {
         "dependencies": {
             "bar": {
-                "properties": {
-                    "foo": {"type": "integer"},
-                    "bar": {"type": "integer"},
-                },
-            },
-        },
+                "properties": {"foo": {"type": "integer"}, "bar": {"type": "integer"}}
+            }
+        }
     }
     data_tests = [
-        DataTest(
-            name="single, neither",
-            schema=schema_single,
-            data={},
-            valid=True,
-        ),
+        DataTest(name="single, neither", schema=schema_single, data={}, valid=True),
         DataTest(
             name="single, nondependant",
             schema=schema_single,
             data={"foo": 1},
             valid=True,
         ),
         DataTest(
@@ -397,30 +319,23 @@
             valid=True,
         ),
         DataTest(
             name="single, missing dependency",
             schema=schema_single,
             data={"bar": 2},
             valid=False,
-            expected_errors={
-                '': [messages.MISSING_DEPENDENT_FIELD],
-            }
+            expected_errors={"": [messages.MISSING_DEPENDENT_FIELD]},
         ),
         DataTest(
             name="single, ignores non-objects",
             schema=schema_single,
             data="foo",
             valid=True,
         ),
-        DataTest(
-            name="multiple, neither",
-            schema=schema_multiple,
-            data={},
-            valid=True,
-        ),
+        DataTest(name="multiple, neither", schema=schema_multiple, data={}, valid=True),
         DataTest(
             name="multiple, nondependants",
             schema=schema_multiple,
             data={"foo": 1, "bar": 2},
             valid=True,
         ),
         DataTest(
@@ -430,34 +345,30 @@
             valid=True,
         ),
         DataTest(
             name="multiple, missing dependency",
             schema=schema_multiple,
             data={"foo": 1, "quux": 2},
             valid=False,
-            expected_errors={
-                '': [messages.MISSING_DEPENDENT_FIELD],
-            },
+            expected_errors={"": [messages.MISSING_DEPENDENT_FIELD]},
         ),
         DataTest(
             name="multiple, missing other dependency",
             schema=schema_multiple,
             data={"bar": 1, "quux": 2},
             valid=False,
-            expected_errors={
-                '': [messages.MISSING_DEPENDENT_FIELD],
-            },
+            expected_errors={"": [messages.MISSING_DEPENDENT_FIELD]},
         ),
         DataTest(
             name="multiple, missing both dependencies",
             schema=schema_multiple,
             data={"quux": 1},
             valid=False,
             expected_errors={
-                '': [messages.MISSING_DEPENDENT_FIELD, messages.MISSING_DEPENDENT_FIELD],
+                "": [messages.MISSING_DEPENDENT_FIELD, messages.MISSING_DEPENDENT_FIELD]
             },
         ),
         DataTest(
             name="multiple subschema, valid",
             schema=schema_multiple_subschema,
             data={"foo": 1, "bar": 2},
             valid=True,
@@ -469,95 +380,72 @@
             valid=True,
         ),
         DataTest(
             name="multiple subschema, wrong type",
             schema=schema_multiple_subschema,
             data={"foo": "quux", "bar": 2},
             valid=False,
-            expected_errors={
-                'foo': [messages.INVALID_INT],
-            },
+            expected_errors={"foo": [messages.INVALID_INT]},
         ),
         DataTest(
             name="multiple subschema, wrong type other",
             schema=schema_multiple_subschema,
             data={"foo": 2, "bar": "quux"},
             valid=False,
-            expected_errors={
-                'bar': [messages.INVALID_INT],
-            },
+            expected_errors={"bar": [messages.INVALID_INT]},
         ),
         DataTest(
             name="multiple subschema, wrong type both",
             schema=schema_multiple_subschema,
             data={"foo": "quux", "bar": "quux"},
             valid=False,
             expected_errors={
-                'foo': [messages.INVALID_INT],
-                'bar': [messages.INVALID_INT],
+                "foo": [messages.INVALID_INT],
+                "bar": [messages.INVALID_INT],
             },
         ),
-
     ]
 
 
 class Enum(SchemaTest):
-    schema_simple = {
-        "enum": [1, 2, 3],
-    }
-    schema_heterogeneous = {
-        "enum": [6, "foo", [], True, {"foo": 12}],
-    }
+    schema_simple = {"enum": [1, 2, 3]}
+    schema_heterogeneous = {"enum": [6, "foo", [], True, {"foo": 12}]}
     schema_properties = {
         "type": "object",
-        "properties": {
-            "foo": {"enum": ["foo"]},
-            "bar": {"enum": ["bar"]}
-        },
-        "required": ["bar"]
+        "properties": {"foo": {"enum": ["foo"]}, "bar": {"enum": ["bar"]}},
+        "required": ["bar"],
     }
     data_tests = [
-        DataTest(
-            name="simple, valid",
-            schema=schema_simple,
-            data=1,
-            valid=True,
-        ),
+        DataTest(name="simple, valid", schema=schema_simple, data=1, valid=True),
         DataTest(
             name="simple, invalid",
             schema=schema_simple,
             data=4,
             valid=False,
-            expected_errors={
-                '': [messages.VALUE_NOT_IN_CHOICES],
-            }
+            expected_errors={"": [messages.VALUE_NOT_IN_CHOICES]},
         ),
         DataTest(
             name="heterogeneous, valid",
             schema=schema_heterogeneous,
             data=[],
             valid=True,
         ),
         DataTest(
             name="heterogeneous, invalid",
             schema=schema_heterogeneous,
             data=None,
             valid=False,
-            expected_errors={
-                '': [messages.VALUE_NOT_IN_CHOICES],
-            }
+            expected_errors={"": [messages.VALUE_NOT_IN_CHOICES]},
         ),
         DataTest(
             name="heterogeneous, deep valid",
             schema=schema_heterogeneous,
             data={"foo": False},
             valid=False,
-            expected_errors={
-                '': [messages.VALUE_NOT_IN_CHOICES],
-            }
+            expected_errors={"": [messages.VALUE_NOT_IN_CHOICES]},
         ),
         DataTest(
             name="properties, both valid",
             schema=schema_properties,
             data={"foo": "foo", "bar": "bar"},
             valid=True,
         ),
@@ -568,944 +456,753 @@
             valid=True,
         ),
         DataTest(
             name="properties, missing required",
             schema=schema_properties,
             data={"foo": "foo"},
             valid=False,
-            expected_errors={
-                'bar': [messages.MISSING_REQUIRED_FIELD],
-            }
+            expected_errors={"bar": [messages.MISSING_REQUIRED_FIELD]},
         ),
         DataTest(
             name="properties, missing all",
             schema=schema_properties,
             data={},
             valid=False,
-            expected_errors={
-                'bar': [messages.MISSING_REQUIRED_FIELD],
-            }
+            expected_errors={"bar": [messages.MISSING_REQUIRED_FIELD]},
         ),
     ]
 
 
 class Format(SchemaTest):
     schema = {
         "type": "object",
         "properties": {
             "datetimes": {
                 "type": "array",
-                "items": {"type": "string", "format": "date-time"}
-            },
-            "emails": {
-                "type": "array",
-                "items": {"type": "string", "format": "email"}
-            },
-            "ipv4s": {
-                "type": "array",
-                "items": {"type": "string", "format": "ipv4"}
-            },
-            "ipv6s": {
-                "type": "array",
-                "items": {"type": "string", "format": "ipv6"}
+                "items": {"type": "string", "format": "date-time"},
             },
+            "emails": {"type": "array", "items": {"type": "string", "format": "email"}},
+            "ipv4s": {"type": "array", "items": {"type": "string", "format": "ipv4"}},
+            "ipv6s": {"type": "array", "items": {"type": "string", "format": "ipv6"}},
             "hostnames": {
                 "type": "array",
-                "items": {"type": "string", "format": "hostname"}
-            },
-            "urls": {
-                "type": "array",
-                "items": {"type": "string", "format": "url"}
+                "items": {"type": "string", "format": "hostname"},
             },
+            "urls": {"type": "array", "items": {"type": "string", "format": "url"}},
             "regexes": {
                 "type": "array",
-                "items": {"type": "string", "format": "regex"}
+                "items": {"type": "string", "format": "regex"},
             },
         },
     }
     data_tests = [
         DataTest(
-            name='datetime. valid',
-            data={'datetimes': [
-                "2013-03-25T12:42:31+00:32",
-                "2013-03-25T22:04:10.04399Z",
-            ]},
-            valid=True
+            name="datetime. valid",
+            data={
+                "datetimes": ["2013-03-25T12:42:31+00:32", "2013-03-25T22:04:10.04399Z"]
+            },
+            valid=True,
         ),
         DataTest(
-            name='datetime. invalid',
-            data={'datetimes': [
-                "2015-05-13 13:35:15.718978",
-                "2015-05-13 13:35:15",
-                "13-05-2013",
-            ]},
+            name="datetime. invalid",
+            data={
+                "datetimes": [
+                    "2015-05-13 13:35:15.718978",
+                    "2015-05-13 13:35:15",
+                    "13-05-2013",
+                ]
+            },
             valid=False,
             expected_errors={
-                'datetimes.0': [messages.INVALID_DATETIME],
-                'datetimes.1': [messages.INVALID_DATETIME],
-                'datetimes.2': [messages.INVALID_DATETIME],
-            }
+                "datetimes.0": [messages.INVALID_DATETIME],
+                "datetimes.1": [messages.INVALID_DATETIME],
+                "datetimes.2": [messages.INVALID_DATETIME],
+            },
         ),
         DataTest(
-            name='email. valid',
-            data={'emails': [
-                'johndoe@domain.com',
-                'john.doe@domain.com',
-                'john.doe@sub.domain.com',
-                'j@sub.domain.com',
-                'j@d.com',
-                'j@domain.co.uk',
-            ]},
-            valid=True
-        ),
-        DataTest(
-            name='email. invalid',
-            data={'emails': [
-                '',
-                'johndoe',
-                'johndoe@domain',
-                'johndoe@domain.',
-                '@domain',
-                '@domain.com',
-                'domain.com',
-            ]},
-            valid=False,
-            expected_errors={
-                'emails.0': [messages.INVALID_EMAIL],
-                'emails.1': [messages.INVALID_EMAIL],
-                'emails.2': [messages.INVALID_EMAIL],
-                'emails.3': [messages.INVALID_EMAIL],
-                'emails.4': [messages.INVALID_EMAIL],
-                'emails.5': [messages.INVALID_EMAIL],
-                'emails.6': [messages.INVALID_EMAIL],
-            }
+            name="email. valid",
+            data={
+                "emails": [
+                    "johndoe@domain.com",
+                    "john.doe@domain.com",
+                    "john.doe@sub.domain.com",
+                    "j@sub.domain.com",
+                    "j@d.com",
+                    "j@domain.co.uk",
+                ]
+            },
+            valid=True,
         ),
         DataTest(
-            name='ipv4. valid',
-            data={'ipv4s': [
-                '98.139.180.149',
-                '69.89.31.226',
-                '192.168.1.1',
-                '127.0.0.0',
-                '0.0.0.0',
-                '255.255.255.255',
-            ]},
-            valid=True
-        ),
-        DataTest(
-            name='ipv4. invalid',
-            data={'ipv4s': [
-                '',
-                '0',
-                '0.',
-                '0.0',
-                '0.0.',
-                '0.0.0',
-                '0.0.0.0.',
-                '0.0.0.0.0',
-                '256.256.256.256',
-                '2002:4559:1FE2::4559:1FE2',
-                '2002:4559:1FE2:0:0:0:4559:1FE2',
-                '2002:4559:1FE2:0000:0000:0000:4559:1FE2',
-            ]},
+            name="email. invalid",
+            data={
+                "emails": [
+                    "",
+                    "johndoe",
+                    "johndoe@domain",
+                    "johndoe@domain.",
+                    "@domain",
+                    "@domain.com",
+                    "domain.com",
+                ]
+            },
             valid=False,
             expected_errors={
-                'ipv4s.0': [messages.INVALID_IPV4],
-                'ipv4s.1': [messages.INVALID_IPV4],
-                'ipv4s.2': [messages.INVALID_IPV4],
-                'ipv4s.3': [messages.INVALID_IPV4],
-                'ipv4s.4': [messages.INVALID_IPV4],
-                'ipv4s.5': [messages.INVALID_IPV4],
-                'ipv4s.6': [messages.INVALID_IPV4],
-                'ipv4s.7': [messages.INVALID_IPV4],
-                'ipv4s.8': [messages.INVALID_IPV4],
-                'ipv4s.9': [messages.INVALID_IPV4],
-                'ipv4s.10': [messages.INVALID_IPV4],
-                'ipv4s.11': [messages.INVALID_IPV4],
-            }
+                "emails.0": [messages.INVALID_EMAIL],
+                "emails.1": [messages.INVALID_EMAIL],
+                "emails.2": [messages.INVALID_EMAIL],
+                "emails.3": [messages.INVALID_EMAIL],
+                "emails.4": [messages.INVALID_EMAIL],
+                "emails.5": [messages.INVALID_EMAIL],
+                "emails.6": [messages.INVALID_EMAIL],
+            },
         ),
         DataTest(
-            name='ipv6. valid',
-            data={'ipv6s': [
-                '2002:4559:1FE2::4559:1FE2',
-                '2002:4559:1FE2:0:0:0:4559:1FE2',
-                '2002:4559:1FE2:0000:0000:0000:4559:1FE2',
-            ]},
-            valid=True
-        ),
-        DataTest(
-            name='ipv6. invalid',
-            data={'ipv6s': [
-                '',
-                '98.139.180.149',
-                '69.89.31.226',
-                '192.168.1.1',
-                '127.0.0.0',
-                '0.0.0.0',
-                '255.255.255.255',
-            ]},
+            name="ipv4. valid",
+            data={
+                "ipv4s": [
+                    "98.139.180.149",
+                    "69.89.31.226",
+                    "192.168.1.1",
+                    "127.0.0.0",
+                    "0.0.0.0",
+                    "255.255.255.255",
+                ]
+            },
+            valid=True,
+        ),
+        DataTest(
+            name="ipv4. invalid",
+            data={
+                "ipv4s": [
+                    "",
+                    "0",
+                    "0.",
+                    "0.0",
+                    "0.0.",
+                    "0.0.0",
+                    "0.0.0.0.",
+                    "0.0.0.0.0",
+                    "256.256.256.256",
+                    "2002:4559:1FE2::4559:1FE2",
+                    "2002:4559:1FE2:0:0:0:4559:1FE2",
+                    "2002:4559:1FE2:0000:0000:0000:4559:1FE2",
+                ]
+            },
             valid=False,
             expected_errors={
-                'ipv6s.0': [messages.INVALID_IPV6],
-                'ipv6s.1': [messages.INVALID_IPV6],
-                'ipv6s.2': [messages.INVALID_IPV6],
-                'ipv6s.3': [messages.INVALID_IPV6],
-                'ipv6s.4': [messages.INVALID_IPV6],
-                'ipv6s.5': [messages.INVALID_IPV6],
-                'ipv6s.6': [messages.INVALID_IPV6],
-            }
+                "ipv4s.0": [messages.INVALID_IPV4],
+                "ipv4s.1": [messages.INVALID_IPV4],
+                "ipv4s.2": [messages.INVALID_IPV4],
+                "ipv4s.3": [messages.INVALID_IPV4],
+                "ipv4s.4": [messages.INVALID_IPV4],
+                "ipv4s.5": [messages.INVALID_IPV4],
+                "ipv4s.6": [messages.INVALID_IPV4],
+                "ipv4s.7": [messages.INVALID_IPV4],
+                "ipv4s.8": [messages.INVALID_IPV4],
+                "ipv4s.9": [messages.INVALID_IPV4],
+                "ipv4s.10": [messages.INVALID_IPV4],
+                "ipv4s.11": [messages.INVALID_IPV4],
+            },
         ),
         DataTest(
-            name='hostname. valid',
-            data={'hostnames': [
-                'localhost',
-                'google',
-                'google.com',
-                'xn--hxajbheg2az3al.xn--jxalpdlp',
-                'a'*63,
-            ]},
+            name="ipv6. valid",
+            data={
+                "ipv6s": [
+                    "2002:4559:1FE2::4559:1FE2",
+                    "2002:4559:1FE2:0:0:0:4559:1FE2",
+                    "2002:4559:1FE2:0000:0000:0000:4559:1FE2",
+                ]
+            },
             valid=True,
         ),
         DataTest(
-            name='hostname. invalid',
-            data={'hostnames': [
-                '...',
-                'a'*64,
-                '-hi-',
-                '_hi_',
-                '*hi*',
-            ]},
+            name="ipv6. invalid",
+            data={
+                "ipv6s": [
+                    "",
+                    "98.139.180.149",
+                    "69.89.31.226",
+                    "192.168.1.1",
+                    "127.0.0.0",
+                    "0.0.0.0",
+                    "255.255.255.255",
+                ]
+            },
             valid=False,
             expected_errors={
-                'hostnames.0': [messages.INVALID_HOSTNAME],
-                'hostnames.1': [messages.INVALID_HOSTNAME],
-                'hostnames.2': [messages.INVALID_HOSTNAME],
-                'hostnames.3': [messages.INVALID_HOSTNAME],
-                'hostnames.4': [messages.INVALID_HOSTNAME],
-            }
+                "ipv6s.0": [messages.INVALID_IPV6],
+                "ipv6s.1": [messages.INVALID_IPV6],
+                "ipv6s.2": [messages.INVALID_IPV6],
+                "ipv6s.3": [messages.INVALID_IPV6],
+                "ipv6s.4": [messages.INVALID_IPV6],
+                "ipv6s.5": [messages.INVALID_IPV6],
+                "ipv6s.6": [messages.INVALID_IPV6],
+            },
         ),
         DataTest(
-            name='urls. valid',
-            data={'urls': [
-                'http://www.domain',
-                'http://www.com',
-                'http://www.domain.com.',
-                'http://www.domain.com/.',
-                'http://www.domain.com/..',
-                'http://www.domain.com//cataglog//index.html',
-                'http://www.domain.net/',
-                'http://www.domain.com/level2/leafnode-L2.xhtml/',
-                'http://www.domain.com/level2/level3/leafnode-L3.xhtml/',
-                'http://www.domain.com?pageid=123&testid=1524',
-                'http://www.domain.com/do.html#A',
-            ]},
+            name="hostname. valid",
+            data={
+                "hostnames": [
+                    "localhost",
+                    "google",
+                    "google.com",
+                    "xn--hxajbheg2az3al.xn--jxalpdlp",
+                    "a" * 63,
+                ]
+            },
             valid=True,
         ),
         DataTest(
-            name='urls. invalid',
-            data={'urls': [
-                '',
-                'http://',
-                'http://www.',
-                'www.',
-                'http://www. .com',
-                'domain.com',
-                'www.domain.com',
-                'http:/www.domain.com',
-                'http//www.domain.com',
-                'http:www.domain.com',
-                'htp://domain.com/',
-                'http://sub.domain.com\\en-us\\default.aspx\\',
-                'http:\\\\msdn.domain.com\\en-us\\library\\default.aspx\\',
-                'http:\\\\www.domain.com\\leafnode-L1.html',
-                './',
-                '../',
-                'http:\\\\www.domain.com\\leafnode-L1.xhtml\\',
-            ]},
+            name="hostname. invalid",
+            data={"hostnames": ["...", "a" * 64, "-hi-", "_hi_", "*hi*"]},
             valid=False,
             expected_errors={
-                'urls.0': [messages.INVALID_URL],
-                'urls.1': [messages.INVALID_URL],
-                'urls.2': [messages.INVALID_URL],
-                'urls.3': [messages.INVALID_URL],
-                'urls.4': [messages.INVALID_URL],
-                'urls.5': [messages.INVALID_URL],
-                'urls.6': [messages.INVALID_URL],
-                'urls.7': [messages.INVALID_URL],
-                'urls.8': [messages.INVALID_URL],
-                'urls.9': [messages.INVALID_URL],
-                'urls.10': [messages.INVALID_URL],
-                'urls.11': [messages.INVALID_URL],
-                'urls.12': [messages.INVALID_URL],
-                'urls.13': [messages.INVALID_URL],
-                'urls.14': [messages.INVALID_URL],
-                'urls.15': [messages.INVALID_URL],
-                'urls.16': [messages.INVALID_URL],
-            }
+                "hostnames.0": [messages.INVALID_HOSTNAME],
+                "hostnames.1": [messages.INVALID_HOSTNAME],
+                "hostnames.2": [messages.INVALID_HOSTNAME],
+                "hostnames.3": [messages.INVALID_HOSTNAME],
+                "hostnames.4": [messages.INVALID_HOSTNAME],
+            },
         ),
         DataTest(
-            name='regexes. valid',
-            data={'regexes': [
-                '[0-9]+',
-            ]},
+            name="urls. valid",
+            data={
+                "urls": [
+                    "http://www.domain",
+                    "http://www.com",
+                    "http://www.domain.com.",
+                    "http://www.domain.com/.",
+                    "http://www.domain.com/..",
+                    "http://www.domain.com//cataglog//index.html",
+                    "http://www.domain.net/",
+                    "http://www.domain.com/level2/leafnode-L2.xhtml/",
+                    "http://www.domain.com/level2/level3/leafnode-L3.xhtml/",
+                    "http://www.domain.com?pageid=123&testid=1524",
+                    "http://www.domain.com/do.html#A",
+                ]
+            },
             valid=True,
         ),
         DataTest(
-            name='regexes. invalid',
-            data={'regexes': [
-                '[0-9]++',
-            ]},
+            name="urls. invalid",
+            data={
+                "urls": [
+                    "",
+                    "http://",
+                    "http://www.",
+                    "www.",
+                    "http://www. .com",
+                    "domain.com",
+                    "www.domain.com",
+                    "http:/www.domain.com",
+                    "http//www.domain.com",
+                    "http:www.domain.com",
+                    "htp://domain.com/",
+                    "http://sub.domain.com\\en-us\\default.aspx\\",
+                    "http:\\\\msdn.domain.com\\en-us\\library\\default.aspx\\",
+                    "http:\\\\www.domain.com\\leafnode-L1.html",
+                    "./",
+                    "../",
+                    "http:\\\\www.domain.com\\leafnode-L1.xhtml\\",
+                ]
+            },
             valid=False,
             expected_errors={
-                'regexes.0': [messages.INVALID_REGEX],
-            }
+                "urls.0": [messages.INVALID_URL],
+                "urls.1": [messages.INVALID_URL],
+                "urls.2": [messages.INVALID_URL],
+                "urls.3": [messages.INVALID_URL],
+                "urls.4": [messages.INVALID_URL],
+                "urls.5": [messages.INVALID_URL],
+                "urls.6": [messages.INVALID_URL],
+                "urls.7": [messages.INVALID_URL],
+                "urls.8": [messages.INVALID_URL],
+                "urls.9": [messages.INVALID_URL],
+                "urls.10": [messages.INVALID_URL],
+                "urls.11": [messages.INVALID_URL],
+                "urls.12": [messages.INVALID_URL],
+                "urls.13": [messages.INVALID_URL],
+                "urls.14": [messages.INVALID_URL],
+                "urls.15": [messages.INVALID_URL],
+                "urls.16": [messages.INVALID_URL],
+            },
+        ),
+        DataTest(name="regexes. valid", data={"regexes": ["[0-9]+"]}, valid=True),
+        DataTest(
+            name="regexes. invalid",
+            data={"regexes": ["[0-9]++"]},
+            valid=False,
+            expected_errors={"regexes.0": [messages.INVALID_REGEX]},
         ),
     ]
 
 
 class Items(SchemaTest):
-    schema_items = {
-        "items": {"type": "integer"},
-    }
-    schema_array = {
-        "items": [
-            {"type": "integer"},
-            {"type": "string"}
-        ]
-    }
+    schema_items = {"items": {"type": "integer"}}
+    schema_array = {"items": [{"type": "integer"}, {"type": "string"}]}
     data_tests = [
         DataTest(
-            name='schema_items. valid items',
+            name="schema_items. valid items",
             schema=schema_items,
             data=[1, 2, 3],
             valid=True,
         ),
         DataTest(
-            name='schema_items. wrong type of items',
+            name="schema_items. wrong type of items",
             schema=schema_items,
-            data=[1, 'x'],
+            data=[1, "x"],
             valid=False,
-            expected_errors={
-                '1': [messages.INVALID_INT],
-            }
+            expected_errors={"1": [messages.INVALID_INT]},
         ),
         DataTest(
-            name='schema_items. ignores non-arrays',
+            name="schema_items. ignores non-arrays",
             schema=schema_items,
             data={"foo": "bar"},
             valid=True,
         ),
         DataTest(
-            name='schema_array. correct types',
+            name="schema_array. correct types",
             schema=schema_array,
             data=[1, "foo"],
             valid=True,
         ),
         DataTest(
-            name='schema_array. wrong types',
+            name="schema_array. wrong types",
             schema=schema_array,
             data=["foo", 1],
             valid=False,
             expected_errors={
-                '0': [messages.INVALID_INT],
-                '1': [messages.INVALID_STRING],
-            }
+                "0": [messages.INVALID_INT],
+                "1": [messages.INVALID_STRING],
+            },
         ),
     ]
 
 
 class MaxItems(SchemaTest):
-    schema = {
-        "maxItems": 2
-    }
+    schema = {"maxItems": 2}
     data_tests = [
+        DataTest(name="shorter is valid", data=[1], valid=True),
+        DataTest(name="exact length is valid", data=[1, 2], valid=True),
         DataTest(
-            name='shorter is valid',
-            data=[1],
-            valid=True,
-        ),
-        DataTest(
-            name='exact length is valid',
-            data=[1, 2],
-            valid=True,
-        ),
-        DataTest(
-            name='too long is invalid',
+            name="too long is invalid",
             data=[1, 2, 3],
             valid=False,
-            expected_errors={
-                '': [messages.FIELD_TOO_LONG],
-            }
-        ),
-        DataTest(
-            name='ignores non-arrays',
-            data="foobar",
-            valid=True,
+            expected_errors={"": [messages.FIELD_TOO_LONG]},
         ),
+        DataTest(name="ignores non-arrays", data="foobar", valid=True),
     ]
 
 
 class MaxLength(SchemaTest):
-    schema = {
-        "maxLength": 2
-    }
+    schema = {"maxLength": 2}
     data_tests = [
+        DataTest(name="shorter is valid", data="f", valid=True),
+        DataTest(name="exact length is valid", data="fo", valid=True),
         DataTest(
-            name='shorter is valid',
-            data='f',
-            valid=True,
-        ),
-        DataTest(
-            name='exact length is valid',
-            data='fo',
-            valid=True,
-        ),
-        DataTest(
-            name='too long is invalid',
-            data='foo',
+            name="too long is invalid",
+            data="foo",
             valid=False,
-            expected_errors={
-                '': [messages.FIELD_TOO_LONG],
-            }
-        ),
-        DataTest(
-            name='ignores non-strings',
-            data=100,
-            valid=True,
+            expected_errors={"": [messages.FIELD_TOO_LONG]},
         ),
+        DataTest(name="ignores non-strings", data=100, valid=True),
     ]
 
 
 class MaxProperties(SchemaTest):
-    schema = {
-        "maxProperties": 2
-    }
+    schema = {"maxProperties": 2}
     data_tests = [
+        DataTest(name="shorter is valid", data={"foo": 1}, valid=True),
+        DataTest(name="exact length is valid", data={"foo": 1, "bar": 2}, valid=True),
         DataTest(
-            name='shorter is valid',
-            data={"foo": 1},
-            valid=True,
-        ),
-        DataTest(
-            name='exact length is valid',
-            data={"foo": 1, "bar": 2},
-            valid=True,
-        ),
-        DataTest(
-            name='too long is invalid',
+            name="too long is invalid",
             data={"foo": 1, "bar": 2, "baz": 3},
             valid=False,
-            expected_errors={
-                '': [messages.TOO_MANY_PROPERTIES],
-            }
-        ),
-        DataTest(
-            name='ignores non-objects',
-            data='foobar',
-            valid=True,
+            expected_errors={"": [messages.TOO_MANY_PROPERTIES]},
         ),
+        DataTest(name="ignores non-objects", data="foobar", valid=True),
     ]
 
 
 class Maximum(SchemaTest):
-    schema = {
-        "maximum": 3.0,
-    }
-    schema_exclusive = {
+    # exclusiveMaximum behaviour changed from draft-04 to draft-06
+    # http://json-schema.org/draft-06/json-schema-release-notes.html#backwards-incompatible-changes
+    schema = {"maximum": 3.0}
+    draft4_schema_exclusive = {
+        "$schema": "http://json-schema.org/draft-04/schema",
         "maximum": 3.0,
         "exclusiveMaximum": True,
     }
+    draft6_schema_exclusive = {
+        "$schema": "http://json-schema.org/draft-06/schema",
+        "exclusiveMaximum": 3.0,
+    }
+
     data_tests = [
+        DataTest(name="below", data=2.6, valid=True),
         DataTest(
-            name='below',
-            data=2.6,
+            name="above",
+            data=3.5,
+            valid=False,
+            expected_errors={"": [messages.NUMBER_TOO_HIGH]},
+        ),
+        DataTest(
+            name="ignores non-numbers", data={"foo": 1, "bar": 2, "baz": 3}, valid=True
+        ),
+        DataTest(
+            name="draft4 exclusive. below",
+            schema=draft4_schema_exclusive,
+            data=2.2,
             valid=True,
         ),
         DataTest(
-            name='above',
-            data=3.5,
+            name="draft4_exclusive. boundary point",
+            schema=draft4_schema_exclusive,
+            data=3.0,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_HIGH],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_HIGH]},
         ),
         DataTest(
-            name='ignores non-numbers',
-            data={"foo": 1, "bar": 2, "baz": 3},
-            valid=True,
+            name="draft4_exclusive. above",
+            schema=draft4_schema_exclusive,
+            data=3.5,
+            valid=False,
+            expected_errors={"": [messages.NUMBER_TOO_HIGH]},
         ),
         DataTest(
-            name='exclusive. below',
-            schema=schema_exclusive,
+            name="draft6 exclusive. below",
+            schema=draft6_schema_exclusive,
             data=2.2,
             valid=True,
         ),
         DataTest(
-            name='exclusive. boundary point',
-            schema=schema_exclusive,
+            name="draft6_exclusive. boundary point",
+            schema=draft6_schema_exclusive,
             data=3.0,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_HIGH],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_HIGH]},
         ),
         DataTest(
-            name='exclusive. above',
-            schema=schema_exclusive,
+            name="draft6_exclusive. above",
+            schema=draft6_schema_exclusive,
             data=3.5,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_HIGH],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_HIGH]},
         ),
     ]
 
 
 class MinItems(SchemaTest):
-    schema = {
-        "minItems": 1,
-    }
+    schema = {"minItems": 1}
     data_tests = [
+        DataTest(name="longer is valid", data=[1, 2], valid=True),
+        DataTest(name="exact length is valid", data=[1], valid=True),
         DataTest(
-            name='longer is valid',
-            data=[1, 2],
-            valid=True,
-        ),
-        DataTest(
-            name='exact length is valid',
-            data=[1],
-            valid=True,
-        ),
-        DataTest(
-            name='too short is invalid',
+            name="too short is invalid",
             data=[],
             valid=False,
-            expected_errors={
-                '': [messages.FIELD_TOO_SHORT],
-            }
-        ),
-        DataTest(
-            name='ignores non-arrays',
-            data="",
-            valid=True,
+            expected_errors={"": [messages.FIELD_TOO_SHORT]},
         ),
+        DataTest(name="ignores non-arrays", data="", valid=True),
     ]
 
 
 class MinProperties(SchemaTest):
-    schema = {
-        "minProperties": 1,
-    }
+    schema = {"minProperties": 1}
     data_tests = [
+        DataTest(name="longer is valid", data={"foo": 1, "bar": 2}, valid=True),
+        DataTest(name="exact length is valid", data={"foo": 1}, valid=True),
         DataTest(
-            name='longer is valid',
-            data={"foo": 1, "bar": 2},
-            valid=True,
-        ),
-        DataTest(
-            name='exact length is valid',
-            data={"foo": 1},
-            valid=True,
-        ),
-        DataTest(
-            name='too short is invalid',
+            name="too short is invalid",
             data={},
             valid=False,
-            expected_errors={
-                '': [messages.NOT_ENOUGH_PROPERTIES],
-            }
-        ),
-        DataTest(
-            name='ignores non-objects',
-            data='',
-            valid=True,
+            expected_errors={"": [messages.NOT_ENOUGH_PROPERTIES]},
         ),
+        DataTest(name="ignores non-objects", data="", valid=True),
     ]
 
 
 class Minimum(SchemaTest):
-    schema = {
-        "minimum": 1.1,
-    }
-    schema_exclusive = {
+    # exclusiveMinimum behaviour changed from draft-04 to draft-06
+    # http://json-schema.org/draft-06/json-schema-release-notes.html#backwards-incompatible-changes
+    schema = {"minimum": 1.1}
+    draft4_schema_exclusive = {
+        "$schema": "http://json-schema.org/draft-04/schema",
         "minimum": 1.1,
         "exclusiveMinimum": True,
     }
+    draft6_schema_exclusive = {
+        "$schema": "http://json-schema.org/draft-06/schema",
+        "exclusiveMinimum": 1.1,
+    }
+
     data_tests = [
+        DataTest(name="above", data=2.6, valid=True),
         DataTest(
-            name='above',
-            data=2.6,
-            valid=True,
-        ),
-        DataTest(
-            name='below',
+            name="below",
             data=0.6,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_LOW],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_LOW]},
         ),
+        DataTest(name="ignores non-numbers", data="x", valid=True),
         DataTest(
-            name='ignores non-numbers',
-            data='x',
+            name="exclusive. above",
+            schema=draft4_schema_exclusive,
+            data=1.2,
             valid=True,
         ),
         DataTest(
-            name='exclusive. above',
-            schema=schema_exclusive,
+            name="exclusive. above",
+            schema=draft6_schema_exclusive,
             data=1.2,
             valid=True,
         ),
         DataTest(
-            name='exclusive. boundary point',
-            schema=schema_exclusive,
+            name="draft4 exclusive. boundary point",
+            schema=draft4_schema_exclusive,
             data=1.1,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_LOW],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_LOW]},
+        ),
+        DataTest(
+            name="draft6 exclusive. boundary point",
+            schema=draft6_schema_exclusive,
+            data=1.1,
+            valid=False,
+            expected_errors={"": [messages.NUMBER_TOO_LOW]},
         ),
         DataTest(
-            name='exclusive. below',
-            schema=schema_exclusive,
+            name="draft4 exclusive. below",
+            schema=draft4_schema_exclusive,
             data=0.6,
             valid=False,
-            expected_errors={
-                '': [messages.NUMBER_TOO_LOW],
-            }
+            expected_errors={"": [messages.NUMBER_TOO_LOW]},
+        ),
+        DataTest(
+            name="draft6 exclusive. below",
+            schema=draft6_schema_exclusive,
+            data=0.6,
+            valid=False,
+            expected_errors={"": [messages.NUMBER_TOO_LOW]},
         ),
     ]
 
 
 class MultipleOf(SchemaTest):
-    schema_int = {
-        "multipleOf": 2,
-    }
-    schema_number = {
-        "multipleOf": 1.5,
-    }
-    schema_small_number = {
-        "multipleOf": 0.0001,
-    }
+    schema_int = {"multipleOf": 2}
+    schema_number = {"multipleOf": 1.5}
+    schema_small_number = {"multipleOf": 0.0001}
     data_tests = [
+        DataTest(name="int. valid", schema=schema_int, data=10, valid=True),
+        DataTest(name="int. valid float", schema=schema_int, data=10.0, valid=True),
         DataTest(
-            name='int. valid',
-            schema=schema_int,
-            data=10,
-            valid=True,
-        ),
-        DataTest(
-            name='int. valid float',
-            schema=schema_int,
-            data=10.0,
-            valid=True,
-        ),
-        DataTest(
-            name='int. invalid',
+            name="int. invalid",
             schema=schema_int,
             data=7,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_MULTIPLE_OF],
-            }
+            expected_errors={"": [messages.NOT_MULTIPLE_OF]},
         ),
+        DataTest(name="int. ignores non-numbers", data="x", valid=True),
         DataTest(
-            name='int. ignores non-numbers',
-            data='x',
-            valid=True,
-        ),
-        DataTest(
-            name='number. zero is multiple of anything',
+            name="number. zero is multiple of anything",
             schema=schema_number,
             data=0,
             valid=True,
         ),
+        DataTest(name="number. valid", schema=schema_number, data=4.5, valid=True),
         DataTest(
-            name='number. valid',
-            schema=schema_number,
-            data=4.5,
-            valid=True,
-        ),
-        DataTest(
-            name='number. invalid',
+            name="number. invalid",
             schema=schema_number,
             data=35,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_MULTIPLE_OF],
-            }
+            expected_errors={"": [messages.NOT_MULTIPLE_OF]},
         ),
         DataTest(
-            name='small number. valid',
+            name="small number. valid",
             schema=schema_small_number,
             data=0.0075,
             valid=True,
         ),
         DataTest(
-            name='small number. invalid',
+            name="small number. invalid",
             schema=schema_small_number,
             data=0.00751,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_MULTIPLE_OF],
-            }
+            expected_errors={"": [messages.NOT_MULTIPLE_OF]},
         ),
-
     ]
 
 
 class Not(SchemaTest):
-    schema_not = {
-        "not": {"type": "integer"},
-    }
-    schema_multiple = {
-        "not": {"type": ["integer", "boolean"]},
-    }
+    schema_not = {"not": {"type": "integer"}}
+    schema_multiple = {"not": {"type": ["integer", "boolean"]}}
     schema_complex = {
-        "not": {
-            "type": "object",
-            "properties": {
-                "foo": {"type": "string"},
-            },
-        },
-    }
-    schema_forbidden = {
-        "properties": {
-            "foo": {
-                "not": {},
-            },
-        },
+        "not": {"type": "object", "properties": {"foo": {"type": "string"}}}
     }
+    schema_forbidden = {"properties": {"foo": {"not": {}}}}
     data_tests = [
+        DataTest(name="not. allowed", schema=schema_not, data="foo", valid=True),
         DataTest(
-            name='not. allowed',
-            schema=schema_not,
-            data='foo',
-            valid=True,
-        ),
-        DataTest(
-            name='not. disallowed',
+            name="not. disallowed",
             schema=schema_not,
             data=1,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_ALLOWED_VALUE],
-            }
+            expected_errors={"": [messages.NOT_ALLOWED_VALUE]},
         ),
         DataTest(
-            name='multiple. allowed',
-            schema=schema_multiple,
-            data='foo',
-            valid=True,
+            name="multiple. allowed", schema=schema_multiple, data="foo", valid=True
         ),
         DataTest(
-            name='multiple. mismatch',
+            name="multiple. mismatch",
             schema=schema_multiple,
             data=1,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_ALLOWED_VALUE],
-            }
+            expected_errors={"": [messages.NOT_ALLOWED_VALUE]},
         ),
         DataTest(
-            name='multiple. other mismatch',
+            name="multiple. other mismatch",
             schema=schema_multiple,
             data=True,
             valid=False,
-            expected_errors={
-                '': [messages.NOT_ALLOWED_VALUE],
-            }
+            expected_errors={"": [messages.NOT_ALLOWED_VALUE]},
         ),
+        DataTest(name="complex. match", schema=schema_complex, data=1, valid=True),
         DataTest(
-            name='complex. match',
-            schema=schema_complex,
-            data=1,
-            valid=True,
-        ),
-        DataTest(
-            name='complex. other match',
+            name="complex. other match",
             schema=schema_complex,
             data={"foo": 1},
             valid=True,
         ),
         DataTest(
-            name='complex. mismatch',
+            name="complex. mismatch",
             schema=schema_complex,
             data={"foo": "bar"},
             valid=False,
-            expected_errors={
-                '': [messages.NOT_ALLOWED_VALUE],
-            }
+            expected_errors={"": [messages.NOT_ALLOWED_VALUE]},
         ),
         DataTest(
-            name='forbidden. present',
+            name="forbidden. present",
             schema=schema_forbidden,
             data={"foo": 1, "bar": 2},
             valid=False,
-            expected_errors={
-                'foo': [messages.NOT_ALLOWED_VALUE],
-            }
+            expected_errors={"foo": [messages.NOT_ALLOWED_VALUE]},
         ),
         DataTest(
-            name='forbidden. absent',
+            name="forbidden. absent",
             schema=schema_forbidden,
             data={"bar": 1, "baz": 2},
             valid=True,
         ),
     ]
 
 
 class OneOf(SchemaTest):
     schema = {
         "type": "object",
-        "properties": {
-            "A": {"type": "boolean"},
-            "B": {"type": "boolean"}
-        },
-        "oneOf": [
-            {"required": ["A"]},
-            {"required": ["B"]}
-        ]
+        "properties": {"A": {"type": "boolean"}, "B": {"type": "boolean"}},
+        "oneOf": [{"required": ["A"]}, {"required": ["B"]}],
     }
     data_tests = [
         DataTest(
             name="Empty object",
             data={},
             valid=False,
-            expected_errors={
-                '': [messages.NOT_VALID_UNDER_ANY_SCHEMA],
-            }
-        ),
-        DataTest(
-            name="Mismatch B",
-            data={"A": True},
-            valid=True,
-        ),
-        DataTest(
-            name="Mismatch A",
-            data={"B": True},
-            valid=True,
+            expected_errors={"": [messages.NOT_VALID_UNDER_ANY_SCHEMA]},
         ),
+        DataTest(name="Mismatch B", data={"A": True}, valid=True),
+        DataTest(name="Mismatch A", data={"B": True}, valid=True),
         DataTest(
             name="Both values",
             data={"A": False, "B": False},
             valid=False,
-            expected_errors={
-                '': [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS],
-            }
+            expected_errors={"": [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS]},
         ),
         DataTest(
             name="Wrong type for A",
             data={"A": 1, "B": False},
             valid=False,
             expected_errors={
-                '': [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS],
-                'A': [messages.INVALID_BOOLEAN],
-            }
+                "": [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS],
+                "A": [messages.INVALID_BOOLEAN],
+            },
         ),
         DataTest(
             name="Wrong type for both",
             data={"A": 1, "B": 1},
             valid=False,
             expected_errors={
-                '': [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS],
-                'A': [messages.INVALID_BOOLEAN],
-                'B': [messages.INVALID_BOOLEAN],
-            }
+                "": [messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS],
+                "A": [messages.INVALID_BOOLEAN],
+                "B": [messages.INVALID_BOOLEAN],
+            },
         ),
     ]
 
 
 class Pattern(SchemaTest):
-    schema = {
-        "pattern": "^a*$",
-    }
+    schema = {"pattern": "^a*$"}
     data_tests = [
-        DataTest(
-            name="valid",
-            data='aaa',
-            valid=True,
-        ),
+        DataTest(name="valid", data="aaa", valid=True),
         DataTest(
             name="invalid",
-            data='abc',
+            data="abc",
             valid=False,
-            expected_errors={
-                '': [messages.REGEX_NOT_MATCHED],
-            }
-        ),
-        DataTest(
-            name="ignores non-strings",
-            data=True,
-            valid=True,
+            expected_errors={"": [messages.REGEX_NOT_MATCHED]},
         ),
+        DataTest(name="ignores non-strings", data=True, valid=True),
     ]
 
 
 class PatternProperties(SchemaTest):
-    schema_single = {
-        "patternProperties": {
-            "f.*o": {"type": "integer"},
-        },
-    }
+    schema_single = {"patternProperties": {"f.*o": {"type": "integer"}}}
     schema_multiple = {
-        "patternProperties": {
-            "a*": {"type": "integer"},
-            "aaa*": {"maximum": 20},
-        },
+        "patternProperties": {"a*": {"type": "integer"}, "aaa*": {"maximum": 20}}
     }
     schema_complex = {
         "patternProperties": {
             "[0-9]{2,}": {"type": "boolean"},
             "X_": {"type": "string"},
-        },
+        }
     }
     data_tests = [
         DataTest(
-            name="single. valid",
-            schema=schema_single,
-            data={"foo": 1},
-            valid=True,
+            name="single. valid", schema=schema_single, data={"foo": 1}, valid=True
         ),
         DataTest(
             name="single. multiple valid",
             schema=schema_single,
             data={"foo": 1, "foooooo": 2},
             valid=True,
         ),
         DataTest(
             name="single. invalid",
             schema=schema_single,
             data={"foo": "bar", "fooooo": 2},
             valid=False,
-            expected_errors={
-                'foo': [messages.INVALID_INT],
-            }
+            expected_errors={"foo": [messages.INVALID_INT]},
         ),
         DataTest(
             name="single. multiple invalid",
             schema=schema_single,
             data={"foo": "bar", "foooooo": "baz"},
             valid=False,
             expected_errors={
-                'foo': [messages.INVALID_INT],
-                'foooooo': [messages.INVALID_INT],
-            }
+                "foo": [messages.INVALID_INT],
+                "foooooo": [messages.INVALID_INT],
+            },
         ),
         DataTest(
             name="single. ignores non-objects",
             schema=schema_single,
             data=12,
             valid=True,
         ),
         DataTest(
-            name="multiple. valid",
-            schema=schema_multiple,
-            data={"a": 21},
-            valid=True,
+            name="multiple. valid", schema=schema_multiple, data={"a": 21}, valid=True
         ),
         DataTest(
             name="multiple. simultaneous valid",
             schema=schema_multiple,
             data={"aaaa": 18},
             valid=True,
         ),
@@ -1516,156 +1213,123 @@
             valid=True,
         ),
         DataTest(
             name="multiple. invalid one",
             schema=schema_multiple,
             data={"a": "bar"},
             valid=False,
-            expected_errors={
-                'a': [messages.INVALID_INT],
-            }
+            expected_errors={"a": [messages.INVALID_INT]},
         ),
         DataTest(
             name="multiple. invalid other",
             schema=schema_multiple,
             data={"aaaa": 31},
             valid=False,
-            expected_errors={
-                'aaaa': [messages.NUMBER_TOO_HIGH],
-            }
+            expected_errors={"aaaa": [messages.NUMBER_TOO_HIGH]},
         ),
         DataTest(
             name="multiple. invalid both",
             schema=schema_multiple,
             data={"aaa": "foo", "aaaa": 31},
             valid=False,
             expected_errors={
-                'aaa': [messages.INVALID_INT],
-                'aaaa': [messages.NUMBER_TOO_HIGH],
-            }
+                "aaa": [messages.INVALID_INT],
+                "aaaa": [messages.NUMBER_TOO_HIGH],
+            },
         ),
         DataTest(
             name="complex. non recognized members are ignored",
             schema=schema_complex,
             data={"answer 1": "42"},
             valid=True,
         ),
         DataTest(
             name="complex. recognized members are accounted for",
             schema=schema_complex,
             data={"a31b": None},
             valid=False,
-            expected_errors={
-                'a31b': [messages.INVALID_BOOLEAN],
-            }
+            expected_errors={"a31b": [messages.INVALID_BOOLEAN]},
         ),
         DataTest(
             name="complex. regexes are case sensitive",
             schema=schema_complex,
-            data={"a_x_3": 3 },
+            data={"a_x_3": 3},
             valid=True,
         ),
         DataTest(
             name="complex. regexes are case sensitive 2",
             schema=schema_complex,
             data={"a_X_3": 3},
             valid=False,
-            expected_errors={
-                'a_X_3': [messages.INVALID_STRING],
-            }
+            expected_errors={"a_X_3": [messages.INVALID_STRING]},
         ),
     ]
 
 
 class Properties(SchemaTest):
-    schema = {
-        "properties": {
-            "foo": {"type": "integer"},
-            "bar": {"type": "string"}
-        }
-    }
+    schema = {"properties": {"foo": {"type": "integer"}, "bar": {"type": "string"}}}
     schema_mixed = {
         "properties": {
             "foo": {"type": "array", "maxItems": 3},
-            "bar": {"type": "array"}
+            "bar": {"type": "array"},
         },
         "patternProperties": {"f.o": {"minItems": 2}},
-        "additionalProperties": {"type": "integer"}
+        "additionalProperties": {"type": "integer"},
     }
     data_tests = [
-        DataTest(
-            name="both present",
-            data={"foo": 1, "bar": "baz"},
-            valid=True,
-        ),
+        DataTest(name="both present", data={"foo": 1, "bar": "baz"}, valid=True),
         DataTest(
             name="one invalid",
             data={"foo": 1, "bar": {}},
             valid=False,
-            expected_errors={
-                'bar': [messages.INVALID_STRING],
-            }
+            expected_errors={"bar": [messages.INVALID_STRING]},
         ),
         DataTest(
             name="both invalid",
             data={"foo": [], "bar": {}},
             valid=False,
             expected_errors={
-                'foo': [messages.INVALID_INT],
-                'bar': [messages.INVALID_STRING],
-            }
-        ),
-        DataTest(
-            name="other properties",
-            data={"quux": []},
-            valid=True,
-        ),
-        DataTest(
-            name="ignores non-objects",
-            data=[],
-            valid=True,
+                "foo": [messages.INVALID_INT],
+                "bar": [messages.INVALID_STRING],
+            },
         ),
+        DataTest(name="other properties", data={"quux": []}, valid=True),
+        DataTest(name="ignores non-objects", data=[], valid=True),
         DataTest(
             name="mixed. property validates property",
             schema=schema_mixed,
             data={"foo": [1, 2]},
             valid=True,
         ),
         DataTest(
             name="mixed. property invalidates property",
             schema=schema_mixed,
             data={"foo": [1, 2, 3, 4]},
             valid=False,
-            expected_errors={
-                'foo': [messages.FIELD_TOO_LONG],
-            }
+            expected_errors={"foo": [messages.FIELD_TOO_LONG]},
         ),
         DataTest(
             name="mixed. patternProperty invalidates property",
             schema=schema_mixed,
             data={"foo": []},
             valid=False,
-            expected_errors={
-                'foo': [messages.FIELD_TOO_SHORT],
-            }
+            expected_errors={"foo": [messages.FIELD_TOO_SHORT]},
         ),
         DataTest(
             name="mixed. patternProperty validates nonproperty",
             schema=schema_mixed,
             data={"fxo": [1, 2]},
             valid=True,
         ),
         DataTest(
             name="mixed. patternProperty invalidates nonproperty",
             schema=schema_mixed,
             data={"fxo": []},
             valid=False,
-            expected_errors={
-                'fxo': [messages.FIELD_TOO_SHORT],
-            }
+            expected_errors={"fxo": [messages.FIELD_TOO_SHORT]},
         ),
         DataTest(
             name="mixed. additionalProperty ignores property",
             schema=schema_mixed,
             data={"bar": []},
             valid=True,
         ),
@@ -1676,388 +1340,279 @@
             valid=True,
         ),
         DataTest(
             name="mixed. additionalProperty invalidates others",
             schema=schema_mixed,
             data={"quux": "foo"},
             valid=False,
-            expected_errors={
-                'quux': [messages.INVALID_INT],
-            }
+            expected_errors={"quux": [messages.INVALID_INT]},
         ),
     ]
 
 
 class Ref(SchemaTest):
-    schema_root = {
-        "properties": {
-            "foo": {"$ref": "#"},
-        },
-        "additionalProperties": False,
-    }
+    schema_root = {"properties": {"foo": {"$ref": "#"}}, "additionalProperties": False}
     schema_relative = {
-        "properties": {
-            "foo": {"type": "integer"},
-            "bar": {"$ref": "#/properties/foo"},
-        },
-    }
-    schema_relative_array = {
-        "items": [
-            {"type": "integer"},
-            {"$ref": "#/items/0"},
-        ],
+        "properties": {"foo": {"type": "integer"}, "bar": {"$ref": "#/properties/foo"}}
     }
+    schema_relative_array = {"items": [{"type": "integer"}, {"$ref": "#/items/0"}]}
     schema_escaped = {
         "tilda~field": {"type": "integer"},
         "slash/field": {"type": "integer"},
         "percent%field": {"type": "integer"},
         "properties": {
             "tilda": {"$ref": "#/tilda~0field"},
             "slash": {"$ref": "#/slash~1field"},
-            "percent": {"$ref": "#/percent%25field"}
-        }
+            "percent": {"$ref": "#/percent%25field"},
+        },
     }
     schema_nested = {
         "definitions": {
             "a": {"type": "integer"},
             "b": {"$ref": "#/definitions/a"},
             "c": {"$ref": "#/definitions/b"},
         },
         "$ref": "#/definitions/c",
     }
     data_tests = [
         DataTest(
-            name="root. match",
-            schema=schema_root,
-            data={"foo": False},
-            valid=True,
+            name="root. match", schema=schema_root, data={"foo": False}, valid=True
         ),
         DataTest(
             name="root. recursive match",
             schema=schema_root,
             data={"foo": {"foo": False}},
             valid=True,
         ),
         DataTest(
             name="root. mismatch",
             schema=schema_root,
             data={"bar": False},
             valid=False,
-            expected_errors={
-                '': [messages.UNEXPECTED_FIELD],
-            }
+            expected_errors={"": [messages.UNEXPECTED_FIELD]},
         ),
         DataTest(
             name="root. recursive mismatch",
             schema=schema_root,
             data={"foo": {"bar": False}},
             valid=False,
-            expected_errors={
-                'foo': [messages.UNEXPECTED_FIELD],
-            }
+            expected_errors={"foo": [messages.UNEXPECTED_FIELD]},
         ),
         DataTest(
-            name="relative. match",
-            schema=schema_relative,
-            data={"bar": 3},
-            valid=True,
+            name="relative. match", schema=schema_relative, data={"bar": 3}, valid=True
         ),
         DataTest(
             name="relative. mismatch",
             schema=schema_relative,
             data={"bar": True},
             valid=False,
-            expected_errors={
-                'bar': [messages.INVALID_INT],
-            }
+            expected_errors={"bar": [messages.INVALID_INT]},
         ),
         DataTest(
             name="relative array. match",
             schema=schema_relative_array,
             data=[1, 2],
             valid=True,
         ),
         DataTest(
             name="relative array. mismatch",
             schema=schema_relative_array,
             data=[1, "foo"],
             valid=False,
-            expected_errors={
-                '1': [messages.INVALID_INT],
-            }
+            expected_errors={"1": [messages.INVALID_INT]},
         ),
         DataTest(
             name="escaped. slash",
             schema=schema_escaped,
             data={"slash": "aoeu"},
             valid=False,
-            expected_errors={
-                'slash': [messages.INVALID_INT],
-            }
+            expected_errors={"slash": [messages.INVALID_INT]},
         ),
         DataTest(
             name="escaped. tilda",
             schema=schema_escaped,
             data={"tilda": "aoeu"},
             valid=False,
-            expected_errors={
-                'tilda': [messages.INVALID_INT],
-            }
+            expected_errors={"tilda": [messages.INVALID_INT]},
         ),
         DataTest(
             name="escaped. percent",
             schema=schema_escaped,
             data={"percent": "aoeu"},
             valid=False,
-            expected_errors={
-                'percent': [messages.INVALID_INT],
-            }
+            expected_errors={"percent": [messages.INVALID_INT]},
         ),
         DataTest(
             name="escaped. all",
             schema=schema_escaped,
-            data={
-                "slash": "aoeu",
-                "tilda": "aoeu",
-                "percent": "aoeu"
-            },
+            data={"slash": "aoeu", "tilda": "aoeu", "percent": "aoeu"},
             valid=False,
             expected_errors={
-                'slash': [messages.INVALID_INT],
-                'tilda': [messages.INVALID_INT],
-                'percent': [messages.INVALID_INT],
-            }
-        ),
-        DataTest(
-            name="nested. valid",
-            schema=schema_nested,
-            data=5,
-            valid=True,
+                "slash": [messages.INVALID_INT],
+                "tilda": [messages.INVALID_INT],
+                "percent": [messages.INVALID_INT],
+            },
         ),
+        DataTest(name="nested. valid", schema=schema_nested, data=5, valid=True),
         DataTest(
             name="nested. invalid",
             schema=schema_nested,
-            data='a',
+            data="a",
             valid=False,
-            expected_errors={
-                '': [messages.INVALID_INT],
-            }
+            expected_errors={"": [messages.INVALID_INT]},
         ),
     ]
 
 
 class Required(SchemaTest):
-    schema = {
-        "properties": {
-            "foo": {},
-            "bar": {}
-        },
-        "required": ["foo"],
-    }
-    schema_default = {
-        "properties": {
-            "foo": {}
-        },
-    }
+    schema = {"properties": {"foo": {}, "bar": {}}, "required": ["foo"]}
+    schema_default = {"properties": {"foo": {}}}
     data_tests = [
-        DataTest(
-            name="valid",
-            data={"foo": 1},
-            valid=True,
-        ),
+        DataTest(name="valid", data={"foo": 1}, valid=True),
         DataTest(
             name="invalid",
             data={"bar": 1},
             valid=False,
-            expected_errors={
-                'foo': [messages.MISSING_REQUIRED_FIELD],
-            }
+            expected_errors={"foo": [messages.MISSING_REQUIRED_FIELD]},
         ),
         DataTest(
-            name="not required by default",
-            schema=schema_default,
-            data={},
-            valid=True,
+            name="not required by default", schema=schema_default, data={}, valid=True
         ),
     ]
 
 
 class Type(SchemaTest):
     type_tests = [
         # -------------------------------------------------------
         # type          data        expected error
         # -------------------------------------------------------
         # array
-        ('array',       [],         None),
-        ('array',       [1, 2],     None),
-        ('array',       None,       messages.INVALID_ARRAY),
-        ('array',       {},         messages.INVALID_ARRAY),
-        ('array',       "[]",       messages.INVALID_ARRAY),
-        ('array',       "abc",      messages.INVALID_ARRAY),
-        ('array',       1,          messages.INVALID_ARRAY),
-
+        ("array", [], None),
+        ("array", [1, 2], None),
+        ("array", None, messages.INVALID_ARRAY),
+        ("array", {}, messages.INVALID_ARRAY),
+        ("array", "[]", messages.INVALID_ARRAY),
+        ("array", "abc", messages.INVALID_ARRAY),
+        ("array", 1, messages.INVALID_ARRAY),
         # boolean
-        ('boolean',     True,       None),
-        ('boolean',     False,      None),
-        ('boolean',     None,       messages.INVALID_BOOLEAN),
-        ('boolean',     "True",     messages.INVALID_BOOLEAN),
-        ('boolean',     "False",    messages.INVALID_BOOLEAN),
-        ('boolean',     0,          messages.INVALID_BOOLEAN),
-        ('boolean',     1,          messages.INVALID_BOOLEAN),
-
+        ("boolean", True, None),
+        ("boolean", False, None),
+        ("boolean", None, messages.INVALID_BOOLEAN),
+        ("boolean", "True", messages.INVALID_BOOLEAN),
+        ("boolean", "False", messages.INVALID_BOOLEAN),
+        ("boolean", 0, messages.INVALID_BOOLEAN),
+        ("boolean", 1, messages.INVALID_BOOLEAN),
         # integer
-        ('integer',     0,          None),
-        ('integer',     1,          None),
-        ('integer',     -500,       None),
-        ('integer',     1000000,    None),
-        ('integer',     None,       messages.INVALID_INT),
-        ('integer',     1.2,        messages.INVALID_INT),
-        ('integer',     "1",        messages.INVALID_INT),
-
+        ("integer", 0, None),
+        ("integer", 1, None),
+        ("integer", -500, None),
+        ("integer", 1000000, None),
+        ("integer", None, messages.INVALID_INT),
+        ("integer", 1.2, messages.INVALID_INT),
+        ("integer", "1", messages.INVALID_INT),
         # number
-        ('number',      0,          None),
-        ('number',      1,          None),
-        ('number',      -500,       None),
-        ('number',      1000000,    None),
-        ('number',      1.2,        None),
-        ('number',      -34.7,      None),
-        ('number',      None,       messages.INVALID_NUMBER),
-        ('number',      "1",        messages.INVALID_NUMBER),
-        ('number',      True,       messages.INVALID_NUMBER),
-
+        ("number", 0, None),
+        ("number", 1, None),
+        ("number", -500, None),
+        ("number", 1000000, None),
+        ("number", 1.2, None),
+        ("number", -34.7, None),
+        ("number", None, messages.INVALID_NUMBER),
+        ("number", "1", messages.INVALID_NUMBER),
+        ("number", True, messages.INVALID_NUMBER),
         # null
-        ('null',        None,       None),
-        ('null',        [],         messages.NOT_NULL),
-        ('null',        {},         messages.NOT_NULL),
-        ('null',        0,          messages.NOT_NULL),
-        ('null',        "",         messages.NOT_NULL),
-
+        ("null", None, None),
+        ("null", [], messages.NOT_NULL),
+        ("null", {}, messages.NOT_NULL),
+        ("null", 0, messages.NOT_NULL),
+        ("null", "", messages.NOT_NULL),
         # object
-        ('object',      {},         None),
-        ('object',      {'a': 1},   None),
-        ('object',      None,       messages.INVALID_OBJECT),
-        ('object',      [],         messages.INVALID_OBJECT),
-        ('object',      0,          messages.INVALID_OBJECT),
-        ('object',      "",         messages.INVALID_OBJECT),
-        ('object',      "abc",      messages.INVALID_OBJECT),
-
+        ("object", {}, None),
+        ("object", {"a": 1}, None),
+        ("object", None, messages.INVALID_OBJECT),
+        ("object", [], messages.INVALID_OBJECT),
+        ("object", 0, messages.INVALID_OBJECT),
+        ("object", "", messages.INVALID_OBJECT),
+        ("object", "abc", messages.INVALID_OBJECT),
         # string
-        ('string',      "",         None),
-        ('string',      "abc",      None),
-        ('string',      "-",        None),
-        ('string',      "...",      None),
-        ('string',      u"",        None),
-        ('string',      u"abc",     None),
-        ('string',      u"España",  None),
-        ('string',      "1",        None),
-        ('string',      None,       messages.INVALID_STRING),
-        ('string',      1,          messages.INVALID_STRING),
-        ('string',      [],         messages.INVALID_STRING),
-        ('string',      {},         messages.INVALID_STRING),
+        ("string", "", None),
+        ("string", "abc", None),
+        ("string", "-", None),
+        ("string", "...", None),
+        ("string", u"", None),
+        ("string", u"abc", None),
+        ("string", u"España", None),
+        ("string", "1", None),
+        ("string", None, messages.INVALID_STRING),
+        ("string", 1, messages.INVALID_STRING),
+        ("string", [], messages.INVALID_STRING),
+        ("string", {}, messages.INVALID_STRING),
     ]
     data_tests = [
         DataTest(
-            name='%02d_%s' % (i+1, data_type),
+            name="%02d_%s" % (i + 1, data_type),
             data=data,
             valid=expected_error is None,
-            expected_errors={'': [expected_error]} if expected_error else None,
+            expected_errors={"": [expected_error]} if expected_error else None,
             schema={"type": data_type},
         )
         for i, (data_type, data, expected_error) in enumerate(type_tests)
     ]
 
 
 class Unique(SchemaTest):
-    schema = {
-        "uniqueItems": True,
-    }
+    schema = {"uniqueItems": True}
     data_tests = [
-        DataTest(
-            name="unique array",
-            data=[1, 2],
-            valid=True,
-        ),
+        DataTest(name="unique array", data=[1, 2], valid=True),
         DataTest(
             name="non-unique array",
             data=[1, 1],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
         DataTest(
             name="non-unique numbers",
             data=[1.0, 1.00, 1],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
         DataTest(
             name="unique objects array",
             data=[{"foo": "bar"}, {"foo": "baz"}],
             valid=True,
         ),
         DataTest(
             name="non-unique objects array",
             data=[{"foo": "bar"}, {"foo": "bar"}],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
         DataTest(
             name="unique nested objects array",
-            data=[
-                {"foo": {"bar": {"baz": True}}},
-                {"foo": {"bar": {"baz": False}}}
-            ],
+            data=[{"foo": {"bar": {"baz": True}}}, {"foo": {"bar": {"baz": False}}}],
             valid=True,
         ),
         DataTest(
             name="non-unique nested objects array",
-            data=[
-                {"foo": {"bar": {"baz": True}}},
-                {"foo": {"bar": {"baz": True}}}
-            ],
+            data=[{"foo": {"bar": {"baz": True}}}, {"foo": {"bar": {"baz": True}}}],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
-        ),
-        DataTest(
-            name="unique array of arrays",
-            data=[["foo"], ["bar"]],
-            valid=True,
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
+        DataTest(name="unique array of arrays", data=[["foo"], ["bar"]], valid=True),
         DataTest(
             name="non-unique array of arrays",
             data=[["foo"], ["foo"]],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
-        ),
-        DataTest(
-            name="1 and True",
-            data=[1, True],
-            valid=True,
-        ),
-        DataTest(
-            name="0 and False",
-            data=[0, False],
-            valid=True,
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
+        DataTest(name="1 and True", data=[1, True], valid=True),
+        DataTest(name="0 and False", data=[0, False], valid=True),
         DataTest(
-            name="unique heterogeneous types",
-            data=[{}, [1], True, None, 1],
-            valid=True,
+            name="unique heterogeneous types", data=[{}, [1], True, None, 1], valid=True
         ),
         DataTest(
             name="non-unique heterogeneous types",
             data=[{}, [1], True, None, {}, 1],
             valid=False,
-            expected_errors={
-                '': [messages.NOT_UNIQUE],
-            }
+            expected_errors={"": [messages.NOT_UNIQUE]},
         ),
     ]
```

### Comparing `spidermon-1.8.0/tests/test_validators_schematics.py` & `spidermon-1.9.0/tests/test_validators_schematics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,479 +1,341 @@
 from __future__ import absolute_import
 import schematics
+from schematics.exceptions import ValidationError
 from schematics.models import Model
 from schematics.types import (
     StringType,
-    DateTimeType, DateType,
-    FloatType, IntType, LongType, DecimalType,
-    BooleanType, EmailType, URLType,
-    UUIDType, IPv4Type, MD5Type, SHA1Type,
+    DateTimeType,
+    DateType,
+    FloatType,
+    IntType,
+    LongType,
+    DecimalType,
+    BooleanType,
+    EmailType,
+    URLType,
+    UUIDType,
+    IPv4Type,
+    MD5Type,
+    SHA1Type,
 )
 from schematics.types.compound import ListType, DictType, ModelType
 
 from spidermon.contrib.validation import SchematicsValidator, messages
 
 
-SCHEMATICS1 = schematics.__version__.startswith('1.')
+SCHEMATICS1 = schematics.__version__.startswith("1.")
 
 
 def test_rogue_fields():
     """
     messages:
         - UNEXPECTED_FIELD
     """
     _test_data(
-        model=Model,
-        data={'a': 1},
-        expected=(False, {'a': [messages.UNEXPECTED_FIELD]}),
-    )
-    _test_data(
-        model=Model,
-        data={'a': 1},
-        expected=(True, {}),
-        strict=False
+        model=Model, data={"a": 1}, expected=(False, {"a": [messages.UNEXPECTED_FIELD]})
     )
+    _test_data(model=Model, data={"a": 1}, expected=(True, {}), strict=False)
 
 
 def test_required():
     """
     messages:
         - MISSING_REQUIRED_FIELD
     """
+
     class DataRequired(Model):
         a = StringType(required=True)
 
     class DataNotRequired(Model):
         a = StringType(required=False)
 
     _test_data(
         model=DataRequired,
         data={},
-        expected=(False, {'a': [messages.MISSING_REQUIRED_FIELD]}),
-    )
-    _test_data(
-        model=DataNotRequired,
-        data={},
-        expected=(True, {}),
+        expected=(False, {"a": [messages.MISSING_REQUIRED_FIELD]}),
     )
+    _test_data(model=DataNotRequired, data={}, expected=(True, {}))
 
 
 def test_choices():
     """
     messages:
         - VALUE_NOT_IN_CHOICES
     """
+
     class Data(Model):
-        a = StringType(choices=['a', 'b'])
+        a = StringType(choices=["a", "b"])
         b = IntType(choices=[1, 2, 3])
 
+    _test_data(model=Data, data={}, expected=(True, {}))
+    _test_data(model=Data, data={"a": "b", "b": 3}, expected=(True, {}))
     _test_data(
         model=Data,
-        data={},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={
-            'a': 'b',
-            'b': 3,
-        },
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={
-            'a': 'c',
-            'b': 4,
-        },
-        expected=(False, {
-            'a': [messages.VALUE_NOT_IN_CHOICES],
-            'b': [messages.VALUE_NOT_IN_CHOICES],
-        }),
+        data={"a": "c", "b": 4},
+        expected=(
+            False,
+            {
+                "a": [messages.VALUE_NOT_IN_CHOICES],
+                "b": [messages.VALUE_NOT_IN_CHOICES],
+            },
+        ),
     )
 
 
 def test_string_valid():
     """
     messages:
         - INVALID_STRING
     """
+
     class Data(Model):
         a = StringType()
 
+    _test_data(model=Data, data={"a": "hello there!"}, expected=(True, {}))
     _test_data(
-        model=Data,
-        data={'a': 'hello there!'},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': []},
-        expected=(False, {'a': [messages.INVALID_STRING]}),
+        model=Data, data={"a": []}, expected=(False, {"a": [messages.INVALID_STRING]})
     )
 
 
 def test_string_lengths():
     """
     messages:
         - FIELD_TOO_SHORT
         - FIELD_TOO_LONG
     """
+
     class Data(Model):
         a = StringType(min_length=2, max_length=5)
 
+    _test_data(model=Data, data={"a": "12"}, expected=(True, {}))
+    _test_data(model=Data, data={"a": "12345"}, expected=(True, {}))
     _test_data(
-        model=Data,
-        data={'a': '12'},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': '12345'},
-        expected=(True, {}),
+        model=Data, data={"a": "1"}, expected=(False, {"a": [messages.FIELD_TOO_SHORT]})
     )
     _test_data(
         model=Data,
-        data={'a': '1'},
-        expected=(False, {'a': [messages.FIELD_TOO_SHORT]}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': '123456'},
-        expected=(False, {'a': [messages.FIELD_TOO_LONG]}),
+        data={"a": "123456"},
+        expected=(False, {"a": [messages.FIELD_TOO_LONG]}),
     )
 
 
 def test_string_regex():
     """
     messages:
         - REGEX_NOT_MATCHED
     """
+
     class Data(Model):
-        a = StringType(regex='.*def.*')
+        a = StringType(regex=".*def.*")
 
     _test_data(
         model=Data,
-        data={'a': 'abc'},
-        expected=(False, {'a': [messages.REGEX_NOT_MATCHED]}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': 'abcdefghi'},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': 'def'},
-        expected=(True, {}),
+        data={"a": "abc"},
+        expected=(False, {"a": [messages.REGEX_NOT_MATCHED]}),
     )
+    _test_data(model=Data, data={"a": "abcdefghi"}, expected=(True, {}))
+    _test_data(model=Data, data={"a": "def"}, expected=(True, {}))
 
 
 def test_datetime():
     """
     messages:
         - INVALID_DATETIME
     """
+
     class Data(Model):
         a = DateTimeType()
 
     class DataWithFormats(Model):
-        a = DateTimeType(formats=('%Y-%m-%d %H:%M:%S.%f', '%Y-%m-%d %H:%M:%S'))
+        a = DateTimeType(formats=("%Y-%m-%d %H:%M:%S.%f", "%Y-%m-%d %H:%M:%S"))
 
     if SCHEMATICS1:
-        INVALID = [
-            '2015-05-13 13:35:15.718978',
-            '2015-05-13 13:35:15',
-        ]
+        INVALID = ["2015-05-13 13:35:15.718978", "2015-05-13 13:35:15"]
     else:
-        INVALID = [
-            'foo',
-            '1-2-3',
-        ]
-        CUSTOM_FORMAT = [
-            '2015-05-13 13:35:15.718978',
-            '2015-05-13 13:35:15',
-        ]
-    VALID = [
-        '2015-05-13T13:35:15.718978',
-        '2015-05-13T13:35:15',
-    ]
+        INVALID = ["foo", "1-2-3"]
+        CUSTOM_FORMAT = ["2015-05-13 13:35:15.718978", "2015-05-13 13:35:15"]
+    VALID = ["2015-05-13T13:35:15.718978", "2015-05-13T13:35:15"]
     _test_valid_invalid(
         model=Data,
         valid=VALID,
         invalid=INVALID,
         expected_error=messages.INVALID_DATETIME,
     )
     if SCHEMATICS1:
         for dt in INVALID:
-            _test_data(
-                model=DataWithFormats,
-                data={'a': dt},
-                expected=(True, {}),
-            )
+            _test_data(model=DataWithFormats, data={"a": dt}, expected=(True, {}))
     else:
         for dt in CUSTOM_FORMAT:
-            _test_data(
-                model=DataWithFormats,
-                data={'a': dt},
-                expected=(True, {}),
-            )
+            _test_data(model=DataWithFormats, data={"a": dt}, expected=(True, {}))
 
 
 def test_date():
     """
     messages:
         - INVALID_DATE
     """
+
     class Data(Model):
         a = DateType()
 
-    INVALID = [
-        '2015-05-13 13:35:15',
-        '13-05-2013',
-        '2015-20-13',
-        '2015-01-40',
-    ]
-    VALID = [
-        '2015-05-13',
-        '2050-01-01',
-    ]
+    INVALID = ["2015-05-13 13:35:15", "13-05-2013", "2015-20-13", "2015-01-40"]
+    VALID = ["2015-05-13", "2050-01-01"]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_DATE,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_DATE
     )
 
 
 def test_int():
     """
     messages:
         - INVALID_INT
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = IntType(min_value=-10, max_value=10)
         b = IntType()
 
-    INVALID = [
-        '',
-        'a',
-        '2a',
-        '2015-05-13 13:35:15',
-        '7.2',
-    ]
-    VALID = [
-        '1',
-        '8',
-        '-2',
-        '-7',
-        1,
-        8,
-        -2,
-        -7,
-    ]
+    INVALID = ["", "a", "2a", "2015-05-13 13:35:15", "7.2"]
+    VALID = ["1", "8", "-2", "-7", 1, 8, -2, -7]
     if SCHEMATICS1:
         VALID.append(7.2)
     else:
         INVALID.append(7.2)
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_INT,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_INT
     )
     _test_data(
-        model=Data,
-        data={'a': -20},
-        expected=(False, {'a': [messages.NUMBER_TOO_LOW]}),
+        model=Data, data={"a": -20}, expected=(False, {"a": [messages.NUMBER_TOO_LOW]})
     )
     _test_data(
-        model=Data,
-        data={'a': 11},
-        expected=(False, {'a': [messages.NUMBER_TOO_HIGH]}),
+        model=Data, data={"a": 11}, expected=(False, {"a": [messages.NUMBER_TOO_HIGH]})
     )
 
 
 def test_float():
     """
     messages:
         - INVALID_FLOAT
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = FloatType(min_value=-10, max_value=10)
 
-    INVALID = [
-        '',
-        'a',
-        '2a',
-        '2015-05-13 13:35:15',
-    ]
+    INVALID = ["", "a", "2a", "2015-05-13 13:35:15"]
     VALID = [
-        '1',
-        '-2',
-        '8',
-        '2.3',
-        '5.2354958',
-        '-9.231',
+        "1",
+        "-2",
+        "8",
+        "2.3",
+        "5.2354958",
+        "-9.231",
         1,
         -2,
         8,
         2.3,
         5.2354958,
         -9.231,
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_FLOAT,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_FLOAT
     )
     _test_data(
-        model=Data,
-        data={'a': -20},
-        expected=(False, {'a': [messages.NUMBER_TOO_LOW]}),
+        model=Data, data={"a": -20}, expected=(False, {"a": [messages.NUMBER_TOO_LOW]})
     )
     _test_data(
-        model=Data,
-        data={'a': 11},
-        expected=(False, {'a': [messages.NUMBER_TOO_HIGH]}),
+        model=Data, data={"a": 11}, expected=(False, {"a": [messages.NUMBER_TOO_HIGH]})
     )
 
 
 def test_long():
     """
     messages:
         - INVALID_LONG
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = LongType(min_value=-10, max_value=10)
 
-    INVALID = [
-        '',
-        'a',
-        '2a',
-        '2015-05-13 13:35:15',
-        '2.3',
-        '5.2354958',
-    ]
-    VALID = [
-        '1',
-        '-2',
-        '8',
-        1,
-        -2,
-        8,
-    ]
+    INVALID = ["", "a", "2a", "2015-05-13 13:35:15", "2.3", "5.2354958"]
+    VALID = ["1", "-2", "8", 1, -2, 8]
     if SCHEMATICS1:
         expected_error = messages.INVALID_LONG
     else:
         expected_error = messages.INVALID_INT
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=expected_error,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=expected_error
     )
     _test_data(
-        model=Data,
-        data={'a': -20},
-        expected=(False, {'a': [messages.NUMBER_TOO_LOW]}),
+        model=Data, data={"a": -20}, expected=(False, {"a": [messages.NUMBER_TOO_LOW]})
     )
     _test_data(
-        model=Data,
-        data={'a': 11},
-        expected=(False, {'a': [messages.NUMBER_TOO_HIGH]}),
+        model=Data, data={"a": 11}, expected=(False, {"a": [messages.NUMBER_TOO_HIGH]})
     )
 
 
 def test_decimal():
     """
     messages:
         - INVALID_DECIMAL
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = DecimalType(min_value=-10, max_value=10)
 
-    INVALID = [
-        '',
-        'a',
-        '2a',
-        '2015-05-13 13:35:15',
-    ]
+    INVALID = ["", "a", "2a", "2015-05-13 13:35:15"]
     VALID = [
-        '1',
-        '-2',
-        '8',
-        '2.3',
-        '5.2354958',
-        '-9.231',
+        "1",
+        "-2",
+        "8",
+        "2.3",
+        "5.2354958",
+        "-9.231",
         1,
         -2,
         8,
         2.3,
         5.2354958,
         -9.231,
     ]
     _test_valid_invalid(
         model=Data,
         valid=VALID,
         invalid=INVALID,
         expected_error=messages.INVALID_DECIMAL,
     )
     _test_data(
-        model=Data,
-        data={'a': -20},
-        expected=(False, {'a': [messages.NUMBER_TOO_LOW]}),
+        model=Data, data={"a": -20}, expected=(False, {"a": [messages.NUMBER_TOO_LOW]})
     )
     _test_data(
-        model=Data,
-        data={'a': 11},
-        expected=(False, {'a': [messages.NUMBER_TOO_HIGH]}),
+        model=Data, data={"a": 11}, expected=(False, {"a": [messages.NUMBER_TOO_HIGH]})
     )
 
 
 def test_boolean():
     """
     messages:
         - INVALID_BOOLEAN
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = BooleanType()
 
-    INVALID = [
-        '',
-        'a',
-        '2'
-        'TRUE',
-        'FALSE',
-        'TruE',
-        'FalsE',
-    ]
-    VALID = [
-        0,
-        1,
-        '0',
-        '1',
-        'True',
-        'False',
-        'true',
-        'false',
-        True,
-        False
-    ]
+    INVALID = ["", "a", "2" "TRUE", "FALSE", "TruE", "FalsE"]
+    VALID = [0, 1, "0", "1", "True", "False", "true", "false", True, False]
     _test_valid_invalid(
         model=Data,
         valid=VALID,
         invalid=INVALID,
         expected_error=messages.INVALID_BOOLEAN,
     )
 
@@ -481,474 +343,438 @@
 def test_email():
     """
     messages:
         - INVALID_EMAIL
         - NUMBER_TOO_LOW
         - NUMBER_TOO_HIGH
     """
+
     class Data(Model):
         a = EmailType()
 
     INVALID = [
-        '',
-        'johndoe',
-        'johndoe@domain'
-        'johndoe@domain.'
-        '@domain'
-        '@domain.com'
-        'domain.com'
+        "",
+        "johndoe",
+        "johndoe@domain" "johndoe@domain." "@domain" "@domain.com" "domain.com",
     ]
     VALID = [
-        'johndoe@domain.com',
-        'john.doe@domain.com',
-        'john.doe@sub.domain.com',
-        'j@sub.domain.com',
-        'j@d.com',
-        'j@domain.co.uk',
+        "johndoe@domain.com",
+        "john.doe@domain.com",
+        "john.doe@sub.domain.com",
+        "j@sub.domain.com",
+        "j@d.com",
+        "j@domain.co.uk",
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_EMAIL,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_EMAIL
     )
 
 
 def test_url():
     """
     messages:
         - INVALID_URL
     """
+
     class Data(Model):
         a = URLType()
 
     INVALID = [
-        '',
-        'http://',
-        'http://www.',
-        'www.',
-        'http://www. .com',
-        'domain.com',
-        'www.domain.com',
-        'http:/www.domain.com',
-        'http//www.domain.com',
-        'http:www.domain.com',
-        'htp://domain.com/',
-        'http://sub.domain.com\\en-us\\default.aspx\\',
-        'http:\\\\msdn.domain.com\\en-us\\library\\default.aspx\\',
-        'http:\\\\www.domain.com\\leafnode-L1.html',
-        './',
-        '../',
-        'http:\\\\www.domain.com\\leafnode-L1.xhtml\\',
-    ]
-    VALID = [
-        'http://www.domain',
-        'http://www.com',
-        'http://www.domain.com.',
-        'http://www.domain.com/.',
-        'http://www.domain.com/..',
-        'http://www.domain.com//cataglog//index.html',
-        'http://www.domain.net/',
-        'http://www.domain.com/level2/leafnode-L2.xhtml/',
-        'http://www.domain.com/level2/level3/leafnode-L3.xhtml/',
-        'http://www.domain.com?pageid=123&testid=1524',
-        'http://www.domain.com/do.html#A',
+        "",
+        "http://",
+        "http://www.",
+        "www.",
+        "http://www. .com",
+        "domain.com",
+        "www.domain.com",
+        "http:/www.domain.com",
+        "http//www.domain.com",
+        "http:www.domain.com",
+        "htp://domain.com/",
+        "http://sub.domain.com\\en-us\\default.aspx\\",
+        "http:\\\\msdn.domain.com\\en-us\\library\\default.aspx\\",
+        "http:\\\\www.domain.com\\leafnode-L1.html",
+        "./",
+        "../",
+        "http:\\\\www.domain.com\\leafnode-L1.xhtml\\",
+    ]
+    VALID = [
+        "http://www.domain",
+        "http://www.com",
+        "http://www.domain.com.",
+        "http://www.domain.com/.",
+        "http://www.domain.com/..",
+        "http://www.domain.com//cataglog//index.html",
+        "http://www.domain.net/",
+        "http://www.domain.com/level2/leafnode-L2.xhtml/",
+        "http://www.domain.com/level2/level3/leafnode-L3.xhtml/",
+        "http://www.domain.com?pageid=123&testid=1524",
+        "http://www.domain.com/do.html#A",
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_URL,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_URL
     )
 
 
 def test_uuid():
     """
     messages:
         - INVALID_UUID
     """
+
     class Data(Model):
         a = UUIDType()
 
     INVALID = [
-        '',
-        '678as6sd88ads67',
-        '678as6sd88ads67-alskjlasd',
-        'xxxxxxxx-xxxx-Mxxx-Nxxx-xxxxxxxxxxxx',
-        '2.25.290383009913173870543740933812899923227',
-    ]
-    VALID = [
-        '12345678-1234-5678-1234-567812345678',
-        '12345678123456781234567812345678',
-        'urn:uuid:12345678-1234-5678-1234-567812345678',
-        'cfc63f3f-f3a7-465a-8183-acf055c6d472',
-        '00000000-0000-0000-0000-000000000000',
-        '01234567-89ab-cdef-0123456789abcdef',
-        '0123456789abcdef0123456789abcdef',
+        "",
+        "678as6sd88ads67",
+        "678as6sd88ads67-alskjlasd",
+        "xxxxxxxx-xxxx-Mxxx-Nxxx-xxxxxxxxxxxx",
+        "2.25.290383009913173870543740933812899923227",
+    ]
+    VALID = [
+        "12345678-1234-5678-1234-567812345678",
+        "12345678123456781234567812345678",
+        "urn:uuid:12345678-1234-5678-1234-567812345678",
+        "cfc63f3f-f3a7-465a-8183-acf055c6d472",
+        "00000000-0000-0000-0000-000000000000",
+        "01234567-89ab-cdef-0123456789abcdef",
+        "0123456789abcdef0123456789abcdef",
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_UUID,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_UUID
     )
 
 
 def test_ipv4type():
     """
     messages:
         - INVALID_IPV4
     """
+
     class Data(Model):
         a = IPv4Type()
 
     INVALID = [
-        '',
-        '0',
-        '0.',
-        '0.0',
-        '0.0.',
-        '0.0.0',
-        '0.0.0.0.',
-        '0.0.0.0.0',
-        '256.256.256.256',
-        '2002:4559:1FE2::4559:1FE2',
-        '2002:4559:1FE2:0:0:0:4559:1FE2',
-        '2002:4559:1FE2:0000:0000:0000:4559:1FE2',
-    ]
-    VALID = [
-        '98.139.180.149',
-        '69.89.31.226',
-        '192.168.1.1',
-        '127.0.0.0',
-        '0.0.0.0',
-        '255.255.255.255',
+        "",
+        "0",
+        "0.",
+        "0.0",
+        "0.0.",
+        "0.0.0",
+        "0.0.0.0.",
+        "0.0.0.0.0",
+        "256.256.256.256",
+        "2002:4559:1FE2::4559:1FE2",
+        "2002:4559:1FE2:0:0:0:4559:1FE2",
+        "2002:4559:1FE2:0000:0000:0000:4559:1FE2",
+    ]
+    VALID = [
+        "98.139.180.149",
+        "69.89.31.226",
+        "192.168.1.1",
+        "127.0.0.0",
+        "0.0.0.0",
+        "255.255.255.255",
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_IPV4,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_IPV4
     )
 
 
 def test_md5():
     """
     messages:
         - INVALID_HASH
         - INVALID_HASH_LENGTH
     """
+
     class Data(Model):
         a = MD5Type()
 
     INVALID = [
-        '_b1a9953c4611296a827abf8a47804d7',
-        'zb1a9953c4611296a827abf8a47804d7',
-        'Gb1a9953c4611296a827abf8a47804d7',
+        "_b1a9953c4611296a827abf8a47804d7",
+        "zb1a9953c4611296a827abf8a47804d7",
+        "Gb1a9953c4611296a827abf8a47804d7",
         # FIXME: PY3: schematics uses integer conversion for validating hex and
         # Py3 integers can contain underscores.
         # '8b1_9953c4611296a827abf8c47804d1',
     ]
     VALID = [
-        '8b1a9953c4611296a827abf8c47804d7',
-        '7dd4bbe8a38600b556f79ca44c9b5132',
-        '11111111111111111111111111111111',
-        '8B1A9953C4611296A827ABF8C47804D1',
+        "8b1a9953c4611296a827abf8c47804d7",
+        "7dd4bbe8a38600b556f79ca44c9b5132",
+        "11111111111111111111111111111111",
+        "8B1A9953C4611296A827ABF8C47804D1",
     ]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_HASH,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_HASH
     )
     _test_data(
         model=Data,
-        data={'a': '8b1a9953c4611296a827abf8c47804d'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "8b1a9953c4611296a827abf8c47804d"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
     _test_data(
         model=Data,
-        data={'a': '8b1a9953c4611296'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "8b1a9953c4611296"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
     _test_data(
         model=Data,
-        data={'a': '8b1a9953c46112968b1a9953c46112968b1a9953c4611296'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "8b1a9953c46112968b1a9953c46112968b1a9953c4611296"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
 
 
 def test_sha1():
     """
     messages:
         - INVALID_HASH
         - INVALID_HASH_LENGTH
     """
+
     class Data(Model):
         a = SHA1Type()
 
     INVALID = [
-        '_03d40e1a2ede7e31f3c3b45a9e87d12ed33402e',
-        'g03d40e1a2ede7e31f3c3b45a9e87d12ed33402e',
-        'z03d40e1a2ede7e31f3c3b45a9e87d12ed33402e',
-        'G03d40e1a2ede7e31f3c3b45a9e87d12ed33402e',
+        "_03d40e1a2ede7e31f3c3b45a9e87d12ed33402e",
+        "g03d40e1a2ede7e31f3c3b45a9e87d12ed33402e",
+        "z03d40e1a2ede7e31f3c3b45a9e87d12ed33402e",
+        "G03d40e1a2ede7e31f3c3b45a9e87d12ed33402e",
         # FIXME: PY3: schematics uses integer conversion for validating hex and
         # Py3 integers can contain underscores.
         # 'a03d_0e1a2ede7e31f3c3b45a9e87d12ed33402e',
     ]
-    VALID = [
-        'a03d70e1a2ede7e31f3c3b45a9e87d12ed33402e',
-    ]
+    VALID = ["a03d70e1a2ede7e31f3c3b45a9e87d12ed33402e"]
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_HASH,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_HASH
     )
     _test_data(
         model=Data,
-        data={'a': 'a03d70e1a2ede7e31f3c3b45a9e87d12ed33402'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "a03d70e1a2ede7e31f3c3b45a9e87d12ed33402"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
     _test_data(
         model=Data,
-        data={'a': '8b1a9953c4611296'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "8b1a9953c4611296"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
     _test_data(
         model=Data,
-        data={'a': '8b1a9953c46112968b1a9953c46112968b1a9953c4611296'},
-        expected=(False, {'a': [messages.INVALID_HASH_LENGTH]}),
+        data={"a": "8b1a9953c46112968b1a9953c46112968b1a9953c4611296"},
+        expected=(False, {"a": [messages.INVALID_HASH_LENGTH]}),
     )
 
 
 def test_list():
     """
     messages:
         - INVALID_LIST
         - LIST_TOO_SHORT
         - LIST_TOO_LARGE
         - INVALID_INT
     """
+
     class Data(Model):
         a = ListType(field=IntType(), min_size=3, max_size=5)
 
+    _test_data(model=Data, data={"a": [1, 2, 3]}, expected=(True, {}))
+    _test_data(model=Data, data={"a": ["1", "2", "3"]}, expected=(True, {}))
     _test_data(
-        model=Data,
-        data={'a': [1, 2, 3]},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': ["1", "2", "3"]},
-        expected=(True, {}),
-    )
-    _test_data(
-        model=Data,
-        data={'a': Data},
-        expected=(False, {'a': [messages.INVALID_LIST]}),
+        model=Data, data={"a": Data}, expected=(False, {"a": [messages.INVALID_LIST]})
     )
     if SCHEMATICS1:
         _test_data(
             model=Data,
-            data={'a': ["a", "b", "c"]},
-            expected=(False, {'a': [messages.INVALID_INT]}),
+            data={"a": ["a", "b", "c"]},
+            expected=(False, {"a": [messages.INVALID_INT]}),
         )
     else:
         _test_data(
             model=Data,
-            data={'a': ["a", "b", "c"]},
+            data={"a": ["a", "b", "c"]},
             expected=(
                 False,
                 {
-                    'a.0': [messages.INVALID_INT],
-                    'a.1': [messages.INVALID_INT],
-                    'a.2': [messages.INVALID_INT]
-                }
+                    "a.0": [messages.INVALID_INT],
+                    "a.1": [messages.INVALID_INT],
+                    "a.2": [messages.INVALID_INT],
+                },
             ),
         )
     _test_data(
         model=Data,
-        data={'a': [1, 2]},
-        expected=(False, {'a': [messages.LIST_TOO_SHORT]}),
+        data={"a": [1, 2]},
+        expected=(False, {"a": [messages.LIST_TOO_SHORT]}),
     )
     _test_data(
         model=Data,
-        data={'a': [1, 2, 3, 4, 5, 6]},
-        expected=(False, {'a': [messages.LIST_TOO_LONG]}),
+        data={"a": [1, 2, 3, 4, 5, 6]},
+        expected=(False, {"a": [messages.LIST_TOO_LONG]}),
     )
 
 
 def test_dict():
     """
     messages:
         - INVALID_DICT
         - INVALID_INT
     """
+
     class Data(Model):
         a = DictType(field=IntType)
 
-    INVALID = [
-        'a',
-        Data,
-    ]
-    VALID = [
-        {},
-        {'some': 1},
-    ]
+    INVALID = ["a", Data]
+    VALID = [{}, {"some": 1}]
     if SCHEMATICS1:
         VALID.append([])
     else:
         INVALID.append([])
     _test_valid_invalid(
-        model=Data,
-        valid=VALID,
-        invalid=INVALID,
-        expected_error=messages.INVALID_DICT,
+        model=Data, valid=VALID, invalid=INVALID, expected_error=messages.INVALID_DICT
     )
     if SCHEMATICS1:
         _test_data(
             model=Data,
-            data={'a': {'some': "a"}},
-            expected=(False, {'a': [messages.INVALID_INT]}),
+            data={"a": {"some": "a"}},
+            expected=(False, {"a": [messages.INVALID_INT]}),
         )
     else:
         _test_data(
             model=Data,
-            data={'a': {'some': "a"}},
-            expected=(False, {'a.some': [messages.INVALID_INT]}),
+            data={"a": {"some": "a"}},
+            expected=(False, {"a.some": [messages.INVALID_INT]}),
         )
 
 
 def test_models():
     """
     messages:
         - UNEXPECTED_FIELD
         - MISSING_REQUIRED_FIELD
         - INVALID_FLOAT
     """
+
     class Coordinates(Model):
         latitude = FloatType(required=True)
         longitude = FloatType(required=True)
 
     class Geo(Model):
         coordinates = ModelType(Coordinates, required=True)
 
     class Data(Model):
         geo = ModelType(Geo, required=True)
 
     _test_data(
         model=Data,
-        data={'a': {}},
-        expected=(False, {
-            'a': [messages.UNEXPECTED_FIELD],
-            'geo': [messages.MISSING_REQUIRED_FIELD],
-        }),
+        data={"a": {}},
+        expected=(
+            False,
+            {
+                "a": [messages.UNEXPECTED_FIELD],
+                "geo": [messages.MISSING_REQUIRED_FIELD],
+            },
+        ),
     )
     _test_data(
         model=Data,
-        data={'geo': None},
-        expected=(False, {
-            'geo': [messages.MISSING_REQUIRED_FIELD]
-        }),
+        data={"geo": None},
+        expected=(False, {"geo": [messages.MISSING_REQUIRED_FIELD]}),
     )
     _test_data(
         model=Data,
-        data={'geo': {}},
-        expected=(False, {
-            'geo.coordinates': [messages.MISSING_REQUIRED_FIELD]
-        }),
+        data={"geo": {}},
+        expected=(False, {"geo.coordinates": [messages.MISSING_REQUIRED_FIELD]}),
     )
     _test_data(
         model=Data,
-        data={'geo': {
-            'coordinates': None,
-        }},
-        expected=(False, {
-            'geo.coordinates': [messages.MISSING_REQUIRED_FIELD]
-        }),
+        data={"geo": {"coordinates": None}},
+        expected=(False, {"geo.coordinates": [messages.MISSING_REQUIRED_FIELD]}),
     )
     _test_data(
         model=Data,
-        data={'geo': {
-            'coordinates': {},
-        }},
-        expected=(False, {
-            'geo.coordinates.latitude': [messages.MISSING_REQUIRED_FIELD],
-            'geo.coordinates.longitude': [messages.MISSING_REQUIRED_FIELD],
-        }),
+        data={"geo": {"coordinates": {}}},
+        expected=(
+            False,
+            {
+                "geo.coordinates.latitude": [messages.MISSING_REQUIRED_FIELD],
+                "geo.coordinates.longitude": [messages.MISSING_REQUIRED_FIELD],
+            },
+        ),
     )
     _test_data(
         model=Data,
-        data={'geo': {
-            'coordinates': {
-                'latitude': None,
-                'longitude': None,
+        data={"geo": {"coordinates": {"latitude": None, "longitude": None}}},
+        expected=(
+            False,
+            {
+                "geo.coordinates.latitude": [messages.MISSING_REQUIRED_FIELD],
+                "geo.coordinates.longitude": [messages.MISSING_REQUIRED_FIELD],
             },
-        }},
-        expected=(False, {
-            'geo.coordinates.latitude': [messages.MISSING_REQUIRED_FIELD],
-            'geo.coordinates.longitude': [messages.MISSING_REQUIRED_FIELD],
-        }),
+        ),
     )
     _test_data(
         model=Data,
-        data={'geo': {
-            'coordinates': {
-                'latitude': "y",
-                'longitude': "x",
+        data={"geo": {"coordinates": {"latitude": "y", "longitude": "x"}}},
+        expected=(
+            False,
+            {
+                "geo.coordinates.latitude": [messages.INVALID_FLOAT],
+                "geo.coordinates.longitude": [messages.INVALID_FLOAT],
             },
-        }},
-        expected=(False, {
-            'geo.coordinates.latitude': [messages.INVALID_FLOAT],
-            'geo.coordinates.longitude': [messages.INVALID_FLOAT],
-        }),
+        ),
     )
     _test_data(
         model=Data,
-        data={'geo': {
-            'coordinates': {
-                'latitude': 40.42,
-                'longitude': -3.71,
-            },
-        }},
+        data={"geo": {"coordinates": {"latitude": 40.42, "longitude": -3.71}}},
         expected=(True, {}),
     )
 
 
 def test_multiple_errors_per_field():
     """
     messages:
         - FIELD_TOO_SHORT
         - REGEX_NOT_MATCHED
     """
+
     class Data(Model):
-        a = StringType(min_length=3, regex=r'foo')
+        a = StringType(min_length=3, regex=r"foo")
 
-    data = {'a': 'z'}
+    data = {"a": "z"}
     v = SchematicsValidator(Data)
     result = v.validate(data, strict=True)
     assert result[0] is False
     error_messages = result[1]
-    assert 'a' in error_messages
+    assert "a" in error_messages
     expected = [messages.FIELD_TOO_SHORT, messages.REGEX_NOT_MATCHED]
-    assert sorted(error_messages['a']) == expected
+    assert sorted(error_messages["a"]) == expected
 
 
 def _test_data(model, data, expected, strict=True):
     v = SchematicsValidator(model)
     assert expected == v.validate(data, strict=strict)
 
 
-def _test_valid_invalid(model, valid, invalid, expected_error, expected_field='a'):
+def _test_valid_invalid(model, valid, invalid, expected_error, expected_field="a"):
     for dt in valid:
-        _test_data(
-            model=model,
-            data={expected_field: dt},
-            expected=(True, {}),
-        )
+        _test_data(model=model, data={expected_field: dt}, expected=(True, {}))
     for dt in invalid:
         _test_data(
             model=model,
             data={expected_field: dt},
             expected=(False, {expected_field: [expected_error]}),
         )
+
+
+def test_validation_error_on_model_level_validation():
+    class TestModel(Model):
+        field_a = StringType()
+
+        def validate_field_a(self, data, value):
+            raise ValidationError("Model-level validation failed.")
+
+    _test_data(
+        model=TestModel,
+        data={"field_a": "some_data"},
+        expected=(False, {"field_a": ["Model-level validation failed."]}),
+    )
```

### Comparing `spidermon-1.8.0/tests/test_suites.py` & `spidermon-1.9.0/tests/test_suites.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import absolute_import
 import pytest
 
 from spidermon import MonitorSuite
-from spidermon.exceptions import (InvalidMonitor, InvalidMonitorIterable,
-                                  InvalidMonitorClass, InvalidMonitorTuple,
-                                  NotAllowedMethod)
+from spidermon.exceptions import (
+    InvalidMonitor,
+    InvalidMonitorIterable,
+    InvalidMonitorClass,
+    InvalidMonitorTuple,
+    NotAllowedMethod,
+)
 
 from .fixtures.suites import *
 
 
 class SuiteDefinition(object):
     def __init__(self, suite_class, monitors=None, expected_number_of_monitors=0):
         self.suite_class = suite_class
@@ -16,67 +20,63 @@
         self.expected_number_of_monitors = expected_number_of_monitors
 
 
 CLASS_SUITE_DEFINITIONS = [
     # ---------------------------------------------------------------------------------
     #               suite_class    monitors               expected_number_of_monitors
     # ---------------------------------------------------------------------------------
-
     # no monitors
-    SuiteDefinition(EmptySuite,    [],                                              0),
-    SuiteDefinition(Suite01,       [],                                              3),
-    SuiteDefinition(Suite02,       [],                                              5),
-    SuiteDefinition(Suite03,       [],                                              8),
-    SuiteDefinition(Suite04,       [],                                             13),
-
+    SuiteDefinition(EmptySuite, [], 0),
+    SuiteDefinition(Suite01, [], 3),
+    SuiteDefinition(Suite02, [], 5),
+    SuiteDefinition(Suite03, [], 8),
+    SuiteDefinition(Suite04, [], 13),
     # monitors as classes
-    SuiteDefinition(EmptySuite,    [EmptyMonitor],                                  0),
-    SuiteDefinition(EmptySuite,    [Monitor01],                                     3),
-    SuiteDefinition(EmptySuite,    [Monitor02],                                     2),
-    SuiteDefinition(EmptySuite,    [Monitor01, Monitor02],                          5),
-    SuiteDefinition(EmptySuite,    [Suite01],                                       3),
-    SuiteDefinition(EmptySuite,    [Suite01, Suite02],                              8),
-    SuiteDefinition(EmptySuite,    [Suite01, Suite02, Monitor01, Monitor02],       13),
-    SuiteDefinition(Suite01,       [Suite01, Suite02, Monitor01, Monitor02],       16),
-    SuiteDefinition(Suite02,       [Suite01, Suite02, Monitor01, Monitor02],       18),
-    SuiteDefinition(Suite03,       [Suite01, Suite02, Monitor01, Monitor02],       21),
-    SuiteDefinition(Suite04,       [Suite01, Suite02, Monitor01, Monitor02],       26),
-
+    SuiteDefinition(EmptySuite, [EmptyMonitor], 0),
+    SuiteDefinition(EmptySuite, [Monitor01], 3),
+    SuiteDefinition(EmptySuite, [Monitor02], 2),
+    SuiteDefinition(EmptySuite, [Monitor01, Monitor02], 5),
+    SuiteDefinition(EmptySuite, [Suite01], 3),
+    SuiteDefinition(EmptySuite, [Suite01, Suite02], 8),
+    SuiteDefinition(EmptySuite, [Suite01, Suite02, Monitor01, Monitor02], 13),
+    SuiteDefinition(Suite01, [Suite01, Suite02, Monitor01, Monitor02], 16),
+    SuiteDefinition(Suite02, [Suite01, Suite02, Monitor01, Monitor02], 18),
+    SuiteDefinition(Suite03, [Suite01, Suite02, Monitor01, Monitor02], 21),
+    SuiteDefinition(Suite04, [Suite01, Suite02, Monitor01, Monitor02], 26),
     # monitors as instances
-    SuiteDefinition(EmptySuite,    [Suite01()],                                     3),
-    SuiteDefinition(EmptySuite,    [Suite02()],                                     5),
-    SuiteDefinition(EmptySuite,    [Suite03()],                                     8),
-    SuiteDefinition(EmptySuite,    [Suite04()],                                    13),
-    SuiteDefinition(EmptySuite,    [Suite01(), Suite02(), Suite03(), Suite04()],   29),
-
+    SuiteDefinition(EmptySuite, [Suite01()], 3),
+    SuiteDefinition(EmptySuite, [Suite02()], 5),
+    SuiteDefinition(EmptySuite, [Suite03()], 8),
+    SuiteDefinition(EmptySuite, [Suite04()], 13),
+    SuiteDefinition(EmptySuite, [Suite01(), Suite02(), Suite03(), Suite04()], 29),
     # monitors as tuples
-    SuiteDefinition(EmptySuite,    [('M1', Monitor01)],                             3),
-    SuiteDefinition(EmptySuite,    [('M1', Monitor01), ('M2', Monitor02)],          5),
-    SuiteDefinition(EmptySuite,    [('S', Suite04)],                               13),
+    SuiteDefinition(EmptySuite, [("M1", Monitor01)], 3),
+    SuiteDefinition(EmptySuite, [("M1", Monitor01), ("M2", Monitor02)], 5),
+    SuiteDefinition(EmptySuite, [("S", Suite04)], 13),
 ]
-INVALID_SUITE_DEFINITION_NON_ITERABLE   = SuiteDefinition(EmptySuite, 10)
-INVALID_SUITE_DEFINITION_NONE           = SuiteDefinition(EmptySuite, [None])
-INVALID_SUITE_DEFINITION_NUMBER         = SuiteDefinition(EmptySuite, [10])
-INVALID_SUITE_DEFINITION_CLASS          = SuiteDefinition(EmptySuite, [object])
-INVALID_SUITE_DEFINITION_TUPLE1         = SuiteDefinition(EmptySuite, [(1,)])
-INVALID_SUITE_DEFINITION_TUPLE3         = SuiteDefinition(EmptySuite, [(1, 2, 3)])
-INVALID_SUITE_DEFINITION_TUPLE2_WRONG1  = SuiteDefinition(EmptySuite, [(1, 2)])
-INVALID_SUITE_DEFINITION_TUPLE2_WRONG2  = SuiteDefinition(EmptySuite, [('A', 2)])
+INVALID_SUITE_DEFINITION_NON_ITERABLE = SuiteDefinition(EmptySuite, 10)
+INVALID_SUITE_DEFINITION_NONE = SuiteDefinition(EmptySuite, [None])
+INVALID_SUITE_DEFINITION_NUMBER = SuiteDefinition(EmptySuite, [10])
+INVALID_SUITE_DEFINITION_CLASS = SuiteDefinition(EmptySuite, [object])
+INVALID_SUITE_DEFINITION_TUPLE1 = SuiteDefinition(EmptySuite, [(1,)])
+INVALID_SUITE_DEFINITION_TUPLE3 = SuiteDefinition(EmptySuite, [(1, 2, 3)])
+INVALID_SUITE_DEFINITION_TUPLE2_WRONG1 = SuiteDefinition(EmptySuite, [(1, 2)])
+INVALID_SUITE_DEFINITION_TUPLE2_WRONG2 = SuiteDefinition(EmptySuite, [("A", 2)])
 
 INVALID_SUITE_DEFINITIONS = [
     # --------------------------------------------------------------
     # definition                                raises
     # --------------------------------------------------------------
-    (INVALID_SUITE_DEFINITION_NONE,             InvalidMonitor),
-    (INVALID_SUITE_DEFINITION_NUMBER,           InvalidMonitor),
-    (INVALID_SUITE_DEFINITION_CLASS,            InvalidMonitorClass),
-    (INVALID_SUITE_DEFINITION_TUPLE1,           InvalidMonitorTuple),
-    (INVALID_SUITE_DEFINITION_TUPLE3,           InvalidMonitorTuple),
-    (INVALID_SUITE_DEFINITION_TUPLE2_WRONG1,    InvalidMonitorTuple),
-    (INVALID_SUITE_DEFINITION_TUPLE2_WRONG2,    InvalidMonitor),
+    (INVALID_SUITE_DEFINITION_NONE, InvalidMonitor),
+    (INVALID_SUITE_DEFINITION_NUMBER, InvalidMonitor),
+    (INVALID_SUITE_DEFINITION_CLASS, InvalidMonitorClass),
+    (INVALID_SUITE_DEFINITION_TUPLE1, InvalidMonitorTuple),
+    (INVALID_SUITE_DEFINITION_TUPLE3, InvalidMonitorTuple),
+    (INVALID_SUITE_DEFINITION_TUPLE2_WRONG1, InvalidMonitorTuple),
+    (INVALID_SUITE_DEFINITION_TUPLE2_WRONG2, InvalidMonitor),
 ]
 
 
 def test_creation_error_non_iterable():
     with pytest.raises(InvalidMonitorIterable):
         _test_creation_from_init(INVALID_SUITE_DEFINITION_NON_ITERABLE)
     with pytest.raises(InvalidMonitorIterable):
@@ -115,16 +115,15 @@
     for definition in CLASS_SUITE_DEFINITIONS:
         _test_creation_from_add_monitor(definition)
 
 
 def _test_creation_from_init(definition):
     suite = definition.suite_class(monitors=definition.monitors)
     check_suite(
-        suite=suite,
-        expected_number_of_monitors=definition.expected_number_of_monitors,
+        suite=suite, expected_number_of_monitors=definition.expected_number_of_monitors
     )
 
 
 def test_not_allowed_methods():
     suite = EmptySuite()
     with pytest.raises(NotAllowedMethod):
         suite.addTest()
@@ -132,33 +131,31 @@
         suite.addTests()
 
 
 def _test_creation_from_add_monitors(definition):
     suite = definition.suite_class()
     suite.add_monitors(definition.monitors)
     check_suite(
-        suite=suite,
-        expected_number_of_monitors=definition.expected_number_of_monitors,
+        suite=suite, expected_number_of_monitors=definition.expected_number_of_monitors
     )
 
 
 def _test_creation_from_add_monitor(definition):
     suite = definition.suite_class()
     for monitor in definition.monitors:
         suite.add_monitor(monitor)
     check_suite(
-        suite=suite,
-        expected_number_of_monitors=definition.expected_number_of_monitors,
+        suite=suite, expected_number_of_monitors=definition.expected_number_of_monitors
     )
 
 
 def check_suite(suite, expected_number_of_monitors):
-    #print
-    #print suite.debug_tree()
-    #print
+    # print
+    # print suite.debug_tree()
+    # print
     assert isinstance(suite, MonitorSuite)
     assert suite.number_of_monitors == expected_number_of_monitors
     for monitor in suite:
         assert isinstance(monitor, (Monitor, MonitorSuite))
     all_monitors = suite.all_monitors
     assert len(all_monitors) == expected_number_of_monitors
     for test in all_monitors:
```

### Comparing `spidermon-1.8.0/tests/test_descriptions.py` & `spidermon-1.9.0/tests/test_descriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from __future__ import absolute_import
 from .fixtures.descriptions import *
 
 MONITOR_DESCRIPTIONS = [
     # --------------------------------------------------------------
     # monitor class                 description
     # --------------------------------------------------------------
-    (NotDescriptedMonitor,          ''),
-    (DocstringDescriptedMonitor,    'docstring monitor description'),
-    (DescoratedDescriptedMonitor,   'decorator monitor description'),
-    (DescoratedDescriptedMonitor2,  'decorator monitor description'),
+    (NotDescriptedMonitor, ""),
+    (DocstringDescriptedMonitor, "docstring monitor description"),
+    (DescoratedDescriptedMonitor, "decorator monitor description"),
+    (DescoratedDescriptedMonitor2, "decorator monitor description"),
 ]
 
 SUITE_DESCRIPTIONS = [
     # --------------------------------------------------------------
     # suite class                   description
     # --------------------------------------------------------------
-    (NotDescriptedSuite,            ''),
-    (DocstringDescriptedSuite,      'docstring suite description'),
-    (DescoratedDescriptedSuite,     'decorator suite description'),
-    (DescoratedDescriptedSuite2,    'decorator suite description'),
+    (NotDescriptedSuite, ""),
+    (DocstringDescriptedSuite, "docstring suite description"),
+    (DescoratedDescriptedSuite, "decorator suite description"),
+    (DescoratedDescriptedSuite2, "decorator suite description"),
 ]
 
 METHOD_DESCRIPTIONS = [
     # ---------------------------------------------------------------------------------------------
     # monitor class                 method name                     description
     # ---------------------------------------------------------------------------------------------
-    (DescriptedMethodsMonitor,      'test_not_descripted',          ''),
-    (DescriptedMethodsMonitor,      'test_docstring_descripted',    'docstring method description'),
-    (DescriptedMethodsMonitor,      'test_decorator_descripted',    'decorator method description'),
-    (DescriptedMethodsMonitor,      'test_decorator_descripted2',   'decorator method description'),
+    (DescriptedMethodsMonitor, "test_not_descripted", ""),
+    (
+        DescriptedMethodsMonitor,
+        "test_docstring_descripted",
+        "docstring method description",
+    ),
+    (
+        DescriptedMethodsMonitor,
+        "test_decorator_descripted",
+        "decorator method description",
+    ),
+    (
+        DescriptedMethodsMonitor,
+        "test_decorator_descripted2",
+        "decorator method description",
+    ),
 ]
 
 
 def test_monitor_descriptions():
     for monitor_class, description in MONITOR_DESCRIPTIONS:
         assert monitor_class().monitor_description == description
```

### Comparing `spidermon-1.8.0/tests/fixtures/expressions.py` & `spidermon-1.9.0/tests/fixtures/expressions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,181 +1,155 @@
 from six import PY2
 
-SYNTAXERROR_EXPRESSIONS = [
-    '?',
-    'a string',
-    'a=',
-]
+SYNTAXERROR_EXPRESSIONS = ["?", "a string", "a="]
 
 INVALID_EXPRESSIONS = [
     None,
     0,
-    '',
+    "",
     """
     """,
-    'a > b\na > b',
-    'import os',
-    'from os import *',
-    'for i in range(10): pass',
-    'def something(): pass',
-    'lambda x: x',
+    "a > b\na > b",
+    "import os",
+    "from os import *",
+    "for i in range(10): pass",
+    "def something(): pass",
+    "lambda x: x",
     "del a",
     # "print(a)",
     "raise Exception",
     "pass",
     "return",
     "yield x",
-
     # Assignment Operations
     "a = 1",
     "a += 1",
     "a -= 1",
     "a *= 1",
     "a /= 1",
     "a %= 1",
     "a **= 1",
     "a //= 1",
 ]
 
 VALID_EXPRESSIONS = [
     # Strings
     "'single quoted string'",
-    "\"double quoted string\"",
+    '"double quoted string"',
     "u'unicode single quoted string'",
-    "u\"unicode double quoted string\"",
-
+    'u"unicode double quoted string"',
     # Numbers
     "0",
     ".5",
     "-10",
     "10",
     "1.0",
     "-1.0",
     "3.14j",
-
     # Sequences
     "[1, 2, 3]",
     "{'a': 1, 'b': 1}",
     "set()",
     "(1, 2)",
     "len(a)",
-
     # Constants
     "None",
     "True",
     "False",
-
     # Arithmetic Operations
     "-a",
     "a + 1",
     "a - 1",
     "a / 1",
     "a * 1",
     "a % 1",
     "a ** 1",
     "a // 1",
-
     # Comparison Operations
     "a == b",
     "a != b",
     "a > b",
     "a < b",
     "a >= b",
     "a <= b",
     "1 < a < 10",
-
     # Bitwise Operations
     "a & b",
     "a | b",
     "a ^ b",
     "~a",
     "a << b",
     "a >> b",
-
     # Logical Operations
     "a and b",
     "a or b",
     "not a",
-
     # Membership Operations
     "a in b",
     "a not in b",
-
     # Identity Operations
     "a is 10",
     "a is not 10",
-
     # Inline if statement
     "a if b else c",
-
     # Subscripting
     "a[1]",
     "a[1:2]",
     "a[1:2, 3]",
-
     # Comprehensions
     "[i for i in range(10)]",
     "{i: i**2 for i in range(10)}",
     "{i for i in range(10)}",
     "[n for n in range(10) if n>5]",
-
     # Attribute access
-    "stats.scraped_items"
+    "stats.scraped_items",
 ]
 
 
 EXPRESSIONS_TO_EVALUATE = [
-    ('stats.item_scraped_count == 10000', False),
-    ('stats.item_scraped_count != 10000', True),
-    ('stats.item_scraped_count < 10000', False),
-    ('stats.item_scraped_count > 10000', True),
-    ('stats.item_scraped_count <= 10000', False),
-    ('stats.item_scraped_count >= 10000', True),
-    ('10000 < stats.item_scraped_count < 100000', True),
-    ('stats.item_scraped_count == .5', False),
-    ('stats.item_scraped_count < .5', False),
-    ('stats.item_scraped_count > .5', True),
-
+    ("stats.item_scraped_count == 10000", False),
+    ("stats.item_scraped_count != 10000", True),
+    ("stats.item_scraped_count < 10000", False),
+    ("stats.item_scraped_count > 10000", True),
+    ("stats.item_scraped_count <= 10000", False),
+    ("stats.item_scraped_count >= 10000", True),
+    ("10000 < stats.item_scraped_count < 100000", True),
+    ("stats.item_scraped_count == .5", False),
+    ("stats.item_scraped_count < .5", False),
+    ("stats.item_scraped_count > .5", True),
     ('stats.finish_reason in ["finished"]', True),
     ('stats.finish_reason in ["a", "b"]', False),
     ('stats.finish_reason not in ["a", "b"]', True),
     ('stats.finish_reason in {"finished": 0}', True),
     ('stats.finish_reason in {"finished": 0}.keys()', True),
     ('stats.finish_reason in ("finished",)', True),
     ('len(stats.finish_reason) == len("finished")', True),
-    ('stats.finish_reason is not None', True),
-    ('len(stats.finish_reason) > 0', True),
-    ('(len(stats.finish_reason) > 0) == True', True),
-    ('(len(stats.finish_reason) > 0) != False', True),
-    ('(len(stats.finish_reason) > 0) is not False', True),
-    ('(len(stats.finish_reason) > 0) is True', True),
-
+    ("stats.finish_reason is not None", True),
+    ("len(stats.finish_reason) > 0", True),
+    ("(len(stats.finish_reason) > 0) == True", True),
+    ("(len(stats.finish_reason) > 0) != False", True),
+    ("(len(stats.finish_reason) > 0) is not False", True),
+    ("(len(stats.finish_reason) > 0) is True", True),
     ('stats["downloader/exception_count"] == 16', True),
     ('-stats["downloader/exception_count"] == -16', True),
     ('stats["downloader/exception_count"]+1 == 17', True),
     ('stats["downloader/exception_count"]-1 == 15', True),
     ('stats["downloader/exception_count"]/2 == 8', True),
     ('stats["downloader/exception_count"]*2 == 32', True),
     ('stats["downloader/exception_count"]%3 == 1', True),
     ('stats["downloader/exception_count"]**2 == 256', True),
     ('stats["downloader/exception_count"]//2 == 8', True),
     ('stats["downloader/exception_count"]*2/2 == 16', True),
-
-    ('stats.has_errors and stats.has_redirections', True),
-    ('stats.has_errors or stats.has_redirections', True),
-    ('not stats.has_errors', False),
-    ('stats.has_errors is True', True),
-    ('stats.has_errors is not True', False),
-    ('True if stats.has_errors else False', True),
-    ('True if not stats.has_errors else False', False),
-    ('stats.item_scraped_count in range(29830, 29840)', True),
+    ("stats.has_errors and stats.has_redirections", True),
+    ("stats.has_errors or stats.has_redirections", True),
+    ("not stats.has_errors", False),
+    ("stats.has_errors is True", True),
+    ("stats.has_errors is not True", False),
+    ("True if stats.has_errors else False", True),
+    ("True if not stats.has_errors else False", False),
+    ("stats.item_scraped_count in range(29830, 29840)", True),
 ]
 
 
 if PY2:
-    VALID_EXPRESSIONS.extend([
-        "51924361L",
-        "a <> b",
-    ])
-    EXPRESSIONS_TO_EVALUATE.extend([
-        ('stats.item_scraped_count <> 10000', True),
-    ])
+    VALID_EXPRESSIONS.extend(["51924361L", "a <> b"])
+    EXPRESSIONS_TO_EVALUATE.extend([("stats.item_scraped_count <> 10000", True)])
```

### Comparing `spidermon-1.8.0/tests/fixtures/ordering.py` & `spidermon-1.9.0/tests/fixtures/ordering.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,42 +46,39 @@
         pass
 
 
 # ----------------------------------
 # Methods ordering
 # ----------------------------------
 class UnorderedMethodsMonitor(Monitor):
-
     def test_a(self):
         pass
 
     def test_b(self):
         pass
 
     def test_c(self):
         pass
 
 
 class OrderedMethodsMonitor(Monitor):
-
     @monitors.order(3)
     def test_a(self):
         pass
 
     @monitors.order(2)
     def test_b(self):
         pass
 
     @monitors.order(1)
     def test_c(self):
         pass
 
 
 class EqualOrderedMethodsMonitor(Monitor):
-
     @monitors.order(5)
     def test_a(self):
         pass
 
     @monitors.order(5)
     def test_b(self):
         pass
```

### Comparing `spidermon-1.8.0/tests/fixtures/levels.py` & `spidermon-1.9.0/tests/fixtures/levels.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,54 +29,89 @@
 
 
 # ----------------------------------
 # Monitors
 # ----------------------------------
 class Monitors:
     class NoLevelMonitor:
-        class NoLevelMethod(NoLevelMethodMonitor): pass
-        class HighLevelMethod(HighLevelMethodMonitor): pass
-        class NormalLevelMethod(NormalLevelMethodMonitor): pass
-        class LowLevelMethod(LowLevelMethodMonitor): pass
+        class NoLevelMethod(NoLevelMethodMonitor):
+            pass
+
+        class HighLevelMethod(HighLevelMethodMonitor):
+            pass
+
+        class NormalLevelMethod(NormalLevelMethodMonitor):
+            pass
+
+        class LowLevelMethod(LowLevelMethodMonitor):
+            pass
 
     class HighLevelMonitor:
         @monitors.level.high
-        class NoLevelMethod(NoLevelMethodMonitor): pass
+        class NoLevelMethod(NoLevelMethodMonitor):
+            pass
+
         @monitors.level.high
-        class HighLevelMethod(HighLevelMethodMonitor): pass
+        class HighLevelMethod(HighLevelMethodMonitor):
+            pass
+
         @monitors.level.high
-        class NormalLevelMethod(NormalLevelMethodMonitor): pass
+        class NormalLevelMethod(NormalLevelMethodMonitor):
+            pass
+
         @monitors.level.high
-        class LowLevelMethod(LowLevelMethodMonitor): pass
+        class LowLevelMethod(LowLevelMethodMonitor):
+            pass
 
     class NormalLevelMonitor:
         @monitors.level.normal
-        class NoLevelMethod(NoLevelMethodMonitor): pass
+        class NoLevelMethod(NoLevelMethodMonitor):
+            pass
+
         @monitors.level.normal
-        class HighLevelMethod(HighLevelMethodMonitor): pass
+        class HighLevelMethod(HighLevelMethodMonitor):
+            pass
+
         @monitors.level.normal
-        class NormalLevelMethod(NormalLevelMethodMonitor): pass
+        class NormalLevelMethod(NormalLevelMethodMonitor):
+            pass
+
         @monitors.level.normal
-        class LowLevelMethod(LowLevelMethodMonitor): pass
+        class LowLevelMethod(LowLevelMethodMonitor):
+            pass
 
     class LowLevelMonitor:
         @monitors.level.low
-        class NoLevelMethod(NoLevelMethodMonitor): pass
+        class NoLevelMethod(NoLevelMethodMonitor):
+            pass
+
         @monitors.level.low
-        class HighLevelMethod(HighLevelMethodMonitor): pass
+        class HighLevelMethod(HighLevelMethodMonitor):
+            pass
+
         @monitors.level.low
-        class NormalLevelMethod(NormalLevelMethodMonitor): pass
+        class NormalLevelMethod(NormalLevelMethodMonitor):
+            pass
+
         @monitors.level.low
-        class LowLevelMethod(LowLevelMethodMonitor): pass
+        class LowLevelMethod(LowLevelMethodMonitor):
+            pass
 
 
 # ----------------------------------
 # Suites
 # ----------------------------------
 class Suites:
-    class NoLevelSuite(MonitorSuite): pass
+    class NoLevelSuite(MonitorSuite):
+        pass
+
     @monitors.level.high
-    class HighLevelSuite(MonitorSuite): pass
+    class HighLevelSuite(MonitorSuite):
+        pass
+
     @monitors.level.normal
-    class NormalLevelSuite(MonitorSuite): pass
+    class NormalLevelSuite(MonitorSuite):
+        pass
+
     @monitors.level.low
-    class LowLevelSuite(MonitorSuite): pass
+    class LowLevelSuite(MonitorSuite):
+        pass
```

### Comparing `spidermon-1.8.0/tests/fixtures/validators.py` & `spidermon-1.9.0/tests/fixtures/validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,35 +11,20 @@
 
 class TreeValidator(Model):
     child = BaseType(required=True)
 
 
 tree_schema = {
     "$schema": "http://json-schema.org/draft-04/schema",
-    "required": [
-        "child"
-    ],
+    "required": ["child"],
     "type": "object",
-    "properties": {
-        "child": {
-            "type": "object"
-        }
-    }
+    "properties": {"child": {"type": "object"}},
 }
 
 test_schema = {
     "$schema": "http://json-schema.org/draft-04/schema",
-    "required": [
-        "url"
-    ],
+    "required": ["url"],
     "type": "object",
-    "properties": {
-        "url": {
-            "type": "string"
-        },
-        "title": {
-            "type": "string"
-        },
-    }
+    "properties": {"url": {"type": "string"}, "title": {"type": "string"}},
 }
 
 test_schema_string = json.dumps(test_schema)
```

### Comparing `spidermon-1.8.0/tests/fixtures/names.py` & `spidermon-1.9.0/tests/fixtures/names.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,62 +5,62 @@
 # ----------------------------------
 # Monitors
 # ----------------------------------
 class UnnamedMonitor(Monitor):
     def test_without_name(self):
         pass
 
-    @monitors.name('A Test')
+    @monitors.name("A Test")
     def test_with_name(self):
         pass
 
 
-@monitors.name('Class Monitor')
+@monitors.name("Class Monitor")
 class NamedMonitor(Monitor):
     def test_without_name(self):
         pass
 
-    @monitors.name('A Test')
+    @monitors.name("A Test")
     def test_with_name(self):
         pass
 
 
 # ----------------------------------
 # Child Suites
 # ----------------------------------
 class BaseChildSuite(MonitorSuite):
     monitors = [
         UnnamedMonitor,
         NamedMonitor,
-        ('Instance Monitor', UnnamedMonitor),
-        ('Instance Monitor', NamedMonitor),
+        ("Instance Monitor", UnnamedMonitor),
+        ("Instance Monitor", NamedMonitor),
     ]
 
 
 class ChildUnnamedSuite(BaseChildSuite):
     pass
 
 
-@monitors.name('The Child Suite')
+@monitors.name("The Child Suite")
 class ChildNamedSuite(BaseChildSuite):
     pass
 
 
 # ----------------------------------
 # Top Suites
 # ----------------------------------
 class BaseTopSuite(MonitorSuite):
     monitors = [
         ChildUnnamedSuite,
         ChildNamedSuite,
-        ('Instance Suite Name', ChildUnnamedSuite),
-        ('Instance Suite Name', ChildNamedSuite),
+        ("Instance Suite Name", ChildUnnamedSuite),
+        ("Instance Suite Name", ChildNamedSuite),
     ]
 
 
 class UnnamedTopSuite(BaseTopSuite):
     pass
 
 
-@monitors.name('The Top Suite')
+@monitors.name("The Top Suite")
 class NamedTopSuite(BaseTopSuite):
     pass
```

### Comparing `spidermon-1.8.0/tests/fixtures/descriptions.py` & `spidermon-1.9.0/tests/fixtures/descriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,61 +12,62 @@
 
 class NotDescriptedMonitor(BaseMonitor):
     pass
 
 
 class DocstringDescriptedMonitor(BaseMonitor):
     """docstring monitor description"""
+
     pass
 
 
-@monitors.description('decorator monitor description')
+@monitors.description("decorator monitor description")
 class DescoratedDescriptedMonitor(BaseMonitor):
     pass
 
 
-@monitors.description('decorator monitor description')
+@monitors.description("decorator monitor description")
 class DescoratedDescriptedMonitor2(BaseMonitor):
     """docstring monitor description"""
 
 
 # ----------------------------------
 # Suites
 # ----------------------------------
 class NotDescriptedSuite(MonitorSuite):
     pass
 
 
 class DocstringDescriptedSuite(MonitorSuite):
     """docstring suite description"""
+
     pass
 
 
-@monitors.description('decorator suite description')
+@monitors.description("decorator suite description")
 class DescoratedDescriptedSuite(MonitorSuite):
     pass
 
 
-@monitors.description('decorator suite description')
+@monitors.description("decorator suite description")
 class DescoratedDescriptedSuite2(MonitorSuite):
     """docstring suite description"""
 
 
 # ----------------------------------
 # Methods
 # ----------------------------------
 class DescriptedMethodsMonitor(Monitor):
-
     def test_not_descripted(self):
         pass
 
     def test_docstring_descripted(self):
         """docstring method description"""
         pass
 
-    @monitors.description('decorator method description')
+    @monitors.description("decorator method description")
     def test_decorator_descripted(self):
         pass
 
-    @monitors.description('decorator method description')
+    @monitors.description("decorator method description")
     def test_decorator_descripted2(self):
         """docstring method description"""
```

### Comparing `spidermon-1.8.0/tests/test_data.py` & `spidermon-1.9.0/tests/test_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 from __future__ import absolute_import
 import pytest
 
 from spidermon.data import Data
 from spidermon.exceptions import InvalidDataOperation
 
+
 @pytest.fixture
 def data():
     return Data(item_scraped_count=150)
 
 
 def test_attribute_access(data):
-    assert(data['item_scraped_count'] == 150)
+    assert data["item_scraped_count"] == 150
 
 
 def test_dictionary_access(data):
-    assert(data.item_scraped_count == 150)
+    assert data.item_scraped_count == 150
 
 
 def test_attribute_set(data):
     with pytest.raises(InvalidDataOperation):
-        data.item_scraped_count = 'some value'
+        data.item_scraped_count = "some value"
 
 
 def test_dictionary_set(data):
     with pytest.raises(InvalidDataOperation):
-        data['item_scraped_count'] = 'some value'
+        data["item_scraped_count"] = "some value"
 
 
 def test_delete(data):
     with pytest.raises(InvalidDataOperation):
-        del data['item_scraped_count']
+        del data["item_scraped_count"]
 
 
 def test_pop(data):
     with pytest.raises(InvalidDataOperation):
-        data.pop('item_scraped_count', None)
+        data.pop("item_scraped_count", None)
 
 
 def test_clear(data):
     with pytest.raises(InvalidDataOperation):
         data.clear()
 
 
 def test_update(data):
     with pytest.raises(InvalidDataOperation):
-        data.update({'item_scraped_count': 0})
+        data.update({"item_scraped_count": 0})
 
 
 def test_setdefault(data):
     with pytest.raises(InvalidDataOperation):
-        data.setdefault('another_value', 0)
+        data.setdefault("another_value", 0)
```

### Comparing `spidermon-1.8.0/tests/test_levels.py` & `spidermon-1.9.0/tests/test_levels.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,99 +9,82 @@
 
 
 LEVEL_TESTS = [
     # ---------------------------------------------------------------------------------------
     # suite                     monitor/methods                                expected level
     # ---------------------------------------------------------------------------------------
     # Suite No Level
-    (Suites.NoLevelSuite,       Monitors.NoLevelMonitor.NoLevelMethod,         NORMAL),
-    (Suites.NoLevelSuite,       Monitors.NoLevelMonitor.HighLevelMethod,       HIGH),
-    (Suites.NoLevelSuite,       Monitors.NoLevelMonitor.NormalLevelMethod,     NORMAL),
-    (Suites.NoLevelSuite,       Monitors.NoLevelMonitor.LowLevelMethod,        LOW),
-
-    (Suites.NoLevelSuite,       Monitors.HighLevelMonitor.NoLevelMethod,       HIGH),
-    (Suites.NoLevelSuite,       Monitors.HighLevelMonitor.HighLevelMethod,     HIGH),
-    (Suites.NoLevelSuite,       Monitors.HighLevelMonitor.NormalLevelMethod,   NORMAL),
-    (Suites.NoLevelSuite,       Monitors.HighLevelMonitor.LowLevelMethod,      LOW),
-
-    (Suites.NoLevelSuite,       Monitors.NormalLevelMonitor.NoLevelMethod,     NORMAL),
-    (Suites.NoLevelSuite,       Monitors.NormalLevelMonitor.HighLevelMethod,   HIGH),
-    (Suites.NoLevelSuite,       Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
-    (Suites.NoLevelSuite,       Monitors.NormalLevelMonitor.LowLevelMethod,    LOW),
-
-    (Suites.NoLevelSuite,       Monitors.LowLevelMonitor.NoLevelMethod,        LOW),
-    (Suites.NoLevelSuite,       Monitors.LowLevelMonitor.HighLevelMethod,      HIGH),
-    (Suites.NoLevelSuite,       Monitors.LowLevelMonitor.NormalLevelMethod,    NORMAL),
-    (Suites.NoLevelSuite,       Monitors.LowLevelMonitor.LowLevelMethod,       LOW),
-
+    (Suites.NoLevelSuite, Monitors.NoLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.NoLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NoLevelSuite, Monitors.NoLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.NoLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NoLevelSuite, Monitors.HighLevelMonitor.NoLevelMethod, HIGH),
+    (Suites.NoLevelSuite, Monitors.HighLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NoLevelSuite, Monitors.HighLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.HighLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NoLevelSuite, Monitors.NormalLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.NormalLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NoLevelSuite, Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.NormalLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NoLevelSuite, Monitors.LowLevelMonitor.NoLevelMethod, LOW),
+    (Suites.NoLevelSuite, Monitors.LowLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NoLevelSuite, Monitors.LowLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NoLevelSuite, Monitors.LowLevelMonitor.LowLevelMethod, LOW),
     # Suite High
-    (Suites.HighLevelSuite,     Monitors.NoLevelMonitor.NoLevelMethod,         HIGH),
-    (Suites.HighLevelSuite,     Monitors.NoLevelMonitor.HighLevelMethod,       HIGH),
-    (Suites.HighLevelSuite,     Monitors.NoLevelMonitor.NormalLevelMethod,     NORMAL),
-    (Suites.HighLevelSuite,     Monitors.NoLevelMonitor.LowLevelMethod,        LOW),
-
-    (Suites.HighLevelSuite,     Monitors.HighLevelMonitor.NoLevelMethod,       HIGH),
-    (Suites.HighLevelSuite,     Monitors.HighLevelMonitor.HighLevelMethod,     HIGH),
-    (Suites.HighLevelSuite,     Monitors.HighLevelMonitor.NormalLevelMethod,   NORMAL),
-    (Suites.HighLevelSuite,     Monitors.HighLevelMonitor.LowLevelMethod,      LOW),
-
-    (Suites.HighLevelSuite,     Monitors.NormalLevelMonitor.NoLevelMethod,     NORMAL),
-    (Suites.HighLevelSuite,     Monitors.NormalLevelMonitor.HighLevelMethod,   HIGH),
-    (Suites.HighLevelSuite,     Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
-    (Suites.HighLevelSuite,     Monitors.NormalLevelMonitor.LowLevelMethod,    LOW),
-
-    (Suites.HighLevelSuite,     Monitors.LowLevelMonitor.NoLevelMethod,        LOW),
-    (Suites.HighLevelSuite,     Monitors.LowLevelMonitor.HighLevelMethod,      HIGH),
-    (Suites.HighLevelSuite,     Monitors.LowLevelMonitor.NormalLevelMethod,    NORMAL),
-    (Suites.HighLevelSuite,     Monitors.LowLevelMonitor.LowLevelMethod,       LOW),
-
+    (Suites.HighLevelSuite, Monitors.NoLevelMonitor.NoLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.NoLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.NoLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.HighLevelSuite, Monitors.NoLevelMonitor.LowLevelMethod, LOW),
+    (Suites.HighLevelSuite, Monitors.HighLevelMonitor.NoLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.HighLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.HighLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.HighLevelSuite, Monitors.HighLevelMonitor.LowLevelMethod, LOW),
+    (Suites.HighLevelSuite, Monitors.NormalLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.HighLevelSuite, Monitors.NormalLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.HighLevelSuite, Monitors.NormalLevelMonitor.LowLevelMethod, LOW),
+    (Suites.HighLevelSuite, Monitors.LowLevelMonitor.NoLevelMethod, LOW),
+    (Suites.HighLevelSuite, Monitors.LowLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.HighLevelSuite, Monitors.LowLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.HighLevelSuite, Monitors.LowLevelMonitor.LowLevelMethod, LOW),
     # Suite Normal
-    (Suites.NormalLevelSuite,   Monitors.NoLevelMonitor.NoLevelMethod,         NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.NoLevelMonitor.HighLevelMethod,       HIGH),
-    (Suites.NormalLevelSuite,   Monitors.NoLevelMonitor.NormalLevelMethod,     NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.NoLevelMonitor.LowLevelMethod,        LOW),
-
-    (Suites.NormalLevelSuite,   Monitors.HighLevelMonitor.NoLevelMethod,       HIGH),
-    (Suites.NormalLevelSuite,   Monitors.HighLevelMonitor.HighLevelMethod,     HIGH),
-    (Suites.NormalLevelSuite,   Monitors.HighLevelMonitor.NormalLevelMethod,   NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.HighLevelMonitor.LowLevelMethod,      LOW),
-
-    (Suites.NormalLevelSuite,   Monitors.NormalLevelMonitor.NoLevelMethod,     NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.NormalLevelMonitor.HighLevelMethod,   HIGH),
-    (Suites.NormalLevelSuite,   Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.NormalLevelMonitor.LowLevelMethod,    LOW),
-
-    (Suites.NormalLevelSuite,   Monitors.LowLevelMonitor.NoLevelMethod,        LOW),
-    (Suites.NormalLevelSuite,   Monitors.LowLevelMonitor.HighLevelMethod,      HIGH),
-    (Suites.NormalLevelSuite,   Monitors.LowLevelMonitor.NormalLevelMethod,    NORMAL),
-    (Suites.NormalLevelSuite,   Monitors.LowLevelMonitor.LowLevelMethod,       LOW),
-
+    (Suites.NormalLevelSuite, Monitors.NoLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.NoLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NormalLevelSuite, Monitors.NoLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.NoLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NormalLevelSuite, Monitors.HighLevelMonitor.NoLevelMethod, HIGH),
+    (Suites.NormalLevelSuite, Monitors.HighLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NormalLevelSuite, Monitors.HighLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.HighLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NormalLevelSuite, Monitors.NormalLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.NormalLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NormalLevelSuite, Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.NormalLevelMonitor.LowLevelMethod, LOW),
+    (Suites.NormalLevelSuite, Monitors.LowLevelMonitor.NoLevelMethod, LOW),
+    (Suites.NormalLevelSuite, Monitors.LowLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.NormalLevelSuite, Monitors.LowLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.NormalLevelSuite, Monitors.LowLevelMonitor.LowLevelMethod, LOW),
     # Suite Low
-    (Suites.LowLevelSuite,      Monitors.NoLevelMonitor.NoLevelMethod,         LOW),
-    (Suites.LowLevelSuite,      Monitors.NoLevelMonitor.HighLevelMethod,       HIGH),
-    (Suites.LowLevelSuite,      Monitors.NoLevelMonitor.NormalLevelMethod,     NORMAL),
-    (Suites.LowLevelSuite,      Monitors.NoLevelMonitor.LowLevelMethod,        LOW),
-
-    (Suites.LowLevelSuite,      Monitors.HighLevelMonitor.NoLevelMethod,       HIGH),
-    (Suites.LowLevelSuite,      Monitors.HighLevelMonitor.HighLevelMethod,     HIGH),
-    (Suites.LowLevelSuite,      Monitors.HighLevelMonitor.NormalLevelMethod,   NORMAL),
-    (Suites.LowLevelSuite,      Monitors.HighLevelMonitor.LowLevelMethod,      LOW),
-
-    (Suites.LowLevelSuite,      Monitors.NormalLevelMonitor.NoLevelMethod,     NORMAL),
-    (Suites.LowLevelSuite,      Monitors.NormalLevelMonitor.HighLevelMethod,   HIGH),
-    (Suites.LowLevelSuite,      Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
-    (Suites.LowLevelSuite,      Monitors.NormalLevelMonitor.LowLevelMethod,    LOW),
-
-    (Suites.LowLevelSuite,      Monitors.LowLevelMonitor.NoLevelMethod,        LOW),
-    (Suites.LowLevelSuite,      Monitors.LowLevelMonitor.HighLevelMethod,      HIGH),
-    (Suites.LowLevelSuite,      Monitors.LowLevelMonitor.NormalLevelMethod,    NORMAL),
-    (Suites.LowLevelSuite,      Monitors.LowLevelMonitor.LowLevelMethod,       LOW),
+    (Suites.LowLevelSuite, Monitors.NoLevelMonitor.NoLevelMethod, LOW),
+    (Suites.LowLevelSuite, Monitors.NoLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.LowLevelSuite, Monitors.NoLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.LowLevelSuite, Monitors.NoLevelMonitor.LowLevelMethod, LOW),
+    (Suites.LowLevelSuite, Monitors.HighLevelMonitor.NoLevelMethod, HIGH),
+    (Suites.LowLevelSuite, Monitors.HighLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.LowLevelSuite, Monitors.HighLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.LowLevelSuite, Monitors.HighLevelMonitor.LowLevelMethod, LOW),
+    (Suites.LowLevelSuite, Monitors.NormalLevelMonitor.NoLevelMethod, NORMAL),
+    (Suites.LowLevelSuite, Monitors.NormalLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.LowLevelSuite, Monitors.NormalLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.LowLevelSuite, Monitors.NormalLevelMonitor.LowLevelMethod, LOW),
+    (Suites.LowLevelSuite, Monitors.LowLevelMonitor.NoLevelMethod, LOW),
+    (Suites.LowLevelSuite, Monitors.LowLevelMonitor.HighLevelMethod, HIGH),
+    (Suites.LowLevelSuite, Monitors.LowLevelMonitor.NormalLevelMethod, NORMAL),
+    (Suites.LowLevelSuite, Monitors.LowLevelMonitor.LowLevelMethod, LOW),
 ]
 
 
 def test_levels():
     for suite, monitor, expected_level in LEVEL_TESTS:
         suite = suite()
         suite.add_monitor(monitor)
         assert suite.all_monitors[0].level == expected_level
-
-
```

### Comparing `spidermon-1.8.0/tests/test_expressions.py` & `spidermon-1.9.0/tests/test_expressions.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,11 +28,12 @@
 
 def test_valid_expressions(interpreter):
     for expression in VALID_EXPRESSIONS:
         interpreter.check(expression)
 
 
 def test_evaluated_expressions(interpreter):
-    data = Data({'stats': Data(STATS_TO_EVALUATE)})
+    data = Data({"stats": Data(STATS_TO_EVALUATE)})
     for expression, result in EXPRESSIONS_TO_EVALUATE:
-        assert result == interpreter.eval(expression, data), \
-            'Expression fails: "%s" != %s' % (expression, result)
+        assert result == interpreter.eval(
+            expression, data
+        ), 'Expression fails: "%s" != %s' % (expression, result)
```

### Comparing `spidermon-1.8.0/tests/test_loaders.py` & `spidermon-1.9.0/tests/test_loaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,57 +12,41 @@
 def loader():
     return MonitorLoader()
 
 
 def test_loading(loader):
     check_suite(
         suite=loader.load_suite_from_monitor(EmptyMonitor),
-        expected_number_of_monitors=0
+        expected_number_of_monitors=0,
     )
     check_suite(
-        suite=loader.load_suite_from_monitor(Monitor01),
-        expected_number_of_monitors=3
+        suite=loader.load_suite_from_monitor(Monitor01), expected_number_of_monitors=3
     )
     check_suite(
-        suite=loader.load_suite_from_monitor(Monitor02),
-        expected_number_of_monitors=2
+        suite=loader.load_suite_from_monitor(Monitor02), expected_number_of_monitors=2
     )
 
 
 def test_loading_errors(loader):
     with pytest.raises(InvalidMonitor):
         loader.load_suite_from_monitor(None)
     with pytest.raises(InvalidMonitor):
         loader.load_suite_from_monitor(10)
     with pytest.raises(InvalidMonitor):
         loader.load_suite_from_monitor(object)
 
 
 def test_testcase_names(loader):
-    _check_testcase_names(
-        loader=loader,
-        monitor_class=EmptyMonitor,
-        expected_names=[]
-    )
+    _check_testcase_names(loader=loader, monitor_class=EmptyMonitor, expected_names=[])
     _check_testcase_names(
         loader=loader,
         monitor_class=Monitor01,
-        expected_names=[
-            'test_a',
-            'test_b',
-            'test_c',
-        ]
+        expected_names=["test_a", "test_b", "test_c"],
     )
     _check_testcase_names(
-        loader=loader,
-        monitor_class=Monitor02,
-        expected_names=[
-            'test_d',
-            'test_e',
-        ]
+        loader=loader, monitor_class=Monitor02, expected_names=["test_d", "test_e"]
     )
 
 
 def _check_testcase_names(loader, monitor_class, expected_names):
     names = loader.get_testcase_names(monitor_class)
     assert names == expected_names
-
```

### Comparing `spidermon-1.8.0/tests/test_names.py` & `spidermon-1.9.0/tests/test_names.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,206 +2,203 @@
 import pytest
 
 from .fixtures.names import *
 from six.moves import zip
 
 
 NAMES = [
-    'UnnamedMonitor/A Test',
-    'UnnamedMonitor/test_without_name',
-    'Class Monitor/A Test',
-    'Class Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'UnnamedMonitor/A Test',
-    'UnnamedMonitor/test_without_name',
-    'Class Monitor/A Test',
-    'Class Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'UnnamedMonitor/A Test',
-    'UnnamedMonitor/test_without_name',
-    'Class Monitor/A Test',
-    'Class Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'UnnamedMonitor/A Test',
-    'UnnamedMonitor/test_without_name',
-    'Class Monitor/A Test',
-    'Class Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
+    "UnnamedMonitor/A Test",
+    "UnnamedMonitor/test_without_name",
+    "Class Monitor/A Test",
+    "Class Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "UnnamedMonitor/A Test",
+    "UnnamedMonitor/test_without_name",
+    "Class Monitor/A Test",
+    "Class Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "UnnamedMonitor/A Test",
+    "UnnamedMonitor/test_without_name",
+    "Class Monitor/A Test",
+    "Class Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "UnnamedMonitor/A Test",
+    "UnnamedMonitor/test_without_name",
+    "Class Monitor/A Test",
+    "Class Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
 ]
 
 MONITOR_NAMES = [
-    'UnnamedMonitor',
-    'UnnamedMonitor',
-    'Class Monitor',
-    'Class Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'UnnamedMonitor',
-    'UnnamedMonitor',
-    'Class Monitor',
-    'Class Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'UnnamedMonitor',
-    'UnnamedMonitor',
-    'Class Monitor',
-    'Class Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'UnnamedMonitor',
-    'UnnamedMonitor',
-    'Class Monitor',
-    'Class Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
-    'Instance Monitor',
+    "UnnamedMonitor",
+    "UnnamedMonitor",
+    "Class Monitor",
+    "Class Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "UnnamedMonitor",
+    "UnnamedMonitor",
+    "Class Monitor",
+    "Class Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "UnnamedMonitor",
+    "UnnamedMonitor",
+    "Class Monitor",
+    "Class Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "UnnamedMonitor",
+    "UnnamedMonitor",
+    "Class Monitor",
+    "Class Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
+    "Instance Monitor",
 ]
 
 METHOD_NAMES = [
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
-    'A Test',
-    'test_without_name',
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
+    "A Test",
+    "test_without_name",
 ]
 
 FULL_NAMES_UNNNAMED_SUITE = [
-    'UnnamedMonitor/A Test',
-    'UnnamedMonitor/test_without_name',
-    'Class Monitor/A Test',
-    'Class Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'Instance Monitor/A Test',
-    'Instance Monitor/test_without_name',
-    'The Child Suite/UnnamedMonitor/A Test',
-    'The Child Suite/UnnamedMonitor/test_without_name',
-    'The Child Suite/Class Monitor/A Test',
-    'The Child Suite/Class Monitor/test_without_name',
-    'The Child Suite/Instance Monitor/A Test',
-    'The Child Suite/Instance Monitor/test_without_name',
-    'The Child Suite/Instance Monitor/A Test',
-    'The Child Suite/Instance Monitor/test_without_name',
-    'Instance Suite Name/UnnamedMonitor/A Test',
-    'Instance Suite Name/UnnamedMonitor/test_without_name',
-    'Instance Suite Name/Class Monitor/A Test',
-    'Instance Suite Name/Class Monitor/test_without_name',
-    'Instance Suite Name/Instance Monitor/A Test',
-    'Instance Suite Name/Instance Monitor/test_without_name',
-    'Instance Suite Name/Instance Monitor/A Test',
-    'Instance Suite Name/Instance Monitor/test_without_name',
-    'Instance Suite Name/UnnamedMonitor/A Test',
-    'Instance Suite Name/UnnamedMonitor/test_without_name',
-    'Instance Suite Name/Class Monitor/A Test',
-    'Instance Suite Name/Class Monitor/test_without_name',
-    'Instance Suite Name/Instance Monitor/A Test',
-    'Instance Suite Name/Instance Monitor/test_without_name',
-    'Instance Suite Name/Instance Monitor/A Test',
-    'Instance Suite Name/Instance Monitor/test_without_name',
+    "UnnamedMonitor/A Test",
+    "UnnamedMonitor/test_without_name",
+    "Class Monitor/A Test",
+    "Class Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "Instance Monitor/A Test",
+    "Instance Monitor/test_without_name",
+    "The Child Suite/UnnamedMonitor/A Test",
+    "The Child Suite/UnnamedMonitor/test_without_name",
+    "The Child Suite/Class Monitor/A Test",
+    "The Child Suite/Class Monitor/test_without_name",
+    "The Child Suite/Instance Monitor/A Test",
+    "The Child Suite/Instance Monitor/test_without_name",
+    "The Child Suite/Instance Monitor/A Test",
+    "The Child Suite/Instance Monitor/test_without_name",
+    "Instance Suite Name/UnnamedMonitor/A Test",
+    "Instance Suite Name/UnnamedMonitor/test_without_name",
+    "Instance Suite Name/Class Monitor/A Test",
+    "Instance Suite Name/Class Monitor/test_without_name",
+    "Instance Suite Name/Instance Monitor/A Test",
+    "Instance Suite Name/Instance Monitor/test_without_name",
+    "Instance Suite Name/Instance Monitor/A Test",
+    "Instance Suite Name/Instance Monitor/test_without_name",
+    "Instance Suite Name/UnnamedMonitor/A Test",
+    "Instance Suite Name/UnnamedMonitor/test_without_name",
+    "Instance Suite Name/Class Monitor/A Test",
+    "Instance Suite Name/Class Monitor/test_without_name",
+    "Instance Suite Name/Instance Monitor/A Test",
+    "Instance Suite Name/Instance Monitor/test_without_name",
+    "Instance Suite Name/Instance Monitor/A Test",
+    "Instance Suite Name/Instance Monitor/test_without_name",
 ]
 
 FULL_NAMES_NAMED_SUITE = [
-    'The Top Suite/UnnamedMonitor/A Test',
-    'The Top Suite/UnnamedMonitor/test_without_name',
-    'The Top Suite/Class Monitor/A Test',
-    'The Top Suite/Class Monitor/test_without_name',
-    'The Top Suite/Instance Monitor/A Test',
-    'The Top Suite/Instance Monitor/test_without_name',
-    'The Top Suite/Instance Monitor/A Test',
-    'The Top Suite/Instance Monitor/test_without_name',
-    'The Top Suite/The Child Suite/UnnamedMonitor/A Test',
-    'The Top Suite/The Child Suite/UnnamedMonitor/test_without_name',
-    'The Top Suite/The Child Suite/Class Monitor/A Test',
-    'The Top Suite/The Child Suite/Class Monitor/test_without_name',
-    'The Top Suite/The Child Suite/Instance Monitor/A Test',
-    'The Top Suite/The Child Suite/Instance Monitor/test_without_name',
-    'The Top Suite/The Child Suite/Instance Monitor/A Test',
-    'The Top Suite/The Child Suite/Instance Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/UnnamedMonitor/A Test',
-    'The Top Suite/Instance Suite Name/UnnamedMonitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Class Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Class Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Instance Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Instance Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Instance Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Instance Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/UnnamedMonitor/A Test',
-    'The Top Suite/Instance Suite Name/UnnamedMonitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Class Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Class Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Instance Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Instance Monitor/test_without_name',
-    'The Top Suite/Instance Suite Name/Instance Monitor/A Test',
-    'The Top Suite/Instance Suite Name/Instance Monitor/test_without_name',
+    "The Top Suite/UnnamedMonitor/A Test",
+    "The Top Suite/UnnamedMonitor/test_without_name",
+    "The Top Suite/Class Monitor/A Test",
+    "The Top Suite/Class Monitor/test_without_name",
+    "The Top Suite/Instance Monitor/A Test",
+    "The Top Suite/Instance Monitor/test_without_name",
+    "The Top Suite/Instance Monitor/A Test",
+    "The Top Suite/Instance Monitor/test_without_name",
+    "The Top Suite/The Child Suite/UnnamedMonitor/A Test",
+    "The Top Suite/The Child Suite/UnnamedMonitor/test_without_name",
+    "The Top Suite/The Child Suite/Class Monitor/A Test",
+    "The Top Suite/The Child Suite/Class Monitor/test_without_name",
+    "The Top Suite/The Child Suite/Instance Monitor/A Test",
+    "The Top Suite/The Child Suite/Instance Monitor/test_without_name",
+    "The Top Suite/The Child Suite/Instance Monitor/A Test",
+    "The Top Suite/The Child Suite/Instance Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/UnnamedMonitor/A Test",
+    "The Top Suite/Instance Suite Name/UnnamedMonitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Class Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Class Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Instance Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Instance Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Instance Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Instance Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/UnnamedMonitor/A Test",
+    "The Top Suite/Instance Suite Name/UnnamedMonitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Class Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Class Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Instance Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Instance Monitor/test_without_name",
+    "The Top Suite/Instance Suite Name/Instance Monitor/A Test",
+    "The Top Suite/Instance Suite Name/Instance Monitor/test_without_name",
 ]
 
 
 @pytest.fixture
 def named_top_suite():
     return NamedTopSuite()
 
+
 @pytest.fixture
 def unnamed_top_suite():
     return UnnamedTopSuite()
 
 
 def test_names(named_top_suite, unnamed_top_suite):
+    _check_names(generated_names=_generate_names(named_top_suite), expected_names=NAMES)
     _check_names(
-        generated_names=_generate_names(named_top_suite),
-        expected_names=NAMES,
-    )
-    _check_names(
-        generated_names=_generate_names(unnamed_top_suite),
-        expected_names=NAMES,
+        generated_names=_generate_names(unnamed_top_suite), expected_names=NAMES
     )
 
 
 def test_monitor_names(named_top_suite, unnamed_top_suite):
     _check_names(
         generated_names=_generate_monitor_names(named_top_suite),
         expected_names=MONITOR_NAMES,
```

### Comparing `spidermon-1.8.0/tests/test_ordering.py` & `spidermon-1.9.0/tests/test_ordering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,73 @@
 from __future__ import absolute_import
 from .fixtures.ordering import *
 
 SUITE_SEQUENCES = [
     # ------------------------------------------------------------------------------------------------------------
     # monitor sequence                                      expected sequence
     # ------------------------------------------------------------------------------------------------------------
-
     # Unordered: should follow same insertion order (FIFO)
-    ([Unordered.A, Unordered.B],                            [Unordered.A, Unordered.B]),
-    ([Unordered.B, Unordered.A],                            [Unordered.B, Unordered.A]),
-    ([Unordered.C, Unordered.D],                            [Unordered.C, Unordered.D]),
-    ([Unordered.D, Unordered.C],                            [Unordered.D, Unordered.C]),
-    ([Unordered.A, Unordered.B, Unordered.C, Unordered.D],  [Unordered.A, Unordered.B, Unordered.C, Unordered.D]),
-    ([Unordered.D, Unordered.C, Unordered.B, Unordered.A],  [Unordered.D, Unordered.C, Unordered.B, Unordered.A]),
-    ([Unordered.C, Unordered.B, Unordered.A, Unordered.D],  [Unordered.C, Unordered.B, Unordered.A, Unordered.D]),
-    ([Unordered.A, Unordered.A, Unordered.B, Unordered.B],  [Unordered.A, Unordered.A, Unordered.B, Unordered.B]),
-    ([Unordered.C, Unordered.C, Unordered.B, Unordered.B],  [Unordered.C, Unordered.C, Unordered.B, Unordered.B]),
-
+    ([Unordered.A, Unordered.B], [Unordered.A, Unordered.B]),
+    ([Unordered.B, Unordered.A], [Unordered.B, Unordered.A]),
+    ([Unordered.C, Unordered.D], [Unordered.C, Unordered.D]),
+    ([Unordered.D, Unordered.C], [Unordered.D, Unordered.C]),
+    (
+        [Unordered.A, Unordered.B, Unordered.C, Unordered.D],
+        [Unordered.A, Unordered.B, Unordered.C, Unordered.D],
+    ),
+    (
+        [Unordered.D, Unordered.C, Unordered.B, Unordered.A],
+        [Unordered.D, Unordered.C, Unordered.B, Unordered.A],
+    ),
+    (
+        [Unordered.C, Unordered.B, Unordered.A, Unordered.D],
+        [Unordered.C, Unordered.B, Unordered.A, Unordered.D],
+    ),
+    (
+        [Unordered.A, Unordered.A, Unordered.B, Unordered.B],
+        [Unordered.A, Unordered.A, Unordered.B, Unordered.B],
+    ),
+    (
+        [Unordered.C, Unordered.C, Unordered.B, Unordered.B],
+        [Unordered.C, Unordered.C, Unordered.B, Unordered.B],
+    ),
     # Ordered: should follow decorators order (A, B, C, D)
-    ([Ordered.A, Ordered.B],                                [Ordered.A, Ordered.B]),
-    ([Ordered.B, Ordered.A],                                [Ordered.A, Ordered.B]),
-    ([Ordered.C, Ordered.D],                                [Ordered.C, Ordered.D]),
-    ([Ordered.D, Ordered.C],                                [Ordered.C, Ordered.D]),
-    ([Ordered.A, Ordered.B, Ordered.C, Ordered.D],          [Ordered.A, Ordered.B, Ordered.C, Ordered.D]),
-    ([Ordered.D, Ordered.C, Ordered.B, Ordered.A],          [Ordered.A, Ordered.B, Ordered.C, Ordered.D]),
-    ([Ordered.C, Ordered.B, Ordered.A, Ordered.D],          [Ordered.A, Ordered.B, Ordered.C, Ordered.D]),
-    ([Ordered.A, Ordered.A, Ordered.B, Ordered.B],          [Ordered.A, Ordered.A, Ordered.B, Ordered.B]),
-    ([Ordered.C, Ordered.C, Ordered.B, Ordered.B],          [Ordered.B, Ordered.B, Ordered.C, Ordered.C]),
+    ([Ordered.A, Ordered.B], [Ordered.A, Ordered.B]),
+    ([Ordered.B, Ordered.A], [Ordered.A, Ordered.B]),
+    ([Ordered.C, Ordered.D], [Ordered.C, Ordered.D]),
+    ([Ordered.D, Ordered.C], [Ordered.C, Ordered.D]),
+    (
+        [Ordered.A, Ordered.B, Ordered.C, Ordered.D],
+        [Ordered.A, Ordered.B, Ordered.C, Ordered.D],
+    ),
+    (
+        [Ordered.D, Ordered.C, Ordered.B, Ordered.A],
+        [Ordered.A, Ordered.B, Ordered.C, Ordered.D],
+    ),
+    (
+        [Ordered.C, Ordered.B, Ordered.A, Ordered.D],
+        [Ordered.A, Ordered.B, Ordered.C, Ordered.D],
+    ),
+    (
+        [Ordered.A, Ordered.A, Ordered.B, Ordered.B],
+        [Ordered.A, Ordered.A, Ordered.B, Ordered.B],
+    ),
+    (
+        [Ordered.C, Ordered.C, Ordered.B, Ordered.B],
+        [Ordered.B, Ordered.B, Ordered.C, Ordered.C],
+    ),
 ]
 
 METHOD_SEQUENCES = [
     # --------------------------------------------------------------
     # monitor class                 expected methods sequence
     # --------------------------------------------------------------
-    (UnorderedMethodsMonitor,       ['test_a', 'test_b', 'test_c']),
-    (OrderedMethodsMonitor,         ['test_c', 'test_b', 'test_a']),
-    (EqualOrderedMethodsMonitor,    ['test_a', 'test_b', 'test_c']),
+    (UnorderedMethodsMonitor, ["test_a", "test_b", "test_c"]),
+    (OrderedMethodsMonitor, ["test_c", "test_b", "test_a"]),
+    (EqualOrderedMethodsMonitor, ["test_a", "test_b", "test_c"]),
 ]
 
 
 def test_suite_ordering():
     for monitors_sequence, expected_sequence in SUITE_SEQUENCES:
         suite = MonitorSuite()
         suite.add_monitors(monitors_sequence)
```

### Comparing `spidermon-1.8.0/spidermon/utils/text.py` & `spidermon-1.9.0/spidermon/utils/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 DEFAULT_LINE_LENGTH = 70
-DEFAULT_LINE_CHAR = '-'
-DEFAULT_LINE_BOLD_CHAR = '='
-DEFAULT_LINE_LIGHT_CHAR = '-'
+DEFAULT_LINE_CHAR = "-"
+DEFAULT_LINE_BOLD_CHAR = "="
+DEFAULT_LINE_LIGHT_CHAR = "-"
 
 
 def line(length=DEFAULT_LINE_LENGTH, char=DEFAULT_LINE_CHAR):
-    return char*length
+    return char * length
 
 
 def line_title(title, length=DEFAULT_LINE_LENGTH, char=DEFAULT_LINE_CHAR):
-    title_length = len(title)+2
-    left_length = (length-title_length)//2
+    title_length = len(title) + 2
+    left_length = (length - title_length) // 2
     right_length = left_length + length - title_length - left_length * 2
-    return '%s %s %s' % (char*left_length, title, char*right_length)
+    return "%s %s %s" % (char * left_length, title, char * right_length)
 
 
 class Message(object):
     def __init__(self, text=None):
-        self.msg = text or ''
+        self.msg = text or ""
 
     def write(self, text):
         self.msg += text
 
     def write_line(self, text=None):
-        self.msg += '%s\n' % (text or '')
+        self.msg += "%s\n" % (text or "")
 
     def write_separator(self, length=DEFAULT_LINE_LENGTH, char=DEFAULT_LINE_CHAR):
         self.write_line(line(length=length, char=char))
 
     def write_bold_separator(self, length=DEFAULT_LINE_LENGTH):
         self.write_separator(length=length, char=DEFAULT_LINE_BOLD_CHAR)
```

### Comparing `spidermon-1.8.0/spidermon/utils/hubstorage.py` & `spidermon-1.9.0/spidermon/utils/hubstorage.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,48 +3,50 @@
 """
 from __future__ import absolute_import
 import os
 from codecs import decode
 
 import six
 from six.moves import map
+
 try:
     try:
         from scrapinghub import HubstorageClient
     except ImportError:
         from hubstorage.client import HubstorageClient
 except ImportError:
     HubstorageClient = None
 
 
 class _Hubstorage(object):
-
     def __init__(self):
-        self.available = 'SHUB_JOBKEY' in os.environ and HubstorageClient is not None
+        self.available = "SHUB_JOBKEY" in os.environ and HubstorageClient is not None
         self._client = None
         self._project = None
         self._job = None
         if self.available:
-            self.job_key = os.environ['SHUB_JOBKEY']
-            self._project_id, self._spider_id, self._job_id = map(int, self.job_key.split('/'))
+            self.job_key = os.environ["SHUB_JOBKEY"]
+            self._project_id, self._spider_id, self._job_id = map(
+                int, self.job_key.split("/")
+            )
         else:
             self._project_id = None
             self._spider_id = None
             self._job_id = None
 
     @property
     def auth(self):
         if six.PY2:
-            return os.environ['SHUB_JOBAUTH'].decode('hex')
+            return os.environ["SHUB_JOBAUTH"].decode("hex")
         else:
-            return decode(os.environ['SHUB_JOBAUTH'], 'hex_codec').decode('utf-8')
+            return decode(os.environ["SHUB_JOBAUTH"], "hex_codec").decode("utf-8")
 
     @property
     def endpoint(self):
-        return os.environ.get('SHUB_STORAGE')
+        return os.environ.get("SHUB_STORAGE")
 
     @property
     def project_id(self):
         return self._project_id
 
     @property
     def spider_id(self):
@@ -53,16 +55,15 @@
     @property
     def job_id(self):
         return self._job_id
 
     @property
     def client(self):
         if self._client is None:
-            self._client = HubstorageClient(endpoint=self.endpoint,
-                                            auth=self.auth)
+            self._client = HubstorageClient(endpoint=self.endpoint, auth=self.auth)
         return self._client
 
     @property
     def project(self):
         if self._project is None:
             self._project = self.client.get_project(str(self.project_id))
         return self._project
```

### Comparing `spidermon-1.8.0/spidermon/core/options.py` & `spidermon-1.9.0/spidermon/core/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,41 @@
 
 class OptionsMetaclassBase(abc.ABCMeta):
     __options_class__ = None
 
     def __new__(mcs, name, bases, attrs):
         cls = super(OptionsMetaclassBase, mcs).__new__(mcs, name, bases, attrs)
         if not cls.__options_class__:
-            raise TypeError('Options class not defined! '
-                            'are you trying to use OptionsMetaclassBase?')
+            raise TypeError(
+                "Options class not defined! "
+                "are you trying to use OptionsMetaclassBase?"
+            )
         cls.options = cls.__options_class__()
         return cls
 
 
 class OptionsBase(object):
-    __options_name__ = 'options'
+    __options_name__ = "options"
 
     @classmethod
     def add_or_create(cls, target):
         if not hasattr(target, cls.__options_name__):
             setattr(target, cls.__options_name__, cls())
             return True
         return False
 
     def _get_attributes(self):
-        return dict([(k, v) for k, v in self.__dict__.items()
-                     if not k.startswith('_')])
+        return dict([(k, v) for k, v in self.__dict__.items() if not k.startswith("_")])
 
     def __str__(self):
-        return '<{name}:({attributes})>'.format(
+        return "<{name}:({attributes})>".format(
             name=self.__class__.__name__,
-            attributes=', '.join('%s=%s' % (attr, getattr(self, attr))
-                                 for attr in self._get_attributes())
+            attributes=", ".join(
+                "%s=%s" % (attr, getattr(self, attr)) for attr in self._get_attributes()
+            ),
         )
 
 
 class MonitorOptions(OptionsBase):
     def __init__(self):
         self.name = settings.MONITOR.DEFAULT_NAME
         self.description = settings.MONITOR.DEFAULT_DESCRIPTION
```

### Comparing `spidermon-1.8.0/spidermon/core/monitors.py` & `spidermon-1.9.0/spidermon/core/monitors.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,82 +4,85 @@
 from spidermon.data import Data
 from spidermon import settings
 from .options import MonitorOptions, MonitorOptionsMetaclass
 import six
 
 
 class Monitor(six.with_metaclass(MonitorOptionsMetaclass, TestCase)):
-    def __init__(self, methodName='runTest', name=None):
+    def __init__(self, methodName="runTest", name=None):
         super(Monitor, self).__init__(methodName)
         self._name = name
         self._data = None
         self._parent = None
         self._init_method()
 
     @property
     def name(self):
-        return '/'.join([self.monitor_name, self.method_name])
+        return "/".join([self.monitor_name, self.method_name])
 
     @property
     def full_name(self):
         parts = []
         if self.parent and self.parent.full_name:
             parts.append(self.parent.full_name)
         parts.append(self.name)
-        return '/'.join(parts)
+        return "/".join(parts)
 
     @property
     def level(self):
-        return self.method_level or \
-               self.monitor_level or \
-               self.parent_level or \
-               settings.MONITOR.LEVELS.DEFAULT
+        return (
+            self.method_level
+            or self.monitor_level
+            or self.parent_level
+            or settings.MONITOR.LEVELS.DEFAULT
+        )
 
     @property
     def order(self):
         return self.method.options.order
 
     @property
     def monitor_name(self):
-        return self._name or \
-               self.options.name or \
-               self.__class__.__name__
+        return self._name or self.options.name or self.__class__.__name__
 
     @property
     def monitor_full_name(self):
         parts = []
         if self.parent and self.parent.full_name:
             parts.append(self.parent.full_name)
         parts.append(self.monitor_name)
-        return '/'.join(parts)
+        return "/".join(parts)
 
     @property
     def monitor_description(self):
-        return self.options.description or \
-               self.__class__.__doc__ or \
-               settings.MONITOR.DEFAULT_DESCRIPTION
+        return (
+            self.options.description
+            or self.__class__.__doc__
+            or settings.MONITOR.DEFAULT_DESCRIPTION
+        )
 
     @property
     def monitor_level(self):
         return self.options.level
 
     @property
     def method(self):
         return getattr(self, self._testMethodName)
 
     @property
     def method_name(self):
-        return self.method.options.name or \
-               self._testMethodName
+        return self.method.options.name or self._testMethodName
 
     @property
     def method_description(self):
-        return self.method.options.description or \
-               self.method.__func__.__doc__ or \
-               settings.MONITOR.DEFAULT_DESCRIPTION
+        return (
+            self.method.options.description
+            or self.method.__func__.__doc__
+            or settings.MONITOR.DEFAULT_DESCRIPTION
+        )
 
     @property
     def method_level(self):
         return self.method.options.level
 
     @property
     def parent(self):
@@ -92,20 +95,20 @@
     def set_parent(self, parent):
         self._parent = parent
 
     def init_data(self, data):
         self.data = data
 
     def debug_tree(self, level=0):
-        return level*'\t' + repr(self) + '\n'
+        return level * "\t" + repr(self) + "\n"
 
     def _init_method(self):
         MonitorOptions.add_or_create(self.method.__func__)
 
     def __repr__(self):
-        return '<MONITOR:(%s) at %s>' % (self.name, hex(id(self)))
+        return "<MONITOR:(%s) at %s>" % (self.name, hex(id(self)))
 
     def __str__(self):
         return self.name
 
     def __hash__(self):
         return hash(id(self))
```

### Comparing `spidermon-1.8.0/spidermon/core/actions.py` & `spidermon-1.9.0/spidermon/core/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         return {}
 
     @property
     def name(self):
-        return self.options.name or \
-               self.__class__.__name__
+        return self.options.name or self.__class__.__name__
 
     def run(self, result, data):
         self.result = result
         self.data = data
         result.start_action(self)
         try:
             self.run_action()
@@ -56,15 +55,15 @@
     def monitors_failed(self):
         return len(self.result.monitors_failed_results) > 0
 
     def get_meta(self):
         return {}
 
     def __repr__(self):
-        return '<ACTION:(%s) at %s>' % (self.name, hex(id(self)))
+        return "<ACTION:(%s) at %s>" % (self.name, hex(id(self)))
 
     def __str__(self):
         return repr(self)
 
 
 class DummyAction(Action):
     def run_action(self):
```

### Comparing `spidermon-1.8.0/spidermon/core/factories.py` & `spidermon-1.9.0/spidermon/core/factories.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from __future__ import absolute_import
 import six
 
 import inspect
 
-from spidermon.exceptions import (InvalidMonitor, InvalidMonitorClass, InvalidMonitorTuple)
+from spidermon.exceptions import (
+    InvalidMonitor,
+    InvalidMonitorClass,
+    InvalidMonitorTuple,
+)
 from .monitors import Monitor
 from .actions import Action
 
 
 class MonitorFactory(object):
     @classmethod
     def load_monitor(cls, monitor, name=None):
         from .suites import MonitorSuite
+
         if inspect.isclass(monitor):
             return cls.load_monitor_from_class(monitor_class=monitor, name=name)
         elif isinstance(monitor, tuple):
             return cls.load_monitor_from_tuple(monitor_tuple=monitor)
         elif isinstance(monitor, (Monitor, MonitorSuite)):
             return monitor
         cls.raise_invalid_monitor()
 
     @classmethod
     def load_monitor_from_class(cls, monitor_class, name=None):
         from .suites import MonitorSuite
+
         if issubclass(monitor_class, Monitor):
             from spidermon.loaders import MonitorLoader
+
             loader = MonitorLoader()
-            monitor = loader.load_suite_from_monitor(monitor_class=monitor_class, name=name)
+            monitor = loader.load_suite_from_monitor(
+                monitor_class=monitor_class, name=name
+            )
         elif issubclass(monitor_class, MonitorSuite):
             monitor = monitor_class(name=name)
         else:
             cls.raise_invalid_class()
         return cls.load_monitor(monitor=monitor, name=name)
 
     @classmethod
@@ -40,29 +49,35 @@
         name, monitor = monitor_tuple
         if not isinstance(name, six.string_types):
             cls.raise_invalid_tuple()
         return cls.load_monitor(monitor=monitor, name=name)
 
     @classmethod
     def raise_invalid_monitor(cls):
-        raise InvalidMonitor('Wrong Monitor definition, it should be:\n'
-                             '- an instance of a Monitor/MonitorSuite object.\n'
-                             '- a subclass of Monitor/MonitorSuite.\n'
-                             '- a tuple with the format (name, monitor).\n'
-                             '- a string containing an evaluable python expression.')
+        raise InvalidMonitor(
+            "Wrong Monitor definition, it should be:\n"
+            "- an instance of a Monitor/MonitorSuite object.\n"
+            "- a subclass of Monitor/MonitorSuite.\n"
+            "- a tuple with the format (name, monitor).\n"
+            "- a string containing an evaluable python expression."
+        )
 
     @classmethod
     def raise_invalid_class(cls):
-        raise InvalidMonitorClass('Wrong Monitor class definition, it should be '
-                                  'an instance of a Monitor/MonitorSuite object.')
+        raise InvalidMonitorClass(
+            "Wrong Monitor class definition, it should be "
+            "an instance of a Monitor/MonitorSuite object."
+        )
 
     @classmethod
     def raise_invalid_tuple(cls):
-        raise InvalidMonitorTuple('Wrong Monitor tuple definition, it should be '
-                                  'a tuple with the format (name, monitor)')
+        raise InvalidMonitorTuple(
+            "Wrong Monitor tuple definition, it should be "
+            "a tuple with the format (name, monitor)"
+        )
 
 
 class ActionFactory(object):
     @classmethod
     def load_action(cls, action, crawler=None):
         if inspect.isclass(action):
             return cls.load_action_from_class(action_class=action, crawler=crawler)
@@ -70,27 +85,30 @@
             return action
         cls.raise_invalid_action()
 
     @classmethod
     def load_action_from_class(cls, action_class, crawler=None):
         if not issubclass(action_class, Action):
             cls.raise_invalid_class()
-        if crawler and hasattr(action_class, 'from_crawler'):
+        if crawler and hasattr(action_class, "from_crawler"):
             return action_class.from_crawler(crawler)
         else:
             return action_class()
 
-
     @classmethod
     def raise_invalid_action(cls):
         raise Exception
-        raise InvalidMonitor('Wrong Monitor definition, it should be:\n'
-                             '- an instance of a Monitor/MonitorSuite object.\n'
-                             '- a subclass of Monitor/MonitorSuite.\n'
-                             '- a tuple with the format (name, monitor).\n'
-                             '- a string containing an evaluable python expression.')
+        raise InvalidMonitor(
+            "Wrong Monitor definition, it should be:\n"
+            "- an instance of a Monitor/MonitorSuite object.\n"
+            "- a subclass of Monitor/MonitorSuite.\n"
+            "- a tuple with the format (name, monitor).\n"
+            "- a string containing an evaluable python expression."
+        )
 
     @classmethod
     def raise_invalid_class(cls):
         raise Exception
-        raise InvalidMonitorClass('Wrong Monitor class definition, it should be '
-                                  'an instance of a Monitor/MonitorSuite object.')
+        raise InvalidMonitorClass(
+            "Wrong Monitor class definition, it should be "
+            "an instance of a Monitor/MonitorSuite object."
+        )
```

### Comparing `spidermon-1.8.0/spidermon/core/suites.py` & `spidermon-1.9.0/spidermon/core/suites.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from __future__ import absolute_import
 import six
 
 from unittest import TestSuite
 import inspect
 import collections
 
-from spidermon.exceptions import (InvalidMonitorIterable, NotAllowedMethod)
+from spidermon.exceptions import InvalidMonitorIterable, NotAllowedMethod
 from spidermon import settings
 
 from .monitors import Monitor
 from .options import MonitorOptionsMetaclass
 from .factories import MonitorFactory, ActionFactory
 
 
 class MonitorSuite(six.with_metaclass(MonitorOptionsMetaclass, TestSuite)):
     monitors = []
     monitors_finished_actions = []
     monitors_passed_actions = []
     monitors_failed_actions = []
 
-    def __init__(self, name=None, monitors=None,
-                 monitors_finished_actions=None,
-                 monitors_passed_actions=None,
-                 monitors_failed_actions=None,
-                 order=None,
-                 crawler=None):
+    def __init__(
+        self,
+        name=None,
+        monitors=None,
+        monitors_finished_actions=None,
+        monitors_passed_actions=None,
+        monitors_failed_actions=None,
+        order=None,
+        crawler=None,
+    ):
         self._tests = []
         self._removed_tests = 0
         self._name = name
         self._parent = None
         self._order = order
         self._crawler = crawler
 
@@ -46,65 +50,65 @@
         self.add_monitors_passed_actions(monitors_passed_actions or [])
 
         declarative_monitors_failed_actions = self.monitors_failed_actions
         self.monitors_failed_actions = []
         self.add_monitors_failed_actions(declarative_monitors_failed_actions)
         self.add_monitors_failed_actions(monitors_failed_actions or [])
 
-
     @property
     def name(self):
-        return self._name or \
-               self.options.name or \
-               self.__class__.__name__
+        return self._name or self.options.name or self.__class__.__name__
 
     @property
     def level(self):
-        return self.options.level or \
-               self.parent_level
+        return self.options.level or self.parent_level
 
     @property
     def parent_level(self):
         if self.parent:
             return self.parent.level
         return settings.MONITOR.LEVELS.DEFAULT
 
     @property
     def full_name(self):
         parts = []
         if self.parent and self.parent.full_name:
             parts.append(self.parent.full_name)
         if self.have_custom_name:
             parts.append(self.name)
-        return '/'.join(parts)
+        return "/".join(parts)
 
     @property
     def have_custom_name(self):
-        return self._name or \
-               self.options.name
+        return self._name or self.options.name
 
     @property
     def description(self):
-        return self.options.description or \
-               self.__class__.__doc__ or \
-               settings.MONITOR.DEFAULT_DESCRIPTION
+        return (
+            self.options.description
+            or self.__class__.__doc__
+            or settings.MONITOR.DEFAULT_DESCRIPTION
+        )
 
     @property
     def parent(self):
         return self._parent
 
     @property
     def order(self):
-        return self._order if self._order is not None else None or \
-               self.options.order
+        return self._order if self._order is not None else None or self.options.order
 
     @property
     def number_of_monitors(self):
-        return sum([1 if isinstance(monitor, Monitor) else monitor.number_of_monitors
-                    for monitor in self])
+        return sum(
+            [
+                1 if isinstance(monitor, Monitor) else monitor.number_of_monitors
+                for monitor in self
+            ]
+        )
 
     @property
     def all_monitors(self):
         monitors = []
         for monitor in self:
             if isinstance(monitor, Monitor):
                 monitors += [monitor]
@@ -117,15 +121,15 @@
 
     def init_data(self, data):
         for test in self:
             test.init_data(data)
 
     def add_monitors(self, monitors):
         if not isinstance(monitors, collections.Iterable):
-            raise InvalidMonitorIterable('Monitors definition is not iterable')
+            raise InvalidMonitorIterable("Monitors definition is not iterable")
         for m in monitors:
             self.add_monitor(m)
 
     def add_monitor(self, monitor, name=None):
         monitor = MonitorFactory.load_monitor(monitor, name)
         monitor.set_parent(self)
         super(MonitorSuite, self).addTest(monitor)
@@ -153,38 +157,52 @@
         self._add_action(action, self.monitors_failed_actions)
 
     def _add_action(self, action, target_actions_list):
         action = ActionFactory.load_action(action, crawler=self._crawler)
         target_actions_list.append(action)
 
     def debug_tree(self, level=0):
-        s = level*'\t' + repr(self) + '\n'
+        s = level * "\t" + repr(self) + "\n"
         for test in self:
-            s += test.debug_tree(level=level+1)
+            s += test.debug_tree(level=level + 1)
         return s
 
-    def debug_monitors(self, show_monitor=True, show_method=True, show_level=True,
-                       show_order=False, show_description=True):
+    def debug_monitors(
+        self,
+        show_monitor=True,
+        show_method=True,
+        show_level=True,
+        show_order=False,
+        show_description=True,
+    ):
         def debug_attribute(condition, name, value):
-            return '%12s: %s\n' % (name, str(value)) if condition else ''
-        s = '-'*80 + '\n'
+            return "%12s: %s\n" % (name, str(value)) if condition else ""
+
+        s = "-" * 80 + "\n"
         for t in self.all_monitors:
-            s += debug_attribute(show_monitor,      'MONITOR',      t.monitor_full_name)
-            s += debug_attribute(show_method,       'METHOD',       t.method_name)
-            s += debug_attribute(show_level,        'LEVEL',        t.level)
-            s += debug_attribute(show_order,        'ORDER',        t.order)
-            s += debug_attribute(show_description,  'DESCRIPTION',  t.method_description or '...')
-            s += '-'*80 + '\n'
+            s += debug_attribute(show_monitor, "MONITOR", t.monitor_full_name)
+            s += debug_attribute(show_method, "METHOD", t.method_name)
+            s += debug_attribute(show_level, "LEVEL", t.level)
+            s += debug_attribute(show_order, "ORDER", t.order)
+            s += debug_attribute(
+                show_description, "DESCRIPTION", t.method_description or "..."
+            )
+            s += "-" * 80 + "\n"
         return s
 
     def _reorder_tests(self):
         self._tests = sorted(self._tests, key=lambda x: x.order, reverse=False)
 
     def __repr__(self):
-        return '<SUITE:%s[%d,%s] at %s>' % (self.name, len(self._tests), self.number_of_monitors, hex(id(self)))
+        return "<SUITE:%s[%d,%s] at %s>" % (
+            self.name,
+            len(self._tests),
+            self.number_of_monitors,
+            hex(id(self)),
+        )
 
     def __str__(self):
         return self.name
 
     def __not_allowed_method(self, *args, **kwargs):
         raise NotAllowedMethod
```

### Comparing `spidermon-1.8.0/spidermon/loaders.py` & `spidermon-1.9.0/spidermon/loaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 from .exceptions import InvalidMonitor
 from six.moves import filter
 
 
 class MonitorLoader(TestLoader):
     def load_suite_from_monitor(self, monitor_class, name=None):
         if not (inspect.isclass(monitor_class) and issubclass(monitor_class, Monitor)):
-            raise InvalidMonitor('monitor must be a class subclassing Monitor')
+            raise InvalidMonitor("monitor must be a class subclassing Monitor")
         test_function_names = self.get_testcase_names(monitor_class)
-        if not test_function_names and hasattr(monitor_class, 'runTest'):
-            test_function_names = ['runTest']
-        monitors = [monitor_class(fn_name, name=name)
-                    for fn_name in test_function_names]
+        if not test_function_names and hasattr(monitor_class, "runTest"):
+            test_function_names = ["runTest"]
+        monitors = [
+            monitor_class(fn_name, name=name) for fn_name in test_function_names
+        ]
         loaded_suite = MonitorSuite(
-            monitors=monitors,
-            order=monitor_class.options.order
+            monitors=monitors, order=monitor_class.options.order
         )
         return loaded_suite
 
     def get_testcase_names(self, monitor_class):
-        def is_test_method(attrname, class_name=monitor_class, prefix=self.testMethodPrefix):
-            return attrname.startswith(prefix) and \
-                hasattr(getattr(class_name, attrname), '__call__')
+        def is_test_method(
+            attrname, class_name=monitor_class, prefix=self.testMethodPrefix
+        ):
+            return attrname.startswith(prefix) and hasattr(
+                getattr(class_name, attrname), "__call__"
+            )
+
         test_function_names = list(filter(is_test_method, dir(monitor_class)))
         if self.sortTestMethodsUsing:
             test_function_names.sort(key=_cmp_to_key(self.sortTestMethodsUsing))
         return test_function_names
 
     # TODO: hide methods?
```

### Comparing `spidermon-1.8.0/spidermon/contrib/monitors/mixins/spider.py` & `spidermon-1.9.0/spidermon/contrib/monitors/mixins/spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,120 +3,116 @@
 from spidermon.contrib.stats.analyzer import StatsAnalyzer
 from spidermon.contrib.stats.counters import DictPercentCounter, PercentCounter
 from spidermon.exceptions import NotConfigured
 
 from .job import JobMonitorMixin
 from .stats import StatsMonitorMixin
 
-DOWNLOADER_RESPONSE_COUNT = 'downloader/response_count'
-DOWNLOADER_RESPONSE_STATUS = 'downloader/response_status_count/'
-DOWNLOADER_STATUS_CODES_INFORMATIONAL = [r'1\d{2}$']
-DOWNLOADER_STATUS_CODES_SUCCESSFUL = [r'2\d{2}$']
-DOWNLOADER_STATUS_CODES_REDIRECTIONS = [r'3\d{2}$']
-DOWNLOADER_STATUS_CODES_BAD_REQUESTS = [r'4\d{2}$']
-DOWNLOADER_STATUS_CODES_INTERNAL_SERVER_ERRORS = [r'5\d{2}$']
-DOWNLOADER_STATUS_CODES_OTHERS = ['[^1-5].*$']
-DOWNLOADER_STATUS_CODES_ERRORS = DOWNLOADER_STATUS_CODES_BAD_REQUESTS + \
-    DOWNLOADER_STATUS_CODES_INTERNAL_SERVER_ERRORS
+DOWNLOADER_RESPONSE_COUNT = "downloader/response_count"
+DOWNLOADER_RESPONSE_STATUS = "downloader/response_status_count/"
+DOWNLOADER_STATUS_CODES_INFORMATIONAL = [r"1\d{2}$"]
+DOWNLOADER_STATUS_CODES_SUCCESSFUL = [r"2\d{2}$"]
+DOWNLOADER_STATUS_CODES_REDIRECTIONS = [r"3\d{2}$"]
+DOWNLOADER_STATUS_CODES_BAD_REQUESTS = [r"4\d{2}$"]
+DOWNLOADER_STATUS_CODES_INTERNAL_SERVER_ERRORS = [r"5\d{2}$"]
+DOWNLOADER_STATUS_CODES_OTHERS = ["[^1-5].*$"]
+DOWNLOADER_STATUS_CODES_ERRORS = (
+    DOWNLOADER_STATUS_CODES_BAD_REQUESTS
+    + DOWNLOADER_STATUS_CODES_INTERNAL_SERVER_ERRORS
+)
 
 
 class ResponsesInfo(object):
     def __init__(self, stats):
         self._stats_analyzer = StatsAnalyzer(stats=stats)
-        self.count = self._stats_analyzer.search(
-            DOWNLOADER_RESPONSE_COUNT + '$'
-        ).get(DOWNLOADER_RESPONSE_COUNT, 0)
+        self.count = self._stats_analyzer.search(DOWNLOADER_RESPONSE_COUNT + "$").get(
+            DOWNLOADER_RESPONSE_COUNT, 0
+        )
 
         # all status codes
         self.all = DictPercentCounter(total=self.count)
-        self._add_status_codes(
-            pattern=None,
-            target=self.all
-        )
+        self._add_status_codes(pattern=None, target=self.all)
 
         # 1xx. informational
         self.informational = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_INFORMATIONAL,
-            target=self.informational
+            pattern=DOWNLOADER_STATUS_CODES_INFORMATIONAL, target=self.informational
         )
 
         # 2xx. successful
         self.successful = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_SUCCESSFUL,
-            target=self.successful
+            pattern=DOWNLOADER_STATUS_CODES_SUCCESSFUL, target=self.successful
         )
 
         # 3xx. redirections
         self.redirections = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_REDIRECTIONS,
-            target=self.redirections
+            pattern=DOWNLOADER_STATUS_CODES_REDIRECTIONS, target=self.redirections
         )
 
         # 4xx. bad requests
         self.bad_requests = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_BAD_REQUESTS,
-            target=self.bad_requests
+            pattern=DOWNLOADER_STATUS_CODES_BAD_REQUESTS, target=self.bad_requests
         )
 
         # 5xx. internal server errors
         self.internal_server_errors = DictPercentCounter(total=self.count)
         self._add_status_codes(
             pattern=DOWNLOADER_STATUS_CODES_INTERNAL_SERVER_ERRORS,
-            target=self.internal_server_errors
+            target=self.internal_server_errors,
         )
 
         # >= 6xx. others
         self.others = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_OTHERS, target=self.others)
+            pattern=DOWNLOADER_STATUS_CODES_OTHERS, target=self.others
+        )
 
         # errors (4xx + 5xx)
         self.errors = DictPercentCounter(total=self.count)
         self._add_status_codes(
-            pattern=DOWNLOADER_STATUS_CODES_ERRORS, target=self.errors)
+            pattern=DOWNLOADER_STATUS_CODES_ERRORS, target=self.errors
+        )
 
     def _add_status_codes(self, pattern, target):
         for code, counter in self._get_response_codes(pattern).items():
             target.add_value(code, counter.count)
 
     def _get_response_codes(self, codes=None):
-        codes = codes or ['[^/]+']
+        codes = codes or ["[^/]+"]
         return_codes = {}
         for code in codes:
             return_codes.update(self._get_response_code(code))
         return return_codes
 
     def _get_response_code(self, code):
         return dict(
             [
                 (code, PercentCounter(count, self.count))
-                for count, code in
-                self._stats_analyzer.search(
-                    pattern=DOWNLOADER_RESPONSE_STATUS + ('(%s)$' % code),
-                    include_matches=True
+                for count, code in self._stats_analyzer.search(
+                    pattern=DOWNLOADER_RESPONSE_STATUS + ("(%s)$" % code),
+                    include_matches=True,
                 ).values()
             ]
         )
 
 
 class SpiderMonitorMixin(StatsMonitorMixin, JobMonitorMixin):
     @property
     def crawler(self):
         if not self.data.crawler:
-            raise NotConfigured('Crawler not available!')
+            raise NotConfigured("Crawler not available!")
         return self.data.crawler
 
     @property
     def spider(self):
         if not self.data.spider:
-            raise NotConfigured('Spider not available!')
+            raise NotConfigured("Spider not available!")
         return self.data.spider
 
     @property
     def responses(self):
-        if not hasattr(self, '_responses'):
+        if not hasattr(self, "_responses"):
             self._responses = ResponsesInfo(self.stats)
         return self._responses
```

### Comparing `spidermon-1.8.0/spidermon/contrib/monitors/mixins/validation.py` & `spidermon-1.9.0/spidermon/contrib/monitors/mixins/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from __future__ import absolute_import
-from spidermon.contrib.stats.counters import PercentCounter, DictPercentCounter, AttributeDictPercentCounter
+from spidermon.contrib.stats.counters import (
+    PercentCounter,
+    DictPercentCounter,
+    AttributeDictPercentCounter,
+)
 from spidermon.contrib.stats.analyzer import StatsAnalyzer
 from spidermon.contrib.scrapy.stats import STATS_DEFAULT_VALIDATION_PREFIX
 
 from .stats import StatsMonitorMixin
 
 
 class MetaDictPercentCounter(DictPercentCounter):
     def add_values(self, key, subkey, value):
         if key not in self._dict:
             self._create_item(key)
         self[key].add_value(subkey, value)
 
 
 class ErrorsDictPercentCounter(AttributeDictPercentCounter):
-    __attribute_dict_name__ = 'fields'
+    __attribute_dict_name__ = "fields"
 
 
 class ErrorsInfo(MetaDictPercentCounter):
     __items_class__ = ErrorsDictPercentCounter
 
 
 class FieldErrorsDictPercentCounter(AttributeDictPercentCounter):
-    __attribute_dict_name__ = 'errors'
+    __attribute_dict_name__ = "errors"
 
 
 class FieldErrorsInfo(MetaDictPercentCounter):
     __items_class__ = FieldErrorsDictPercentCounter
 
     def __init__(self, fields_count, items_count):
         super(FieldErrorsInfo, self).__init__(items_count)
@@ -42,135 +46,163 @@
         self.count = items_count
         self.errors = PercentCounter(count=items_with_errors, total=items_count)
         self.dropped = PercentCounter(count=items_dropped, total=items_count)
 
 
 class ValidationInfo(object):
     def __init__(self, stats, prefix=None):
-        self.analyzer = StatsAnalyzer(stats=stats, prefix=prefix or STATS_DEFAULT_VALIDATION_PREFIX)
+        self.analyzer = StatsAnalyzer(
+            stats=stats, prefix=prefix or STATS_DEFAULT_VALIDATION_PREFIX
+        )
 
         # items
-        items_count = sum(self.analyzer.search('items$').values())
-        items_with_errors_count = sum(self.analyzer.search('items/errors$').values())
-        items_dropped_count = sum(self.analyzer.search('items/dropped$').values())
+        items_count = sum(self.analyzer.search("items$").values())
+        items_with_errors_count = sum(self.analyzer.search("items/errors$").values())
+        items_dropped_count = sum(self.analyzer.search("items/dropped$").values())
         self.items = ItemsInfo(
             items_count=items_count,
             items_with_errors=items_with_errors_count,
-            items_dropped=items_dropped_count)
+            items_dropped=items_dropped_count,
+        )
 
         # errors & fields
-        fields_count = sum(self.analyzer.search('fields$').values())
+        fields_count = sum(self.analyzer.search("fields$").values())
         self.errors = ErrorsInfo(items_count)
-        self.fields = FieldErrorsInfo(fields_count=fields_count, items_count=items_count)
+        self.fields = FieldErrorsInfo(
+            fields_count=fields_count, items_count=items_count
+        )
 
-        field_errors = self.analyzer.search('fields/errors/([^/]+)$', include_matches=True)
+        field_errors = self.analyzer.search(
+            "fields/errors/([^/]+)$", include_matches=True
+        )
         for _, error in field_errors.values():
-            field_errors_per_field = self.analyzer.search('fields/errors/%s/([^/]+)$' % error, include_matches=True)
+            field_errors_per_field = self.analyzer.search(
+                "fields/errors/%s/([^/]+)$" % error, include_matches=True
+            )
             for count, field in field_errors_per_field.values():
                 self.errors.add_values(key=error, subkey=field, value=count)
                 self.fields.add_values(key=field, subkey=error, value=count)
 
 
 class ValidationMonitorMixin(StatsMonitorMixin):
     @property
     def validation(self):
-        if not hasattr(self, '_validation'):
+        if not hasattr(self, "_validation"):
             self._validation = ValidationInfo(self.stats)
         return self._validation
 
     def check_missing_required_fields(self, field_names=None, allowed_count=0):
         if not field_names:
-            missing_count = self.validation.errors['missing_required_field'].count
+            missing_count = self.validation.errors["missing_required_field"].count
             self._check_missing_required_count(missing_count, allowed_count)
         else:
             for field_name in field_names:
                 self.check_missing_required_field(field_name, allowed_count)
 
     def check_missing_required_field(self, field_name, allowed_count=0):
-        missing_count = self.validation.fields[field_name].errors['missing_required_field'].count
+        missing_count = (
+            self.validation.fields[field_name].errors["missing_required_field"].count
+        )
         self._check_missing_required_count(missing_count, allowed_count)
 
     def _check_missing_required_count(self, missing_count, allowed_count):
         self.assertLessEqual(
             missing_count,
             allowed_count,
-            msg='{count} required field{plural} are missing!{threshold_info}'.format(
+            msg="{count} required field{plural} are missing!{threshold_info}".format(
                 count=missing_count,
-                plural='' if missing_count == 1 else 's',
-                threshold_info=(' (maximum allowed %d)' % allowed_count) if allowed_count > 0 else '',
-            )
+                plural="" if missing_count == 1 else "s",
+                threshold_info=(" (maximum allowed %d)" % allowed_count)
+                if allowed_count > 0
+                else "",
+            ),
         )
 
-    def check_missing_required_fields_percent(self, field_names=None, allowed_percent=0):
+    def check_missing_required_fields_percent(
+        self, field_names=None, allowed_percent=0
+    ):
         if not field_names:
-            missing_percent = self.validation.errors['missing_required_field'].percent
+            missing_percent = self.validation.errors["missing_required_field"].percent
             self._check_missing_required_percent(missing_percent, allowed_percent)
         else:
             for field_name in field_names:
                 self.check_missing_required_field_percent(field_name, allowed_percent)
 
     def check_missing_required_field_percent(self, field_name, allowed_percent=0):
-        missing_percent = self.validation.fields[field_name].errors['missing_required_field'].percent
+        missing_percent = (
+            self.validation.fields[field_name].errors["missing_required_field"].percent
+        )
         self._check_missing_required_percent(missing_percent, allowed_percent)
 
     def _check_missing_required_percent(self, missing_percent, allowed_percent=0):
         self.assertLessEqual(
             missing_percent,
             allowed_percent,
-            msg='{percent}% of required fields are missing!{threshold_info}'.format(
-                percent=missing_percent*100,
-                threshold_info=(' (maximum allowed %.0f%%)' % (allowed_percent*100)) if allowed_percent > 0 else '',
-            )
+            msg="{percent}% of required fields are missing!{threshold_info}".format(
+                percent=missing_percent * 100,
+                threshold_info=(" (maximum allowed %.0f%%)" % (allowed_percent * 100))
+                if allowed_percent > 0
+                else "",
+            ),
         )
 
     def check_fields_errors(self, field_names=None, errors=None, allowed_count=0):
         if not field_names:
             errors_count = self.validation.errors.count
             self._check_field_errors(errors_count, allowed_count)
         else:
             for field_name in field_names:
                 self.check_field_errors(field_name, errors, allowed_count)
 
     def check_field_errors(self, field_name, errors=None, allowed_count=0):
         if errors:
-            errors_count = sum([self.validation.fields[field_name].errors[e].count for e in errors])
+            errors_count = sum(
+                [self.validation.fields[field_name].errors[e].count for e in errors]
+            )
         else:
             errors_count = self.validation.fields[field_name].errors.count
         self._check_field_errors(errors_count, allowed_count)
 
     def _check_field_errors(self, errors_count, allowed_count):
         self.assertLessEqual(
             errors_count,
             allowed_count,
-            msg='{count} field{count_plural} {verb} validation errors!{threshold_info}'.format(
+            msg="{count} field{count_plural} {verb} validation errors!{threshold_info}".format(
                 count=errors_count,
-                count_plural='' if errors_count == 1 else 's',
-                verb='has' if errors_count == 1 else 'have',
-                threshold_info=(' (maximum allowed %d)' % allowed_count) if allowed_count > 0 else '',
-            )
+                count_plural="" if errors_count == 1 else "s",
+                verb="has" if errors_count == 1 else "have",
+                threshold_info=(" (maximum allowed %d)" % allowed_count)
+                if allowed_count > 0
+                else "",
+            ),
         )
 
-    def check_fields_errors_percent(self, field_names=None, errors=None, allowed_percent=0):
+    def check_fields_errors_percent(
+        self, field_names=None, errors=None, allowed_percent=0
+    ):
         if not field_names:
             errors_percent = self.validation.errors.percent
             self._check_field_errors_percent(errors_percent, allowed_percent)
         else:
             for field_name in field_names:
                 self.check_field_errors_percent(field_name, errors, allowed_percent)
 
     def check_field_errors_percent(self, field_name, errors=None, allowed_percent=0):
         if errors:
-            errors_percent = sum([self.validation.fields[field_name].errors[e].percent for e in errors])
+            errors_percent = sum(
+                [self.validation.fields[field_name].errors[e].percent for e in errors]
+            )
         else:
             errors_percent = self.validation.fields[field_name].errors.percent
         self._check_field_errors_percent(errors_percent, allowed_percent)
 
-
     def _check_field_errors_percent(self, errors_percent, allowed_percent):
         self.assertLessEqual(
             errors_percent,
             allowed_percent,
-            msg='{percent}% of fields have validation errors!{threshold_info}'.format(
-                percent=errors_percent*100,
-                threshold_info=(' (maximum allowed %.0f%%)' % (allowed_percent*100)) if allowed_percent > 0 else '',
-            )
+            msg="{percent}% of fields have validation errors!{threshold_info}".format(
+                percent=errors_percent * 100,
+                threshold_info=(" (maximum allowed %.0f%%)" % (allowed_percent * 100))
+                if allowed_percent > 0
+                else "",
+            ),
         )
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/slack/__init__.py` & `spidermon-1.9.0/spidermon/contrib/actions/slack/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,137 +5,156 @@
 from slackclient import SlackClient
 
 from spidermon.contrib.actions.templates import ActionWithTemplates
 from spidermon.exceptions import NotConfigured
 import six
 
 
-class SlackMessageManager():
+class SlackMessageManager:
     sender_token = None
     sender_name = None
 
     def __init__(self, sender_token=None, sender_name=None):
         sender_token = sender_token or self.sender_token
         if not sender_token:
-            raise NotConfigured('You must provide a slack token.')
+            raise NotConfigured("You must provide a slack token.")
 
         self.sender_name = sender_name or self.sender_name
         if not self.sender_name:
-            raise NotConfigured('You must provide a slack sender name.')
+            raise NotConfigured("You must provide a slack sender name.")
 
         self._client = SlackClient(sender_token)
         self._users = None
 
     @property
     def users(self):
         if self._users is None:
             self._users = self._get_users_info()
         return self._users
 
-    def send_message(self, to, text, parse=None, link_names=1, attachments=None, use_mention=False):
+    def send_message(
+        self, to, text, parse=None, link_names=1, attachments=None, use_mention=False
+    ):
         if isinstance(to, list):
-            return [self.send_message(
-                to=recipient,
+            return [
+                self.send_message(
+                    to=recipient,
+                    text=text,
+                    parse=parse,
+                    link_names=link_names,
+                    attachments=attachments,
+                    use_mention=use_mention,
+                )
+                for recipient in to
+            ]
+        elif to.startswith("@"):
+            return self._send_user_message(
+                username=to,
                 text=text,
                 parse=parse,
                 link_names=link_names,
                 attachments=attachments,
-                use_mention=use_mention,
-            ) for recipient in to]
-        elif to.startswith('@'):
-                return self._send_user_message(
-                    username=to,
-                    text=text,
-                    parse=parse,
-                    link_names=link_names,
-                    attachments=attachments)
+            )
         else:
             if use_mention:
-                if to.startswith('#'):
-                    text = '@channel: ' + text
+                if to.startswith("#"):
+                    text = "@channel: " + text
                 else:
-                    text = '@group: ' + text
+                    text = "@group: " + text
             return self._send_channel_message(
                 channel=to,
                 text=text,
                 parse=parse,
                 link_names=link_names,
                 attachments=attachments,
             )
 
     def _get_user_id(self, username):
-        name = username[1:] if username.startswith('@') else username
+        name = username[1:] if username.startswith("@") else username
         user = self.users.get(name, None)
-        return user['id'] if user else None
+        return user["id"] if user else None
 
     def _get_users_info(self):
-        return dict([
-            (member['name'].lower(), member)
-            for member in self._api_call('users.list')['members']
-        ])
+        return dict(
+            [
+                (member["name"].lower(), member)
+                for member in self._api_call("users.list")["members"]
+            ]
+        )
 
     def _api_call(self, method, **kwargs):
         response = self._client.api_call(method, **kwargs)
         if isinstance(response, six.string_types):  # slackclient < v1.0
             response = json.loads(response)
         return response
 
     def _get_user_channel(self, user_id):
-        return self._api_call('im.open', user=user_id)['channel']['id']
+        return self._api_call("im.open", user=user_id)["channel"]["id"]
 
-    def _send_user_message(self, username, text, parse='full', link_names=1, attachments=None):
+    def _send_user_message(
+        self, username, text, parse="full", link_names=1, attachments=None
+    ):
         user_id = self._get_user_id(username)
         if user_id:
             user_channel = self._get_user_channel(user_id)
             return self._send_channel_message(
                 channel=user_channel,
                 text=text,
                 parse=parse,
                 link_names=link_names,
                 attachments=attachments,
             )
 
-    def _send_channel_message(self, channel, text, parse='full', link_names=1, attachments=None):
+    def _send_channel_message(
+        self, channel, text, parse="full", link_names=1, attachments=None
+    ):
         return self._api_call(
-            'chat.postMessage',
+            "chat.postMessage",
             channel=channel,
             text=text,
             parse=parse,
             link_names=link_names,
             attachments=self._parse_attachments(attachments),
             username=self.sender_name,
-            icon_url=self.users[self.sender_name]['profile']['image_48'],
+            icon_url=self.users[self.sender_name]["profile"]["image_48"],
         )
 
     def _parse_attachments(self, attachments):
         if not attachments:
             return None
         else:
             python_attachments = ast.literal_eval(attachments)
             return json.dumps(python_attachments)
 
 
 class SendSlackMessage(ActionWithTemplates):
     message = None
     attachments = None
-    message_template = 'slack/default/message.jinja'
-    attachments_template = 'slack/default/attachments.jinja'
+    message_template = "slack/default/message.jinja"
+    attachments_template = "slack/default/attachments.jinja"
     recipients = None
     sender_token = None
     sender_name = None
     include_message = True
     include_attachments = True
     fake = False
 
-    def __init__(self,
-                 sender_token=None, sender_name=None,
-                 recipients=None,
-                 message=None, message_template=None, include_message=None,
-                 attachments=None, attachments_template=None, include_attachments=None,
-                 fake=None):
+    def __init__(
+        self,
+        sender_token=None,
+        sender_name=None,
+        recipients=None,
+        message=None,
+        message_template=None,
+        include_message=None,
+        attachments=None,
+        attachments_template=None,
+        include_attachments=None,
+        fake=None,
+    ):
         super(SendSlackMessage, self).__init__()
         self.fake = fake or self.fake
         if not self.fake:
             self.manager = SlackMessageManager(
                 sender_token=sender_token or self.sender_token,
                 sender_name=sender_name or self.sender_name,
             )
@@ -145,43 +164,51 @@
         self.message = message or self.message
         self.message_template = message_template or self.message_template
         self.include_message = include_message or self.include_message
         self.attachments = attachments or self.attachments
         self.attachments_template = attachments_template or self.attachments_template
         self.include_attachments = include_attachments or self.include_attachments
         if not self.fake and not self.recipients:
-            raise NotConfigured("You must provide at least one recipient for the message.")
+            raise NotConfigured(
+                "You must provide at least one recipient for the message."
+            )
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         return {
-            'sender_token': crawler.settings.get('SPIDERMON_SLACK_SENDER_TOKEN'),
-            'sender_name': crawler.settings.get('SPIDERMON_SLACK_SENDER_NAME'),
-            'recipients': crawler.settings.get('SPIDERMON_SLACK_RECIPIENTS'),
-            'message': crawler.settings.get('SPIDERMON_SLACK_MESSAGE'),
-            'message_template': crawler.settings.get('SPIDERMON_SLACK_MESSAGE_TEMPLATE'),
-            'attachments': crawler.settings.get('SPIDERMON_SLACK_ATTACHMENTS'),
-            'attachments_template': crawler.settings.get('SPIDERMON_SLACK_ATTACHMENTS_TEMPLATE'),
-            'include_message': crawler.settings.getbool('SPIDERMON_SLACK_INCLUDE_MESSAGE'),
-            'include_attachments': crawler.settings.getbool('SPIDERMON_SLACK_INCLUDE_ATTACHMENTS'),
-            'fake': crawler.settings.getbool('SPIDERMON_SLACK_FAKE'),
+            "sender_token": crawler.settings.get("SPIDERMON_SLACK_SENDER_TOKEN"),
+            "sender_name": crawler.settings.get("SPIDERMON_SLACK_SENDER_NAME"),
+            "recipients": crawler.settings.get("SPIDERMON_SLACK_RECIPIENTS"),
+            "message": crawler.settings.get("SPIDERMON_SLACK_MESSAGE"),
+            "message_template": crawler.settings.get(
+                "SPIDERMON_SLACK_MESSAGE_TEMPLATE"
+            ),
+            "attachments": crawler.settings.get("SPIDERMON_SLACK_ATTACHMENTS"),
+            "attachments_template": crawler.settings.get(
+                "SPIDERMON_SLACK_ATTACHMENTS_TEMPLATE"
+            ),
+            "include_message": crawler.settings.getbool(
+                "SPIDERMON_SLACK_INCLUDE_MESSAGE"
+            ),
+            "include_attachments": crawler.settings.getbool(
+                "SPIDERMON_SLACK_INCLUDE_ATTACHMENTS"
+            ),
+            "fake": crawler.settings.getbool("SPIDERMON_SLACK_FAKE"),
         }
 
     def run_action(self):
         message = self.get_message()
         attachments = self.get_attachments()
         if not self.fake:
             self.manager.send_message(
-                to=self.recipients,
-                text=message,
-                attachments=attachments,
+                to=self.recipients, text=message, attachments=attachments
             )
         else:
-            print('message:', message)
-            print('attachments:', attachments)
+            print("message:", message)
+            print("attachments:", attachments)
 
     def get_message(self):
         if self.include_message:
             if self.message:
                 return self.render_text_template(self.message)
             else:
                 return self.render_template(self.message_template)
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/macros.jinja` & `spidermon-1.9.0/spidermon/contrib/actions/slack/templates/slack/spider/notifier/macros.jinja`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/slack/notifiers.py` & `spidermon-1.9.0/spidermon/contrib/actions/slack/notifiers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 from __future__ import absolute_import
 from . import SendSlackMessage
 
 
 class SendSlackMessageSpiderStarted(SendSlackMessage):
-    message_template = 'slack/spider/notifier/start/message.jinja'
+    message_template = "slack/spider/notifier/start/message.jinja"
     include_attachments = False
 
 
 class SendSlackMessageSpiderFinished(SendSlackMessage):
-    message_template = 'slack/spider/notifier/finish/message.jinja'
-    attachments_template = 'slack/spider/notifier/finish/attachments.jinja'
+    message_template = "slack/spider/notifier/finish/message.jinja"
+    attachments_template = "slack/spider/notifier/finish/attachments.jinja"
     include_ok_attachments = False
     include_error_attachments = True
     include_report_link = True
     report_index = 0
 
-    def __init__(self,
-                 include_ok_attachments=None,
-                 include_error_attachments=None,
-                 include_report_link=None,
-                 report_index=None,
-                 *args, **kwargs):
+    def __init__(
+        self,
+        include_ok_attachments=None,
+        include_error_attachments=None,
+        include_report_link=None,
+        report_index=None,
+        *args,
+        **kwargs
+    ):
         super(SendSlackMessageSpiderFinished, self).__init__(*args, **kwargs)
-        self.include_ok_attachments = include_ok_attachments or self.include_ok_attachments
-        self.include_error_attachments = include_error_attachments or self.include_error_attachments
+        self.include_ok_attachments = (
+            include_ok_attachments or self.include_ok_attachments
+        )
+        self.include_error_attachments = (
+            include_error_attachments or self.include_error_attachments
+        )
         self.include_report_link = include_report_link or self.include_report_link
         self.report_index = report_index or self.report_index
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(SendSlackMessageSpiderFinished, cls).from_crawler_kwargs(crawler)
-        kwargs.update({
-            'include_ok_attachments': crawler.settings.get('SPIDERMON_SLACK_NOTIFIER_INCLUDE_OK_ATTACHMENTS'),
-            'include_error_attachments': crawler.settings.get('SPIDERMON_SLACK_NOTIFIER_INCLUDE_ERROR_ATTACHMENTS'),
-            'include_report_link': crawler.settings.get('SPIDERMON_SLACK_NOTIFIER_INCLUDE_REPORT_LINK'),
-            'report_index': crawler.settings.get('SPIDERMON_SLACK_NOTIFIER_REPORT_INDEX'),
-        })
+        kwargs.update(
+            {
+                "include_ok_attachments": crawler.settings.get(
+                    "SPIDERMON_SLACK_NOTIFIER_INCLUDE_OK_ATTACHMENTS"
+                ),
+                "include_error_attachments": crawler.settings.get(
+                    "SPIDERMON_SLACK_NOTIFIER_INCLUDE_ERROR_ATTACHMENTS"
+                ),
+                "include_report_link": crawler.settings.get(
+                    "SPIDERMON_SLACK_NOTIFIER_INCLUDE_REPORT_LINK"
+                ),
+                "report_index": crawler.settings.get(
+                    "SPIDERMON_SLACK_NOTIFIER_REPORT_INDEX"
+                ),
+            }
+        )
         return kwargs
 
     def get_attachments(self):
-        if (self.monitors_failed and self.include_error_attachments) or\
-           (self.monitors_passed and self.include_ok_attachments):
+        if (self.monitors_failed and self.include_error_attachments) or (
+            self.monitors_passed and self.include_ok_attachments
+        ):
             return super(SendSlackMessageSpiderFinished, self).get_attachments()
         else:
             return None
 
     def get_template_context(self):
         context = super(SendSlackMessageSpiderFinished, self).get_template_context()
-        context.update({
-            'include_ok_attachments': self.include_ok_attachments,
-            'include_error_attachments': self.include_error_attachments,
-            'include_report_link': self.include_report_link,
-            'report_index': self.report_index,
-        })
+        context.update(
+            {
+                "include_ok_attachments": self.include_ok_attachments,
+                "include_error_attachments": self.include_error_attachments,
+                "include_report_link": self.include_report_link,
+                "report_index": self.report_index,
+            }
+        )
         return context
 
 
 class SendSlackMessageSpiderRunning(SendSlackMessageSpiderFinished):
-    message_template = 'slack/spider/notifier/periodic/message.jinja'
-    attachments_template = 'slack/spider/notifier/periodic/attachments.jinja'
+    message_template = "slack/spider/notifier/periodic/message.jinja"
+    attachments_template = "slack/spider/notifier/periodic/attachments.jinja"
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/email/__init__.py` & `spidermon-1.9.0/spidermon/contrib/actions/email/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,118 +19,133 @@
     reply_to = None
     body_text = None
     body_text_template = None
     body_html = None
     body_html_template = None
     fake = False
 
-    def __init__(self,
-                 sender,
-                 to, cc=None, bcc=None, reply_to=None,
-                 subject=None, subject_template=None,
-                 body_text=None, body_text_template=None,
-                 body_html=None, body_html_template=None,
-                 fake=None,
-                 *args, **kwargs):
+    def __init__(
+        self,
+        sender,
+        to,
+        cc=None,
+        bcc=None,
+        reply_to=None,
+        subject=None,
+        subject_template=None,
+        body_text=None,
+        body_text_template=None,
+        body_html=None,
+        body_html_template=None,
+        fake=None,
+        *args,
+        **kwargs
+    ):
         super(SendEmail, self).__init__(*args, **kwargs)
         self.sender = sender or self.sender
         self.subject = subject or self.subject
         self.subject_template = subject_template or self.subject_template
         self.to = to or self.to
         self.cc = cc or self.cc
         self.bcc = bcc or self.bcc
         self.reply_to = reply_to or self.reply_to
         self.body_text = body_text or self.body_text
         self.body_text_template = body_text_template or self.body_text_template
         self.body_html = body_html or self.body_html
         self.body_html_template = body_html_template or self.body_html_template
         self.fake = fake or self.fake
         if not self.fake and not self.to:
-            raise NotConfigured("You must provide at least one recipient for the message.")
+            raise NotConfigured(
+                "You must provide at least one recipient for the message."
+            )
         if not self.subject:
             raise NotConfigured("You must provide a subject for the message.")
-        if not (self.body_text or body_text_template or body_html or self.body_html_template):
+        if not (
+            self.body_text or body_text_template or body_html or self.body_html_template
+        ):
             raise NotConfigured("You must provide a body for the message.")
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         return {
-            'sender': crawler.settings.get('SPIDERMON_EMAIL_SENDER'),
-            'subject': crawler.settings.get('SPIDERMON_EMAIL_SUBJECT'),
-            'subject_template': crawler.settings.get('SPIDERMON_EMAIL_SUBJECT_TEMPLATE'),
-            'to': crawler.settings.get('SPIDERMON_EMAIL_TO'),
-            'cc': crawler.settings.get('SPIDERMON_EMAIL_CC'),
-            'bcc': crawler.settings.get('SPIDERMON_EMAIL_BCC'),
-            'reply_to': crawler.settings.get('SPIDERMON_EMAIL_REPLY_TO'),
-            'body_text': crawler.settings.get('SPIDERMON_BODY_TEXT'),
-            'body_text_template': crawler.settings.get('SPIDERMON_BODY_TEXT_TEMPLATE'),
-            'body_html': crawler.settings.get('SPIDERMON_BODY_HTML'),
-            'body_html_template': crawler.settings.get('SPIDERMON_BODY_HTML_TEMPLATE'),
-            'fake': crawler.settings.getbool('SPIDERMON_EMAIL_FAKE'),
-            'context': crawler.settings.getdict('SPIDERMON_EMAIL_CONTEXT'),
+            "sender": crawler.settings.get("SPIDERMON_EMAIL_SENDER"),
+            "subject": crawler.settings.get("SPIDERMON_EMAIL_SUBJECT"),
+            "subject_template": crawler.settings.get(
+                "SPIDERMON_EMAIL_SUBJECT_TEMPLATE"
+            ),
+            "to": crawler.settings.get("SPIDERMON_EMAIL_TO"),
+            "cc": crawler.settings.get("SPIDERMON_EMAIL_CC"),
+            "bcc": crawler.settings.get("SPIDERMON_EMAIL_BCC"),
+            "reply_to": crawler.settings.get("SPIDERMON_EMAIL_REPLY_TO"),
+            "body_text": crawler.settings.get("SPIDERMON_BODY_TEXT"),
+            "body_text_template": crawler.settings.get("SPIDERMON_BODY_TEXT_TEMPLATE"),
+            "body_html": crawler.settings.get("SPIDERMON_BODY_HTML"),
+            "body_html_template": crawler.settings.get("SPIDERMON_BODY_HTML_TEMPLATE"),
+            "fake": crawler.settings.getbool("SPIDERMON_EMAIL_FAKE"),
+            "context": crawler.settings.getdict("SPIDERMON_EMAIL_CONTEXT"),
         }
 
     def run_action(self):
         message = self.get_message()
         if not self.fake:
             self.send_message(message)
         else:
-            print('-'*40)
+            print("-" * 40)
             print(message.as_string())
-            print('-'*40)
+            print("-" * 40)
 
     def get_subject(self):
         if self.subject:
             return self.render_text_template(self.subject)
         elif self.subject_template:
             return self.render_template(self.subject_template)
         else:
-            return ''
+            return ""
 
     def get_body_text(self):
         if self.body_text:
             return self.render_text_template(self.body_text)
         elif self.body_text_template:
             return self.render_template(self.body_text_template)
         else:
-            return ''
+            return ""
 
     def get_body_html(self):
-        html = ''
+        html = ""
         if self.body_html:
             html = transform(self.render_text_template(self.body_html))
         elif self.body_html_template:
             html = transform(self.render_template(self.body_html_template))
         return html
 
     def get_message(self):
         subject = self.get_subject()
         body_text = self.get_body_text()
         body_html = self.get_body_html()
 
-        message = MIMEMultipart('alternative')
-        message.set_charset('UTF-8')
+        message = MIMEMultipart("alternative")
+        message.set_charset("UTF-8")
 
-        message['Subject'] = subject
-        message['From'] = self.sender
-        message['To'] = self._format_recipients(self.to)
+        message["Subject"] = subject
+        message["From"] = self.sender
+        message["To"] = self._format_recipients(self.to)
         if self.cc:
-            message['Cc'] = self._format_recipients(self.cc)
+            message["Cc"] = self._format_recipients(self.cc)
         if self.bcc:
-            message['Bcc'] = self._format_recipients(self.bcc)
+            message["Bcc"] = self._format_recipients(self.bcc)
         if self.reply_to:
-            message['reply-to'] = self.reply_to
+            message["reply-to"] = self.reply_to
 
-        message.attach(MIMEText(body_text, 'plain'))
+        message.attach(MIMEText(body_text, "plain"))
         if body_html:
-            message.attach(MIMEText(body_html, 'html'))
+            message.attach(MIMEText(body_html, "html"))
 
         return message
 
     def send_message(self, message):
         raise NotImplementedError
 
     def _format_recipients(self, recipients):
         if isinstance(recipients, (list, tuple)):
-            return ', '.join(recipients)
+            return ", ".join(recipients)
         else:
             return recipients
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/email/ses.py` & `spidermon-1.9.0/spidermon/contrib/actions/email/ses.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,18 @@
             raise NotConfigured("You must provide the AWS Access Key.")
         if not self.fake and not self.aws_secret_key:
             raise NotConfigured("You must provide the AWS Secret Key.")
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(SendSESEmail, cls).from_crawler_kwargs(crawler)
-        kwargs.update({
-            'aws_access_key': crawler.settings.get('SPIDERMON_AWS_ACCESS_KEY'),
-            'aws_secret_key': crawler.settings.get('SPIDERMON_AWS_SECRET_KEY'),
-        })
+        kwargs.update(
+            {
+                "aws_access_key": crawler.settings.get("SPIDERMON_AWS_ACCESS_KEY"),
+                "aws_secret_key": crawler.settings.get("SPIDERMON_AWS_SECRET_KEY"),
+            }
+        )
         return kwargs
 
     def send_message(self, message):
         session = boto.connect_ses(self.aws_access_key, self.aws_secret_key)
         session.send_raw_email(raw_message=message.as_string())
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/jobs/tags.py` & `spidermon-1.9.0/spidermon/contrib/actions/jobs/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,40 +12,38 @@
         tags = tags or self.tags
         self.tags = tags if isinstance(tags, list) else [tags]
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(JobTagsAction, cls).from_crawler_kwargs(crawler)
         if cls.tag_settings:
-            kwargs.update({
-                'tags': crawler.settings.get(cls.tag_settings),
-            })
+            kwargs.update({"tags": crawler.settings.get(cls.tag_settings)})
         return kwargs
 
     def run_action(self):
         if self.tags:
             if not self.data.job:
-                raise NotConfigured('Job not available!')
+                raise NotConfigured("Job not available!")
             job_metadata = self.data.job.metadata
             self.process_tags(job_metadata)
             job_metadata.save()
 
     def process_tags(self, job_metadata):
         raise NotImplementedError
 
 
 class AddJobTags(JobTagsAction):
-    tag_settings = 'SPIDERMON_JOB_TAGS_TO_ADD'
+    tag_settings = "SPIDERMON_JOB_TAGS_TO_ADD"
 
     def process_tags(self, job_metadata):
         for tag in self.tags:
-            if tag not in job_metadata['tags']:
-                job_metadata['tags'].append(tag)
+            if tag not in job_metadata["tags"]:
+                job_metadata["tags"].append(tag)
 
 
 class RemoveJobTags(JobTagsAction):
-    tag_settings = 'SPIDERMON_JOB_TAGS_TO_REMOVE'
+    tag_settings = "SPIDERMON_JOB_TAGS_TO_REMOVE"
 
     def process_tags(self, job_metadata):
         for tag in self.tags:
-            if tag in job_metadata['tags']:
-                job_metadata['tags'].remove(tag)
+            if tag in job_metadata["tags"]:
+                job_metadata["tags"].remove(tag)
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/s3.py` & `spidermon-1.9.0/spidermon/contrib/actions/reports/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,47 +5,53 @@
 from boto.s3.key import Key
 
 from spidermon.exceptions import NotConfigured
 
 from . import CreateReport
 
 
-DEFAULT_S3_REGION_ENDPOINT = 's3.amazonaws.com'
-DEFAULT_S3_CONTENT_TYPE = 'text/html'
-URL_SECRET_KEY = 'The secret to life the universe and everything'
+DEFAULT_S3_REGION_ENDPOINT = "s3.amazonaws.com"
+DEFAULT_S3_CONTENT_TYPE = "text/html"
+URL_SECRET_KEY = "The secret to life the universe and everything"
 
 
 class S3Uploader(object):
     def __init__(self, aws_key, aws_secret):
         self.connection = S3Connection(
-            aws_access_key_id=aws_key,
-            aws_secret_access_key=aws_secret)
+            aws_access_key_id=aws_key, aws_secret_access_key=aws_secret
+        )
 
-    def upload_from_file(self, source_filename, s3_bucket, s3_filename, headers=None, make_public=False):
-        with open(source_filename, 'r') as f:
+    def upload_from_file(
+        self, source_filename, s3_bucket, s3_filename, headers=None, make_public=False
+    ):
+        with open(source_filename, "r") as f:
             self._upload_with_method(
                 bucket=s3_bucket,
-                method_name='set_contents_from_file',
+                method_name="set_contents_from_file",
                 filename=s3_filename,
                 content=f,
                 headers=headers,
                 make_public=make_public,
             )
 
-    def upload_from_content(self, content, s3_bucket, s3_filename, headers=None, make_public=False):
+    def upload_from_content(
+        self, content, s3_bucket, s3_filename, headers=None, make_public=False
+    ):
         self._upload_with_method(
             bucket=s3_bucket,
-            method_name='set_contents_from_string',
+            method_name="set_contents_from_string",
             filename=s3_filename,
             content=content,
             headers=headers,
             make_public=make_public,
         )
 
-    def _upload_with_method(self, bucket, method_name, filename, content, headers=None, make_public=False):
+    def _upload_with_method(
+        self, bucket, method_name, filename, content, headers=None, make_public=False
+    ):
         # Get bucket without validation (Needed to be used with credentials w/o listing perms)
         bucket = self.connection.get_bucket(bucket, validate=False)
         f = Key(bucket)
         f.key = filename
         getattr(f, method_name)(content, headers=headers)
         if make_public:
             f.make_public()
@@ -56,18 +62,26 @@
     aws_secret_key = None
     s3_bucket = None
     s3_filename = None
     s3_region_endpoint = DEFAULT_S3_REGION_ENDPOINT
     make_public = True
     content_type = DEFAULT_S3_CONTENT_TYPE
 
-    def __init__(self, aws_access_key=None, aws_secret_key=None,
-                 s3_bucket=None, s3_filename=None, s3_region_endpoint=None,
-                 make_public=False, content_type=None,
-                 *args, **kwargs):
+    def __init__(
+        self,
+        aws_access_key=None,
+        aws_secret_key=None,
+        s3_bucket=None,
+        s3_filename=None,
+        s3_region_endpoint=None,
+        make_public=False,
+        content_type=None,
+        *args,
+        **kwargs
+    ):
         super(CreateS3Report, self).__init__(*args, **kwargs)
 
         self.aws_access_key = aws_access_key or self.aws_access_key
         self.aws_secret_key = aws_secret_key or self.aws_secret_key
         self.s3_bucket = s3_bucket or self.s3_bucket
         self.s3_region_endpoint = s3_region_endpoint or self.s3_region_endpoint
         self.s3_filename = s3_filename or self.s3_filename
@@ -81,53 +95,56 @@
             raise NotConfigured("You must define the s3 bucket.")
         if not self.s3_filename:
             raise NotConfigured("You must define the s3 filename.")
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(CreateS3Report, cls).from_crawler_kwargs(crawler)
-        kwargs.update({
-            'aws_access_key': crawler.settings.get('SPIDERMON_AWS_ACCESS_KEY'),
-            'aws_secret_key': crawler.settings.get('SPIDERMON_AWS_SECRET_KEY'),
-            's3_bucket': crawler.settings.get('SPIDERMON_REPORT_S3_BUCKET'),
-            's3_filename': crawler.settings.get('SPIDERMON_REPORT_S3_FILENAME'),
-            's3_region_endpoint': crawler.settings.get('SPIDERMON_REPORT_S3_REGION_ENDPOINT'),
-            'make_public': crawler.settings.get('SPIDERMON_REPORT_S3_MAKE_PUBLIC'),
-            'content_type': crawler.settings.get('SPIDERMON_REPORT_S3_CONTENT_TYPE'),
-        })
+        kwargs.update(
+            {
+                "aws_access_key": crawler.settings.get("SPIDERMON_AWS_ACCESS_KEY"),
+                "aws_secret_key": crawler.settings.get("SPIDERMON_AWS_SECRET_KEY"),
+                "s3_bucket": crawler.settings.get("SPIDERMON_REPORT_S3_BUCKET"),
+                "s3_filename": crawler.settings.get("SPIDERMON_REPORT_S3_FILENAME"),
+                "s3_region_endpoint": crawler.settings.get(
+                    "SPIDERMON_REPORT_S3_REGION_ENDPOINT"
+                ),
+                "make_public": crawler.settings.get("SPIDERMON_REPORT_S3_MAKE_PUBLIC"),
+                "content_type": crawler.settings.get(
+                    "SPIDERMON_REPORT_S3_CONTENT_TYPE"
+                ),
+            }
+        )
         return kwargs
 
     def after_render_report(self):
         s3 = S3Uploader(self.aws_access_key, self.aws_secret_key)
         s3.upload_from_content(
             content=self.report,
             s3_bucket=self.s3_bucket,
             s3_filename=self.get_s3_filename(),
-            headers={'Content-Type': self.content_type},
+            headers={"Content-Type": self.content_type},
             make_public=self.make_public,
         )
 
     def get_s3_filename(self):
-        return 'reports/{secret}/{filename}'.format(
+        return "reports/{secret}/{filename}".format(
             secret=self.get_url_secret(),
             filename=self.render_text_template(self.s3_filename),
         )
 
     def get_s3_report_url(self):
-        return 'https://{region}/{bucket}/{filename}'.format(
+        return "https://{region}/{bucket}/{filename}".format(
             region=self.s3_region_endpoint,
             bucket=self.s3_bucket,
             filename=self.get_s3_filename(),
         )
 
     def get_url_secret(self):
         secret = URL_SECRET_KEY
         if self.data.job:
-            secret += str(self.data.job.key.split('/')[0])
+            secret += str(self.data.job.key.split("/")[0])
         return hashlib.md5(secret.encode()).hexdigest()
 
     def get_meta(self):
         report_url = self.get_s3_report_url()
-        return {
-            'reports_links': self.data.meta.get('reports', []) + [report_url]
-        }
-
+        return {"reports_links": self.data.meta.get("reports", []) + [report_url]}
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/__init__.py` & `spidermon-1.9.0/spidermon/contrib/actions/reports/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 class CreateReport(ActionWithTemplates):
     template = None
 
     def __init__(self, template=None, *args, **kwargs):
         super(CreateReport, self).__init__(*args, **kwargs)
         self.template = template or self.template
-        self.report = ''
+        self.report = ""
         if not self.template:
             raise NotConfigured("You must define one template file.")
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(CreateReport, cls).from_crawler_kwargs(crawler)
-        kwargs.update({
-            'template': crawler.settings.get('SPIDERMON_REPORT_TEMPLATE'),
-            'context': crawler.settings.getdict('SPIDERMON_REPORT_CONTEXT'),
-        })
+        kwargs.update(
+            {
+                "template": crawler.settings.get("SPIDERMON_REPORT_TEMPLATE"),
+                "context": crawler.settings.getdict("SPIDERMON_REPORT_CONTEXT"),
+            }
+        )
         return kwargs
 
     def run_action(self):
         self.before_render_report()
         self.render_report()
         self.after_render_report()
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.jinja` & `spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.jinja`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.css` & `spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/monitors/result.css`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/report.css` & `spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/report.css`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/email.css` & `spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/email.css`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/base.jinja` & `spidermon-1.9.0/spidermon/contrib/actions/reports/templates/reports/email/bases/report/base.jinja`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/reports/files.py` & `spidermon-1.9.0/spidermon/contrib/actions/reports/files.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,15 @@
         self.filename = filename or self.filename
         if not self.filename:
             raise NotConfigured("You must define a template output file.")
 
     @classmethod
     def from_crawler_kwargs(cls, crawler):
         kwargs = super(CreateFileReport, cls).from_crawler_kwargs(crawler)
-        kwargs.update({
-            'filename': crawler.settings.get('SPIDERMON_REPORT_FILENAME'),
-        })
+        kwargs.update({"filename": crawler.settings.get("SPIDERMON_REPORT_FILENAME")})
         return kwargs
 
     def after_render_report(self):
         rendered_filename = self.render_text_template(self.filename)
 
         with open(rendered_filename, "w") as f:
             f.write(self.report)
```

### Comparing `spidermon-1.8.0/spidermon/contrib/actions/templates.py` & `spidermon-1.9.0/spidermon/contrib/actions/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,14 @@
 
     def render_template(self, template):
         template = self.get_template(template)
         return template.render(self.get_template_context())
 
     def get_template_context(self):
         context = {
-            'result': self.result,
-            'data': self.data,
-            'monitors_passed': self.monitors_passed,
-            'monitors_failed': self.monitors_failed,
+            "result": self.result,
+            "data": self.data,
+            "monitors_passed": self.monitors_passed,
+            "monitors_failed": self.monitors_failed,
         }
         context.update(self.context)
         return context
```

### Comparing `spidermon-1.8.0/spidermon/contrib/scrapy/extensions.py` & `spidermon-1.9.0/spidermon/contrib/scrapy/extensions.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,31 +9,49 @@
 from spidermon.contrib.scrapy.runners import SpiderMonitorRunner
 from spidermon.utils.hubstorage import hs
 from spidermon.python import factory
 from spidermon.python.monitors import ExpressionsMonitor
 
 
 class Spidermon(object):
-
-    def __init__(self, crawler,
-                 spider_opened_suites=None, spider_closed_suites=None,
-                 spider_opened_expression_suites=None, spider_closed_expression_suites=None,
-                 expressions_monitor_class=None,
-                 periodic_suites=None):
-        if not crawler.settings.getbool('SPIDERMON_ENABLED'):
+    def __init__(
+        self,
+        crawler,
+        spider_opened_suites=None,
+        spider_closed_suites=None,
+        engine_stopped_suites=None,
+        spider_opened_expression_suites=None,
+        spider_closed_expression_suites=None,
+        engine_stopped_expression_suites=None,
+        expressions_monitor_class=None,
+        periodic_suites=None,
+    ):
+        if not crawler.settings.getbool("SPIDERMON_ENABLED"):
             raise NotConfigured
         self.crawler = crawler
 
-        self.spider_opened_suites = [self.load_suite(s) for s in spider_opened_suites or []]
-        self.spider_opened_suites += [self.load_expression_suite(s, expressions_monitor_class)
-                                      for s in spider_opened_expression_suites or []]
-
-        self.spider_closed_suites = [self.load_suite(s) for s in spider_closed_suites or []]
-        self.spider_closed_suites += [self.load_expression_suite(s, expressions_monitor_class)
-                                      for s in spider_closed_expression_suites or []]
+        self.spider_opened_suites = [
+            self.load_suite(s) for s in spider_opened_suites or []
+        ]
+        self.spider_opened_suites += [
+            self.load_expression_suite(s, expressions_monitor_class)
+            for s in spider_opened_expression_suites or []
+        ]
+
+        self.spider_closed_suites = [
+            self.load_suite(s) for s in spider_closed_suites or []
+        ]
+        self.spider_closed_suites += [
+            self.load_expression_suite(s, expressions_monitor_class)
+            for s in spider_closed_expression_suites or []
+        ]
+
+        self.engine_stopped_suites = [self.load_suite(s) for s in engine_stopped_suites or []]
+        self.engine_stopped_suites += [self.load_expression_suite(s, expressions_monitor_class)
+                                       for s in engine_stopped_expression_suites or []]
 
         self.periodic_suites = periodic_suites or {}
         self.periodic_tasks = {}
 
     def load_suite(self, suite_to_load):
         try:
             suite_class = load_object(suite_to_load)
@@ -45,34 +63,50 @@
 
     def load_expression_suite(self, suite_to_load, monitor_class=None):
         if monitor_class:
             monitor_class = load_object(monitor_class)
         else:
             monitor_class = ExpressionsMonitor
         monitor = factory.create_monitor_class_from_dict(
-            monitor_dict=suite_to_load,
-            monitor_class=monitor_class
+            monitor_dict=suite_to_load, monitor_class=monitor_class
         )
         suite = MonitorSuite(crawler=self.crawler)
         suite.add_monitor(monitor)
         return suite
 
     @classmethod
     def from_crawler(cls, crawler):
         ext = cls(
             crawler=crawler,
-            spider_opened_suites=crawler.settings.getlist('SPIDERMON_SPIDER_OPEN_MONITORS'),
-            spider_closed_suites=crawler.settings.getlist('SPIDERMON_SPIDER_CLOSE_MONITORS'),
-            spider_opened_expression_suites=crawler.settings.getlist('SPIDERMON_SPIDER_OPEN_EXPRESSION_MONITORS'),
-            spider_closed_expression_suites=crawler.settings.getlist('SPIDERMON_SPIDER_CLOSE_EXPRESSION_MONITORS'),
-            expressions_monitor_class=crawler.settings.get('SPIDERMON_EXPRESSIONS_MONITOR_CLASS'),
-            periodic_suites=crawler.settings.getdict('SPIDERMON_PERIODIC_MONITORS'),
+            spider_opened_suites=crawler.settings.getlist(
+                "SPIDERMON_SPIDER_OPEN_MONITORS"
+            ),
+            spider_closed_suites=crawler.settings.getlist(
+                "SPIDERMON_SPIDER_CLOSE_MONITORS"
+            ),
+            engine_stopped_suites=crawler.settings.getlist(
+                "SPIDERMON_ENGINE_STOP_MONITORS"
+            ),
+            spider_opened_expression_suites=crawler.settings.getlist(
+                "SPIDERMON_SPIDER_OPEN_EXPRESSION_MONITORS"
+            ),
+            spider_closed_expression_suites=crawler.settings.getlist(
+                "SPIDERMON_SPIDER_CLOSE_EXPRESSION_MONITORS"
+            ),
+            engine_stopped_expression_suites=crawler.settings.getlist(
+                "SPIDERMON_ENGINE_STOP_EXPRESSION_MONITORS"
+            ),
+            expressions_monitor_class=crawler.settings.get(
+                "SPIDERMON_EXPRESSIONS_MONITOR_CLASS"
+            ),
+            periodic_suites=crawler.settings.getdict("SPIDERMON_PERIODIC_MONITORS"),
         )
         crawler.signals.connect(ext.spider_opened, signal=signals.spider_opened)
         crawler.signals.connect(ext.spider_closed, signal=signals.spider_closed)
+        crawler.signals.connect(ext.engine_stopped, signal=signals.engine_stopped)
         return ext
 
     def spider_opened(self, spider):
         self._run_suites(spider, self.spider_opened_suites)
         self.periodic_tasks[spider] = []
         for suite, time in self.periodic_suites.items():
             task = LoopingCall(self._run_periodic_suites, spider, [suite])
@@ -80,24 +114,28 @@
             task.start(time, now=False)
 
     def spider_closed(self, spider):
         self._run_suites(spider, self.spider_closed_suites)
         for task in self.periodic_tasks[spider]:
             task.stop()
 
+    def engine_stopped(self):
+        spider = self.crawler.spider
+        self._run_suites(spider, self.engine_stopped_suites)
+
     def _run_periodic_suites(self, spider, suites):
         suites = [self.load_suite(s) for s in suites]
         self._run_suites(spider, suites)
 
     def _run_suites(self, spider, suites):
         data = self._generate_data_for_spider(spider)
         for suite in suites:
             runner = SpiderMonitorRunner(spider=spider)
             runner.run(suite, **data)
 
     def _generate_data_for_spider(self, spider):
         return {
-            'stats': self.crawler.stats.get_stats(spider),
-            'crawler': self.crawler,
-            'spider': spider,
-            'job': hs.job if hs.available else None,
+            "stats": self.crawler.stats.get_stats(spider),
+            "crawler": self.crawler,
+            "spider": spider,
+            "job": hs.job if hs.available else None,
         }
```

### Comparing `spidermon-1.8.0/spidermon/contrib/scrapy/pipelines.py` & `spidermon-1.9.0/spidermon/contrib/scrapy/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,28 @@
 
 from spidermon.contrib.validation import SchematicsValidator, JSONSchemaValidator
 from schematics.models import Model
 
 from .stats import ValidationStatsManager
 
 
-DEFAULT_ERRORS_FIELD = '_validation'
+DEFAULT_ERRORS_FIELD = "_validation"
 DEFAULT_ADD_ERRORS_TO_ITEM = False
 DEFAULT_DROP_ITEMS_WITH_ERRORS = False
 
 
 class ItemValidationPipeline(object):
-
-    def __init__(self, validators, stats,
-                 drop_items_with_errors=DEFAULT_DROP_ITEMS_WITH_ERRORS,
-                 add_errors_to_items=DEFAULT_ADD_ERRORS_TO_ITEM,
-                 errors_field=None):
+    def __init__(
+        self,
+        validators,
+        stats,
+        drop_items_with_errors=DEFAULT_DROP_ITEMS_WITH_ERRORS,
+        add_errors_to_items=DEFAULT_ADD_ERRORS_TO_ITEM,
+        errors_field=None,
+    ):
         self.drop_items_with_errors = drop_items_with_errors
         self.add_errors_to_items = add_errors_to_items or DEFAULT_ADD_ERRORS_TO_ITEM
         self.errors_field = errors_field or DEFAULT_ERRORS_FIELD
         self.validators = validators
         self.stats = ValidationStatsManager(stats)
         for _type, vals in validators.items():
             [self.stats.add_validator(_type, val.name) for val in vals]
@@ -46,59 +49,69 @@
             for obj, paths in schema.items():
                 key = obj.__name__
                 paths = paths if type(paths) in (list, tuple) else [paths]
                 objects = [loader(v) for v in paths]
                 validators[key].extend(objects)
 
         for loader, name in [
-            (cls._load_jsonschema_validator, 'SPIDERMON_VALIDATION_SCHEMAS'),
-            (cls._load_schematics_validator, 'SPIDERMON_VALIDATION_MODELS'),
+            (cls._load_jsonschema_validator, "SPIDERMON_VALIDATION_SCHEMAS"),
+            (cls._load_schematics_validator, "SPIDERMON_VALIDATION_MODELS"),
         ]:
             res = crawler.settings.get(name)
             if not res:
                 continue
             if type(res) not in allowed_types:
-                raise NotConfigured('Invalid <{}> type for <{}> settings, dict or list/tuple'
-                                    'is required'.format(type(res), name))
+                raise NotConfigured(
+                    "Invalid <{}> type for <{}> settings, dict or list/tuple"
+                    "is required".format(type(res), name)
+                )
             set_validators(loader, res)
 
         if not validators:
             raise NotConfigured("No validators were found")
 
         return cls(
             validators=validators,
             stats=crawler.stats,
-            drop_items_with_errors=crawler.settings.getbool('SPIDERMON_VALIDATION_DROP_ITEMS_WITH_ERRORS'),
-            add_errors_to_items=crawler.settings.getbool('SPIDERMON_VALIDATION_ADD_ERRORS_TO_ITEMS'),
-            errors_field=crawler.settings.get('SPIDERMON_VALIDATION_ERRORS_FIELD'),
+            drop_items_with_errors=crawler.settings.getbool(
+                "SPIDERMON_VALIDATION_DROP_ITEMS_WITH_ERRORS"
+            ),
+            add_errors_to_items=crawler.settings.getbool(
+                "SPIDERMON_VALIDATION_ADD_ERRORS_TO_ITEMS"
+            ),
+            errors_field=crawler.settings.get("SPIDERMON_VALIDATION_ERRORS_FIELD"),
         )
 
     @classmethod
     def _load_jsonschema_validator(cls, schema):
         if isinstance(schema, six.string_types):
-            if schema.endswith('.json'):
-                with open(schema, 'r') as f:
+            if schema.endswith(".json"):
+                with open(schema, "r") as f:
                     schema = json.load(f)
             else:
                 schema = load_object(schema)
                 if isinstance(schema, six.string_types):
                     schema = json.loads(schema)
         if not isinstance(schema, dict):
-            raise NotConfigured('Invalid schema, jsonschemas must be defined as:\n'
-                                '- a python dict.\n'
-                                '- an object path to a python dict.\n'
-                                '- an object path to a JSON string.\n'
-                                '- a path to a JSON file.')
+            raise NotConfigured(
+                "Invalid schema, jsonschemas must be defined as:\n"
+                "- a python dict.\n"
+                "- an object path to a python dict.\n"
+                "- an object path to a JSON string.\n"
+                "- a path to a JSON file."
+            )
         return JSONSchemaValidator(schema)
 
     @classmethod
     def _load_schematics_validator(cls, model_path):
         model_class = load_object(model_path)
         if not issubclass(model_class, Model):
-            raise NotConfigured('Invalid model, models must subclass schematics.models.Model')
+            raise NotConfigured(
+                "Invalid model, models must subclass schematics.models.Model"
+            )
         return SchematicsValidator(model_class)
 
     def process_item(self, item, _):
         validators = self.find_validators(item)
         if not validators:
             # No validators match this specific item type
             return item
@@ -120,16 +133,15 @@
         find = lambda x: self.validators.get(x.__name__, [])
         return find(item.__class__) or find(Item)
 
     def _convert_item_to_dict(self, item):
         serialized_json = BytesIO()
         exporter = JsonLinesItemExporter(serialized_json)
         exporter.export_item(item)
-        data = json.loads(to_native_str(
-            serialized_json.getvalue(), exporter.encoding))
+        data = json.loads(to_native_str(serialized_json.getvalue(), exporter.encoding))
         serialized_json.close()
         return data
 
     def _add_errors_to_item(self, item, errors):
         try:
             if self.errors_field not in item.__class__.fields:
                 item.__class__.fields[self.errors_field] = Field()
@@ -146,15 +158,15 @@
         """
         This method drops the item after detecting validation errors. Note
         that you could override it to add more details about the item that
         is being dropped or to drop the item only when some specific errors
         are detected.
         """
         self.stats.add_dropped_item()
-        raise DropItem('Validation failed!')
+        raise DropItem("Validation failed!")
 
     def _add_error_stats(self, errors):
         """
         This method adds validation error stats that can be later used to
         detect alert conditions in the monitors.
         """
         for field_name, messages in errors.items():
```

### Comparing `spidermon-1.8.0/spidermon/contrib/scrapy/stats.py` & `spidermon-1.9.0/spidermon/contrib/scrapy/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from __future__ import absolute_import
 from slugify import slugify
 
 
-STATS_DEFAULT_VALIDATION_PREFIX = 'spidermon/validation'
+STATS_DEFAULT_VALIDATION_PREFIX = "spidermon/validation"
 
 
 class NAMES:
-    ITEMS = 'items'
-    DROPPED = 'dropped'
-    FIELDS = 'fields'
-    ERRORS = 'errors'
-    VALIDATORS = 'validators'
+    ITEMS = "items"
+    DROPPED = "dropped"
+    FIELDS = "fields"
+    ERRORS = "errors"
+    VALIDATORS = "validators"
 
 
 class ValidationStatsManager(object):
     def __init__(self, stats, prefix=None, slugify=True):
         self.stats = stats
         self.prefix = prefix or STATS_DEFAULT_VALIDATION_PREFIX
         self.slugify = slugify
 
     def add_validator(self, type, class_name):
         self.stats.inc_value(self._get_stats_name(NAMES.VALIDATORS))
-        self.stats.set_value(self._get_stats_name(NAMES.VALIDATORS, type, class_name), True)
+        self.stats.set_value(
+            self._get_stats_name(NAMES.VALIDATORS, type, class_name), True
+        )
 
     def add_field_error(self, field, error):
         self.stats.inc_value(self._get_stats_name(NAMES.FIELDS, NAMES.ERRORS))
         self.stats.inc_value(self._get_stats_name(NAMES.FIELDS, NAMES.ERRORS, error))
-        self.stats.inc_value(self._get_stats_name(NAMES.FIELDS, NAMES.ERRORS, error) + '/' + field)
+        self.stats.inc_value(
+            self._get_stats_name(NAMES.FIELDS, NAMES.ERRORS, error) + "/" + field
+        )
 
     def add_fields(self, count):
         self.stats.inc_value(self._get_stats_name(NAMES.FIELDS), count=count)
 
     def add_item(self):
         self.stats.inc_value(self._get_stats_name(NAMES.ITEMS))
 
     def add_dropped_item(self):
         self.stats.inc_value(self._get_stats_name(NAMES.ITEMS, NAMES.DROPPED))
 
     def add_item_with_errors(self):
         self.stats.inc_value(self._get_stats_name(NAMES.ITEMS, NAMES.ERRORS))
 
     def _get_stats_name(self, *names):
-        return '/'.join([self.prefix] + list([self._get_name(n) for n in names]))
+        return "/".join([self.prefix] + list([self._get_name(n) for n in names]))
 
     def _get_name(self, name):
-        return slugify(text=name, separator='_').lower() if self.slugify else name
+        return slugify(text=name, separator="_").lower() if self.slugify else name
```

### Comparing `spidermon-1.8.0/spidermon/contrib/scrapy/runners.py` & `spidermon-1.9.0/spidermon/contrib/scrapy/runners.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import absolute_import
 
 import logging
 
-from spidermon.results.monitor import (MonitorResult, actions_step_required,
-                                       monitors_step_required)
+from spidermon.results.monitor import (
+    MonitorResult,
+    actions_step_required,
+    monitors_step_required,
+)
 from spidermon.runners import MonitorRunner
 from spidermon.utils.text import Message, line, line_title
 
-LOG_MESSAGE_HEADER = 'Spidermon'
+LOG_MESSAGE_HEADER = "Spidermon"
 
 
 class SpiderMonitorResult(MonitorResult):
-
     def __init__(self, spider):
         super(SpiderMonitorResult, self).__init__()
         self.spider = spider
 
     def next_step(self):
         super(SpiderMonitorResult, self).next_step()
         self.write_title()
@@ -73,53 +75,59 @@
         super(SpiderMonitorResult, self).add_action_error(action, error)
         self.write_item_result(action)
 
     def write_title(self):
         self.log_info(line_title(self.step.name))
 
     def write_item_result(self, item, extra=None):
-        self.log_info('%s... %s%s' % (item.name, self.step[item].status, ' (%s)' % extra if extra else ''))
+        self.log_info(
+            "%s... %s%s"
+            % (item.name, self.step[item].status, " (%s)" % extra if extra else "")
+        )
 
     def write_run_footer(self):
-        self.log_info("{count:d} {item_name}{plural_suffix} in {time:.3f}s".format(
-            count=self.step.number_of_items,
-            item_name=self.step.item_result_class.name,
-            plural_suffix='' if self.step.number_of_items == 1 else 's',
-            time=self.step.time_taken,
-        ))
+        self.log_info(
+            "{count:d} {item_name}{plural_suffix} in {time:.3f}s".format(
+                count=self.step.number_of_items,
+                item_name=self.step.item_result_class.name,
+                plural_suffix="" if self.step.number_of_items == 1 else "s",
+                time=self.step.time_taken,
+            )
+        )
 
     def write_step_summary(self):
-        summary = ('OK' if self.step.successful else 'FAILED')
+        summary = "OK" if self.step.successful else "FAILED"
         infos = self.step.get_infos()
         if infos and sum(infos.values()):
-            summary += ' (%s)' % ', '.join(['%s=%s' % (k, v) for k, v in infos.items() if v])
+            summary += " (%s)" % ", ".join(
+                ["%s=%s" % (k, v) for k, v in infos.items() if v]
+            )
         self.log_info(summary)
 
     def write_errors(self):
         for status in self.step.error_statuses:
             for item in self.step.items_for_status(status):
                 msg = Message()
                 msg.write_line()
                 msg.write_bold_separator()
-                msg.write_line('%s: %s' % (item.status, item.item.name))
+                msg.write_line("%s: %s" % (item.status, item.item.name))
                 msg.write_light_separator()
                 msg.write(item.error)
                 self.log_error(msg)
 
     def log_error(self, msg):
         self.log(msg, level=logging.ERROR)
 
     def log_info(self, msg):
         self.log(msg, level=logging.INFO)
 
     def log(self, msg, level=logging.DEBUG):
-        self.spider.log('[%s] %s' % (LOG_MESSAGE_HEADER, msg), level=level)
+        self.spider.log("[%s] %s" % (LOG_MESSAGE_HEADER, msg), level=level)
 
 
 class SpiderMonitorRunner(MonitorRunner):
-
     def __init__(self, spider):
         super(SpiderMonitorRunner, self).__init__()
         self.spider = spider
 
     def create_result(self):
         return SpiderMonitorResult(self.spider)
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/validator.py` & `spidermon-1.9.0/spidermon/contrib/validation/validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import absolute_import
 import re
 from collections import defaultdict
 
 
-RE_PATTERN_INSTANCE = type(re.compile(''))
+RE_PATTERN_INSTANCE = type(re.compile(""))
 
 
 class Validator(object):
     default_translator = None
-    name = 'validator'
+    name = "validator"
 
     def __init__(self, translator=None, use_default_translator=True):
         self._errors = defaultdict(list)
         if not translator and use_default_translator and self.default_translator:
             translator = self.default_translator
         self._translator = translator
 
@@ -32,13 +32,19 @@
         return len(self._errors) > 0
 
     @property
     def errors(self):
         if not self._translator:
             return self._errors
         else:
-            return dict([(field_name, self._translator.translate_messages(messages))
-                         for field_name, messages in self._errors.items()])
+            return dict(
+                [
+                    (field_name, self._translator.translate_messages(messages))
+                    for field_name, messages in self._errors.items()
+                ]
+            )
 
     def _add_errors(self, errors):
         for field_name, messages in errors.items():
-            self._errors[field_name] += messages if isinstance(messages, list) else [messages]
+            self._errors[field_name] += (
+                messages if isinstance(messages, list) else [messages]
+            )
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/translator.py` & `spidermon-1.9.0/spidermon/contrib/validation/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
         return [self.translate_message(m) for m in messages]
 
     def translate_message(self, message):
         for target_message, pattern in self.compiled_messages.items():
             if pattern.search(message):
                 return self.messages[target_message]  # TO-DO: Add substitution?
         return message
-
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/schematics/validator.py` & `spidermon-1.9.0/spidermon/contrib/validation/schematics/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 from spidermon.contrib.validation.validator import Validator
 from .translator import SchematicsMessageTranslator
 from . import monkeypatches
 
 
 class SchematicsValidator(Validator):
     default_translator = SchematicsMessageTranslator()
-    name = 'Schematics'
+    name = "Schematics"
 
     def __init__(self, model, translator=None, use_default_translator=True):
         super(SchematicsValidator, self).__init__(
-            translator=translator,
-            use_default_translator=use_default_translator,
+            translator=translator, use_default_translator=use_default_translator
         )
         self._model = model
         self._fields_required = {}
         self._save_required_fields()
         self._data = {}
 
     def _validate(self, data, strict=False):
@@ -58,51 +57,60 @@
             self._model._fields[field_name].required = required
 
     def _set_field_as_not_required(self, field_name):
         if field_name in self._model._fields:
             self._model._fields[field_name].required = False
 
     def _add_errors(self, errors):
-        if schematics.__version__.startswith('1.'):
+        if schematics.__version__.startswith("1."):
             for field_name, messages in errors.items():
                 if isinstance(messages, dict):
-                    transformed_errors = self._get_transformed_child_errors(field_name, messages)
+                    transformed_errors = self._get_transformed_child_errors(
+                        field_name, messages
+                    )
                     self._add_errors(transformed_errors)
                 else:
-                    self._errors[field_name] += messages if isinstance(messages, list) else [messages]
+                    self._errors[field_name] += (
+                        messages if isinstance(messages, list) else [messages]
+                    )
         else:
             from schematics.datastructures import FrozenDict
 
             for field_name, messages in errors.items():
                 if isinstance(messages, (dict, FrozenDict)):
-                    transformed_errors = self._get_transformed_child_errors(field_name, messages)
+                    transformed_errors = self._get_transformed_child_errors(
+                        field_name, messages
+                    )
                     self._add_errors(transformed_errors)
                 else:
                     messages = self._clean_messages(messages)
                     self._errors[field_name] += messages
 
     def _get_transformed_child_errors(self, field_name, errors):
-        return dict([('%s.%s' % (field_name, k), v) for k, v in errors.items()])
+        return dict([("%s.%s" % (field_name, k), v) for k, v in errors.items()])
 
     def _clean_messages(self, messages):
         """
         This is necessary when using Schematics 2.*, because it encapsulates
         the validation error messages in a different way.
         """
-        from schematics.exceptions import BaseError
+        from schematics.exceptions import BaseError, ErrorMessage
         from schematics.datastructures import FrozenList
 
-        if not isinstance(messages, list):
+        if type(messages) not in (list, FrozenList):
             messages = [messages]
 
         clean_messages = []
         for message in messages:
             if isinstance(message, BaseError):
                 message = message.messages
-                if isinstance(message, FrozenList):
-                    for err in message:
-                        # err is an ErrorMessage object
-                        clean_messages.append(str(err))
+
+            if isinstance(message, ErrorMessage):
+                clean_messages.append(message.summary)
+            elif isinstance(message, FrozenList):
+                for err in message:
+                    # err is an ErrorMessage object
+                    clean_messages.append(err.summary)
             else:
                 clean_messages.append(message)
 
         return clean_messages
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/schematics/monkeypatches.py` & `spidermon-1.9.0/spidermon/contrib/validation/schematics/monkeypatches.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
     def _force_list(self, value):
         if value is None or value == EMPTY_LIST:
             return []
         try:
             return list(value)
         except Exception as e:
-            raise ConversionError('Invalid list')
+            raise ConversionError("Invalid list")
+
     ListType._force_list = _force_list
 
 
 # Apply monkeypatches
-if schematics.__version__.startswith('1.'):
+if schematics.__version__.startswith("1."):
     monkeypatch_urltype()
     monkeypatch_listtype()
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/utils.py` & `spidermon-1.9.0/spidermon/contrib/validation/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import absolute_import
 import re
 
 URL_REGEX = re.compile(
-    r'^(?:http|ftp)s?://'  # http:// or https://
-    r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'  # domain...
-    r'localhost|' # localhost...
-    r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # ...or ip
-    r'(?::\d+)?'  # optional port
-    r'(?:/?|[/?]\S+)$', re.IGNORECASE)
+    r"^(?:http|ftp)s?://"  # http:// or https://
+    r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"  # domain...
+    r"localhost|"  # localhost...
+    r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"  # ...or ip
+    r"(?::\d+)?"  # optional port
+    r"(?:/?|[/?]\S+)$",
+    re.IGNORECASE,
+)
 
 EMAIL_REGEX = re.compile(
     # dot-atom
     r"(^[-!#$%&'*+/=?^_`{}|~0-9A-Z]+(\.[-!#$%&'*+/=?^_`{}|~0-9A-Z]+)*"
     # quoted-string
-    r'|^"([\001-\010\013\014\016-\037!#-\[\]-\177]|\\[\001-011\013\014\016'
-    r'-\177])*"'
+    r'|^"([\001-\010\013\014\016-\037!#-\[\]-\177]|\\[\001-011\013\014\016' r'-\177])*"'
     # domain
-    r')@(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+[A-Z]{2,32}\.?$',
-    re.IGNORECASE
+    r")@(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+[A-Z]{2,32}\.?$",
+    re.IGNORECASE,
 )
 
 
 def is_valid_url(url):
     return not URL_REGEX.match(url) is None
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/jsonschema/validator.py` & `spidermon-1.9.0/spidermon/contrib/validation/jsonschema/validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from __future__ import absolute_import
 import re
 
-from jsonschema.validators import Draft4Validator
-
+from jsonschema.validators import validator_for
 from spidermon.contrib.validation.validator import Validator
 
 from .translator import JSONSchemaMessageTranslator
 from .formats import format_checker
 
 
 REQUIRED_RE = re.compile("'(.+)' is a required property")
 
 
 class JSONSchemaValidator(Validator):
     default_translator = JSONSchemaMessageTranslator()
-    name = 'JSONSchema'
+    name = "JSONSchema"
 
     def __init__(self, schema, translator=None, use_default_translator=True):
         super(JSONSchemaValidator, self).__init__(
-            translator=translator,
-            use_default_translator=use_default_translator,
+            translator=translator, use_default_translator=use_default_translator
         )
         self._schema = schema
 
     def _validate(self, data, strict=False):
-        validator = Draft4Validator(
-            schema=self._schema,
-            format_checker=format_checker,
-        )
+        validator_cls = validator_for(self._schema)
+        validator = validator_cls(schema=self._schema, format_checker=format_checker)
         errors = validator.iter_errors(data)
-        for e in errors:
-            #print e
-            absolute_path = list(e.absolute_path)
-            required_match = REQUIRED_RE.search(e.message)
+
+        for error in errors:
+            absolute_path = list(error.absolute_path)
+            required_match = REQUIRED_RE.search(error.message)
             if required_match:
                 absolute_path.append(required_match.group(1))
-            field_name = '.'.join([str(p) for p in absolute_path])
-            self._add_errors({field_name: [e.message]})
+            field_name = ".".join([str(p) for p in absolute_path])
+            self._add_errors({field_name: [error.message]})
```

### Comparing `spidermon-1.8.0/spidermon/contrib/validation/jsonschema/translator.py` & `spidermon-1.9.0/spidermon/contrib/validation/jsonschema/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,43 @@
 from __future__ import absolute_import
 from spidermon.contrib.validation.translator import MessageTranslator
 from spidermon.contrib.validation import messages
 
 
 class JSONSchemaMessageTranslator(MessageTranslator):
     messages = {
-        r"^.+ is a required property$":                         messages.MISSING_REQUIRED_FIELD,
-
-        r"^.+ is not of type u?'array'$":                       messages.INVALID_ARRAY,
-        r"^.+ is not of type u?'boolean'$":                     messages.INVALID_BOOLEAN,
-        r"^.+ is not of type u?'integer'$":                     messages.INVALID_INT,
-        r"^.+ is not of type u?'number'$":                      messages.INVALID_NUMBER,
-        r"^.+ is not of type u?'object'$":                      messages.INVALID_OBJECT,
-        r"^.+ is not of type u?'string'$":                      messages.INVALID_STRING,
-        r"^.+ is not of type u?'null'$":                        messages.NOT_NULL,
-
-        r"^.+ is not valid under any of the given schemas$":    messages.NOT_VALID_UNDER_ANY_SCHEMA,
-        r"^.+ is valid under each of .+$":                      messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS,
-
-        r"^Additional items are not allowed .*$":               messages.TOO_MANY_ITEMS,
-        r"^Additional properties are not allowed .*$":          messages.UNEXPECTED_FIELD,
-
-        r"^.+ is a dependency of .+$":                          messages.MISSING_DEPENDENT_FIELD,
-        r"^.* is not one of .+$":                               messages.VALUE_NOT_IN_CHOICES,
-
-        r"^.* is not a 'date-time'$":                           messages.INVALID_DATETIME,
-        r"^.* is not a 'email'$":                               messages.INVALID_EMAIL,
-        r"^.* is not a 'ipv4'$":                                messages.INVALID_IPV4,
-        r"^.* is not a 'ipv6'$":                                messages.INVALID_IPV6,
-        r"^.* is not a 'hostname'$":                            messages.INVALID_HOSTNAME,
-        r"^.* is not a 'url'$":                                 messages.INVALID_URL,
-        r"^.* is not a 'uri'$":                                 messages.INVALID_URI,
-        r"^.* is not a 'regex'$":                               messages.INVALID_REGEX,
-        r"^.* is not a 'color'$":                               messages.INVALID_COLOR,
-
-        r"^.* has too many properties$":                        messages.TOO_MANY_PROPERTIES,
-        r"^.* does not have enough properties":                 messages.NOT_ENOUGH_PROPERTIES,
-
-        r"^.* is greater than the maximum of .*$":              messages.NUMBER_TOO_HIGH,
-        r"^.* is greater than or equal to the maximum of .*$":  messages.NUMBER_TOO_HIGH,
-
-        r"^.* is less than the minimum of .*$":                 messages.NUMBER_TOO_LOW,
-        r"^.* is less than or equal to the minimum of .*$":     messages.NUMBER_TOO_LOW,
-
-        r"^.* is not a multiple of .*$":                        messages.NOT_MULTIPLE_OF,
-
-        r"^.* is not allowed for .*$":                          messages.NOT_ALLOWED_VALUE,
-
-
-        r"^.+ is too short$":                                   messages.FIELD_TOO_SHORT,
-        r"^.+ is too long$":                                    messages.FIELD_TOO_LONG,
-
-        r"^.+ does not match .*$":                              messages.REGEX_NOT_MATCHED,
-        r"^.+ has non-unique elements$":                        messages.NOT_UNIQUE,
+        r"^.+ is a required property$": messages.MISSING_REQUIRED_FIELD,
+        r"^.+ is not of type u?'array'$": messages.INVALID_ARRAY,
+        r"^.+ is not of type u?'boolean'$": messages.INVALID_BOOLEAN,
+        r"^.+ is not of type u?'integer'$": messages.INVALID_INT,
+        r"^.+ is not of type u?'number'$": messages.INVALID_NUMBER,
+        r"^.+ is not of type u?'object'$": messages.INVALID_OBJECT,
+        r"^.+ is not of type u?'string'$": messages.INVALID_STRING,
+        r"^.+ is not of type u?'null'$": messages.NOT_NULL,
+        r"^.+ is not valid under any of the given schemas$": messages.NOT_VALID_UNDER_ANY_SCHEMA,
+        r"^.+ is valid under each of .+$": messages.VALID_FOR_SEVERAL_EXCLUSIVE_SCHEMAS,
+        r"^Additional items are not allowed .*$": messages.TOO_MANY_ITEMS,
+        r"^Additional properties are not allowed .*$": messages.UNEXPECTED_FIELD,
+        r"^.+ is a dependency of .+$": messages.MISSING_DEPENDENT_FIELD,
+        r"^.* is not one of .+$": messages.VALUE_NOT_IN_CHOICES,
+        r"^.* is not a 'date-time'$": messages.INVALID_DATETIME,
+        r"^.* is not a 'email'$": messages.INVALID_EMAIL,
+        r"^.* is not a 'ipv4'$": messages.INVALID_IPV4,
+        r"^.* is not a 'ipv6'$": messages.INVALID_IPV6,
+        r"^.* is not a 'hostname'$": messages.INVALID_HOSTNAME,
+        r"^.* is not a 'url'$": messages.INVALID_URL,
+        r"^.* is not a 'uri'$": messages.INVALID_URI,
+        r"^.* is not a 'regex'$": messages.INVALID_REGEX,
+        r"^.* is not a 'color'$": messages.INVALID_COLOR,
+        r"^.* has too many properties$": messages.TOO_MANY_PROPERTIES,
+        r"^.* does not have enough properties": messages.NOT_ENOUGH_PROPERTIES,
+        r"^.* is greater than the maximum of .*$": messages.NUMBER_TOO_HIGH,
+        r"^.* is greater than or equal to the maximum of .*$": messages.NUMBER_TOO_HIGH,
+        r"^.* is less than the minimum of .*$": messages.NUMBER_TOO_LOW,
+        r"^.* is less than or equal to the minimum of .*$": messages.NUMBER_TOO_LOW,
+        r"^.* is not a multiple of .*$": messages.NOT_MULTIPLE_OF,
+        r"^.* is not allowed for .*$": messages.NOT_ALLOWED_VALUE,
+        r"^.+ is too short$": messages.FIELD_TOO_SHORT,
+        r"^.+ is too long$": messages.FIELD_TOO_LONG,
+        r"^.+ does not match .*$": messages.REGEX_NOT_MATCHED,
+        r"^.+ has non-unique elements$": messages.NOT_UNIQUE,
     }
-
```

### Comparing `spidermon-1.8.0/spidermon/contrib/stats/analyzer.py` & `spidermon-1.9.0/spidermon/contrib/stats/analyzer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import absolute_import
 import re
 
 
 class StatsAnalyzer(object):
     def __init__(self, stats, prefix=None):
         self.stats = stats
-        self.prefix = prefix or ''
+        self.prefix = prefix or ""
 
     def search(self, pattern, include_matches=False):
         pattern = re.compile(self._get_pattern(pattern))
         results = {}
         for key, count in self.stats.items():
             match = pattern.match(key)
             if match:
                 if include_matches:
-                    results[key] = (count, match.group(1) if len(match.groups()) else '')
+                    results[key] = (
+                        count,
+                        match.group(1) if len(match.groups()) else "",
+                    )
                 else:
                     results[key] = count
         return results
 
     def _get_pattern(self, pattern):
         if self.prefix:
-            return '/'.join([self.prefix, pattern])
+            return "/".join([self.prefix, pattern])
         else:
-            return pattern
+            return pattern
```

### Comparing `spidermon-1.8.0/spidermon/contrib/stats/counters.py` & `spidermon-1.9.0/spidermon/contrib/stats/counters.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
     @property
     def count(self):
         raise NotImplementedError
 
     @property
     def percent(self):
-        if self._total <= 0 or self.count <=0:
+        if self._total <= 0 or self.count <= 0:
             return 0
         else:
             return float(self.count) / float(self._total)
 
     def __str__(self):
-        return '(count=%d, percent=%.2f)' % (self.count, self.percent)
+        return "(count=%d, percent=%.2f)" % (self.count, self.percent)
 
     def __repr__(self):
         return self.__str__()
 
 
 class PercentCounter(PercentCounterBase):
     def __init__(self, count=0, total=0):
@@ -71,26 +71,26 @@
     def __keytransform__(self, key):
         return key
 
     def _immutable(self, *args, **kws):
         raise TypeError
 
     def __str__(self):
-        return '(count=%d, percent=%.2f, %s)' % (
+        return "(count=%d, percent=%.2f, %s)" % (
             self.count,
             self.percent,
             str(self._dict),
         )
 
     __setitem__ = _immutable
     __delitem__ = _immutable
 
 
 class AttributeDictPercentCounter(PercentCounterBase):
-    __attribute_dict_name__ = 'dict'
+    __attribute_dict_name__ = "dict"
 
     def __init__(self, total):
         super(AttributeDictPercentCounter, self).__init__(total)
         setattr(self, self.__attribute_dict_name__, DictPercentCounter(total))
 
     @property
     def attribute_dict(self):
@@ -100,16 +100,16 @@
     def count(self):
         return sum([e.count for e in self.attribute_dict.values()])
 
     def add_value(self, key, value):
         self.attribute_dict.add_value(key, value)
 
     def __str__(self):
-        return '(count=%d, percent=%.2f, %s=%s)' % (
+        return "(count=%d, percent=%.2f, %s=%s)" % (
             self.count,
             self.percent,
             self.__attribute_dict_name__,
-            str(self.attribute_dict)
+            str(self.attribute_dict),
         )
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `spidermon-1.8.0/spidermon/runners.py` & `spidermon-1.9.0/spidermon/runners.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 from spidermon.results.monitor import MonitorResult
 from spidermon.results.text import TextMonitorResult
 from spidermon.exceptions import InvalidMonitor, InvalidResult
 from spidermon.data import Data
 
 
 class MonitorRunner(object):
-    data_immutable_dicts = ['stats']
-    data_default_data = {
-        'meta': {},
-    }
+    data_immutable_dicts = ["stats"]
+    data_default_data = {"meta": {}}
 
     def __init__(self):
         self.suite = None
         self.result = None
         self.data = None
 
     def run(self, suite, **data):
         if not isinstance(suite, MonitorSuite):
-            raise InvalidMonitor('Runners must receive a MonitorSuite instance')
+            raise InvalidMonitor("Runners must receive a MonitorSuite instance")
         self.suite = suite
         data = dict(self.data_default_data, **data)
         self.data = self.transform_data(**data)
         self.suite.init_data(self.data)
         self.result = self.create_result()
         if not isinstance(self.result, MonitorResult):
-            raise InvalidResult('Runners must use a MonitorResult instance')
+            raise InvalidResult("Runners must use a MonitorResult instance")
         return self.run_suite()
 
     def transform_data(self, **data):
         data = data or {}
         new_data_dict = {}
         for attr_name, attr in data.items():
             if attr_name in self.data_immutable_dicts:
@@ -62,26 +60,26 @@
 
         # Run monitors passed actions
         self.result.next_step()
         if self.result.monitor_results and self.result.all_monitors_passed:
             self.run_monitors_passed()
         else:
             self.result.skip_all_step_actions(
-                actions=self.suite.monitors_passed_actions,
-                reason='A Monitor failed')
+                actions=self.suite.monitors_passed_actions, reason="A Monitor failed"
+            )
         self.result.finish_step()
 
         # Run monitors failed actions
         self.result.next_step()
         if self.result.monitor_results and not self.result.all_monitors_passed:
             self.run_monitors_failed()
         else:
             self.result.skip_all_step_actions(
-                actions=self.suite.monitors_failed_actions,
-                reason='No Monitors failed')
+                actions=self.suite.monitors_failed_actions, reason="No Monitors failed"
+            )
         self.result.finish_step()
 
     def run_monitors_finished(self):
         self.suite.on_monitors_finished(self.result)
         for action in self.suite.monitors_finished_actions:
             action.run(self.result, self.data)
```

### Comparing `spidermon-1.8.0/spidermon/data.py` & `spidermon-1.9.0/spidermon/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,27 @@
     example:
     >> s = Data({'scraped_items': 100})
     >> s['scraped_items']
     100
     >> s.scraped_items
     100
     """
+
     def __getattr__(self, name):
         if name in self:
             return self[name]
         else:
             raise AttributeError("Key '%s' not found." % name)
 
     def _immutable(self, *args, **kws):
-        raise InvalidDataOperation('Immutable Data! You cannot add or modify read-only data.')
+        raise InvalidDataOperation(
+            "Immutable Data! You cannot add or modify read-only data."
+        )
 
     update = _immutable
     setdefault = _immutable
     clear = _immutable
     pop = _immutable
     popitem = _immutable
     __setitem__ = _immutable
     __delitem__ = _immutable
-    __setattr__ = _immutable
+    __setattr__ = _immutable
```

### Comparing `spidermon-1.8.0/spidermon/settings.py` & `spidermon-1.9.0/spidermon/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # ----------------------------------
 # Status
 # ----------------------------------
-UNDEFINED_STATUS = '?'
+UNDEFINED_STATUS = "?"
 
 # ----------------------------------
 # Monitors
 # ----------------------------------
-_MONITOR_STATUS_SUCCESS = 'OK'
-_MONITOR_STATUS_FAILURE = 'FAIL'
-_MONITOR_STATUS_SKIPPED = 'SKIPPED'
-_MONITOR_STATUS_ERROR = 'ERROR'
-_MONITOR_STATUS_EXPECTED_FAILURE = 'EXPECTED FAILURE'
-_MONITOR_STATUS_UNEXPECTED_SUCCESS = 'UNEXPECTED SUCCESS'
-
-_MONITOR_LEVEL_HIGH = 'HIGH'
-_MONITOR_LEVEL_NORMAL = 'NORMAL'
-_MONITOR_LEVEL_LOW = 'LOW'
+_MONITOR_STATUS_SUCCESS = "OK"
+_MONITOR_STATUS_FAILURE = "FAIL"
+_MONITOR_STATUS_SKIPPED = "SKIPPED"
+_MONITOR_STATUS_ERROR = "ERROR"
+_MONITOR_STATUS_EXPECTED_FAILURE = "EXPECTED FAILURE"
+_MONITOR_STATUS_UNEXPECTED_SUCCESS = "UNEXPECTED SUCCESS"
+
+_MONITOR_LEVEL_HIGH = "HIGH"
+_MONITOR_LEVEL_NORMAL = "NORMAL"
+_MONITOR_LEVEL_LOW = "LOW"
 
 
 class MONITOR:
     class STATUS:
         SUCCESS = _MONITOR_STATUS_SUCCESS
         FAILURE = _MONITOR_STATUS_FAILURE
         SKIPPED = _MONITOR_STATUS_SKIPPED
@@ -38,90 +38,73 @@
         )
         SUCCESSFUL = (
             _MONITOR_STATUS_SUCCESS,
             _MONITOR_STATUS_SKIPPED,
             _MONITOR_STATUS_EXPECTED_FAILURE,
             _MONITOR_STATUS_UNEXPECTED_SUCCESS,
         )
-        ERROR = (
-            _MONITOR_STATUS_FAILURE,
-            _MONITOR_STATUS_ERROR,
-        )
+        ERROR = (_MONITOR_STATUS_FAILURE, _MONITOR_STATUS_ERROR)
         DEFAULT = UNDEFINED_STATUS
 
     class LEVEL:
         HIGH = _MONITOR_LEVEL_HIGH
         NORMAL = _MONITOR_LEVEL_NORMAL
         LOW = _MONITOR_LEVEL_LOW
 
     class LEVELS:
-        ALL = (
-            _MONITOR_LEVEL_HIGH,
-            _MONITOR_LEVEL_NORMAL,
-            _MONITOR_LEVEL_LOW,
-        )
+        ALL = (_MONITOR_LEVEL_HIGH, _MONITOR_LEVEL_NORMAL, _MONITOR_LEVEL_LOW)
         DEFAULT = _MONITOR_LEVEL_NORMAL
 
     DEFAULT_NAME = None
-    DEFAULT_DESCRIPTION = ''
+    DEFAULT_DESCRIPTION = ""
     DEFAULT_ORDER = 1
 
+
 # ----------------------------------
 # Actions
 # ----------------------------------
-_ACTION_STATUS_SUCCESS = 'OK'
-_ACTION_STATUS_ERROR = 'ERROR'
-_ACTION_STATUS_SKIPPED = 'SKIPPED'
+_ACTION_STATUS_SUCCESS = "OK"
+_ACTION_STATUS_ERROR = "ERROR"
+_ACTION_STATUS_SKIPPED = "SKIPPED"
 
 
 class ACTION:
     class STATUS:
         SUCCESS = _ACTION_STATUS_SUCCESS
         ERROR = _ACTION_STATUS_ERROR
         SKIPPED = _ACTION_STATUS_SKIPPED
 
     class STATUSES(object):
-        ALL = (
-            _ACTION_STATUS_SUCCESS,
-            _ACTION_STATUS_ERROR,
-            _ACTION_STATUS_SKIPPED,
-        )
-        SUCCESSFUL = (
-            _ACTION_STATUS_SUCCESS,
-            _ACTION_STATUS_SKIPPED,
-        )
-        ERROR = (
-            _ACTION_STATUS_ERROR,
-        )
+        ALL = (_ACTION_STATUS_SUCCESS, _ACTION_STATUS_ERROR, _ACTION_STATUS_SKIPPED)
+        SUCCESSFUL = (_ACTION_STATUS_SUCCESS, _ACTION_STATUS_SKIPPED)
+        ERROR = (_ACTION_STATUS_ERROR,)
         DEFAULT = UNDEFINED_STATUS
 
-    DEFAULT_DESCRIPTION = ''
+    DEFAULT_DESCRIPTION = ""
 
 
 # ----------------------------------
 # Steps
 # ----------------------------------
-_STEP_MONITORS = 'MONITORS'
-_STEP_MONITORS_FINISHED = 'FINISHED ACTIONS'
-_STEP_MONITORS_PASSED = 'PASSED ACTIONS'
-_STEP_MONITORS_FAILED = 'FAILED ACTIONS'
+_STEP_MONITORS = "MONITORS"
+_STEP_MONITORS_FINISHED = "FINISHED ACTIONS"
+_STEP_MONITORS_PASSED = "PASSED ACTIONS"
+_STEP_MONITORS_FAILED = "FAILED ACTIONS"
 
 
 class STEPS:
     MONITORS = _STEP_MONITORS
     MONITORS_FINISHED = _STEP_MONITORS_FINISHED
     MONITORS_PASSED = _STEP_MONITORS_PASSED
     MONITORS_FAILED = _STEP_MONITORS_FAILED
     ALL = (
         _STEP_MONITORS,
         _STEP_MONITORS_FINISHED,
         _STEP_MONITORS_PASSED,
         _STEP_MONITORS_FAILED,
     )
-    MONITOR_RELATED = (
-        _STEP_MONITORS,
-    )
+    MONITOR_RELATED = (_STEP_MONITORS,)
     ACTION_RELATED = (
         _STEP_MONITORS_FINISHED,
         _STEP_MONITORS_PASSED,
         _STEP_MONITORS_FAILED,
-    )
+    )
```

### Comparing `spidermon-1.8.0/spidermon/python/context.py` & `spidermon-1.9.0/spidermon/python/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import absolute_import
 from spidermon.exceptions import NotConfigured
 
 
 class Context(dict):
-    '''
+    """
     Stores context for python expressions.
 
     Also keeps track of not configured components (variables) of the context
     to throw NotConfigured exception in the right time, when test is
     evaluated by interpreter, instead of throwing it in building-context time
-    '''
+    """
+
     def __init__(self, *args, **kwargs):
         super(Context, self).__init__(*args, **kwargs)
         self._notconfigured = []
 
     def __getitem__(self, item):
         if item in self._notconfigured:
-            raise NotConfigured('{} not available!'.format(item))
+            raise NotConfigured("{} not available!".format(item))
         return super(Context, self).__getitem__(item)
 
     def extend_via_attrs(self, obj, attrs):
-        '''Extend context with names of object attributes and their values'''
+        """Extend context with names of object attributes and their values"""
         for attr in attrs:
             try:
                 super(Context, self).__setitem__(attr, getattr(obj, attr))
             except NotConfigured:
                 self._notconfigured.append(attr)
-
```

### Comparing `spidermon-1.8.0/spidermon/python/factory.py` & `spidermon-1.9.0/spidermon/python/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,57 +8,62 @@
 from spidermon.exceptions import InvalidMonitor, NotConfigured
 from spidermon import settings
 
 
 class PythonExpressionsMonitor(Monitor):
     _classes_counter = 0
     _test_methods_counter = 0
-    _test_methods_prefix = 'test'
+    _test_methods_prefix = "test"
 
     @classmethod
     def generate_class_name(cls):
         cls._classes_counter += 1
-        return '%s%d' % (cls.__name__, cls._classes_counter)
+        return "%s%d" % (cls.__name__, cls._classes_counter)
 
     @classmethod
     def generate_method_name(cls):
         cls._test_methods_counter += 1
-        return '%s_python_expression_%d' % (cls._test_methods_prefix,
-                                            cls._test_methods_counter)
+        return "%s_python_expression_%d" % (
+            cls._test_methods_prefix,
+            cls._test_methods_counter,
+        )
 
     def get_context_data(self):
-        raise NotConfigured('Context data needs to be set up')
+        raise NotConfigured("Context data needs to be set up")
 
 
 def create_monitor_class_from_json(monitor_json, monitor_class=None):
     monitor_dict = json.loads(monitor_json)
     validate(monitor_dict, schemas.MONITOR_SCHEMA)
     return create_monitor_class_from_dict(monitor_dict, monitor_class)
 
 
 def create_monitor_class_from_dict(monitor_dict, monitor_class=None):
     tests = []
-    for test in monitor_dict.get('tests', []):
-        tests.append((
-            test['expression'],
-            test.get('name', None),
-            test.get('description', None),
-            test.get('fail_message', None),
-        ))
+    for test in monitor_dict.get("tests", []):
+        tests.append(
+            (
+                test["expression"],
+                test.get("name", None),
+                test.get("description", None),
+                test.get("fail_message", None),
+            )
+        )
     klass = _create_monitor_class(tests, monitor_class)
-    klass.options.name = monitor_dict.get('name', settings.MONITOR.DEFAULT_NAME)
-    klass.options.description = monitor_dict.get('description',
-                                                 settings.MONITOR.DEFAULT_DESCRIPTION)
+    klass.options.name = monitor_dict.get("name", settings.MONITOR.DEFAULT_NAME)
+    klass.options.description = monitor_dict.get(
+        "description", settings.MONITOR.DEFAULT_DESCRIPTION
+    )
     return klass
 
 
 def _create_monitor_class(expressions, monitor_class=None):
     monitor_class = monitor_class or PythonExpressionsMonitor
     if not issubclass(monitor_class, PythonExpressionsMonitor):
-        msg = 'Python expressions monitors must subclass PythonExpressionsMonitor'
+        msg = "Python expressions monitors must subclass PythonExpressionsMonitor"
         raise InvalidMonitor(msg)
     klass = type(monitor_class.generate_class_name(), (monitor_class,), {})
     for e in expressions:
         if isinstance(e, tuple):
             method = _create_test_method(*e)
         else:
             method = _create_test_method(e)
@@ -68,17 +73,21 @@
 
 def _create_test_method(expression, name=None, description=None, fail_reason=None):
     def _test_method(self):
         interpreter = Interpreter()
         context = self.get_context_data()
         result = interpreter.eval(expression, context=context)
         if result is not None:
-            self.assertTrue(bool(result),
-                            msg=('Expression not safisfied: "%s"' % expression)
-                            if not fail_reason else
-                            interpreter.eval(fail_reason, context=context))
+            self.assertTrue(
+                bool(result),
+                msg=('Expression not safisfied: "%s"' % expression)
+                if not fail_reason
+                else interpreter.eval(fail_reason, context=context),
+            )
+
     test_method = _test_method
     MonitorOptions.add_or_create(test_method)
     test_method.options.name = name or settings.MONITOR.DEFAULT_NAME
-    test_method.options.description = description or settings.MONITOR.DEFAULT_DESCRIPTION
+    test_method.options.description = (
+        description or settings.MONITOR.DEFAULT_DESCRIPTION
+    )
     return test_method
-
```

### Comparing `spidermon-1.8.0/spidermon/python/schemas.py` & `spidermon-1.9.0/spidermon/python/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 MONITOR_SCHEMA = {
     "type": "object",
     "properties": {
-        "name": {"type" : "string", "minLength": 1},
-        "description": {"type" : "string", "minLength": 1},
+        "name": {"type": "string", "minLength": 1},
+        "description": {"type": "string", "minLength": 1},
         "tests": {
             "type": "array",
             "items": {
                 "type": "object",
                 "properties": {
-                    "name": {"type" : "string", "minLength": 1},
-                    "description": {"type" : "string", "minLength": 1},
-                    "expression": {"type" : "string", "minLength": 1},
-                    "fail_reason": {"type" : "string", "minLength": 1},
+                    "name": {"type": "string", "minLength": 1},
+                    "description": {"type": "string", "minLength": 1},
+                    "expression": {"type": "string", "minLength": 1},
+                    "fail_reason": {"type": "string", "minLength": 1},
                 },
                 "required": ["name", "expression"],
             },
         },
     },
     "required": ["name", "tests"],
-}
+}
```

### Comparing `spidermon-1.8.0/spidermon/exceptions.py` & `spidermon-1.9.0/spidermon/exceptions.py`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/spidermon/decorators/__init__.py` & `spidermon-1.9.0/spidermon/decorators/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 class DecoratorWithAttributes(object):
     name = None
     attributes = {}
 
     def __init__(self):
         if not self.name:
-            raise AttributeError('No name defined!')
+            raise AttributeError("No name defined!")
         if not self.attributes:
-            raise AttributeError('No attributes defined!')
+            raise AttributeError("No attributes defined!")
 
     def __getattr__(self, name):
         if name not in self.attributes:
-            raise AttributeError("Invalid {attribute} '{name}', allowed values: {values}".format(
-                attribute=self.name,
-                name=name,
-                values=', '.join(["'%s'" % attr for attr in self.attributes.keys()])))
+            raise AttributeError(
+                "Invalid {attribute} '{name}', allowed values: {values}".format(
+                    attribute=self.name,
+                    name=name,
+                    values=", ".join(
+                        ["'%s'" % attr for attr in self.attributes.keys()]
+                    ),
+                )
+            )
         else:
             return self.attributes[name]
 
 
 class OptionsDecorator(object):
     @classmethod
     def set_value(cls, options_class, value_name):
         def value_decorator(value):
             def decorator(fn):
                 options_class.add_or_create(fn)
                 setattr(fn.options, value_name, value)
                 return fn
+
             return decorator
+
         return value_decorator
 
     @classmethod
     def set_fixed_value(cls, options_class, value_name, value):
         def decorator(fn):
             options_class.add_or_create(fn)
             setattr(fn.options, value_name, value)
             return fn
+
         return decorator
```

### Comparing `spidermon-1.8.0/spidermon/templates.py` & `spidermon-1.9.0/spidermon/templates.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,45 +2,42 @@
 import inspect
 import os
 import datetime
 import pprint as pretty_print
 
 from jinja2 import Environment, FileSystemLoader, Template
 
-DEFAULT_TEMPLATE_FOLDERS = ['templates']
+DEFAULT_TEMPLATE_FOLDERS = ["templates"]
 
 
 def get_log_errors(logs):
-    return [e for e in logs.list() if e['level'] >= 40]
+    return [e for e in logs.list() if e["level"] >= 40]
 
 
 def make_list(obj):
     return list(obj)
 
 
 def pprint(obj):
     return pretty_print.pformat(obj)
 
 
 def format_time(time):
     if not isinstance(time, datetime.timedelta):
-        time = datetime.timedelta(seconds=int(time / 1000.))
-    return ':'.join(str(time).split(':')[:2])+'h'
+        time = datetime.timedelta(seconds=int(time / 1000.0))
+    return ":".join(str(time).split(":")[:2]) + "h"
 
 
 FILTERS = {
-    'pprint': pprint,
-    'list': make_list,
-    'get_log_errors': get_log_errors,
-    'format_time': format_time,
-}
-GLOBALS = {
-    'datetime': datetime,
-    'str': str,
+    "pprint": pprint,
+    "list": make_list,
+    "get_log_errors": get_log_errors,
+    "format_time": format_time,
 }
+GLOBALS = {"datetime": datetime, "str": str}
 
 
 class TemplateLoader(object):
     def __init__(self):
         self.paths = []
         self.reload_env()
 
@@ -55,28 +52,26 @@
             caller_folder = os.path.join(caller_folder, path)
         if folder:
             self.add_path(os.path.join(caller_folder, folder))
         else:
             self.discover_folder(caller_folder)
 
     def discover_folder(self, candidate_folder):
-        for folder in [os.path.join(candidate_folder, dir)
-                       for dir in DEFAULT_TEMPLATE_FOLDERS]:
+        for folder in [
+            os.path.join(candidate_folder, dir) for dir in DEFAULT_TEMPLATE_FOLDERS
+        ]:
             self.add_path(folder)
 
     def reload_env(self):
         loader = FileSystemLoader(self.paths)
-        self.env = Environment(
-            loader=loader,
-            lstrip_blocks=True,
-            trim_blocks=True,
-            )
+        self.env = Environment(loader=loader, lstrip_blocks=True, trim_blocks=True)
         for filter_name, filter in FILTERS.items():
             self.env.filters[filter_name] = filter
 
         for global_name, global_value in GLOBALS.items():
             self.env.globals[global_name] = global_value
 
     def get_template(self, name):
         return self.env.get_template(name)
 
+
 template_loader = TemplateLoader()
```

### Comparing `spidermon-1.8.0/spidermon/results/text.py` & `spidermon-1.9.0/spidermon/results/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 from spidermon.utils.text import line_title
 
 from .monitor import MonitorResult, monitors_step_required, actions_step_required
 
 
 DOTS = {
     # Monitors
-    settings.MONITOR.STATUS.SUCCESS: '.',
-    settings.MONITOR.STATUS.ERROR: 'E',
-    settings.MONITOR.STATUS.FAILURE: 'F',
-    settings.MONITOR.STATUS.SKIPPED: 's',
-    settings.MONITOR.STATUS.EXPECTED_FAILURE: 'x',
-    settings.MONITOR.STATUS.UNEXPECTED_SUCCESS: 'u',
-
+    settings.MONITOR.STATUS.SUCCESS: ".",
+    settings.MONITOR.STATUS.ERROR: "E",
+    settings.MONITOR.STATUS.FAILURE: "F",
+    settings.MONITOR.STATUS.SKIPPED: "s",
+    settings.MONITOR.STATUS.EXPECTED_FAILURE: "x",
+    settings.MONITOR.STATUS.UNEXPECTED_SUCCESS: "u",
     # Actions
-    settings.ACTION.STATUS.SUCCESS: '.',
-    settings.ACTION.STATUS.ERROR: 'E',
-    settings.ACTION.STATUS.SKIPPED: 's',
+    settings.ACTION.STATUS.SUCCESS: ".",
+    settings.ACTION.STATUS.ERROR: "E",
+    settings.ACTION.STATUS.SKIPPED: "s",
 }
 
 
 class TextMonitorResult(MonitorResult):
 
-    SEPARATOR_BOLD = '='
-    SEPARATOR_LIGHT = '-'
+    SEPARATOR_BOLD = "="
+    SEPARATOR_LIGHT = "-"
     LINE_LENGTH = 70
 
     def __init__(self, stream=sys.stderr, verbosity=1):
         super(TextMonitorResult, self).__init__()
         self.stream = stream
         self.show_all = verbosity > 1
         self.use_dots = verbosity == 1
@@ -106,27 +105,27 @@
     def write(self, text):
         self.stream.write(text)
 
     def write_flush(self):
         self.stream.flush()
 
     def write_line_light(self):
-        self.write_line(self.SEPARATOR_LIGHT*self.LINE_LENGTH)
+        self.write_line(self.SEPARATOR_LIGHT * self.LINE_LENGTH)
 
     def write_line_bold(self):
-        self.write_line(self.SEPARATOR_BOLD*self.LINE_LENGTH)
+        self.write_line(self.SEPARATOR_BOLD * self.LINE_LENGTH)
 
     def write_title(self, title):
         self.write_line(line_title(title))
 
     def write_line(self, text=None):
-        self.write('%s\n' % (text or ''))
+        self.write("%s\n" % (text or ""))
 
     def write_run_status(self, text, extra=None):
-        self.write_line('%s%s' % (text, ' (%s)' % extra if extra else ''))
+        self.write_line("%s%s" % (text, " (%s)" % extra if extra else ""))
 
     def write_run_start(self, item):
         if self.show_all:
             self.write(item.name)
             self.write(" ... ")
             self.write_flush()
 
@@ -135,33 +134,37 @@
             self.write_run_status(self.step[item].status, extra)
         elif self.use_dots:
             self.write(DOTS[self.step[item].status])
             self.write_flush()
 
     def write_run_footer(self):
         self.write_line_light()
-        self.write_line("{count:d} {item_name}{plural_suffix} in {time:.3f}s".format(
-            count=self.step.number_of_items,
-            item_name=self.step.item_result_class.name,
-            plural_suffix='' if self.step.number_of_items == 1 else 's',
-            time=self.step.time_taken,
-        ))
+        self.write_line(
+            "{count:d} {item_name}{plural_suffix} in {time:.3f}s".format(
+                count=self.step.number_of_items,
+                item_name=self.step.item_result_class.name,
+                plural_suffix="" if self.step.number_of_items == 1 else "s",
+                time=self.step.time_taken,
+            )
+        )
         self.write_line()
 
     def write_errors(self):
         self.write_line()
         for status in self.step.error_statuses:
             for item in self.step.items_for_status(status):
                 self.write_line_bold()
-                self.write_line('%s: %s' % (item.status, item.item.name))
+                self.write_line("%s: %s" % (item.status, item.item.name))
                 self.write_line_light()
                 self.write_line(item.error)
                 self.write_line()
 
     def write_step_summary(self):
-        self.write('OK' if self.step.successful else 'FAILED')
+        self.write("OK" if self.step.successful else "FAILED")
         infos = self.step.get_infos()
         if infos and sum(infos.values()):
-            self.write_line(' (%s)' % ', '.join(['%s=%s' % (k, v) for k, v in infos.items() if v]))
+            self.write_line(
+                " (%s)" % ", ".join(["%s=%s" % (k, v) for k, v in infos.items() if v])
+            )
         else:
             self.write_line()
         self.write_line()
```

### Comparing `spidermon-1.8.0/spidermon/results/monitor.py` & `spidermon-1.9.0/spidermon/results/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,45 @@
 def step_required_decorator(allowed_steps):
     def _step_required_decorator(fn):
         def decorator(self, *args, **kwargs):
             if self.step.name not in allowed_steps:
                 raise ValueError  # TO-DO
             else:
                 return fn(self, *args, **kwargs)
+
         return decorator
+
     return _step_required_decorator
 
+
 monitors_step_required = step_required_decorator(settings.STEPS.MONITOR_RELATED)
 actions_step_required = step_required_decorator(settings.STEPS.ACTION_RELATED)
 
 
 class MonitorResult(unittest.TestResult):
-
     def __init__(self):
         super(MonitorResult, self).__init__()
-        self._steps = OrderedDict([(step, self._get_step_class(step)(step))
-                                   for step in settings.STEPS.ALL])
+        self._steps = OrderedDict(
+            [(step, self._get_step_class(step)(step)) for step in settings.STEPS.ALL]
+        )
         self._current_step = None
 
     @property
     def all_monitors_passed(self):
         return self._step_monitors.successful
 
     @property
     def monitor_results(self):
         return self._step_monitors.all_items
 
     @property
     def monitors_passed_results(self):
-        return self._step_monitors.items_for_statuses(settings.MONITOR.STATUSES.SUCCESSFUL)
+        return self._step_monitors.items_for_statuses(
+            settings.MONITOR.STATUSES.SUCCESSFUL
+        )
 
     @property
     def monitors_failed_results(self):
         return self._step_monitors.items_for_statuses(settings.MONITOR.STATUSES.ERROR)
 
     @property
     def monitors_finished_action_results(self):
@@ -66,15 +71,17 @@
     def start(self):
         pass
 
     def finish(self):
         pass
 
     def next_step(self):
-        index = 0 if not self.step else list(self._steps.keys()).index(self.step.name)+1
+        index = (
+            0 if not self.step else list(self._steps.keys()).index(self.step.name) + 1
+        )
         self._current_step = list(self._steps.items())[index][1]
         self.step.start()
 
     def finish_step(self):
         self.step.finish()
 
     @monitors_step_required
```

### Comparing `spidermon-1.8.0/spidermon/results/items.py` & `spidermon-1.9.0/spidermon/results/items.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,28 +8,28 @@
         self.status = settings.UNDEFINED_STATUS
         self.error = None
         self.reason = None
         self.id = id(self)
 
 
 class MonitorResult(ItemResult):
-    name = 'monitor'
+    name = "monitor"
 
     def __init__(self, item):
         super(MonitorResult, self).__init__(item)
         self.status = settings.MONITOR.STATUSES.DEFAULT
 
     @property
     def monitor(self):
         return self.item
 
 
 class ActionResult(ItemResult):
-    name = 'action'
+    name = "action"
 
     def __init__(self, item):
         super(ActionResult, self).__init__(item)
         self.status = settings.ACTION.STATUSES.DEFAULT
 
     @property
     def action(self):
-        return self.item
+        return self.item
```

### Comparing `spidermon-1.8.0/LICENSE` & `spidermon-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spidermon-1.8.0/setup.py` & `spidermon-1.9.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 from setuptools import setup, find_packages
 
-test_requirements = [
-    'pytest>=2.7.0',
-    'tox'
-]
+test_requirements = ["pytest>=2.7.0", "tox"]
 
 setup(
-    name='spidermon',
-    version='1.8.0',
-    url='https://github.com/scrapinghub/spidermon',
-    author='Scrapinghub',
-    author_email='info@scrapinghub.com',
-    description=('Spidermon is a framework to build monitors for Scrapy '
-                 'spiders.'),
-    long_description=('Spidermon is a framework to build monitors for Scrapy '
-                      'spiders.'),
-    license='BSD',
+    name="spidermon",
+    version="1.9.0",
+    url="https://github.com/scrapinghub/spidermon",
+    author="Scrapinghub",
+    author_email="info@scrapinghub.com",
+    description=("Spidermon is a framework to build monitors for Scrapy " "spiders."),
+    long_description=(
+        "Spidermon is a framework to build monitors for Scrapy " "spiders."
+    ),
+    license="BSD",
     packages=find_packages(),
-    package_data={'spidermon': ['VERSION']},
+    package_data={"spidermon": ["VERSION"]},
     zip_safe=False,
     include_package_data=True,
-    install_requires=[
-        'six>=1.9.0',
-    ],
+    install_requires=["jsonschema", "python-slugify", "six>=1.9.0"],
     tests_require=test_requirements,
     extras_require={
         # Specific monitors and tools to support notifications and reports
-        'monitoring': [
-            'scrapy',
-            'Jinja2',
-            'slackclient',
-            'boto',
-            'premailer'
+        "monitoring": [
+            "scrapy",
+            "Jinja2",
+            "slackclient",
+            "boto",
+            "premailer",
+            "sentry-sdk",
         ],
         # Data validation
-        'validation': [
-            'jsonschema',
-            'schematics',
-            'python-slugify',
-            'strict-rfc3339'
-        ],
+        "validation": ["schematics", "strict-rfc3339"],
         # Tools to run the tests
-        'tests': test_requirements,
+        "tests": test_requirements,
+        "pep8": ["black"],
         # Tools to build and publish the documentation
-        'docs': [
-            'sphinx',
-            'sphinx-rtd-theme',
-            's3cmd'
-        ]
+        "docs": ["sphinx", "sphinx-rtd-theme", "s3cmd"],
     },
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Framework :: Scrapy',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: System :: Monitoring',
+        "Development Status :: 5 - Production/Stable",
+        "Framework :: Scrapy",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Topic :: Internet :: WWW/HTTP",
+        "Topic :: System :: Monitoring",
     ],
 )
```

