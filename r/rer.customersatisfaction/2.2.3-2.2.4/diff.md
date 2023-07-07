# Comparing `tmp/rer.customersatisfaction-2.2.3.tar.gz` & `tmp/rer.customersatisfaction-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.customersatisfaction-2.2.3.tar", last modified: Thu May 25 15:10:30 2023, max compression
+gzip compressed data, was "rer.customersatisfaction-2.2.4.tar", last modified: Fri Jul  7 13:54:17 2023, max compression
```

## Comparing `rer.customersatisfaction-2.2.3.tar` & `rer.customersatisfaction-2.2.4.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.953227 rer.customersatisfaction-2.2.3/
--rw-r--r--   0 roman      (502) staff       (20)      399 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/.eslintrc.json
--rw-r--r--   0 roman      (502) staff       (20)     1926 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/.gitlab-ci.yml
--rw-r--r--   0 roman      (502) staff       (20)      278 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/.prettierrc.json
--rw-r--r--   0 roman      (502) staff       (20)      131 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/.stylelintrc.json
--rw-r--r--   0 roman      (502) staff       (20)     1651 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/.travis.yml
--rw-r--r--   0 roman      (502) staff       (20)     1690 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)      142 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)      586 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      675 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      236 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)    10801 2023-05-25 15:10:30.953426 rer.customersatisfaction-2.2.3/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     5510 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/README.rst
--rw-r--r--   0 roman      (502) staff       (20)       27 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/constraints.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/constraints_plone52.txt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.924119 rer.customersatisfaction-2.2.3/docs/
--rw-r--r--   0 roman      (502) staff       (20)   297500 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/MA_Plone5_uso_CustomerSatisfaction.pdf
--rw-r--r--   0 roman      (502) staff       (20)     7939 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)   107242 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/customer-satisfaction-global.png
--rw-r--r--   0 roman      (502) staff       (20)    57908 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/customer-satisfaction_1-Recensione.jpg
--rw-r--r--   0 roman      (502) staff       (20)    25049 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/customer-satisfaction_2-Elenco-Recensioni.jpg
--rw-r--r--   0 roman      (502) staff       (20)    19731 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/customer-satisfaction_3-Dettaglio-Commenti.jpg
--rw-r--r--   0 roman      (502) staff       (20)       95 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)     3144 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/package.json
--rw-r--r--   0 roman      (502) staff       (20)      195 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/postcss.config.js
--rw-r--r--   0 roman      (502) staff       (20)     2463 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/publiccode.yml
--rw-r--r--   0 roman      (502) staff       (20)       42 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/requirements.txt
--rw-r--r--   0 roman      (502) staff       (20)      518 2023-05-25 15:10:30.953971 rer.customersatisfaction-2.2.3/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     2628 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.911360 rer.customersatisfaction-2.2.3/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.924380 rer.customersatisfaction-2.2.3/src/rer/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.928767 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/
--rw-r--r--   0 roman      (502) staff       (20)      141 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.931370 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1058 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     1988 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1198 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction.pt
--rw-r--r--   0 roman      (502) staff       (20)     1801 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction.py
--rw-r--r--   0 roman      (502) staff       (20)      599 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_global.pt
--rw-r--r--   0 roman      (502) staff       (20)      954 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_global.py
--rw-r--r--   0 roman      (502) staff       (20)     2142 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_viewlet.pt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.931594 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/overrides/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     4008 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/show_feedbacks.pt
--rw-r--r--   0 roman      (502) staff       (20)     3315 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/show_feedbacks.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.932034 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.913090 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.912169 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.933430 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.933659 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.933934 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.934173 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.934449 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/Context/
--rw-r--r--   0 roman      (502) staff       (20)      189 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/Context/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.934687 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/
--rw-r--r--   0 roman      (502) staff       (20)     1232 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/index.js
--rw-r--r--   0 roman      (502) staff       (20)     6427 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.935472 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/
--rw-r--r--   0 roman      (502) staff       (20)      205 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiConfing.js
--rw-r--r--   0 roman      (502) staff       (20)      911 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiFetch.js
--rw-r--r--   0 roman      (502) staff       (20)      796 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/commentsDataAggregator.js
--rw-r--r--   0 roman      (502) staff       (20)      276 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/index.js
--rw-r--r--   0 roman      (502) staff       (20)     1049 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/index.js
--rw-r--r--   0 roman      (502) staff       (20)      627 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.css
--rw-r--r--   0 roman      (502) staff       (20)      246 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.test.js
--rw-r--r--   0 roman      (502) staff       (20)      366 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.css
--rw-r--r--   0 roman      (502) staff       (20)      665 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.js
--rw-r--r--   0 roman      (502) staff       (20)      362 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/reportWebVitals.js
--rw-r--r--   0 roman      (502) staff       (20)      241 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/setupTests.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.935708 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.936180 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/
--rw-r--r--   0 roman      (502) staff       (20)     2982 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/ApiContext.js
--rw-r--r--   0 roman      (502) staff       (20)     1449 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/TranslationsContext.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.937123 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/
--rw-r--r--   0 roman      (502) staff       (20)      693 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.js
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.less
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.937400 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/
--rw-r--r--   0 roman      (502) staff       (20)     2162 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/ExportCSV.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.937876 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/
--rw-r--r--   0 roman      (502) staff       (20)     7214 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.jsx
--rw-r--r--   0 roman      (502) staff       (20)     1077 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.less
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.938351 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/
--rw-r--r--   0 roman      (502) staff       (20)     2305 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.jsx
--rw-r--r--   0 roman      (502) staff       (20)      456 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.less
--rw-r--r--   0 roman      (502) staff       (20)      279 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/index.js
--rw-r--r--   0 roman      (502) staff       (20)     1547 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/utils.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.938861 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/
--rw-r--r--   0 roman      (502) staff       (20)      957 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/apiFetch.js
--rw-r--r--   0 roman      (502) staff       (20)      921 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/vocabulary.js
--rw-r--r--   0 roman      (502) staff       (20)     2185 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/logo_rer.gif
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.914059 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.942091 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/
--rw-r--r--   0 roman      (502) staff       (20)     4612 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/2.js
--rw-r--r--   0 roman      (502) staff       (20)       91 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/2.js.map
--rw-r--r--   0 roman      (502) staff       (20)      693 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css
--rw-r--r--   0 roman      (502) staff       (20)      861 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css.map
--rw-r--r--   0 roman      (502) staff       (20)   471333 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js
--rw-r--r--   0 roman      (502) staff       (20)     1369 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js.map
--rw-r--r--   0 roman      (502) staff       (20)     1497 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.css
--rw-r--r--   0 roman      (502) staff       (20)     1802 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.css.map
--rw-r--r--   0 roman      (502) staff       (20)   320962 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.js
--rw-r--r--   0 roman      (502) staff       (20)     1082 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.js.map
--rw-r--r--   0 roman      (502) staff       (20)     2790 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.css
--rw-r--r--   0 roman      (502) staff       (20)     3534 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.js
--rw-r--r--   0 roman      (502) staff       (20)      669 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/viewlets.py
--rw-r--r--   0 roman      (502) staff       (20)     1588 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1409 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/contentrules.py
--rw-r--r--   0 roman      (502) staff       (20)      990 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/contentrules.zcml
--rw-r--r--   0 roman      (502) staff       (20)      431 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/events.py
--rw-r--r--   0 roman      (502) staff       (20)      495 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.943499 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/
--rw-r--r--   0 roman      (502) staff       (20)      611 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/README.rst
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.914397 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.943974 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)     1105 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/LC_MESSAGES/collective.honeypot.po
--rw-r--r--   0 roman      (502) staff       (20)     4803 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/LC_MESSAGES/rer.customersatisfaction.po
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.914605 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.944434 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)      879 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/LC_MESSAGES/collective.honeypot.po
--rw-r--r--   0 roman      (502) staff       (20)     4301 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/LC_MESSAGES/rer.customersatisfaction.po
--rw-r--r--   0 roman      (502) staff       (20)     1262 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/manual.pot
--rw-r--r--   0 roman      (502) staff       (20)     3574 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/rer.customersatisfaction.pot
--rw-r--r--   0 roman      (502) staff       (20)     1769 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      561 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/update.sh
--rw-r--r--   0 roman      (502) staff       (20)      834 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/permissions.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.915194 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.944890 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/2000/
--rw-r--r--   0 roman      (502) staff       (20)      356 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/2000/controlpanel.xml
--rw-r--r--   0 roman      (502) staff       (20)      226 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/2000/registry.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.946049 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      828 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      198 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)      240 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.946559 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)     1208 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)      142 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/registry/settings.xml
--rw-r--r--   0 roman      (502) staff       (20)      794 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.947474 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      291 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      134 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      352 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 roman      (502) staff       (20)      521 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/registry.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.947966 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      194 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.948664 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     5580 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/common.py
--rw-r--r--   0 roman      (502) staff       (20)      203 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.949523 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1766 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2667 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/crud.py
--rw-r--r--   0 roman      (502) staff       (20)     6004 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.950207 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/sites_list/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/sites_list/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      335 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/sites_list/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      730 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/sites_list/get.py
--rw-r--r--   0 roman      (502) staff       (20)      567 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/setuphandlers.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.951141 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      956 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/catalog.py
--rw-r--r--   0 roman      (502) staff       (20)      451 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     4382 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/store.py
--rw-r--r--   0 roman      (502) staff       (20)     2682 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.953011 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     4715 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_customer_satisfaction_add.py
--rw-r--r--   0 roman      (502) staff       (20)     7153 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_customer_satisfaction_get.py
--rw-r--r--   0 roman      (502) staff       (20)     3174 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_delete_content.py
--rw-r--r--   0 roman      (502) staff       (20)     1871 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_events.py
--rw-r--r--   0 roman      (502) staff       (20)     2471 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)     4782 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_show_feedbacks_view.py
--rw-r--r--   0 roman      (502) staff       (20)     3388 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_store.py
--rw-r--r--   0 roman      (502) staff       (20)      784 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/upgrades.py
--rw-r--r--   0 roman      (502) staff       (20)      762 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/upgrades.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-05-25 15:10:30.926235 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)    10801 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     8737 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      149 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)        4 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      249 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)        4 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/top_level.txt
--rw-r--r--   0 roman      (502) staff       (20)     2888 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/webpack.config.js
--rw-r--r--   0 roman      (502) staff       (20)   835088 2023-05-25 15:10:30.000000 rer.customersatisfaction-2.2.3/yarn.lock
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.052181 rer.customersatisfaction-2.2.4/
+-rw-r--r--   0 roman      (502) staff       (20)      399 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/.eslintrc.json
+-rw-r--r--   0 roman      (502) staff       (20)     1926 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/.gitlab-ci.yml
+-rw-r--r--   0 roman      (502) staff       (20)      278 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/.prettierrc.json
+-rw-r--r--   0 roman      (502) staff       (20)      131 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/.stylelintrc.json
+-rw-r--r--   0 roman      (502) staff       (20)     1651 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/.travis.yml
+-rw-r--r--   0 roman      (502) staff       (20)     1814 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/CHANGES.rst
+-rw-r--r--   0 roman      (502) staff       (20)      142 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/CONTRIBUTORS.rst
+-rw-r--r--   0 roman      (502) staff       (20)      586 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/DEVELOP.rst
+-rw-r--r--   0 roman      (502) staff       (20)    18092 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/LICENSE.GPL
+-rw-r--r--   0 roman      (502) staff       (20)      675 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/LICENSE.rst
+-rw-r--r--   0 roman      (502) staff       (20)      236 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/MANIFEST.in
+-rw-r--r--   0 roman      (502) staff       (20)    10981 2023-07-07 13:54:17.052380 rer.customersatisfaction-2.2.4/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)     5510 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/README.rst
+-rw-r--r--   0 roman      (502) staff       (20)       27 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/constraints.txt
+-rw-r--r--   0 roman      (502) staff       (20)      105 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/constraints_plone52.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.022226 rer.customersatisfaction-2.2.4/docs/
+-rw-r--r--   0 roman      (502) staff       (20)   297500 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/MA_Plone5_uso_CustomerSatisfaction.pdf
+-rw-r--r--   0 roman      (502) staff       (20)     7939 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/conf.py
+-rw-r--r--   0 roman      (502) staff       (20)   107242 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/customer-satisfaction-global.png
+-rw-r--r--   0 roman      (502) staff       (20)    57908 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/customer-satisfaction_1-Recensione.jpg
+-rw-r--r--   0 roman      (502) staff       (20)    25049 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/customer-satisfaction_2-Elenco-Recensioni.jpg
+-rw-r--r--   0 roman      (502) staff       (20)    19731 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/customer-satisfaction_3-Dettaglio-Commenti.jpg
+-rw-r--r--   0 roman      (502) staff       (20)       95 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/docs/index.rst
+-rw-r--r--   0 roman      (502) staff       (20)     3144 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/package.json
+-rw-r--r--   0 roman      (502) staff       (20)      195 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/postcss.config.js
+-rw-r--r--   0 roman      (502) staff       (20)     2463 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/publiccode.yml
+-rw-r--r--   0 roman      (502) staff       (20)       42 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/requirements.txt
+-rw-r--r--   0 roman      (502) staff       (20)      518 2023-07-07 13:54:17.052921 rer.customersatisfaction-2.2.4/setup.cfg
+-rw-r--r--   0 roman      (502) staff       (20)     2628 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/setup.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.008974 rer.customersatisfaction-2.2.4/src/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.022606 rer.customersatisfaction-2.2.4/src/rer/
+-rw-r--r--   0 roman      (502) staff       (20)       80 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.027095 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/
+-rw-r--r--   0 roman      (502) staff       (20)      141 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.029693 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1058 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     1988 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1198 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction.pt
+-rw-r--r--   0 roman      (502) staff       (20)     1801 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction.py
+-rw-r--r--   0 roman      (502) staff       (20)      599 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_global.pt
+-rw-r--r--   0 roman      (502) staff       (20)      954 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_global.py
+-rw-r--r--   0 roman      (502) staff       (20)     2142 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_viewlet.pt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.029963 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/overrides/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/overrides/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)     4008 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/show_feedbacks.pt
+-rw-r--r--   0 roman      (502) staff       (20)     3315 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/show_feedbacks.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.030374 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.011161 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.010183 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.031841 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.032070 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.032297 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.032525 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.032763 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/Context/
+-rw-r--r--   0 roman      (502) staff       (20)      189 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/Context/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.032993 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/
+-rw-r--r--   0 roman      (502) staff       (20)     1232 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/index.js
+-rw-r--r--   0 roman      (502) staff       (20)     6444 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.033683 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/
+-rw-r--r--   0 roman      (502) staff       (20)      205 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiConfing.js
+-rw-r--r--   0 roman      (502) staff       (20)      911 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiFetch.js
+-rw-r--r--   0 roman      (502) staff       (20)      796 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/commentsDataAggregator.js
+-rw-r--r--   0 roman      (502) staff       (20)      276 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/index.js
+-rw-r--r--   0 roman      (502) staff       (20)     1049 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/index.js
+-rw-r--r--   0 roman      (502) staff       (20)      627 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.css
+-rw-r--r--   0 roman      (502) staff       (20)      246 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.test.js
+-rw-r--r--   0 roman      (502) staff       (20)      366 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.css
+-rw-r--r--   0 roman      (502) staff       (20)      665 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.js
+-rw-r--r--   0 roman      (502) staff       (20)      362 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/reportWebVitals.js
+-rw-r--r--   0 roman      (502) staff       (20)      241 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/setupTests.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.033913 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.034362 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/
+-rw-r--r--   0 roman      (502) staff       (20)     2982 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/ApiContext.js
+-rw-r--r--   0 roman      (502) staff       (20)     1449 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/TranslationsContext.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.035217 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/
+-rw-r--r--   0 roman      (502) staff       (20)      693 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.js
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.less
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.035440 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/
+-rw-r--r--   0 roman      (502) staff       (20)     2162 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/ExportCSV.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.035910 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/
+-rw-r--r--   0 roman      (502) staff       (20)     7214 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.jsx
+-rw-r--r--   0 roman      (502) staff       (20)     1077 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.less
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.036364 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/
+-rw-r--r--   0 roman      (502) staff       (20)     2305 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.jsx
+-rw-r--r--   0 roman      (502) staff       (20)      456 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.less
+-rw-r--r--   0 roman      (502) staff       (20)      279 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/index.js
+-rw-r--r--   0 roman      (502) staff       (20)     1547 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/utils.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.036878 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/
+-rw-r--r--   0 roman      (502) staff       (20)      957 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/apiFetch.js
+-rw-r--r--   0 roman      (502) staff       (20)      921 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/vocabulary.js
+-rw-r--r--   0 roman      (502) staff       (20)     2185 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/logo_rer.gif
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.012127 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.040472 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/
+-rw-r--r--   0 roman      (502) staff       (20)     4612 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/2.js
+-rw-r--r--   0 roman      (502) staff       (20)       91 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/2.js.map
+-rw-r--r--   0 roman      (502) staff       (20)      693 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css
+-rw-r--r--   0 roman      (502) staff       (20)      861 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css.map
+-rw-r--r--   0 roman      (502) staff       (20)   471349 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js
+-rw-r--r--   0 roman      (502) staff       (20)     1369 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js.map
+-rw-r--r--   0 roman      (502) staff       (20)     1497 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.css
+-rw-r--r--   0 roman      (502) staff       (20)     1802 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.css.map
+-rw-r--r--   0 roman      (502) staff       (20)   320962 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.js
+-rw-r--r--   0 roman      (502) staff       (20)     1082 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.js.map
+-rw-r--r--   0 roman      (502) staff       (20)     2790 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.css
+-rw-r--r--   0 roman      (502) staff       (20)     3534 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.js
+-rw-r--r--   0 roman      (502) staff       (20)      669 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/viewlets.py
+-rw-r--r--   0 roman      (502) staff       (20)     1588 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1409 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/contentrules.py
+-rw-r--r--   0 roman      (502) staff       (20)      990 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/contentrules.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      431 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/events.py
+-rw-r--r--   0 roman      (502) staff       (20)      495 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.041917 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/
+-rw-r--r--   0 roman      (502) staff       (20)      611 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/README.rst
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.012457 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.042387 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)     1105 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/LC_MESSAGES/collective.honeypot.po
+-rw-r--r--   0 roman      (502) staff       (20)     4803 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/LC_MESSAGES/rer.customersatisfaction.po
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.012663 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.042854 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)      879 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/LC_MESSAGES/collective.honeypot.po
+-rw-r--r--   0 roman      (502) staff       (20)     4301 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/LC_MESSAGES/rer.customersatisfaction.po
+-rw-r--r--   0 roman      (502) staff       (20)     1262 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/manual.pot
+-rw-r--r--   0 roman      (502) staff       (20)     3574 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/rer.customersatisfaction.pot
+-rw-r--r--   0 roman      (502) staff       (20)     1769 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/update.py
+-rwxr-xr-x   0 roman      (502) staff       (20)      561 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/update.sh
+-rw-r--r--   0 roman      (502) staff       (20)      834 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/permissions.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.013240 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.043316 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/2000/
+-rw-r--r--   0 roman      (502) staff       (20)      356 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/2000/controlpanel.xml
+-rw-r--r--   0 roman      (502) staff       (20)      226 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/2000/registry.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.044518 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)      828 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/actions.xml
+-rw-r--r--   0 roman      (502) staff       (20)      198 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      105 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/catalog.xml
+-rw-r--r--   0 roman      (502) staff       (20)      240 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.045072 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/registry/
+-rw-r--r--   0 roman      (502) staff       (20)     1208 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/registry/resources.xml
+-rw-r--r--   0 roman      (502) staff       (20)      142 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/registry/settings.xml
+-rw-r--r--   0 roman      (502) staff       (20)      794 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/rolemap.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.046063 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      291 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/actions.xml
+-rw-r--r--   0 roman      (502) staff       (20)      134 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      352 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 roman      (502) staff       (20)      521 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/registry.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.046462 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      194 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.047170 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     5580 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/common.py
+-rw-r--r--   0 roman      (502) staff       (20)      203 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.048207 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1766 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     2667 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/crud.py
+-rw-r--r--   0 roman      (502) staff       (20)     6004 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.048879 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/sites_list/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/sites_list/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      335 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/sites_list/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      730 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/sites_list/get.py
+-rw-r--r--   0 roman      (502) staff       (20)      567 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/setuphandlers.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.050088 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      956 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/catalog.py
+-rw-r--r--   0 roman      (502) staff       (20)      451 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     4382 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/store.py
+-rw-r--r--   0 roman      (502) staff       (20)     2682 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/testing.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.051985 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     4715 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_customer_satisfaction_add.py
+-rw-r--r--   0 roman      (502) staff       (20)     7153 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_customer_satisfaction_get.py
+-rw-r--r--   0 roman      (502) staff       (20)     3174 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_delete_content.py
+-rw-r--r--   0 roman      (502) staff       (20)     1871 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_events.py
+-rw-r--r--   0 roman      (502) staff       (20)     2471 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_setup.py
+-rw-r--r--   0 roman      (502) staff       (20)     4782 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_show_feedbacks_view.py
+-rw-r--r--   0 roman      (502) staff       (20)     3388 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_store.py
+-rw-r--r--   0 roman      (502) staff       (20)      784 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/upgrades.py
+-rw-r--r--   0 roman      (502) staff       (20)      762 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/upgrades.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-07-07 13:54:17.024632 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/
+-rw-r--r--   0 roman      (502) staff       (20)    10981 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)     8737 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (502) staff       (20)      149 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/entry_points.txt
+-rw-r--r--   0 roman      (502) staff       (20)        4 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/namespace_packages.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/not-zip-safe
+-rw-r--r--   0 roman      (502) staff       (20)      249 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/requires.txt
+-rw-r--r--   0 roman      (502) staff       (20)        4 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/top_level.txt
+-rw-r--r--   0 roman      (502) staff       (20)     2888 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/webpack.config.js
+-rw-r--r--   0 roman      (502) staff       (20)   835088 2023-07-07 13:54:16.000000 rer.customersatisfaction-2.2.4/yarn.lock
```

### Comparing `rer.customersatisfaction-2.2.3/.gitlab-ci.yml` & `rer.customersatisfaction-2.2.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/.travis.yml` & `rer.customersatisfaction-2.2.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/CHANGES.rst` & `rer.customersatisfaction-2.2.4/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+2.2.4 (2023-07-07)
+------------------
+
+- add escape chars for csv in the customer-satisfaction-gloabal view.
+  [folix-01]
+
+
 2.2.3 (2023-05-25)
 ------------------
 - Add export to customer-satisfaction-global view
   [folix-01]
 - Add Spanish translations.
   [macagua]
 - Fix english translations.
