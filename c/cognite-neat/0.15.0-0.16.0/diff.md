# Comparing `tmp/cognite_neat-0.15.0.tar.gz` & `tmp/cognite_neat-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.15.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.16.0.tar", max compression
```

## Comparing `cognite_neat-0.15.0.tar` & `cognite_neat-0.16.0.tar`

### file list

```diff
@@ -1,98 +1,103 @@
--rw-r--r--   0        0        0    11351 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/LICENSE
--rw-r--r--   0        0        0     8765 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/README.md
--rw-r--r--   0        0        0       23 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0     9922 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/graph2assets_relationships.py
--rw-r--r--   0        0        0     7016 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/graphs_and_rules.py
--rw-r--r--   0        0        0    14129 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/sheet2cdf.py
--rw-r--r--   0        0        0    11867 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/base_workflows/sme_graph_capture.py
--rw-r--r--   0        0        0      761 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2792 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1400 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     5073 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8228 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    38635 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    39837 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    18682 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6698 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    11439 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0     1009 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15269 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1958 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11906 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     8743 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-07-08 16:11:35.912624 cognite_neat-0.15.0/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    20765 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0    11636 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4882 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      775 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6977 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79716 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-07-08 16:11:35.916624 cognite_neat-0.15.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15613 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0      315 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8063 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0      270 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0      291 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1390 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    24055 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4578 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-07-08 16:11:35.920624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1370103 2023-07-08 16:11:35.928624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
--rw-r--r--   0        0        0     2667 2023-07-08 16:11:35.928624 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
--rw-r--r--   0        0        0  5883237 2023-07-08 16:11:35.960625 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
--rw-r--r--   0        0        0     2633 2023-07-08 16:11:35.960625 cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-08 16:11:35.964625 cognite_neat-0.15.0/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2579 2023-07-08 16:11:36.428626 cognite_neat-0.15.0/pyproject.toml
--rw-r--r--   0        0        0    10442 1970-01-01 00:00:00.000000 cognite_neat-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-10 10:32:40.430806 cognite_neat-0.16.0/LICENSE
+-rw-r--r--   0        0        0     8765 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/README.md
+-rw-r--r--   0        0        0       61 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/_version.py
+-rw-r--r--   0        0        0     9946 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/base_workflows/graph2assets_relationships.py
+-rw-r--r--   0        0        0     6927 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/base_workflows/graphs_and_rules.py
+-rw-r--r--   0        0        0    14165 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/base_workflows/sheet2cdf.py
+-rw-r--r--   0        0        0    11808 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/base_workflows/sme_graph_capture.py
+-rw-r--r--   0        0        0      761 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     5574 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      758 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/exceptions.py
+-rw-r--r--   0        0        0      772 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/__init__.py
+-rw-r--r--   0        0        0     2229 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/labels.py
+-rw-r--r--   0        0        0     5048 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/models.py
+-rw-r--r--   0        0        0    39829 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py
+-rw-r--r--   0        0        0    20940 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5428 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     5379 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6677 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      122 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    11390 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10358 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15241 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0       73 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9594 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0     1270 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/rules/__init__.py
+-rw-r--r--   0        0        0     1683 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/rules/_loader.py
+-rw-r--r--   0        0        0     2914 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/rules/_parser.py
+-rw-r--r--   0        0        0    30685 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/rules/models.py
+-rw-r--r--   0        0        0     8228 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/rules/to_rdf_path.py
+-rw-r--r--   0        0        0    11890 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/utils/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/utils/auxiliary.py
+-rw-r--r--   0        0        0      689 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/utils/cdf.py
+-rw-r--r--   0        0        0     8733 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/utils/utils.py
+-rw-r--r--   0        0        0     2559 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    20772 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0    11636 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4882 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      775 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6977 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-07-10 10:32:40.434806 cognite_neat-0.16.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79716 2023-07-10 10:32:40.438806 cognite_neat-0.16.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-07-10 10:32:40.438806 cognite_neat-0.16.0/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-07-10 10:32:40.438806 cognite_neat-0.16.0/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-07-10 10:32:40.438806 cognite_neat-0.16.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-07-10 10:32:40.438806 cognite_neat-0.16.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15548 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3533 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11456 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0      315 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8063 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0      270 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0      291 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1390 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    24029 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4578 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-07-10 10:32:40.442806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1370103 2023-07-10 10:32:40.450806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js
+-rw-r--r--   0        0        0     2667 2023-07-10 10:32:40.450806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt
+-rw-r--r--   0        0        0  5883237 2023-07-10 10:32:40.478805 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map
+-rw-r--r--   0        0        0     2633 2023-07-10 10:32:40.482806 cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-10 10:32:40.486806 cognite_neat-0.16.0/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2858 2023-07-10 10:32:40.950804 cognite_neat-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0    10658 1970-01-01 00:00:00.000000 cognite_neat-0.16.0/PKG-INFO
```

### Comparing `cognite_neat-0.15.0/LICENSE` & `cognite_neat-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/README.md` & `cognite_neat-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/base_workflows/graph2assets_relationships.py` & `cognite_neat-0.16.0/cognite/neat/base_workflows/graph2assets_relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import time
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
 from cognite.neat.base_workflows.graphs_and_rules import GraphsAndRulesBaseWorkflow
