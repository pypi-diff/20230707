# Comparing `tmp/cognite_neat-0.14.1.tar.gz` & `tmp/cognite_neat-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.14.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.14.2.tar", max compression
```

## Comparing `cognite_neat-0.14.1.tar` & `cognite_neat-0.14.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    11351 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/LICENSE
--rw-r--r--   0        0        0     8765 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/README.md
--rw-r--r--   0        0        0       23 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0     9922 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7016 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14103 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11867 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      761 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2792 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1400 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     5053 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    30296 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    39839 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    18682 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6700 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    11439 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11914 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     8743 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    20731 2023-06-30 11:58:15.607223 cognite_neat-0.14.1/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0    11637 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4361 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      775 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6977 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-06-30 11:58:15.611223 cognite_neat-0.14.1/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79716 2023-06-30 11:58:15.619224 cognite_neat-0.14.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-06-30 11:58:15.619224 cognite_neat-0.14.1/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-06-30 11:58:15.619224 cognite_neat-0.14.1/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-06-30 11:58:15.619224 cognite_neat-0.14.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-06-30 11:58:15.619224 cognite_neat-0.14.1/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15613 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      315 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      270 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      291 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1040 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    24005 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4578 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-06-30 11:58:15.623224 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370103 2023-06-30 11:58:15.631225 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
--rw-r--r--   0        0        0     2667 2023-06-30 11:58:15.631225 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
--rw-r--r--   0        0        0  5883237 2023-06-30 11:58:15.663227 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
--rw-r--r--   0        0        0     2633 2023-06-30 11:58:15.667227 cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-30 11:58:15.671228 cognite_neat-0.14.1/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2577 2023-06-30 11:58:16.179267 cognite_neat-0.14.1/pyproject.toml
--rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/LICENSE
+-rw-r--r--   0        0        0     8765 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/README.md
+-rw-r--r--   0        0        0       23 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0     9922 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     7016 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14103 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11867 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0      761 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1400 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     5053 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    37631 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-07-07 11:11:16.038610 cognite_neat-0.14.2/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    39837 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    18682 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6698 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    11439 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0     1009 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15269 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1958 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11906 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     8743 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    20731 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0    11637 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4361 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      775 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6977 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79716 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-07-07 11:11:16.042610 cognite_neat-0.14.2/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-07-07 11:11:16.046610 cognite_neat-0.14.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15613 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      315 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      270 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      291 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1040 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    23999 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4578 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-07 11:11:16.050610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370103 2023-07-07 11:11:16.058610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
+-rw-r--r--   0        0        0     2667 2023-07-07 11:11:16.062610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883237 2023-07-07 11:11:16.094610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
+-rw-r--r--   0        0        0     2633 2023-07-07 11:11:16.094610 cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-07 11:11:16.098610 cognite_neat-0.14.2/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2577 2023-07-07 11:11:16.602612 cognite_neat-0.14.2/pyproject.toml
+-rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.14.2/PKG-INFO
```

### Comparing `cognite_neat-0.14.1/LICENSE` & `cognite_neat-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/README.md` & `cognite_neat-0.14.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.14.2/cognite/neat/base_workflows/graph2assets_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/base_workflows/graphs_and_rules.py` & `cognite_neat-0.14.2/cognite/neat/base_workflows/graphs_and_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/base_workflows/sheet2cdf.py` & `cognite_neat-0.14.2/cognite/neat/base_workflows/sheet2cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/base_workflows/sme_graph_capture.py` & `cognite_neat-0.14.2/cognite/neat/base_workflows/sme_graph_capture.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/constants.py` & `cognite_neat-0.14.2/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/app.py` & `cognite_neat-0.14.2/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/configuration.py` & `cognite_neat-0.14.2/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.14.2/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.14.2/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.14.2/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import logging
 import math
+import re
 import warnings
 from datetime import datetime
+from pathlib import Path
 from typing import Dict, List, Optional, Self, Union
 
 import pandas as pd
 from graphql import GraphQLBoolean, GraphQLFloat, GraphQLInt, GraphQLString
-from pydantic import BaseModel, Field, HttpUrl, ValidationError, parse_obj_as, root_validator, validator
+from pydantic import BaseModel, Field, HttpUrl, ValidationError, constr, parse_obj_as, root_validator, validator
 from rdflib import XSD, Literal, Namespace, URIRef
 
 from cognite.neat.core.configuration import PREFIXES, Tables
 from cognite.neat.core.data_classes.rules import Entity, RuleType, parse_rule
 
 # mapping of XSD types to Python and GraphQL types
 DATA_TYPE_MAPPING = {
@@ -23,72 +25,119 @@
     "nonNegativeInteger": {"python": "int", "GraphQL": GraphQLInt},
     "negativeInteger": {"python": "int", "GraphQL": GraphQLInt},
     "long": {"python": "int", "GraphQL": GraphQLInt},
     "string": {"python": "str", "GraphQL": GraphQLString},
     "anyURI": {"python": "str", "GraphQL": GraphQLString},
     "normalizedString": {"python": "str", "GraphQL": GraphQLString},
     "token": {"python": "str", "GraphQL": GraphQLString},
+    # Graphql does not have a datetime type this is CDF specific
+    "dateTime": {"python": "datetime", "GraphQL": "Timestamp"},
 }
 METADATA_VALUE_MAX_LENGTH = 5120
 
 
 class URL(BaseModel):
     url: HttpUrl
 
 
