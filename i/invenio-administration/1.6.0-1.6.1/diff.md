# Comparing `tmp/invenio-administration-1.6.0.tar.gz` & `tmp/invenio-administration-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-administration-1.6.0.tar", last modified: Mon Jul  3 08:43:34 2023, max compression
+gzip compressed data, was "dist/invenio-administration-1.6.1.tar", last modified: Fri Jul  7 13:47:26 2023, max compression
```

## Comparing `invenio-administration-1.6.0.tar` & `invenio-administration-1.6.1.tar`

### file list

```diff
@@ -1,379 +1,451 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.eslintrc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)   132884 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/marshmallow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/menu/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/menu/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32571 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/static/images/dashboard.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/details.html
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration/views/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/views/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/invenio_administration/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/invenio_administration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 08:43:33.000000 invenio-administration-1.6.0/invenio_administration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/mock_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:34.000000 invenio-administration-1.6.0/tests/mock_module/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/mock_module/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/mock_module/administration/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/mock_module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/test_admin_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/test_details_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/test_invenio_administration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:43:27.000000 invenio-administration-1.6.0/tests/test_list_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.eslintrc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)   132884 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/marshmallow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/menu/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32571 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/static/images/dashboard.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/views/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/invenio_administration/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/invenio_administration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/mock_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:26.000000 invenio-administration-1.6.1/tests/mock_module/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/mock_module/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/mock_module/administration/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/mock_module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/test_admin_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/test_details_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/test_invenio_administration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:47:14.000000 invenio-administration-1.6.1/tests/test_list_view.py
```

### Comparing `invenio-administration-1.6.0/.editorconfig` & `invenio-administration-1.6.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/.github/workflows/pypi-publish.yml` & `invenio-administration-1.6.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/.github/workflows/tests.yml` & `invenio-administration-1.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/.tx/config` & `invenio-administration-1.6.1/.tx/config`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2022 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # invenio-administration is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 # TODO: Transifex integration
 #
@@ -20,17 +21,17 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-administration-messages]
+[o:inveniosoftware:p:invenio:r:invenio-administration-messages]
 file_filter = invenio_administration/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_administration/translations/messages.pot
 source_lang = en
 type = PO
 
 # Translate JavaScript strings
 # 1) Navigate to the invenio_administration/assets/semantic-ui/translations/invenio_administration folder
@@ -55,13 +56,12 @@
 # 9) Pull translations for all languages from Transifex
 #    $ tx pull -a
 # 10) Compile .po files for all languages
 #    $ npm run compile_catalog
 # 11) Convert .po file for a single language
 #    $ npm run compile_catalog lang <lang>
 
-[invenio.invenio-administration-messages-ui]
+[o:inveniosoftware:p:invenio:r:invenio-administration-messages-ui]
 file_filter = invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/<lang>/messages.po
 source_file = invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
 source_lang = en
 type = PO
-
```

### Comparing `invenio-administration-1.6.0/CHANGES.rst` & `invenio-administration-1.6.1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     invenio-administration is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.6.1 (2023-07-07)
+
+- skip `fields.Method` from jsonify
+
 Version 1.6.0 (2023-07-03)
 
 - Adding a mapping for the fields.Method
 
 Version 1.5.0 (2023-06-15)
 
 - setup: upgrade invenio dependencies
```

### Comparing `invenio-administration-1.6.0/CONTRIBUTING.rst` & `invenio-administration-1.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/MANIFEST.in` & `invenio-administration-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/PKG-INFO` & `invenio-administration-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 1.6.0
+Version: 1.6.1
 Summary: "Invenio module that adds administration panel to the system."
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.6.1 (2023-07-07)
+        
+        - skip `fields.Method` from jsonify
+        
         Version 1.6.0 (2023-07-03)
         
         - Adding a mapping for the fields.Method
         
         Version 1.5.0 (2023-06-15)
         
         - setup: upgrade invenio dependencies
