# Comparing `tmp/decore_Base-0.0.24.tar.gz` & `tmp/decore_Base-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.24.tar", last modified: Thu Jun 22 12:19:02 2023, max compression
+gzip compressed data, was "decore_Base-0.0.25.tar", last modified: Fri Jul  7 07:54:24 2023, max compression
```

## Comparing `decore_Base-0.0.24.tar` & `decore_Base-0.0.25.tar`

### file list

```diff
@@ -1,237 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 12:18:54.000000 decore_Base-0.0.24/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 12:18:54.000000 decore_Base-0.0.24/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-22 12:18:54.000000 decore_Base-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 12:19:02.731172 decore_Base-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-06-22 12:18:54.000000 decore_Base-0.0.24/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-06-22 12:18:54.000000 decore_Base-0.0.24/README_DE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 12:19:02.000000 decore_Base-0.0.24/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/decore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.707172 decore_Base-0.0.24/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.711172 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    33933 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/586.6cfbf2b5.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/app.aff5db90.js
--rw-r--r--   0 runner    (1001) docker     (123)   376913 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/static/js/vendor.6fe961ae.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/bases/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/person_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.715172 decore_Base-0.0.24/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)    57344 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/sample/state/querybase.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.719172 decore_Base-0.0.24/decore_base/uniform/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/decore_base/uniform/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-22 12:18:54.000000 decore_Base-0.0.24/decore_base/uniform/reform_server_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/decore.rst.out
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/language.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/model.rst.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)    79165 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    46074 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.723172 decore_Base-0.0.24/docs/page/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.703173 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.727172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    42879 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/page/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:19:02.731172 decore_Base-0.0.24/docs/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-22 12:18:54.000000 decore_Base-0.0.24/docs/state/querybase.db
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 12:18:54.000000 decore_Base-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 12:18:54.000000 decore_Base-0.0.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-22 12:19:02.731172 decore_Base-0.0.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.547332 decore_Base-0.0.25/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.531332 decore_Base-0.0.25/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-07 07:54:14.000000 decore_Base-0.0.25/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.531332 decore_Base-0.0.25/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 07:54:14.000000 decore_Base-0.0.25/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-07 07:54:14.000000 decore_Base-0.0.25/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-07 07:54:14.000000 decore_Base-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-07-07 07:54:24.547332 decore_Base-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-07-07 07:54:14.000000 decore_Base-0.0.25/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-07 07:54:14.000000 decore_Base-0.0.25/README_DE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.531332 decore_Base-0.0.25/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-07-07 07:54:24.000000 decore_Base-0.0.25/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-07 07:54:24.000000 decore_Base-0.0.25/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:54:24.000000 decore_Base-0.0.25/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 07:54:24.000000 decore_Base-0.0.25/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 07:54:24.000000 decore_Base-0.0.25/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.531332 decore_Base-0.0.25/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/classes/globals_keybase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/decore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.527332 decore_Base-0.0.25/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.535332 decore_Base-0.0.25/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.539332 decore_Base-0.0.25/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.539332 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.543332 decore_Base-0.0.25/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.543332 decore_Base-0.0.25/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    33933 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/js/586.6cfbf2b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/js/app.aff5db90.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376913 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/static/js/vendor.6fe961ae.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.543332 decore_Base-0.0.25/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.543332 decore_Base-0.0.25/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:54:24.547332 decore_Base-0.0.25/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 07:54:14.000000 decore_Base-0.0.25/decore_base/uniform/reform_server_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 07:54:14.000000 decore_Base-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-07 07:54:24.547332 decore_Base-0.0.25/setup.cfg
```

### Comparing `decore_Base-0.0.24/.github/FUNDING.yml` & `decore_Base-0.0.25/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/.gitignore` & `decore_Base-0.0.25/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/LICENSE` & `decore_Base-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/PKG-INFO` & `decore_Base-0.0.25/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.24
+Version: 0.0.25
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 License-File: LICENSE
 
+decore Base | UI fastly
+=======================
 Introduction
 ------------
 decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms, do scientific work or perform teaching and learning functions.
 
+Notes
+-----
 **decore Base is currently a work in progress, only locally deployable, only available for Windows and not yet production ready**.
 
 The recommended IDE is Visual Studio Code and all my comments and documentation here will also refer to vscode only.
 
 `Insights into the current status of the Decore project. <https://github.com/users/KemoPanzah/projects/1/views/1>`_
 
 .. image:: https://ko-fi.com/img/githubbutton_sm.svg
    :target: https://ko-fi.com/P5P2JCC5B
    :alt: Buy me a coffee
 