+Description = constr(min_length=1, max_length=255)
+
+
 class Resource(BaseModel):
     # Solution model
-    class_name: str = Field(alias="Class")
-    description: str = Field(alias="Description", default="")
+    description: Description = Field(alias="Description", default=None)
 
-    # Solution CDF resource
-    cdf_resource_type: str = Field(alias="Resource Type")
+    # Solution CDF resource, it is not needed when working with FDM, this is only for
+    # Classic CDF data model
+    cdf_resource_type: str = Field(alias="Resource Type", default=None)
 
-    # Solution model advance configuration
+    # Advance data modeling: Keeping track if Resource got deprecated or not
     deprecated: bool = Field(default=False)
     deprecation_date: Optional[datetime] = Field(alias="deprecationDate", default=None)
     replaced_by: str = Field(alias="replacedBy", default=None)
-    similar_to: HttpUrl = Field(alias="similarTo", default=None)
-    similarity_score: float = Field(alias="similarityScore", default=None)
-    equal_to: HttpUrl = Field(alias="equalTo", default=None)
+
+    # Advance data modeling: Relation to existing resources for purpose of mapping
+    source: HttpUrl = Field(
+        alias="Source", description="Source of information for given entity, e.g. CIM", default=None
+    )
+    source_entity_name: str = Field(
+        alias="Source Entity Name", description="Closest entity in source, e.g. Substation", default=None
+    )
+    match_type: str = Field(
+        alias="Match Type", description="Type of match between source entity and one being defined", default=None
+    )
+    comment: str = Field(alias="Comment", description="Comment about mapping", default=None)
+    issues: List[str] = Field(default=None, description="Storing list of pydantic validation issues")
+    valid: bool = Field(default=True, description="Indicates whether resource is valid or not")
 
     @validator(
         "deprecated",
         "deprecation_date",
         "replaced_by",
-        "similar_to",
-        "similarity_score",
-        "equal_to",
-        "description",
+        "source",
+        "source_entity_name",
+        "match_type",
+        "comment",
         pre=True,
     )
     def replace_float_nan_with_default(cls, value, field):
         if isinstance(value, float) and math.isnan(value):
             return field.default
         return value
 
+    class Config:
+        allow_population_by_field_name = True
+        anystr_strip_whitespace = True
+
+
+class_id_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]+[._-]{0,1}[a-zA-Z0-9]+)+$"
+
+ExternalId = constr(min_length=1, max_length=255)
+
 
 class Class(Resource):
+    class_id: ExternalId = Field(
+        alias="Class",
+    )
+    class_name: ExternalId = Field(alias="Name", default=None)
     # Solution model
-    parent_class: str = Field(alias="Parent Class", default=None)
+    parent_class: ExternalId = Field(alias="Parent Class", default=None)
 
     # Solution CDF resource
-    parent_asset: str = Field(alias="Parent Asset", default=None)
+    parent_asset: ExternalId = Field(alias="Parent Asset", default=None)
 
     @validator("parent_class", "parent_asset", pre=True)
     def replace_float_nan_with_default(cls, value, field):
         if isinstance(value, float) and math.isnan(value):
             return field.default
         return value
 
+    @validator("class_id", always=True)
+    def is_class_id_compliant(cls, value):
+        if not re.match(class_id_compliance_regex, value):
+            raise ValueError(
+                f"Invalid class_id {value} in Class sheet, it must obey regex {class_id_compliance_regex} !"
+            )
+        else:
+            return value
+
+    @validator("class_name", always=True)
+    def set_class_name_if_none(cls, value, values):
+        return values["class_id"] if value is None and "class_id" in values else value
+
+
+property_id_compliance_regex = r"^(\*)|(([a-zA-Z]+[a-zA-Z0-9]+[._-]{0,1}[a-zA-Z0-9]+)+)$"
+
 
 class Property(Resource):
     # Solution model
-    property_name: str = Field(alias="Property")
-    expected_value_type: str = Field(alias="Type")
+    class_id: ExternalId = Field(alias="Class")
+    property_id: ExternalId = Field(alias="Property")
+    property_name: ExternalId = Field(alias="Name", default=None)
+    expected_value_type: ExternalId = Field(alias="Type")
     min_count: Optional[int] = Field(alias="Min Count", default=0)
     max_count: Optional[int] = Field(alias="Max Count", default=None)
 
     # OWL property
     property_type: str = "DatatypeProperty"
 
     # Solution CDF resource
@@ -126,14 +175,45 @@
         pre=True,
     )
     def replace_float_nan_with_default(cls, value, field):
         if isinstance(value, float) and math.isnan(value):
             return field.default
         return value
 