```

### Comparing `invenio-administration-1.6.0/README.rst` & `invenio-administration-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/docs/Makefile` & `invenio-administration-1.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/docs/conf.py` & `invenio-administration-1.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/docs/index.rst` & `invenio-administration-1.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/docs/make.bat` & `invenio-administration-1.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/admin.py` & `invenio-administration-1.6.1/invenio_administration/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # 
 # Translators:
 # Bessem Aamira <bessemamira@gmail.com>, 2022
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
@@ -56,18 +56,18 @@
 msgid "Delete"
 msgstr "حذف"
 
 msgid "Cancel"
 msgstr "إلغاء"
 
 msgid "Delete {{title}}"
-msgstr "حذف {{عنوان}}"
+msgstr "حذف  {{title}}"
 
 msgid "Are you sure you want to delete {{resourceName}}? "
-msgstr "هل أنت متأكد من حذف {{إسم المورد}} ؟"
+msgstr "هل أنت متأكد من حذف {{resourceName}}؟"
 
 msgid "Error"
 msgstr "خطأ"
 
 msgid "Server was not able to process your request."
 msgstr "الموزّع لم يتمكّن من معالجة طلبك."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -28,53 +28,53 @@
 msgid "results per page"
 msgstr ""
 
 msgid "result(s) found"
 msgstr ""
 
 msgid "Add"
-msgstr "Ajouter"
+msgstr "Aggiungi"
 
 msgid "Remove field"
 msgstr ""
 
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "Éditer"
+msgstr "Modifica"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "Supprimer"
+msgstr "Cancella"
 
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Annulla"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "Erreur"
+msgstr "Errore"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
-msgstr "Enregistrer"
+msgstr "Memorizza"
 
 msgid "Search"
-msgstr "Recherche"
+msgstr "Cerca"
 
 msgid "Clear query"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
@@ -64,15 +65,15 @@
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr "Biztosan törölni akarja? {{resourceName}}?"
 
 msgid "Error"
 msgstr "Hiba"
 
 msgid "Server was not able to process your request."
-msgstr "A szerver nem tudta feldolgozni az ön kérését."
+msgstr "A szerver nem tudta feldolgozni az Ön kérését."
 
 msgid "Save"
 msgstr "Mentés"
 
 msgid "Search"
 msgstr "Keresés"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Alizee Pace <alizee.pace@gmail.com>, 2022
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: pt\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -28,53 +27,53 @@
 msgid "results per page"
 msgstr ""
 
 msgid "result(s) found"
 msgstr ""
 
 msgid "Add"
-msgstr "Aggiungi"
+msgstr ""
 
 msgid "Remove field"
 msgstr ""
 
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "Modifica"
+msgstr "Editar"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "Cancella"
+msgstr "Apagar"
 
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancelar"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "Errore"
+msgstr "Erro"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
-msgstr "Memorizza"
+msgstr ""
 
 msgid "Search"
-msgstr "Cerca"
+msgstr "Pesquisar"
 
 msgid "Clear query"
 msgstr ""
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ja\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: no\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -27,53 +27,53 @@
 msgid "results per page"
 msgstr ""
 
 msgid "result(s) found"
 msgstr ""
 
 msgid "Add"
-msgstr ""
+msgstr "Legg til"
 
 msgid "Remove field"
 msgstr ""
 
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "編集"
+msgstr "Endre"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "削除"
+msgstr "Slett"
 
 msgid "Cancel"
-msgstr "キャンセル"
+msgstr "Avbryt"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "エラー"
+msgstr "Feil"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
 msgstr ""
 
 msgid "Search"
-msgstr "検索"
+msgstr "Søk"
 
 msgid "Clear query"
 msgstr ""
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: no\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: sk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -27,53 +27,53 @@
 msgid "results per page"
 msgstr ""
 
 msgid "result(s) found"
 msgstr ""
 
 msgid "Add"
-msgstr "Legg til"
+msgstr ""
 
 msgid "Remove field"
 msgstr ""
 
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "Endre"
+msgstr "Editovať"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "Slett"
+msgstr "Zmazať"
 
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Preruš"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "Feil"
+msgstr "Chyba"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
-msgstr ""
+msgstr "Nahraj"
 
 msgid "Search"