-from cognite.neat.core.extractors.labels import upload_labels
-from cognite.neat.core.extractors.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.rdf_to_relationships import (
+from cognite.neat.core.extractors.cdfcore.labels import upload_labels
+from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.core.validator import validate_asset_hierarchy
 from cognite.neat.core.workflow.model import FlowMessage
```

### Comparing `cognite_neat-0.15.0/cognite/neat/base_workflows/graphs_and_rules.py` & `cognite_neat-0.16.0/cognite/neat/base_workflows/graphs_and_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
-from cognite.neat.core import loader, parser
+from cognite.neat.core import loader, rules
 from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.loader.graph_store import NeatGraphStore, drop_graph_store
+from cognite.neat.core.rules.models import TransformationRules
 from cognite.neat.core.transformer import RuleProcessingReport, domain2app_knowledge_graph
 from cognite.neat.core.workflow import utils
 from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
 from cognite.neat.core.workflow.cdf_store import CdfStore
 
 
 class GraphsAndRulesBaseWorkflow(BaseWorkflow):
@@ -35,16 +35,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
-        tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
-        self.transformation_rules = parser.parse_transformation_rules(tables)
+        self.transformation_rules = rules.load_rules_from_excel_file(rules_file_path)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules from {rules_file_path.name!r}.")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
```

### Comparing `cognite_neat-0.15.0/cognite/neat/base_workflows/sheet2cdf.py` & `cognite_neat-0.16.0/cognite/neat/base_workflows/sheet2cdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.core import loader, parser
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
-from cognite.neat.core.extractors.labels import upload_labels
-from cognite.neat.core.extractors.rdf_to_assets import (
+from cognite.neat.core import loader, rules
+from cognite.neat.core.extractors.cdfcore.labels import upload_labels
+from cognite.neat.core.extractors.cdfcore.rdf_to_assets import (
     NeatMetadataKeys,
     categorize_assets,
     rdf2assets,
     remove_non_existing_labels,
     unique_asset_labels,
     upload_assets,
 )
-from cognite.neat.core.extractors.rdf_to_relationships import (
+from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.core.loader.graph_store import NeatGraphStore
+from cognite.neat.core.rules.models import TransformationRules
 from cognite.neat.core.validator import validate_asset_hierarchy
 from cognite.neat.core.workflow import utils
 from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
 from cognite.neat.core.workflow.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
     prom_cdf_resource_stats = Gauge(
@@ -67,16 +67,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, rules_file, version)
 
-        self.raw_tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
-        self.transformation_rules = parser.parse_transformation_rules(self.raw_tables)
+        self.transformation_rules = rules.load_rules_from_excel_file(rules_file_path)
 
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules from {rules_file_path.name!r}."
         logging.info(output_text)
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
 
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         return FlowMessage(output_text=output_text)
@@ -98,15 +97,16 @@
         # total number of rows in the sheet that have been processed by the workflow
         # and report back reasons why
 
         self.triples = self.transformation_rules.instances
         self.instance_ids = {triple[0] for triple in self.triples}
 
         output_text = f"Loaded {len(self.instance_ids)} instances out of"
-        output_text += f" {len(self.raw_tables['Instances'])} rows in Instances sheet"
+        # Todo: This is no longer exposed in the rules package. Need to extend the load methods to return a rapport.
+        # output_text += f" {len(self.raw_tables['Instances'])} rows in Instances sheet"
 
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_load_instances_to_source_graph(self, flow_msg: FlowMessage = None):
         # Load parsed instances to source graph
```

### Comparing `cognite_neat-0.15.0/cognite/neat/base_workflows/sme_graph_capture.py` & `cognite_neat-0.16.0/cognite/neat/base_workflows/sme_graph_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 
-from cognite.neat.core import extractors, loader, parser
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
-from cognite.neat.core.extractors.labels import upload_labels
-from cognite.neat.core.extractors.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.rdf_to_relationships import (
+from cognite.neat.core import extractors, loader, rules
+from cognite.neat.core.extractors.cdfcore.labels import upload_labels
+from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils import add_triples
+from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.core.utils.utils import add_triples
 from cognite.neat.core.validator import validate_asset_hierarchy
 from cognite.neat.core.workflow import utils
 from cognite.neat.core.workflow.base import BaseWorkflow
 from cognite.neat.core.workflow.cdf_store import CdfStore
 from cognite.neat.core.workflow.model import FlowMessage
 
 
@@ -59,16 +59,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
-        tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
-        self.transformation_rules = parser.parse_transformation_rules(tables)
+        self.transformation_rules = rules.load_rules_from_excel_file(rules_file_path)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configure_graph_store(self, flow_msg: FlowMessage = None):
```

### Comparing `cognite_neat-0.15.0/cognite/neat/constants.py` & `cognite_neat-0.16.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/app.py` & `cognite_neat-0.16.0/cognite/neat/core/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from cognite.client import CogniteClient
 from fastapi import FastAPI
 
-from cognite.neat.core.data_classes.config import Config
-from cognite.neat.core.utils import get_cognite_client_from_config
+from cognite.neat.core.configuration import Config
+from cognite.neat.core.utils.utils import get_cognite_client_from_config
 from cognite.neat.core.workflow.cdf_store import CdfStore
 from cognite.neat.core.workflow.manager import WorkflowManager
 from cognite.neat.core.workflow.triggers import TriggerManager
 
 
 class NeatApp:
     def __init__(self, config: Config, cdf_client: CogniteClient = None):
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.16.0/cognite/neat/core/rules/to_rdf_path.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.16.0/cognite/neat/core/rules/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 import logging
 import math
 import re
 import warnings
 from datetime import datetime
 from pathlib import Path
-from typing import ClassVar, Dict, List, Optional, Self
+from typing import ClassVar, Dict, List, Optional
 
 import pandas as pd
 from graphql import GraphQLBoolean, GraphQLFloat, GraphQLInt, GraphQLString
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     HttpUrl,
     ValidationError,
     constr,
     field_validator,
     model_validator,
     parse_obj_as,
-    root_validator,
     validator,
 )
 from pydantic.fields import FieldInfo
 from rdflib import XSD, Literal, Namespace, URIRef
 
-from cognite.neat.core.configuration import PREFIXES, Tables
-from cognite.neat.core.data_classes.rules import Entity, RuleType, parse_rule
+from cognite.neat.core.configuration import PREFIXES
+
+from .to_rdf_path import Entity, RuleType, parse_rule
+
+__all__ = ["Class", "Instance", "Metadata", "Prefixes", "Property", "Resource", "TransformationRules"]
 
 # mapping of XSD types to Python and GraphQL types
 DATA_TYPE_MAPPING = {
     "boolean": {"python": "bool", "GraphQL": GraphQLBoolean},
     "float": {"python": "float", "GraphQL": GraphQLFloat},
     "integer": {"python": "int", "GraphQL": GraphQLInt},
     "nonPositiveInteger": {"python": "int", "GraphQL": GraphQLInt},
@@ -406,43 +408,18 @@
         if isinstance(value, str):
             if value:
                 return value.replace(", ", ",").split(",")
             if cls.model_fields[info.field_name].default is None:
                 return None
         return value
 
-    @classmethod
-    def create_from_dataframe(cls, raw_dfs) -> Self:
-        expected_tables = Tables.as_set()
-        if missing_tables := (expected_tables - set(raw_dfs)):
-            raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
-
-        return Metadata(
-            **dict(zip(raw_dfs[Tables.metadata][0], raw_dfs[Tables.metadata][1])),
-            source=raw_dfs[Tables.metadata].source if "source" in dir(raw_dfs[Tables.metadata]) else None,
-        )
-
 
 class Prefixes(RuleModel):
     prefixes: Dict[str, Namespace] = PREFIXES
 
-    @staticmethod
-    def create_from_dataframe(raw_dfs: pd.DataFrame) -> dict[str, Namespace]:
-        prefixes = {}
-        for i, row in raw_dfs.iterrows():
-            try:
-                url = URL(url=row["URI"]).url
-                prefixes[row["Prefix"]] = Namespace(url)
-            except ValueError as e:
-                msg = f"Prefix <{row['Prefix']}> has invalid URL: <{row['URI']}> fix this in Prefixes sheet at the row {i + 2} in the rule file!"
-                logging.error(msg)
-                raise ValueError(msg) from e
-
-        return prefixes
-
 
 class Instance(RuleModel):
     """Class deals with instances of classes in the data model"""
 
     instance: Optional[URIRef] = Field(alias="Instance", default=None)
     property_: Optional[URIRef] = Field(alias="Property", default=None)
     value: Optional[Literal | URIRef] = Field(alias="Value", default=None)
@@ -774,193 +751,14 @@
             source = row.source_class
             target = row.target_class
             target_targets = class_linkage[class_linkage.source_class == target].target_class.values
             if source in target_targets and (source, target) not in sym_pairs:
                 sym_pairs.add((source, target))
         return sym_pairs
 
-    def define_relationships(self, stop_on_exception: bool = False) -> RelationshipDefinitions:
-        relationships = {}
-
-        # Unique ids used to check for redefinitions of relationships
-        ids = set()
-
-        for row, rule in self.properties.items():
-            if "Relationship" in rule.cdf_resource_type:
-                relationship = RelationshipDefinition(
-                    source_class=rule.class_id,
-                    target_class=rule.expected_value_type,
-                    property_=rule.property_id,
-                    labels=list(
-                        set([rule.label, rule.class_id, rule.expected_value_type, "non-historic", rule.property_id])
-                    ),
-                    target_type=rule.target_type,
-                    source_type=rule.source_type,
-                    relationship_external_id_rule=rule.relationship_external_id_rule,
-                )
-
-                id_ = f"{rule.class_id}({rule.property_id})"
-                if id_ in ids:
-                    msg = f"Relationship {rule.property_id} redefined at {row} in transformation rules!"
-                    if stop_on_exception:
-                        logging.error(msg)
-                        raise ValueError(msg)
-                    else:
-                        msg += " Skipping redefinition!"
-                        warnings.warn(msg, stacklevel=2)
-                        logging.warning(msg)
-                else:
-                    relationships[row] = relationship
-                    ids.add(id_)
-
-        if relationships:
-            return RelationshipDefinitions(
-                data_set_id=self.metadata.data_set_id,
-                prefix=self.metadata.prefix,
-                namespace=self.metadata.namespace,
-                relationships=relationships,
-            )
-
-        msg = "No relationship defined in transformation rule sheet!"
-        if stop_on_exception:
-            logging.error(msg)
-            raise ValueError(msg)
-        else:
-            warnings.warn(msg, stacklevel=2)
-            logging.warning(msg)
-            return RelationshipDefinitions(
-                data_set_id=self.metadata.data_set_id,
-                prefix=self.metadata.prefix,
-                namespace=self.metadata.namespace,
-                relationships={},
-            )
-
     def get_entity_names(self):
         class_names = set()
         property_names = set()
         for class_, properties in self.to_dataframe().items():
             class_names.add(class_)
             property_names = property_names.union(set(properties.index))
         return class_names.union(property_names)
-
-
-class AssetClassMapping(BaseModel):
-    external_id: str
-    name: str
-    parent_external_id: Optional[str] = None
-    description: Optional[str] = None
-    metadata: Optional[dict] = {}
-
-    @root_validator(pre=True)
-    def create_metadata(cls, values: dict):
-        fields = values.keys()
-
-        # adding metadata key in case if it is missing
-        values["metadata"] = {} if "metadata" not in values else values["metadata"]
-
-        for field in fields:
-            if field not in ["external_id", "name", "parent_external_id", "data_set_id", "metadata", "description"]:
-                values["metadata"][field] = ""
-        return values
-
-
-class AssetTemplate(BaseModel):
-    """This class is used to validate, repair and wrangle rdf asset dictionary according to the
-    expected format of cognite sdk Asset dataclass."""
-
-    external_id_prefix: Optional[str] = None  # convenience field to add prefix to external_ids
-    external_id: str
-    name: Optional[str] = None
-    parent_external_id: Optional[str] = None
-    metadata: Optional[dict] = {}
-    description: Optional[str] = None
-    data_set_id: Optional[int] = None
-
-    @root_validator(pre=True)
-    def preprocess_fields(cls, values: dict):
-        fields = values.keys()
-
-        # Adding metadata key in case if it is missing
-        values["metadata"] = {} if "metadata" not in values else values["metadata"]
-
-        for field in fields:
-            # Enrich: adding any field that is not in the list of expected fields to metadata
-            if field not in [
-                "external_id",
-                "name",
-                "parent_external_id",
-                "data_set_id",
-                "metadata",
-                "description",
-                "external_id_prefix",
-            ]:
-                values["metadata"][field] = values[field]
-
-            # Repair: in case if name/description is list instead of single value list elements are joined
-            elif field in ["name", "description"] and isinstance(values[field], list):
-                msg = f"{values['type']} instance {values['identifier']} property {field} "
-                msg += f"has multiple values {values[field]}, "
-                msg += f"these values will be joined in a single string: {', '.join(values[field])}"
-                logging.info(msg)
-                values[field] = ", ".join(values[field])[: METADATA_VALUE_MAX_LENGTH - 1]
-
-            # Repair: in case if external_id or parent_external_id are lists, we take the first value
-            elif field in ["external_id", "parent_external_id"] and isinstance(values[field], list):
-                msg = f"{values['type']} instance {values['identifier']} property {field} "
-                msg += f"has multiple values {values[field]}, "
-                msg += f"only the first one will be used: {values[field][0]}"
-                logging.info(msg)
-                values[field] = values[field][0]
-
-        # Setting asset to be by default active
-        values["metadata"]["active"] = "true"
-
-        # Handling case when the external_id is not provided by defaulting to the original identifier
-        # The original identifier probably has its namespace removed
-        if "external_id" not in fields and "identifier" in fields:
-            values["external_id"] = values["identifier"]
-
-        return values
-
-    @validator("metadata")
-    def to_list_if_comma(cls, value):
-        for key, v in value.items():
-            if isinstance(v, list):
-                value[key] = ", ".join(v)[: METADATA_VALUE_MAX_LENGTH - 1]
-        return value
-
-    @validator("metadata")
-    def to_str(cls, value):
-        for key, v in value.items():
-            value[key] = str(v)
-        return value
-
-    @validator("external_id", always=True)
-    def add_prefix_to_external_id(cls, value, values):
-        if values["external_id_prefix"]:
-            return values["external_id_prefix"] + value
-        else:
-            return value
-
-    @validator("parent_external_id")
-    def add_prefix_to_parent_external_id(cls, value, values):
-        if values["external_id_prefix"]:
-            return values["external_id_prefix"] + value
-        else:
-            return value
-
-
-class RelationshipDefinition(BaseModel):
-    source_class: str
-    target_class: str
-    property_: str
-    labels: Optional[List[str]] = None
-    target_type: str = "Asset"
-    source_type: str = "Asset"
-    relationship_external_id_rule: Optional[str] = None
-
-
-class RelationshipDefinitions(RuleModel):
-    data_set_id: int
-    prefix: str
-    namespace: Namespace
-    relationships: dict[str, RelationshipDefinition]
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.16.0/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.16.0/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import warnings
 
 import pandas as pd
 from rdflib import RDF, XSD, Literal, Namespace
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
+from cognite.neat.core.rules.models import TransformationRules
 
 
 def sheet2triples(
     graph_capturing_sheet: dict[str, pd.DataFrame],
     transformation_rule: TransformationRules,
     separator: str = ",",
     namespace: str = None,
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import traceback
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelDefinition
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
+from cognite.neat.core.rules.models import TransformationRules
 
 
 def upload_labels(
     client: CogniteClient,
     transformation_rules: TransformationRules,
     extra_labels: list = None,
     stop_on_exception: bool = False,
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/rdf_to_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
 from cognite.client.exceptions import CogniteDuplicatedError
 from deepdiff import DeepDiff
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
-from cognite.neat.core.data_classes import AssetTemplate, Property
-from cognite.neat.core.data_classes.config import EXCLUDE_PATHS
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
+from cognite.neat.core.configuration import EXCLUDE_PATHS
+from cognite.neat.core.extractors.cdfcore.models import AssetTemplate
 from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
+from cognite.neat.core.rules.models import Property, TransformationRules
+from cognite.neat.core.utils.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
 
 @dataclass
 class NeatMetadataKeys:
     start_time: str = "start_time"
     end_time: str = "end_time"
     update_time: str = "update_time"
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/cdfcore/rdf_to_relationships.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,84 @@
 import logging
+import warnings
 
 # import traceback
 from typing import Dict, List, Set, Union
 from warnings import warn
 
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelFilter, Relationship, RelationshipUpdate
 from cognite.client.exceptions import CogniteDuplicatedError
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
-from cognite.neat.core.extractors.rdf_to_assets import _categorize_cdf_assets
+from cognite.neat.core.extractors.cdfcore.models import RelationshipDefinition, RelationshipDefinitions
+from cognite.neat.core.extractors.cdfcore.rdf_to_assets import _categorize_cdf_assets
 from cognite.neat.core.loader.graph_store import NeatGraphStore
-from cognite.neat.core.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
+from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.core.utils.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
 
-# should be renamed to rdf2relationship_data_frame -> rdf2relationships
 
+def define_relationships(rules: TransformationRules, stop_on_exception: bool = False) -> RelationshipDefinitions:
+    relationships = {}
+
+    # Unique ids used to check for redefinitions of relationships
+    ids = set()
+
+    for row, rule in rules.properties.items():
+        if "Relationship" in rule.cdf_resource_type:
+            relationship = RelationshipDefinition(
+                source_class=rule.class_id,
+                target_class=rule.expected_value_type,
+                property_=rule.property_id,
+                labels=list(
+                    set([rule.label, rule.class_id, rule.expected_value_type, "non-historic", rule.property_id])
+                ),
+                target_type=rule.target_type,
+                source_type=rule.source_type,
+                relationship_external_id_rule=rule.relationship_external_id_rule,
+            )
+
+            id_ = f"{rule.class_id}({rule.property_id})"
+            if id_ in ids:
+                msg = f"Relationship {rule.property_id} redefined at {row} in transformation rules!"
+                if stop_on_exception:
+                    logging.error(msg)
+                    raise ValueError(msg)
+                else:
+                    msg += " Skipping redefinition!"
+                    warnings.warn(msg, stacklevel=2)
+                    logging.warning(msg)
+            else:
+                relationships[row] = relationship
+                ids.add(id_)
+
+    if relationships:
+        return RelationshipDefinitions(
+            data_set_id=rules.metadata.data_set_id,
+            prefix=rules.metadata.prefix,
+            namespace=rules.metadata.namespace,
+            relationships=relationships,
+        )
+
+    msg = "No relationship defined in transformation rule sheet!"
+    if stop_on_exception:
+        logging.error(msg)
+        raise ValueError(msg)
+    else:
+        warnings.warn(msg, stacklevel=2)
+        logging.warning(msg)
+        return RelationshipDefinitions(
+            data_set_id=rules.metadata.data_set_id,
+            prefix=rules.metadata.prefix,
+            namespace=rules.metadata.namespace,
+            relationships={},
+        )
 
+
+# should be renamed to rdf2relationship_data_frame -> rdf2relationships
 def rdf2relationships(
     graph_store: NeatGraphStore,
     transformation_rules: TransformationRules,
     stop_on_exception: bool = False,
 ) -> pd.DataFrame:
     """_summary_
 
@@ -34,15 +92,15 @@
     Returns
     -------
     Dict[str, Asset]
         _description_
     """
 
     # Step 1: Generate relationship definitions
-    relationship_definitions = transformation_rules.define_relationships(stop_on_exception)
+    relationship_definitions = define_relationships(transformation_rules, stop_on_exception)
 
     # Step 2: Generation relationships
 
     query_statement_template_by_reference = """
     SELECT ?source ?target
     WHERE {
         ?source a prefix:source_class .
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 
 from openpyxl import Workbook
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
 from openpyxl.utils.cell import get_column_letter
 from openpyxl.worksheet.datavalidation import DataValidation
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.extractors.rules_to_graphql import repair_name as to_graphql_name
+from cognite.neat.core.rules.models import TransformationRules
 
 
 def _add_index_identifiers(workbook: Workbook, sheet: str, no_rows: int):
     """Adds index-based auto identifier to a sheet identifier column"""
     for i in range(no_rows):
         prefix = to_graphql_name(sheet, "class", True)
         workbook[sheet][f"A{i+2}"] = f'=IF(ISBLANK(B{i+2}), "","{prefix}-{i+1}")'
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.16.0/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import warnings
 
 from graphql import GraphQLError, GraphQLField, GraphQLList, GraphQLNonNull, GraphQLObjectType, GraphQLSchema
 from graphql import assert_name as assert_graphql_name
 from graphql import print_schema
 
-from cognite.neat.core.data_classes.transformation_rules import DATA_TYPE_MAPPING, Property, TransformationRules
+from cognite.neat.core.rules.models import DATA_TYPE_MAPPING, Property, TransformationRules
 
 
 def get_invalid_names(entity_names: set) -> set:
     """Returns a set of invalid entity names"""
     invalid_names = set()
     for entity_name in entity_names:
         try:
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/loader/config.py` & `cognite_neat-0.16.0/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/loader/graph.py` & `cognite_neat-0.16.0/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.16.0/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.16.0/cognite/neat/core/loader/graph_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import pyoxigraph
 import requests
 from prometheus_client import Gauge, Summary
 from rdflib import Graph, Namespace
 from rdflib.plugins.stores.sparqlstore import SPARQLUpdateStore
 from rdflib.query import Result
 
-from cognite.neat.core.configuration import DEFAULT_NAMESPACE, PREFIXES
-from cognite.neat.core.data_classes.config import RdfStoreType
+from cognite.neat.core.configuration import DEFAULT_NAMESPACE, PREFIXES, RdfStoreType
 from cognite.neat.core.data_stores import oxrdflib
 from cognite.neat.core.loader.graph import rdf_file_to_graph
 
 prom_qsm = Summary("store_query_time_summary", "Time spent processing queries", ["query"])
 prom_sq = Gauge("store_single_query_time", "Time spent processing a single query", ["query"])
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.16.0/cognite/neat/core/mocks/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import warnings
 
 import pandas as pd
 from prometheus_client import Gauge
 from rdflib import RDF, Literal, Namespace, URIRef
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
-from cognite.neat.core.utils import get_generation_order, prettify_generation_order, remove_namespace
+from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.core.utils.utils import get_generation_order, prettify_generation_order, remove_namespace
 
 neat_total_processed_mock_triples = Gauge(
     "neat_total_processed_mock_triples", "Number of processed mock triples", ["state"]
 )
 neat_mock_triples_processing_timing = Gauge(
     "neat_mock_triples_processing_timing", "Generation of mock knowledge graph timing metrics", ["aggregation"]
 )
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/modeler.py` & `cognite_neat-0.16.0/cognite/neat/core/modeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Methods to transform Excel Sheet to Data Model
 """
 
 from rdflib import DCTERMS, OWL, RDFS, SKOS, XSD
 from rdflib.graph import RDF, BNode, Collection, Graph, Literal, Namespace, URIRef
 
 from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.data_classes.data_model_definitions import DataModelingDefinition
-from cognite.neat.core.data_classes.transformation_rules import Class
+from cognite.neat.core.rules.data_model_definitions import DataModelingDefinition
+from cognite.neat.core.rules.models import Class
 
 SHACL = Namespace("http://www.w3.org/ns/shacl#")
 
 
 def _wrangle_owl_properties(data_model_definition: DataModelingDefinition) -> dict[str, dict[str, set]]:
     """Wrangles the properties of the data model definition into a dictionary for easier conversion to RDF
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.16.0/cognite/neat/core/rules/_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
 
 import pandas as pd
+from rdflib import Namespace
 
-from cognite.neat.core.configuration import Tables
-from cognite.neat.core.data_classes import Instance, Metadata, Prefixes, TransformationRules
+from .models import URL, Instance, Metadata, Prefixes, TransformationRules
 
 
-def parse_transformation_rules(
-    raw_dfs: dict[str, pd.DataFrame], allow_validation_errors: bool = False
-) -> TransformationRules:
-    metadata = Metadata.create_from_dataframe(raw_dfs)
-    prefixes = Prefixes.create_from_dataframe(raw_dfs[Tables.prefixes])
-    instances = parse_instances(raw_dfs, metadata, prefixes) if Tables.instances in raw_dfs else None
+def from_tables(raw_dfs: dict[str, pd.DataFrame], allow_validation_errors: bool = False) -> TransformationRules:
+    expected_tables = Tables.as_set()
+    if missing_tables := (expected_tables - set(raw_dfs)):
+        raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
+
+    metadata = _parse_metadata(raw_dfs[Tables.metadata])
+    prefixes = _parse_prefix(raw_dfs[Tables.prefixes])
+
+    instances = _parse_instances(raw_dfs, metadata, prefixes) if Tables.instances in raw_dfs else None
 
     if not allow_validation_errors:
         return TransformationRules(
             prefixes=prefixes,
             metadata=metadata,
             classes={class_.get("Class"): class_ for class_ in raw_dfs[Tables.classes].to_dict(orient="records")},
             properties={
@@ -24,25 +27,55 @@
             },
             instances=instances,
         )
     else:
         raise NotImplementedError("Allowing validation errors is not yet implemented!")
 
 
-def parse_instances(raw_dfs: dict[str, pd.DataFrame], metadata: Metadata, prefixes: Prefixes) -> list[tuple]:
-    expected_tables = Tables.as_set()
-    if missing_tables := (expected_tables - set(raw_dfs)):
-        raise ValueError(f"Missing the following tables {', '.join(missing_tables)}")
-
+def _parse_instances(raw_dfs: dict[str, pd.DataFrame], metadata: Metadata, prefixes: Prefixes) -> list[tuple]:
     prefixes[metadata.prefix] = metadata.namespace
 
     instances = []
     for row_no, row in raw_dfs[Tables.instances].iterrows():
         try:
             triple = Instance(**row.to_dict(), namespace=metadata.namespace, prefixes=prefixes)
-            instances += [(triple.instance, triple.property_, triple.value)]
         except Exception:
             msg = f"Skipping row <{row_no + 3}> in Instance sheet\nReason: prefix in Property or Value column not defined!\n"
             print(msg)
             logging.info(msg)
+        else:
+            instances += [(triple.instance, triple.property_, triple.value)]
 
     return instances
+
+
+def _parse_metadata(meta_df: pd.DataFrame) -> Metadata:
+    return Metadata(
+        **dict(zip(meta_df[0], meta_df[1])),
+        source=meta_df.source if "source" in dir(meta_df) else None,
+    )
+
+
+def _parse_prefix(prefix_df: pd.DataFrame) -> dict[str, Namespace]:
+    prefixes = {}
+    for i, row in prefix_df.iterrows():
+        try:
+            url = URL(url=row["URI"]).url
+            prefixes[row["Prefix"]] = Namespace(url)
+        except ValueError as e:
+            msg = f"Prefix <{row['Prefix']}> has invalid URL: <{row['URI']}> fix this in Prefixes sheet at the row {i + 2} in the rule file!"
+            logging.error(msg)
+            raise ValueError(msg) from e
+
+    return prefixes
+
+
+class Tables:
+    prefixes = "Prefixes"
+    properties = "Properties"
+    classes = "Classes"
+    metadata = "Metadata"
+    instances = "Instances"
+
+    @classmethod
+    def as_set(cls) -> set[str]:
+        return {value for attr, value in cls.__dict__.items() if not attr.startswith("_") and attr != "as_set"}
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.16.0/cognite/neat/core/query_generator/sparql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
 from cognite.neat.core.configuration import PREFIXES
-from cognite.neat.core.data_classes.rules import (
+from cognite.neat.core.rules.to_rdf_path import (
     AllProperties,
     AllReferences,
     Hop,
     SingleProperty,
     Traversal,
     Triple,
     parse_traversal,
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/transformer.py` & `cognite_neat-0.16.0/cognite/neat/core/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import pandas as pd
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 from pydantic import BaseModel
 from rdflib import RDF, Graph
 from rdflib.term import Literal
 
-from cognite.neat.core.data_classes.rules import AllProperties, AllReferences, RawLookup, parse_rule
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.query_generator.sparql import build_sparql_query
-from cognite.neat.core.utils import remove_namespace
+from cognite.neat.core.rules.models import TransformationRules
+from cognite.neat.core.rules.to_rdf_path import AllProperties, AllReferences, RawLookup, parse_rule
+from cognite.neat.core.utils.utils import remove_namespace
 
 prom_total_proc_rules_g = Gauge("neat_total_processed_rules", "Number of processed rules", ["state"])
 rules_processing_timing_metric = Gauge(
     "neat_rules_processing_timing", "Transformation rules processing timing metrics", ["aggregation"]
 )
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/utils.py` & `cognite_neat-0.16.0/cognite/neat/core/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import pandas as pd
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import CredentialProvider, OAuthClientCredentials, OAuthInteractive
 from cognite.client.exceptions import CogniteDuplicatedError, CogniteReadTimeout
 from rdflib.term import URIRef
 
-from cognite.neat.core.data_classes.config import InteractiveClient, ServiceClient
 from cognite.neat.core.loader.graph_store import NeatGraphStore
+from cognite.neat.core.utils.cdf import InteractiveClient, ServiceClient
 
 
 def get_cognite_client_from_config(config: ServiceClient) -> CogniteClient:
     credentials = OAuthClientCredentials(
         token_url=config.token_url, client_id=config.client_id, client_secret=config.client_secret, scopes=config.scopes
     )
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/validator.py` & `cognite_neat-0.16.0/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/base.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from threading import Event
 
 import yaml
 from cognite.client import ClientConfig as CogniteClientConfig
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 
-from cognite.neat.core.data_classes.config import ClientConfig, Config
 from cognite.neat.core.data_stores.metrics import NeatMetricsCollector
-from cognite.neat.core.utils import retry_decorator
+from cognite.neat.core.utils.utils import retry_decorator
 from cognite.neat.core.workflow import cdf_store
 from cognite.neat.core.workflow.model import (
     FlowMessage,
     StepExecutionStatus,
     StepType,
     WorkflowConfigItem,
     WorkflowDefinition,
@@ -25,14 +24,16 @@
     WorkflowState,
     WorkflowStepDefinition,
     WorkflowStepEvent,
     WorkflowSystemComponent,
 )
 from cognite.neat.core.workflow.tasks import WorkflowTaskBuilder
 
+from ..configuration import Config
+from ..utils.cdf import ClientConfig
 from . import utils
 
 summary_metrics = Gauge("neat_workflow_summary_metrics", "Workflow execution summary metrics", ["wf_name", "name"])
 steps_metrics = Gauge("neat_workflow_steps_metrics", "Workflow step level metrics", ["wf_name", "step_name", "name"])
 timing_metrics = Gauge("neat_workflow_timing_metrics", "Workflow timing metrics", ["wf_name", "component", "name"])
```

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/model.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.16.0/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.16.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.16.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/default/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.core import loader, parser
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
-from cognite.neat.core.extractors.labels import upload_labels
-from cognite.neat.core.extractors.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
-from cognite.neat.core.extractors.rdf_to_relationships import (
+from cognite.neat.core import loader, rules
+from cognite.neat.core.extractors.cdfcore.labels import upload_labels
+from cognite.neat.core.extractors.cdfcore.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.core.extractors.cdfcore.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.core.loader.graph_store import NeatGraphStore, drop_graph_store
+from cognite.neat.core.rules.models import TransformationRules
 from cognite.neat.core.transformer import RuleProcessingReport, domain2app_knowledge_graph
 from cognite.neat.core.validator import validate_asset_hierarchy
 from cognite.neat.core.workflow import utils
 from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
 from cognite.neat.core.workflow.cdf_store import CdfStore
 
 with contextlib.suppress(ValueError):
@@ -58,16 +58,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
-        tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
-        self.transformation_rules = parser.parse_transformation_rules(tables)
+        self.transformation_rules = rules.load_rules_from_excel_file(rules_file_path)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules from {rules_file_path.name!r}.")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
```

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import time
 from pathlib import Path
 
 from cognite.client import CogniteClient
 
-from cognite.neat.core import extractors, loader, parser
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
+from cognite.neat.core import extractors, rules
 from cognite.neat.core.loader.graph_store import NeatGraphStore
+from cognite.neat.core.rules.models import TransformationRules
 from cognite.neat.core.workflow import utils
 from cognite.neat.core.workflow.base import BaseWorkflow
 from cognite.neat.core.workflow.cdf_store import CdfStore
 from cognite.neat.core.workflow.model import FlowMessage
 
 
 class FDMSchemaGenerationNeatWorkflow(BaseWorkflow):
@@ -45,16 +45,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
-        tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
-        self.transformation_rules = parser.parse_transformation_rules(tables)
+        self.transformation_rules = rules.load_rules_from_excel_file(rules_file_path)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_generate_fdm_schema(self, flow_msg: FlowMessage = None):
```

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import time
 from pathlib import Path
 
 import requests
 from cognite.client import CogniteClient
 
-from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.loader.graph_store import NeatGraphStore
+from cognite.neat.core.rules.models import TransformationRules
 from cognite.neat.core.workflow.base import BaseWorkflow, FlowMessage
 
 
 class GraphDbImportNeatWorkflow(BaseWorkflow):
     def __init__(self, name: str, client: CogniteClient):
         super().__init__(name, client, [])
         self.dataset_id: int = 0
```

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.16.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.16.0/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer/explorer.py` & `cognite_neat-0.16.0/cognite/neat/explorer/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 from prometheus_client import REGISTRY, Counter, make_asgi_app
 
 from cognite import neat
 from cognite.neat import constants
-from cognite.neat.core import loader, parser, query_generator
+from cognite.neat.core import query_generator
+from cognite.neat.core import rules as rules_module
 from cognite.neat.core.app import NeatApp
-from cognite.neat.core.data_classes.config import Config, configure_logging
+from cognite.neat.core.configuration import Config, configure_logging
 from cognite.neat.core.loader.config import copy_examples_to_directory
 from cognite.neat.core.workflow import WorkflowFullStateReport, utils
 from cognite.neat.core.workflow.base import WorkflowDefinition
 from cognite.neat.core.workflow.model import FlowMessage, WorkflowConfigItem
 from cognite.neat.explorer.data_classes.rest import (
     DownloadFromCdfRequest,
     NodesAndEdgesRequest,
@@ -157,20 +158,19 @@
         if hash != version:
             neat_app.cdf_store.load_rules_file_from_cdf(file_name, version)
             src = "cdf"
     else:
         neat_app.cdf_store.load_rules_file_from_cdf(file_name, version)
         src = "cdf"
 
-    tables = loader.rules.excel_file_to_table_by_name(path)
     error_text = ""
     properties = []
     classes = []
     try:
-        rules = parser.parse_transformation_rules(tables)
+        rules = rules_module.load_rules_from_excel_file(path)
         properties = [
             {
                 "class": value.class_id,
                 "property": value.property_id,
                 "property_description": value.description,
                 "property_type": value.expected_value_type,
                 "cdf_resource_type": value.cdf_resource_type,
```

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.16.0/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.16555d84.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.16.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.16.0/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.15.0/pyproject.toml` & `cognite_neat-0.16.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.15.0"
+version = "0.16.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
@@ -37,42 +37,48 @@
 neat = "cognite.neat.main:run"
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pandas = "*"
 rdflib = "*"
-openpyxl = "*"
 pydantic = "^2"
-gspread = "*"
-google-api-python-client = "*"
-google-auth-oauthlib = "*"
 PyYAML = "*"
 requests = "*"
 urllib3 = "^1.26"
+
 uvicorn = {extras = ["standard"], version = "^0.21.0"}
 prometheus-client = "^0.17.0"
 cognite-sdk = "^6"
 deepdiff = "*"
 fastapi = "^0.100"
 schedule = "^1"
 python-multipart = "^0.0.6"
 oxrdflib = {version = "^0.3.3", extras = ["oxigraph"]}
 graphql-core = "^3.2.3"
 
+openpyxl = {version="*", optional=true}
+
+gspread = {version="*", optional=true}
+google-api-python-client = {version="*", optional=true}
+google-auth-oauthlib = {version="*", optional=true}
+
 mkdocs =  {version="*", optional=true}
 mkdocs-jupyter = {version="*", optional=true}
 mkdocs-material-extensions = {version="*", optional=true}
 mkdocs-git-revision-date-localized-plugin = {version="*", optional=true}
 mkdocs-git-authors-plugin = {version="*", optional=true}
 mkdocs-gitbook = {version="*", optional=true}
 mkdocs-glightbox = {version="*", optional=true}
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin", "mkdocs-git-authors-plugin", "mkdocs-gitbook", "mkdocs-glightbox"]
+google = ["gspread", "google-api-python-client", "google-auth-oauthlib"]
+excel = ["openpyxl"]
+all = ["gspread", "google-api-python-client", "google-auth-oauthlib", "openpyxl"]
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 safety = "*"
```

### Comparing `cognite_neat-0.15.0/PKG-INFO` & `cognite_neat-0.16.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.15.0
+Version: 0.16.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Provides-Extra: docs
+Provides-Extra: excel
+Provides-Extra: google
 Requires-Dist: PyYAML
 Requires-Dist: cognite-sdk (>=6,<7)
 Requires-Dist: deepdiff
 Requires-Dist: fastapi (>=0.100,<0.101)
-Requires-Dist: google-api-python-client
-Requires-Dist: google-auth-oauthlib
+Requires-Dist: google-api-python-client ; extra == "google" or extra == "all"
+Requires-Dist: google-auth-oauthlib ; extra == "google" or extra == "all"
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
-Requires-Dist: gspread
+Requires-Dist: gspread ; extra == "google" or extra == "all"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
 Requires-Dist: mkdocs-gitbook ; extra == "docs"
 Requires-Dist: mkdocs-glightbox ; extra == "docs"
 Requires-Dist: mkdocs-jupyter ; extra == "docs"
 Requires-Dist: mkdocs-material-extensions ; extra == "docs"
-Requires-Dist: openpyxl
+Requires-Dist: openpyxl ; extra == "excel" or extra == "all"
 Requires-Dist: oxrdflib[oxigraph] (>=0.3.3,<0.4.0)
 Requires-Dist: pandas
 Requires-Dist: prometheus-client (>=0.17.0,<0.18.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: rdflib
 Requires-Dist: requests
```