+    @validator("class_id", always=True)
+    def is_class_id_compliant(cls, value):
+        if not re.match(class_id_compliance_regex, value):
+            raise ValueError(
+                f"Invalid class_id {value} in Property sheet, it must obey regex {class_id_compliance_regex} !"
+            )
+        else:
+            return value
+
+    @validator("property_id", always=True)
+    def is_property_id_compliant(cls, value):
+        if not re.match(property_id_compliance_regex, value):
+            raise ValueError(
+                f"Invalid property_id {value} in Property sheet, it must obey regex {property_id_compliance_regex} !"
+            )
+        else:
+            return value
+
+    @validator("expected_value_type", always=True)
+    def is_expected_value_type_compliant(cls, value):
+        if not re.match(class_id_compliance_regex, value):
+            raise ValueError(
+                f"Invalid Type {value} in Property sheet, it must obey regex {class_id_compliance_regex} !"
+            )
+        else:
+            return value
+
+    @validator("property_name", always=True)
+    def set_property_name_if_none(cls, value, values):
+        return values["property_id"] if value is None and "property_id" in values else value
+
     @validator("rule_type", pre=True)
     def to_lowercase(cls, value):
         return value.casefold() if value else value
 
     @validator("skip_rule", pre=True)
     def from_string(cls, value):
         if isinstance(value, str):
@@ -150,15 +230,15 @@
     def split_str(cls, v):
         if v:
             return [v.strip() for v in v.split(",")] if "," in v else [v]
 
     @validator("label")
     def set_relationship_label(cls, value, values):
         if "Relationship" in values.get("cdf_resource_type") and not value:
-            return values.get("property_name")
+            return values.get("property_id")
         return value
 
     @validator("cdf_resource_type", pre=True)
     def to_list_if_comma(cls, value, field):
         if isinstance(value, str):
             if value:
                 return value.replace(", ", ",").split(",")
@@ -177,71 +257,167 @@
     def no_rule(cls, value, values):
         if values.get("rule_type") is None:
             return True
         else:
             return value
 
 
+# regex expressions for compliance of Metadata sheet parsing
+prefix_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]+[_-]{0,1}[a-zA-Z0-9]+)+$"
+cdf_space_name_compliance_regex = rf"(?!^(space|cdf|dms|pg3|shared|system|node|edge)$)({prefix_compliance_regex})"
+data_model_name_compliance_regex = r"^([a-zA-Z]+[a-zA-Z0-9]+[_]{0,1}[a-zA-Z0-9])+$"
+version_compliance_regex = r"^([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+[_-]{1}[a-zA-Z0-9]+)|([0-9]+[_-]{1}[0-9]+[_-]{1}[0-9]+)|([0-9]+[_-]{1}[0-9])|([0-9]+)$"
+
+Prefix = constr(min_length=1, max_length=43)
+
+
 class Metadata(BaseModel):
-    prefix: str = Field(alias="shortName")
-    namespace: Namespace = None
-    version: str
-    isCurrentVersion: bool = True
+    prefix: Prefix = Field(
+        alias="shortName",
+        description="This is used as prefix for generation of RDF OWL/SHACL data model representation",
+    )
+    cdf_space_name: Prefix = Field(
+        description="This is used as CDF space name to which model is intend to be stored. By default it is set to 'playground'",
+        alias="cdfSpaceName",
+        default="playground",
+    )
+
+    namespace: Namespace = Field(
+        description="This is used as RDF namespace for generation of RDF OWL/SHACL data model representation and/or for generation of RDF graphs",
+        min_length=1,
+        max_length=2048,
+        default=None,
+    )
+    data_model_name: ExternalId = Field(
+        description="Name that uniquely identifies data model",
+        alias="dataModelName",
+        default=None,
+    )
+
+    version: str = Field(
+        min_length=1,
+        max_length=43,
+    )
+    is_current_version: bool = Field(alias="isCurrentVersion", default=True)
     created: datetime
     updated: datetime = Field(default_factory=lambda: datetime.utcnow())
-    title: str
-    description: Optional[str] = None
-    abstract: Optional[str] = None
+    title: str = Field(min_length=1, max_length=255)
+    description: Description
     creator: str | list[str]
     contributor: Optional[str | list[str]] = None
     rights: Optional[str] = "Restricted for Internal Use of Cognite"
     externalIdPrefix: str = Field(alias="externalIdPrefix", default=None)
-    data_set_id: int = Field(alias="dataSetId")
+    data_set_id: int = Field(alias="dataSetId", default=None)
+    imports: list[str] = Field(
+        description="Placeholder in case when data model is modular, i.e. provided as set of Excel files",
+        default=None,
+    )
+    source: str | Path = Field(
+        description="File path to Excel file which was used to produce Transformation Rules",
+        default=None,
+    )
+    issues: List[str] = Field(default=None, description="Storing list of pydantic validation issues")
+    valid: bool = Field(default=True, description="Indicates whether resource is valid or not")
 
     @validator(
         "externalIdPrefix",
         "contributor",
         "contributor",
         "description",
         "rights",
         pre=True,
     )
     def replace_float_nan_with_default(cls, value, field):
         if isinstance(value, float) and math.isnan(value):
             return field.default
         return value
 
+    @validator("prefix", always=True)
+    def make_prefix_compliant(cls, value):
+        repaired_string = re.sub(r"[^-_a-zA-Z0-9]", "", value.replace(" ", "-"))
+        if not re.match(prefix_compliance_regex, repaired_string):
+            raise ValueError(
+                f"Invalid prefix/shortName {value} in Metadata sheet, it must obey regex {prefix_compliance_regex} !"
+            )
+        else:
+            return repaired_string
+
+    @validator("cdf_space_name", always=True)
+    def make_cdf_space_name_compliant(cls, value):
+        repaired_string = re.sub(r"[^-_a-zA-Z0-9]", "", value.replace(" ", "-"))
+        if not re.match(cdf_space_name_compliance_regex, repaired_string):
+            raise ValueError(
+                f"Invalid cdfSpaceName {value} in Metadata sheet, it must obey regex {cdf_space_name_compliance_regex} !"
+            )
+        else:
+            return repaired_string
+
     @validator("namespace", always=True)