-msgstr "Søk"
+msgstr "Hľadaj"
 
 msgid "Clear query"
 msgstr ""
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -39,41 +39,41 @@
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "Editar"
+msgstr "編輯"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "Apagar"
+msgstr "刪除"
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "Erro"
+msgstr "錯誤"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
 msgstr ""
 
 msgid "Search"
-msgstr "Pesquisar"
+msgstr "搜尋"
 
 msgid "Clear query"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: rw\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: ja\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -39,41 +39,41 @@
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "Editovať"
+msgstr "編集"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "Zmazať"
+msgstr "削除"
 
 msgid "Cancel"
-msgstr "Preruš"
+msgstr "キャンセル"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "Chyba"
+msgstr "エラー"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
-msgstr "Nahraj"
+msgstr ""
 
 msgid "Search"
-msgstr "Hľadaj"
+msgstr "検索"
 
 msgid "Clear query"
 msgstr ""
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Sam Arbid, 2022
+# Rim Sharif, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
@@ -25,15 +26,15 @@
 msgid "No matching resources found."
 msgstr "Inga matchande resurser hittades."
 
 msgid "results per page"
 msgstr "resultat per sida"
 
 msgid "result(s) found"
-msgstr "result(at) hittades"
+msgstr "resultat hittades"
 
 msgid "Add"
 msgstr "Lägg till"
 
 msgid "Remove field"
 msgstr "Ta bort fält"
 
@@ -64,15 +65,15 @@
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr "Är du säker på att du vill ta bort {{resourceName}}?"
 
 msgid "Error"
 msgstr "Fel"
 
 msgid "Server was not able to process your request."
-msgstr "Servern kunde inte behandla din begäran."
+msgstr "Servern kunde inte behandla din förfrågan."
 
 msgid "Save"
 msgstr "Spara"
 
 msgid "Search"
 msgstr "Sök"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
-# 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
@@ -69,11 +65,11 @@
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
 msgstr ""
 
 msgid "Search"
-msgstr "Пошук"
+msgstr ""
 
 msgid "Clear query"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
+# Alizee Pace <alizee.pace@gmail.com>, 2022
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:25:02.203Z\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: fr\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Search ..."
 msgstr ""
 
 msgid "There is no resources in this category."
 msgstr ""
@@ -27,53 +28,53 @@
 msgid "results per page"
 msgstr ""
 
 msgid "result(s) found"
 msgstr ""
 
 msgid "Add"
-msgstr ""
+msgstr "Ajouter"
 
 msgid "Remove field"
 msgstr ""
 
 msgid "Sort"
 msgstr ""
 
 msgid "Resource is not editable."
 msgstr ""
 
 msgid "Edit"
-msgstr "編輯"
+msgstr "Éditer"
 
 msgid "Resource is not deletable."
 msgstr ""
 
 msgid "Open list of actions"
 msgstr ""
 
 msgid "Delete"
-msgstr "刪除"
+msgstr "Supprimer"
 
 msgid "Cancel"
-msgstr "取消"
+msgstr "Annuler"
 
 msgid "Delete {{title}}"
 msgstr ""
 
 msgid "Are you sure you want to delete {{resourceName}}? "
 msgstr ""
 
 msgid "Error"
-msgstr "錯誤"
+msgstr "Erreur"
 
 msgid "Server was not able to process your request."
 msgstr ""
 
 msgid "Save"
-msgstr ""
+msgstr "Enregistrer"
 
 msgid "Search"
-msgstr "搜尋"
+msgstr "Recherche"
 
 msgid "Clear query"
 msgstr ""