+This documentation was translated from German into English with Deepl.
+
+Features and Integrations
+-------------------------
+- Ready-made SPA (Single Page Application) with Vue.js using Quasar Framework (https://github.com/quasarframework/quasar)
+- Predefined Webapi for meta and actions with Flask (https://github.com/pallets/flask)
+- Integrated ORM for data management and database interfaces (SQLite) powered by the great Peewee (https://github.com/coleifer/peewee)
+- Data validation using Cerberus (https://github.com/pyeve/cerberus)
+- Password management using pykeepass (https://github.com/libkeepass/pykeepass)
+
+Please support these great projects!
+
 Contribution
 ------------
 The biggest help I can get right now is if you take a look at the project and tell me what you think. I am grateful for any criticism.
 
 My current sample project is included directly in the Python package. To install the example application, please read the documentation in **Example**. Please read **Installation**, **Use** and **Preparation** first.
 
 Anything found in the documentation in terms of features, bugs or ambiguities, please let me know.
@@ -262,15 +278,7 @@
 To build your application, run ``python app.py --build`` in your project root directory. Use the terminal in vscode.
 
 Sample application
 ------------------
 To better understand how decore base works, it is best to look at the sample application. The application represents my continuous development of decore base.
 
 https://github.com/KemoPanzah/decore_Base/tree/master/decore_base/sample
-
-To synchronize the sample application with a subfolder of the project root directory, run ``python app.py --sample`` in your project root directory. Use the terminal in vscode.
-
-To run the sample application after synchronization, use your debugger with the ``[smp] decore base sample`` profile in vscode.
-
-Notes
------
-This documentation was translated from German into English with Deepl.
```

### Comparing `decore_Base-0.0.24/README.rst` & `decore_Base-0.0.25/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+decore Base | UI fastly
+=======================
 Introduction
 ------------
 decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms, do scientific work or perform teaching and learning functions.
 
+Notes
+-----
 **decore Base is currently a work in progress, only locally deployable, only available for Windows and not yet production ready**.
 
 The recommended IDE is Visual Studio Code and all my comments and documentation here will also refer to vscode only.
 
 `Insights into the current status of the Decore project. <https://github.com/users/KemoPanzah/projects/1/views/1>`_
 
 .. image:: https://ko-fi.com/img/githubbutton_sm.svg
    :target: https://ko-fi.com/P5P2JCC5B
    :alt: Buy me a coffee
 
+This documentation was translated from German into English with Deepl.
+
+Features and Integrations
+-------------------------
+- Ready-made SPA (Single Page Application) with Vue.js using Quasar Framework (https://github.com/quasarframework/quasar)
+- Predefined Webapi for meta and actions with Flask (https://github.com/pallets/flask)
+- Integrated ORM for data management and database interfaces (SQLite) powered by the great Peewee (https://github.com/coleifer/peewee)
+- Data validation using Cerberus (https://github.com/pyeve/cerberus)
+- Password management using pykeepass (https://github.com/libkeepass/pykeepass)
+
+Please support these great projects!
+
 Contribution
 ------------
 The biggest help I can get right now is if you take a look at the project and tell me what you think. I am grateful for any criticism.
 
 My current sample project is included directly in the Python package. To install the example application, please read the documentation in **Example**. Please read **Installation**, **Use** and **Preparation** first.
 
 Anything found in the documentation in terms of features, bugs or ambiguities, please let me know.
@@ -247,16 +263,8 @@
 ~~~~~
 To build your application, run ``python app.py --build`` in your project root directory. Use the terminal in vscode.
 
 Sample application
 ------------------
 To better understand how decore base works, it is best to look at the sample application. The application represents my continuous development of decore base.
 
-https://github.com/KemoPanzah/decore_Base/tree/master/decore_base/sample
-
-To synchronize the sample application with a subfolder of the project root directory, run ``python app.py --sample`` in your project root directory. Use the terminal in vscode.
-
-To run the sample application after synchronization, use your debugger with the ``[smp] decore base sample`` profile in vscode.
-
-Notes
------
-This documentation was translated from German into English with Deepl.
+https://github.com/KemoPanzah/decore_Base/tree/master/decore_base/sample
```

### Comparing `decore_Base-0.0.24/README_DE.rst` & `decore_Base-0.0.25/README_DE.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+decore Base | UI fastly
+=======================
 Introduction
 ------------
 decore Base ist ein sofort einsatzbereites "Python to Vue.js" Datenanwendungs-Dashboard, das Ihnen hilft, in wenigen einfachen Schritten von der Idee zur Ansicht zu gelangen. Es richtet sich an diejenigen, die sich auf die Ergebnisse ihrer Algorithmen konzentrieren, wissenschaftlich arbeiten oder Lehr- und Lernfunktionen ausführen wollen.
 
+Notes
+-----
 **decore Base ist derzeit noch in Arbeit, nur lokal einsetzbar, nur für Windows verfügbar und noch nicht produktionsreif**.
 
 Die empfohlene IDE ist Visual Studio Code und alle meine Kommentare und Dokumentationen hier werden sich auch nur auf vscode beziehen.
 
 `Einblicke in den aktuellen Stand des Decore-Projekts <https://github.com/users/KemoPanzah/projects/1/views/1>`_
 
 .. image:: https://ko-fi.com/img/githubbutton_sm.svg
    :target: https://ko-fi.com/P5P2JCC5B
    :alt: Buy me a coffee
 
+Diese Dokumentation wurde mit Deepl vom Deutschen ins Englische übersetzt.
+
+Features and Integrations
+-------------------------
+- Fertige SPA (Single Page Application) mit Vue.js mittels Quasar Framework (https://github.com/quasarframework/quasar)
+- Vordefinierte Webapi für Meta und Aktionen mit Flask (https://github.com/pallets/flask)
+- Integriertes ORM für die Datenverwaltung und Datenbankschnittstellen (SQLite) powered by the great Peewee (https://github.com/coleifer/peewee)
+- Datenvalidierung mittels Cerberus (https://github.com/pyeve/cerberus)
+- Passwortmanagment durch pykeepass (https://github.com/libkeepass/pykeepass)
+
+Bitte unterstützt diese großartigen Projekte!
+
 Contribution
 ------------
 Die größte Hilfe, die ich im Moment bekommen kann, ist, wenn Sie einen Blick auf das Projekt werfen und mir sagen, was Sie davon halten. Ich bin für jede Kritik dankbar.
 
 Mein aktuelles Beispielprojekt ist direkt im Python-Paket enthalten. Um die Beispielanwendung zu installieren, lesen Sie bitte die Dokumentation unter **Beispiel**. Bitte lesen Sie zuerst **Installation**, **Benutzung** und **Vorbereitung**.
 
 Alles, was in der Dokumentation an Funktionen, Fehlern oder Unklarheiten gefunden wird, bitte ich Sie, mir mitzuteilen.
@@ -247,16 +263,8 @@
 ~~~~~
 Um Ihre Anwendung zu erstellen, führen Sie ``python app.py --build`` in Ihrem Projekt-Stammverzeichnis aus. Verwenden Sie das Terminal in vscode.
 
 Sample application
 ------------------
 Um besser zu verstehen, wie decore base funktioniert, ist es am besten, sich die Beispielanwendung anzusehen. Die Anwendung repräsentiert meine kontinuierliche Entwicklung von decore base.
 
-https://github.com/KemoPanzah/decore_Base/tree/master/decore_base/sample
-
-Um die Beispielanwendung mit einem Unterordner des Projektstammverzeichnisses zu synchronisieren, führen Sie ``python app.py --sample`` in Ihrem Projektstammverzeichnis aus. Verwenden Sie das Terminal in vscode.
-
-Um die Beispielanwendung nach der Synchronisation auszuführen, verwenden Sie Ihren Debugger mit dem Profil ``[smp] decore base sample`` in vscode.
-
-Notes
------
-Diese Dokumentation wurde mit Deepl vom Deutschen ins Englische übersetzt.
+https://github.com/KemoPanzah/decore_Sample
```

### Comparing `decore_Base-0.0.24/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.25/decore_Base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.24
+Version: 0.0.25
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 License-File: LICENSE
 
+decore Base | UI fastly
+=======================
 Introduction
 ------------
 decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms, do scientific work or perform teaching and learning functions.
 
+Notes
+-----
 **decore Base is currently a work in progress, only locally deployable, only available for Windows and not yet production ready**.
 
 The recommended IDE is Visual Studio Code and all my comments and documentation here will also refer to vscode only.
 
 `Insights into the current status of the Decore project. <https://github.com/users/KemoPanzah/projects/1/views/1>`_
 
 .. image:: https://ko-fi.com/img/githubbutton_sm.svg
    :target: https://ko-fi.com/P5P2JCC5B
    :alt: Buy me a coffee
 
+This documentation was translated from German into English with Deepl.
+
+Features and Integrations
+-------------------------
+- Ready-made SPA (Single Page Application) with Vue.js using Quasar Framework (https://github.com/quasarframework/quasar)
+- Predefined Webapi for meta and actions with Flask (https://github.com/pallets/flask)
+- Integrated ORM for data management and database interfaces (SQLite) powered by the great Peewee (https://github.com/coleifer/peewee)
+- Data validation using Cerberus (https://github.com/pyeve/cerberus)
+- Password management using pykeepass (https://github.com/libkeepass/pykeepass)
+
+Please support these great projects!
+
 Contribution
 ------------
 The biggest help I can get right now is if you take a look at the project and tell me what you think. I am grateful for any criticism.
 
 My current sample project is included directly in the Python package. To install the example application, please read the documentation in **Example**. Please read **Installation**, **Use** and **Preparation** first.
 
 Anything found in the documentation in terms of features, bugs or ambiguities, please let me know.
@@ -262,15 +278,7 @@
 To build your application, run ``python app.py --build`` in your project root directory. Use the terminal in vscode.
 
 Sample application
 ------------------
 To better understand how decore base works, it is best to look at the sample application. The application represents my continuous development of decore base.
 
 https://github.com/KemoPanzah/decore_Base/tree/master/decore_base/sample
-
-To synchronize the sample application with a subfolder of the project root directory, run ``python app.py --sample`` in your project root directory. Use the terminal in vscode.
-
-To run the sample application after synchronization, use your debugger with the ``[smp] decore base sample`` profile in vscode.
-
-Notes
------
-This documentation was translated from German into English with Deepl.
```

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_base.py` & `decore_Base-0.0.25/decore_base/classes/decore_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_fields.py` & `decore_Base-0.0.25/decore_base/classes/decore_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,92 +67,86 @@
             instance.__data__[self.name] = value
             instance._dirty.add(self.name)
         else:
             instance.__data__[self.name] = UUID(value) if value is not None else None
             instance._dirty.add(self.name)
 
 class CustomField(Field):
-
     @property
     def instance(self):
         calling_frames = inspect.getouterframes(inspect.currentframe())
         for frame in calling_frames:
             instance = frame[0].f_locals.get('self')
             if isinstance(instance, self.model):
                 return instance
         return None
 
 class BackRefMetaField(MetaField):
-    def __init__(self,verbose_name=None, help_text=None, filter_fields=None):
-        super().__init__(False, False, False, None, None, False, None, None, None, False, None, help_text, verbose_name, None, None, False)
+    ''' 
+    .. Warning:: The BackRefMetaField's name must match the name of the specified backref in the ForeignKey or ManyToMany field in the reference model.
+
+    The BackRefMetaField is used by the user to represent relationships in the **decore Front** application. For example, it can be assigned to the filter or to a form. It is a MetaField and does not get a column in the database.
+
+    :param null: If True, the field is allowed to be null. Defaults to False.
+    :param default: The default value for the field.
+    :param help_text: Additional text to be displayed in **decore Front**.
+    :param verbose_name: A human-readable name for the field.
+    :param filter_fields: A List of type string. Only the speciefied fields will be displayed in the filter. If None, all fields will be displayed.
+        
+    .. code-block:: python
+
+        class Account(Conform_model):
+            users = ManyToManyField(User, backref='accounts', null=True, verbose_name='Users')
+
+    .. code-block:: python
+
+        class User(Conform_model):
+            accounts = BackRefMetaField(null=True, verbose_name='Accounts')
+        
+    '''
+    def __init__(self, null=False, default=None, help_text=None, verbose_name=None, filter_fields=None):
         self.filter_fields = filter_fields
-    
+        MetaField.__init__(self, null=null, default=default, help_text=help_text, verbose_name=verbose_name)
+        
     def bind(self, model, name, set_attribute):
-        super().bind(model, name, set_attribute)
+        super(BackRefMetaField, self).bind(model, name, set_attribute)
         setattr(model,'br_'+name, getattr(model, name)) 
         delattr(model, name)
 
 class BooleanField(BooleanField):
     pass
 
 class CharField(CharField):
     pass
 
+class PasswordFieldAccessor(object):
+    def __init__(self, model, field, name):
+        self.model = model
+        self.field = field
+        self.name = name
+
+    def __get__(self, instance, instance_type=None):
+        if instance is not None:
+            if instance.__data__.get(self.name) is not None:
+                return globals.keybase.get_entry(self.model.__name__, instance.__data__.get(self.name))
+            else:
+                return None
+        return self.field
+
+    def __set__(self, instance, value):
+        if value is not None:
+            instance.__data__[self.name] = globals.keybase.append(self.model.__name__, instance.id, self.name, str(value))
+        else:
+            instance.__data__[self.name] = None
+        instance._dirty.add(self.name)
+
 class PasswordField(CustomField):
+    accessor_class = PasswordFieldAccessor
     field_type = 'VARCHAR'
 
-    @property
-    def kdb_group(self):
-        t_group = globals.kdb.find_groups_by_name(self.model.__name__, group=globals.kdb.root_group, first=True)
-        if not t_group:
-            t_group = globals.kdb.add_group(globals.kdb.root_group, self.model.__name__)
-            globals.kdb.save()
-        return t_group
-
-    def db_value(self, value):
-        t_entry = None
-        
-        # MEMO - Suche nach einem Eintrag der dem Identifiziern entspricht 
-        i_entry: Entry
-        for i_entry in self.kdb_group.entries:
-            if i_entry.title == self.name and i_entry.username == self.instance.id:
-                t_entry = i_entry
-        
-        # MEMO - Wenn kein Eintrag vorhanden ist, lege einen neuen an und füge diesen der Gruppe hinzu
-        if not t_entry:
-            t_entry = Entry(title=self.name, username=self.instance.id, password=value, kp=globals.kdb)
-            self.kdb_group.append(t_entry)
-            try:
-                globals.kdb.save()
-            except:
-                raise Exception('Could not save to keybase')
-            
-        # MEMO - Wenn der neue Wert nicht mit dem Password im Entry übereinstimmt und auch nicht mit der UUID dann ändere und speichere
-        if not value == t_entry.password and not value == str(t_entry.uuid):
-            t_entry.password = value
-            try:
-                globals.kdb.save()
-            except:
-                raise Exception('Could not save to keybase')
-        
-        # MEMO - schreibe die UUID des Entries in das __data__ Dict um das Kennwort zu verschleiern
-        return str(t_entry.uuid)
-
-    def python_value(self, value):
-        t_entry = None
-        
-        # MEMO - Suche nach einem Eintrag der dem Identifiziern entspricht und gebe das Password des Eintrages zurück
-        i_entry: Entry
-        for i_entry in self.kdb_group.entries:
-            if i_entry.uuid.hex == value:
-                return i_entry.password
-        
-        # MEMO - Wenn kein Eintrag vorhanden ist, gebe None als Passwort aus
-        if not t_entry:
-            return None
 
 class ForeignKeyField(ForeignKeyField):
     pass
 
 class IntegerField(IntegerField):
     pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_list.py` & `decore_Base-0.0.25/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_model.py` & `decore_Base-0.0.25/decore_base/classes/decore_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import logging
 import operator
 from functools import reduce
 from uuid import uuid1
 
-#
 from cerberus import Validator
 from peewee import DQ, FieldAccessor, Model, SqliteDatabase
 from playhouse.migrate import SqliteMigrator, migrate
 from playhouse.reflection import Introspector
 from playhouse.shortcuts import model_to_dict
 
 #
@@ -146,15 +145,15 @@
             else:
                 if type(value) is list:
                     t_exp = None
                     for item in value:
                         t_exp |= DQ(**{key: item})
                     r_item_s = r_item_s.filter(t_exp)
 
-                elif type(value) is str:
+                elif type(value) is str or int:
                     r_item_s = r_item_s.filter(**{key: value})
                 else:
                     raise Exception('Type error in query value')
         
         for key, value in t_mm_query.items():   
             t_rel_model = cls._meta.manytomany[key].rel_model
             t_through_model = cls._meta.manytomany[key]._through_model
@@ -245,36 +244,38 @@
 
     def save(self):
         #TODO - auf try except umstellen und raisen in validate.
         if self.validate():
             t_item = self.__class__.get_or_none(self.__class__.id == self.id)
             if not t_item:
                 try:
+                    globals.keybase.commit(self.id)
                     super(Decore_model,self).save(force_insert=True)
                 except Exception as error:
                     logging.error('%s > %s > %s' % ('save_item', 'Insert error', error))
                     return False
                 else:
                     return True
             elif t_item:
-                # t_data = {k: v for k, v in t_item.__data__.items() if v is not None}
-                if not self.__data__ == t_item.__data__:
+                t_data = {k: v for k, v in t_item.__data__.items() if v is not None}
+                if not self.__data__ == t_data:
                     try:
-                        super(Decore_model,self).save()
+                        globals.keybase.commit(self.id)
+                        super(Decore_model, self).save()
                     except Exception as error:
                         logging.error('%s > %s > %s' % ('save_item', 'Update error', error))
                         return False
                     else:
                         return True
                 else:
                     return True
         else:
             logging.error('%s > %s' % ('save_item', 'Validation error'))
             return False
 
     #TODO - return values prüfen; werden die eigentlich benötigt? > delete_instance
     def delete_instance(self):
-        if self(Decore_model, self).delete_instance():
+        if super(Decore_model, self).delete_instance():
             return True
         else:
             logging.error('%s > %s' % ('remove_item', 'Remove error'))
             return False
```

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_pool.py` & `decore_Base-0.0.25/decore_base/classes/decore_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             for key, value in p_value.items():
                 t_return[key] = self.serialize(value)
         elif Decore_object in inspect.getmro(p_value.__class__):
             setattr(p_value,'class', p_value.__class__.__name__)
             for key, value in p_value.__dict__.items():
                 t_return[key] = self.serialize(value)
         elif BackrefAccessor in inspect.getmro(p_value.__class__):
-            p_value = getattr(p_value.model, 'br_'+p_value.field.backref) 
+            p_value.__dict__.update(getattr(p_value.model, 'br_'+p_value.field.backref).__dict__) 
             setattr(p_value,'class', p_value.__class__.__name__)
             for key, value in p_value.__dict__.items():
                 t_return[key] = self.serialize(value)
         elif ManyToManyField in inspect.getmro(p_value.__class__):
             if p_value._is_backref:
                 p_value.__dict__.update(getattr(p_value.model, 'br_'+p_value.name).__dict__) 
             setattr(p_value,'class', p_value.__class__.__name__)
```

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.25/decore_base/classes/decore_prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 from ..globals import globals
 from argparse import ArgumentParser
 from pathlib import Path
 from dirsync import sync
 from shutil import copyfile
 import PyInstaller.__main__
-import sys
 
 
 #TODO reprogramm this class > method for every condition in arg switch > classmethod for every helper function
 class Decore_prompt(object):
     def __init__(self):
         self.parser = ArgumentParser()
         
         self.parser.add_argument('--prepare', action='store_true', help='Prepare decore Base application with helper files to get startet')
-        self.parser.add_argument('--sample', action='store_true', help='Copy the "decore Base" sample application to project root folder')
         self.parser.add_argument('--dev', action='store_true', help='Run decore Base application in development mode')
         self.parser.add_argument('--build', action='store_true', help='Build decore Base application for production')
         self.args, t_unknown_args = self.parser.parse_known_args()
 
         if not t_unknown_args:
             if self.args.prepare:
                 self.copy_launch()
                 self.copy_gitignore()
                 self.sync_spa()
                 self.create_base_dir()
                 self.create_model_dir()
                 exit()
-            elif self.args.sample:
-                if not globals.config.app_id == '364871e4-6727-4e1f-80a2-acc9c83ace92':
-                    self.sync_sample()
-                    exit()
-                else:
-                    raise Exception('You can not use the "sample" command in sample project context')
             elif self.args.dev:
                 globals.flags.purge_unused_database_cols = False
                 globals.flags.dev_mode = True
                 self.sync_spa()
-                
             elif self.args.build:
                 PyInstaller.__main__.run([
                     '--paths="."',
                     '--add-data=spa;spa',
                     '--collect-data=pykeepass',
                     'app.py'
                 ])
@@ -66,20 +57,14 @@
     def sync_spa(self):
         t_prepare_path = Path(__file__).parent.parent.joinpath('prepare')
         t_spa_source = t_prepare_path.joinpath('spa')
         t_spa_destination = Path('spa')
         t_spa_destination.mkdir(parents=True, exist_ok=True)
         sync(str(t_spa_source.absolute()), str(t_spa_destination.absolute()), 'sync', purge=True)
 
-    def sync_sample(self):
-        t_sample_source = Path(__file__).parent.parent.joinpath('sample')
-        t_sample_destination = Path('sample')
-        t_sample_destination.mkdir(parents=True, exist_ok=True)
-        sync(str(t_sample_source.absolute()), str(t_sample_destination.absolute()), 'sync', purge=True)
-    
     def create_base_dir(self):
         t_bases_init_path = Path('bases').joinpath('__init__.py')
         if not t_bases_init_path.exists():
             t_bases_init_path.parent.mkdir(parents=True, exist_ok=True)
             with open(t_bases_init_path, 'w'): pass
 
     def create_model_dir(self):
```

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_query.py` & `decore_Base-0.0.25/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_return.py` & `decore_Base-0.0.25/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_translate.py` & `decore_Base-0.0.25/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/classes/decore_view.py` & `decore_Base-0.0.25/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/decore.py` & `decore_Base-0.0.25/decore_base/decore.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 import json, logging
 from str2type import str2type
 from pathlib import Path
 from collections import OrderedDict
 
 
 class Decore(object):
+    '''
+    This class provides all the necessary functions to define a decore app and passes the collected information to the pool. It also holds the routes for communication with decore Front.
+    '''
     def __init__(self):
         if not globals.flags.production_mode:
             self.prompt = Decore_prompt()
         self.pool = Decore_pool()
         self.api = self.get_api()
         Decore_query.create_table(safe=True)
         
@@ -80,38 +83,86 @@
             logger.setLevel(logging.WARNING)
             serve(self.api, host=HOST, port=PORT)
             
         else:
             self.api.run(HOST, PORT)
 
     def app(self, title):
-        '''Decorator for app registration'''
+        '''
+        A function for opening an app. It is used as a decorator.
+
+        :param str title: The title of the app.
+
+        .. code-block:: python
+
+            @decore.app(title='My App')
+            def main():
+                pass
+        '''
         def wrapper(func):
             self.pool.register(Decore_app('app', None, None, None, title, None, func.__doc__))
             self.pool.extend()
             i_base: Decore_base
             for i_base in self.pool.base_s:
                 i_base.start_shot()
                 i_base.start_work()
             self.start_api()
         return wrapper
 
     def base(self, icon=None, title=None, desc=None, model=Decore_model):
+        '''
+        A function for opening a base. It is used as a decorator.
+
+            The base is the carrier element for the view and the template for the data source.
+
+        :param str icon: The icon of the base.
+        :param str title: The title of the base.
+        :param str desc: The description of the base.
+        :param Model model: The data model of the base. It forms a kind of context for all child elements of the base.
+
+        .. code-block:: python
+
+            @decore.base(icon='mdi-account', title='Person', desc='A basis for managing personal data', model=Person)
+            class Person_base:
+                pass
+        '''
         def wrapper(cls):
             t_base = Decore_base(cls.__name__, icon, title, desc, model)
             t_base.__class__ = type(cls.__name__, (Decore_base, cls), {
                 '__init__': cls.__init__(t_base),
             })
             self.pool.register(t_base)
         return wrapper
 
     l_view_type = Literal['table']
     l_view_pag_type = Literal['client']
 
     def view(self, parent_id=None, icon=None, title=None, desc=None, type: l_view_type = 'table', fields=[], filters=[], query={}, pag_type: l_view_pag_type = 'client', pag_recs=16):
+        '''
+        A function to register a view. It is used as a decorator.
+
+            A view is a container for displaying data.
+        
+        :param str parent_id: The ID of the parent element. Only to be set if the view is to be rendered in another base.
+        :param str icon: The icon of the view.
+        :param str title: The title of the view.
+        :param str desc: The description of the view.
+        :param str type: The type of the view.
+        :param list fields: The active fields of the view.
+        :param list filters: The fields that are used in filter.
+        :param dict query: The default query of the view.
+        :param str pag_type: The pagination type of the view.
+        :param int pag_recs: The pagination records of the view.
+
+        .. code-block:: python
+
+            @decore.view(icon='mdi-account', title='Person', desc='A view for managing personal data', type='table', fields=[Person.id, Person.name, Person.age], filters=[Person.name, Person.age], query={'name__eq': 'Kemo'}, pag_type='client', pag_recs=16)
+            def person_view():
+                pass
+        '''
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
                 t_parent_id = parent_id
             t_source_id = t_parent_s[0]
@@ -121,28 +172,68 @@
 
     l_dialog_type = Literal['standard', 'tabs', 'stepper']
     l_dialog_display = Literal['modal', 'drawer']
     l_dialog_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
 
     # TODO - Überprüfen ob element mit gleicher ID schon vorhanden ist und Execption
     def dialog(self, parent_id=None, icon=None, title=None, desc=None, type: l_dialog_type = 'standard', display: l_dialog_display = 'drawer', activator: l_dialog_activator = 'none'):
+        '''
+        A function to register a dialog. It is used as a decorator.
+
+            A dialog is a carrier for widgets.
+
+        :param str parent_id: The ID of the parent element. Only to be set if the dialog is to be rendered in a view of another base.
+        :param str icon: The icon of the dialog.
+        :param str title: The title of the dialog.
+        :param str desc: The description of the dialog.
+        :param str type: The type of the dialog.
+        :param str display: The display type of the dialog.
+        :param str activator: The activator type of the dialog.
+
+        .. code-block:: python
+
+            @decore.dialog(icon='mdi-account', title='Person', desc='A dialog for managing personal data', type='standard', display='drawer', activator='default-menu')
+            def person_dialog():
+                pass
+                
+        '''
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
                 t_parent_id = parent_id
             t_source_id = t_parent_s[0]
             self.pool.register(Decore_dialog(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, display, activator))
             func()
         return wrapper
 
     l_widget_type = Literal['default', 'info', 'form', 'table']
 
     def widget(self, parent_id=None, icon=None, title=None, desc=None, type: l_widget_type = 'default', layout='cera', fields=[]):
+        '''
+        A function to register a widget. It is used as a decorator.
+
+            A widget is an element for displaying or editing a single item from the data.
+
+        :param str parent_id: The ID of the parent element. Only to be set if the widget is to be rendered in a dialog of another base.
+        :param str icon: The icon of the widget.
+        :param str title: The title of the widget.
+        :param str desc: The description of the widget.
+        :param str type: The type of the widget.
+        :param str layout: The layout of the widget.
+        :param list fields: The active fields of the widget.
+
+        .. code-block:: python
+        
+            @decore.widget(icon='mdi-account', title='Person', desc='A widget for managing personal data', type='form', layout='cera', fields=[Person.name, Person.age])
+            def person_widget():
+                pass
+                
+        '''
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
                 t_parent_id = parent_id
             t_source_id = t_parent_s[0]
```

### Comparing `decore_Base-0.0.24/decore_base/globals.py` & `decore_Base-0.0.25/decore_base/globals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
-from pykeepass import create_database, PyKeePass
 from uuid import uuid4
 import json,logging,sys
 
+from .classes.globals_keybase import Global_keybase
+
 logging.basicConfig(format='[%(levelname)s] | %(message)s', level=logging.INFO)
 
 class Global_flags(object):
     def __init__(self):
         self.production_mode = self.set_production_mode()
         self.dev_mode = False
         self.purge_unused_database_cols = False
@@ -53,19 +54,10 @@
     def server_port(self):
         return self.__data__['remote']['server_port']
 
 class Globals(object):
     def __init__(self):
         self.flags = Global_flags()
         self.config = Global_config()
-        #TODO - move to model
-        self.kdb = self.get_kdb()
+        self.keybase = Global_keybase(Path().joinpath(self.config.state_path).joinpath('keybase.kdbx'))
 
-    #TODO - move to model
-    def get_kdb(self):
-        t_kdp_path = Path().joinpath(self.config.state_path).joinpath('keybase.kdbx')
-        t_kdp_path.parent.mkdir(parents=True, exist_ok=True)
-        if not t_kdp_path.exists():
-            create_database(str(t_kdp_path.absolute()), password='12345678')
-        return PyKeePass(str(t_kdp_path.absolute()), password='12345678')
-    
 globals = Globals()
```

### Comparing `decore_Base-0.0.24/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.25/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/powershell.py` & `decore_Base-0.0.25/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/powershell2.py` & `decore_Base-0.0.25/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/return_value.py` & `decore_Base-0.0.25/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.25/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.25/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.25/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/.gitignore` & `decore_Base-0.0.25/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.25/decore_base/prepare/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.25/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.25/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.25/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.25/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.25/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/js/586.6cfbf2b5.js` & `decore_Base-0.0.25/decore_base/prepare/spa/static/js/586.6cfbf2b5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.25/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/js/app.aff5db90.js` & `decore_Base-0.0.25/decore_base/prepare/spa/static/js/app.aff5db90.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/static/js/vendor.6fe961ae.js` & `decore_Base-0.0.25/decore_base/prepare/spa/static/js/vendor.6fe961ae.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.25/decore_base/prepare/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/conform_model.py` & `decore_Base-0.0.25/decore_base/uniform/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/depricated/askform_base.py` & `decore_Base-0.0.25/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/depricated/buyform_base.py` & `decore_Base-0.0.25/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/depricated/conform_base.py` & `decore_Base-0.0.25/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/depricated/deform_base.py` & `decore_Base-0.0.25/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/perform_model.py` & `decore_Base-0.0.25/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/reform_client_model.py` & `decore_Base-0.0.25/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/decore_base/uniform/reform_server_model.py` & `decore_Base-0.0.25/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.24/setup.cfg` & `decore_Base-0.0.25/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -13,75 +13,54 @@
 	Operating System :: Microsoft :: Windows
 
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
-	alabaster==0.7.13
 	altgraph==0.17.3
 	argon2-cffi==21.3.0
 	argon2-cffi-bindings==21.2.0
-	Babel==2.12.1
 	blinker==1.6.2
 	Cerberus==1.3.4
 	certifi==2023.5.7
 	cffi==1.15.1
 	charset-normalizer==3.1.0
 	click==8.1.3
 	colorama==0.4.6
 	construct==2.10.68
-	coverage==7.2.5
 	dirsync==2.2.5
-	docutils==0.20.1
-	exceptiongroup==1.1.1
 	Flask==2.3.2
-	Flask-Cors==3.0.10
+	Flask-Cors==4.0.0
 	Flask-WTF==1.1.1
 	future==0.18.3
 	idna==3.4
-	imagesize==1.4.1
-	importlib-metadata==6.6.0
-	iniconfig==2.0.0
+	importlib-metadata==6.7.0
 	itsdangerous==2.1.2
 	Jinja2==3.1.2
 	libretranslatepy==2.1.1
 	lxml==4.9.2
-	MarkupSafe==2.1.2
-	mimesis==9.0.0
-	packaging==23.1
+	MarkupSafe==2.1.3
+	mimesis==10.1.0
 	peewee==3.16.2
 	pefile==2023.2.7
-	pluggy==1.0.0
 	pycparser==2.21
-	pycryptodomex==3.17
-	Pygments==2.15.1
-	pyinstaller==5.11.0
-	pyinstaller-hooks-contrib==2023.3
-	pykeepass==4.0.3
-	pytest==7.3.1
-	pytest-cov==4.0.0
+	pycryptodomex==3.18.0
+	pyinstaller==5.13.0
+	pyinstaller-hooks-contrib==2023.4
+	pykeepass==4.0.5
 	python-dateutil==2.8.2
-	pywin32-ctypes==0.2.0
-	requests==2.30.0
+	pywin32-ctypes==0.2.2
+	requests==2.31.0
 	six==1.16.0
-	snowballstemmer==2.2.0
-	Sphinx==7.0.1
-	sphinxcontrib-applehelp==1.0.4
-	sphinxcontrib-devhelp==1.0.2
-	sphinxcontrib-htmlhelp==2.0.1
-	sphinxcontrib-jsmath==1.0.1
-	sphinxcontrib-qthelp==1.0.3
-	sphinxcontrib-serializinghtml==1.1.5
 	str2type==0.4.1
-	tomli==2.0.1
 	translate==3.6.1
-	urllib3==2.0.2
+	urllib3==2.0.3
 	waitress==2.1.2
-	Werkzeug==2.3.4
+	Werkzeug==2.3.6
 	WTForms==3.0.1
 	zipp==3.15.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