-    def set_namespace(cls, value, values):
+    def set_namespace_if_none(cls, value, values):
         if value is None:
-            return Namespace(f"http://purl.org/cognite/{values['prefix']}#")
+            if values["cdf_space_name"] == "playground":
+                return Namespace(f"http://purl.org/cognite/{values['prefix']}#")
+            else:
+                return Namespace(f"http://purl.org/cognite/{values['cdf_space_name']}/{values['prefix']}#")
         try:
-            _ = parse_obj_as(HttpUrl, value)
-            return Namespace(value)
+            return Namespace(parse_obj_as(HttpUrl, value))
         except ValidationError as e:
-            raise ValueError(f"Invalid namespace {value}, it must be a valid URL!") from e
+            raise ValueError(f"Invalid namespace {value} in Metadata sheet, it must be a valid URL!") from e
+
+    @validator("namespace", always=True)
+    def fix_namespace_ending(cls, value):
+        return value if value.endswith("#") or value.endswith("/") else f"{value}#"
+
+    @validator("data_model_name", always=True)
+    def set_data_model_name_if_none(cls, value, values):
+        return values["prefix"] if value is None else value
+
+    @validator("data_model_name", always=True)
+    def make_data_model_name_compliant(cls, value):
+        repaired_string = re.sub(r"[^_a-zA-Z0-9]", "", re.sub("[- .]+", "_", value))
+        if not re.match(data_model_name_compliance_regex, repaired_string):
+            raise ValueError(
+                f"Invalid name {repaired_string} in Metadata sheet, it must obey regex {data_model_name_compliance_regex} !"
+            )
+        else:
+            return repaired_string
+
+    @validator("version", always=True)
+    def make_version_compliant(cls, value):
+        repaired_string = re.sub(r"[^-_a-zA-Z0-9]", "", re.sub("[ .]+", "_", value))
+        if not re.match(version_compliance_regex, repaired_string):
+            raise ValueError(
+                f"Invalid version {repaired_string} in Metadata sheet, it must obey regex {version_compliance_regex} !"
+            )
+        else:
+            return repaired_string
 
     @validator("creator", "contributor")
     def to_list_if_comma(cls, value, field):
         if isinstance(value, str):
             if value:
                 return value.replace(", ", ",").split(",")
             if field.default is None:
                 return None
         return value
 
     class Config:
         allow_population_by_field_name = True
+        anystr_strip_whitespace = True
 
     @classmethod
     def create_from_dataframe(cls, raw_dfs) -> Self:
         expected_tables = Tables.as_set()
         if missing_tables := (expected_tables - set(raw_dfs)):
             raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
-        return Metadata(**dict(zip(raw_dfs[Tables.metadata][0], raw_dfs[Tables.metadata][1])))
+
+        return Metadata(
+            **dict(zip(raw_dfs[Tables.metadata][0], raw_dfs[Tables.metadata][1])),
+            source=raw_dfs[Tables.metadata].source if "source" in dir(raw_dfs[Tables.metadata]) else None,
+        )
 
 
 class Prefixes(BaseModel):
     prefixes: Dict[str, Namespace] = PREFIXES
 
     @staticmethod
     def create_from_dataframe(raw_dfs: pd.DataFrame) -> dict[str, Namespace]:
@@ -357,125 +533,116 @@
                 parse_rule(rule.rule, RuleType.rawlookup).table.name
                 for rule in self.properties.values()
                 if rule.is_raw_lookup
             }
         )
 
     @validator("properties", each_item=True)
-    def is_valid_mapping(cls, value, values):
+    def class_property_exist(cls, value, values):
         if classes := values.get("classes"):
-            if value.class_name not in classes:
-                raise ValueError(f"invalid mapping rule, {value.class_name} does not exist ")
+            if value.class_id not in classes:
+                raise ValueError(f"Property <{value.property_id}> defined for non-existing class <{value.class_id}>!")
         return value
 
     @validator("properties", each_item=True)
     def value_type_exist(cls, value, values):
         if classes := values.get("classes"):
             if value.property_type == "ObjectProperty" and value.expected_value_type not in classes:
-                msg = f"Property <{value.property_name}> defined for class <{value.class_name}> has "
+                msg = f"Property <{value.property_id}> defined for class <{value.class_id}> has "
                 msg += f"value type <{value.expected_value_type}> which is not defined!"
                 raise ValueError(msg)
         return value
 
     @validator("properties", each_item=True)
     def add_missing_label(cls, value):
         "Add label if missing for relationships"
         if value.label is None and "Relationship" in value.cdf_resource_type:
-            value.label = value.property_name
+            value.label = value.property_id
         return value
 
     @validator("properties")
     def is_type_defined_as_object(cls, value):
         "Checks if property expected value type is defined as object"