```

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot` & `invenio-administration-1.6.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/config.py` & `invenio-administration-1.6.1/invenio_administration/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/errors.py` & `invenio-administration-1.6.1/invenio_administration/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/ext.py` & `invenio-administration-1.6.1/invenio_administration/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/generators.py` & `invenio-administration-1.6.1/invenio_administration/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/marshmallow_utils.py` & `invenio-administration-1.6.1/invenio_administration/marshmallow_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     fields.Time: "time",
     fields.Date: "date",
     fields.TimeDelta: "timedelta",
     fields.Decimal: "decimal",
     # TODO: This is needed for the is_current_user in the administration
     # of the user resources. It might be better to implement also a handler for this.
     # See https://github.com/inveniosoftware/invenio-administration/issues/174
-    fields.Method:  None,
+    # For the moment it is skipped when we call `jsonify_schema`
+    fields.Method: None,
     # invenio fields
     invenio_fields.SanitizedUnicode: "string",
     invenio_fields.links.Links: "array",
     invenio_fields.links.Link: "string",
     invenio_fields.tzdatetime.TZDateTime: "datetime",
     invenio_fields.sanitizedhtml.SanitizedHTML: "string",
 }
@@ -51,16 +52,18 @@
 
 def jsonify_schema(schema):
     """Marshmallow schema to dict."""
     schema_dict = {}
 
     for field, field_type in schema.fields.items():
         is_links = isinstance(field_type, invenio_fields.links.Links)
+        # skip `fields.Method`
+        is_method = isinstance(field_type, fields.Method)
 
-        if is_links:
+        if is_links or is_method:
             continue
 
         is_read_only = field_type.dump_only
         is_create_only = field_type.metadata["create_only"] \
             if "create_only" in field_type.metadata else False
 
         field_type_name = field_type.__class__
```

### Comparing `invenio-administration-1.6.0/invenio_administration/menu/menu.py` & `invenio-administration-1.6.1/invenio_administration/menu/menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/static/images/dashboard.png` & `invenio-administration-1.6.1/invenio_administration/static/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/base.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/create.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/details.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/edit.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/index.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/search.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-administration-1.6.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/af/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/af/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ar/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,60 +3,59 @@
 # This file is distributed under the same license as the
 # invenio-administration project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Bessem Aamira <bessemamira@gmail.com>, 2022
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
-msgstr "تمّت تهيئة مورد غير صالح {مورد} للعرض {عرض}."
+msgstr "تمّت تهيئة مورد غير صالح {resource} للعرض {view}."
 
 #: invenio_administration/errors.py:35
 msgid "No extension found with name '{extension_name}' ."
-msgstr "لا يوجد إمتداد بإسم '{إسم_الإمتداد}'."
+msgstr "لا يوجد إمتداد بإسم '{extension_name}'."
 
 #: invenio_administration/errors.py:47
 msgid "Invalid actions configuration, order or schema missing"
 msgstr "إجراءات التهيئة غير صالحة، الترتيب أو المخطّط مفقود"
 
 #: invenio_administration/errors.py:57
 msgid "Cannot instantiate resource view {name} without a resource."
-msgstr "لا يمكن إنشاء مثيل عرض مورد {الإسم} بدون مورد."
+msgstr "لا يمكن إنشاء مثيل عرض مورد {name} بدون مورد."
 
 #: invenio_administration/errors.py:72
 msgid ""
 "Cannot instantiate resource view {name} without an associated flask "
 "extension."
 msgstr ""
-"لا يمكن إنشاء مثيل عرض مورد {الإسم} ليس مرتبطا بإمتداد فلاسك flask "
-"extension."
+"لا يمكن إنشاء مثيل عرض مورد {name} ليس مرتبطا بإمتداد فلاسك flask extension."
 
 #: invenio_administration/errors.py:87
 msgid ""
 "Cannot instantiate administration view {name} without a default GET view"