```

### Comparing `rer.customersatisfaction-2.2.3/DEVELOP.rst` & `rer.customersatisfaction-2.2.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/LICENSE.GPL` & `rer.customersatisfaction-2.2.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/LICENSE.rst` & `rer.customersatisfaction-2.2.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/PKG-INFO` & `rer.customersatisfaction-2.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.customersatisfaction
-Version: 2.2.3
+Version: 2.2.4
 Summary: Customer satisfaction
 Home-page: https://github.com/collective/rer.customersatisfaction
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.customersatisfaction
 Project-URL: Source, https://github.com/collective/rer.customersatisfaction
@@ -213,14 +213,21 @@
         - Leonardo J. Caballero G., @macagua
         
         
         Changelog
         =========
         
         
+        2.2.4 (2023-07-07)
+        ------------------
+        
+        - add escape chars for csv in the customer-satisfaction-gloabal view.
+          [folix-01]
+        
+        
         2.2.3 (2023-05-25)
         ------------------
         - Add export to customer-satisfaction-global view
           [folix-01]
         - Add Spanish translations.
           [macagua]
         - Fix english translations.
```

### Comparing `rer.customersatisfaction-2.2.3/README.rst` & `rer.customersatisfaction-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/MA_Plone5_uso_CustomerSatisfaction.pdf` & `rer.customersatisfaction-2.2.4/docs/MA_Plone5_uso_CustomerSatisfaction.pdf`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/conf.py` & `rer.customersatisfaction-2.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/customer-satisfaction-global.png` & `rer.customersatisfaction-2.2.4/docs/customer-satisfaction-global.png`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/customer-satisfaction_1-Recensione.jpg` & `rer.customersatisfaction-2.2.4/docs/customer-satisfaction_1-Recensione.jpg`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/customer-satisfaction_2-Elenco-Recensioni.jpg` & `rer.customersatisfaction-2.2.4/docs/customer-satisfaction_2-Elenco-Recensioni.jpg`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/docs/customer-satisfaction_3-Dettaglio-Commenti.jpg` & `rer.customersatisfaction-2.2.4/docs/customer-satisfaction_3-Dettaglio-Commenti.jpg`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/package.json` & `rer.customersatisfaction-2.2.4/package.json`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/publiccode.yml` & `rer.customersatisfaction-2.2.4/publiccode.yml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/setup.cfg` & `rer.customersatisfaction-2.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/setup.py` & `rer.customersatisfaction-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.customersatisfaction",
-    version="2.2.3",
+    version="2.2.4",
     description="Customer satisfaction",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/adapters.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/adapters.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/configure.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction.pt` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction.pt`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_global.pt` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_global.pt`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_global.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_global.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/customer_satisfaction_viewlet.pt` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/customer_satisfaction_viewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/show_feedbacks.pt` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/show_feedbacks.pt`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/show_feedbacks.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/show_feedbacks.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/index.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/FilterForm/index.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/index.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -171,15 +171,15 @@
     result = result.slice(0, -1) + lineDelimiter;
 
     array.forEach(item => {
         let ctr = 0;
         keys.forEach(key => {
             if (ctr > 0) result += columnDelimiter;
 
-            result += String(key.csv_value(item)).replace(',', "");
+            result += String(key.csv_value(item)).replace(',', "").replace("#", "");
             // eslint-disable-next-line no-plusplus
             ctr++;
         });
         result += lineDelimiter;
     });
 
     return result;
```

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiFetch.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/apiFetch.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/commentsDataAggregator.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/Comments/CommentsTable/utils/commentsDataAggregator.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/index.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App/index.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.css` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/App.css`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/customer_satisfaction_global/src/index.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/ApiContext.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/ApiContext.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/TranslationsContext.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/TranslationsContext.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/App.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/ExportCSV.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CSV/ExportCSV.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.jsx` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.jsx`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.less` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/CustomerSatisfactionList/index.less`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.jsx` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/Menu/Menu.jsx`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/utils.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/history/utils.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/apiFetch.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/apiFetch.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/vocabulary.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/javascripts/utils/vocabulary.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/apps/history/logo_rer.gif` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/apps/history/logo_rer.gif`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/2.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/2.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css.map` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.css.map`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21816,15 +21816,15 @@
                 n = function(e) {
                     var t, n = du;
                     return t = "", n.forEach((function(e) {
                         t += e.name + ","
                     })), t = t.slice(0, -1) + "\n", e.forEach((function(e) {
                         var r = 0;
                         n.forEach((function(n) {
-                            r > 0 && (t += ","), t += String(n.csv_value(e)).replace(",", ""), r++
+                            r > 0 && (t += ","), t += String(n.csv_value(e)).replace(",", "").replace("#", ""), r++
                         })), t += "\n"
                     })), t
                 }(e);
             if (null != n) {
                 n.match(/^data:text\/csv/i) || (n = "data:text/csv;charset=utf-8,".concat(n)), t.setAttribute("href", encodeURI(n)), t.setAttribute("download", "Customer Satisfaction.csv"), t.click()
             }
         }