-        defined_objects = {property_.class_name for property_ in value.values()}
+        defined_objects = {property_.class_id for property_ in value.values()}
 
         if undefined_objects := [
             id
             for id, property_ in value.items()
             if property_.property_type == "ObjectProperty" and property_.expected_value_type not in defined_objects
         ]:
             msg = [
                 f"\nProperty at {id} has type <{value[id].expected_value_type}> for which mapping is not defined!"
                 for id in undefined_objects
             ]
             raise ValueError("".join(msg))
         return value
 
-    @validator("properties", each_item=True)
-    def class_property_exist(cls, value, values):
-        if classes := values.get("classes"):
-            if value.class_name not in classes:
-                raise ValueError(
-                    f"Property <{value.property_name}> defined for non-existing class <{value.class_name}>!"
-                )
-        return value
-
     @validator("prefixes")
     def add_data_model_prefix_namespace(cls, value, values):
         value[values["metadata"].prefix] = values["metadata"].namespace
         return value
 
     def get_labels(self) -> set[str]:
         """Return CDF labels for classes and relationships."""
-        class_labels = {class_.class_name for class_ in self.classes.values()}
+        class_labels = {class_.class_id for class_ in self.classes.values()}
 
-        property_labels = {property_.property_name for property_ in self.properties.values()}
+        property_labels = {property_.property_id for property_ in self.properties.values()}
 
         relationship_labels = {
             rule.label for rule in self.properties.values() if "Relationship" in rule.cdf_resource_type
         }
 
         return class_labels.union(relationship_labels).union(property_labels)
 
     def get_defined_classes(self) -> set[str]:
         """Returns classes that have been defined in the data model."""
-        return {property.class_name for property in self.properties.values()}
+        return {property.class_id for property in self.properties.values()}
 
     def get_classes_with_properties(self) -> dict[str, list[Property]]:
         """Returns classes that have been defined in the data model."""
         # TODO: Do not particularly like method name, find something more suitable
         class_property_pairs = {}
 
         for property_ in self.properties.values():
-            class_ = property_.class_name
+            class_ = property_.class_id
             if class_ in class_property_pairs:
                 class_property_pairs[class_] += [property_]
             else:
                 class_property_pairs[class_] = [property_]
 
         return class_property_pairs
 
     def get_class_property_pairs(self) -> dict[str, dict[str, Property]]:
         """This method will actually consider only the first definition of given property!"""
         class_property_pairs = {}
 
         for class_, properties in self.get_classes_with_properties().items():
             processed_properties = {}
             for property_ in properties:
-                if property_.property_name in processed_properties:
+                if property_.property_id in processed_properties:
                     warnings.warn(
                         "Property has been defined more than once! Only first definition will be considered.",
                         stacklevel=2,
                     )
                     continue
-                processed_properties[property_.property_name] = property_
+                processed_properties[property_.property_id] = property_
             class_property_pairs[class_] = processed_properties
 
         return class_property_pairs
 
     def check_data_model_definitions(self):
         """Check if data model definitions are valid."""
         issues = set()
         for class_, properties in self.get_classes_with_properties().items():
             analyzed_properties = []
-            for property in properties:
-                if property.property_name not in analyzed_properties:
-                    analyzed_properties.append(property.property_name)
+            for property_ in properties:
+                if property_.property_id not in analyzed_properties:
+                    analyzed_properties.append(property_.property_id)
                 else:
-                    issues.add(f"Property {property.property_name} of class {class_} has been defined more than once!")
+                    issues.add(f"Property {property_.property_id} of class {class_} has been defined more than once!")
         return issues
 
     def reduce_data_model(self, desired_classes: set, skip_validation: bool = False) -> TransformationRules:
         """Reduce the data model to only include desired classes and their properties.
 
         Parameters
         ----------
@@ -518,15 +685,15 @@
         }
 
         logging.info(f"Reducing data model to only include the following classes: {possible_classes}")
         for class_ in possible_classes:
             reduced_data_model["classes"][class_] = self.classes[class_]
 
         for id_, property_definition in self.properties.items():
-            if property_definition.class_name in possible_classes:
+            if property_definition.class_id in possible_classes:
                 reduced_data_model["properties"][id_] = property_definition
 
         if skip_validation:
             return TransformationRules.construct(**reduced_data_model)
         else:
             return TransformationRules(**reduced_data_model)
 
@@ -543,16 +710,16 @@
         data_model = {}
 
         defined_classes = self.get_classes_with_properties()
 
         for class_ in defined_classes:
             properties = {}
             for property_ in defined_classes[class_]:
-                if property_.property_name not in properties:
-                    properties[property_.property_name] = {
+                if property_.property_id not in properties:
+                    properties[property_.property_id] = {
                         "property_type": property_.property_type,
                         "value_type": property_.expected_value_type,
                         "min_count": property_.min_count,
                         "max_count": property_.max_count,
                     }
 
             data_model[class_] = pd.DataFrame(properties).T
@@ -563,17 +730,17 @@
         """Returns a dataframe with the class linkage of the data model."""
 
         class_linkage = pd.DataFrame(columns=["source_class", "target_class", "connecting_property", "max_occurrence"])
         for property_ in self.properties.values():
             if property_.property_type == "ObjectProperty":
                 new_row = pd.Series(
                     {
-                        "source_class": property_.class_name,
+                        "source_class": property_.class_id,
                         "target_class": property_.expected_value_type,
-                        "connecting_property": property_.property_name,
+                        "connecting_property": property_.property_id,
                         "max_occurrence": property_.max_count,
                     }
                 )
                 class_linkage = pd.concat([class_linkage, new_row.to_frame().T], ignore_index=True)
 
         class_linkage.drop_duplicates(inplace=True)
 
@@ -610,28 +777,28 @@
 
         # Unique ids used to check for redefinitions of relationships
         ids = set()
 
         for row, rule in self.properties.items():
             if "Relationship" in rule.cdf_resource_type:
                 relationship = RelationshipDefinition(
-                    source_class=rule.class_name,
+                    source_class=rule.class_id,
                     target_class=rule.expected_value_type,
-                    property_=rule.property_name,
+                    property_=rule.property_id,
                     labels=list(
-                        set([rule.label, rule.class_name, rule.expected_value_type, "non-historic", rule.property_name])
+                        set([rule.label, rule.class_id, rule.expected_value_type, "non-historic", rule.property_id])
                     ),
                     target_type=rule.target_type,
                     source_type=rule.source_type,
                     relationship_external_id_rule=rule.relationship_external_id_rule,
                 )
 
-                id_ = f"{rule.class_name}({rule.property_name})"
+                id_ = f"{rule.class_id}({rule.property_id})"
                 if id_ in ids:
-                    msg = f"Relationship {rule.property_name} redefined at {row} in transformation rules!"
+                    msg = f"Relationship {rule.property_id} redefined at {row} in transformation rules!"
                     if stop_on_exception:
                         logging.error(msg)
                         raise ValueError(msg)
                     else:
                         msg += " Skipping redefinition!"
                         warnings.warn(msg, stacklevel=2)
                         logging.warning(msg)
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.14.2/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.14.2/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     dict
         Dict containing keys as class names and list of their properties
     """
 
     classes = {}
 
     for property_ in transformation_rules.properties.keys():