-msgstr "لا يمكن إنشاء مثيل تصرّف في عرض {الإسم} بدون default GET view."
+msgstr "لا يمكن إنشاء مثيل تصرّف في عرض {name} بدون default GET view."
 
 #: invenio_administration/menu/menu.py:75
 #, python-format
 msgid "%(icon)s Administration"
 msgstr "%(icon)sالإدارة"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/base.html:26
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/bg/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ca/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/cs/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/da/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: da\n"
+"Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
 msgstr ""
 
 #: invenio_administration/errors.py:35
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/de/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/de/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/el/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/el/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/en/LC_MESSAGES/messages.mo` & `invenio-administration-1.6.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/en/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/es/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/et/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/et/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Persian (Iran) (https://app.transifex.com/inveniosoftware/teams/23537/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fa_IR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
 msgstr ""
 
 #: invenio_administration/errors.py:35
 msgid "No extension found with name '{extension_name}' ."
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/fa/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/fr/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/gl/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
+"Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
 msgstr ""
 
 #: invenio_administration/errors.py:35
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/hr/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/hu/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-administration project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -68,15 +69,15 @@
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/index.html:29
 msgid "Welcome to Invenio Administration"
 msgstr "Üdvözöljük az Invenio Administration felületén"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/index.html:30
 msgid "My managment tool"
-msgstr "Kezelő eszközeim"
+msgstr "Kezelőeszközeim"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/macros.html:14
 msgid "Back"
 msgstr "Vissza"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/search.html:26
 msgid "Create"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/it/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/it/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ja/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ka/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/lt/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/messages.pot` & `invenio-administration-1.6.1/invenio_administration/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/no/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/no/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/pl/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/pt/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ro/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-administration project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
+# Nicolaie Constantinescu, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Last-Translator: Nicolaie Constantinescu, 2023\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
@@ -101,19 +102,19 @@
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header.html:72
 msgid "Dashboard"
 msgstr ""
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:17
 msgid "Log in"
-msgstr ""
+msgstr "Log in"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:21
 msgid "Sign up"
-msgstr ""
+msgstr "Sign up"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:32
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:41
 msgid "New OAI-PMH set"
 msgstr ""
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:38
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/ru/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/rw/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/ne/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Nepali (https://app.transifex.com/inveniosoftware/teams/23537/ne/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: ne\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
 msgstr ""
 
 #: invenio_administration/errors.py:35
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/sk/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/sv/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # This file is distributed under the same license as the
 # invenio-administration project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Sam Arbid, 2022
+# Rim Sharif, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -110,32 +111,32 @@
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:17
 msgid "Log in"
 msgstr "Logga in"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:21
 msgid "Sign up"
-msgstr "Skriva upp"
+msgstr "Registrera konto"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:32
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:41
 msgid "New OAI-PMH set"
 msgstr "Nytt OAI-PMH set"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:38
 msgid "Actions"
-msgstr "Aktioner"
+msgstr "Åtgärder"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:52
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:93
 msgid "My account"
 msgstr "Mitt konto"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:87
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:116
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html:123
 msgid "Log out"
 msgstr "Logga ut"
 
 #: invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html:1
 msgid "Toggle side menu"
-msgstr "Växla sidomenyn"
+msgstr "Växla sidomeny"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/tr/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/uk/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_administration/errors.py:21
 msgid "Invalid resource {resource} configured for view {view}."
 msgstr ""
 
 #: invenio_administration/errors.py:35
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Weizheng Lu, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-administration-1.6.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-administration 0.1.6\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:22+0200\n"
 "PO-Revision-Date: 2022-10-12 07:22+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-administration-1.6.0/invenio_administration/views/base.py` & `invenio-administration-1.6.1/invenio_administration/views/base.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/views/dashboard.py` & `invenio-administration-1.6.1/invenio_administration/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration/webpack.py` & `invenio-administration-1.6.1/invenio_administration/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/invenio_administration.egg-info/PKG-INFO` & `invenio-administration-1.6.1/invenio_administration.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 1.6.0
+Version: 1.6.1
 Summary: "Invenio module that adds administration panel to the system."
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.6.1 (2023-07-07)
+        
+        - skip `fields.Method` from jsonify
+        
         Version 1.6.0 (2023-07-03)
         
         - Adding a mapping for the fields.Method
         
         Version 1.5.0 (2023-06-15)
         
         - setup: upgrade invenio dependencies
```

### Comparing `invenio-administration-1.6.0/invenio_administration.egg-info/SOURCES.txt` & `invenio-administration-1.6.1/invenio_administration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 README.rst
 babel.ini
 pytest.ini
 run-js-linter.sh
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/i18n-pull.yml
+.github/workflows/i18n-push.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 .tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
@@ -116,42 +118,54 @@
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
@@ -160,18 +174,20 @@
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
+invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
 invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
 invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
 invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
 invenio_administration/menu/__init__.py
@@ -193,39 +209,53 @@
 invenio_administration/translations/af/LC_MESSAGES/messages.po
 invenio_administration/translations/ar/LC_MESSAGES/messages.po
 invenio_administration/translations/bg/LC_MESSAGES/messages.po
 invenio_administration/translations/ca/LC_MESSAGES/messages.po
 invenio_administration/translations/cs/LC_MESSAGES/messages.po
 invenio_administration/translations/da/LC_MESSAGES/messages.po
 invenio_administration/translations/de/LC_MESSAGES/messages.po
+invenio_administration/translations/de_AT/LC_MESSAGES/messages.po
+invenio_administration/translations/de_DE/LC_MESSAGES/messages.po
 invenio_administration/translations/el/LC_MESSAGES/messages.po
 invenio_administration/translations/en/LC_MESSAGES/messages.mo
 invenio_administration/translations/en/LC_MESSAGES/messages.po
+invenio_administration/translations/en_AT/LC_MESSAGES/messages.po
+invenio_administration/translations/en_HU/LC_MESSAGES/messages.po
 invenio_administration/translations/es/LC_MESSAGES/messages.po
+invenio_administration/translations/es_CU/LC_MESSAGES/messages.po
+invenio_administration/translations/es_MX/LC_MESSAGES/messages.po
 invenio_administration/translations/et/LC_MESSAGES/messages.po
 invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
 invenio_administration/translations/fa/LC_MESSAGES/messages.po
+invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_administration/translations/fr/LC_MESSAGES/messages.po
+invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_administration/translations/gl/LC_MESSAGES/messages.po
+invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_administration/translations/hr/LC_MESSAGES/messages.po
 invenio_administration/translations/hu/LC_MESSAGES/messages.po
+invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_administration/translations/it/LC_MESSAGES/messages.po
 invenio_administration/translations/ja/LC_MESSAGES/messages.po
 invenio_administration/translations/ka/LC_MESSAGES/messages.po
 invenio_administration/translations/lt/LC_MESSAGES/messages.po
+invenio_administration/translations/ne/LC_MESSAGES/messages.po
 invenio_administration/translations/no/LC_MESSAGES/messages.po
 invenio_administration/translations/pl/LC_MESSAGES/messages.po
 invenio_administration/translations/pt/LC_MESSAGES/messages.po
 invenio_administration/translations/ro/LC_MESSAGES/messages.po
 invenio_administration/translations/ru/LC_MESSAGES/messages.po
 invenio_administration/translations/rw/LC_MESSAGES/messages.po
 invenio_administration/translations/sk/LC_MESSAGES/messages.po
 invenio_administration/translations/sv/LC_MESSAGES/messages.po
+invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_administration/translations/tr/LC_MESSAGES/messages.po
 invenio_administration/translations/uk/LC_MESSAGES/messages.po
+invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
 invenio_administration/views/__init__.py
 invenio_administration/views/base.py
 invenio_administration/views/dashboard.py
 tests/conftest.py
 tests/test_admin_menu.py
```

### Comparing `invenio-administration-1.6.0/invenio_administration.egg-info/requires.txt` & `invenio-administration-1.6.1/invenio_administration.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/run-js-linter.sh` & `invenio-administration-1.6.1/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/run-tests.sh` & `invenio-administration-1.6.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/setup.cfg` & `invenio-administration-1.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/conftest.py` & `invenio-administration-1.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/mock_module/administration/mock.py` & `invenio-administration-1.6.1/tests/mock_module/administration/mock.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/mock_module/config.py` & `invenio-administration-1.6.1/tests/mock_module/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/test_admin_menu.py` & `invenio-administration-1.6.1/tests/test_admin_menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/test_base.py` & `invenio-administration-1.6.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.6.0/tests/test_invenio_administration.py` & `invenio-administration-1.6.1/tests/test_invenio_administration.py`

 * *Files identical despite different names*