```

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js.map` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/customer_satisfaction_global.js.map`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.css` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.css`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.css.map` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.css.map`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/dist/prod/history.js.map` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/dist/prod/history.js.map`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.css` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.css`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.js` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/static/rer-customersatisfaction.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/browser/viewlets.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/configure.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/contentrules.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/contentrules.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/contentrules.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/contentrules.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/README.rst` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/LC_MESSAGES/collective.honeypot.po` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/LC_MESSAGES/collective.honeypot.po`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/es/LC_MESSAGES/rer.customersatisfaction.po` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/es/LC_MESSAGES/rer.customersatisfaction.po`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/LC_MESSAGES/collective.honeypot.po` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/LC_MESSAGES/collective.honeypot.po`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/it/LC_MESSAGES/rer.customersatisfaction.po` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/it/LC_MESSAGES/rer.customersatisfaction.po`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/manual.pot` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/rer.customersatisfaction.pot` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/rer.customersatisfaction.pot`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/update.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/locales/update.sh` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/locales/update.sh`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/permissions.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/permissions.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/actions.xml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/registry/resources.xml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/default/rolemap.xml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/profiles/uninstall/registry.xml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/common.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/common.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/configure.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/crud.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/crud.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/customer_satisfaction/get.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/customer_satisfaction/get.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/restapi/services/sites_list/get.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/restapi/services/sites_list/get.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/setuphandlers.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/catalog.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/catalog.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/storage/store.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/storage/store.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/testing.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/testing.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_customer_satisfaction_add.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_customer_satisfaction_add.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_customer_satisfaction_get.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_customer_satisfaction_get.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_delete_content.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_delete_content.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_events.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_setup.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_show_feedbacks_view.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_show_feedbacks_view.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/tests/test_store.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/upgrades.py` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/upgrades.py`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer/customersatisfaction/upgrades.zcml` & `rer.customersatisfaction-2.2.4/src/rer/customersatisfaction/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/PKG-INFO` & `rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.customersatisfaction
-Version: 2.2.3
+Version: 2.2.4
 Summary: Customer satisfaction
 Home-page: https://github.com/collective/rer.customersatisfaction
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.customersatisfaction
 Project-URL: Source, https://github.com/collective/rer.customersatisfaction
@@ -213,14 +213,21 @@
         - Leonardo J. Caballero G., @macagua
         
         
         Changelog
         =========
         
         
+        2.2.4 (2023-07-07)
+        ------------------
+        
+        - add escape chars for csv in the customer-satisfaction-gloabal view.
+          [folix-01]
+        
+        
         2.2.3 (2023-05-25)
         ------------------
         - Add export to customer-satisfaction-global view
           [folix-01]
         - Add Spanish translations.
           [macagua]
         - Fix english translations.
```

### Comparing `rer.customersatisfaction-2.2.3/src/rer.customersatisfaction.egg-info/SOURCES.txt` & `rer.customersatisfaction-2.2.4/src/rer.customersatisfaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/webpack.config.js` & `rer.customersatisfaction-2.2.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `rer.customersatisfaction-2.2.3/yarn.lock` & `rer.customersatisfaction-2.2.4/yarn.lock`

 * *Files identical despite different names*