-        class_ = transformation_rules.properties[property_].class_name
+        class_ = transformation_rules.properties[property_].class_id
 
         if class_ in classes:
             classes[class_] += [transformation_rules.properties[property_]]
         else:
             classes[class_] = [transformation_rules.properties[property_]]
 
     return classes
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.14.2/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     >>> repair_name("windSpeed", "class", True)
     'WindSpeed'
     >>> repair_name("22windSpeed", "class")
     '_22windSpeed'
     """
 
     # Remove any non GraphQL compliant characters
-    repaired_string = re.sub(r"[^_a-zA-Z0-9/_]", "", name)
+    repaired_string = re.sub(r"[^_a-zA-Z0-9]", "", name)
 
     # Name must start with a letter or underscore
     if repaired_string[0].isdigit():
         repaired_string = f"_{repaired_string}"
 
     if not fix_casing:
         return repaired_string
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/loader/config.py` & `cognite_neat-0.14.2/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/loader/graph.py` & `cognite_neat-0.14.2/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.14.2/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.14.2/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/loader/rules.py` & `cognite_neat-0.14.2/cognite/neat/core/loader/rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,22 @@
     client_google = gspread.service_account()
     spreadsheet = client_google.open_by_key(sheet_id)
     return {worksheet.title: pd.DataFrame(worksheet.get_all_records()) for worksheet in spreadsheet.worksheets()}
 
 
 def excel_file_to_table_by_name(filepath: Path) -> dict[str, pd.DataFrame]:
     workbook: Workbook = load_workbook(filepath)
-    return {
+
+    sheets = {
         sheetname: pd.read_excel(
             filepath,
             sheet_name=sheetname,
             header=None if sheetname == "Metadata" else 0,
             skiprows=1 if sheetname in ["Classes", "Properties", "Instances"] else None,
         )
         for sheetname in workbook.sheetnames
     }
+
+    for sheetname in sheets:
+        sheets[sheetname].source = filepath
+
+    return sheets
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.14.2/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/modeler.py` & `cognite_neat-0.14.2/cognite/neat/core/modeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # TODO: Add support for deprecated, replaced_by, similar_to, equal_to
     properties = {}
 
     for property_ in data_model_definition.properties.values():
         if property_.property_name != "*":
             if property_.property_name not in properties:
                 properties[property_.property_name] = {
-                    "domain": {data_model_definition.namespace[property_.class_name]},
+                    "domain": {data_model_definition.namespace[property_.class_id]},
                     "range": {
                         data_model_definition.namespace[property_.expected_value_type]
                         if property_.property_type == "ObjectProperty"
                         else XSD[property_.expected_value_type]
                     },
                     "property_type": {
                         OWL[property_.property_type],
@@ -43,15 +43,15 @@
                     "description": {property_.description or None},
                     # "equal_to": {property_.equal_to or None},
                     # "similar_to": {property_.similar_to or None},
                     # "replaced_by": {property_.replaced_by or None},
                     # "deprecated": {property_.deprecated or None},
                 }
             else:
-                properties[property_.property_name]["domain"].add(data_model_definition.namespace[property_.class_name])
+                properties[property_.property_name]["domain"].add(data_model_definition.namespace[property_.class_id])
                 properties[property_.property_name]["range"].add(
                     data_model_definition.namespace[property_.expected_value_type]
                     if property_.property_type == "ObjectProperty"
                     else XSD[property_.expected_value_type]
                 )
                 properties[property_.property_name]["property_type"].add(OWL[property_.property_type])
                 properties[property_.property_name]["description"].add(property_.description or None)
@@ -210,57 +210,57 @@
         Ontology graph
     data_model_definition : DataModelingDefinition
         Instance of DataModelingDefinition class
     class_ : Class
         Class to be added to ontology graph
     """
     # TODO: Simplify by only providing namespace instead of data_model_definition
-    ontology_graph.add((data_model_definition.namespace[class_.class_name], RDF.type, OWL.Class))
-    ontology_graph.add((data_model_definition.namespace[class_.class_name], RDFS.subClassOf, OWL.Thing))
+    ontology_graph.add((data_model_definition.namespace[class_.class_id], RDF.type, OWL.Class))
+    ontology_graph.add((data_model_definition.namespace[class_.class_id], RDFS.subClassOf, OWL.Thing))
 
     # add datatype recognition
-    ontology_graph.add((data_model_definition.namespace[class_.class_name], RDFS.label, Literal(class_.class_name)))
+    ontology_graph.add((data_model_definition.namespace[class_.class_id], RDFS.label, Literal(class_.class_id)))
 
     if class_.description:
         ontology_graph.add(
-            (data_model_definition.namespace[class_.class_name], RDFS.comment, Literal(class_.description))
+            (data_model_definition.namespace[class_.class_id], RDFS.comment, Literal(class_.description))
         )
 
     if class_.parent_class:
         ontology_graph.add(
             (
-                data_model_definition.namespace[class_.class_name],
+                data_model_definition.namespace[class_.class_id],
                 RDFS.subClassOf,
                 data_model_definition.namespace[class_.parent_class],
             )
         )
 
     if class_.deprecated:
         ontology_graph.add(
             (
-                data_model_definition.namespace[class_.class_name],
+                data_model_definition.namespace[class_.class_id],
                 OWL.deprecated,
                 Literal(class_.deprecated, datatype=XSD.boolean),
             )
         )
 
     if class_.replaced_by:
         ontology_graph.add(
             (
-                data_model_definition.namespace[class_.class_name],
+                data_model_definition.namespace[class_.class_id],
                 DCTERMS.isReplacedBy,
                 data_model_definition.namespace[class_.replaced_by],
             )
         )
 
     if class_.similar_to:
-        ontology_graph.add((data_model_definition.namespace[class_.class_name], SKOS.exactMatch, class_.similar_to))
+        ontology_graph.add((data_model_definition.namespace[class_.class_id], SKOS.exactMatch, class_.similar_to))
 
     if class_.equal_to:
-        ontology_graph.add((data_model_definition.namespace[class_.class_name], OWL.equivalentClass, class_.equal_to))
+        ontology_graph.add((data_model_definition.namespace[class_.class_id], OWL.equivalentClass, class_.equal_to))
 
 
 def data_model_definition2owl(
     data_model_definition: DataModelingDefinition,
     prefixes: dict[str, Namespace] = PREFIXES,
     owl_graph: Graph = None,
 ) -> Graph:
@@ -317,33 +317,33 @@
         for prefix, namespace in prefixes.items():
             shacl_graph.bind(prefix, namespace)
 
     node_shapes = {}
     for shacl_constraint in data_model_definition.properties.values():
         property_name = shacl_constraint.property_name
         if property_name != "*":
-            class_name = shacl_constraint.class_name
-            node_shape_name = f"{class_name}Shape"
+            class_id = shacl_constraint.class_id
+            node_shape_name = f"{class_id}Shape"
 
             # adds node shape to shacl graph
             if node_shape_name not in node_shapes:
                 node_shapes[node_shape_name] = {}
                 shacl_graph.add((data_model_definition.namespace[node_shape_name], RDF.type, SHACL.NodeShape))
                 shacl_graph.add(
                     (
                         data_model_definition.namespace[node_shape_name],
                         RDFS.comment,
-                        Literal(data_model_definition.classes[class_name].description),
+                        Literal(data_model_definition.classes[class_id].description),
                     )
                 )
                 shacl_graph.add(
                     (
                         data_model_definition.namespace[node_shape_name],
                         SHACL.targetClass,
-                        data_model_definition.namespace[class_name],
+                        data_model_definition.namespace[class_id],
                     )
                 )
 
             # adds property shape to shacl graph
             property_shape_node = BNode()
             shacl_graph.add((data_model_definition.namespace[node_shape_name], SHACL.property, property_shape_node))
             shacl_graph.add((property_shape_node, SHACL.path, data_model_definition.namespace[property_name]))
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.14.2/cognite/neat/core/parser/transformation_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 import pandas as pd
 
 from cognite.neat.core.configuration import Tables
 from cognite.neat.core.data_classes import Instance, Metadata, Prefixes, TransformationRules
 
 
-def parse_transformation_rules(raw_dfs: dict[str, pd.DataFrame]) -> TransformationRules:
+def parse_transformation_rules(
+    raw_dfs: dict[str, pd.DataFrame], allow_validation_errors: bool = False
+) -> TransformationRules:
     metadata = Metadata.create_from_dataframe(raw_dfs)
     prefixes = Prefixes.create_from_dataframe(raw_dfs[Tables.prefixes])
     instances = parse_instances(raw_dfs, metadata, prefixes) if Tables.instances in raw_dfs else None
 
-    return TransformationRules(
-        prefixes=prefixes,
-        metadata=metadata,
-        classes={class_.get("Class"): class_ for class_ in raw_dfs[Tables.classes].to_dict(orient="records")},
-        properties={
-            f"row {i+3}": property_ for i, property_ in enumerate(raw_dfs[Tables.properties].to_dict(orient="records"))
-        },
-        instances=instances,
-    )
+    if not allow_validation_errors:
+        return TransformationRules(
+            prefixes=prefixes,
+            metadata=metadata,
+            classes={class_.get("Class"): class_ for class_ in raw_dfs[Tables.classes].to_dict(orient="records")},
+            properties={
+                f"row {i+3}": property_
+                for i, property_ in enumerate(raw_dfs[Tables.properties].to_dict(orient="records"))
+            },
+            instances=instances,
+        )
+    else:
+        raise NotImplementedError("Allowing validation errors is not yet implemented!")
 
 
 def parse_instances(raw_dfs: dict[str, pd.DataFrame], metadata: Metadata, prefixes: Prefixes) -> list[tuple]:
     expected_tables = Tables.as_set()
     if missing_tables := (expected_tables - set(raw_dfs)):
         raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.14.2/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/transformer.py` & `cognite_neat-0.14.2/cognite/neat/core/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,20 +151,20 @@
             logging.info(f" {COMMIT_BATCH_SIZE} nodes committed")
             commit_counter = 0
 
     proc_start_time = time.perf_counter()
     for sheet_row, rule_definition in transformation_rules.properties.items():
         if not rule_definition.rule or rule_definition.skip_rule:
             continue
-        msg = f"Processing {sheet_row}: class <{rule_definition.class_name}> "
+        msg = f"Processing {sheet_row}: class <{rule_definition.class_id}> "
         msg += f"property <{rule_definition.property_name}> rule <{rule_definition.rule}>"
 
         processing_report_rec = RuleProcessingReportRec(
             row_id=sheet_row,
-            rule_name=f"{rule_definition.class_name}_{rule_definition.property_name}",
+            rule_name=f"{rule_definition.class_id}_{rule_definition.property_name}",
             rule_type=rule_definition.rule_type,
             rule_expression=rule_definition.rule,
         )
         logging.info(msg)
         try:
             start_time = time.perf_counter()
             # Parse rule:
@@ -176,15 +176,15 @@
             else:
                 query = build_sparql_query(domain_knowledge_graph, rule.traversal, transformation_rules.prefixes)
 
             logging.info(f"Query: {query}")
 
             if query_results := list(domain_knowledge_graph.query(query)):
                 # Generate URI for class and property in target namespace
-                class_URI = transformation_rules.metadata.namespace[rule_definition.class_name]
+                class_URI = transformation_rules.metadata.namespace[rule_definition.class_id]
                 property_URI = transformation_rules.metadata.namespace[rule_definition.property_name]
 
                 # Turn query results into dataframe
                 instance_df = pd.DataFrame(query_results, columns=list(Triple))
 
                 # If we are not grabbing all properties for class instances
                 # then we are able to replace source property URI with target property URI
@@ -245,15 +245,15 @@
             failed += 1
             elapsed_time = time.perf_counter() - start_time
             processing_report_rec.elapsed_time = elapsed_time
             processing_report_rec.status = "failed"
             processing_report_rec.error_message = str(e)
             prom_total_proc_rules_g.labels(state="failed").inc()
             logging.error(
-                f" Error while processing rule {rule_definition.rule} for class {rule_definition.class_name} \
+                f" Error while processing rule {rule_definition.rule} for class {rule_definition.class_id} \
                 and property {rule_definition.property_name}"
             )
             logging.error(traceback.format_exc())
             if stop_on_exception:
                 raise e
 
         if processing_report:
```

### Comparing `cognite_neat-0.14.1/cognite/neat/core/utils.py` & `cognite_neat-0.14.2/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/validator.py` & `cognite_neat-0.14.2/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/base.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/model.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.14.2/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.14.2/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.14.2/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.14.2/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.14.2/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer/explorer.py` & `cognite_neat-0.14.2/cognite/neat/explorer/explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,29 +165,29 @@
     error_text = ""
     properties = []
     classes = []
     try:
         rules = parser.parse_transformation_rules(tables)
         properties = [
             {
-                "class": value.class_name,
-                "property": value.property_name,
+                "class": value.class_id,
+                "property": value.property_id,
                 "property_description": value.description,
                 "property_type": value.expected_value_type,
                 "cdf_resource_type": value.cdf_resource_type,
                 "cdf_metadata_type": value.resource_type_property,
                 "rule_type": value.rule_type,
                 "rule": value.rule,
             }
             for value in rules.properties.values()
         ]
 
         classes = [
             {
-                "class": value.class_name,
+                "class": value.class_id,
                 "class_description": value.description,
                 "cdf_resource_type": value.cdf_resource_type,
                 "cdf_parent_resource": value.parent_asset,
             }
             for value in rules.classes.values()
         ]
     except Exception as e:
```

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.14.2/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.14.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.14.2/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.14.1/pyproject.toml` & `cognite_neat-0.14.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.14.1"
+version = "0.14.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
```

### Comparing `cognite_neat-0.14.1/PKG-INFO` & `cognite_neat-0.14.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.14.1
+Version: 0.14.2
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

